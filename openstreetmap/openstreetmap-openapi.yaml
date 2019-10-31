swagger: "2.0"
x-collection-name: OpenStreetMap
x-complete: 1
info:
  title: Open Street Map (OSM)
  description: todo-add-description
  version: 1.0.0
host: ' http:'
basePath: //nominatim.openstreetmap.org
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lookup:
    get:
      summary: OSM - Address lookup
      description: '[Full description of the service:](http://wiki.openstreetmap.org/wiki/Nominatim#Address_lookup)'
      operationId: LookupGet
      x-api-path-slug: lookup-get
      parameters:
      - in: query
        name: format
      - in: query
        name: osm_ids
      responses:
        200:
          description: OK
      tags:
      - Maps
      - OSM
      - Address
      - Lookup
  /reverse:
    get:
      summary: OSM - Reverse
      description: '[Full description of the service:](http://wiki.openstreetmap.org/wiki/Nominatim#Reverse_Geocoding)'
      operationId: ReverseGet
      x-api-path-slug: reverse-get
      parameters:
      - in: query
        name: format
      - in: query
        name: lat
      - in: query
        name: lon
      responses:
        200:
          description: OK
      tags:
      - Maps
      - OSM
      - Reverse
  /search:
    get:
      summary: OSM - Search
      description: '[Full documentation](http://wiki.openstreetmap.org/wiki/Nominatim#Search)'
      operationId: SearchGet
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: format
      - in: query
        name: q
      responses:
        200:
          description: OK
      tags:
      - Maps
      - OSM
      - Search