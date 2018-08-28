---
swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 0
info:
  title: AWS Internet of Things API Get Topic Rule
  version: 1.0.0
  description: Gets information about the specified rule.
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
  /?Action=DeleteTopicRule:
    get:
      summary: Delete Topic Rule
      description: Deletes the specified rule.
      operationId: deleteTopicRule
      x-api-path-slug: actiondeletetopicrule-get
      parameters:
      - in: query
        name: ruleName
        description: The name of the rule
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topic Rules
  /?Action=DisableTopicRule:
    get:
      summary: Disable Topic Rule
      description: Disables the specified rule.
      operationId: disableTopicRule
      x-api-path-slug: actiondisabletopicrule-get
      parameters:
      - in: query
        name: ruleName
        description: The name of the rule to disable
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topic Rules
  /?Action=EnableTopicRule:
    get:
      summary: Enable Topic Rule
      description: Enables the specified rule.
      operationId: enableTopicRule
      x-api-path-slug: actionenabletopicrule-get
      parameters:
      - in: query
        name: ruleName
        description: The name of the topic rule to enable
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topic Rules
  /?Action=GetTopicRule:
    get:
      summary: Get Topic Rule
      description: Gets information about the specified rule.
      operationId: getTopicRule
      x-api-path-slug: actiongettopicrule-get
      parameters:
      - in: query
        name: ruleName
        description: The name of the rule
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