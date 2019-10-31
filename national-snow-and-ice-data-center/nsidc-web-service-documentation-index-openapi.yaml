swagger: "2.0"
x-collection-name: National Snow and Ice Data Center
x-complete: 1
info:
  title: NSIDC Web Service Documentation Index
  description: this-api-allows-programmers-to-build-national-snow-and-ice-data-center-data-and-metadata-services-into-their-applications-
  version: 1.0.0
host: nsidc.org
basePath: /api/dataset/2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Facets:
    get:
      summary: View the facet information corresponding to a search
      description: In the NSIDC Search and Arctic Data Explorer interfaces, this endpoint
        is used in conjunction with /OpenSearch whenever a user submits a new search.
        Consequently, it has the same parameters as /OpenSearch.
      operationId: facets
      x-api-path-slug: facets-get
      parameters:
      - in: query
        name: count
        description: The number of search results per page desired by the client;
          OpenSearch 1
      - in: query
        name: endDate
        description: The end date in yyyy-mm-dd format
      - in: query
        name: facetFilters
        description: Describes faceted restrictions on the search
      - in: query
        name: searchTerms
        description: URL-encoded keyword or keywords desired by the client; OpenSearch
          1
      - in: query
        name: sortKeys
        description: Sort the results by most relevant (default), smallest or largest
          spatial area, shortest or longest temporal duration, or most recently updated;
          partial implementation of OpenSearch SRU 1
      - in: query
        name: source
        description: Custom parameter for selecting which source to use; the Arctic
          Data Explorer (ADE) uses data aggregated from many sources, including, but
          not limited to, NSIDC
      - in: query
        name: spatial
        description: 4 comma separated values - W, S, E, N; OpenSearch-Geo 1
      - in: query
        name: startDate
        description: The start date in yyyy-mm-dd format
      - in: query
        name: startIndex
        description: First search result desired by the search client; OpenSearch
          1
      responses:
        200:
          description: OK
      tags:
      - Environment
  /OpenSearch:
    get:
      summary: Search documents using the OpenSearch 1.1 Specification
      description: This endpoint uses parameters from the OpenSearch 1.1 specification,
        as well as parameters from the OpenSearch Geo (1.0) and SRU (1.0) extensions.
      operationId: OpenSearch.get
      x-api-path-slug: opensearch-get
      parameters:
      - in: query
        name: count
        description: The number of search results per page desired by the client;
          OpenSearch 1
      - in: query
        name: endDate
        description: The end date in yyyy-mm-dd format
      - in: query
        name: facetFilters
        description: Describes faceted restrictions on the search
      - in: query
        name: searchTerms
        description: URL-encoded keyword or keywords desired by the client; OpenSearch
          1
      - in: query
        name: sortKeys
        description: Sort the results by most relevant (default), smallest or largest
          spatial area, shortest or longest temporal duration, or most recently updated;
          partial implementation of OpenSearch SRU 1
      - in: query
        name: source
        description: Custom parameter for selecting which source to use; the Arctic
          Data Explorer (ADE) uses data aggregated from many sources, including, but
          not limited to, NSIDC
      - in: query
        name: spatial
        description: 4 comma separated values - W, S, E, N; OpenSearch-Geo 1
      - in: query
        name: startDate
        description: The start date in yyyy-mm-dd format
      - in: query
        name: startIndex
        description: First search result desired by the search client; OpenSearch
          1
      responses:
        200:
          description: OK
      tags:
      - Environment
  /OpenSearchDescription:
    get:
      summary: Describes the web interface of NSIDC's data search engine
      description: Describes the web interface of NSIDC's data search engine
      operationId: OpenSearchDescription.get
      x-api-path-slug: opensearchdescription-get
      responses:
        200:
          description: OK
      tags:
      - Environment
  /suggest:
    get:
      summary: Suggest search terms based on a partial query
      description: In NSIDC Search and the Arctic Data Explorer, this endpoint is
        queried whenever the user types into the search terms box, and the returned
        suggestions are displayed in a dropdown beneath the search terms box. The
        q parameter and returned JSON follow the specifications of the OpenSearch
        Suggestions 1.0 extension.
      operationId: getSuggest
      x-api-path-slug: suggest-get
      parameters:
      - in: query
        name: q
        description: Search terms typed into the interface (minimum two characters)
      - in: query
        name: source
        description: Custom parameter for selecting which source to use; the Arctic
          Data Explorer (ADE) uses data aggregated from many sources, including, but
          not limited to, NSIDC
      responses:
        200:
          description: OK
      tags:
      - Environment