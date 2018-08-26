---
swagger: "2.0"
x-collection-name: AWS Security Token Service
x-complete: 1
info:
  title: AWS Security Token Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AssumeRoleWithWebIdentity:
    get:
      summary: Assume Role With Web Identity
      description: |-
        Returns a set of temporary security credentials for users who have been authenticated
              in a mobile or web application with a web identity provider, such as Amazon Cognito, Login with Amazon,
              Facebook, Google, or any OpenID Connect-compatible identity provider.
      operationId: assumeRoleWithWebIdentity
      x-api-path-slug: actionassumerolewithwebidentity-get
      parameters:
      - in: query
        name: DurationSeconds
        description: The duration, in seconds, of the role session
        type: string
      - in: query
        name: Policy
        description: An IAM policy in JSON format
        type: string
      - in: query
        name: ProviderId
        description: The fully qualified host component of the domain name of the
          identity      provider
        type: string
      - in: query
        name: RoleArn
        description: The Amazon Resource Name (ARN) of the role that the caller is
          assuming
        type: string
      - in: query
        name: RoleSessionName
        description: An identifier for the assumed role session
        type: string
      - in: query
        name: WebIdentityToken
        description: The OAuth 2
        type: string
      responses:
        200:
          description: OK
      tags:
      - Roles
---