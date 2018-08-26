---
swagger: "2.0"
x-collection-name: AWS WAF
x-complete: 0
info:
  title: AWS WAF API Delete Web ACL
  version: 1.0.0
  description: 'Service: AWS WAFPermanently deletes a.'
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AssociateWebACL:
    get:
      summary: Associate Web ACL
      description: 'Service: AWS WAF RegionalAssociates a web ACL with a resource.'
      operationId: associateWebACL
      x-api-path-slug: actionassociatewebacl-get
      parameters:
      - in: query
        name: ResourceArn
        description: The ARN (Amazon Resource Name) of the resource to be protected
        type: string
      - in: query
        name: WebACLId
        description: A unique identifier (ID) for the web ACL
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
  /?Action=CreateWebACL:
    get:
      summary: Create Web ACL
      description: 'Service: AWS WAFCreates a WebACL, which contains the Rules that
        identify the CloudFront web requests that you want to allow, block, or count.'
      operationId: createWebACL
      x-api-path-slug: actioncreatewebacl-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: DefaultAction
        description: The action that you want  AWS WAF to take when a request doesnt
          match the criteria specified in any of the Rule objects that are associated
          with the WebACL
        type: string
      - in: query
        name: MetricName
        description: A friendly name or description for the metrics for this WebACL
        type: string
      - in: query
        name: Name
        description: A friendly name or description of the WebACL
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
  /?Action=DeleteWebACL:
    get:
      summary: Delete Web ACL
      description: 'Service: AWS WAFPermanently deletes a.'
      operationId: deleteWebACL
      x-api-path-slug: actiondeletewebacl-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: WebACLId
        description: The WebACLId of the WebACL that you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
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