swagger: "2.0"
x-collection-name: AWS Key Management Service
x-complete: 1
info:
  title: AWS Key Management Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CancelKeyDeletion:
    get:
      summary: Cancel Key Deletion
      description: Cancels the deletion of a customer master key (CMK).
      operationId: cancelKeyDeletion
      x-api-path-slug: actioncancelkeydeletion-get
      parameters:
      - in: query
        name: KeyId
        description: The unique identifier for the customer master key (CMK) for which
          to cancel      deletion
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys