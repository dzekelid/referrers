{
  "info": {
    "name": "Plentymarkets Activate a referrer",
    "_postman_id": "c8351be3-a8de-46e4-aaba-a72b0cc935f0",
    "description": "Activate a referrer for a barcode.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "bffb20af-93b0-45ba-b95a-3918ee229f83",
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
              "id": "7110ba5e-3b9b-40be-a52d-abbacc5d97e0"
            }
          ]
        },
        {
          "id": "46ed5136-be46-4ce5-b885-eca39b8a148a",
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
              "id": "27d94609-b805-46d0-a876-bf91a7f3030f"
            }
          ]
        },
        {
          "id": "5c0a90b6-b80f-4d99-b785-d83a7583eee7",
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
              "id": "cb1975ee-2dcc-4f6a-bd0a-7e39396e1725"
            }
          ]
        }
      ]
    },
    {
      "name": "Activate",
      "item": [
        {
          "id": "f3cf5197-97b6-45e6-b6f2-ad691799875d",
          "name": "postRestItemsBarcodesBarcodeReferrer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/barcodes/:barcodeId/referrer"
              ],
              "variable": [
                {
                  "id": "barcodeId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
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
            "description": "Activate a referrer for a barcode."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da7c5f0b-ccbe-4968-8ea2-4c371077f7d2"
            }
          ]
        }
      ]
    }
  ]
}