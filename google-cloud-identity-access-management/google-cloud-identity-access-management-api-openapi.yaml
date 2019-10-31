swagger: "2.0"
x-collection-name: Google Cloud Identity Access Management
x-complete: 1
info:
  title: Google Identity and Access Management (IAM)
  description: manages-identity-and-access-control-for-google-cloud-platform-resources-including-the-creation-of-service-accounts-which-you-can-use-to-authenticate-to-google-and-make-api-calls-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: iam.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/roles:queryGrantableRoles:
    post:
      summary: Query Roles
      description: |-
        Queries roles that can be granted on a particular resource.
        A role is grantable if it can be used as the role in a binding for a policy
        for that resource.
      operationId: iam.roles.queryGrantableRoles
      x-api-path-slug: v1rolesquerygrantableroles-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Role
  /v1/{name}:
    delete:
      summary: Delete Service Account Key
      description: Deletes a ServiceAccountKey.
      operationId: iam.projects.serviceAccounts.keys.delete
      x-api-path-slug: v1name-delete
      parameters:
      - in: path
        name: name
        description: The resource name of the service account key in the following
          format:`projects/{PROJECT_ID}/serviceAccounts/{SERVICE_ACCOUNT_EMAIL}/keys/{key}`
      responses:
        200:
          description: OK
      tags:
      - Service Account Key
    get:
      summary: Get Service Account Key
      description: |-
        Gets the ServiceAccountKey
        by key id.
      operationId: iam.projects.serviceAccounts.keys.get
      x-api-path-slug: v1name-get
      parameters:
      - in: path
        name: name
        description: The resource name of the service account key in the following
          format:`projects/{PROJECT_ID}/serviceAccounts/{SERVICE_ACCOUNT_EMAIL}/keys/{key}`
      - in: query
        name: publicKeyType
        description: The output format of the public key requested
      responses:
        200:
          description: OK
      tags:
      - Service Account Key
    put:
      summary: Update Service Account Key
      description: |-
        Updates a ServiceAccount.

        Currently, only the following fields are updatable:
        `display_name` .
        The `etag` is mandatory.
      operationId: iam.projects.serviceAccounts.update
      x-api-path-slug: v1name-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The resource name of the service account in the following format:`projects/{PROJECT_ID}/serviceAccounts/{SERVICE_ACCOUNT_EMAIL}`
      responses:
        200:
          description: OK
      tags:
      - Service Account Key
  /v1/{name}/keys:
    get:
      summary: Get Service Account Keys
      description: Lists ServiceAccountKeys.
      operationId: iam.projects.serviceAccounts.keys.list
      x-api-path-slug: v1namekeys-get
      parameters:
      - in: query
        name: keyTypes
        description: Filters the types of keys the user wants to include in the listresponse
      - in: path
        name: name
        description: The resource name of the service account in the following format:`projects/{PROJECT_ID}/serviceAccounts/{SERVICE_ACCOUNT_EMAIL}`
      responses:
        200:
          description: OK
      tags:
      - Service Account Key
    post:
      summary: Create Service Account Key
      description: |-
        Creates a ServiceAccountKey
        and returns it.
      operationId: iam.projects.serviceAccounts.keys.create
      x-api-path-slug: v1namekeys-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The resource name of the service account in the following format:`projects/{PROJECT_ID}/serviceAccounts/{SERVICE_ACCOUNT_EMAIL}`
      responses:
        200:
          description: OK
      tags:
      - Service Account Key
  /v1/{name}/serviceAccounts:
    get:
      summary: Get Service Accounts
      description: Lists ServiceAccounts for a project.
      operationId: iam.projects.serviceAccounts.list
      x-api-path-slug: v1nameserviceaccounts-get
      parameters:
      - in: path
        name: name
        description: Required
      - in: query
        name: pageSize
        description: Optional limit on the number of service accounts to include in
          theresponse
      - in: query
        name: pageToken
        description: Optional pagination token returned in an earlierListServiceAccountsResponse
      responses:
        200:
          description: OK
      tags:
      - Service Account
    post:
      summary: Create Service Account
      description: |-
        Creates a ServiceAccount
        and returns it.
      operationId: iam.projects.serviceAccounts.create
      x-api-path-slug: v1nameserviceaccounts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Service Account
  /v1/{name}:signBlob:
    post:
      summary: Sign Blob
      description: Signs a blob using a service account's system-managed private key.
      operationId: iam.projects.serviceAccounts.signBlob
      x-api-path-slug: v1namesignblob-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The resource name of the service account in the following format:`projects/{PROJECT_ID}/serviceAccounts/{SERVICE_ACCOUNT_EMAIL}`
      responses:
        200:
          description: OK
      tags:
      - Blob
  /v1/{name}:signJwt:
    post:
      summary: Sign JWT
      description: |-
        Signs a JWT using a service account's system-managed private key.

        If no expiry time (`exp`) is provided in the `SignJwtRequest`, IAM sets an
        an expiry time of one hour by default. If you request an expiry time of
        more than one hour, the request will fail.
      operationId: iam.projects.serviceAccounts.signJwt
      x-api-path-slug: v1namesignjwt-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The resource name of the service account in the following format:`projects/{PROJECT_ID}/serviceAccounts/{SERVICE_ACCOUNT_EMAIL}`
      responses:
        200:
          description: OK
      tags:
      - JWT
  /v1/{resource}:getIamPolicy:
    post:
      summary: Return IAM Access Control Policy
      description: |-
        Returns the IAM access control policy for a
        ServiceAccount.
      operationId: iam.projects.serviceAccounts.getIamPolicy
      x-api-path-slug: v1resourcegetiampolicy-post
      parameters:
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy is being requested'
      responses:
        200:
          description: OK
      tags:
      - IAM
  /v1/{resource}:setIamPolicy:
    post:
      summary: Set IAM Access Control Policy
      description: |-
        Sets the IAM access control policy for a
        ServiceAccount.
      operationId: iam.projects.serviceAccounts.setIamPolicy
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
      - IAM
  /v1/{resource}:testIamPermissions:
    post:
      summary: Tests Permissions
      description: |-
        Tests the specified permissions against the IAM access control policy
        for a ServiceAccount.
      operationId: iam.projects.serviceAccounts.testIamPermissions
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
      - Permission