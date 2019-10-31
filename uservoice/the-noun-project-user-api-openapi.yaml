swagger: "2.0"
x-collection-name: UserVoice
x-complete: 1
info:
  title: The Noun Project User API
  version: 1.0.0
host: /user
basePath: http://api.thenounproject.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/{username}/uploads:
    get:
      summary: Get user uploads with user
      description: Returns a list of uploads associated with a user
      operationId: getUserUploadsWithUser
      x-api-path-slug: userusernameuploads-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of results
      - in: query
        name: offset
        description: Number of results to displace or skip over
      - in: query
        name: page
        description: Number of results of limit length to displace or skip over
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - User
      - Username
      - Uploads
  /user/{user_id}/collections:
    get:
      summary: Get user collections
      description: Returns a list of collections associated with a user
      operationId: getUserCollections
      x-api-path-slug: useruser-idcollections-get
      parameters:
      - in: path
        name: user_id
        description: User id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Collections
  /user/{user_id}/collections/{slug}:
    get:
      summary: Get user collection
      description: Returns a single collection associated with a user
      operationId: getUserCollection
      x-api-path-slug: useruser-idcollectionsslug-get
      parameters:
      - in: path
        name: slug
        description: Collection slug
      - in: path
        name: user_id
        description: User id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Collections
      - Slug