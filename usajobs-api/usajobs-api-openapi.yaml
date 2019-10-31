swagger: "2.0"
x-collection-name: USAJobs API
x-complete: 1
info:
  title: USAJobs API
  description: federal-state-and-local-government-agencies-are-hiring-and-have-thousands-of-job-openings-across-the-country-posted-on-usajobs-gov-and-local-government-jobs-sites-
  termsOfService: https://www.usa.gov/About/developer-resources/terms-of-service.shtml
  version: 1.0.0
host: api.usa.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /jobs/search.json:
    get:
      summary: Search Jobs
      description: his Jobs API allows you to tap into a list of current jobs openings
        with the government.
      operationId: searchJobs
      x-api-path-slug: jobssearch-json-get
      parameters:
      - in: query
        name: from
        description: Specifies the starting record
        type: string
        format: string
      - in: query
        name: hi
        description: No highlighting is included by default
        type: string
        format: string
      - in: query
        name: Lat_lon
        description: Comma-separated pair denoting the position of the searcher looking
          for a job
        type: string
        format: string
      - in: query
        name: organization_ids
        description: A comma-separated string specifying which federal, state, or
          local agencies to use as a filter
        type: string
        format: string
      - in: query
        name: query
        description: Attempts to extract as much signal as possible from the input
          text
        type: string
        format: string
      - in: query
        name: size
        description: Specifies how many results are returned (up to 100 at a time)
        type: string
        format: string
      - in: query
        name: tags
        description: A comma-separated string specifying the level of government
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Jobs