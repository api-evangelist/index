swagger: "2.0"
x-collection-name: APIs.Guru
x-complete: 1
info:
  title: APIs.guru
  description: wikipedia-for-web-apis--repository-of-api-specs-in-openapifka-swagger-2-0-format-warning-if-you-want-to-be-notified-about-changes-in-advance-please-subscribe-to-our-gitter-channelhttpsgitter-imapisguruapimodels-client-sample-demohttpsapis-gurusimpleui-repohttpsgithub-comapisgurusimpleui
  contact:
    name: APIs.guru
    url: http://APIs.guru
    email: founders@apis.guru
  version: 2.0.1
host: api.apis.guru
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /list.json:
    get:
      summary: List all APIs
      description: |-
        List all APIs in the directory.
        Returns links to OpenAPI specification for each API in the directory.
        If API exist in multiple versions `preferred` one is explicitly marked.

        Some basic info from OpenAPI spec is cached inside each object.
        This allows to generate some simple views without need to fetch OpenAPI spec for each API.
      operationId: listAPIs
      x-api-path-slug: list-json-get
      responses:
        200:
          description: OK
      tags:
      - APIs
      - Definitions
      - Discovery
  /metrics.json:
    get:
      summary: Get basic metrics
      description: |-
        Some basic metrics for the entire directory.
        Just stunning numbers to put on a front page and are intended purely for WoW effect :)
      operationId: getMetrics
      x-api-path-slug: metrics-json-get
      responses:
        200:
          description: OK
      tags:
      - APIs
      - Definitions
      - Discovery