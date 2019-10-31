swagger: "2.0"
x-collection-name: MapQuest
x-complete: 1
info:
  title: 'MapQuest Search API: Place Search'
  description: place-search-is-a-spatiallyaware-search-engine-most-commonly-used-to-return-point-of-interest-poi-results-near-a-geographic-point-of-reference-or-within-a-geographic-boundary-such-as-find-all-coffee-shops-within-the-extent-of-the-current-map--results-can-be-ordered-by-distance-or-relevance--this-api-complements-the-search-ahead-api-by-performing-the-backend-search-necessary-to-fulfill-category-or-franchise-requests-
  version: 1.0.0
host: www.mapquestapi.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search/v4/place:
    get:
      summary: Search for places with optional geographic and categorical contexts.
      description: Get a list of search results ordered by relevance or distance from
        a spatial reference point, optionally filtered by category, and optionally
        bounded within a geographic constraint.
      operationId: get-a-list-of-search-results-ordered-by-relevance-or-distance-from-a-spatial-reference-point-optiona
      x-api-path-slug: searchv4place-get
      parameters:
      - in: query
        name: bbox
        description: A geographic rectangle used to bound the search
      - in: query
        name: category
        description: The categories of places to search over
      - in: query
        name: circle
        description: A geographic circle used to bound the search
      - in: query
        name: corridor
        description: A collection of points defining a route used for the search
      - in: query
        name: feedback
      - in: query
        name: key
        description: A valid and authorized MapQuest API key
      - in: query
        name: limit
        description: (Deprecated
      - in: query
        name: location
        description: A geographic context used for searching, ranking, and ordering
          results
      - in: query
        name: page
        description: The page within the result set to return, where pageSize determines
          the page size
      - in: query
        name: pageSize
        description: The number of results to return per page
      - in: query
        name: q
        description: A query phrase
      - in: query
        name: sort
        description: The scheme used to order results
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Places