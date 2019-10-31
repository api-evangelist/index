swagger: "2.0"
x-collection-name: Vestorly
x-complete: 1
info:
  title: Vestorly
  description: vestorly-developers-api
  termsOfService: http://www.vestorly.com/terms/
  contact:
    name: Vestorly Team
  version: 1.0.0
host: staging.vestorly.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /advisors/{id}:
    get:
      summary: Get Advisors
      description: Returns a single advisor given their ID
      operationId: findAdvisorByID
      x-api-path-slug: advisorsid-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: Advisor Id to fetch
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Advisors
  /articles:
    get:
      summary: Get Articles
      description: Returns all articles
      operationId: findArticles
      x-api-path-slug: articles-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: limit
        description: Limit on the number of articles to return
      - in: query
        name: sort_by
        description: Field on model to sort by
      - in: query
        name: sort_direction
        description: Direction of sort (used with sort_by parameter)
      - in: query
        name: text_query
        description: Search query parameter
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Articles
  /articles/{id}:
    get:
      summary: Get Articles
      description: Returns a single article
      operationId: findArticleByID
      x-api-path-slug: articlesid-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: Article Id to fetch
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Articles
  /events:
    get:
      summary: Get Events
      description: Returns all events
      operationId: findEvents
      x-api-path-slug: events-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Events
    post:
      summary: Post Events
      description: Creates a new event in the system
      operationId: createEvent
      x-api-path-slug: events-post
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: body
        name: event
        description: Event
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Events
  /events/{id}:
    get:
      summary: Get Events
      description: Returns a single event if the user has access
      operationId: findEventByID
      x-api-path-slug: eventsid-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: Mongo ID of event to fetch
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Events
  /groups:
    get:
      summary: Get Groups
      description: Returns all groups
      operationId: findGroups
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Groups
    post:
      summary: Post Groups
      description: Creates a new Group
      operationId: createGroup
      x-api-path-slug: groups-post
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: body
        name: group
        description: Group to add
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Groups
  /groups/{id}:
    delete:
      summary: Delete Groups
      description: Deletes a Group
      operationId: deleteGroup
      x-api-path-slug: groupsid-delete
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: id of group to delete
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Groups
    get:
      summary: Get Groups
      description: Returns a single group if user has access
      operationId: findGroupByID
      x-api-path-slug: groupsid-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: Mongo ID of group to fetch
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Groups
    put:
      summary: Put Groups
      description: Updates a Group
      operationId: updateGroupById
      x-api-path-slug: groupsid-put
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: body
        name: group
        description: Group to update
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: id of group to update
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Groups
  /member_events:
    get:
      summary: Get Member Events
      description: Returns all MemberEvents
      operationId: findMemberEvents
      x-api-path-slug: member-events-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Member
      - Events
  /member_reports:
    get:
      summary: Get Member Reports
      description: Returns all member reports
      operationId: findMemberReports
      x-api-path-slug: member-reports-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Member
      - Reports
  /members:
    get:
      summary: Get Members
      description: Returns all members
      operationId: findMembers
      x-api-path-slug: members-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: limit
        description: Number of members to return
      - in: query
        name: start
        description: Skips number of members from start
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Members
    post:
      summary: Post Members
      description: Create a new member in the Vestorly Platform
      operationId: createMember
      x-api-path-slug: members-post
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: body
        name: member
        description: Member you want to create
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Members
  /members/{id}:
    get:
      summary: Get Members
      description: Returns a single member
      operationId: findMemberByID
      x-api-path-slug: membersid-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: Mongo ID of member to fetch
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Members
    put:
      summary: Put Members
      description: Updates a single member
      operationId: updateMemberByID
      x-api-path-slug: membersid-put
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: Mongo ID of member to fetch
      - in: body
        name: member
        description: Member you want to update
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Members
  /newsletter_settings:
    get:
      summary: Get Newsletter Settings
      description: Returns all newsletter settings
      operationId: findNewsletterSettings
      x-api-path-slug: newsletter-settings-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Newsletter
      - Settings
  /newsletter_settings/{id}:
    get:
      summary: Get Newsletter Settings
      description: Returns a single newsletter settings if the user has access
      operationId: findNewsletterSettingsByID
      x-api-path-slug: newsletter-settingsid-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: Mongo ID of newsletter settings to fetch
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Newsletter
      - Settings
    put:
      summary: Put Newsletter Settings
      description: Update a single newsletter setting by ID
      operationId: updateNewsletterSettingsByID
      x-api-path-slug: newsletter-settingsid-put
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: Mongo ID of newsletter settings to update
      - in: body
        name: newsletter_setting
        description: newsletter settings
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Newsletter
      - Settings
  /newsletters:
    get:
      summary: Get Newsletters
      description: Returns all newsletters
      operationId: findNewsletters
      x-api-path-slug: newsletters-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Newsletters
  /newsletters/{id}:
    get:
      summary: Get Newsletters
      description: Get a newsletter by ID
      operationId: getNewsletterByID
      x-api-path-slug: newslettersid-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: Mongo ID of event to get
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Newsletters
    put:
      summary: Put Newsletters
      description: Updates a newsletter
      operationId: updateNewsletterByID
      x-api-path-slug: newslettersid-put
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: Mongo ID of event to update
      - in: body
        name: newsletter
        description: Newsletter
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Newsletters
  /posts:
    get:
      summary: Get Posts
      description: Query all posts
      operationId: findPosts
      x-api-path-slug: posts-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: external_url
        description: Filter by External URL
      - in: query
        name: is_published
        description: Filter by is_published boolean
      - in: query
        name: text_query
        description: Filter post by parameters
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Posts
    post:
      summary: Add Post
      description: Create a new post in the Vestorly Platform
      operationId: createPost
      x-api-path-slug: posts-post
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: body
        name: post
        description: Post you want to create
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/{id}:
    get:
      summary: Get Post
      description: Query all posts
      operationId: getPostByID
      x-api-path-slug: postsid-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: ID of post to fetch
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Posts
    put:
      summary: Update Post
      description: Update A Post
      operationId: updatePostByID
      x-api-path-slug: postsid-put
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: id of post to update
      - in: body
        name: post
        description: Post you want to update
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - S
  /sessions:
    post:
      summary: Post Sessions
      description: Login To Vestorly Platform
      operationId: login
      x-api-path-slug: sessions-post
      parameters:
      - in: query
        name: password
        description: Password in Vestorly Platform
      - in: query
        name: username
        description: Username in the vestorly platform
      responses:
        200:
          description: OK
      tags:
      - Sessions
  /sessions/{id}:
    delete:
      summary: Delete Sessions
      description: Logout of the vestorly platform
      operationId: logout
      x-api-path-slug: sessionsid-delete
      parameters:
      - in: path
        name: id
        description: ID of pet to session
      - in: query
        name: vestorly-auth
        description: Authenication token
      - in: query
        name: vestorly_auth
        description: Authenication token
      responses:
        200:
          description: OK
      tags:
      - Sessions
  /sources:
    get:
      summary: Get Sources
      description: Returns all sources
      operationId: findSources
      x-api-path-slug: sources-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Sources
    post:
      summary: Post Sources
      description: Create source
      operationId: createSource
      x-api-path-slug: sources-post
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: body
        name: source
        description: Source
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Sources
  /sources/{id}:
    get:
      summary: Get Sources
      description: Get Source By ID
      operationId: getSourceByID
      x-api-path-slug: sourcesid-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: ID of source to fetch
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Sources
    put:
      summary: Put Sources
      description: Update Source By ID
      operationId: updateSourceByID
      x-api-path-slug: sourcesid-put
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: ID of source to fetch
      - in: body
        name: source
        description: Source
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Sources