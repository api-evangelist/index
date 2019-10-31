swagger: "2.0"
x-collection-name: Google OAuth2
x-complete: 1
info:
  title: Google OAuth2
  description: obtains-enduser-authorization-grants-for-use-with-other-google-apis-
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /oauth2/v2/certs:
    get:
      summary: Get Certificate
      description: Get the certification for this session.
      operationId: oauth2.getCertForOpenIdConnect
      x-api-path-slug: oauth2v2certs-get
      responses:
        200:
          description: OK
      tags:
      - Certificate
      - Certfication
  /oauth2/v2/tokeninfo:
    post:
      summary: Get Token Info
      description: Get the token information for this session.
      operationId: oauth2.tokeninfo
      x-api-path-slug: oauth2v2tokeninfo-post
      parameters:
      - in: query
        name: access_token
      - in: query
        name: id_token
      - in: query
        name: token_handle
      responses:
        200:
          description: OK
      tags:
      - Token
  /oauth2/v2/userinfo:
    get:
      summary: Get User Info
      description: Get the user information for this session.
      operationId: oauth2.userinfo.get
      x-api-path-slug: oauth2v2userinfo-get
      responses:
        200:
          description: OK
      tags:
      - User
  /userinfo/v2/me:
    get:
      summary: Get Me
      description: Get the currently authenticated user for this session.
      operationId: oauth2.userinfo.v2.me.get
      x-api-path-slug: userinfov2me-get
      responses:
        200:
          description: OK
      tags:
      - User