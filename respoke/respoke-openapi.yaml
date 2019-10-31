swagger: "2.0"
x-collection-name: Respoke
x-complete: 1
info:
  title: Respoke REST API
  description: add-live-voice-video-text-and-data-features-to-your-website-or-app-
  termsOfService: https://www.respoke.io/files/respoke-tos-20141007.pdf
  version: v1
host: api.respoke.io
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  admin-sessions/:
    post:
      summary: Admin Sessions
      description: Log in with the account username and password. Get an Admin-Token.
      operationId: postAdminSessions
      x-api-path-slug: adminsessions-post
      parameters:
      - in: query
        name: password
        description: Your password
      - in: query
        name: username
        description: Your username
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Sessions
  adminsessions/:
    post:
      summary: Permissions
      description: Full API permissions are obtained by POSTing your username and
        password to [base]/adminsessions.
      operationId: postAdminsessions
      x-api-path-slug: adminsessions-post
      parameters:
      - in: query
        name: password
        description: Your username
      - in: query
        name: username
        description: username
      responses:
        200:
          description: OK
      tags:
      - Adminsessions
  appauthsessions/:
    post:
      summary: App Auth Sessions
      description: Your users authenticate to Respoke using an App-Token obtained
        when they POST your tokenId to [base]/appauthsessions.
      operationId: postAppauthsessions
      x-api-path-slug: appauthsessions-post
      parameters:
      - in: query
        name: App-Token
        description: Your application token
      responses:
        200:
          description: OK
      tags:
      - Appauthsessions
  apps/:
    get:
      summary: Apps
      description: Create an app.
      operationId: getApps
      x-api-path-slug: apps-get
      parameters:
      - in: header
        name: Admin-Token
        description: Your admin token
      responses:
        200:
          description: OK
      tags:
      - Apps
  roles/:
    post:
      summary: Roles
      description: Create roleId and roleName for creating tokens.
      operationId: postRoles
      x-api-path-slug: roles-post
      parameters:
      - schema:
          $ref: '#/definitions/holder'
      - in: header
        name: App-Secret
        description: Your application secret
      responses:
        200:
          description: OK
      tags:
      - Roles
  session-tokens/:
    post:
      summary: Session Tokens
      description: An end-user client posts a tokenId from POST [base]/tokens to authenticate
        to an app as endpointId.
      operationId: postSessionTokens
      x-api-path-slug: sessiontokens-post
      parameters:
      - schema:
          $ref: '#/definitions/holder'
      - in: header
        name: App-Token
        description: Your application token
      responses:
        200:
          description: OK
      tags:
      - Session
      - Tokens
  tokens/:
    post:
      summary: Tokens
      description: Get an access token tokenId for an end-user.
      operationId: postTokens
      x-api-path-slug: tokens-post
      parameters:
      - schema:
          $ref: '#/definitions/holder'
      - in: header
        name: App-Secret
        description: Your application secret
      responses:
        200:
          description: OK
      tags:
      - Tokens
    put:
      summary: Tokens
      description: By using the App-Secret header, you can perform API calls to obtain
        Respoke sessions for your users via POST to [base]/tokens. App-Secrets are
        found in the Dev Console.
      operationId: putTokens
      x-api-path-slug: tokens-put
      parameters:
      - in: query
        name: App-Secret
        description: Your application token
      responses:
        200:
          description: OK
      tags:
      - Tokens
  turn/:
    post:
      summary: Turn
      description: Get TURN credentials.
      operationId: postTurn
      x-api-path-slug: turn-post
      parameters:
      - in: header
        name: App-Token
        description: Get TURN credentials
      responses:
        200:
          description: OK
      tags:
      - Turn