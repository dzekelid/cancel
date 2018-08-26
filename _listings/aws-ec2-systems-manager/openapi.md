---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 1
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CancelCommand:
    get:
      summary: Cancel Command
      description: Attempts to cancel the command specified by the Command ID.
      operationId: cancelCommand
      x-api-path-slug: actioncancelcommand-get
      parameters:
      - in: query
        name: CommandId
        description: The ID of the command you want to cancel
        type: string
      - in: query
        name: InstanceIds
        description: (Optional) A list of instance IDs on which you want to cancel
          the command
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Command
---