swagger: "2.0"
x-collection-name: EU BON UTIS
x-complete: 1
info:
  title: EU BON UTIS
  description: the-unified-taxonomic-information-service-utis-is-the-taxonomic-backbone-for-the-eubon-project
  termsOfService: https://www.biodiversitycatalogue.org/services/79
  version: "1.0"
host: cybertaxonomy.eu
basePath: /eu-bon/utis/1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /capabilities:
    get:
      summary: Capabilities
      description: Capabilities
      operationId: getCapabilities
      x-api-path-slug: capabilities-get
      responses:
        200:
          description: OK
      tags:
      - Capabilities
  /search:
    get:
      summary: Search
      description: Search
      operationId: getSearch
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: addSynonymy
        description: Indicates whether the synonymy of the accepted taxon should be
          included into the response
      - in: query
        name: providers
        description: A list of provider id strings concatenated by comma characters
      - in: query
        name: query
        description: The scientific name to search for
      - in: query
        name: searchMode
        description: Specifies the searchMode
      - in: query
        name: timeout
        description: The maximum of milliseconds to wait for responses from any of
          the providers
      responses:
        200:
          description: OK
      tags:
      - Search