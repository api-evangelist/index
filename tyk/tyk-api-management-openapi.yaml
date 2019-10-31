swagger: "2.0"
x-collection-name: Tyk
x-complete: 1
info:
  title: Tyk Gateway REST API
  description: the-api-for-managing-the-tyk-api-management-gateway-allowing-api-control-over-the-operation-of-a-variety-of-apis-
  termsOfService: https://tyk.io/terms-and-conditions/
  version: "1.9"
host: '{baseURL}'
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tyk/keys/:
    get:
      summary: Get Keys
      description: Gets a list of *key* IDs (will only work with non-hashed installations)
      operationId: gets-a-list-of-key-ids-will-only-work-with-nonhashed-installations
      x-api-path-slug: tykkeys-get
      parameters:
      - in: query
        name: api_id
        description: Back-end to target
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - API Key
  /tyk/keys/create:
    post:
      summary: Create Key
      description: Create a new *API token* with the *session object* defined in the
        body
      operationId: create-a-new-api-token-with-the-session-object-defined-in-the-body
      x-api-path-slug: tykkeyscreate-post
      parameters:
      - in: body
        name: session_object
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: suppress_reset
        description: Adding the `suppress_reset` parameter and setting it to `1`,
          will cause Tyk to not reset the quota limit that is in the current live
          quota manager
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - API Key
  /tyk/keys/{keyId}:
    put:
      summary: Update Key
      description: Update an *API token* with the *session object* defined in the
        body, this operatin overwrites the existing object
      operationId: update-an-api-token-with-the-session-object-defined-in-the-body-this-operatin-overwrites-the-existin
      x-api-path-slug: tykkeyskeyid-put
      parameters:
      - in: query
        name: api_id
        description: Back-end to target
      - in: path
        name: keyId
        description: Access Token
      - in: body
        name: session_object
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: suppress_reset
        description: Adding the `suppress_reset` parameter and setting it to `1`,
          will cause Tyk to not reset the quota limit that is in the current live
          quota manager
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - API Key
    post:
      summary: Add Custom Key
      description: Add a pre-specified *API token* with the *session object* defined
        in the body, this operatin creates a custom token that dsoes not use the gateway
        naming convention for tokens
      operationId: add-a-prespecified-api-token-with-the-session-object-defined-in-the-body-this-operatin-creates-a-cus
      x-api-path-slug: tykkeyskeyid-post
      parameters:
      - in: path
        name: keyId
        description: Access Token
      - in: body
        name: session_object
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - API Key
    delete:
      summary: Remove Key
      description: Remove this *API token* from the gateway, this will completely
        destroy the token and metadata associated with the token and instantly stop
        access from being granted
      operationId: remove-this-api-token-from-the-gateway-this-will-completely-destroy-the-token-and-metadata-associate
      x-api-path-slug: tykkeyskeyid-delete
      parameters:
      - in: query
        name: api_id
        description: Back-end to target
      - in: path
        name: keyId
        description: Access Token
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - API Key
  /tyk/apis/:
    get:
      summary: Get APIs
      description: Gets a list of *API Definition* objects that are currently live
        on the gateway
      operationId: gets-a-list-of-api-definition-objects-that-are-currently-live-on-the-gateway
      x-api-path-slug: tykapis-get
      parameters:
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - API
    post:
      summary: Create API
      description: Create an *API Definition* object
      operationId: create-an-api-definition-object
      x-api-path-slug: tykapis-post
      parameters:
      - in: body
        name: api_definition
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - API
  /tyk/apis/{apiID}:
    get:
      summary: Get API
      description: Gets an *API Definition* object, if it exists
      operationId: gets-an-api-definition-object-if-it-exists
      x-api-path-slug: tykapisapiid-get
      parameters:
      - in: path
        name: apiID
        description: API ID
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - API
    delete:
      summary: Delete API
      description: Deletes an *API Definition* object, if it exists
      operationId: deletes-an-api-definition-object-if-it-exists
      x-api-path-slug: tykapisapiid-delete
      parameters:
      - in: path
        name: apiID
        description: API ID
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - API
    put:
      summary: Update API
      description: Updates an *API Definition* object, if it exists
      operationId: updates-an-api-definition-object-if-it-exists
      x-api-path-slug: tykapisapiid-put
      parameters:
      - in: path
        name: apiID
        description: API ID
      - in: body
        name: api_definition
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - API
  /tyk/health/:
    get:
      summary: Check Health
      description: Gets the health check values for an API if it is being recorded
      operationId: gets-the-health-check-values-for-an-api-if-it-is-being-recorded
      x-api-path-slug: tykhealth-get
      parameters:
      - in: query
        name: api_id
        description: API ID to query
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - API Health
  /tyk/reload/:
    get:
      summary: Reload Gateway
      description: Will reload the targetted gateway
      operationId: will-reload-the-targetted-gateway
      x-api-path-slug: tykreload-get
      parameters:
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - API Reload
  /tyk/reload/group:
    get:
      summary: Reload Group
      description: Will reload the cluster via the targeted gateway
      operationId: will-reload-the-cluster-via-the-targeted-gateway
      x-api-path-slug: tykreloadgroup-get
      parameters:
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - API Reload
  /tyk/oauth/clients/create:
    post:
      summary: OAuth Create Client
      description: Create a new OAuth client
      operationId: create-a-new-oauth-client
      x-api-path-slug: tykoauthclientscreate-post
      parameters:
      - in: body
        name: oauth_client
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - OAuth
  /tyk/oauth/clients/{apiId}/{clientId}:
    delete:
      summary: Delete Client
      description: Delete the OAuth client
      operationId: delete-the-oauth-client
      x-api-path-slug: tykoauthclientsapiidclientid-delete
      parameters:
      - in: path
        name: apiId
        description: API ID that owns this client (back end)
      - in: path
        name: clientId
        description: OAuth Client ID to delete
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - OAuth
  /tyk/oauth/clients/{apiId}:
    get:
      summary: OAuth Get Clients
      description: Get a list of OAuth clients bound to this back end
      operationId: get-a-list-of-oauth-clients-bound-to-this-back-end
      x-api-path-slug: tykoauthclientsapiid-get
      parameters:
      - in: path
        name: apiId
        description: API ID that owns this client (back end)
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - OAuth
  /tyk/oauth/authorize-client/:
    post:
      summary: OAuth Authorize Client
      description: The final request from an authorising party for a redirect URI
        during the Tyk OAuth flow
      operationId: the-final-request-from-an-authorising-party-for-a-redirect-uri-during-the-tyk-oauth-flow
      x-api-path-slug: tykoauthauthorizeclient-post
      parameters:
      - in: formData
        name: client_id
        description: Should be provided by requesting client as part of authorisation
          request
      - in: formData
        name: key_rules
        description: A string representation of a *Session Object (form-encoded)*
      - in: formData
        name: redirect_uri
        description: Should be provided by requesting client as part of authorisation
          request
      - in: formData
        name: response_type
        description: Should be provided by requesting client as part of authorisation
          request, this should be either `code` or `token` depending on the methods
          you have specified for the API
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - OAuth
  /tyk/oauth/refresh/{keyId}:
    delete:
      summary: Invalidate Key
      description: Invalidate a refresh token
      operationId: invalidate-a-refresh-token
      x-api-path-slug: tykoauthrefreshkeyid-delete
      parameters:
      - in: query
        name: apiID
        description: API ID
      - in: path
        name: keyId
        description: Access Token
      - in: header
        name: x-tyk-authorization
        description: tyk gateway shared secret
      responses:
        200:
          description: OK
      tags:
      - OAuth