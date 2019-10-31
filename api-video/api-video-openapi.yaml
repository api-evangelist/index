swagger: "2.0"
x-collection-name: api.video
x-complete: 1
info:
  title: api.video
  description: the-simplest-way-to-put-video-on-the-web
  version: 1.0.0
host: ws.api.video
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /videos/{id}/thumbnail:
    parameters:
      summary: Parameters Videos Thumbnail
      description: Parameters videos thumbnail.
      operationId: parametersVeosThumbnail
      x-api-path-slug: videosidthumbnail-parameters
      responses:
        200:
          description: Successful response
      tags:
      - Parameters
      - Videos
      - Thumbnail
    patch:
      summary: Patch Videos Thumbnail
      description: |-
        Pick a thumbnail from the given time code.

        It may take up to 1h before the new thumbnail to be delivered by our CDN.
      operationId: patchVeosThumbnail
      x-api-path-slug: videosidthumbnail-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Videos
      - Thumbnail
    post:
      summary: Post Videos Thumbnail
      description: It may take up to 1h before the new thumbnail to be delivered by
        our CDN.
      operationId: postVeosThumbnail
      x-api-path-slug: videosidthumbnail-post
      responses:
        200:
          description: Successful response
      tags:
      - Videos
      - Thumbnail
  /videos/{videoId}:
    parameters:
      summary: Parameters Videos Videoid
      description: Parameters videos videoid.
      operationId: parametersVeosVeo
      x-api-path-slug: videosvideoid-parameters
      responses:
        200:
          description: Successful response
      tags:
      - Parameters
      - Videos
    patch:
      summary: Patch Videos Videoid
      description: Patch videos videoid.
      operationId: patchVeosVeo
      x-api-path-slug: videosvideoid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Videos
  /players/{id}:
    parameters:
      summary: Parameters Players
      description: Parameters players.
      operationId: parametersPlayers
      x-api-path-slug: playersid-parameters
      responses:
        200:
          description: Successful response
      tags:
      - Parameters
      - Players
    patch:
      summary: Patch Players
      description: It may take up to 10min before the new player configuration is
        available from our CDN.
      operationId: patchPlayers
      x-api-path-slug: playersid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Players
    get:
      summary: Get Players
      description: Get players.
      operationId: getPlayers
      x-api-path-slug: playersid-get
      responses:
        200:
          description: Successful response
      tags:
      - Players
  /token:
    post:
      summary: Post Token
      description: Post token.
      operationId: postToken
      x-api-path-slug: token-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Token
  /videos/{id}:
    parameters:
      summary: Parameters Videos
      description: Parameters videos.
      operationId: parametersVeos
      x-api-path-slug: videosid-parameters
      responses:
        200:
          description: Successful response
      tags:
      - Parameters
      - Videos
    get:
      summary: Get Videos
      description: Get videos.
      operationId: getVeos
      x-api-path-slug: videosid-get
      responses:
        200:
          description: Successful response
      tags:
      - Videos
    delete:
      summary: Delete Videos
      description: Delete videos.
      operationId: deleteVeos
      x-api-path-slug: videosid-delete
      responses:
        200:
          description: Successful response
      tags:
      - Videos
  /videos:
    post:
      summary: Post Videos
      description: Post videos.
      operationId: postVeos
      x-api-path-slug: videos-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Videos
    get:
      summary: Get Videos
      description: Get videos.
      operationId: getVeos
      x-api-path-slug: videos-get
      parameters:
      - in: query
        name: keyword
      - in: query
        name: metadata
      - in: query
        name: tags
      responses:
        200:
          description: Successful response
      tags:
      - Videos
  /players:
    get:
      summary: Get Players
      description: Get players.
      operationId: getPlayers
      x-api-path-slug: players-get
      responses:
        200:
          description: Successful response
      tags:
      - Players
    post:
      summary: Post Players
      description: Post players.
      operationId: postPlayers
      x-api-path-slug: players-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Players
  /refresh:
    post:
      summary: Post Refresh
      description: Post refresh.
      operationId: postRefresh
      x-api-path-slug: refresh-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Refresh
  /videos/{id}/source:
    parameters:
      summary: Parameters Videos Source
      description: Parameters videos source.
      operationId: parametersVeosSource
      x-api-path-slug: videosidsource-parameters
      responses:
        200:
          description: Successful response
      tags:
      - Parameters
      - Videos
      - Source
    post:
      summary: Post Videos Source
      description: Post videos source.
      operationId: postVeosSource
      x-api-path-slug: videosidsource-post
      parameters:
      - in: header
        name: Content-Range
      - in: header
        name: Expect
      responses:
        200:
          description: Successful response
      tags:
      - Videos
      - Source