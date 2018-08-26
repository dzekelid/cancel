---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/offchain/limit/cancel:
    post:
      summary: Add API Offchain Limit Cancel
      description: Add api offchain limit cancel.
      operationId: ApiOffchainLimitCancelPost
      x-api-path-slug: apioffchainlimitcancel-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Limit
      - Cancel
  /api/Operations/{id}/cancel:
    post:
      summary: Add API Operations  Cancel
      description: Add api operations  cancel.
      operationId: ApiOperationsByIdCancelPost
      x-api-path-slug: apioperationsidcancel-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Operations
      - ""
      - Cancel
  /api/Operations/cancel:
    post:
      summary: Add API Operations Cancel
      description: Add api operations cancel.
      operationId: ApiOperationsCancelPost
      x-api-path-slug: apioperationscancel-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Cancel
---