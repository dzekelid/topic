swagger: "2.0"
x-collection-name: AWS Simple Email Service
x-complete: 1
info:
  title: AWS Simple Email Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SetIdentityNotificationTopic:
    get:
      summary: Set Identity Notification Topic
      description: |-
        Given an identity (an email address or a domain), sets the Amazon Simple Notification Service (Amazon SNS) topic to which Amazon SES will publish
                bounce, complaint, and/or delivery notifications for emails sent with that identity as the Source.
      operationId: setIdentityNotificationTopic
      x-api-path-slug: actionsetidentitynotificationtopic-get
      parameters:
      - in: query
        name: Identity
        description: The identity for which the Amazon SNS topic will be set
        type: string
      - in: query
        name: NotificationType
        description: The type of notifications that will be published to the specified
          Amazon SNS topic
        type: string
      - in: query
        name: SnsTopic
        description: The Amazon Resource Name (ARN) of the Amazon SNS topic
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity