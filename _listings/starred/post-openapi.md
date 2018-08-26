---
swagger: "2.0"
x-collection-name: Starred
x-complete: 0
info:
  title: Starred Webhook v1.0
  description: |-
    Webhook v1.0 is our standard webhook response. This version will be deprecated soon. We highly recommend migrating to Webhook v1.1

    Please get in touch with our support to migrate your account to Webhook v1.1
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
  /:
    post:
      summary: Webhook v1.0
      description: |-
        Webhook v1.0 is our standard webhook response. This version will be deprecated soon. We highly recommend migrating to Webhook v1.1

        Please get in touch with our support to migrate your account to Webhook v1.1
      operationId: UnnammedEndpointPost2
      x-api-path-slug: post
      responses:
        200:
          description: OK
      tags:
      - Webhook
      - V1
      - "0"
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