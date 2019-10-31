swagger: "2.0"
x-collection-name: Next Caller
x-complete: 1
info:
  title: Next Caller
  description: advanced-caller-id--obtain-name-address-and-email-of-your-inbound-callers-
  version: 1.0.0
host: api.sandbox.nextcaller.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{version}/records/:
    parameters:
      summary: Parameters Version Records
      description: Parameters version records.
      operationId: parametersVersionRecords
      x-api-path-slug: versionrecords-parameters
      responses:
        200:
          description: OK
      tags:
      - Version
      - Records
    get:
      summary: Get Version Records
      description: Returns Nextcaller member detailed info.
      operationId: getVersionRecords
      x-api-path-slug: versionrecords-get
      parameters:
      - in: query
        name: format
        description: 'Specifies a format of response: JSON or XML'
      - in: query
        name: phone
        description: Specifies the callers phone number
      - in: path
        name: version
        description: Specifies a api version
      responses:
        200:
          description: OK
      tags:
      - Version
      - Records
  /{version}/users/{nextcaller_id}/?format={format}:
    parameters:
      summary: Parameters Version Users Nextcaller Format Format
      description: Parameters version users nextcaller format format.
      operationId: parametersVersionUsersNextcallerFormatFormat
      x-api-path-slug: versionusersnextcaller-idformatformat-parameters
      responses:
        200:
          description: OK
      tags:
      - Version
      - Users
      - Nextcaller
      - Id
      - ?format=format
    post:
      summary: Post Version Users Nextcaller Format Format
      description: Allows you to update caller's info on Nextcaller.
      operationId: postVersionUsersNextcallerFormatFormat
      x-api-path-slug: versionusersnextcaller-idformatformat-post
      parameters:
      - in: query
        name: Content-Type
        description: Advanced Caller ID
      - in: header
        name: Content-Type
      - in: path
        name: format
        description: 'Specifies a format of response: JSON or XML'
      - in: path
        name: nextcaller_id
        description: The ID of the user whose profile you wish to edit
      - in: path
        name: version
        description: Specifies a api version
      responses:
        200:
          description: OK
      tags:
      - Version
      - Users
      - Nextcaller
      - Id
      - ?format=format