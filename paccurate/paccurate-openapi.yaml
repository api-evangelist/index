swagger: "2.0"
x-collection-name: Paccurate
x-complete: 1
info:
  title: paccurate.io
  version: 0.1.1
host: api.paccurate.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    post:
      summary: Post
      description: a pure-JSON endpoint for packing requests.
      operationId: .post
      x-api-path-slug: post
      parameters:
      - in: body
        name: pack
        description: complete set of items, boxes, and parameters to pack
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Packaging