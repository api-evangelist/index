swagger: "2.0"
x-collection-name: Tropo
x-complete: 1
info:
  title: Tropo
  description: tropo-is-a-cloud-communications-api-and-platform-for-building-scalable-voice-and-sms-applications-
  version: v1
host: api.tropo.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /applications:
    delete:
      summary: Delete Applications
      description: Delete applications.
      operationId: deleteApplications
      x-api-path-slug: applications-delete
      parameters:
      - in: query
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Applications
    get:
      summary: Get Applications
      description: Get applications.
      operationId: getApplications
      x-api-path-slug: applications-get
      parameters:
      - in: query
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Applications
    post:
      summary: Post Applications
      description: Post applications.
      operationId: postApplications
      x-api-path-slug: applications-post
      parameters:
      - in: query
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Applications
    put:
      summary: Put Applications
      description: Put applications.
      operationId: putApplications
      x-api-path-slug: applications-put
      parameters:
      - in: query
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Applications
  /applications/{AppId}/addresses:
    delete:
      summary: Delete Applications Appid Addresses
      description: Delete applications appid addresses.
      operationId: deleteApplicationsAppAddresses
      x-api-path-slug: applicationsappidaddresses-delete
      parameters:
      - in: path
        name: AppId
      - in: query
        name: applicationId
      responses:
        200:
          description: OK
      tags:
      - Applications
      - AppId
      - Addresses
    get:
      summary: Get Applications Appid Addresses
      description: Get applications appid addresses.
      operationId: getApplicationsAppAddresses
      x-api-path-slug: applicationsappidaddresses-get
      parameters:
      - in: path
        name: AppId
      - in: query
        name: applicationId
      responses:
        200:
          description: OK
      tags:
      - Applications
      - AppId
      - Addresses
    post:
      summary: Post Applications Appid Addresses
      description: Post applications appid addresses.
      operationId: postApplicationsAppAddresses
      x-api-path-slug: applicationsappidaddresses-post
      parameters:
      - in: path
        name: AppId
      - in: query
        name: applicationId
      - in: query
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Applications
      - AppId
      - Addresses
  /exchanges:
    get:
      summary: Get Exchanges
      description: Get exchanges.
      operationId: getExchanges
      x-api-path-slug: exchanges-get
      parameters:
      - in: query
        name: applicationId
      responses:
        200:
          description: OK
      tags:
      - Exchanges
  /sessions:
    post:
      summary: Post Sessions
      description: Post sessions.
      operationId: postSessions
      x-api-path-slug: sessions-post
      parameters:
      - in: query
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Sessions