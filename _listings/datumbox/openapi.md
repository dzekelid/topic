swagger: "2.0"
x-collection-name: Datumbox
x-complete: 1
info:
  title: DatumBox
  description: datumbox-offers-a-machine-learning-platform-composed-of-14-classifiers-and-natural-language-processing-functions--functions-include-sentiment-analysis-topic-classification-readability-assessment-language-detection-and-much-more-
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