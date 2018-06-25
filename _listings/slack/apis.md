---
name: Slack
x-slug: slack
description: Slack is a team communication application providing services such as
  real-time messaging, archiving, and to search for modern teams. It offers one-on-one
  messaging, private groups, persistent chat rooms, and direct messaging as well as
  group chats organized by topic. All content inside Slack is searchable from one
  search box and it integrates with a number of third-party services, including Google
  Docs, Dropbox, Heroku, Crashlytics, GitHub, and Zendesk.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Conversations
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/apis.md
specificationVersion: "0.14"
apis:
- name: Slack Close Conversation
  x-api-slug: slack
  description: Closes a direct message or multi-person direct message.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.close
  tags: Messaging,Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-close-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-close-post-openapi.md
- name: Slack Join Conversation
  x-api-slug: slack
  description: Joins an existing conversation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.join
  tags: Messaging,Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-join-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-join-post-openapi.md
- name: Slack Create Conversation
  x-api-slug: slack
  description: Initiates a public or private channel-based conversation
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.create
  tags: Messaging,Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-create-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-create-post-openapi.md
- name: Slack Unarchve Conversation
  x-api-slug: slack
  description: Reverses conversation archival.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.unarchive
  tags: Messaging,Conversations, Archives
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-unarchive-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-unarchive-post-openapi.md
- name: Slack List Conversations
  x-api-slug: slack
  description: Lists all channels in a Slack team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.list
  tags: Messaging,Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-list-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-list-get-openapi.md
- name: Slack Set Conversation Topic
  x-api-slug: slack
  description: Sets the topic for a conversation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.setTopic
  tags: Messaging,Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-settopic-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-settopic-post-openapi.md
- name: Slack Get Conversation Members
  x-api-slug: slack
  description: Retrieve members of a conversation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.members
  tags: Messaging,Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-members-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-members-get-openapi.md
- name: Slack Open Conversation
  x-api-slug: slack
  description: Opens or resumes a direct message or multi-person direct message.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.open
  tags: Messaging,Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-open-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-open-post-openapi.md
- name: Slack Leave Conversation
  x-api-slug: slack
  description: Leaves a conversation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.leave
  tags: Messaging,Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-leave-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-leave-post-openapi.md
- name: Slack Remove User From Conversation
  x-api-slug: slack
  description: Removes a user from a conversation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.kick
  tags: Messaging,Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-kick-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-kick-post-openapi.md
- name: Slack Rename Conversation
  x-api-slug: slack
  description: Renames a conversation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.rename
  tags: Messaging,Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-rename-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-rename-post-openapi.md
- name: Slack Get Conversation History
  x-api-slug: slack
  description: Fetches a conversation's history of messages and events.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.history
  tags: Messaging,Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-history-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-history-get-openapi.md
- name: Slack Set Conversation Purpose
  x-api-slug: slack
  description: Sets the purpose for a conversation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.setPurpose
  tags: Messaging,Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-setpurpose-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-setpurpose-post-openapi.md
- name: Slack Get Conversation
  x-api-slug: slack
  description: Retrieve information about a conversation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.info
  tags: Messaging,Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-info-get-openapi.md
- name: Slack Open Dialog
  x-api-slug: slack
  description: Open a dialog with a user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//dialog.open
  tags: Messaging,Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/dialog-open-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/dialog-open-get-openapi.md
- name: Slack Invite User To Conversation
  x-api-slug: slack
  description: Invites users to a channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.invite
  tags: Messaging,Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-invite-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-invite-post-openapi.md
- name: Slack Archive Conversation
  x-api-slug: slack
  description: Archives a conversation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.archive
  tags: Messaging,Conversations, Archives
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-archive-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-archive-post-openapi.md
- name: Slack Reply Conversation
  x-api-slug: slack
  description: Retrieve a thread of messages posted to a conversation
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//conversations.replies
  tags: Messaging,Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-replies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/conversations-replies-get-openapi.md
- name: Slack
  x-api-slug: slack
  description: Slack is a team communication application providing services such as
    real-time messaging, archiving, and to search for modern teams. It offers one-on-one
    messaging, private groups, persistent chat rooms, and direct messaging as well
    as group chats organized by topic. All content inside Slack is searchable from
    one search box and it integrates with a number of third-party services, including
    Google Docs, Dropbox, Heroku, Crashlytics, GitHub, and Zendesk.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Conversations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/slack/openapi.md
x-common:
- type: x-website
  url: https://api.slack.com
- type: x-application-gallery
  url: https://slack.com/apps
- type: x-blog
  url: http://slackhq.com/
- type: x-blog
  url: https://medium.com/slack-developer-blog
- type: x-blog-rss
  url: http://slackhq.com/rss
- type: x-blog-rss
  url: https://medium.com/feed/slack-developer-blog
- type: x-branding
  url: https://slack.com/brand-guidelines
- type: x-buttons
  url: https://api.slack.com/docs/slack-button
- type: x-c-sharp-sdk
  url: https://api.slack.com/web
- type: x-change-log
  url: https://api.slack.com/changelog
- type: x-developer
  url: https://api.slack.com/
- type: x-faq
  url: https://api.slack.com/faq
- type: x-getting-started
  url: https://slack.com/getting-started
- type: x-github
  url: https://github.com/slackhq
- type: x-incoming-webhooks
  url: https://api.slack.com/incoming-webhooks
- type: x-oauth-overview
  url: https://api.slack.com/docs/oauth
- type: x-oauth-scopes
  url: https://api.slack.com/docs/oauth-scopes
- type: x-outgoing-webhooks
  url: https://api.slack.com/outgoing-webhooks
- type: x-presence
  url: https://api.slack.com/docs/presence
- type: x-pricing
  url: https://slack.com/pricing
- type: x-privacy
  url: https://slack.com/privacy-policy
- type: x-rate-limits
  url: https://api.slack.com/docs/rate-limits
- type: x-real-time-messaging-api
  url: https://api.slack.com/rtm
- type: x-road-map
  url: https://api.slack.com/roadmap
- type: x-security
  url: https://slack.com/security
- type: x-status
  url: https://status.slack.com/
- type: x-support
  url: https://get.slack.help/hc/en-us
- type: x-terms-of-service
  url: https://slack.com/terms-of-service
- type: x-transparency-report
  url: https://slack.com/transparency-report
- type: x-twitter
  url: https://twitter.com/slackapi
- type: x-website
  url: http://slack.com
- type: x-website
  url: https://slack.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---