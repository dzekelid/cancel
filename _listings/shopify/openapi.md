swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/orders/4528049998/fulfillments/3770145678/cancel.json:
    post:
      summary: Cancel a fulfillment.
      description: Cancel a fulfillment..
      operationId: postAdminOrders4528049998Fulfillments3770145678Cancel.json
      x-api-path-slug: adminorders4528049998fulfillments3770145678cancel-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Cancel
      - Fulfillment
  /admin/orders/4554953422/cancel.json:
    post:
      summary: Canceling an Order
      description: Canceling an order.
      operationId: postAdminOrders4554953422Cancel.json
      x-api-path-slug: adminorders4554953422cancel-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Canceling
      - Order