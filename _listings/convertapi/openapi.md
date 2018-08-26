---
swagger: "2.0"
x-collection-name: ConvertAPI
x-complete: 1
info:
  title: Convert API
  description: the-convertapi-provides-online-api-for-creating-pdf-and-images-from-various-sources-like-word-document-web-pages-or-raw-html-codes--in-just-few-minutes-you-can-integrate-it-into-your-application-and-use-it-easily--return-to-apis-list-
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
  /Web2Pdf:
    post:
      summary: Web to PDF
      description: The API for converting Web Pages to PDF files.
      operationId: web2pdf
      x-api-path-slug: web2pdf-post
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
        name: Background
        description: Print web page background
      - in: query
        name: ConversionDelay
        description: Delay in seconds before page load and PDF creation
      - in: query
        name: CoverUrl
        description: Use html document as cover
      - in: query
        name: CUrl
        description: URI of a web page to convert
      - in: query
        name: DocumentTitle
        description: Set the title of the generated pdf file
      - in: query
        name: FooterLine
        description: Display line above the footer
      - in: query
        name: FooterSpacing
        description: Spacing between footer and content
      - in: query
        name: FooterTextCenter
        description: Center aligned footer text
      - in: query
        name: FooterTextFont
        description: Set footer font name
      - in: query
        name: FooterTextLeft
        description: Left aligned footer text
      - in: query
        name: FooterTextRight
        description: Right aligned footer text
      - in: query
        name: FooterTextSize
        description: Set footer font size
      - in: query
        name: FooterUrl
        description: Adds a html footer
      - in: query
        name: HeaderLine
        description: Display line below the header
      - in: query
        name: HeaderSpacing
        description: Spacing between header and content
      - in: query
        name: HeaderTextCenter
        description: Center aligned header text
      - in: query
        name: HeaderTextFont
        description: Set header font name
      - in: query
        name: HeaderTextLeft
        description: Left aligned header text
      - in: query
        name: HeaderTextRight
        description: Right aligned header text
      - in: query
        name: HeaderTextSize
        description: Set header font size
      - in: query
        name: HeaderUrl
        description: Adds a html header
      - in: query
        name: InfoStamp
        description: Show date stamp and conversion url in header
      - in: query
        name: LowQuality
        description: Generates lower quality PDF, makes smaller file size
      - in: query
        name: MarginBottom
        description: Set the page bottom margin
      - in: query
        name: MarginLeft
        description: Set the page left margin
      - in: query
        name: MarginRight
        description: Set the page right margin
      - in: query
        name: MarginTop
        description: Set the page top margin
      - in: query
        name: Outline
        description: Show outline in PDF file
      - in: query
        name: PageHeight
        description: Custom page height
      - in: query
        name: PageNo
        description: Show page number in footer
      - in: query
        name: PageOrientation
        description: 'PDF page orientation: portrait, landscape'
      - in: query
        name: PageSize
        description: PDF page paper sizes
      - in: query
        name: PageWidth
        description: Custom page width
      - in: query
        name: Plugins
        description: Enable plugins such as flash
      - in: query
        name: PrintType
        description: Use print media-type(print css sheet) instead of screen
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
      - PDF
---