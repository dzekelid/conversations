---
name: Instructure
x-slug: instructure
description: Instructure makes software that makes smarter people. Products include
  Canvas LMS, Bridge and Canvas Network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
x-kinRank: "8"
x-alexaRank: "367"
tags: Conversations
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/apis.md
specificationVersion: "0.14"
apis:
- name: Instructure Canvas Conversations API List conversations
  x-api-slug: instructure-canvas-conversations-api
  description: List conversations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations
  tags: Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversations-get-openapi.md
- name: Instructure Canvas Conversations API Create a conversation
  x-api-slug: instructure-canvas-conversations-api
  description: Create a conversation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations
  tags: Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversations-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversations-post-openapi.md
- name: Instructure Canvas Conversations API Batch update conversations
  x-api-slug: instructure-canvas-conversations-api
  description: Batch update conversations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations
  tags: Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversations-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversations-put-openapi.md
- name: Instructure Canvas Conversations API Get running batches
  x-api-slug: instructure-canvas-conversations-api
  description: Get running batches.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/batches
  tags: Conversations,Batches
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsbatches-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsbatches-get-openapi.md
- name: Instructure Canvas Conversations API Find recipients
  x-api-slug: instructure-canvas-conversations-api
  description: Find recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/find_recipients
  tags: Conversations,Find,Recipients
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsfind-recipients-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsfind-recipients-get-openapi.md
- name: Instructure Canvas Conversations API Mark all as read
  x-api-slug: instructure-canvas-conversations-api
  description: Mark all as read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/mark_all_as_read
  tags: Conversations,Mark,,As,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsmark-all-as-read-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsmark-all-as-read-post-openapi.md
- name: Instructure Canvas Conversations API Unread count
  x-api-slug: instructure-canvas-conversations-api
  description: Unread count.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/unread_count
  tags: Conversations,Unread,Count
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsunread-count-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsunread-count-get-openapi.md
- name: Instructure Canvas Conversations API Delete a conversation
  x-api-slug: instructure-canvas-conversations-api
  description: Delete a conversation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/{id}
  tags: Conversations,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsid-delete-openapi.md
- name: Instructure Canvas Conversations API Get a single conversation
  x-api-slug: instructure-canvas-conversations-api
  description: Get a single conversation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/{id}
  tags: Conversations,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsid-get-openapi.md
- name: Instructure Canvas Conversations API Edit a conversation
  x-api-slug: instructure-canvas-conversations-api
  description: Edit a conversation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/{id}
  tags: Conversations,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsid-put-openapi.md
- name: Instructure Canvas Conversations API Add a message
  x-api-slug: instructure-canvas-conversations-api
  description: Add a message.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/{id}/add_message
  tags: Conversations,Id,Add,Message
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsidadd-message-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsidadd-message-post-openapi.md
- name: Instructure Canvas Conversations API Add recipients
  x-api-slug: instructure-canvas-conversations-api
  description: Add recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/{id}/add_recipients
  tags: Conversations,Id,Add,Recipients
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsidadd-recipients-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsidadd-recipients-post-openapi.md
- name: Instructure Canvas Conversations API Delete a message
  x-api-slug: instructure-canvas-conversations-api
  description: Delete a message.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/{id}/remove_messages
  tags: Conversations,Id,Remove,Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsidremove-messages-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/conversationsidremove-messages-post-openapi.md
- name: Instructure Canvas Conversations API
  x-api-slug: instructure-canvas-conversations-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Conversations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/instructure/openapi.md
x-common:
- type: x-blog
  url: http://blog.instructure.com
- type: x-blog-rss
  url: http://voice.instructure.com/CMS/UI/Modules/BizBlogger/rss.aspx?tabid=772438&moduleid=1638884&maxcount=25&t=415c2e5d197a4d6f7cdcc81385b677f1
- type: x-crunchbase
  url: https://crunchbase.com/organization/instructure
- type: x-crunchbase
  url: http://www.crunchbase.com/company/instructure
- type: x-email
  url: info@instructure.com
- type: x-email
  url: jobs@instructure.com
- type: x-email
  url: privacy@instructure.com
- type: x-email
  url: legal@instructure.com
- type: x-github
  url: https://github.com/instructure
- type: x-twitter
  url: https://twitter.com/instructure
- type: x-website
  url: http://instructure.com
- type: x-website
  url: https://canvas.instructure.com/doc/api/index.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---