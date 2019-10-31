swagger: "2.0"
x-collection-name: Google Cloud Source Repositories
x-complete: 1
info:
  title: Cloud Source Repositories
  description: access-source-code-repositories-hosted-by-google-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: sourcerepo.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:
    delete:
      summary: Delete Repo
      description: Deletes a repo.
      operationId: sourcerepo.projects.repos.delete
      x-api-path-slug: v1name-delete
      parameters:
      - in: path
        name: name
        description: The name of the repo to delete
      responses:
        200:
          description: OK
      tags:
      - Repository
    get:
      summary: Get Repo
      description: Returns information about a repo.
      operationId: sourcerepo.projects.repos.get
      x-api-path-slug: v1name-get
      parameters:
      - in: path
        name: name
        description: The name of the requested repository
      responses:
        200:
          description: OK
      tags:
      - Repository
  /v1/{name}/repos:
    get:
      summary: Get Repos
      description: Returns all repos belonging to a project.
      operationId: sourcerepo.projects.repos.list
      x-api-path-slug: v1namerepos-get
      parameters:
      - in: path
        name: name
        description: The project ID whose repos should be listed
      responses:
        200:
          description: OK
      tags:
      - Repository
  /v1/{parent}/repos:
    post:
      summary: Create Repo
      description: |-
        Creates a repo in the given project with the given name..

        If the named repository already exists, `CreateRepo` returns
        `ALREADY_EXISTS`.
      operationId: sourcerepo.projects.repos.create
      x-api-path-slug: v1parentrepos-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: parent
        description: The project in which to create the repo
      responses:
        200:
          description: OK
      tags:
      - Repository
  /v1/{resource}:getIamPolicy:
    get:
      summary: Get Access Control Policy
      description: |-
        Gets the access control policy for a resource.
        Returns an empty policy if the resource exists and does not have a policy
        set.
      operationId: sourcerepo.projects.repos.getIamPolicy
      x-api-path-slug: v1resourcegetiampolicy-get
      parameters:
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy is being requested'
      responses:
        200:
          description: OK
      tags:
      - Repository Policy
  /v1/{resource}:setIamPolicy:
    post:
      summary: Set Access Control Policy
      description: |-
        Sets the access control policy on the specified resource. Replaces any
        existing policy.
      operationId: sourcerepo.projects.repos.setIamPolicy
      x-api-path-slug: v1resourcesetiampolicy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy is being specified'
      responses:
        200:
          description: OK
      tags:
      - Repository Policy
  /v1/{resource}:testIamPermissions:
    post:
      summary: Return Permissions
      description: |-
        Returns permissions that a caller has on the specified resource.
        If the resource does not exist, this will return an empty set of
        permissions, not a NOT_FOUND error.
      operationId: sourcerepo.projects.repos.testIamPermissions
      x-api-path-slug: v1resourcetestiampermissions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy detail is being
          requested'
      responses:
        200:
          description: OK
      tags:
      - Repository Policy