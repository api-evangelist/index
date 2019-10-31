swagger: "2.0"
x-collection-name: Google Slides
x-complete: 1
info:
  title: Google Slides
  description: an-api-for-creating-and-editing-google-slides-presentations-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: slides.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/presentations:
    post:
      summary: Create Presentation
      description: |-
        Creates a new presentation using the title given in the request. Other
        fields in the request are ignored.
        Returns the created presentation.
      operationId: slides.presentations.create
      x-api-path-slug: v1presentations-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Presentation
  /v1/presentations/{presentationId}:
    get:
      summary: Get Presentation
      description: Gets the latest version of the specified presentation.
      operationId: slides.presentations.get
      x-api-path-slug: v1presentationspresentationid-get
      parameters:
      - in: path
        name: presentationId
        description: The ID of the presentation to retrieve
      responses:
        200:
          description: OK
      tags:
      - Presentation
  /v1/presentations/{presentationId}/pages/{pageObjectId}:
    get:
      summary: Get Presentation Page
      description: Gets the latest version of the specified page in the presentation.
      operationId: slides.presentations.pages.get
      x-api-path-slug: v1presentationspresentationidpagespageobjectid-get
      parameters:
      - in: path
        name: pageObjectId
        description: The object ID of the page to retrieve
      - in: path
        name: presentationId
        description: The ID of the presentation to retrieve
      responses:
        200:
          description: OK
      tags:
      - Presentation
      - Page
  /v1/presentations/{presentationId}:batchUpdate:
    post:
      summary: Update Presentation
      description: |-
        Applies one or more updates to the presentation.

        Each request is validated before
        being applied. If any request is not valid, then the entire request will
        fail and nothing will be applied.

        Some requests have replies to
        give you some information about how they are applied. Other requests do
        not need to return information; these each return an empty reply.
        The order of replies matches that of the requests.

        For example, suppose you call batchUpdate with four updates, and only the
        third one returns information. The response would have two empty replies:
        the reply to the third request, and another empty reply, in that order.

        Because other users may be editing the presentation, the presentation
        might not exactly reflect your changes: your changes may
        be altered with respect to collaborator changes. If there are no
        collaborators, the presentation should reflect your changes. In any case,
        the updates in your request are guaranteed to be applied together
        atomically.
      operationId: slides.presentations.batchUpdate
      x-api-path-slug: v1presentationspresentationidbatchupdate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: presentationId
        description: The presentation to apply the updates to
      responses:
        200:
          description: OK
      tags:
      - Presentation