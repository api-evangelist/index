swagger: "2.0"
x-collection-name: Google Knowledge Graph Search
x-complete: 1
info:
  title: Knowledge Graph Search
  description: searches-the-google-knowledge-graph-for-entities-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: kgsearch.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/entities:search:
    get:
      summary: Search Knowledge Graph
      description: |-
        Searches Knowledge Graph for entities that match the constraints.
        A list of matched entities will be returned in response, which will be in
        JSON-LD format and compatible with http://schema.org
      operationId: kgsearch.entities.search
      x-api-path-slug: v1entitiessearch-get
      parameters:
      - in: query
        name: ids
        description: The list of entity id to be used for search instead of query
          string
      - in: query
        name: indent
        description: Enables indenting of json results
      - in: query
        name: languages
        description: The list of language codes (defined in ISO 693) to run the query
          with,e
      - in: query
        name: limit
        description: Limits the number of entities to be returned
      - in: query
        name: prefix
        description: Enables prefix match against names and aliases of entities
      - in: query
        name: query
        description: The literal query string for search
      - in: query
        name: types
        description: Restricts returned entities with these types, e
      responses:
        200:
          description: OK
      tags:
      - Knowledge Graph