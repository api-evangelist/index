swagger: "2.0"
x-collection-name: Google URL Shortener
x-complete: 1
info:
  title: URL Shortener
  description: lets-you-create-inspect-and-manage-goo-gl-short-urls
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /urlshortener/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /url:
    get:
      summary: Get Short URLs
      description: Expands a short URL or gets creation time and analytics.
      operationId: urlshortener.url.get
      x-api-path-slug: url-get
      parameters:
      - in: query
        name: projection
        description: Additional information to return
      - in: query
        name: shortUrl
        description: The short URL, including the protocol
      responses:
        200:
          description: OK
      tags:
      - Short URL
    post:
      summary: Create Short URL
      description: Creates a new short URL.
      operationId: urlshortener.url.insert
      x-api-path-slug: url-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Short URL
  /url/history:
    get:
      summary: Get URL History
      description: Retrieves a list of URLs shortened by a user.
      operationId: urlshortener.url.list
      x-api-path-slug: urlhistory-get
      parameters:
      - in: query
        name: projection
        description: Additional information to return
      - in: query
        name: start-token
        description: Token for requesting successive pages of results
      responses:
        200:
          description: OK
      tags:
      - Short URL