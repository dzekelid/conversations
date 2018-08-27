---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: Reverb Post My Conversations
  description: Post my conversations.
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /conversations/{conversation_id}/offer:
    post:
      summary: Post Conversations Conversation Offer
      description: Make an offer to the other participant in the conversation
      operationId: postConversationsConversationOffer
      x-api-path-slug: conversationsconversation-idoffer-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: conversation_id
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - Conversation
      - Id
      - Offer
  /conversations/{id}/offer:
    post:
      summary: Post Conversations Offer
      description: Make an offer to the other participant in the conversation
      operationId: postConversationsOffer
      x-api-path-slug: conversationsidoffer-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - Id
      - Offer
  /listings/{listing_id}/conversations:
    post:
      summary: Post Listings Listing Conversations
      description: Post listings listing conversations.
      operationId: postListingsListingConversations
      x-api-path-slug: listingslisting-idconversations-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Conversations
  /my/conversations:
    get:
      summary: Get My Conversations
      description: Get a list of your conversations
      operationId: getMyConversations
      x-api-path-slug: myconversations-get
      parameters:
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: search
        description: Query string to search conversations by
      - in: query
        name: unread_only
        description: Show unread conversations only
      responses:
        200:
          description: OK
      tags:
      - My
      - Conversations
    post:
      summary: Post My Conversations
      description: Post my conversations.
      operationId: postMyConversations
      x-api-path-slug: myconversations-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - My
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