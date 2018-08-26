{
  "info": {
    "name": "Plentymarkets List referrers",
    "_postman_id": "606f48c9-c224-418e-a61f-7cf76f8351b9",
    "description": "Lists referrers with the desired columns/attributes.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "2a45b240-6021-4077-9415-4c64a7fabdac",
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
              "id": "25edc762-05ae-4922-a0f6-b8230f083832"
            }
          ]
        },
        {
          "id": "f8472a70-3de5-489c-8eda-7466121090b3",
          "name": "getRestOrdersReferrers",
          "request": {
            "url": "http://example.com/rest/orders/referrers?columns=%7B%7D",
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
            "description": "Lists referrers with the desired columns/attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "520c3f2e-8f04-4f31-9384-93e75231b71b"
            }
          ]
        }
      ]
    }
  ]
}