swagger: "2.0"
x-collection-name: Google Civic Information
x-complete: 1
info:
  title: Google Civic Information
  description: provides-polling-places-early-vote-locations-contest-data-election-officials-and-government-representatives-for-u-s--residential-addresses-
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /civicinfo/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /divisions:
    get:
      summary: Search Political Divisions
      description: Searches for political divisions by their natural name or OCD ID.
      operationId: civicinfo.divisions.search
      x-api-path-slug: divisions-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: query
        description: The search query
      responses:
        200:
          description: OK
      tags:
      - Division
  /elections:
    get:
      summary: List Elections
      description: List of available elections to query.
      operationId: civicinfo.elections.electionQuery
      x-api-path-slug: elections-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Election
  /representatives:
    get:
      summary: Lookup Representatives
      description: Looks up political geography and representative information for
        a single address.
      operationId: civicinfo.representatives.representativeInfoByAddress
      x-api-path-slug: representatives-get
      parameters:
      - in: query
        name: address
        description: The address to look up
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: includeOffices
        description: Whether to return information about offices and officials
      - in: query
        name: levels
        description: A list of office levels to filter by
      - in: query
        name: roles
        description: A list of office roles to filter by
      responses:
        200:
          description: OK
      tags:
      - Representative
  /representatives/{ocdId}:
    get:
      summary: Get Representative
      description: Looks up representative information for a single geographic division.
      operationId: civicinfo.representatives.representativeInfoByDivision
      x-api-path-slug: representativesocdid-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: levels
        description: A list of office levels to filter by
      - in: path
        name: ocdId
        description: The Open Civic Data division identifier of the division to look
          up
      - in: query
        name: recursive
        description: If true, information about all divisions contained in the division
          requested will be included as well
      - in: query
        name: roles
        description: A list of office roles to filter by
      responses:
        200:
          description: OK
      tags:
      - Representative
  /voterinfo:
    get:
      summary: Looks Up Voter Information
      description: Looks up information relevant to a voter based on the voter's registered
        address.
      operationId: civicinfo.elections.voterInfoQuery
      x-api-path-slug: voterinfo-get
      parameters:
      - in: query
        name: address
        description: The registered address of the voter to look up
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: electionId
        description: The unique ID of the election to look up
      - in: query
        name: officialOnly
        description: If set to true, only data from official state sources will be
          returned
      - in: query
        name: returnAllAvailableData
        description: If set to true, the query will return the success codeand include
          any partial information when it is unable to determine a matching address
          or unable to determine the election for electionId=0 queries
      responses:
        200:
          description: OK
      tags:
      - Voter Information