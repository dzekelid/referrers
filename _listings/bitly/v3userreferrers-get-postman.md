{
  "info": {
    "name": "Bitly User Metrics API User Referrers",
    "_postman_id": "d59586d0-a519-46c7-8c5a-a0adb13259d3",
    "description": "Returns aggregate metrics about the pages referring click traffic to all of the authenticated users Bitlinks.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "82922105-0c81-4664-8ca9-5ec8b5a00e7e",
          "name": "userClicks",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/clicks?format=%7B%7D&limit=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the aggregate number of clicks on all of the authenticated users Bitlinks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f02d24a-1a55-4fdf-97c5-f80828c2d9ad"
            }
          ]
        },
        {
          "id": "9db9fb01-b1a6-4839-a419-2be43465b948",
          "name": "userCountries",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/countries?limit=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns aggregate metrics about the countries referring click traffic to all of the authenticated users Bitlinks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b39a661-7fb1-482e-a037-253b431fe06f"
            }
          ]
        },
        {
          "id": "75d0bf07-42f5-42a3-b261-37be0592a24a",
          "name": "userPopularEarnedbyClicks",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/popular_earned_by_clicks?domain=%7B%7D&limit=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the top links to your tracking domain (or domains) created by users not associated with your account, ordered by clicks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66776200-5159-48e2-8cfc-091b67d8897c"
            }
          ]
        },
        {
          "id": "ad272573-95fb-453d-b973-34a17a37d6d5",
          "name": "userPopularEarnedByShortens",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/popular_earned_by_shortens?domain=%7B%7D&limit=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the top links to your tracking domain (or domains) created by users not associated with your account, ordered by shortens."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6576ecc-0885-4c55-8f65-0500573a5271"
            }
          ]
        },
        {
          "id": "b037ad9f-d343-4690-8dcf-6e8b06f04cef",
          "name": "userPopularLinks",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/popular_links?limit=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the authenticated users most-clicked Bitlinks (ordered by number of clicks) in a given time period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60fb3a3f-a0b8-44f3-9de9-1b98db34f9ea"
            }
          ]
        },
        {
          "id": "c2b9f3c1-f559-4a6d-b545-90ccbfdd0970",
          "name": "userPopularOwnedByClicks",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/popular_owned_by_clicks?domain=%7B%7D&limit=%7B%7D&subaccount=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the top links to your tracking domain (or domains) created by you or your subaccounts ordered by clicks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a0561bb-ac3f-4795-a060-69fc4581c8d0"
            }
          ]
        },
        {
          "id": "4213366a-de11-4f90-b9d5-151b52a711af",
          "name": "userPopularOwnedByShortens",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/popular_owned_by_shortens?domain=%7B%7D&limit=%7B%7D&subaccount=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the top links to your tracking domain (or domains) created by you or your subaccounts ordered by number of shortens."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9ef5d64-ea52-4b0e-98a7-252881363dbd"
            }
          ]
        },
        {
          "id": "31c47cf3-0186-49b3-9b33-a32bde64c3a0",
          "name": "userReferrers",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/referrers?limit=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns aggregate metrics about the pages referring click traffic to all of the authenticated users Bitlinks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bc35288-b514-471e-9119-149b56cdaf7b"
            }
          ]
        }
      ]
    }
  ]
}