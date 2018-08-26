---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Get Topics Topic
  description: Get a given topic
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /topics/{topic}/:
    delete:
      summary: Delete Topics Topic
      description: Delete a given topic
      operationId: deleteTopicsTopic
      x-api-path-slug: topicstopic-delete
      parameters:
      - in: path
        name: topic
        description: The topic ID or slug
      responses:
        200:
          description: OK
      tags:
      - Topics
      - Topic
    get:
      summary: Get Topics Topic
      description: Get a given topic
      operationId: getTopicsTopic
      x-api-path-slug: topicstopic-get
      parameters:
      - in: path
        name: topic
        description: The topic ID or slug
      responses:
        200:
          description: OK
      tags:
      - Topics
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