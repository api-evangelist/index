swagger: "2.0"
x-collection-name: SmartBear Software
x-complete: 1
info:
  title: Ready! API TestServer API
  description: a-rest-api-based-api-testing-framework-submit-json-test-recipes-using-your-favorite-http-client-or-one-of-the-existing-opensource-clientstools-on-github--to-run-api-tests-either-asynchronously-or-synchronously-java-client-httpsgithub-comsmartbearreadyapitestserverclient-maven-plugin-httpsgithub-comolensmarreadyapitestservermavenplugin---nodejs-cli-httpsgithub-comolensmarreadyapitestservercli-testrecipe-from-swagger-generator-httpsgithub-comolensmartestserverswaggercodegen-cucumber-integration-httpsgithub-comolensmartestservercucumbercheck-out-samples-at-httpsgithub-comsmartbearreadyapitestserversamples-and-the-documentation-at-httpreadyapi-smartbear-comtestserverstart--try-it-outa-useatyourownrisk-sandbox-is-provided-at-httptestserver-readyapi-io8080--feel-free-to-try-it-out-using-swaggerui-or-any-other-tool-of-your-liking-use-demouserdemopassword-as-your-basic-authentication-credentials--the-sandbox-is-currently-configured-to-support-only-rest-requests-and-propertytransfers--if-you-want-to-try-datasourcesdatasinksscripts-in-your-api-tests-you-will-need-to-install-and-run-your-own-instance-of-the-testserver--download-it-from-httpssmartbear-comproductreadyapitestserveroverview
  contact:
    name: SmartBear Software
    url: http://smartbear.com/testserver
  version: 1.2.1
host: testserver.readyapi.io:8080
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /readyapi/executions:
    get:
      summary: Returns test run results stored on the TestServer.
      description: Use this operation to get results of the latest test runs stored
        on the TestServer.<br/> The number of stored results is [configurable](http://readyapi.smartbear.com/testserver/reference/server_properties).
      operationId: getExecutions
      x-api-path-slug: readyapiexecutions-get
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
      - Executions
    post:
      summary: Runs a test recipe.
      description: Use this operation to send a test recipe to the TestServer. The
        recipe contents is passed in the request body (should be valid JSON contents).
      operationId: postRecipe
      x-api-path-slug: readyapiexecutions-post
      parameters:
      - in: query
        name: async
        description: Specifies when the TestServer replies:`true` - Immediately
      - in: body
        name: body
        description: JSON-based test recipe contents
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: callback
        description: The URL, to which the results will be posted
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
      - Executions
  /readyapi/executions/xml:
    post:
      summary: Executes a Ready! API project.
      description: Use this operation to send a Ready! API test project to the TestServer.
        You command the TestServer to execute the entire project, or an individual
        test suite or test case in it. The recipe request should have a Ready! API
        project file (.xml) attached to it.
      operationId: postProjectExecution
      x-api-path-slug: readyapiexecutionsxml-post
      parameters:
      - in: query
        name: async
        description: Specifies when TestServer replies:`true` - Immediately
      - in: body
        name: body
        description: Ready! API XML project
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: callback
        description: The URL, to which the results will be posted
      - in: query
        name: clientCertFileName
        description: The name of the separately provided client certificate file
      - in: query
        name: clientCertPassword
        description: The password for the separately provided client certificate file
      - in: query
        name: environment
        description: The target environment for tests execution
      - in: query
        name: testCaseName
        description: The name of the test case to run
      - in: query
        name: testSuiteName
        description: The name of the test suite to run
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
      - Executions
  /readyapi/executions/composite:
    post:
      summary: Executes a zipped Ready! API composite project.
      description: Use this operation to send a zipped Ready! API composite project
        to the TestServer. You command the TestServer to execute the entire project,
        or an individual test suite or test case in it. The recipe request should
        have a Ready! API project file (.xml) attached to it.
      operationId: postCompositeProjectExecution
      x-api-path-slug: readyapiexecutionscomposite-post
      parameters:
      - in: query
        name: async
        description: Specifies when TestServer replies:`true` - Immediately
      - in: body
        name: body
        description: Ready! API XML project
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: callback
        description: The URL, to which the results will be posted
      - in: query
        name: clientCertFileName
        description: The name of the separately provided client certificate file
      - in: query
        name: clientCertPassword
        description: The password for the separately provided client certificate file
      - in: query
        name: environment
        description: The target environment for tests execution
      - in: query
        name: testCaseName
        description: The name of the test case to run
      - in: query
        name: testSuiteName
        description: The name of the test suite to run
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
      - Executions
  /readyapi/executions/{executionID}:
    delete:
      summary: Cancels the specified recipe execution
      description: Use this operation to stop the run specified by <i>executionID</i>.
        You can find in the response to your execution request ([see how](http://readyapi.smartbear.com/testserver/tutorials/your_first_recipe/results)),
        or you can send a GET <code>/readyapi/executions</code> request to the TestServer.
      operationId: cancelExecution
      x-api-path-slug: readyapiexecutionsexecutionid-delete
      parameters:
      - in: path
        name: executionID
        description: The id of the test run to stop
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
      - Executions
  /readyapi/executions/{executionID}/status:
    get:
      summary: Returns the status of the specified recipe execution.
      description: Use this operation to get information on the recipe execution specified
        by <i>executionID</i>.  You can find in the response to your execution request
        ([see how](http://readyapi.smartbear.com/testserver/tutorials/your_first_recipe/results)),
        or you can send a GET <code>/readyapi/executions</code> request to the TestServer.
      operationId: getExecutionStatus
      x-api-path-slug: readyapiexecutionsexecutionidstatus-get
      parameters:
      - in: path
        name: executionID
        description: The id of the desired test run
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
      - Executions
  /readyapi/executions/{executionID}/logs:
    get:
      summary: Returns the transaction logs for the specified recipe execution.
      description: Use this operation to get transaction logs (individual request
        and recponse of executed test steps) of the recipe execution specified by
        <i>executionID</i>.  You can find it in the response of your execution request
        ([see how](http://readyapi.smartbear.com/testserver/tutorials/your_first_recipe/results)),
        or you can send a GET <code>/readyapi/executions/{executionID}/logs</code>
        request to the TestServer.
      operationId: getMessageExchanges
      x-api-path-slug: readyapiexecutionsexecutionidlogs-get
      parameters:
      - in: path
        name: executionID
        description: The id of the desired test run
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
      - Executions
  /readyapi/executions/{executionId}/files:
    post:
      summary: Posts a file for the specified test run
      description: Use this operation to send additional files required by the executed
        test recipes. For example, you may need to send an Excel file for your test
        recipe that uses an Excel data source. The test recipe will be in the "PENDING"
        status until it receives the required file. Use the <code>multipart/form-data</code>
        media type for this request.
      operationId: addFile
      x-api-path-slug: readyapiexecutionsexecutionidfiles-post
      parameters:
      - in: query
        name: async
        description: Specifies when the TestServer replies:`true` - Immediately
      - in: body
        name: body
        description: Required file as `form-data`
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: executionId
        description: The id of the test run that waits for the files
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
      - Executions
  /readyapi/executions/{executionID}/transactions/{transactionId}:
    get:
      summary: Gets message exchange for a test step execution transaction
      description: A particular execution of a test step is referred as transaction.
        Use this operation to get the request and response for a transaction in HAR
        format.
      operationId: getMessageExchange
      x-api-path-slug: readyapiexecutionsexecutionidtransactionstransactionid-get
      parameters:
      - in: path
        name: executionID
        description: The id of the test run to get the logs for
      - in: path
        name: transactionId
        description: The id of the transaction (test step execution) to get the message
          exchange (request and response) for
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
      - Executions