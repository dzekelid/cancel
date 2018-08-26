---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 1
info:
  title: Context.IO
  description: context-io-is-the-missing-email-api-that-makes-it-easy-and-fast-to-integrate-your-users-email-data-in-your-application-
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
---