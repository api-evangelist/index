swagger: "2.0"
x-collection-name: Medium
x-complete: 1
info:
  title: Medium.com
  description: mediums-unofficial-api-documentation-using-openapi-specification--official-apiofficial-api-document-can-also-be-viewed-for-most-up-to-date-api-spec-at-httpsgithub-commediummediumapidocshttpsgithub-commediummediumapidocs-developer-blog--welcome-to-the-medium-apihttpsmedium-comblogwelcometothemediumapi3418f956552
  termsOfService: https://medium.com/@feerst/2b405a832a2f
  contact:
    name: Hossain Khan
    url: https://github.com/amardeshbd/medium-api-specification
  version: 1.0.0
host: api.medium.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me:
    get:
      summary: User details
      description: Returns details of the user who has granted permission to the application.
      operationId: me.get
      x-api-path-slug: me-get
      responses:
        200:
          description: OK
      tags:
      - Me
  /publications/{publicationId}/contributors:
    get:
      summary: Contributors of Publication
      description: This endpoint returns a list of contributors for a given publication.
        In other words, a list of Medium users who are allowed to publish under a
        publication, as well as a description of their exact role in the publication
        (for now, either an editor or a writer).
      operationId: publications.publicationId.contributors.get
      x-api-path-slug: publicationspublicationidcontributors-get
      parameters:
      - in: path
        name: publicationId
        description: A unique identifier for the publication
      responses:
        200:
          description: OK
      tags:
      - Publications
      - Publication
      - Contributors
  /publications/{publicationId}/posts:
    post:
      summary: Create Publication Post
      description: |-
        creating a post and associating it with a publication on Medium. The request also shows this association, considering posts a collection of resources under a publication

        There are additional rules around publishing that each request to this API must respect:
          - If the authenticated user is an 'editor' for the publication, they can create posts with any publish status. Posts published as 'public' or 'unlisted' will appear in collection immediately, while posts created as 'draft' will remain in pending state under publication.
          - If the authenticated user is a 'writer' for the chosen publication, they can only create a post as a 'draft'. That post will remain in pending state under publication until an editor for the publication approves it.
          - If the authenticated user is neither a 'writer' nor an 'editor', they are not allowed to create any posts in a publication.
      operationId: publications.publicationId.posts.post
      x-api-path-slug: publicationspublicationidposts-post
      parameters:
      - in: body
        name: body
        description: Creates a post for publication
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: publicationId
        description: Here publicationId is the id of the publication the post is being
          created under
      responses:
        200:
          description: OK
      tags:
      - Publications
      - Publication
      - Posts
  /users/{authorId}/posts:
    post:
      summary: Create User Post
      description: Creates a post on the authenticated user???s profile.
      operationId: users.authorId.posts.post
      x-api-path-slug: usersauthoridposts-post
      parameters:
      - in: path
        name: authorId
        description: authorId is the user id of the authenticated user
      - in: body
        name: body
        description: Creates a post for user
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
      - Author
      - Posts
  /users/{userId}/publications:
    get:
      summary: User's publications
      description: Returns a full list of publications that the user is related to
        in some way. This includes all publications the user is subscribed to, writes
        to, or edits.
      operationId: users.userId.publications.get
      x-api-path-slug: usersuseridpublications-get
      parameters:
      - in: path
        name: userId
        description: A unique identifier for the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Publications