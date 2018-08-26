---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 1
info:
  title: Bitly User Metrics API
  description: the-bitly-user-metrics-api
  termsOfService: http://dev.bitly.com/best_practices.html
  version: v3
host: api-ssl.bitly.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/user/referrers:
    get:
      summary: User Referrers
      description: Returns aggregate metrics about the pages referring click traffic
        to all of the authenticated users Bitlinks.
      operationId: userReferrers
      x-api-path-slug: v3userreferrers-get
      parameters:
      - in: query
        name: limit
        description: 1 to 1000 (default=100)
      - in: query
        name: rollup
        description: Return data for multiple units rolled up to a single result instead
          of a separate value for each period of time
      - in: query
        name: timezone
        description: 'an integer hour offset from UTC (-14 to 14), or a timezone string
          default: America/New_York'
      - in: query
        name: unit
        description: 'minute, hour, day, week or month, default: day'
      - in: query
        name: units
        description: an integer representing the time units to query data for
      - in: query
        name: unit_reference_ts
        description: 'an epoch timestamp, indicating the most recent time for which
          to pull metrics, default: now'
      responses:
        200:
          description: OK
      tags:
      - User
      - Referrers
  /v3/user/referring_domains:
    get:
      summary: User Referring Domains
      description: eturns aggregate metrics about the domains referring click traffic
        to all of the authenticated users Bitlinks. If the user is a master account,
        or is a subaccount with full_reports permission, the user may choose to view
        the metrics of any account belonging to the master account.
      operationId: userReferringDomains
      x-api-path-slug: v3userreferring-domains-get
      parameters:
      - in: query
        name: exclude_social_networks
        description: If true, exclude domains that are part of a social network that
          bitly tracks (default=true)
      - in: query
        name: limit
        description: 1 to 1000 (default=100)
      - in: query
        name: login
        description: an optional string consisting of the account name used to report
          the appropriate statistics; defaults to the current user
      - in: query
        name: rollup
        description: Return data for multiple units rolled up to a single result instead
          of a separate value for each period of time
      - in: query
        name: timezone
        description: 'an integer hour offset from UTC (-14 to 14), or a timezone string
          default: America/New_York'
      - in: query
        name: unit
        description: 'minute, hour, day, week or month, default: day'
      - in: query
        name: units
        description: an integer representing the time units to query data for
      - in: query
        name: unit_reference_ts
        description: 'an epoch timestamp, indicating the most recent time for which
          to pull metrics, default: now'
      responses:
        200:
          description: OK
      tags:
      - User
      - Referring
      - Domains
---