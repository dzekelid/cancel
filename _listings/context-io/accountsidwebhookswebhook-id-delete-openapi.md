---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Delete Accounts Webhooks Webhook
  description: Cancels a WebHook.
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
  /accounts/{id}/webhooks/{webhook_id}:
    delete:
      summary: Delete Accounts Webhooks Webhook
      description: Cancels a WebHook.
      operationId: Delete_cancelAccountWebhook_
      x-api-path-slug: accountsidwebhookswebhook-id-delete
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: webhook_id
        description: Unique id of the webhook instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Webhooks
      - Webhook
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