---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Statistics Get Latest Topic Data
  description: Get lastest value for a topic.
  version: 1.0.0
host: www.xignite.com
basePath: xStatistics.json/XigniteStatistics
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetTopicDetails:
    get:
      summary: Get Topic Details
      description: ""
      operationId: postGettopicdetails
      x-api-path-slug: gettopicdetails-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Topic
      - Details
  /GetTopicStatistics:
    get:
      summary: Get Topic Statistics
      description: Get statistics for a topic and a period.
      operationId: postGettopicstatistics
      x-api-path-slug: gettopicstatistics-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Topic
      - Statistics
  /GetTopicData:
    get:
      summary: Get Topic Data
      description: Get time-series data for a topic.
      operationId: postGettopicdata
      x-api-path-slug: gettopicdata-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Topic
      - Data
  /GetLatestTopicData:
    get:
      summary: Get Latest Topic Data
      description: Get lastest value for a topic.
      operationId: postGetlatesttopicdata
      x-api-path-slug: getlatesttopicdata-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Latest
      - Topic
      - Data
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