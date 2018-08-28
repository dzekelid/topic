swagger: "2.0"
x-collection-name: NewsCred
x-complete: 1
info:
  title: News Cred
  description: returns-a-list-of-articles-according-to-the-specified-set-of-parameters-
  version: v1
host: api.newscred.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /topic/{guid]/articles/:
    get:
      summary: Topic Articles
      description: Returns a list of articles related to the specified topic.
      operationId: getTopicGu]Articles
      x-api-path-slug: topicguidarticles-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: article_filter_mode
        description: Enables article_filter_name and indicates filtering type
      - in: query
        name: article_filter_name
        description: Limit items to a predefined list of articles
      - in: query
        name: categories
        description: Limit items to the categories specified
      - in: query
        name: from_date
        description: Beginning of date range for which items are searched
      - in: query
        name: get_topics
        description: Set to true to include associated topics inline with each article
      - in: path
        name: guid
        description: The topic guid
      - in: query
        name: has_images
        description: Return only articles that have associated images (accessible
          via article/GUID/images)
      - in: query
        name: languages
        description: Limit items to those in the specified language
      - in: query
        name: licensed
        description: Search exclusively for fully licensed, full text content
      - in: query
        name: media_types
        description: Limit the media type of the returned items
      - in: query
        name: offset
        description: Number of items to skip before beginning the result set
      - in: query
        name: pagesize
        description: Number of items to return
      - in: query
        name: sort
        description: Sort order for returned items
      - in: query
        name: sources
        description: List of sources to retrieve items from
      - in: query
        name: source_countries
        description: Search against only sources from the specified countries
      - in: query
        name: source_filter_mode
        description: Enables source_filter_name and indicates filtering type
      - in: query
        name: source_filter_name
        description: Limit items to a predefined list of sources
      - in: query
        name: to_date
        description: End of date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - News
      - Topic
      - Articles
  topic/{guid}/:
    get:
      summary: Topic
      description: Return the topic specified by the given GUID.
      operationId: getTopicGu
      x-api-path-slug: topicguid-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      responses:
        200:
          description: OK
      tags:
      - News
      - Topic
  topic/{guid}/sources/:
    get:
      summary: Topic Sources
      description: The guid for the topic.
      operationId: getTopicGuSources
      x-api-path-slug: topicguidsources-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: from_date
        description: Beginning of date range for which items are searched
      - in: query
        name: offset
        description: Number of items to skip before beginning the result set
      - in: query
        name: pagesize
        description: Number of items to return
      - in: query
        name: sources
        description: List of sources to retrieve items from
      - in: query
        name: source_countries
        description: Search against only sources from the specified countries
      - in: query
        name: source_filter_mode
        description: Enables source_filter_name and indicates filtering type
      - in: query
        name: source_filter_name
        description: Limit items to a predefined list of sources
      - in: path
        name: Topic Sources
        description: The guid for the topic
      - in: query
        name: to_date
        description: End of date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - News
      - Topic
      - Sources
  topic/{guid}/topics/:
    get:
      summary: Related Topics
      description: Returns a list of topics related to the topic specified.
      operationId: getTopicGuTopics
      x-api-path-slug: topicguidtopics-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: from_date
        description: Beginning of date range for which items are searched
      - in: query
        name: guid
        description: The guid for the topic
      - in: query
        name: offset
        description: Number of items to skip before beginning the result set
      - in: query
        name: pagesize
        description: Number of items to return
      - in: query
        name: topics
        description: List of topics to retrieve items from
      - in: query
        name: topic_classifications
        description: Limit results to those with the specified topic classification
      - in: query
        name: topic_filter_mode
        description: Enables topic_filter_name and indicates filtering type
      - in: query
        name: topic_filter_name
        description: Limit items to a predefined list of topics
      - in: query
        name: topic_subclassifications
        description: Limit results to those with the specified topic sub-classification
      - in: query
        name: to_date
        description: End of date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - News
      - Topic
      - Topics
  topic/{guid}/tweets/:
    get:
      summary: Related Tweets
      description: Returns a list of real-time tweets related to the specified topic.
      operationId: getTopicGuTweets
      x-api-path-slug: topicguidtweets-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: path
        name: guid
        description: The guid for the topic
      - in: query
        name: offset
        description: Number of tweets to skip before beginning the result set
      - in: query
        name: pagesize
        description: Number of tweets to return
      responses:
        200:
          description: OK
      tags:
      - News
      - Topic
      - Tweets
  topic/{guid}/videos/:
    get:
      summary: Topic Videos
      description: Returns a list of videos related to the specified topic.
      operationId: getTopicGuVeos
      x-api-path-slug: topicguidvideos-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: categories
        description: Limit videos to the categories specified
      - in: path
        name: guid
        description: The guid for the topic
      - in: query
        name: offset
        description: Number of videos to skip before beginning the result set
      - in: query
        name: pagesize
        description: Number of videos to return
      responses:
        200:
          description: OK
      tags:
      - News
      - Topic
      - Videos
  topic/{topic_guid}/stories/:
    get:
      summary: Topic Stories
      description: Find the top stories that are happening for a given topic. A story
        is a collection of similar articles.
      operationId: getTopicTopicGuStories
      x-api-path-slug: topictopic-guidstories-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: article_filter_mode
        description: Enables article_filter_name and indicates filtering type
      - in: query
        name: article_filter_name
        description: Limit items to a predefined list of articles
      - in: query
        name: categories
        description: Limit items to the categories specified
      - in: query
        name: cluster_size
        description: Number of articles returned for each story
      - in: query
        name: from_date
        description: Beginning of date range for which items are searched
      - in: query
        name: get_topics
        description: Set to true to include associated topics inline with each article
      - in: query
        name: has_images
        description: Return only articles that have associated images (accessible
          via article/GUID/images)
      - in: query
        name: languages
        description: Limit items to those in the specified language
      - in: query
        name: licensed
        description: Search exclusively for fully licensed, full text content
      - in: query
        name: media_types
        description: Limit the media type of the returned items
      - in: query
        name: offset
        description: Number of items to skip before beginning the result set
      - in: query
        name: pagesize
        description: Number of items to return
      - in: query
        name: sources
        description: List of sources to retrieve items from
      - in: query
        name: source_countries
        description: Search against only sources from the specified countries
      - in: query
        name: source_filter_mode
        description: Enables source_filter_name and indicates filtering type
      - in: query
        name: source_filter_name
        description: Limit items to a predefined list of sources
      - in: path
        name: topic_guid
        description: The topic guid
      - in: query
        name: to_date
        description: End of date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - News
      - Topic
      - Topic
      - Stories