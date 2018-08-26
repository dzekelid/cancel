---
swagger: "2.0"
x-collection-name: AWS CloudFormation
x-complete: 1
info:
  title: AWS CloudFormation API
  version: 1.0.0
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
---