---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Cancel an order
  description: Cancels an order. The ID of the order must be specified.
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
  /rest/orders/{orderId}/cancel:
    put:
      summary: Cancel an order
      description: Cancels an order. The ID of the order must be specified.
      operationId: putRestOrdersOrderCancel
      x-api-path-slug: restordersorderidcancel-put
      parameters:
      - in: body
        name: /rest/orders/{orderId}/cancel
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Order
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