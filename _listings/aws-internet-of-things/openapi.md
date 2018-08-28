swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 1
info:
  title: AWS Internet of Things API
  version: 1.0.0
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
  /?Action=ListTopicRules:
    get:
      summary: List Topic Rules
      description: Lists the rules for the specific topic.
      operationId: listTopicRules
      x-api-path-slug: actionlisttopicrules-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of results to return
        type: string
      - in: query
        name: nextToken
        description: A token used to retrieve the next value
        type: string
      - in: query
        name: ruleDisabled
        description: Specifies whether the rule is disabled
        type: string
      - in: query
        name: topic
        description: The topic
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topic Rules
  /?Action=ReplaceTopicRule:
    get:
      summary: Replace Topic Rule
      description: Replaces the specified rule.
      operationId: replaceTopicRule
      x-api-path-slug: actionreplacetopicrule-get
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