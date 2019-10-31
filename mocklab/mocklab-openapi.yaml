swagger: "2.0"
x-collection-name: MockLab
x-complete: 1
info:
  title: WireMock
  version: 1.0.0
basePath: /__admin
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /mappings:
    delete:
      summary: Delete Mappings
      description: Delete all stub mappings
      operationId: deleteMappings
      x-api-path-slug: mappings-delete
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
    get:
      summary: Get Mappings
      description: Get all stub mappings
      operationId: getMappings
      x-api-path-slug: mappings-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: The start index of the results to return
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
    post:
      summary: Post Mappings
      description: Create a new stub mapping
      operationId: postMappings
      x-api-path-slug: mappings-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
  /mappings/find-by-metadata:
    post:
      summary: Post Mappings Find By Metadata
      description: Find stubs by matching on their metadata
      operationId: postMappingsFindByMetadata
      x-api-path-slug: mappingsfindbymetadata-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Find
      - Metadata
  /mappings/remove-by-metadata:
    post:
      summary: Post Mappings Remove By Metadata
      description: Remove stubs by matching on their metadata
      operationId: postMappingsRemoveByMetadata
      x-api-path-slug: mappingsremovebymetadata-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Remove
      - Metadata
  /mappings/reset:
    post:
      summary: Post Mappings Reset
      description: Reset stub mappings (restore to defaults defined back the backing
        store)
      operationId: postMappingsReset
      x-api-path-slug: mappingsreset-post
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Reset
  /mappings/save:
    post:
      summary: Post Mappings Save
      description: Save all persistent stub mappings to the backing store
      operationId: postMappingsSave
      x-api-path-slug: mappingssave-post
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Save
  /mappings/{stubMappingId}:
    delete:
      summary: Delete Mappings Stubmappingid
      description: Delete mappings stubmappingid.
      operationId: deleteMappingsStubmapping
      x-api-path-slug: mappingsstubmappingid-delete
      parameters:
      - in: path
        name: stubMappingId
        description: The UUID of stub mapping
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Stubmappingid
    get:
      summary: Get Mappings Stubmappingid
      description: Get mappings stubmappingid.
      operationId: getMappingsStubmapping
      x-api-path-slug: mappingsstubmappingid-get
      parameters:
      - in: path
        name: stubMappingId
        description: The UUID of stub mapping
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Stubmappingid
    put:
      summary: Put Mappings Stubmappingid
      description: Update an existing stub mapping
      operationId: putMappingsStubmapping
      x-api-path-slug: mappingsstubmappingid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: stubMappingId
        description: The UUID of stub mapping
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Stubmappingid
  /near-misses/request:
    post:
      summary: Post Near Misses Request
      description: Find at most 3 near misses for closest stub mappings to the specified
        request
      operationId: postNearMissesRequest
      x-api-path-slug: nearmissesrequest-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Near
      - Misses
      - Request
  /near-misses/request-pattern:
    post:
      summary: Post Near Misses Request Pattern
      description: Find at most 3 near misses for closest logged requests to the specified
        request pattern
      operationId: postNearMissesRequestPattern
      x-api-path-slug: nearmissesrequestpattern-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Near
      - Misses
      - Request
      - Pattern
  /recordings/snapshot:
    post:
      summary: Post Recordings Snapshot
      description: Take a snapshot recording
      operationId: postRecordingsSnapshot
      x-api-path-slug: recordingssnapshot-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Recordings
      - Snapshot
  /recordings/start:
    post:
      summary: Post Recordings Start
      description: Start recording stub mappings
      operationId: postRecordingsStart
      x-api-path-slug: recordingsstart-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Recordings
      - Start
  /recordings/status:
    get:
      summary: Get Recordings Status
      description: Get the recording status (started or stopped)
      operationId: getRecordingsStatus
      x-api-path-slug: recordingsstatus-get
      responses:
        200:
          description: Successful response
      tags:
      - Recordings
      - Status
  /recordings/stop:
    post:
      summary: Post Recordings Stop
      description: Stop recording stub mappings
      operationId: postRecordingsStop
      x-api-path-slug: recordingsstop-post
      responses:
        200:
          description: Successful response
      tags:
      - Recordings
      - Stop
  /requests:
    delete:
      summary: Delete Requests
      description: Delete all received requests
      operationId: deleteRequests
      x-api-path-slug: requests-delete
      responses:
        200:
          description: Successful response
      tags:
      - Requests
    get:
      summary: Get Requests
      description: Get received requests
      operationId: getRequests
      x-api-path-slug: requests-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: since
        description: Only return logged requests after this date
      responses:
        200:
          description: Successful response
      tags:
      - Requests
  /requests/count:
    post:
      summary: Post Requests Count
      description: Count requests logged in the journal matching the specified criteria
      operationId: postRequestsCount
      x-api-path-slug: requestscount-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Requests
      - Count
  /requests/find:
    post:
      summary: Post Requests Find
      description: Retrieve details of requests logged in the journal matching the
        specified criteria
      operationId: postRequestsFind
      x-api-path-slug: requestsfind-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Requests
      - Find
  /requests/reset:
    post:
      summary: Post Requests Reset
      description: Empty the request journal
      operationId: postRequestsReset
      x-api-path-slug: requestsreset-post
      responses:
        200:
          description: Successful response
      tags:
      - Requests
      - Reset
  /requests/unmatched:
    get:
      summary: Get Requests Unmatched
      description: Get details of logged requests that weren't matched by any stub
        mapping
      operationId: getRequestsUnmatched
      x-api-path-slug: requestsunmatched-get
      responses:
        200:
          description: Successful response
      tags:
      - Requests
      - Unmatched
  /requests/unmatched/near-misses:
    get:
      summary: Get Requests Unmatched Near Misses
      description: Retrieve near-misses for all unmatched requests
      operationId: getRequestsUnmatchedNearMisses
      x-api-path-slug: requestsunmatchednearmisses-get
      responses:
        200:
          description: Successful response
      tags:
      - Requests
      - Unmatched
      - Near
      - Misses
  /requests/{requestId}:
    get:
      summary: Get Requests Requestid
      description: Get requests requestid.
      operationId: getRequestsRequest
      x-api-path-slug: requestsrequestid-get
      parameters:
      - in: path
        name: requestId
        description: The UUID of the logged request
      responses:
        200:
          description: Successful response
      tags:
      - Requests
      - Requestid
  /scenarios:
    get:
      summary: Get Scenarios
      description: Get all scenarios
      operationId: getScenarios
      x-api-path-slug: scenarios-get
      responses:
        200:
          description: Successful response
      tags:
      - Scenarios
  /scenarios/reset:
    post:
      summary: Post Scenarios Reset
      description: Reset the state of all scenarios
      operationId: postScenariosReset
      x-api-path-slug: scenariosreset-post
      responses:
        200:
          description: Successful response
      tags:
      - Scenarios
      - Reset
  /settings:
    post:
      summary: Post Settings
      description: Update global settings
      operationId: postSettings
      x-api-path-slug: settings-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Settings
  /shutdown:
    post:
      summary: Post Shutdown
      description: Shutdown the WireMock server
      operationId: postShutdown
      x-api-path-slug: shutdown-post
      responses:
        200:
          description: Successful response
      tags:
      - Shutdown