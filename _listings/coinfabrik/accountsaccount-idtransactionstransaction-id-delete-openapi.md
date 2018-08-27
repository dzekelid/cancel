---
swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 0
info:
  title: CoinFabrik Cancel request money
  description: Lets a user cancel a money request. Money requests can be canceled
    by the sender or the recipient.
  contact:
    name: CoinFabrik
    url: http://www.coinfabrik.com/
  version: 1.0.0
host: api.coinbase.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{account_id}/transactions/{transaction_id}:
    delete:
      summary: Cancel request money
      description: Lets a user cancel a money request. Money requests can be canceled
        by the sender or the recipient.
      operationId: lets-a-user-cancel-a-money-request-money-requests-can-be-canceled-by-the-sender-or-the-recipient
      x-api-path-slug: accountsaccount-idtransactionstransaction-id-delete
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: path
        name: transaction_id
        description: The transaction id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Cancel
      - Request
      - Money
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