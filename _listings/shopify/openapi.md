---
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
  /admin/orders/4554953422/close.json:
    post:
      summary: Close a processed order
      description: Close a processed order.
      operationId: postAdminOrders4554953422Close.json
      x-api-path-slug: adminorders4554953422close-json-post
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
      - Close
      - Processed
      - Order
  /admin/orders/4554953422/open.json:
    post:
      summary: Re-opening a closed Order
      description: Re-opening a closed order.
      operationId: postAdminOrders4554953422Open.json
      x-api-path-slug: adminorders4554953422open-json-post
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
      - Re-opening
      - Closed
      - Order
---