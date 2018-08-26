{
  "info": {
    "name": "Plentymarkets Deactivate a referrer",
    "_postman_id": "4a4ae1d4-fee1-4a23-9c94-b161cc5656cc",
    "description": "Deactivate a referrer for a barcode. The ID of the barcode and the ID of the referrer must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Deactivate",
      "item": [
        {
          "id": "8a3c296b-03fa-4d06-968e-2da224f9137b",
          "name": "deleteRestCategoriesClients",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/categories/:id/clients"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Deactivate availability for clients."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b84a963-fdab-4957-b587-8281784d2e10"
            }
          ]
        },
        {
          "id": "e6453777-332d-4766-91ef-75c28b02fa7a",
          "name": "deleteRestItemsBarcodesBarcodeReferrerReferrer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/barcodes/:barcodeId/referrer/:referrerId"
              ],
              "variable": [
                {
                  "id": "barcodeId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "referrerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Deactivate a referrer for a barcode. The ID of the barcode and the ID of the referrer must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4018dbc4-7f4d-42de-b056-6609d30078c5"
            }
          ]
        }
      ]
    }
  ]
}