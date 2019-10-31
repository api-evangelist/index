swagger: "2.0"
x-collection-name: Google Cloud User Accounts
x-complete: 1
info:
  title: Cloud User Accounts
  description: creates-and-manages-users-and-groups-for-accessing-google-compute-engine-virtual-machines-
  contact:
    name: Google
    url: https://google.com
  version: vm_alpha
host: www.googleapis.com
basePath: /clouduseraccounts/vm_alpha/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/global/groups:
    get:
      summary: Get Groups
      description: Retrieves the list of groups contained within the specified project.
      operationId: clouduseraccounts.groups.list
      x-api-path-slug: projectglobalgroups-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Group
    post:
      summary: Create Group
      description: Creates a Group resource in the specified project using the data
        included in the request.
      operationId: clouduseraccounts.groups.insert
      x-api-path-slug: projectglobalgroups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Group
  /{project}/global/groups/{groupName}:
    delete:
      summary: Delete Group
      description: Deletes the specified Group resource.
      operationId: clouduseraccounts.groups.delete
      x-api-path-slug: projectglobalgroupsgroupname-delete
      parameters:
      - in: path
        name: groupName
        description: Name of the Group resource to delete
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Group
    get:
      summary: Get Group
      description: Returns the specified Group resource.
      operationId: clouduseraccounts.groups.get
      x-api-path-slug: projectglobalgroupsgroupname-get
      parameters:
      - in: path
        name: groupName
        description: Name of the Group resource to return
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Group
  /{project}/global/groups/{groupName}/addMember:
    post:
      summary: Add User To Group
      description: Adds users to the specified group.
      operationId: clouduseraccounts.groups.addMember
      x-api-path-slug: projectglobalgroupsgroupnameaddmember-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupName
        description: Name of the group for this request
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - User
  /{project}/global/groups/{groupName}/removeMember:
    post:
      summary: Remove Use From Group
      description: Removes users from the specified group.
      operationId: clouduseraccounts.groups.removeMember
      x-api-path-slug: projectglobalgroupsgroupnameremovemember-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupName
        description: Name of the group for this request
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - User
  /{project}/global/groups/{resource}/getIamPolicy:
    get:
      summary: Get IAM Policy
      description: Gets the access control policy for a resource. May be empty if
        no such policy or resource exists.
      operationId: clouduseraccounts.groups.getIamPolicy
      x-api-path-slug: projectglobalgroupsresourcegetiampolicy-get
      parameters:
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: resource
        description: Name of the resource for this request
      responses:
        200:
          description: OK
      tags:
      - IAM
  /{project}/global/groups/{resource}/setIamPolicy:
    post:
      summary: Set IAM Policy
      description: Sets the access control policy on the specified resource. Replaces
        any existing policy.
      operationId: clouduseraccounts.groups.setIamPolicy
      x-api-path-slug: projectglobalgroupsresourcesetiampolicy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: resource
        description: Name of the resource for this request
      responses:
        200:
          description: OK
      tags:
      - IAM
  /{project}/global/groups/{resource}/testIamPermissions:
    post:
      summary: Test IAM Permissions
      description: Returns permissions that a caller has on the specified resource.
      operationId: clouduseraccounts.groups.testIamPermissions
      x-api-path-slug: projectglobalgroupsresourcetestiampermissions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: resource
        description: Name of the resource for this request
      responses:
        200:
          description: OK
      tags:
      - IAM
  /{project}/global/operations:
    get:
      summary: Get Operations
      description: Retrieves the list of operation resources contained within the
        specified project.
      operationId: clouduseraccounts.globalAccountsOperations.list
      x-api-path-slug: projectglobaloperations-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Operation
  /{project}/global/operations/{operation}:
    delete:
      summary: Delete Operation
      description: Deletes the specified operation resource.
      operationId: clouduseraccounts.globalAccountsOperations.delete
      x-api-path-slug: projectglobaloperationsoperation-delete
      parameters:
      - in: path
        name: operation
        description: Name of the Operations resource to delete
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Operation
    get:
      summary: Get Operation
      description: Retrieves the specified operation resource.
      operationId: clouduseraccounts.globalAccountsOperations.get
      x-api-path-slug: projectglobaloperationsoperation-get
      parameters:
      - in: path
        name: operation
        description: Name of the Operations resource to return
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Operation
  /{project}/global/users:
    get:
      summary: Get Users
      description: Retrieves a list of users contained within the specified project.
      operationId: clouduseraccounts.users.list
      x-api-path-slug: projectglobalusers-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - User
    post:
      summary: Create User
      description: Creates a User resource in the specified project using the data
        included in the request.
      operationId: clouduseraccounts.users.insert
      x-api-path-slug: projectglobalusers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - User
  /{project}/global/users/{resource}/getIamPolicy:
    get:
      summary: Get User IAM Policy
      description: Gets the access control policy for a resource. May be empty if
        no such policy or resource exists.
      operationId: clouduseraccounts.users.getIamPolicy
      x-api-path-slug: projectglobalusersresourcegetiampolicy-get
      parameters:
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: resource
        description: Name of the resource for this request
      responses:
        200:
          description: OK
      tags:
      - User IAM
  /{project}/global/users/{resource}/setIamPolicy:
    post:
      summary: Set User IAM Policy
      description: Sets the access control policy on the specified resource. Replaces
        any existing policy.
      operationId: clouduseraccounts.users.setIamPolicy
      x-api-path-slug: projectglobalusersresourcesetiampolicy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: resource
        description: Name of the resource for this request
      responses:
        200:
          description: OK
      tags:
      - User IAM
  /{project}/global/users/{resource}/testIamPermissions:
    post:
      summary: Test User IAM Permissions
      description: Returns permissions that a caller has on the specified resource.
      operationId: clouduseraccounts.users.testIamPermissions
      x-api-path-slug: projectglobalusersresourcetestiampermissions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: resource
        description: Name of the resource for this request
      responses:
        200:
          description: OK
      tags:
      - User IAM
  /{project}/global/users/{user}:
    delete:
      summary: Delete User
      description: Deletes the specified User resource.
      operationId: clouduseraccounts.users.delete
      x-api-path-slug: projectglobalusersuser-delete
      parameters:
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: user
        description: Name of the user resource to delete
      responses:
        200:
          description: OK
      tags:
      - User
    get:
      summary: Get User
      description: Returns the specified User resource.
      operationId: clouduseraccounts.users.get
      x-api-path-slug: projectglobalusersuser-get
      parameters:
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: user
        description: Name of the user resource to return
      responses:
        200:
          description: OK
      tags:
      - User
  /{project}/global/users/{user}/addPublicKey:
    post:
      summary: Add Public Key
      description: Adds a public key to the specified User resource with the data
        included in the request.
      operationId: clouduseraccounts.users.addPublicKey
      x-api-path-slug: projectglobalusersuseraddpublickey-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: user
        description: Name of the user for this request
      responses:
        200:
          description: OK
      tags:
      - Public Key
  /{project}/global/users/{user}/removePublicKey:
    post:
      summary: Remove Public Key
      description: Removes the specified public key from the user.
      operationId: clouduseraccounts.users.removePublicKey
      x-api-path-slug: projectglobalusersuserremovepublickey-post
      parameters:
      - in: query
        name: fingerprint
        description: The fingerprint of the public key to delete
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: user
        description: Name of the user for this request
      responses:
        200:
          description: OK
      tags:
      - Public Key
  /{project}/zones/{zone}/authorizedKeysView/{user}:
    post:
      summary: Get Public Keys
      description: Returns a list of authorized public keys for a specific user account.
      operationId: clouduseraccounts.linux.getAuthorizedKeysView
      x-api-path-slug: projectzoneszoneauthorizedkeysviewuser-post
      parameters:
      - in: query
        name: instance
        description: The fully-qualified URL of the virtual machine requesting the
          view
      - in: query
        name: login
        description: Whether the view was requested as part of a user-initiated login
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: user
        description: The user account for which you want to get a list of authorized
          public keys
      - in: path
        name: zone
        description: Name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Public Key
  /{project}/zones/{zone}/linuxAccountViews:
    post:
      summary: Get Linux Account Views
      description: Retrieves a list of user accounts for an instance within a specific
        project.
      operationId: clouduseraccounts.linux.getLinuxAccountViews
      x-api-path-slug: projectzoneszonelinuxaccountviews-post
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: instance
        description: The fully-qualified URL of the virtual machine requesting the
          views
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: Name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Public Key