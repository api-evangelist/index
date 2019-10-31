swagger: "2.0"
x-collection-name: Refuge Restrooms
x-complete: 1
info:
  title: Refuge Restrooms
  description: refuge-is-a-web-application-that-seeks-to-provide-safe-restroom-access-for-transgender-intersex-and-gender-nonconforming-individuals-
  version: v1
host: www.refugerestrooms.org
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/restrooms.json:
    get:
      summary: Get all restroom records ordered by date descending.
      description: ""
      operationId: v1.restrooms.json.get
      x-api-path-slug: v1restrooms-json-get
      parameters:
      - in: query
        name: ada
        description: Only return restrooms that are ADA accessible
      - in: query
        name: offset
        description: Pad a number of results
      - in: query
        name: page
        description: Page offset to fetch
      - in: query
        name: per_page
        description: Number of results to return per page
      - in: query
        name: unisex
        description: Only return restrooms that are unisex
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/restrooms/by_date.json:
    get:
      summary: Search for restroom records updated or created on or after a given
        date
      description: ""
      operationId: v1.restrooms.by_date.json.get
      x-api-path-slug: v1restroomsby-date-json-get
      parameters:
      - in: query
        name: ada
        description: Only return restrooms that are ADA accessible
      - in: query
        name: day
        description: Day
      - in: query
        name: month
        description: Month
      - in: query
        name: offset
        description: Pad a number of results
      - in: query
        name: page
        description: Page offset to fetch
      - in: query
        name: per_page
        description: Number of results to return per page
      - in: query
        name: unisex
        description: Only return restrooms that are unisex
      - in: query
        name: updated
        description: Return restroom records updated (rather than created) since given
          date
      - in: query
        name: year
        description: Year
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/restrooms/by_location.json:
    get:
      summary: Search by location.
      description: ""
      operationId: v1.restrooms.by_location.json.get
      x-api-path-slug: v1restroomsby-location-json-get
      parameters:
      - in: query
        name: ada
        description: Only return restrooms that are ADA accessible
      - in: query
        name: lat
        description: latitude
      - in: query
        name: lng
        description: longitude
      - in: query
        name: offset
        description: Pad a number of results
      - in: query
        name: page
        description: Page offset to fetch
      - in: query
        name: per_page
        description: Number of results to return per page
      - in: query
        name: unisex
        description: Only return restrooms that are unisex
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/restrooms/search.json:
    get:
      summary: Perform full-text search of restroom records.
      description: ""
      operationId: v1.restrooms.search.json.get
      x-api-path-slug: v1restroomssearch-json-get
      parameters:
      - in: query
        name: ada
        description: Only return restrooms that are ADA accessible
      - in: query
        name: offset
        description: Pad a number of results
      - in: query
        name: page
        description: Page offset to fetch
      - in: query
        name: per_page
        description: Number of results to return per page
      - in: query
        name: query
        description: Your search query
      - in: query
        name: unisex
        description: Only return restrooms that are unisex
      responses:
        200:
          description: OK
      tags:
      - ""