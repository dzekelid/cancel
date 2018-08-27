---
swagger: "2.0"
x-collection-name: Google Content API for Shopping
x-complete: 0
info:
  title: Google Content API for Shopping API Cancel Order Line Item
  description: Cancels a line item. This method can only be called for non-multi-client
    accounts.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /content/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{merchantId}/orders/{orderId}/cancel:
    post:
      summary: Cancel Order
      description: Cancels all line items in an order. This method can only be called
        for non-multi-client accounts.
      operationId: content.orders.cancel
      x-api-path-slug: merchantidordersorderidcancel-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order to cancel
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Order
  /{merchantId}/orders/{orderId}/cancelLineItem:
    post:
      summary: Cancel Order Line Item
      description: Cancels a line item. This method can only be called for non-multi-client
        accounts.
      operationId: content.orders.cancellineitem
      x-api-path-slug: merchantidordersorderidcancellineitem-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Order
      - Line
      - Item
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