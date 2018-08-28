{
  "info": {
    "name": "Dezrez Clears a state item.",
    "_postman_id": "8cb6b0f7-4938-4de8-846d-da7118265924",
    "description": "Clears a state item..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Clears",
      "item": [
        {
          "id": "394c42ea-4bd0-4936-800b-e4dc0bd94f16",
          "name": "CorePlatformState_ClearStateItemBystateItemReference",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/coreplatformstate/:stateItemReference"
              ],
              "variable": [
                {
                  "id": "stateItemReference",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Clears a state item.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e818ecad-3bfd-49cc-9595-f2a54201982f"
            }
          ]
        }
      ]
    }
  ]
}