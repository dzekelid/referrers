{
  "info": {
    "name": "Bitly User Metrics API User Referring Domains",
    "_postman_id": "a531e512-b65f-41c5-9b97-c5e1f4160aad",
    "description": "eturns aggregate metrics about the domains referring click traffic to all of the authenticated users Bitlinks. If the user is a master account, or is a subaccount with full_reports permission, the user may choose to view the metrics of any account belonging to the master account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "574358c7-7177-4d9c-aac3-40faa639b886",
          "name": "userReferringDomains",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/referring_domains?exclude_social_networks=%7B%7D&limit=%7B%7D&login=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "eturns aggregate metrics about the domains referring click traffic to all of the authenticated users Bitlinks. If the user is a master account, or is a subaccount with full_reports permission, the user may choose to view the metrics of any account belonging to the master account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d862e4fc-caf5-4ed3-93b9-14ca66254e73"
            }
          ]
        }
      ]
    }
  ]
}