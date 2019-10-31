swagger: "2.0"
x-collection-name: Google Safe Browsing
x-complete: 1
info:
  title: Google Safe Browsing
  description: the-safe-browsing-api-is-an-experimental-api-that-allows-client-applications-to-check-urls-against-googles-constantlyupdated-blacklists-of-suspected-phishing-and-malware-pages--your-client-application-can-use-the-api-to-download-an-encrypted-table-for-local-clientside-lookups-of-urls-
  contact:
    name: Google
    url: https://google.com
  version: v4
host: safebrowsing.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v4/encodedFullHashes/{encodedRequest}:
    get:
      summary: Encode Full Hashes
      description: Encode Full Hashes
      operationId: safebrowsing.encodedFullHashes.get
      x-api-path-slug: v4encodedfullhashesencodedrequest-get
      parameters:
      - in: query
        name: clientId
        description: A client ID that (hopefully) uniquely identifies the client implementationof
          the Safe Browsing API
      - in: query
        name: clientVersion
        description: The version of the client implementation
      - in: path
        name: encodedRequest
        description: A serialized FindFullHashesRequest proto
      responses:
        200:
          description: OK
      tags:
      - Hash
  /v4/encodedUpdates/{encodedRequest}:
    get:
      summary: Encoded Updates
      description: Encoded Updates
      operationId: safebrowsing.encodedUpdates.get
      x-api-path-slug: v4encodedupdatesencodedrequest-get
      parameters:
      - in: query
        name: clientId
        description: A client ID that uniquely identifies the client implementation
          of the SafeBrowsing API
      - in: query
        name: clientVersion
        description: The version of the client implementation
      - in: path
        name: encodedRequest
        description: A serialized FetchThreatListUpdatesRequest proto
      responses:
        200:
          description: OK
      tags:
      - Updates
  /v4/fullHashes:find:
    post:
      summary: Find Full Hash Match
      description: Finds the full hashes that match the requested hash prefixes.
      operationId: safebrowsing.fullHashes.find
      x-api-path-slug: v4fullhashesfind-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Hash
  /v4/threatListUpdates:fetch:
    post:
      summary: List Most Recent Threats
      description: |-
        Fetches the most recent threat list updates. A client can request updates
        for multiple lists at once.
      operationId: safebrowsing.threatListUpdates.fetch
      x-api-path-slug: v4threatlistupdatesfetch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Threats
  /v4/threatLists:
    get:
      summary: List Threats
      description: Lists the Safe Browsing threat lists available for download.
      operationId: safebrowsing.threatLists.list
      x-api-path-slug: v4threatlists-get
      responses:
        200:
          description: OK
      tags:
      - Threats
  /v4/threatMatches:find:
    post:
      summary: Find Threat Entry
      description: Finds the threat entries that match the Safe Browsing lists.
      operationId: safebrowsing.threatMatches.find
      x-api-path-slug: v4threatmatchesfind-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Threats