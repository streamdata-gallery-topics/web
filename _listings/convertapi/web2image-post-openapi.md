---
swagger: "2.0"
x-collection-name: ConvertAPI
x-complete: 0
info:
  title: Convert API Web to Image
  description: The API for converting Web Pages to Images.
  version: v1
host: do.convertapi.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Web2Image:
    post:
      summary: Web to Image
      description: The API for converting Web Pages to Images.
      operationId: web2image
      x-api-path-slug: web2image-post
      parameters:
      - in: query
        name: AcceptLanguage
        description: Set accept language header
      - in: query
        name: AlternativeParser
        description: Set alternative parser
      - in: query
        name: ApiKey
        description: API Key should be passed if you purchased membership with credits
      - in: query
        name: AuthPassword
        description: HTTP Authentication password, used if conversion web page is
          protected with HTTP authentication
      - in: query
        name: AuthUsername
        description: HTTP authentication username, used if conversion web page is
          protected with HTTP authentication
      - in: query
        name: ConversionDelay
        description: Delay in seconds before page load and PDF creation
      - in: query
        name: CUrl
        description: URI of a web page to convert
      - in: query
        name: PageHeight
        description: Set screen height
      - in: query
        name: PageWidth
        description: Set screen width
      - in: query
        name: Plugins
        description: Enable plugins such as flash
      - in: query
        name: Scripts
        description: Allow web pages to run javascript
      - in: query
        name: StoreFile
        description: Store file on server and return url to file instead of file stream
          response
      - in: query
        name: Timeout
        description: Conversion timeout in seconds
      - in: query
        name: UserAgent
        description: Set custom user agent
      responses:
        200:
          description: OK
      tags:
      - Web
      - Image
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