---
swagger: "2.0"
x-collection-name: Datumbox
x-complete: 0
info:
  title: Datumbox Identifies the Topic of the Document
  description: The Topic Classification function assigns documents in 12 thematic
    categories based on their keywords, idioms and jargon. It can be used to identify
    the topic of the texts.
  version: 1.0.0
host: api.datumbox.com
basePath: 1.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /TopicClassification.json:
    post:
      summary: Identifies the Topic of the Document
      description: The Topic Classification function assigns documents in 12 thematic
        categories based on their keywords, idioms and jargon. It can be used to identify
        the topic of the texts.
      operationId: TopicClassification
      x-api-path-slug: topicclassification-json-post
      parameters:
      - in: formData
        name: text
        description: The text that you want to analyze
      responses:
        200:
          description: OK
      tags:
      - Topic
      - Classification
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