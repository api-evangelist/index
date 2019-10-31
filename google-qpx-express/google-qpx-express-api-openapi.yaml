swagger: "2.0"
x-collection-name: Google QPX Express
x-complete: 1
info:
  title: QPX Express
  description: finds-the-least-expensive-flights-between-an-origin-and-a-destination-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /qpxExpress/v1/trips
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search:
    post:
      summary: Search Flights
      description: Returns a list of flights.
      operationId: qpxExpress.trips.search
      x-api-path-slug: search-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Flights