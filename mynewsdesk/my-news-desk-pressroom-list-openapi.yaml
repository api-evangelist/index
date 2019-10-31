swagger: "2.0"
x-collection-name: Mynewsdesk
x-complete: 1
info:
  title: My News Desk Pressroom List
  description: mynewsdesk-webservice-for-newsroom-is-a-way-for-you-as-a-registered-customer-to-fetch-information-from-your-newsroom-at-mynewsdesk-to-any-system--you-can-get-all-your-information-as-xml-and-create-email-subscriptions-to-your-material-
  termsOfService: http://www.mynewsdesk.com/about/terms-and-conditions?locale=en
  version: v1
host: www.mynewsdesk.com
basePath: /services/pressroom/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  create_comment/:
    get:
      summary: Create Comment
      description: Create Comment
      operationId: getCreateComment
      x-api-path-slug: create-comment-get
      parameters:
      - in: query
        name: blog
        description: URL of commenters blog/website
      - in: query
        name: body
        description: Content of comment
      - in: query
        name: commentable_id
        description: ID of the material that is commented
      - in: query
        name: email
        description: Email address of commenter
      - in: query
        name: name
        description: Name of commenter
      - in: query
        name: type_of_media
        description: Type of material
      - in: path
        name: unique key
        description: The MyNewsDesk API Key
      - in: query
        name: user_ip
        description: IP number of commenter
      responses:
        200:
          description: OK
      tags:
      - Comment
  list/:
    get:
      summary: Lists news
      description: Lists news
      operationId: getList
      x-api-path-slug: list-get
      parameters:
      - in: query
        name: archived
        description: Fetch items marked as archived, this is useful for fetching old
          events
      - in: query
        name: callback
        description: If format is JSON and callback is specified, the JSON response
          is wrapped in a function call with the specified callback name
      - in: query
        name: format
        description: 'Specify the format of the response: RSS 2'
      - in: query
        name: limit
        description: Set the maximum number of items in the response
      - in: query
        name: offset
        description: Specify which item (sequentially) should be first, skipping preceding
          items
      - in: query
        name: order
        description: 'Specify the sort order of the result: publish date (published),
          latest update (updated) or creation date (created)'
      - in: query
        name: pressroom
        description: Set the pressroom to fetch material from
      - in: query
        name: type_of_media
        description: Fetch material of this type only
      - in: path
        name: unique key
        description: The MyNewsDesk API Key
      responses:
        200:
          description: OK
      tags:
      - News
  pressroom_info/:
    get:
      summary: Pressroom Info
      description: Pressroom Info
      operationId: getPressroomInfo
      x-api-path-slug: pressroom-info-get
      parameters:
      - in: query
        name: pressroom
        description: Set the pressroom to search in
      - in: path
        name: unique key
        description: The MyNewsDesk API Key
      responses:
        200:
          description: OK
      tags:
      - News
      - Pressroom
      - Info
  search/:
    get:
      summary: News Search
      description: News Search
      operationId: getSearch
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: callback
        description: If format is JSON and callback is specified, the JSON response
          is wrapped in a function call with the specified callback name
      - in: query
        name: date_end
        description: End date
      - in: query
        name: date_mode
        description: Specifies how the date parameters are used
      - in: query
        name: date_on
        description: Date
      - in: query
        name: date_start
        description: Start date
      - in: query
        name: format
        description: 'Specify the format of the response: RSS 2'
      - in: query
        name: limit
        description: Set the maximum number of items in the response
      - in: query
        name: page
        description: Page number in the search result
      - in: query
        name: pressroom
        description: Set the pressroom to search in
      - in: query
        name: query
        description: Search string
      - in: query
        name: type_of_media
        description: The type of material to be fetched
      - in: path
        name: unique key
        description: The MyNewsDesk API Key
      responses:
        200:
          description: OK
      tags:
      - News
      - Search
  send_email/:
    get:
      summary: Send Email
      description: Send Email
      operationId: getSendEmail
      x-api-path-slug: send-email-get
      parameters:
      - in: query
        name: from
        description: Name of sender
      - in: query
        name: item_id
        description: ID of the material to be fetched
      - in: query
        name: message
        description: Personal message from the sender to the recipient
      - in: query
        name: to_email
        description: Recipient email address
      - in: query
        name: type_of_media
        description: The type of material to be fetched
      - in: path
        name: unique key
        description: The MyNewsDesk API Key
      responses:
        200:
          description: OK
      tags:
      - Send
      - Email
  subscription/:
    get:
      summary: News Subscription
      description: News Subscription
      operationId: getSubscription
      x-api-path-slug: subscription-get
      parameters:
      - in: query
        name: newsdesk_pressroom
        description: Set the pressroom to search in
      - in: query
        name: newsdesk_subscriber_email
        description: Email address of the subscriber
      - in: query
        name: newsdesk_subscribe_to_type
        description: Send a parameter with the value 1 for each type of material to
          be included in the subscription
      - in: query
        name: unique key
        description: The MyNewsDesk API Key
      responses:
        200:
          description: OK
      tags:
      - News
      - Subscription
  view/:
    get:
      summary: View News
      description: View News
      operationId: getView
      x-api-path-slug: view-get
      parameters:
      - in: query
        name: callback
        description: If format is JSON and callback is specified, the JSON response
          is wrapped in a function call with the specified callback name
      - in: query
        name: format
        description: 'Specify the format of the response: JSON or full XML'
      - in: query
        name: item_id
        description: ID of the material to be fetched
      - in: query
        name: type_of_media
        description: The type of material to be fetched
      - in: path
        name: unique key
        description: The MyNewsDesk API Key
      responses:
        200:
          description: OK
      tags:
      - View
      - News