swagger: "2.0"
x-collection-name: Google Cloud Datastore
x-complete: 1
info:
  title: Google Cloud Datastore
  description: accesses-the-schemaless-nosql-database-to-provide-fully-managed-robust-scalable-storage-for-your-application-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: datastore.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/projects/{projectId}:allocateIds:
    post:
      summary: Allocate ID
      description: |-
        Allocates IDs for the given keys, which is useful for referencing an entity
        before it is inserted.
      operationId: datastore.projects.allocateIds
      x-api-path-slug: v1projectsprojectidallocateids-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: The ID of the project against which to make the request
      responses:
        200:
          description: OK
      tags:
      - ID
  /v1/projects/{projectId}:beginTransaction:
    post:
      summary: Begin New Transaction
      description: Begins a new transaction.
      operationId: datastore.projects.beginTransaction
      x-api-path-slug: v1projectsprojectidbegintransaction-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: The ID of the project against which to make the request
      responses:
        200:
          description: OK
      tags:
      - Transaction
  /v1/projects/{projectId}:commit:
    post:
      summary: Commit Transaction
      description: |-
        Commits a transaction, optionally creating, deleting or modifying some
        entities.
      operationId: datastore.projects.commit
      x-api-path-slug: v1projectsprojectidcommit-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: The ID of the project against which to make the request
      responses:
        200:
          description: OK
      tags:
      - Transaction
  /v1/projects/{projectId}:lookup:
    post:
      summary: Lookup Entity by Key
      description: Looks up entities by key.
      operationId: datastore.projects.lookup
      x-api-path-slug: v1projectsprojectidlookup-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: The ID of the project against which to make the request
      responses:
        200:
          description: OK
      tags:
      - Lookup
  /v1/projects/{projectId}:rollback:
    post:
      summary: Rollback Transaction
      description: Rolls back a transaction.
      operationId: datastore.projects.rollback
      x-api-path-slug: v1projectsprojectidrollback-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: The ID of the project against which to make the request
      responses:
        200:
          description: OK
      tags:
      - Transaction
  /v1/projects/{projectId}:runQuery:
    post:
      summary: Queries for Entities
      description: Queries for entities.
      operationId: datastore.projects.runQuery
      x-api-path-slug: v1projectsprojectidrunquery-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: The ID of the project against which to make the request
      responses:
        200:
          description: OK
      tags:
      - Query