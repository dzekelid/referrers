{
  "info": {
    "name": "Plentymarkets List activated referrers",
    "_postman_id": "555ab5ee-c4a2-4e94-a60e-0a70d02ab533",
    "description": "Lists all activated referrers for a sales price. The ID of the sales price must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "28416e6c-8134-475e-a44e-df77a13befd3",
          "name": "getRestItemsSalesPricesReferrers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/referrers"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists all activated referrers for a sales price. The ID of the sales price must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "900aa740-c54a-4787-a864-39843a5ccdc4"
            }
          ]
        }
      ]
    }
  ]
}