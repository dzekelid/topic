---
swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 0
info:
  title: AWS Internet of Things API Create Topic Rule
  version: 1.0.0
  description: Creates a rule.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateTopicRule:
    get:
      summary: Create Topic Rule
      description: Creates a rule.
      operationId: createTopicRule
      x-api-path-slug: actioncreatetopicrule-get
      parameters:
      - in: query
        name: ruleName
        description: The name of the rule
        type: string
      - in: query
        name: topicRulePayload
        description: The rule payload
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topic Rules
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