---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Delete Conversations by ID's
  description: "Deletes conversation(s) by conversation ID(s). Batch request is supported.\nApp
    Permission\nEditMessages\nUser Permission\nEditMessages\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [conversationId] value is invalid\n\n\n403\nCMN-401\nIn order to call this API
    endpoint, application needs to have [EditMessages] permission"
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