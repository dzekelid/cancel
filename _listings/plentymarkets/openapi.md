swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
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