{
  "info": {
    "name": "Bitly Link Metrics API Link Referrers",
    "_postman_id": "e403deb6-42e0-4a62-89f1-353366c9b11e",
    "description": "Returns metrics about the pages referring click traffic to a single Bitlink.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Link",
      "item": [
        {
          "id": "f8f62459-0453-4574-b148-d407ce155d5c",
          "name": "linkClicks",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/clicks?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the number of clicks on a single Bitlink."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "439b05fc-74fa-44d1-8aff-1e7307f4b6eb"
            }
          ]
        },
        {
          "id": "a5f4eef5-1276-4d17-82f3-dc718c3c8da9",
          "name": "linkClicksbyCountry",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/countries?link=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metrics about the countries referring click traffic to a single Bitlink."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "226b17b2-0bdc-4807-bb04-de2a731f52b7"
            }
          ]
        },
        {
          "id": "7969e6d9-6589-4c5b-95e7-894402ef18c0",
          "name": "userWhoEncodedLink",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/encoders?expand_user=%7B%7D&limit=%7B%7D&link=%7B%7D&my_network=%7B%7D&subaccounts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns users who have encoded this long URL (optionally only those in the requesting users social graph)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9dd4afbd-4786-441d-a565-a7a5bad73025"
            }
          ]
        },
        {
          "id": "2fb30370-b211-4cc0-aaae-f445df0c47a4",
          "name": "usersWhoEncodedLink",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/encoders_by_count?expand_user=%7B%7D&limit=%7B%7D&link=%7B%7D&my_network=%7B%7D&subaccounts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns users who have encoded this link (optionally only those in the requesting users social graph), sorted by the number of clicks on each encoding users link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30649f4d-b37a-44e0-951d-89f1fe893116"
            }
          ]
        },
        {
          "id": "ceb8415d-2591-4635-9586-1b475528310a",
          "name": "numberOfEncoders",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/encoders_count?link=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the number of users who have shortened (encoded) a single Bitlink."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af30296c-25c6-4af9-a1cb-f35f19675711"
            }
          ]
        },
        {
          "id": "3cc4617d-cfe1-4aff-b565-717b48543708",
          "name": "linkReferrers",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/referrers?link=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metrics about the pages referring click traffic to a single Bitlink."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4f01764-c691-4259-a5b6-a77ff2984d57"
            }
          ]
        }
      ]
    }
  ]
}