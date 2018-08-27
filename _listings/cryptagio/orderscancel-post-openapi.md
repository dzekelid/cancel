---
swagger: "2.0"
x-collection-name: Cryptagio
x-complete: 0
info:
  title: Cryptagio Post Orders Cancel
  description: Accepts JSON object. Cancels all orders if no parameters are passed.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders/cancel:
    post:
      summary: Post Orders Cancel
      description: Accepts JSON object. Cancels all orders if no parameters are passed.
      operationId: postOrdersCancel
      x-api-path-slug: orderscancel-post
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Orders
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