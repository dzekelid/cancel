---
swagger: "2.0"
x-collection-name: PayPal
x-complete: 1
info:
  title: PayPal (Sandbox)
  description: bring-payments-to-apps-mobile-and-social-with-adaptive-payments-bsandbox-api-b
  version: 1.0.0
host: svcs.sandbox.paypal.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /AdaptivePayments/CancelPreapproval:
    post:
      summary: Cancel Preapproval
      description: Use the CancelPreapproval API operation to handle the canceling
        of preapprovals. Preapprovals can be canceled regardless of the state they
        are in, such as active, expired, deactivated, and previously canceled.
      operationId: AdaptivePayments.CancelPreapproval.post
      x-api-path-slug: adaptivepaymentscancelpreapproval-post
      responses:
        200:
          description: OK
      tags:
      - Payments
---