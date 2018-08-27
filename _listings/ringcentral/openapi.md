swagger: "2.0"
x-collection-name: RingCentral
x-complete: 1
info:
  title: RingCentral Connect Platform API Explorer
  description: this-is-an-interactive-api-explorer-for-the-ringcentral-connect-platform--to-use-this-service-you-will-need-to-have-a-developer-account---links--a-hrefhttpsnetstorage-ringcentral-comdpwapiexplorerrcplatform-basic-ymlv20180514092722-target-blankringcentral-api-specaspannbspnbspopenapi-fka-swagger-formatnbspnbspnbspnbspspana-hrefhttpsgithub-comoaiopenapispecification-target-blanklearn-more-about-openapia
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
  /restapi/v1.0/subscription/{subscriptionId}:
    delete:
      summary: Cancel Subscription
      description: "Cancels the existent subscription.\nUsage Plan Group\nMedium\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource
        for parameter [subscriptionId] is not found"
      operationId: deleteSubscription
      x-api-path-slug: restapiv1-0subscriptionsubscriptionid-delete
      parameters:
      - in: path
        name: subscriptionId
        description: Internal identifier of a subscription
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Subscription