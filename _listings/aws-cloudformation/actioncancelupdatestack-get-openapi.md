---
swagger: "2.0"
x-collection-name: AWS CloudFormation
x-complete: 0
info:
  title: AWS CloudFormation API Cancel Update Stack
  version: 1.0.0
  description: Cancels an update on the specified stack.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CancelUpdateStack:
    get:
      summary: Cancel Update Stack
      description: Cancels an update on the specified stack.
      operationId: cancelUpdateStack
      x-api-path-slug: actioncancelupdatestack-get
      parameters:
      - in: query
        name: StackName
        description: The name or the unique stack ID that is associated with the stack
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stacks
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