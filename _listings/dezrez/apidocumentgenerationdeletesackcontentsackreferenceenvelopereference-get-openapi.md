---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: "Dezrez deletes an envelope from the the content of a sack \r\nDeprecated
    in favour of the DELETE verb"
  version: 1.0.0
  description: "Deletes an envelope from the the content of a sack \r\ndeprecated
    in favour of the delete verb."
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Peppermint:
    post:
      summary: Submits a referral to dezrez legal
      description: Submits a referral to dezrez legal.
      operationId: Peppermint_SubmitReferralByreferralDataContract
      x-api-path-slug: apipeppermint-post
      parameters:
      - in: body
        name: referralDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Submits
      - Referral
      - To
      - Dezrez
      - Legal
  /api/role/createreferralevent:
    post:
      summary: Creates a referral event on the role
      description: Creates a referral event on the role.
      operationId: Role_CreateReferralEventByreferralData
      x-api-path-slug: apirolecreatereferralevent-post
      parameters:
      - in: body
        name: referralData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Referral
      - Event
      - "On"
      - Role
  /api/coreplatformstate/{stateItemReference}:
    delete:
      summary: Clears a state item.
      description: Clears a state item..
      operationId: CorePlatformState_ClearStateItemBystateItemReference
      x-api-path-slug: apicoreplatformstatestateitemreference-delete
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: stateItemReference
        description: The state item reference
      responses:
        200:
          description: OK
      tags:
      - Clears
      - State
      - Item
  /api/documentgeneration/deletesackcontent/{sackReference}/{envelopereference}:
    get:
      summary: "deletes an envelope from the the content of a sack \r\nDeprecated
        in favour of the DELETE verb"
      description: "Deletes an envelope from the the content of a sack \r\ndeprecated
        in favour of the delete verb."
      operationId: DocumentGeneration_DeleteSackContentDeprecatedBysackReferenceByenvelopereference
      x-api-path-slug: apidocumentgenerationdeletesackcontentsackreferenceenvelopereference-get
      parameters:
      - in: path
        name: envelopereference
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Deletes
      - Envelope
      - From
      - The
      - Content
      - Of
      - Sack
      - Deprecated
      - In
      - Favour
      - Of
      - DELETE
      - Verb
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