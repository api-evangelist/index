swagger: "2.0"
x-collection-name: Pinboard
x-complete: 1
info:
  title: Pinboard
  description: store-manage-and-share-bookmarks-on-pinboard
  version: 1.0.0
host: api.pinboard.in
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /posts/update:
    get:
      summary: Update Tag
      description: Returns the most recent time a bookmark was added, updated or deleted.
        Use this before calling posts/all to see if the data has changed since the
        last fetch.
      operationId: posts.update.get
      x-api-path-slug: postsupdate-get
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/add:
    get:
      summary: Add New Bookmark
      description: Add a new bookmark.
      operationId: posts.add.get
      x-api-path-slug: postsadd-get
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/delete:
    get:
      summary: Delete a Post
      description: Delete a bookmark.
      operationId: posts.delete.get
      x-api-path-slug: postsdelete-get
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/get:
    get:
      summary: Get Posts
      description: Returns one or more posts on a single day matching the arguments.
        If no date or url is given, date of most recent bookmark will be used.
      operationId: posts.get.get
      x-api-path-slug: postsget-get
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/dates:
    get:
      summary: Get Post by Dates
      description: Returns a list of dates with the number of posts at each date.
      operationId: posts.dates.get
      x-api-path-slug: postsdates-get
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Dates
  /posts/recent:
    get:
      summary: Get Recent Posts
      description: Returns a list of the user's most recent posts, filtered by tag.
      operationId: posts.recent.get
      x-api-path-slug: postsrecent-get
      parameters:
      - in: query
        name: count
        description: number of results to return
        type: string
        format: string
      - in: query
        name: tag
        description: filter by up to three tags
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Recent
  /posts/all:
    get:
      summary: Get All Posts
      description: Returns all bookmarks in the user's account.
      operationId: posts.all.get
      x-api-path-slug: postsall-get
      parameters:
      - in: query
        name: fromdt
        description: return only bookmarks created after this time
        type: string
        format: string
      - in: query
        name: meta
        description: include a change detection signature for each bookmark
        type: string
        format: string
      - in: query
        name: results
        description: number of results to return
        type: string
        format: string
      - in: query
        name: start
        description: offset value (default is 0)
        type: string
        format: string
      - in: query
        name: tag
        description: filter by up to three tags
        type: string
        format: string
      - in: query
        name: todt
        description: eturn only bookmarks created before this time
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/suggest:
    get:
      summary: Get Popular Tags
      description: Returns a list of popular tags and recommended tags for a given
        URL. Popular tags are tags used site-wide for the url; recommended tags are
        drawn from the user's own tags.
      operationId: posts.suggest.get
      x-api-path-slug: postssuggest-get
      parameters:
      - in: query
        name: format
        description: the format to return
        type: string
        format: string
      - in: query
        name: url
        description: url to suggest from
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Suggest
  /tags/get:
    get:
      summary: Get Tags
      description: Returns a full list of the user's tags along with the number of
        times they were used.
      operationId: tags.get.get
      x-api-path-slug: tagsget-get
      parameters:
      - in: query
        name: format
        description: the format to return
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/delete:
    get:
      summary: Deletes Tag
      description: Delete an existing tag.
      operationId: tags.delete.get
      x-api-path-slug: tagsdelete-get
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/rename:
    get:
      summary: Rename Tags
      description: Rename an tag, or fold it in to an existing tag.
      operationId: tags.rename.get
      x-api-path-slug: tagsrename-get
      responses:
        200:
          description: OK
      tags:
      - Tags
  /user/secret:
    get:
      summary: Get User Secret
      description: Get the secret RSS token (allows viewing user's private RSS feeds).
      operationId: user.secret.get
      x-api-path-slug: usersecret-get
      responses:
        200:
          description: OK
      tags:
      - User
      - Secret