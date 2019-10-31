swagger: "2.0"
x-collection-name: US Digital Registry
x-complete: 1
info:
  title: U.S. Digital Registry Tag API
  description: provides-a-access-to-the-list-of-tags-applied-to-federal-government-agencies-and-their-social-media-accounts-
  version: 1.0.0
host: usdigitalregistry.digitalgov.gov
basePath: /api/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tags/types.json:
    get:
      summary: Tag Types
      description: This returns a tag based on an ID.
      operationId: Api::V1::Tags#types
      x-api-path-slug: tagstypes-json-get
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags.json:
    get:
      summary: Tags
      description: This lists all tags.  It accepts parameters to perform basic search.
      operationId: Api::V1::Tags#index
      x-api-path-slug: tags-json-get
      parameters:
      - in: query
        name: page
        description: Page number
      - in: query
        name: page_size
        description: Number of results per page
      - in: query
        name: q
        description: String to compare to the short name of tags
      - in: query
        name: type
        description: Comma separated list of tag types
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/{id}.json:
    get:
      summary: Tag
      description: This returns a tag based on an ID.
      operationId: Api::V1::Tags#show
      x-api-path-slug: tagsid-json-get
      parameters:
      - in: path
        name: id
        description: ID of the tag
      responses:
        200:
          description: OK
      tags:
      - Tags