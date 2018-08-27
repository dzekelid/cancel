---
swagger: "2.0"
x-collection-name: VersaPay
x-complete: 0
info:
  title: VersaPay Cancel a Transaction
  description: |-
    Cancel a `new`, `wait_for_request_approval` or `wait_for_bank_account_verification` transaction you created. Transactions cannot be cancelled after they have been sent to the bank and are `in_progress`.<br>
    An API key with administrative access is required to approve a transaction.
  contact:
    name: VersaPay Support
    url: https://www.versapay.com/support
    email: support@versapay.com
  version: 1.0.0
host: secure.versapay.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/transactions/{token}/cancel:
    post:
      summary: Cancel a Transaction
      description: |-
        Cancel a `new`, `wait_for_request_approval` or `wait_for_bank_account_verification` transaction you created. Transactions cannot be cancelled after they have been sent to the bank and are `in_progress`.<br>
        An API key with administrative access is required to approve a transaction.
      operationId: cancelTransaction
      x-api-path-slug: apitransactionstokencancel-post
      parameters:
      - in: path
        name: token
        description: The transaction identifier
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Transactions
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