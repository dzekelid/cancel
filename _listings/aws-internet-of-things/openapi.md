swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 1
info:
  title: AWS Internet of Things API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CancelCertificateTransfer:
    get:
      summary: Cancel Certificate Transfer
      description: Cancels a pending transfer for the specified certificate.
      operationId: cancelCertificateTransfer
      x-api-path-slug: actioncancelcertificatetransfer-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificate Transfers