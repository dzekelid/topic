---
name: Google Cloud Pub Sub
x-slug: google-cloud-pub-sub
description: Cloud Pub/Sub is a fully-managed real-time messaging service that allows
  you to send and receive messages between independent applications. You can leverage
  Cloud Pub/Sub&rsquo;s flexibility to decouple systems and components hosted on Google
  Cloud Platform or elsewhere on the Internet. By building on the same technology
  Google uses, Cloud Pub/Sub is designed to provide &ldquo;at least once&rdquo; delivery
  at low latency with on-demand scalability to 1 million messages per second (and
  beyond).
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Topic
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/topic/master/_listings/google-cloud-pub-sub/apis.md
specificationVersion: "0.14"
apis:
- name: Google Cloud Pub/Sub - Create Topic
  x-api-slug: v1name-put
  description: Creates the given topic with the given name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/topic/master/_listings/google-cloud-pub-sub/v1name-put-openapi.md
- name: Google Cloud Pub/Sub - List Matching Topics
  x-api-slug: v1projecttopics-get
  description: Lists matching topics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/topic/master/_listings/google-cloud-pub-sub/v1projecttopics-get-openapi.md
- name: Google Cloud Pub/Sub - Delete Topic
  x-api-slug: v1topic-delete
  description: |-
    Deletes the topic with the given name. Returns `NOT_FOUND` if the topic
    does not exist. After a topic is deleted, a new topic may be created with
    the same name; this is an entirely new topic with none of the old
    configuration or subscriptions. Existing subscriptions to this topic are
    not deleted, but their `topic` field is set to `_deleted-topic_`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/topic/master/_listings/google-cloud-pub-sub/v1topic-delete-openapi.md
- name: Google Cloud Pub/Sub - Get Topic Configuration
  x-api-slug: v1topic-get
  description: Gets the configuration of a topic.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/topic/master/_listings/google-cloud-pub-sub/v1topic-get-openapi.md
- name: Google Cloud Pub/Sub - Get Topic Subscription
  x-api-slug: v1topicsubscriptions-get
  description: Lists the name of the subscriptions for this topic.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/topic/master/_listings/google-cloud-pub-sub/v1topicsubscriptions-get-openapi.md
- name: Google Cloud Pub/Sub - Publish Topic
  x-api-slug: v1topicpublish-post
  description: |-
    Adds one or more messages to the topic. Returns `NOT_FOUND` if the topic
    does not exist. The message payload must not be empty; it must contain
     either a non-empty data field, or at least one attribute.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-pub-sub-middleware.png
  humanURL: https://cloud.google.com/pubsub/docs/
  baseURL: ://pubsub.googleapis.com//
  tags: Real Time, Google APIs, Internet of Things, Stack Network, Real Time, Event-Driven,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/topic/master/_listings/google-cloud-pub-sub/v1topicpublish-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.cloud.prediction.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.cloud.pub.sub.stack.network
- type: x-change-log
  url: https://cloud.google.com/pubsub/docs/release-notes
- type: x-code
  url: https://cloud.google.com/pubsub/docs/reference/libraries
- type: x-faq
  url: https://cloud.google.com/pubsub/docs/faq
- type: x-getting-started
  url: https://cloud.google.com/pubsub/docs/quickstarts
- type: x-guides
  url: https://cloud.google.com/pubsub/docs/how-to
- type: x-issues
  url: https://issuetracker.google.com/issues?q=componentid:187173%20status:open
- type: x-pricing
  url: https://cloud.google.com/pubsub/pricing
- type: x-rate-limits
  url: https://cloud.google.com/pubsub/quotas
- type: x-service-level-agreement
  url: https://cloud.google.com/pubsub/sla
- type: x-support
  url: https://cloud.google.com/pubsub/docs/support
- type: x-website
  url: https://cloud.google.com/pubsub/docs/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---