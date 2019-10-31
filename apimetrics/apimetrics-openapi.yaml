swagger: "2.0"
x-collection-name: APImetrics
x-complete: 1
info:
  title: APImetrics Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /auth/:
    get:
      summary: List Authentication Settings
      description: List Authentication Settings
      operationId: listAuthenticationSettings
      x-api-path-slug: auth-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Auth
  /auth/{id}/:
    delete:
      summary: Delete an Authentication Setting
      description: Delete an Authentication Setting
      operationId: deleteAnAuthenticationSetting
      x-api-path-slug: authid-delete
      parameters:
      - in: path
        name: id
        description: ID string of authentication string youre upda
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Auth
    get:
      summary: Get an existing Authentication Setting
      description: Get an existing Authentication Setting
      operationId: getAnExistingAuthenticationSetting
      x-api-path-slug: authid-get
      parameters:
      - in: path
        name: id
        description: ID string of authentication string youre upda
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Auth
    put:
      summary: Update an existing Authentication Setting
      description: Update an existing Authentication Setting
      operationId: updateAnExistingAuthenticationSetting
      x-api-path-slug: authid-put
      parameters:
      - in: path
        name: id
        description: ID string of authentication string youre upda
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Auth
  /calls/:
    get:
      summary: List API Calls
      description: List API Calls
      operationId: listAPICalls
      x-api-path-slug: calls-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Calls
    post:
      summary: Create new API Call
      description: Create new API Call
      operationId: createNewAPICall
      x-api-path-slug: calls-post
      parameters:
      - in: body
        name: Body
        description: '{     meta: {         name: Minimal API test name     },     request:
          {         method: get,         url: http://httpbin'
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Calls
  /calls/auth/{auth_id}/:
    get:
      summary: List API Calls by Authentication
      description: List API Calls by Authentication
      operationId: listAPICallsbyAuthentication
      x-api-path-slug: callsauthauth-id-get
      parameters:
      - in: path
        name: auth_id
        description: The ID of the authentication setting
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Calls
      - Auth
      - Auth
  /calls/{id}/:
    delete:
      summary: Delete an API Call
      description: Delete an API Call
      operationId: deleteAnAPICall
      x-api-path-slug: callsid-delete
      parameters:
      - in: path
        name: id
        description: ID string of API Call
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Calls
    get:
      summary: Get an existing API Call
      description: Get an existing API Call
      operationId: getAnExistingAPICall
      x-api-path-slug: callsid-get
      parameters:
      - in: path
        name: id
        description: ID string of API Call
      - in: query
        name: kind
        description: Granularity of data required, one of DAY, WEEK, MONTH, tYEAR
      - in: query
        name: location_id
        description: Location where the API Call was made
      - in: query
        name: time
        description: ISO formatted date string for the period you wish to view
      - in: query
        name: type
        description: Return stats for all calls in the time period specified which
          had this result
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Calls
    put:
      summary: Update an existing API Call
      description: Update an existing API Call
      operationId: updateAnExistingAPICall
      x-api-path-slug: callsid-put
      parameters:
      - in: body
        name: body
        description: '{     request: {         parameters: [             { key: testing,
          value: bar },             { key: raspberry, value: 2 }         ]     } }'
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID string of API Call
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Calls
  /calls/{id}/run:
    post:
      summary: Trigger an API Call to run
      description: Trigger an API Call to run
      operationId: triggerAnAPICallToRun
      x-api-path-slug: callsidrun-post
      parameters:
      - in: body
        name: body
        description: '{     location_id: ,     context: {         foo: 1234,         bar:
          %%RESULT_ID%%,         datum: %%DATETIME%%     } }'
        schema:
          $ref: '#/definitions/holder'
      - in: formData
        name: context
        description: Dictionary of variable names and their values
      - in: path
        name: id
        description: ID string of API Call
      - in: formData
        name: location_id
        description: Location ID of test agent that will make the request
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Calls
      - ""
      - Run
  /calls/{id}/stats/before:
    get:
      summary: List Stats from before a date for an API Call
      description: List Stats from before a date for an API Call
      operationId: listStatsFromBeforeDateAPICall
      x-api-path-slug: callsidstatsbefore-get
      parameters:
      - in: path
        name: id
        description: ID string of API Call
      - in: query
        name: kind
        description: Granularity of data required, one of DAY, WEEK, MONTH, YEAR
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: location_id
        description: Location where the API Call was made
      - in: query
        name: time
        description: ISO formatted date string for the end of the period you wish
          to view
      - in: query
        name: type
        description: Return stats for all calls in the time period specified which
          had this result
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Calls
      - ""
      - Stats
      - Before
  /calls/{id}/stats/since:
    get:
      summary: List Stats since a date for an API Call
      description: List Stats since a date for an API Call
      operationId: listStatsSinceDateAPICall
      x-api-path-slug: callsidstatssince-get
      parameters:
      - in: path
        name: id
        description: ID string of API Call
      - in: query
        name: kind
        description: Granularity of data required, one of DAY, WEEK, MONTH, YEAR
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: location_id
        description: Location where the API Call was made
      - in: query
        name: time
        description: ISO formatted date string for the start of the period you wish
          to view
      - in: query
        name: type
        description: Return stats for all calls in the time period specified which
          had this result
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Calls
      - ""
      - Stats
      - Since
  /deployments/:
    get:
      summary: List all Deployment
      description: List all Deployment
      operationId: listAllDeployments
      x-api-path-slug: deployments-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Deployments
    post:
      summary: Create a new Deployment
      description: Create a new Deployment
      operationId: createANewDeployment
      x-api-path-slug: deployments-post
      parameters:
      - in: body
        name: body
        description: '{     deployment: {         target_id: agxkZXZ-dmlhdGVzdHNyFwsSClRlc3RTZXR1cDIYgICAgKDL6gsM,          frequency:
          12,         location_id:      } }'
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Deployments
  /deployments/call/{call_id}/:
    get:
      summary: Get all Deployments for an API Call
      description: Get all Deployments for an API Call
      operationId: getAllDeploymentForAPICall
      x-api-path-slug: deploymentscallcall-id-get
      parameters:
      - in: path
        name: call_id
        description: ID of the API Call
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Deployments
      - Call
      - Call
  /deployments/workflow/{workflow_id}:
    get:
      summary: Get all Deployments for a Workflow
      description: Get all Deployments for a Workflow
      operationId: getAllDeploymentForAWorkflow
      x-api-path-slug: deploymentsworkflowworkflow-id-get
      parameters:
      - in: path
        name: workflow_id
        description: ID of the Workflow
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Deployments
      - Workflow
      - Workflow
  /deployments/{id}/:
    delete:
      summary: Delete a Deployment
      description: Delete a Deployment
      operationId: deleteADeployment
      x-api-path-slug: deploymentsid-delete
      parameters:
      - in: path
        name: id
        description: ID string of deployment you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Deployments
    get:
      summary: Get an existing Deployment
      description: Get an existing Deployment
      operationId: getAnExistingDeployment
      x-api-path-slug: deploymentsid-get
      parameters:
      - in: path
        name: id
        description: ID string of deployment you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Deployments
    put:
      summary: Update an existing Deployment
      description: Update an existing Deployment
      operationId: updateAnExistingDeployment
      x-api-path-slug: deploymentsid-put
      parameters:
      - in: body
        name: body
        description: '{     deployment: {         target_id: __PARENT_ID__,          frequency:
          15,         location_id:      } }'
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID string of deployment you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Deployments
  /reports/:
    get:
      summary: List all Reports
      description: List all Reports
      operationId: listAllReports
      x-api-path-slug: reports-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Reports
    post:
      summary: Create a new Report
      description: Create a new Report
      operationId: createANewReport
      x-api-path-slug: reports-post
      parameters:
      - in: body
        name: body
        description: '{     meta: {         name: Minimal Report name     } }'
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Reports
  /reports/{id}/:
    delete:
      summary: Delete a Report
      description: Delete a Report
      operationId: deleteAReport
      x-api-path-slug: reportsid-delete
      parameters:
      - in: path
        name: id
        description: ID string of Report you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Reports
    get:
      summary: Get an existing Report
      description: Get an existing Report
      operationId: getAnExistingReport
      x-api-path-slug: reportsid-get
      parameters:
      - in: path
        name: id
        description: ID string of Report you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Reports
    put:
      summary: Update an existing Report
      description: Update an existing Report
      operationId: updateAnExistingReport
      x-api-path-slug: reportsid-put
      parameters:
      - in: body
        name: body
        description: '{     meta: {         name: Minimal Report name bad create     },     groups:
          [         {             name: Group Name,             rows: [                 {                     call_id:
          __PARENT_ID__,                     location_id:                  },                 {                     call_id:
          __PARENT_ID__,                     location_id:                  }             ]         },         {             name:
          Group Name 2,             rows: ['
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID string of Report you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Reports
  /tokens/:
    get:
      summary: List Auth Tokens
      description: List Auth Tokens
      operationId: listAuthTokens
      x-api-path-slug: tokens-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tokens
    post:
      summary: Create a new Auth Token
      description: Create a new Auth Token
      operationId: createANewAuthToken
      x-api-path-slug: tokens-post
      parameters:
      - in: body
        name: body
        description: '{     meta: {         auth_id: agxkZXZ-dmlhdGVzdHNyGgsSDVNlcnZpY2VDb25maWcYgICAgKDLmgsM,         name:
          Minimal token name     } }'
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tokens
  /tokens/auth/{auth_id}/:
    get:
      summary: Get all tokens for an Authentication Setting
      description: Get all tokens for an Authentication Setting
      operationId: getAllTokensForAnAuthenticationSetting
      x-api-path-slug: tokensauthauth-id-get
      parameters:
      - in: path
        name: auth_id
        description: ID of the Authentication Settings
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tokens
      - Auth
      - Auth
  /tokens/{id}/:
    delete:
      summary: Delete an Auth Token
      description: Delete an Auth Token
      operationId: deleteAnAuthToken
      x-api-path-slug: tokensid-delete
      parameters:
      - in: path
        name: id
        description: ID string of Token you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tokens
    get:
      summary: Get an existing Auth Token
      description: Get an existing Auth Token
      operationId: getAnExistingAuthToken
      x-api-path-slug: tokensid-get
      parameters:
      - in: path
        name: id
        description: ID string of Token you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tokens
    put:
      summary: Update an Auth Token
      description: Update an Auth Token
      operationId: updateAnAuthToken
      x-api-path-slug: tokensid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID string of Token you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tokens
  /workflows/:
    get:
      summary: List all Workflows
      description: List all Workflows
      operationId: listAllWorkflows
      x-api-path-slug: workflows-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Workflows
    post:
      summary: Create new Authentication Settings
      description: Create new Authentication Settings
      operationId: createNewAuthenticationSettings
      x-api-path-slug: workflows-post
      parameters:
      - in: body
        name: body
        description: '{     meta: {         name: Minimal Auth Settings name,         domain:
          httpbin'
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Workflows
  /workflows/{id}/:
    delete:
      summary: Delete a Workflow
      description: Delete a Workflow
      operationId: deleteAWorkflow
      x-api-path-slug: workflowsid-delete
      parameters:
      - in: path
        name: id
        description: ID string of Workflow you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Workflows
    get:
      summary: Get an existing Workflow
      description: Get an existing Workflow
      operationId: getAnExistingWorkflow
      x-api-path-slug: workflowsid-get
      parameters:
      - in: path
        name: id
        description: ID string of Workflow you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Workflows
    post:
      summary: Trigger a Workflow to run now
      description: Trigger a Workflow to run now
      operationId: triggerAWorkflowToRunNow
      x-api-path-slug: workflowsid-post
      parameters:
      - in: body
        name: body
        description: '{     location_id: ,     context: {         foo: 1234,         bar:
          %%RESULT_ID%%,         datum: %%DATETIME%%     } }'
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID string of Workflow you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Workflows
    put:
      summary: Create a new Workflow
      description: Create a new Workflow
      operationId: createANewWorkflow
      x-api-path-slug: workflowsid-put
      parameters:
      - in: body
        name: body
        description: '{     workflow: {         call_ids: [             agxkZXZ-dmlhdGVzdHNyFwsSClRlc3RTZXR1cDIYgICAgKDL6gsM,             agxkZXZ-dmlhdGVzdHNyFwsSClRlc3RTZXR1cDIYgICAgKDL6gsM         ],         handle_cookies:
          true     } }'
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID string of Workflow you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Workflows