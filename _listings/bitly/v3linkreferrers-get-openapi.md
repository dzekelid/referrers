---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly Domains API Get Link Referrers
  description: Returns metrics about the pages referring click traffic to a single
    bitly link.
  version: 1.0.0
host: api-ssl.bitly.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/link/referrers:
    get:
      summary: Get Link Referrers
      description: Returns metrics about the pages referring click traffic to a single
        bitly link.
      operationId: Get_link_referrers_
      x-api-path-slug: v3linkreferrers-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: limit
        description: (optional) 1 to 1000 (default=100)
      - in: query
        name: link
        description: a bltly link
      - in: query
        name: rollup
        description: (optional) true or false
      - in: query
        name: timezone
        description: (optional) an integer hour offset from UTC (-14 to 14)
      - in: query
        name: unit
        description: minute, hour, day, week or month
      - in: query
        name: units
        description: an integer representing the time units to query data for
      responses:
        200:
          description: OK
      tags:
      - Link
      - Referrers
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---