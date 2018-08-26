---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Add a Web page Widget
  description: Add a new Web page Widget to the specified playlist
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /playlist/widget/webpage/{playlistId}:
    post:
      summary: Add a Web page Widget
      description: Add a new Web page Widget to the specified playlist
      operationId: WidgetWebpageAdd
      x-api-path-slug: playlistwidgetwebpageplaylistid-post
      parameters:
      - in: formData
        name: duration
        description: The Web page Duration
      - in: formData
        name: modeId
        description: The mode option for Web page, 1- Open Natively, 2- Manual Position,
          3- Best Ft
      - in: formData
        name: name
        description: Optional Widget Name
      - in: formData
        name: offsetLeft
        description: For Manual position, the starting point from the left in pixels
      - in: formData
        name: offsetTop
        description: For Manual position, the starting point from the Top in pixels
      - in: formData
        name: pageHeight
        description: For Manual Position and Best Fit, The height of the page - if
          empty it will use region height
      - in: formData
        name: pageWidth
        description: For Manual Position and Best Fit, The width of the page - if
          empty it will use region width
      - in: path
        name: playlistId
        description: The playlist ID to add a Web page to
      - in: formData
        name: scaling
        description: For Manual position the percentage to scale the Web page (0-100)
      - in: formData
        name: transparency
        description: flag (0,1) should the HTML be shown with a transparent background?
      - in: formData
        name: uri
        description: string containing the location (URL) of the web page
      - in: formData
        name: useDuration
        description: (0, 1) Select 1 only if you will provide duration parameter as
          well
      responses:
        200:
          description: OK
      tags:
      - Web
      - Page
      - Widget
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