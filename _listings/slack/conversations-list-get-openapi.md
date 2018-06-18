---
swagger: "2.0"
x-collection-name: Slack
x-complete: 0
info:
  title: Slack List Conversations
  description: Lists all channels in a Slack team.
  version: 1.0.3
host: slack.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /conversations.close:
    post:
      summary: Close Conversation
      description: Closes a direct message or multi-person direct message.
      operationId: conversations_close
      x-api-path-slug: conversations-close-post
      parameters:
      - in: formData
        name: channel
        description: Conversation to close
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
  /conversations.join:
    post:
      summary: Join Conversation
      description: Joins an existing conversation.
      operationId: conversations_join
      x-api-path-slug: conversations-join-post
      parameters:
      - in: formData
        name: channel
        description: ID of conversation to join
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
  /conversations.create:
    post:
      summary: Create Conversation
      description: Initiates a public or private channel-based conversation
      operationId: conversations_create
      x-api-path-slug: conversations-create-post
      parameters:
      - in: formData
        name: is_private
        description: Create a private channel instead of a public one
      - in: formData
        name: name
        description: Name of the public or private channel to create
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
  /conversations.unarchive:
    post:
      summary: Unarchve Conversation
      description: Reverses conversation archival.
      operationId: conversations_unarchive
      x-api-path-slug: conversations-unarchive-post
      parameters:
      - in: formData
        name: channel
        description: ID of conversation to unarchive
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
      - Archives
  /conversations.list:
    get:
      summary: List Conversations
      description: Lists all channels in a Slack team.
      operationId: conversations_list
      x-api-path-slug: conversations-list-get
      parameters:
      - in: query
        name: cursor
        description: Paginate through collections of data by setting the `cursor`
          parameter to a `next_cursor` attribute returned by a previous requests `response_metadata`
      - in: query
        name: exclude_archived
        description: Set to `true` to exclude archived channels from the list
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: token
        description: Authentication token
      - in: query
        name: types
        description: Mix and match channel types by providing a comma-separated list
          of any combination of `public_channel`, `private_channel`, `mpim`, `im`
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
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