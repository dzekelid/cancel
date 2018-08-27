---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 0
info:
  title: AWS Storage Gateway Service API Cancel Archival
  version: 1.0.0
  description: |-
    Cancels archiving of a virtual tape to the virtual tape shelf (VTS) after the
             archiving process is initiated.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CancelArchival:
    get:
      summary: Cancel Archival
      description: |-
        Cancels archiving of a virtual tape to the virtual tape shelf (VTS) after the
                 archiving process is initiated.
      operationId: cancelArchival
      x-api-path-slug: actioncancelarchival-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: TapeARN
        description: The Amazon Resource Name (ARN) of the virtual tape you want to
          cancel archiving         for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Archival
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