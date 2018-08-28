{
  "info": {
    "name": "Plentymarkets List barcodes by referrer",
    "_postman_id": "5989c27b-4cf8-4031-ae5c-406d06bed6fe",
    "description": "Lists barcodes linked to the specified referrer. The ID of the referrer must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "fca52596-6320-45aa-ae8b-56f740f7cbea",
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
              "id": "fe8595d6-8ada-4f4b-9ac3-8cb66077b1f1"
            }
          ]
        },
        {
          "id": "f97a9a6d-43c4-4301-8231-2882a93ddc6d",
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
              "id": "ff0ec001-cf9a-48fa-918a-f2f367d53780"
            }
          ]
        },
        {
          "id": "18d58f60-e6ae-4051-929b-860a9eec3cdc",
          "name": "getRestItemsBarcodesReferrerReferrer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/barcodes/referrer/:referrerId"
              ],
              "variable": [
                {
                  "id": "referrerId",
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
            "description": "Lists barcodes linked to the specified referrer. The ID of the referrer must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9423188b-d064-4ded-8172-8c40c6b5da0f"
            }
          ]
        }
      ]
    }
  ]
}