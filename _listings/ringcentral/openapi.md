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
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/message-store:
    delete:
      summary: Delete Conversations by ID's
      description: "Deletes conversation(s) by conversation ID(s). Batch request is
        supported.\nApp Permission\nEditMessages\nUser Permission\nEditMessages\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [conversationId] value is invalid\n\n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [EditMessages]
        permission"
      operationId: deleteMessagesByFilter
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmessagestore-delete
      parameters:
      - in: path
        name: accountId
      - in: query
        name: conversationId
      - in: path
        name: extensionId
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - By
      - IDs