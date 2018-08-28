---
swagger: "2.0"
x-collection-name: Google Cloud Pub Sub
x-complete: 0
info:
  title: Google Cloud Pub/Sub API Publish Topic
  description: |-
    Adds one or more messages to the topic. Returns `NOT_FOUND` if the topic
    does not exist. The message payload must not be empty; it must contain
     either a non-empty data field, or at least one attribute.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: pubsub.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:
    put:
      summary: Create Topic
      description: Creates the given topic with the given name.
      operationId: pubsub.projects.topics.create
      x-api-path-slug: v1name-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The name of the topic
      responses:
        200:
          description: OK
      tags:
      - Topic
  /v1/{project}/topics:
    get:
      summary: List Matching Topics
      description: Lists matching topics.
      operationId: pubsub.projects.topics.list
      x-api-path-slug: v1projecttopics-get
      parameters:
      - in: query
        name: pageSize
        description: Maximum number of topics to return
      - in: query
        name: pageToken
        description: The value returned by the last `ListTopicsResponse`; indicates
          that this isa continuation of a prior `ListTopics` call, and that the system
          shouldreturn the next page of data
      - in: path
        name: project
        description: The name of the cloud project that topics belong to
      responses:
        200:
          description: OK
      tags:
      - Topic
  /v1/{topic}:
    delete:
      summary: Delete Topic
      description: |-
        Deletes the topic with the given name. Returns `NOT_FOUND` if the topic
        does not exist. After a topic is deleted, a new topic may be created with
        the same name; this is an entirely new topic with none of the old
        configuration or subscriptions. Existing subscriptions to this topic are
        not deleted, but their `topic` field is set to `_deleted-topic_`.
      operationId: pubsub.projects.topics.delete
      x-api-path-slug: v1topic-delete
      parameters:
      - in: path
        name: topic
        description: Name of the topic to delete
      responses:
        200:
          description: OK
      tags:
      - Topic
    get:
      summary: Get Topic Configuration
      description: Gets the configuration of a topic.
      operationId: pubsub.projects.topics.get
      x-api-path-slug: v1topic-get
      parameters:
      - in: path
        name: topic
        description: The name of the topic to get
      responses:
        200:
          description: OK
      tags:
      - Topic
  /v1/{topic}/subscriptions:
    get:
      summary: Get Topic Subscription
      description: Lists the name of the subscriptions for this topic.
      operationId: pubsub.projects.topics.subscriptions.list
      x-api-path-slug: v1topicsubscriptions-get
      parameters:
      - in: query
        name: pageSize
        description: Maximum number of subscription names to return
      - in: query
        name: pageToken
        description: The value returned by the last `ListTopicSubscriptionsResponse`;
          indicatesthat this is a continuation of a prior `ListTopicSubscriptions`
          call, andthat the system should return the next page of data
      - in: path
        name: topic
        description: The name of the topic that subscriptions are attached to
      responses:
        200:
          description: OK
      tags:
      - Topic
  /v1/{topic}:publish:
    post:
      summary: Publish Topic
      description: |-
        Adds one or more messages to the topic. Returns `NOT_FOUND` if the topic
        does not exist. The message payload must not be empty; it must contain
         either a non-empty data field, or at least one attribute.
      operationId: pubsub.projects.topics.publish
      x-api-path-slug: v1topicpublish-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: topic
        description: The messages in the request will be published on this topic
      responses:
        200:
          description: OK
      tags:
      - Topic
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