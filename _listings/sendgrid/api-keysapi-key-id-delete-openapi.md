---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Delete Api Keys Api Key
  description: |-
    **This endpoint allows you to revoke an existing API Key**

    Authentications using this API Key will fail after this request is made, with some small propogation delay.If the API Key ID does not exist an HTTP 404 will be returned.

    The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

    ## URI Parameters

    | URI Parameter   | Type  | Required?  | Description  |
    |---|---|---|---|
    |api_key_id |string | required | The ID of the API Key you are deleting.|
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api_keys:
    get:
      summary: Get Api Keys
      description: |-
        **This endpoint allows you to retrieve all API Keys that belong to the authenticated user.**

        The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).
      operationId: GET_api_keys
      x-api-path-slug: api-keys-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Api
      - Keys
    post:
      summary: Add Api Keys
      description: |-
        **This endpoint allows you to create a new random API Key for the user.**

        A JSON request body containing a "name" property is required. If number of maximum keys is reached, HTTP 403 will be returned.

        There is a limit of 100 API Keys on your account.

        The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

        See the [API Key Permissions List](https://sendgrid.com/docs/API_Reference/Web_API_v3/API_Keys/api_key_permissions_list.html) for a list of all available scopes.
      operationId: api_keys.post
      x-api-path-slug: api-keys-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Api
      - Keys
  /api_keys/{api_key_id}:
    delete:
      summary: Delete Api Keys Api Key
      description: |-
        **This endpoint allows you to revoke an existing API Key**

        Authentications using this API Key will fail after this request is made, with some small propogation delay.If the API Key ID does not exist an HTTP 404 will be returned.

        The API Keys feature allows customers to be able to generate an API Key credential which can be used for authentication with the SendGrid v3 Web API or the [Mail API Endpoint](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

        ## URI Parameters

        | URI Parameter   | Type  | Required?  | Description  |
        |---|---|---|---|
        |api_key_id |string | required | The ID of the API Key you are deleting.|
      operationId: api_keys.api_key_id.delete
      x-api-path-slug: api-keysapi-key-id-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Api
      - Keys
      - Api
      - Key
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