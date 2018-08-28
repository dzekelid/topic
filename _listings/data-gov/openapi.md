swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 1
info:
  title: Data.gov API
  description: the-data-gov-catalog-is-powered-by-ckan-a-powerful-open-source-data-platform-that-includes-a-robust-api--please-be-aware-that-data-gov-and-the-data-gov-ckan-api-only-contain-metadata-about-datasets--this-metadata-includes-urls-and-descriptions-of-datasets-but-it-does-not-include-the-actual-data-within-each-dataset-
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
    put:
      summary: Put Topics Topic
      description: Update a given topic
      operationId: putTopicsTopic
      x-api-path-slug: topicstopic-put
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: topic
        description: The topic ID or slug
      responses:
        200:
          description: OK
      tags:
      - Topics
      - Topic