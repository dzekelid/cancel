---
swagger: "2.0"
x-collection-name: HitBTC
x-complete: 0
info:
  title: HitBTC Cancel Replace Order
  description: Cancel replace order.
  version: 1.0.0
basePath: /api/2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /order:
    delete:
      summary: Cancel All Open Orders
      description: Cancel all open orders.
      operationId: deleteOrder
      x-api-path-slug: order-delete
      parameters:
      - in: formData
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - ""
      - Open
      - Orders
  /order/{clientOrderId}:
    delete:
      summary: Cancel Order
      description: Cancel order.
      operationId: deleteOrderClientorder
      x-api-path-slug: orderclientorderid-delete
      parameters:
      - in: path
        name: clientOrderId
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Order
    patch:
      summary: Cancel Replace Order
      description: Cancel replace order.
      operationId: patchOrderClientorder
      x-api-path-slug: orderclientorderid-patch
      parameters:
      - in: path
        name: clientOrderId
      - in: formData
        name: price
      - in: formData
        name: quantity
      - in: formData
        name: requestClientId
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Replace
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