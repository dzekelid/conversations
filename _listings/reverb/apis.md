---
name: Reverb
x-slug: reverb
description: 'Reverb&#8217;s mission is to connect people with meaningful content.Reverb
  was created to find and connect the rich associations between words, ideas, content,
  and people. Through our products, we enhance broader knowledge around favorite topics
  by surfacing interesting information readers might not uncover on their own. We
  make tools for content understanding at every level from the single word on up.
  Wordnik: Get a full view of any word you???re interested in, with definitions, example
  sentences, related words, tweets from Twitter, pictures from Flickr, and much more.Reverb
  for Publishers: Reverb for Publishers brings relevant content to web audiences and
  surfaces additional content for publishers.Reverb for Developers: Reverb is committed
  to the open-source community and is proudly contributing infrastructure software
  to power applications and enterprises both small and gigantic. Our involvement with
  the Wordnik API, Scalatra, Swagger and Atmosphere is detailed on our site.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Conversations
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/reverb/apis.md
specificationVersion: "0.14"
apis:
- name: reverb Post Conversations Conversation Offer
  x-api-slug: reverb
  description: Make an offer to the other participant in the conversation
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//conversations/{conversation_id}/offer
  tags: Conversations,Conversation,Id,Offer
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/reverb/conversationsconversation-idoffer-post-openapi.md
- name: reverb Post Conversations Offer
  x-api-slug: reverb
  description: Make an offer to the other participant in the conversation
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//conversations/{id}/offer
  tags: Conversations,Id,Offer
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/reverb/conversationsidoffer-post-openapi.md
- name: reverb Post Listings Listing Conversations
  x-api-slug: reverb
  description: Post listings listing conversations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//listings/{listing_id}/conversations
  tags: Listings,Listing,Id,Conversations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/reverb/listingslisting-idconversations-post-openapi.md
- name: reverb Get My Conversations
  x-api-slug: reverb
  description: Get a list of your conversations
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/conversations
  tags: My,Conversations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/reverb/myconversations-get-openapi.md
- name: reverb Post My Conversations
  x-api-slug: reverb
  description: Post my conversations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/conversations
  tags: My,Conversations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/reverb/myconversations-post-openapi.md
- name: reverb Post My Conversations Conversation Messages
  x-api-slug: reverb
  description: Post my conversations conversation messages.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/conversations/{conversation_id}/messages
  tags: My,Conversations,Conversation,Id,Messages
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/reverb/myconversationsconversation-idmessages-post-openapi.md
- name: reverb Get My Conversations
  x-api-slug: reverb
  description: Display conversation details with messages in natural time order (oldest
    to newest)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/conversations/{id}
  tags: My,Conversations,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/reverb/myconversationsid-get-openapi.md
- name: reverb Put My Conversations
  x-api-slug: reverb
  description: Mark a conversation read/unread
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/conversations/{id}
  tags: My,Conversations,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/reverb/myconversationsid-put-openapi.md
- name: reverb
  x-api-slug: reverb
  description: 'Reverb&#8217;s mission is to connect people with meaningful content.Reverb
    was created to find and connect the rich associations between words, ideas, content,
    and people. Through our products, we enhance broader knowledge around favorite
    topics by surfacing interesting information readers might not uncover on their
    own. We make tools for content understanding at every level from the single word
    on up. Wordnik: Get a full view of any word you???re interested in, with definitions,
    example sentences, related words, tweets from Twitter, pictures from Flickr, and
    much more.Reverb for Publishers: Reverb for Publishers brings relevant content
    to web audiences and surfaces additional content for publishers.Reverb for Developers:
    Reverb is committed to the open-source community and is proudly contributing infrastructure
    software to power applications and enterprises both small and gigantic. Our involvement
    with the Wordnik API, Scalatra, Swagger and Atmosphere is detailed on our site.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api
  tags: Conversations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conversations/master/_listings/reverb/openapi.md
x-common:
- type: x-blog
  url: http://blog.helloreverb.com/
- type: x-blog-rss
  url: http://blog.helloreverb.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/reverb-technologies
- type: x-github
  url: https://github.com/reverb
- type: x-twitter
  url: https://twitter.com/reverb
- type: x-website
  url: https://helloreverb.com/app
- type: x-website
  url: http://reverb.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---