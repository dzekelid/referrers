{
  "info": {
    "name": "PagerDuty REST API Reference",
    "_postman_id": "7a4a3d0e-f9d0-45ca-9781-f3fe2db0118f",
    "description": "REST API Reference.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Folder",
      "item": [
        {
          "id": "0abe4061-85b8-4585-aa60-5fc2d51ca975",
          "name": "list-people-and-integrations-associated-with-a-given-team",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "teams/:teamId/people"
              ],
              "variable": [
                {
                  "id": "teamId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List people and integrations associated with a given team."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7dc45df-3c35-4bd9-9480-ec7b2e27d5fc"
            }
          ]
        }
      ]
    },
    {
      "name": "APIs",
      "item": [
        {
          "id": "9a028c16-17b9-43a8-8b8b-9a1c16d910b5",
          "name": "rest-api-reference",
          "request": {
            "url": "http://example.com/api/api_reference",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "REST API Reference."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5672b7d9-6db4-4859-a0b7-3878e6042026"
            }
          ]
        }
      ]
    }
  ]
}