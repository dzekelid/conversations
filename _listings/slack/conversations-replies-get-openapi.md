---
swagger: "2.0"
x-collection-name: Slack
x-complete: 0
info:
  title: Slack Reply Conversation
  description: Retrieve a thread of messages posted to a conversation
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
  /conversations.setTopic:
    post:
      summary: Set Conversation Topic
      description: Sets the topic for a conversation.
      operationId: conversations_setTopic
      x-api-path-slug: conversations-settopic-post
      parameters:
      - in: formData
        name: channel
        description: Conversation to set the topic of
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: topic
        description: The new topic string
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
  /conversations.members:
    get:
      summary: Get Conversation Members
      description: Retrieve members of a conversation.
      operationId: conversations_members
      x-api-path-slug: conversations-members-get
      parameters:
      - in: query
        name: channel
        description: ID of the conversation to retrieve members for
      - in: query
        name: cursor
        description: Paginate through collections of data by setting the `cursor`
          parameter to a `next_cursor` attribute returned by a previous requests `response_metadata`
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
  /conversations.open:
    post:
      summary: Open Conversation
      description: Opens or resumes a direct message or multi-person direct message.
      operationId: conversations_open
      x-api-path-slug: conversations-open-post
      parameters:
      - in: formData
        name: channel
        description: Resume a conversation by supplying an `im` or `mpim`s ID
      - in: formData
        name: return_im
        description: Boolean, indicates you want the full IM channel definition in
          the response
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: users
        description: Comma separated lists of users
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
  /conversations.leave:
    post:
      summary: Leave Conversation
      description: Leaves a conversation.
      operationId: conversations_leave
      x-api-path-slug: conversations-leave-post
      parameters:
      - in: formData
        name: channel
        description: Conversation to leave
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
  /conversations.kick:
    post:
      summary: Remove User From Conversation
      description: Removes a user from a conversation.
      operationId: conversations_kick
      x-api-path-slug: conversations-kick-post
      parameters:
      - in: formData
        name: channel
        description: ID of conversation to remove user from
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: user
        description: User ID to be removed
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
  /conversations.rename:
    post:
      summary: Rename Conversation
      description: Renames a conversation.
      operationId: conversations_rename
      x-api-path-slug: conversations-rename-post
      parameters:
      - in: formData
        name: channel
        description: ID of conversation to rename
      - in: formData
        name: name
        description: New name for conversation
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
  /conversations.history:
    get:
      summary: Get Conversation History
      description: Fetches a conversation's history of messages and events.
      operationId: conversations_history
      x-api-path-slug: conversations-history-get
      parameters:
      - in: query
        name: channel
        description: Conversation ID to fetch history for
      - in: query
        name: cursor
        description: Paginate through collections of data by setting the `cursor`
          parameter to a `next_cursor` attribute returned by a previous requests `response_metadata`
      - in: query
        name: inclusive
        description: Include messages with latest or oldest timestamp in results only
          when either timestamp is specified
      - in: query
        name: latest
        description: End of time range of messages to include in results
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: oldest
        description: Start of time range of messages to include in results
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
  /conversations.setPurpose:
    post:
      summary: Set Conversation Purpose
      description: Sets the purpose for a conversation.
      operationId: conversations_setPurpose
      x-api-path-slug: conversations-setpurpose-post
      parameters:
      - in: formData
        name: channel
        description: Conversation to set the purpose of
      - in: formData
        name: purpose
        description: A new, specialer purpose
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
  /conversations.info:
    get:
      summary: Get Conversation
      description: Retrieve information about a conversation.
      operationId: conversations_info
      x-api-path-slug: conversations-info-get
      parameters:
      - in: query
        name: channel
        description: Conversation ID to learn more about
      - in: query
        name: include_locale
        description: Set this to `true` to receive the locale for this conversation
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
  /dialog.open:
    get:
      summary: Open Dialog
      description: Open a dialog with a user
      operationId: dialog_open
      x-api-path-slug: dialog-open-get
      parameters:
      - in: query
        name: dialog
        description: The dialog definition
      - in: header
        name: token
        description: Authentication token
      - in: query
        name: trigger_id
        description: Exchange a trigger to post to the user
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
  /conversations.invite:
    post:
      summary: Invite User To Conversation
      description: Invites users to a channel.
      operationId: conversations_invite
      x-api-path-slug: conversations-invite-post
      parameters:
      - in: formData
        name: channel
        description: The ID of the public or private channel to invite user(s) to
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: users
        description: A comma separated list of user IDs
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
  /conversations.archive:
    post:
      summary: Archive Conversation
      description: Archives a conversation.
      operationId: conversations_archive
      x-api-path-slug: conversations-archive-post
      parameters:
      - in: formData
        name: channel
        description: ID of conversation to archive
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
  /conversations.replies:
    get:
      summary: Reply Conversation
      description: Retrieve a thread of messages posted to a conversation
      operationId: conversations_replies
      x-api-path-slug: conversations-replies-get
      parameters:
      - in: query
        name: channel
        description: Conversation ID to fetch thread from
      - in: query
        name: cursor
        description: Paginate through collections of data by setting the `cursor`
          parameter to a `next_cursor` attribute returned by a previous requests `response_metadata`
      - in: query
        name: inclusive
        description: Include messages with latest or oldest timestamp in results only
          when either timestamp is specified
      - in: query
        name: latest
        description: End of time range of messages to include in results
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: oldest
        description: Start of time range of messages to include in results
      - in: query
        name: token
        description: Authentication token
      - in: query
        name: ts
        description: Unique identifier of a threads parent message
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