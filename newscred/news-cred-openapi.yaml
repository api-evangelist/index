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
  articles/:
    get:
      summary: Articles
      description: Returns a list of articles according to the specified set of parameters.
      operationId: getArticles
      x-api-path-slug: articles-get
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
        name: boolean_operator
        description: Indicates the boolean operation to use on search keywords that
          do not have explicit whitelist (+) or blacklist (-) operators on them
      - in: query
        name: categories
        description: Limit items to the categories specified
      - in: query
        name: exact
        description: If this parameter is not specified, then stemming is applied,
          so that for example the query term ship matches articles containing shipping,
          and vice versa
      - in: query
        name: from_date
        description: Beginning of publication date range for which items are searched
      - in: query
        name: get_topics
        description: Set to true to include associated topics inline with each article
      - in: query
        name: has_images
        description: Sort order for returned items
      - in: query
        name: languages
        description: Limit items to those in the specified language
      - in: query
        name: licensed
        description: Search exclusively for fully licensed, full text content
      - in: query
        name: links
        description: Value is a space delimited list of article links
      - in: query
        name: max_length
        description: Returns only articles with at most this many words
      - in: query
        name: media_types
        description: Limit the media type of the returned items
      - in: query
        name: min_length
        description: Returns only articles with at least this many words
      - in: query
        name: mm
        description: 'Minimum Match: specifies how many of the non whitelist/blacklist
          keywords must match for an article to be included in the results'
      - in: query
        name: modified_since
        description: Get only articles that have been modified since the supplied
          date
      - in: query
        name: offset
        description: Number of items to skip before beginning the result set
      - in: query
        name: query
        description: Specifies the set of words and phrases to search for
      - in: query
        name: query_fields
        description: Specifies which field to search when searching for articles
      - in: query
        name: safe_search
        description: Removes articles containing offensive words from search result;
          when set to true
      - in: query
        name: sort
        description: Sort order for returned items
      - in: query
        name: sources
        description: Limit items to the sources specified
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
        name: topics
        description: Value is a space delimited list of topic guids
      - in: query
        name: topic_filter_mode
        description: Enables topic_filter_name and indicates filtering type
      - in: query
        name: topic_filter_name
        description: Limit items to a predefined list of topics
      - in: query
        name: to_date
        description: End of publication date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - News
      - Articles
  author/:
    get:
      summary: Author
      description: Returns an author that has written content available via this API.
      operationId: getAuthor
      x-api-path-slug: author-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      responses:
        200:
          description: OK
      tags:
      - Author
  author/{guid}/articles/:
    get:
      summary: Author Articles
      description: Returns articles written by the specified author and matching the
        given query string.
      operationId: getAuthorGuArticles
      x-api-path-slug: authorguidarticles-get
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
        description: The guid for the author
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
        name: topics
        description: List of topics to retrieve items from
      - in: query
        name: topic_filter_mode
        description: Enables topic_filter_name and indicates filtering type
      - in: query
        name: topic_filter_name
        description: Limit items to a predefined list of topics
      - in: query
        name: to_date
        description: End of date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - News
      - Author
      - Articles
  author/{guid}/topics/:
    get:
      summary: Author Topics
      description: Gets a list of topics related to an author.
      operationId: getAuthorGuTopics
      x-api-path-slug: authorguidtopics-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: from_date
        description: Beginning of date range for which items are searched
      - in: path
        name: guid
        description: The guid for the author
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
      - Author
      - Topics
  categories/:
    get:
      summary: Categories
      description: Search for categories
      operationId: getCategories
      x-api-path-slug: categories-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: autosuggest
        description: If true, partial matches will be returned, i
      - in: query
        name: query
        description: The query string to find categories matching
      responses:
        200:
          description: OK
      tags:
      - News
      - Categories
  category/dashed-name/sources/:
    get:
      summary: Category Sources
      description: Gets a list of sources that write most frequently about the category
        specified by the dashed name
      operationId: getCategoryDashedNameSources
      x-api-path-slug: categorydashednamesources-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: from_date
        description: Beginning of date range for which items are searched
      - in: query
        name: media_types
        description: Space delimited list of media types to retreive articles from
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
      - in: query
        name: to_date
        description: End of date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - News
      - Category
      - Dashed-name
      - Sources
  category/dashed-name/topics/:
    get:
      summary: Category Topics
      description: Gets a list of topics within the category specified by the dashed
        name.
      operationId: getCategoryDashedNameTopics
      x-api-path-slug: categorydashednametopics-get
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
      - Category
      - Dashed-name
      - Topics
  category/{category-name]/stories/:
    get:
      summary: Category Stories
      description: Find the top news stories related to a given category. A story
        is a collection of similar articles.
      operationId: getCategoryCategoryName]Stories
      x-api-path-slug: categorycategorynamestories-get
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
        description: Limit items to those with the specified language
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
        description: Restricts the query to a predefined list of sources
      - in: query
        name: to_date
        description: End of date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - News
      - Category
      - Category-name]
      - Stories
  category/{dashed-name}/articles/:
    get:
      summary: Category Articles
      description: Search for articles within the category specified by dashed name.
      operationId: getCategoryDashedNameArticles
      x-api-path-slug: categorydashednamearticles-get
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
        description: Limit items to those with the specified language
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
        description: Restricts the query to a predefined list of sources
      - in: query
        name: to_date
        description: End of date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - Category
      - Dashed-name
      - Articles
  category/{dashed-name}/images/:
    get:
      summary: Category Images
      description: Gets images related to the specified category.
      operationId: getCategoryDashedNameImages
      x-api-path-slug: categorydashednameimages-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: safe_search
        description: Returns only images marked as safe when set to true
      responses:
        200:
          description: OK
      tags:
      - News
      - Category
      - Dashed-name
      - Images
  image/{guid}/:
    get:
      summary: Image
      description: Returns the image specified by the given GUID.
      operationId: getImageGu
      x-api-path-slug: imageguid-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: path
        name: guid
        description: The guid for the image
      responses:
        200:
          description: OK
      tags:
      - Image
  images/:
    get:
      summary: Search Images
      description: Returns images matched by the query string
      operationId: getImages
      x-api-path-slug: images-get
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
        name: query
        description: Query string you want to search for
      - in: query
        name: to_date
        description: End of date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - Images
  source/:
    get:
      summary: Source
      description: Returns the source represented by the specified GUID.
      operationId: getSource
      x-api-path-slug: source-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: path
        name: GUID
        description: GUID representing news source
      responses:
        200:
          description: OK
      tags:
      - Source
  source/{GUID}/articles/:
    get:
      summary: Source Articles
      description: Returns a list of articles provided by the specified source
      operationId: getSourceGuArticles
      x-api-path-slug: sourceguidarticles-get
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
        name: topics
        description: List of topics to retrieve items from
      - in: query
        name: topic_filter_mode
        description: Enables topic_filter_name and indicates filtering type
      - in: query
        name: topic_filter_name
        description: Limit items to a predefined list of topics
      - in: query
        name: to_date
        description: End of date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - News
      - Source
      - GUID
      - Articles
  source/{GUID}/topics/:
    get:
      summary: Source Topics
      description: Returns a list of topics related to the source specified by the
        given GUID.
      operationId: getSourceGuTopics
      x-api-path-slug: sourceguidtopics-get
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
      - Source
      - GUID
      - Topics
  sources/:
    get:
      summary: Sources
      description: Search sources by name. Returns a list of sources objects
      operationId: getSources
      x-api-path-slug: sources-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: autosuggest
        description: If true, partial matches will be returned starting from 3 characters,
          i
      - in: query
        name: licensed
        description: If true, return only licensed sources with fully licensed content
      - in: query
        name: media_types
        description: Limit the media type of the returned items
      - in: query
        name: query
        description: Query string to search on
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
      responses:
        200:
          description: OK
      tags:
      - News
      - Sources
  stories/:
    get:
      summary: Stories
      description: Returns the top stories related to the specified query. A story
        is a group of similar articles. By default, stories are sorted by a combination
        of recency and importance. If the from_date and/or to_date parameters are
        specified, stories are sorted by importance only.
      operationId: getStories
      x-api-path-slug: stories-get
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
        name: boolean_operator
        description: Indicates the boolean operation to use on search keywords that
          do not have explicit whitelist (+) or blacklist (-) operators on them
      - in: query
        name: categories
        description: Limit items to the categories specified
      - in: query
        name: cluster_size
        description: Number of articles returned for each story
      - in: query
        name: exact
        description: If this parameter is not specified, then stemming is applied,
          so that for example the query term ship matches articles containing shipping,
          and vice versa
      - in: query
        name: from_date
        description: Beginning of publication date range for which items are searched
      - in: query
        name: get_topics
        description: Set to true to include associated topics inline with each article
      - in: query
        name: has_images
        description: Sort order for returned items
      - in: query
        name: languages
        description: Limit items to those in the specified language
      - in: query
        name: licensed
        description: Search exclusively for fully licensed, full text content
      - in: query
        name: links
        description: Value is a space delimited list of article links
      - in: query
        name: max_length
        description: Returns only articles with at most this many words
      - in: query
        name: media_types
        description: Limit the media type of the returned items
      - in: query
        name: min_length
        description: Returns only articles with at least this many words
      - in: query
        name: mm
        description: 'Minimum Match: specifies how many of the non whitelist/blacklist
          keywords must match for an article to be included in the results'
      - in: query
        name: modified_since
        description: Get only articles that have been modified since the supplied
          date
      - in: query
        name: offset
        description: Number of items to skip before beginning the result set
      - in: query
        name: query
        description: Specifies the set of words and phrases to search for
      - in: query
        name: query_fields
        description: Specifies which field to search when searching for articles
      - in: query
        name: safe_search
        description: Removes articles containing offensive words from search result;
          when set to true
      - in: query
        name: sort
        description: Sort order for returned items
      - in: query
        name: sources
        description: Limit items to the sources specified
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
        name: topics
        description: Value is a space delimited list of topic guids
      - in: query
        name: topic_filter_mode
        description: Enables topic_filter_name and indicates filtering type
      - in: query
        name: topic_filter_name
        description: Limit items to a predefined list of topics
      - in: query
        name: to_date
        description: End of publication date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - News
      - Stories
  topic/{guide{/images/:
    get:
      summary: Topic Images
      description: Returns images related to the specified topic.
      operationId: getTopicGueImages
      x-api-path-slug: topicguideimages-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: path
        name: guid
        description: The topic guid
      responses:
        200:
          description: OK
      tags:
      - News
      - Topice
      - Images
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
  topics/:
    get:
      summary: Search Topics
      description: Search for a specific topics.
      operationId: getTopics
      x-api-path-slug: topics-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: exact
        description: If true, the topic name must match the query exactly
      - in: query
        name: query
        description: The query string to find topics for
      responses:
        200:
          description: OK
      tags:
      - News
      - Topics
  topics/extract/:
    get:
      summary: Extract Related Topics
      description: Returns a list of topics extracted from the input query.
      operationId: getTopicsExtract
      x-api-path-slug: topicsextract-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: query
        description: The string to extract topics from
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
      responses:
        200:
          description: OK
      tags:
      - News
      - Topics
      - Extract
  topics/related/:
    get:
      summary: Related Topics
      description: Given some search criteria, returns a list of topics related to
        those criteria.
      operationId: getTopicsRelated
      x-api-path-slug: topicsrelated-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: from_date, to_date
        description: Find topics that were trending (written about more than usual)
          during the specified date range
      - in: query
        name: offset
        description: Number of topics to skip before beginning the result set
      - in: query
        name: pagesize
        description: Number of topics to return
      - in: query
        name: query
        description: Find topics related to these keywords
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
      responses:
        200:
          description: OK
      tags:
      - News
      - Topics
      - Related
  videos/:
    get:
      summary: Videos
      description: Returns videos matching the given query string
      operationId: getVeos
      x-api-path-slug: videos-get
      parameters:
      - in: query
        name: from_date
        description: Beginning of date range for which items are searched
      - in: query
        name: licensed
        description: Return only licensed videos
      - in: query
        name: maxduration
        description: Maximum duration for searched videos (in milliseconds)
      - in: query
        name: minduration
        description: Minimum duration for searched videos (in milliseconds)
      - in: query
        name: offset
        description: Number of items to skip before beginning the result set
      - in: query
        name: pagesize
        description: Number of items to return
      - in: query
        name: query
        description: Query that you want to search on
      - in: query
        name: to_date
        description: End of date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - News
      - Videos