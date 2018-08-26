---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 1
info:
  title: Global Change Information System API
  description: who-we-are-what-the-gcis-is-and-how-we-use-identifiers-and-semantic-information-to-provide-points-of-reference-and-traceability--examples-and-tutorials-for-using-this-system-as-a-researcher-citizen-scientist-application-developer-or-information-theorist--a-description-of-how-the-information-is-structured-including-the-overlaps-between-relational-and-semantic-representations-of-the-information--complete-documentation-for-the-api-including-methods-for-browsing-and-finding-resources-
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /webpage:
    get:
      summary: List web pages.
      description: List the web pages, 20 per page.
      operationId: list-the-web-pages-20-per-page
      x-api-path-slug: webpage-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the web pages
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Web
      - Pages
  /webpage/{webpage_identifier}:
    get:
      summary: Get a representation of a web page.
      description: Get JSON which represents the structure of a web page.
      operationId: get-json-which-represents-the-structure-of-a-web-page
      x-api-path-slug: webpagewebpage-identifier-get
      parameters:
      - in: path
        name: webpage_identifier
        description: webpage_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the web page
      - in: query
        name: with_regions
        description: Include regions associated with the web page
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Web
      - Page
---