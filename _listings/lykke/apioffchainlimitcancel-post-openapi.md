---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Add API Offchain Limit Cancel
  version: 1.0.0
  description: Add api offchain limit cancel.
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