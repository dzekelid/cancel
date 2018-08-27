swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 1
info:
  title: Coinbase API
  description: the-coinbase-v2-api
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