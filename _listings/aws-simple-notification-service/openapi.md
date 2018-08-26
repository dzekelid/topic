---
swagger: "2.0"
x-collection-name: AWS Simple Notification Service
x-complete: 1
info:
  title: AWS Simple Notification Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateTopic:
    get:
      summary: Create Topic
      description: Creates a topic to which notifications can be published.
      operationId: createTopic
      x-api-path-slug: actioncreatetopic-get
      parameters:
      - in: query
        name: Name
        description: The name of the topic you want to create
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topics
  /?Action=DeleteTopic:
    get:
      summary: Delete Topic
      description: Deletes a topic and all its subscriptions.
      operationId: deleteTopic
      x-api-path-slug: actiondeletetopic-get
      parameters:
      - in: query
        name: TopicArn
        description: The ARN of the topic you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topics
  /?Action=GetTopicAttributes:
    get:
      summary: Get Topic Attributes
      description: Returns all of the properties of a topic.
      operationId: getTopicAttributes
      x-api-path-slug: actiongettopicattributes-get
      parameters:
      - in: query
        name: TopicArn
        description: The ARN of the topic whose properties you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topics
  /?Action=ListSubscriptionsByTopic:
    get:
      summary: List Subscriptions By Topic
      description: Returns a list of the subscriptions to a specific topic.
      operationId: listSubscriptionsByTopic
      x-api-path-slug: actionlistsubscriptionsbytopic-get
      parameters:
      - in: query
        name: NextToken
        description: Token returned by the previous ListSubscriptionsByTopic request
        type: string
      - in: query
        name: TopicArn
        description: The ARN of the topic for which you wish to find subscriptions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=ListTopics:
    get:
      summary: List Topics
      description: Returns a list of the requester's topics.
      operationId: listTopics
      x-api-path-slug: actionlisttopics-get
      parameters:
      - in: query
        name: NextToken
        description: Token returned by the previous ListTopics request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topics
  /?Action=SetTopicAttributes:
    get:
      summary: Set Topic Attributes
      description: Allows a topic owner to set an attribute of the topic to a new
        value.
      operationId: setTopicAttributes
      x-api-path-slug: actionsettopicattributes-get
      parameters:
      - in: query
        name: AttributeName
        description: The name of the attribute you want to set
        type: string
      - in: query
        name: AttributeValue
        description: The new value for the attribute
        type: string
      - in: query
        name: TopicArn
        description: The ARN of the topic to modify
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topics
---