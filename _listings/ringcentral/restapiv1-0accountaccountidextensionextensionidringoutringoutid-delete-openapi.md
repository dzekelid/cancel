---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Cancel RingOut Call
  description: "Cancels a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage Plan
    Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n
    \  \n \n\n404\nCMN-102\nResource for parameter [extensionId] is not found"
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/ring-out/{ringoutId}:
    delete:
      summary: Cancel RingOut Call
      description: "Cancels a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
        Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n404\nCMN-102\nResource for parameter [ringOutId] is not
        found"
      operationId: cancelRingOutCallNew
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-delete
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: ringoutId
        description: Internal identifier of a RingOut call
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - RingOut
      - Call
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/ringout/{ringoutId}:
    delete:
      summary: Cancel RingOut Call
      description: "Cancels a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
        Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n404\nCMN-102\nResource for parameter [extensionId] is not
        found"
      operationId: cancelRingOutCall
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-delete
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: ringoutId
        description: Internal identifier of a RingOut call
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - RingOut
      - Call
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