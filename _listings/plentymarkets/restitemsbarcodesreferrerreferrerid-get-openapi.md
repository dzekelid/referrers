---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List barcodes by referrer
  description: Lists barcodes linked to the specified referrer. The ID of the referrer
    must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/sales_prices/{id}/referrers:
    get:
      summary: List activated referrers
      description: Lists all activated referrers for a sales price. The ID of the
        sales price must be specified.
      operationId: getRestItemsSalesPricesReferrers
      x-api-path-slug: restitemssales-pricesidreferrers-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Activated
      - Referrers
    post:
      summary: Activate a referrer
      description: Activates a referrer for a sales price. The ID of the sales price
        must be specified.
      operationId: postRestItemsSalesPricesReferrers
      x-api-path-slug: restitemssales-pricesidreferrers-post
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/referrers
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Referrer
  /rest/orders/referrers:
    get:
      summary: List referrers
      description: Lists referrers with the desired columns/attributes.
      operationId: getRestOrdersReferrers
      x-api-path-slug: restordersreferrers-get
      parameters:
      - in: query
        name: columns
        description: The desired columns/attributes of the order referrer to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Referrers
  /rest/items/barcodes/referrer/{referrerId}:
    get:
      summary: List barcodes by referrer
      description: Lists barcodes linked to the specified referrer. The ID of the
        referrer must be specified.
      operationId: getRestItemsBarcodesReferrerReferrer
      x-api-path-slug: restitemsbarcodesreferrerreferrerid-get
      parameters:
      - in: path
        name: referrerId
      responses:
        200:
          description: OK
      tags:
      - List
      - Barcodes
      - By
      - Referrer
  /rest/items/barcodes/{barcodeId}/referrer:
    post:
      summary: Activate a referrer
      description: Activate a referrer for a barcode.
      operationId: postRestItemsBarcodesBarcodeReferrer
      x-api-path-slug: restitemsbarcodesbarcodeidreferrer-post
      parameters:
      - in: path
        name: barcodeId
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Referrer
  /rest/items/barcodes/{barcodeId}/referrer/{referrerId}:
    delete:
      summary: Deactivate a referrer
      description: Deactivate a referrer for a barcode. The ID of the barcode and
        the ID of the referrer must be specified.
      operationId: deleteRestItemsBarcodesBarcodeReferrerReferrer
      x-api-path-slug: restitemsbarcodesbarcodeidreferrerreferrerid-delete
      parameters:
      - in: path
        name: barcodeId
      - in: path
        name: referrerId
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Referrer
  /rest/items/sales_prices/{id}/accounts:
    get:
      summary: List referrer accounts
      description: Lists all activated referrer accounts of a sales price.
      operationId: getRestItemsSalesPricesAccounts
      x-api-path-slug: restitemssales-pricesidaccounts-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Referrer
      - Accounts
    post:
      summary: Activate a referrer account
      description: Activates a referrer account for a sales price.
      operationId: postRestItemsSalesPricesAccounts
      x-api-path-slug: restitemssales-pricesidaccounts-post
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/accounts
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Referrer
      - Account
  /rest/items/sales_prices/{id}/accounts/{accountType}/{accountId}:
    delete:
      summary: Deactivate a referrer account
      description: Deactivates a referrer account for a sales price.
      operationId: deleteRestItemsSalesPricesAccountsAccounttypeAccount
      x-api-path-slug: restitemssales-pricesidaccountsaccounttypeaccountid-delete
      parameters:
      - in: path
        name: accountId
      - in: path
        name: accountType
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Referrer
      - Account
  /rest/items/sales_prices/{id}/referrers/{referrerId}:
    delete:
      summary: Deactivates a referrer
      description: Deactivates a referrer for a sales price. The ID of the sales price
        and the ID of the referrer must be specified.
      operationId: deleteRestItemsSalesPricesReferrersReferrer
      x-api-path-slug: restitemssales-pricesidreferrersreferrerid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: referrerId
      responses:
        200:
          description: OK
      tags:
      - Deactivates
      - Referrer
  /rest/orders/referrers/{parentReferrerId?}:
    post:
      summary: Create an order referrer
      description: |-
        Create an order referrer. The ID can be specified, a parent ID can be specified to create a sub referrer or if no ID is specified, a referrer ID will be assigned automatically.
        If an ID is specified, the ID may not be used already. If the ID is used already, the referrer will only be created.
        If the ID is automatically assigned, the first ID that has not been used before will be set.
        If the ID is not specified, but a parent referrer ID is given, then the new referrer ID will be a sub referrer of the given parent.
      operationId: postRestOrdersReferrersParentreferrer
      x-api-path-slug: restordersreferrersparentreferrerid-post
      parameters:
      - in: query
        name: data
        description: The attributes of the order referrer to be created
      - in: path
        name: parentReferrerId?
      responses:
        200:
          description: OK
      tags:
      - Order
      - Referrer
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