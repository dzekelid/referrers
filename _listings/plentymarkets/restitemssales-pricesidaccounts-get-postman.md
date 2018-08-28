{
  "info": {
    "name": "Plentymarkets List referrer accounts",
    "_postman_id": "0764113e-3930-48b1-9abe-5c3c6801488a",
    "description": "Lists all activated referrer accounts of a sales price.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Unique",
      "item": [
        {
          "id": "64f5dd7f-4c0f-4391-9ddc-3d1b09a42df0",
          "name": "getRestAccountingLocationsExistingAccounts",
          "request": {
            "url": "http://example.com/rest/accounting/locations/existing_accounts",
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
            "description": "Get all unique posting accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1872727-e5ab-489c-8150-3feb815ee0b5"
            }
          ]
        }
      ]
    },
    {
      "name": "Posting",
      "item": [
        {
          "id": "5e85a7cc-7b23-4dbe-9315-45fb826a83a2",
          "name": "getRestAccountingLocationsAddingAccounts",
          "request": {
            "url": "http://example.com/rest/accounting/locations/posting_accounts",
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
            "description": "Get all posting accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f1afb95-f765-47b0-838f-089758b74046"
            }
          ]
        },
        {
          "id": "fe48c668-31c1-40ba-9b26-f846850c991f",
          "name": "getRestAccountingLocationsLocationAddingAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/posting_accounts"
              ],
              "variable": [
                {
                  "id": "locationId",
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
            "description": "Get all posting accounts by locationid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d8a7fdc-2be0-405f-8918-94bc315d2de4"
            }
          ]
        },
        {
          "id": "b58b5a58-6cc0-4c4d-872d-01365c5b3038",
          "name": "getRestAccountingLocationsLocationTypeAddingAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/:type/posting_accounts"
              ],
              "variable": [
                {
                  "id": "locationId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "type",
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
            "description": "Get all posting accounts by locationid and type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16c0ad16-cb29-4e8a-8b8f-1c86bac521c7"
            }
          ]
        }
      ]
    },
    {
      "name": "Save",
      "item": [
        {
          "id": "4282b85b-5916-4fb7-bb10-bb0870f4190d",
          "name": "postRestAccountingLocationsAddingAccounts",
          "request": {
            "url": "http://example.com/rest/accounting/locations/posting_accounts",
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
            "description": "Save posting accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c3aef6f-d4d3-4c6d-92eb-da007fc801f2"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "ea29dbeb-b266-4a66-822e-da34f28c4a82",
          "name": "getRestAccountingLocationsLocationDebtorAccountsMode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/debtor_accounts/:mode"
              ],
              "variable": [
                {
                  "id": "locationId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "mode",
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
            "description": "Lists the debtor accounts of an accounting location by mode. The ID of the accounting location and the mode have to be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84072550-b5c0-4ef1-b890-c8e8ce50bfbb"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "3d4142fc-7484-439b-9486-851ef570236f",
          "name": "getRestAccounts",
          "request": {
            "url": "http://example.com/rest/accounts?createdAt=%7B%7D&updatedAt=%7B%7D",
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
            "description": "List accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96fc3895-24cd-468e-b516-f98dfe449820"
            }
          ]
        },
        {
          "id": "8b05403b-8f2b-4b46-95a9-8350b6f70319",
          "name": "getRestAccountsContactsContactBanks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/contacts/:contactId/banks"
              ],
              "variable": [
                {
                  "id": "contactId",
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
            "description": "Lists bank accounts of the contact. The ID of the contact must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e60f323-2816-4107-ae20-6f9bbe028090"
            }
          ]
        },
        {
          "id": "82dcf377-7805-4ca9-8a0c-40ed211849f2",
          "name": "getRestItemsSalesPricesAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/accounts"
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
            "description": "Lists all activated referrer accounts of a sales price."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6eb517aa-6a30-4685-bb54-c41ebc50be76"
            }
          ]
        }
      ]
    }
  ]
}