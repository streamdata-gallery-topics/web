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
  /admin/webhooks/503738446.json:
    put:
      summary: Update a Webhook
      description: Update a webhook.
      operationId: putAdminWebhooks503738446.json
      x-api-path-slug: adminwebhooks503738446-json-put
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
      - Webhook
    delete:
      summary: Delete a Webhook
      description: Delete a webhook.
      operationId: deleteAdminWebhooks503738446.json
      x-api-path-slug: adminwebhooks503738446-json-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Webhook
---