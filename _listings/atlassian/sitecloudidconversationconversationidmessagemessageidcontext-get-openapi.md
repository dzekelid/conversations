---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Software Cloud API Get conversation history contextually
  description: Authentication required, with scope participate:conversation This method
    returns messages after and/or before a given messageID including the message itself.
    Default value for 'after' and 'before' query parameters is 0. Max number of messages
    returned is 75.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /site/{cloudId}/conversation:
    get:
      summary: Get a list of conversations
      description: The API returns the list of conversations the app has access to
        Authentication required, with scope participate:conversation
      operationId: ConversationGetAllHandler
      x-api-path-slug: sitecloudidconversation-get
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: query
        name: cursor
        description: The cursor is a string, that you can use to scroll through the
          data set to get more results
      - in: query
        name: exclude-direct
        description: Exclude direct messages from a response
      - in: query
        name: include-archived
        description: Include archived conversations into response
      - in: query
        name: include-private
        description: Include private conversations into response
      - in: query
        name: limit
        description: A maximum number of conversations to return per call
      - in: query
        name: query
        description: A string containing full or part of conversations name
      - in: query
        name: sort
        description: A sort order of the conversations lists
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Conversations
    post:
      summary: Create conversation
      description: Authentication required, with scope manage:conversation
      operationId: ConversationPostHandler
      x-api-path-slug: sitecloudidconversation-post
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      responses:
        200:
          description: OK
      tags:
      - Conversation
  /site/{cloudId}/conversation/user/{userId}:
    get:
      summary: Get a direct conversation of a user
      description: Get a direct conversation of a user.
      operationId: ConversationUserGetHandler
      x-api-path-slug: sitecloudidconversationuseruserid-get
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: userId
        description: The user Id
      responses:
        200:
          description: OK
      tags:
      - Direct
      - Conversation
      - Of
      - User
  /site/{cloudId}/conversation/user/{userId}/message/{messageId}:
    put:
      summary: Edit a message in a direct conversation
      description: Authentication required, with scope participate:conversation
      operationId: UserMessagePutHandler
      x-api-path-slug: sitecloudidconversationuseruseridmessagemessageid-put
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: messageId
        description: The ID of the message
      - in: path
        name: userId
        description: The user Id
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Message
      - In
      - Direct
      - Conversation
    delete:
      summary: Delete a message in a direct conversation
      description: Authentication required, with scope participate:conversation
      operationId: UserMessageDeleteHandler
      x-api-path-slug: sitecloudidconversationuseruseridmessagemessageid-delete
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: messageId
        description: The ID of the message
      - in: path
        name: userId
        description: The user Id
      responses:
        200:
          description: OK
      tags:
      - Message
      - In
      - Direct
      - Conversation
  /site/{cloudId}/conversation/{conversationId}:
    get:
      summary: Get conversation details
      description: Authentication required, with scope participate:conversation
      operationId: ConversationGetHandler
      x-api-path-slug: sitecloudidconversationconversationid-get
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      responses:
        200:
          description: OK
      tags:
      - Conversation
      - Details
    patch:
      summary: Update conversation
      description: Authentication required, with scope manage:conversation
      operationId: ConversationPatchHandler
      x-api-path-slug: sitecloudidconversationconversationid-patch
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      responses:
        200:
          description: OK
      tags:
      - Conversation
  /site/{cloudId}/conversation/{conversationId}/archive:
    put:
      summary: Archive conversation
      description: Authentication required, with scope manage:conversation
      operationId: ConversationArchivePutHandler
      x-api-path-slug: sitecloudidconversationconversationidarchive-put
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      responses:
        200:
          description: OK
      tags:
      - Archive
      - Conversation
  /site/{cloudId}/conversation/{conversationId}/message:
    get:
      summary: Get conversation history
      description: "Authentication required, with scope participate:conversation This
        method returns messages after/before a given messageIDs or/and timestamps.
        If these parameters are omitted the method returns conversation\u2019s latest
        messages. Max number of messages returned is 75."
      operationId: ConversationMessagesGetHandler
      x-api-path-slug: sitecloudidconversationconversationidmessage-get
      parameters:
      - in: query
        name: afterMessage
        description: Returns at most 75 latest messages after a provided messageID
      - in: query
        name: afterTimestamp
        description: Returns at most 75 latest messages after a provided RFC3339 timestamp
          (2006-01-02T15:04:05+07:00)
      - in: query
        name: beforeMessage
        description: Returns at most 75 messages before a provided messageID
      - in: query
        name: beforeTimestamp
        description: Returns at most 75 messages before a provided RFC3339 timestamp
          (2006-01-02T15:04:05+07:00)
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: query
        name: limit
        description: The maximum number of results
      responses:
        200:
          description: OK
      tags:
      - Conversation
      - History
    post:
      summary: Send a message to a conversation
      description: Send a message to a conversation.
      operationId: ConversationMessagePostHandler
      x-api-path-slug: sitecloudidconversationconversationidmessage-post
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      responses:
        200:
          description: OK
      tags:
      - Send
      - Message
      - To
      - Conversation
  /site/{cloudId}/conversation/{conversationId}/message/{messageId}:
    put:
      summary: Edit a message in a conversation
      description: Authentication required, with scope participate:conversation
      operationId: ConversationMessagePutHandler
      x-api-path-slug: sitecloudidconversationconversationidmessagemessageid-put
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: messageId
        description: The ID of the message
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Message
      - In
      - Conversation
    delete:
      summary: Delete a message in a conversation
      description: Authentication required, with scope participate:conversation
      operationId: ConversationMessageDeleteHandler
      x-api-path-slug: sitecloudidconversationconversationidmessagemessageid-delete
      parameters:
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: messageId
        description: The ID of the message
      responses:
        200:
          description: OK
      tags:
      - Message
      - In
      - Conversation
  /site/{cloudId}/conversation/{conversationId}/message/{messageId}/context:
    get:
      summary: Get conversation history contextually
      description: Authentication required, with scope participate:conversation This
        method returns messages after and/or before a given messageID including the
        message itself. Default value for 'after' and 'before' query parameters is
        0. Max number of messages returned is 75.
      operationId: ConversationContextMessagesGetHandler
      x-api-path-slug: sitecloudidconversationconversationidmessagemessageidcontext-get
      parameters:
      - in: query
        name: after
        description: A number of messages to return after the Message
      - in: query
        name: before
        description: A number of messages to return before the Message
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: messageId
        description: The ID of the Message to retrieve
      responses:
        200:
          description: OK
      tags:
      - Conversation
      - History
      - Contextually
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