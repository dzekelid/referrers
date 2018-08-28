{
  "info": {
    "name": "Bitly Domains API Get Link Referrers",
    "_postman_id": "9ebdcf2b-c18a-4100-9932-b4946e2e5738",
    "description": "Returns metrics about the pages referring click traffic to a single bitly link.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Shorten",
      "item": [
        {
          "id": "5b524c1f-de25-4cf0-a28b-ee2b8df3ed4f",
          "name": "Get_shorten_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/shorten?domain=%7B%7D&format=%7B%7D&longUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a long URL, returns a bitly short URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c5dd243-2a55-47cf-a153-f44319d7569b"
            }
          ]
        }
      ]
    },
    {
      "name": "Expand",
      "item": [
        {
          "id": "ccb441fe-9f5d-4f2b-8a39-ad2fa22cfbb2",
          "name": "Get_expand_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/expand?format=%7B%7D&hash=%7B%7D&shortUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a bitly URL or hash (or multiple), returns the target (long) URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0ee82b2-4de7-483d-80a3-a6c6bf3bdce2"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "539b2c18-b1f8-45e5-badd-1c203de1592d",
          "name": "Get_lookup_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/lookup?format=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This is used to query for a bitly link based on a long URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "464e7721-0055-4b7f-b4bf-42e1f1d964b9"
            }
          ]
        },
        {
          "id": "7904e6ff-f38c-4635-892e-93657af17dfc",
          "name": "Get_link_clicks_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/clicks?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns entries from a user's link history in reverse chronological order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "323660ee-097a-421f-9166-eb223ed55f25"
            }
          ]
        },
        {
          "id": "c20d1318-ba23-4919-95e3-abbff26ae5fe",
          "name": "Get_link_countries_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/countries?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metrics about the countries referring click traffic to a single bitly link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ffc077a9-daa4-4163-9372-f0180501585a"
            }
          ]
        },
        {
          "id": "154633ac-e226-4148-bd90-9bc84e032ada",
          "name": "Get_link_referrers_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/referrers?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metrics about the pages referring click traffic to a single bitly link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c112c8ed-eed2-4e03-b16c-b70caf4c32f3"
            }
          ]
        }
      ]
    },
    {
      "name": "Info",
      "item": [
        {
          "id": "18ec83b0-8c61-46ca-b796-9ebd3006f19f",
          "name": "Get_info_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/info?format=%7B%7D&hash=%7B%7D&shortUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This is used to return the page title for a given bitly link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72c4b263-624a-4315-aa5c-6cc29d2725b8"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "c3ef2880-1cec-4e13-9ada-9e18bc36e020",
          "name": "Get_user_info_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/user/info?format=%7B%7D&login=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return information about a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a3e21b2-875d-4475-9bdc-91ea85c0ffd5"
            }
          ]
        },
        {
          "id": "32bcc334-971a-41f0-b463-b31abbf9728f",
          "name": "Get_user_link_history_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/user/link_history?created_after=%7B%7D&created_before=%7B%7D&format=%7B%7D&limit=%7B%7D&user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns entries from a user's link history in reverse chronological order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8ad5cdc-b89f-47a2-a53b-94b097e0ae71"
            }
          ]
        },
        {
          "id": "ca4761a8-a077-448c-9110-37a4d80f73f1",
          "name": "Get_user_popular_links_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/user/popular_links?format=%7B%7D&limit=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the authenticated user's most-clicked bitly links (ordered by number of clicks) in a given time period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb8c3ae0-bc9a-4375-b216-aab5586385ea"
            }
          ]
        }
      ]
    }
  ]
}