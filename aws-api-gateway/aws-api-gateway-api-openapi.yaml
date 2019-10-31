swagger: "2.0"
x-collection-name: AWS API Gateway
x-complete: 1
info:
  title: AWS API Gateway API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    get:
      summary: Root Service
      description: Represents the root of the Amazon API Gateway control service.
      operationId: apiGateway
      x-api-path-slug: get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: UnauthorizedException
        description: TooManyRequestsException
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Root
      - Service
  /apikeys:
    get:
      summary: Get API Keys
      description: Gets the ApiKeys resource representing the set of ApiKey resources
        to identify clients for all of your APIs.
      operationId: apigatewayApi-keys
      x-api-path-slug: apikeys-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
    post:
      summary: Create Key
      description: Creates a new ApiKey resource to represent an API key.
      operationId: apikeyCreate
      x-api-path-slug: apikeys-post
      parameters:
      - in: header
        name: '&quot;description&quot;'
        type: string
      - in: header
        name: '&quot;enabled&quot;'
        type: string
      - in: header
        name: '&quot;name&quot;'
        type: string
      - in: header
        name: '&quot;restApiId&quot;'
        type: string
      - in: header
        name: '&quot;stageKeys&quot;'
        type: string
      - in: header
        name: '&quot;stageName&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: body
        name: restApiId
        description: A list of Stage resources that are associated with the ApiKey
          resource
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: stageName
        description: The stage name in the RestApi that the stage key references
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /restapis:
    post:
      summary: Restapi Create
      description: Creates a new API represented by a RestApi instance in API Gateway.
      operationId: restapiCreate
      x-api-path-slug: restapis-post
      parameters:
      - in: header
        name: '&quot;description&quot;'
        type: string
      - in: header
        name: '&quot;name&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Restapi
      - ""
  /restapis?mode=import&amp;failonwarning=true:
    post:
      summary: Restapi Import
      description: Creates an API from an external API definition.
      operationId: restapiImport
      x-api-path-slug: restapismodeimportampfailonwarningtrue-post
      parameters:
      - in: header
        name: '&quot;$ref&quot;'
        type: string
      - in: header
        name: '&quot;/&quot;'
        type: string
      - in: header
        name: '&quot;200&quot;'
        type: string
      - in: header
        name: '&quot;application/json&quot;'
        type: string
      - in: header
        name: '&quot;basePath&quot;'
        type: string
      - in: header
        name: '&quot;consumes&quot;'
        type: string
      - in: header
        name: '&quot;Content-Type&quot;'
        type: string
      - in: header
        name: '&quot;default&quot;'
        type: string
      - in: header
        name: '&quot;definitions&quot;'
        type: string
      - in: header
        name: '&quot;description&quot;'
        type: string
      - in: header
        name: '&quot;Empty&quot;'
        type: string
      - in: header
        name: '&quot;get&quot;'
        type: string
      - in: header
        name: '&quot;headers&quot;'
        type: string
      - in: header
        name: '&quot;host&quot;'
        type: string
      - in: header
        name: '&quot;httpMethod&quot;'
        type: string
      - in: header
        name: '&quot;info&quot;'
        type: string
      - in: header
        name: '&quot;integration.request.header.Content-Type&quot;'
        type: string
      - in: header
        name: '&quot;method.response.header.Content-Type&quot;'
        type: string
      - in: header
        name: '&quot;passthroughBehavior&quot;'
        type: string
      - in: header
        name: '&quot;paths&quot;'
        type: string
      - in: header
        name: '&quot;produces&quot;'
        type: string
      - in: header
        name: '&quot;requestParameters&quot;'
        type: string
      - in: header
        name: '&quot;requestTemplates&quot;'
        type: string
      - in: header
        name: '&quot;responseParameters&quot;'
        type: string
      - in: header
        name: '&quot;responses&quot;'
        type: string
      - in: header
        name: '&quot;responseTemplates&quot;'
        type: string
      - in: header
        name: '&quot;schema&quot;'
        type: string
      - in: header
        name: '&quot;schemes&quot;'
        type: string
      - in: header
        name: '&quot;statusCode&quot;'
        type: string
      - in: header
        name: '&quot;swagger&quot;'
        type: string
      - in: header
        name: '&quot;title&quot;'
        type: string
      - in: header
        name: '&quot;type&quot;'
        type: string
      - in: header
        name: '&quot;x-amazon-apigateway-integration&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Import
  /apikeys/hzYAVO9Sg98nsNh65VfX81M84O2kyXVy6K1xwHD7:
    get:
      summary: Get API Key
      description: Gets the ApiKey resource with the specified key identifier.
      operationId: apikeyBy-key
      x-api-path-slug: apikeyshzyavo9sg98nsnh65vfx81m84o2kyxvy6k1xwhd7-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
    patch:
      summary: Apikey Update
      description: Changes an API key properties, including the description, enabled,
        and name properties.
      operationId: apikeyUpdate
      x-api-path-slug: apikeyshzyavo9sg98nsnh65vfx81m84o2kyxvy6k1xwhd7-patch
      parameters:
      - in: header
        name: '&quot;op&quot;'
        type: string
      - in: header
        name: '&quot;patchOperations&quot;'
        type: string
      - in: header
        name: '&quot;path&quot;'
        type: string
      - in: header
        name: '&quot;value&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: body
        name: from
        description: Not supported
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: body
        name: op
        description: An update operation to be performed with this PATCH request
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: path
        description: The op operation&#39;s target, as identified by a JSON Pointer
          value that references a location within the targeted resource
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: body
        name: value
        description: The new target value of the update operation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /apikeys?mode=import&amp;format=csv&amp;failonwarnings=false:
    post:
      summary: Imports One Or More API Keys
      description: Imports one or more API keys.
      operationId: apikeyImport
      x-api-path-slug: apikeysmodeimportampformatcsvampfailonwarningsfalse-post
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
      - Imports
  /account:
    patch:
      summary: Account Update
      description: Changes information about the associated Account resource.
      operationId: accountUpdate
      x-api-path-slug: account-patch
      parameters:
      - in: header
        name: '&quot;op&quot;'
        type: string
      - in: header
        name: '&quot;patchOperations&quot;'
        type: string
      - in: header
        name: '&quot;path&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: body
        name: from
        description: Not supported
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: body
        name: op
        description: An update operation to be performed with this PATCH request
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: path
        description: The op operation&#39;s target, as identified by a JSON Pointer
          value that references a location within the targeted resource
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: body
        name: value
        description: The new target value of the update operation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account
  /apikeys/a2TprUZuzf2EKbbmMUotDaHYGg8kgxFypcarGved:
    delete:
      summary: Deletes An Api Key Resource
      description: Deletes an ApiKey resource.
      operationId: apikeyDelete
      x-api-path-slug: apikeysa2tpruzuzf2ekbbmmuotdahygg8kgxfypcargved-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key
      - Resource
  /restapis/mxsmn867vb/authorizers/4unj71:
    delete:
      summary: Authorizer Delete
      description: Deletes an authorizer.
      operationId: authorizerDelete
      x-api-path-slug: restapismxsmn867vbauthorizers4unj71-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: REST API Reference
        description: Link Relations
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Authorizer
  /restapis/mxsmn867vb/authorizers/40j2n8:
    get:
      summary: Authorizer Byid
      description: Gets the Authorizer resource representing a custom authorizer of
        a specified identifier.
      operationId: authorizerBy-id
      x-api-path-slug: restapismxsmn867vbauthorizers40j2n8-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Authorizer
  /restapis/mxsmn867vb/authorizers:
    post:
      summary: Authorizer Create
      description: Creates an Authorizer resource.
      operationId: authorizerCreate
      x-api-path-slug: restapismxsmn867vbauthorizers-post
      parameters:
      - in: header
        name: '&quot;authorizerResultTtlInSeconds&quot;'
        type: string
      - in: header
        name: '&quot;authType&quot;'
        type: string
      - in: header
        name: '&quot;identitySource&quot;'
        type: string
      - in: header
        name: '&quot;name&quot;'
        type: string
      - in: header
        name: '&quot;type&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Authorizer
  /clientcertificates/9ao60f:
    get:
      summary: Clientcertificate Byid
      description: Gets the ClientCertificate resource with the specified identifier.
      operationId: clientcertificateBy-id
      x-api-path-slug: clientcertificates9ao60f-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
      - Byid
  /clientcertificates:
    post:
      summary: Clientcertificate Generate
      description: Generates a new ClientCertificate resource.
      operationId: clientcertificateGenerate
      x-api-path-slug: clientcertificates-post
      parameters:
      - in: header
        name: '&quot;description&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
      - Generate
  /restapis/fugvjdxtri/deployments/dzacq7:
    patch:
      summary: Deployment Update
      description: Changes information about the deployment resource.
      operationId: deploymentUpdate
      x-api-path-slug: restapisfugvjdxtrideploymentsdzacq7-patch
      parameters:
      - in: header
        name: '&quot;op&quot;'
        type: string
      - in: header
        name: '&quot;patchOperations&quot;'
        type: string
      - in: header
        name: '&quot;path&quot;'
        type: string
      - in: header
        name: '&quot;value&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: body
        name: from
        description: Not supported
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: body
        name: op
        description: An update operation to be performed with this PATCH request
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: path
        description: The op operation&#39;s target, as identified by a JSON Pointer
          value that references a location within the targeted resource
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: value
        description: The new target value of the update operation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment
    delete:
      summary: Deployment Delete
      description: Deletes the deployment resource.
      operationId: deploymentDelete
      x-api-path-slug: restapisfugvjdxtrideploymentsdzacq7-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment
  /domainnames/mon-api.com:
    delete:
      summary: Domainname Delete
      description: Deletes the domain name resource.
      operationId: domainnameDelete
      x-api-path-slug: domainnamesmonapi-com-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domainname
  /domainnames/a.b.c.com/basepathmappings:
    get:
      summary: Get Domain Base Path
      description: Gets the BasePathMappings resource representing the collection
        of base path mappings for the specified custom domain name.
      operationId: domainnameBasepathmappings
      x-api-path-slug: domainnamesa-b-c-combasepathmappings-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domain
      - Base
      - Path
  /restapis/fugvjdxtri/resources/3kzxbg5sa2/methods/GET/integration/responses/200:
    patch:
      summary: Integrationresponse Update
      description: Changes information about an integration response.
      operationId: integrationresponseUpdate
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsgetintegrationresponses200-patch
      parameters:
      - in: header
        name: '&quot;op&quot;'
        type: string
      - in: header
        name: '&quot;patchOperations&quot;'
        type: string
      - in: header
        name: '&quot;path&quot;'
        type: string
      - in: header
        name: '&quot;value&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: body
        name: from
        description: Not supported
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: body
        name: op
        description: An update operation to be performed with this PATCH request
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: path
        description: The op operation&#39;s target, as identified by a JSON Pointer
          value that references a location within the targeted resource
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: value
        description: The new target value of the update operation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Integrations
    delete:
      summary: Integration Delete
      description: Deletes an integration response.
      operationId: integrationresponseDelete
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsgetintegrationresponses200-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Integrations
    put:
      summary: Integrationresponse Put
      description: Set up an IntegrationResponse for the integration.
      operationId: integrationresponsePut
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsgetintegrationresponses200-put
      parameters:
      - in: header
        name: '&quot;method.response.header.Content-Type&quot;'
        type: string
      - in: header
        name: '&quot;responseParameters&quot;'
        type: string
      - in: header
        name: '&quot;selectionPattern&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: body
        name: 'CONVERT_TO_BINARY: Converts a response payload from a Base64-encoded
          string to the corresponding binary blob.'
        description: 'CONVERT_TO_TEXT: Converts a response payload from a binary blob
          to a Base64-encoded string'
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Integrations
    get:
      summary: Integration Responses
      description: Specifies the integration&#39;s responses.
      operationId: integrationResponses
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsgetintegrationresponses200-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Integrations
      - Responses
  /restapis/fugvjdxtri/resources/3kzxbg5sa2/methods/GET/integration:
    patch:
      summary: Integration Update
      description: Changes information about an integration.
      operationId: integrationUpdate
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsgetintegration-patch
      parameters:
      - in: header
        name: '&quot;op&quot;'
        type: string
      - in: header
        name: '&quot;patchOperations&quot;'
        type: string
      - in: header
        name: '&quot;path&quot;'
        type: string
      - in: header
        name: '&quot;value&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: body
        name: from
        description: Not supported
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: body
        name: op
        description: An update operation to be performed with this PATCH request
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: path
        description: The op operation&#39;s target, as identified by a JSON Pointer
          value that references a location within the targeted resource
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: value
        description: The new target value of the update operation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Integration
    delete:
      summary: Integration Delete
      description: Deletes an integration.
      operationId: integrationDelete
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsgetintegration-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Integration
    put:
      summary: Integration Put
      description: Set up the method&#39;s integration request.
      operationId: integrationPut
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsgetintegration-put
      parameters:
      - in: header
        name: '&quot;application/json&quot;'
        type: string
      - in: header
        name: '&quot;httpMethod&quot;'
        type: string
      - in: header
        name: '&quot;integration.request.header.Content-Type&quot;'
        type: string
      - in: header
        name: '&quot;passthroughBehavior&quot;'
        type: string
      - in: header
        name: '&quot;requestParameters&quot;'
        type: string
      - in: header
        name: '&quot;requestTemplates&quot;'
        type: string
      - in: header
        name: '&quot;type&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: body
        name: WHEN_NO_MATCH passes the request body for unmapped content types through
          to the integration back end without transformation.
        description: NEVER rejects unmapped content types with an HTTP 415 &#39;Unsupported
          Media Type&#39; response
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Integration
      - Put
  /restapis/fugvjdxtri/resources/3kzxbg5sa2/methods/GET/responses/200:
    get:
      summary: Get Response
      description: Represents a method response of a given HTTP status code returned
        to the client. The method response is passed from the back end through the
        associated integration response that can be transformed using a mapping template.
      operationId: methodResponse
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsgetresponses200-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: responseModels
        description: Specifies the Model resources used for the response&#39;s content-type
        type: string
      - in: query
        name: responseParameters
        description: A key-value map specifying required or optional response parameters
          that Amazon API Gateway can send back to the caller
        type: string
      - in: query
        name: statusCode
        description: The method response&#39;s status code
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Response
    put:
      summary: Methodresponse Put
      description: Set up the method response.
      operationId: methodresponsePut
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsgetresponses200-put
      parameters:
      - in: header
        name: '&quot;application/json&quot;'
        type: string
      - in: header
        name: '&quot;method.response.header.Content-Type&quot;'
        type: string
      - in: header
        name: '&quot;responseModels&quot;'
        type: string
      - in: header
        name: '&quot;responseParameters&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Methods
  /restapis/uojnr9hd57/resources/0cjtch/methods/GET/responses/200:
    patch:
      summary: Methodresponse Update
      description: Update MethodResponse resource&#39;s properties.
      operationId: methodresponseUpdate
      x-api-path-slug: restapisuojnr9hd57resources0cjtchmethodsgetresponses200-patch
      parameters:
      - in: header
        name: '&quot;op&quot;'
        type: string
      - in: header
        name: '&quot;patchOperations&quot;'
        type: string
      - in: header
        name: '&quot;path&quot;'
        type: string
      - in: header
        name: '&quot;value&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: body
        name: from
        description: Not supported
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: body
        name: op
        description: An update operation to be performed with this PATCH request
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: path
        description: The op operation&#39;s target, as identified by a JSON Pointer
          value that references a location within the targeted resource
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: value
        description: The new target value of the update operation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Methods
    delete:
      summary: Methodresponse Delete
      description: Deletes method response settings.
      operationId: methodresponseDelete
      x-api-path-slug: restapisuojnr9hd57resources0cjtchmethodsgetresponses200-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Length
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Method
      - Responses
    get:
      summary: Method Responses
      description: Gets a method response associated with a given HTTP status code.
      operationId: methodResponses
      x-api-path-slug: restapisuojnr9hd57resources0cjtchmethodsgetresponses200-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Length
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Method
      - Responses
  /restapis/fugvjdxtri/resources/3kzxbg5sa2/methods/GET:
    patch:
      summary: Method Update
      description: Update the method settings.
      operationId: methodUpdate
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsget-patch
      parameters:
      - in: header
        name: '&quot;op&quot;'
        type: string
      - in: header
        name: '&quot;patchOperations&quot;'
        type: string
      - in: header
        name: '&quot;path&quot;'
        type: string
      - in: header
        name: '&quot;value&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Cache-Control
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: body
        name: from
        description: Not supported
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: body
        name: op
        description: An update operation to be performed with this PATCH request
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: path
        description: The op operation&#39;s target, as identified by a JSON Pointer
          value that references a location within the targeted resource
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: value
        description: The new target value of the update operation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Method
    get:
      summary: Resource Methods
      description: Gets an API resource&#39;s method of a given HTTP verb.
      operationId: resourceMethods
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsget-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource
      - Methods
  /restapis/8ekh4oszgl/resources/4oa3abz7jc/methods/GET:
    delete:
      summary: Method Delete
      description: Delete the method resource.
      operationId: methodDelete
      x-api-path-slug: restapis8ekh4oszglresources4oa3abz7jcmethodsget-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Method
  /restapis/uojnr9hd57/resources/0cjtch/methods/GET/integration:
    get:
      summary: Method Integration
      description: Gets the method&#39;s integration responsible for passing the client-submitted
        request to the back end and performing necessary transformations to make the
        request compliant with the back end.
      operationId: methodIntegration
      x-api-path-slug: restapisuojnr9hd57resources0cjtchmethodsgetintegration-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Length
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Method
      - Integration
  /restapis/uojnr9hd57/models:
    post:
      summary: Model Create
      description: Creates a new Model for this API.
      operationId: modelCreate
      x-api-path-slug: restapisuojnr9hd57models-post
      parameters:
      - in: header
        name: '&quot;contentType&quot;'
        type: string
      - in: header
        name: '&quot;description&quot;'
        type: string
      - in: header
        name: '&quot;name&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Models
  /restapis/uojnr9hd57/models/CalcOutput:
    delete:
      summary: Model Delete
      description: Deletes a model.
      operationId: modelDelete
      x-api-path-slug: restapisuojnr9hd57modelscalcoutput-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Model
  /restapis/uojnr9hd57/models/output/default_template:
    get:
      summary: Model Generatetemplate
      description: Generates a sample mapping template that can be used to transform
        a payload into the structure of a model.
      operationId: modelGenerate-template
      x-api-path-slug: restapisuojnr9hd57modelsoutputdefault-template-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Model
      - Templates
  /restapis/uojnr9hd57/models/output:
    get:
      summary: Model Byname
      description: Gets information about the Model of a specified name.
      operationId: modelBy-name
      x-api-path-slug: restapisuojnr9hd57modelsoutput-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Model
      - Byname
  /restapis/fugvjdxtri/resources/47rxl6:
    post:
      summary: Resource Createchild
      description: Creates a child API resource of a given API resource.
      operationId: resourceCreate-child
      x-api-path-slug: restapisfugvjdxtriresources47rxl6-post
      parameters:
      - in: header
        name: '&quot;pathPart&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource
  /restapis/uojnr9hd57/resources/0cjtch/methods/GET:
    get:
      summary: Method Byhttpmethod
      description: Gets the method (as a Method resource) on a specified API resource
        (as Resource resource) of the given HTTP method type.
      operationId: methodBy-http-method
      x-api-path-slug: restapisuojnr9hd57resources0cjtchmethodsget-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Length
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Method
      - Methods
  /restapis/fugvjdxtri/resources/3kzxbg5sa2:
    get:
      summary: Resource Byid
      description: Gets an API resource of the Resource type for a given resource
        identifier.
      operationId: resourceBy-id
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource
      - Byid
    post:
      summary: Resource Create
      description: Creates an API resource.
      operationId: resourceCreate
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2-post
      parameters:
      - in: header
        name: '&quot;pathPart&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource
      - ""
  /restapis/fugvjdxtri/:
    patch:
      summary: Restapi Update
      description: Changes properties of a RestApi resource.
      operationId: restapiUpdate
      x-api-path-slug: restapisfugvjdxtri-patch
      parameters:
      - in: header
        name: '&quot;op&quot;'
        type: string
      - in: header
        name: '&quot;patchOperations&quot;'
        type: string
      - in: header
        name: '&quot;path&quot;'
        type: string
      - in: header
        name: '&quot;value&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: body
        name: from
        description: Not supported
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: body
        name: op
        description: An update operation to be performed with this PATCH request
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: path
        description: The op operation&#39;s target, as identified by a JSON Pointer
          value that references a location within the targeted resource
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: value
        description: The new target value of the update operation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Restapi
  /restapis/fugvjdxtri/resources:
    get:
      summary: Restapi Resources
      description: Gets an API&#39;s resource collection as represented by a Resources
        instance.
      operationId: restapiResources
      x-api-path-slug: restapisfugvjdxtriresources-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Restapi
      - Resources
  /restapis/fugvjdxtri/deployments?limit=2:
    get:
      summary: Restapi Deployments
      description: Gets an API&#39;s Deployments resource.
      operationId: restapiDeployments
      x-api-path-slug: restapisfugvjdxtrideploymentslimit2-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Restapi
      - Deployments
  /restapis/l9kujxkzq2/models:
    get:
      summary: Restapi Models
      description: Gets an API&#39;s model collection represented by a Models instance.
      operationId: restapiModels
      x-api-path-slug: restapisl9kujxkzq2models-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Length
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Models
  /restapis/86l3267lf6/authorizers:
    get:
      summary: Restapi Authorizers
      description: Gets an API&#39;s collection of custom authorizers that is represented
        as an Authorizers instance.
      operationId: restapiAuthorizers
      x-api-path-slug: restapis86l3267lf6authorizers-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Length
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Restapi
      - Authorizers
  /restapis/wn611yeyp3?mode=merge:
    put:
      summary: Restapi Put
      description: Update the definition of a REST API, including the resources, methods,
        templates, and models.
      operationId: restapiPut
      x-api-path-slug: restapiswn611yeyp3modemerge-put
      parameters:
      - in: header
        name: '&quot;$ref&quot;'
        type: string
      - in: header
        name: '&quot;/gello&quot;'
        type: string
      - in: header
        name: '&quot;/hello&quot;'
        type: string
      - in: header
        name: '&quot;200&quot;'
        type: string
      - in: header
        name: '&quot;Access-Control-Allow-Headers&quot;'
        type: string
      - in: header
        name: '&quot;Access-Control-Allow-Methods&quot;'
        type: string
      - in: header
        name: '&quot;Access-Control-Allow-Origin&quot;'
        type: string
      - in: header
        name: '&quot;application/json&quot;'
        type: string
      - in: header
        name: '&quot;basePath&quot;'
        type: string
      - in: header
        name: '&quot;consumes&quot;'
        type: string
      - in: header
        name: '&quot;default&quot;'
        type: string
      - in: header
        name: '&quot;definitions&quot;'
        type: string
      - in: header
        name: '&quot;description&quot;'
        type: string
      - in: header
        name: '&quot;Empty&quot;'
        type: string
      - in: header
        name: '&quot;get&quot;'
        type: string
      - in: header
        name: '&quot;headers&quot;'
        type: string
      - in: header
        name: '&quot;host&quot;'
        type: string
      - in: header
        name: '&quot;httpMethod&quot;'
        type: string
      - in: header
        name: '&quot;info&quot;'
        type: string
      - in: header
        name: '&quot;method.response.header.Access-Control-Allow-Headers&quot;'
        type: string
      - in: header
        name: '&quot;method.response.header.Access-Control-Allow-Methods&quot;'
        type: string
      - in: header
        name: '&quot;method.response.header.Access-Control-Allow-Origin&quot;'
        type: string
      - in: header
        name: '&quot;options&quot;'
        type: string
      - in: header
        name: '&quot;passthroughBehavior&quot;'
        type: string
      - in: header
        name: '&quot;paths&quot;'
        type: string
      - in: header
        name: '&quot;post&quot;'
        type: string
      - in: header
        name: '&quot;produces&quot;'
        type: string
      - in: header
        name: '&quot;requestTemplates&quot;'
        type: string
      - in: header
        name: '&quot;responseParameters&quot;'
        type: string
      - in: header
        name: '&quot;responses&quot;'
        type: string
      - in: header
        name: '&quot;schema&quot;'
        type: string
      - in: header
        name: '&quot;schemes&quot;'
        type: string
      - in: header
        name: '&quot;statusCode&quot;'
        type: string
      - in: header
        name: '&quot;swagger&quot;'
        type: string
      - in: header
        name: '&quot;title&quot;'
        type: string
      - in: header
        name: '&quot;type&quot;'
        type: string
      - in: header
        name: '&quot;x-amazon-apigateway-integration&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Restapi
  /restapis/fugvjdxtri/stages/stage1:
    patch:
      summary: Stage Update
      description: Changes information about the stage.
      operationId: stageUpdate
      x-api-path-slug: restapisfugvjdxtristagesstage1-patch
      parameters:
      - in: header
        name: '&quot;op&quot;'
        type: string
      - in: header
        name: '&quot;patchOperations&quot;'
        type: string
      - in: header
        name: '&quot;path&quot;'
        type: string
      - in: header
        name: '&quot;value&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: body
        name: from
        description: Not supported
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: body
        name: op
        description: An update operation to be performed with this PATCH request
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: path
        description: The op operation&#39;s target, as identified by a JSON Pointer
          value that references a location within the targeted resource
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: value
        description: The new target value of the update operation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stage
  /restapis/uycll6xg9a/stages/alpha:
    delete:
      summary: Stage Delete
      description: Deletes a named stage of a given API.
      operationId: stageDelete
      x-api-path-slug: restapisuycll6xg9astagesalpha-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stage
  /restapis/uycll6xg9a/stages/alpha/cache/data:
    delete:
      summary: Stage Flush
      description: Flushes the cached data of a named stage.
      operationId: stageFlush-cache
      x-api-path-slug: restapisuycll6xg9astagesalphacachedata-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stage
      - Flush
  /restapis/uycll6xg9a/stages/alpha/cache/authorizers:
    delete:
      summary: Stage Flush
      description: Flushes all cached Authorizer entries on a named stage.
      operationId: stageFlush-authorizer-cache
      x-api-path-slug: restapisuycll6xg9astagesalphacacheauthorizers-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stage
      - Flush
  /usageplans/{usageplanId}/keys/{keyId}:
    delete:
      summary: Clientcertificate Delete
      description: Deletes the ClientCertificate resource.
      operationId: clientcertificateDelete
      x-api-path-slug: usageplansusageplanidkeyskeyid-delete
      parameters:
      - in: query
        name: Attribute
        description: The AMI attribute
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: ImageId
        description: The ID of the AMI
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certifications
  /clientcertificates/{clientcertificate_id}:
    patch:
      summary: Clientcertificate Update
      description: Changes information about the ClientCertificate resource.
      operationId: clientcertificateUpdate
      x-api-path-slug: clientcertificatesclientcertificate-id-patch
      parameters:
      - in: header
        name: '&quot;op&quot;'
        type: string
      - in: header
        name: '&quot;patchOperations&quot;'
        type: string
      - in: header
        name: '&quot;path&quot;'
        type: string
      - in: header
        name: '&quot;value&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: ExecutableBy.N
        description: Scopes the images by users with explicit launch permissions
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: body
        name: from
        description: Not supported
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: query
        name: ImageId.N
        description: One or more image IDs
        type: string
      - in: body
        name: op
        description: An update operation to be performed with this PATCH request
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: Owner.N
        description: Filters the images by the owner
        type: string
      - in: body
        name: path
        description: The op operation&#39;s target, as identified by a JSON Pointer
          value that references a location within the targeted resource
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: value
        description: The new target value of the update operation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates