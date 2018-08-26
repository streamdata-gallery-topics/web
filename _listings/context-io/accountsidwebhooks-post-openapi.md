---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Post Accounts Webhooks
  description: Creates a new WebHook on an account.
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}/webhooks:
    get:
      summary: Get Accounts Webhooks
      description: List WebHooks configured for an account.
      operationId: listAccountWebhooks_
      x-api-path-slug: accountsidwebhooks-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Webhooks
    post:
      summary: Post Accounts Webhooks
      description: Creates a new WebHook on an account.
      operationId: createAccountWebhook_
      x-api-path-slug: accountsidwebhooks-post
      parameters:
      - in: query
        name: callback_url
        description: A valid URL Context
      - in: query
        name: failure_notif_url
        description: A valid URL Context
      - in: query
        name: filter_cc
        description: Check for new messages where a given name or email address is
          cced
      - in: query
        name: filter_file_name
        description: Check for new messages where a file whose name matches the given
          string is attached
      - in: query
        name: filter_file_revisions
        description: Check for new message where a new revision of a given file is
          attached
      - in: query
        name: filter_folder_added
        description: Check for messages filed in a given folder
      - in: query
        name: filter_folder_removed
        description: Check for messages removed from a given folder
      - in: query
        name: filter_from
        description: Check for new messages received from a given name or email address
      - in: query
        name: filter_new_important
        description: Check for new messages automatically tagged as important by the
          Gmail Priority Inbox algorithm
      - in: query
        name: filter_subject
        description: Check for new messages with a subject matching a given string
          or regular expresion
      - in: query
        name: filter_thread
        description: Check for new messages in a given thread
      - in: query
        name: filter_to
        description: Check for new messages sent to a given name or email address
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: sync_period
        description: Desired maximum delay between the moment the email comes in the
          users mailbox and the time we call the callback_url
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Webhooks
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