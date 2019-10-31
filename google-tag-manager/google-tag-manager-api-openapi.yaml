swagger: "2.0"
x-collection-name: Google Tag Manager
x-complete: 1
info:
  title: Tag Manager
  description: accesses-tag-manager-accounts-and-containers-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tagmanager/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts:
    get:
      summary: Get Accounts
      description: Lists all GTM Accounts that a user has access to.
      operationId: tagmanager.accounts.list
      x-api-path-slug: accounts-get
      responses:
        200:
          description: OK
      tags:
      - Account
  /accounts/{accountId}:
    get:
      summary: Get Account
      description: Gets a GTM Account.
      operationId: tagmanager.accounts.get
      x-api-path-slug: accountsaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      responses:
        200:
          description: OK
      tags:
      - Account
    put:
      summary: Update Account
      description: Updates a GTM Account.
      operationId: tagmanager.accounts.update
      x-api-path-slug: accountsaccountid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the account in storage
      responses:
        200:
          description: OK
      tags:
      - Account
  /accounts/{accountId}/containers:
    get:
      summary: Get Conainers
      description: Lists all Containers that belongs to a GTM Account.
      operationId: tagmanager.accounts.containers.list
      x-api-path-slug: accountsaccountidcontainers-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      responses:
        200:
          description: OK
      tags:
      - Container
    post:
      summary: Create Container
      description: Creates a Container.
      operationId: tagmanager.accounts.containers.create
      x-api-path-slug: accountsaccountidcontainers-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Container
  /accounts/{accountId}/containers/{containerId}:
    delete:
      summary: Delete Container
      description: Deletes a Container.
      operationId: tagmanager.accounts.containers.delete
      x-api-path-slug: accountsaccountidcontainerscontainerid-delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - Container
    get:
      summary: Get Container
      description: Gets a Container.
      operationId: tagmanager.accounts.containers.get
      x-api-path-slug: accountsaccountidcontainerscontainerid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - Container
    put:
      summary: Update Container
      description: Updates a Container.
      operationId: tagmanager.accounts.containers.update
      x-api-path-slug: accountsaccountidcontainerscontainerid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the container in storage
      responses:
        200:
          description: OK
      tags:
      - Container
  /accounts/{accountId}/containers/{containerId}/environments:
    get:
      summary: Get GTM Environments
      description: Lists all GTM Environments of a GTM Container.
      operationId: tagmanager.accounts.containers.environments.list
      x-api-path-slug: accountsaccountidcontainerscontaineridenvironments-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Environment
    post:
      summary: Create GTM Environment
      description: Creates a GTM Environment.
      operationId: tagmanager.accounts.containers.environments.create
      x-api-path-slug: accountsaccountidcontainerscontaineridenvironments-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Environment
  /accounts/{accountId}/containers/{containerId}/environments/{environmentId}:
    delete:
      summary: Delete GTM Environment
      description: Deletes a GTM Environment.
      operationId: tagmanager.accounts.containers.environments.delete
      x-api-path-slug: accountsaccountidcontainerscontaineridenvironmentsenvironmentid-delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: environmentId
        description: The GTM Environment ID
      responses:
        200:
          description: OK
      tags:
      - GTM Environment
    get:
      summary: Get GTM Environment
      description: Gets a GTM Environment.
      operationId: tagmanager.accounts.containers.environments.get
      x-api-path-slug: accountsaccountidcontainerscontaineridenvironmentsenvironmentid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: environmentId
        description: The GTM Environment ID
      responses:
        200:
          description: OK
      tags:
      - GTM Environment
    patch:
      summary: Update GTM Environment
      description: Updates a GTM Environment. This method supports patch semantics.
      operationId: tagmanager.accounts.containers.environments.patch
      x-api-path-slug: accountsaccountidcontainerscontaineridenvironmentsenvironmentid-patch
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: environmentId
        description: The GTM Environment ID
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the environment in storage
      responses:
        200:
          description: OK
      tags:
      - GTM Environment
    put:
      summary: Update GTM Environment
      description: Updates a GTM Environment.
      operationId: tagmanager.accounts.containers.environments.update
      x-api-path-slug: accountsaccountidcontainerscontaineridenvironmentsenvironmentid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: environmentId
        description: The GTM Environment ID
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the environment in storage
      responses:
        200:
          description: OK
      tags:
      - GTM Environment
  /accounts/{accountId}/containers/{containerId}/folders:
    get:
      summary: Get GTM Folders
      description: Lists all GTM Folders of a Container.
      operationId: tagmanager.accounts.containers.folders.list
      x-api-path-slug: accountsaccountidcontainerscontaineridfolders-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Folder
    post:
      summary: Create GTM Folder
      description: Creates a GTM Folder.
      operationId: tagmanager.accounts.containers.folders.create
      x-api-path-slug: accountsaccountidcontainerscontaineridfolders-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Folder
  /accounts/{accountId}/containers/{containerId}/folders/{folderId}:
    delete:
      summary: Delete GTM Folder
      description: Deletes a GTM Folder.
      operationId: tagmanager.accounts.containers.folders.delete
      x-api-path-slug: accountsaccountidcontainerscontaineridfoldersfolderid-delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: folderId
        description: The GTM Folder ID
      responses:
        200:
          description: OK
      tags:
      - GTM Folder
    get:
      summary: Get GTM Folder
      description: Gets a GTM Folder.
      operationId: tagmanager.accounts.containers.folders.get
      x-api-path-slug: accountsaccountidcontainerscontaineridfoldersfolderid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: folderId
        description: The GTM Folder ID
      responses:
        200:
          description: OK
      tags:
      - GTM Folder
    put:
      summary: Update GTM Folder
      description: Updates a GTM Folder.
      operationId: tagmanager.accounts.containers.folders.update
      x-api-path-slug: accountsaccountidcontainerscontaineridfoldersfolderid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the folder in storage
      - in: path
        name: folderId
        description: The GTM Folder ID
      responses:
        200:
          description: OK
      tags:
      - GTM Folder
  /accounts/{accountId}/containers/{containerId}/folders/{folderId}/entities:
    get:
      summary: Get Entities
      description: List all entities in a GTM Folder.
      operationId: tagmanager.accounts.containers.folders.entities.list
      x-api-path-slug: accountsaccountidcontainerscontaineridfoldersfolderidentities-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: folderId
        description: The GTM Folder ID
      responses:
        200:
          description: OK
      tags:
      - Entity
  /accounts/{accountId}/containers/{containerId}/move_folders/{folderId}:
    put:
      summary: Move Entity
      description: Moves entities to a GTM Folder.
      operationId: tagmanager.accounts.containers.move_folders.update
      x-api-path-slug: accountsaccountidcontainerscontaineridmove-foldersfolderid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: folderId
        description: The GTM Folder ID
      - in: query
        name: tagId
        description: The tags to be moved to the folder
      - in: query
        name: triggerId
        description: The triggers to be moved to the folder
      - in: query
        name: variableId
        description: The variables to be moved to the folder
      responses:
        200:
          description: OK
      tags:
      - Entity
  /accounts/{accountId}/containers/{containerId}/reauthorize_environments/{environmentId}:
    put:
      summary: Regenerate Authorization
      description: Re-generates the authorization code for a GTM Environment.
      operationId: tagmanager.accounts.containers.reauthorize_environments.update
      x-api-path-slug: accountsaccountidcontainerscontaineridreauthorize-environmentsenvironmentid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: environmentId
        description: The GTM Environment ID
      responses:
        200:
          description: OK
      tags:
      - Authorization
  /accounts/{accountId}/containers/{containerId}/tags:
    get:
      summary: Get GTM Tags
      description: Lists all GTM Tags of a Container.
      operationId: tagmanager.accounts.containers.tags.list
      x-api-path-slug: accountsaccountidcontainerscontaineridtags-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Tag
    post:
      summary: Create GTM Tag
      description: Creates a GTM Tag.
      operationId: tagmanager.accounts.containers.tags.create
      x-api-path-slug: accountsaccountidcontainerscontaineridtags-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Tag
  /accounts/{accountId}/containers/{containerId}/tags/{tagId}:
    delete:
      summary: Delete GTM Tag
      description: Deletes a GTM Tag.
      operationId: tagmanager.accounts.containers.tags.delete
      x-api-path-slug: accountsaccountidcontainerscontaineridtagstagid-delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: tagId
        description: The GTM Tag ID
      responses:
        200:
          description: OK
      tags:
      - GTM Tag
    get:
      summary: Get GTM Tag
      description: Gets a GTM Tag.
      operationId: tagmanager.accounts.containers.tags.get
      x-api-path-slug: accountsaccountidcontainerscontaineridtagstagid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: tagId
        description: The GTM Tag ID
      responses:
        200:
          description: OK
      tags:
      - GTM Tag
    put:
      summary: Update GTM Tag
      description: Updates a GTM Tag.
      operationId: tagmanager.accounts.containers.tags.update
      x-api-path-slug: accountsaccountidcontainerscontaineridtagstagid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the tag in storage
      - in: path
        name: tagId
        description: The GTM Tag ID
      responses:
        200:
          description: OK
      tags:
      - GTM Tag
  /accounts/{accountId}/containers/{containerId}/triggers:
    get:
      summary: Get GTM Triggers
      description: Lists all GTM Triggers of a Container.
      operationId: tagmanager.accounts.containers.triggers.list
      x-api-path-slug: accountsaccountidcontainerscontaineridtriggers-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Trigger
    post:
      summary: Create GTM Trigger
      description: Creates a GTM Trigger.
      operationId: tagmanager.accounts.containers.triggers.create
      x-api-path-slug: accountsaccountidcontainerscontaineridtriggers-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Trigger
  /accounts/{accountId}/containers/{containerId}/triggers/{triggerId}:
    delete:
      summary: Delete GTM Trigger
      description: Deletes a GTM Trigger.
      operationId: tagmanager.accounts.containers.triggers.delete
      x-api-path-slug: accountsaccountidcontainerscontaineridtriggerstriggerid-delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: triggerId
        description: The GTM Trigger ID
      responses:
        200:
          description: OK
      tags:
      - GTM Trigger
    get:
      summary: Get GTM Trigger
      description: Gets a GTM Trigger.
      operationId: tagmanager.accounts.containers.triggers.get
      x-api-path-slug: accountsaccountidcontainerscontaineridtriggerstriggerid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: triggerId
        description: The GTM Trigger ID
      responses:
        200:
          description: OK
      tags:
      - GTM Trigger
    put:
      summary: Update GTM Trigger
      description: Updates a GTM Trigger.
      operationId: tagmanager.accounts.containers.triggers.update
      x-api-path-slug: accountsaccountidcontainerscontaineridtriggerstriggerid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the trigger in storage
      - in: path
        name: triggerId
        description: The GTM Trigger ID
      responses:
        200:
          description: OK
      tags:
      - GTM Trigger
  /accounts/{accountId}/containers/{containerId}/variables:
    get:
      summary: Get GTM Variables
      description: Lists all GTM Variables of a Container.
      operationId: tagmanager.accounts.containers.variables.list
      x-api-path-slug: accountsaccountidcontainerscontaineridvariables-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Variable
    post:
      summary: Create GTM Variable
      description: Creates a GTM Variable.
      operationId: tagmanager.accounts.containers.variables.create
      x-api-path-slug: accountsaccountidcontainerscontaineridvariables-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Variable
  /accounts/{accountId}/containers/{containerId}/variables/{variableId}:
    delete:
      summary: Delete GTM Variable
      description: Deletes a GTM Variable.
      operationId: tagmanager.accounts.containers.variables.delete
      x-api-path-slug: accountsaccountidcontainerscontaineridvariablesvariableid-delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: variableId
        description: The GTM Variable ID
      responses:
        200:
          description: OK
      tags:
      - GTM Variable
    get:
      summary: Get GTM Variable
      description: Gets a GTM Variable.
      operationId: tagmanager.accounts.containers.variables.get
      x-api-path-slug: accountsaccountidcontainerscontaineridvariablesvariableid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: variableId
        description: The GTM Variable ID
      responses:
        200:
          description: OK
      tags:
      - GTM Variable
    put:
      summary: Update GTM Variable
      description: Updates a GTM Variable.
      operationId: tagmanager.accounts.containers.variables.update
      x-api-path-slug: accountsaccountidcontainerscontaineridvariablesvariableid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the variable in storage
      - in: path
        name: variableId
        description: The GTM Variable ID
      responses:
        200:
          description: OK
      tags:
      - GTM Variable
  /accounts/{accountId}/containers/{containerId}/versions:
    get:
      summary: Get Container Versions
      description: Lists all Container Versions of a GTM Container.
      operationId: tagmanager.accounts.containers.versions.list
      x-api-path-slug: accountsaccountidcontainerscontaineridversions-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: query
        name: headers
        description: Retrieve headers only when true
      - in: query
        name: includeDeleted
        description: Also retrieve deleted (archived) versions when true
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Versions
    post:
      summary: Create Container Version
      description: Creates a Container Version.
      operationId: tagmanager.accounts.containers.versions.create
      x-api-path-slug: accountsaccountidcontainerscontaineridversions-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Versions
  /accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}:
    delete:
      summary: Delete Container Version
      description: Deletes a Container Version.
      operationId: tagmanager.accounts.containers.versions.delete
      x-api-path-slug: accountsaccountidcontainerscontaineridversionscontainerversionid-delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: containerVersionId
        description: The GTM Container Version ID
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Versions
    get:
      summary: Get Container Version
      description: Gets a Container Version.
      operationId: tagmanager.accounts.containers.versions.get
      x-api-path-slug: accountsaccountidcontainerscontaineridversionscontainerversionid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: containerVersionId
        description: The GTM Container Version ID
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Versions
    put:
      summary: Update Container Version
      description: Updates a Container Version.
      operationId: tagmanager.accounts.containers.versions.update
      x-api-path-slug: accountsaccountidcontainerscontaineridversionscontainerversionid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: containerVersionId
        description: The GTM Container Version ID
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the container version in storage
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Versions
  /accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}/publish:
    post:
      summary: Publish Container Version
      description: Publishes a Container Version.
      operationId: tagmanager.accounts.containers.versions.publish
      x-api-path-slug: accountsaccountidcontainerscontaineridversionscontainerversionidpublish-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: containerVersionId
        description: The GTM Container Version ID
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the container version in storage
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Versions
  /accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}/restore:
    post:
      summary: Restore Container Version
      description: Restores a Container Version. This will overwrite the container's
        current configuration (including its variables, triggers and tags). The operation
        will not have any effect on the version that is being served (i.e. the published
        version).
      operationId: tagmanager.accounts.containers.versions.restore
      x-api-path-slug: accountsaccountidcontainerscontaineridversionscontainerversionidrestore-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: containerVersionId
        description: The GTM Container Version ID
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Versions
  /accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}/undelete:
    post:
      summary: Undelete Container Version
      description: Undeletes a Container Version.
      operationId: tagmanager.accounts.containers.versions.undelete
      x-api-path-slug: accountsaccountidcontainerscontaineridversionscontainerversionidundelete-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: containerVersionId
        description: The GTM Container Version ID
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Versions
  /accounts/{accountId}/permissions:
    get:
      summary: Get User Permissions
      description: List all users that have access to the account along with Account
        and Container Permissions granted to each of them.
      operationId: tagmanager.accounts.permissions.list
      x-api-path-slug: accountsaccountidpermissions-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      responses:
        200:
          description: OK
      tags:
      - User Permission
    post:
      summary: Create User Permission
      description: Creates a user's Account & Container Permissions.
      operationId: tagmanager.accounts.permissions.create
      x-api-path-slug: accountsaccountidpermissions-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - User Permission
  /accounts/{accountId}/permissions/{permissionId}:
    delete:
      summary: Remove User
      description: Removes a user from the account, revoking access to it and all
        of its containers.
      operationId: tagmanager.accounts.permissions.delete
      x-api-path-slug: accountsaccountidpermissionspermissionid-delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: permissionId
        description: The GTM User ID
      responses:
        200:
          description: OK
      tags:
      - User
    get:
      summary: Get User
      description: Gets a user's Account & Container Permissions.
      operationId: tagmanager.accounts.permissions.get
      x-api-path-slug: accountsaccountidpermissionspermissionid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: permissionId
        description: The GTM User ID
      responses:
        200:
          description: OK
      tags:
      - User
    put:
      summary: Update User
      description: Updates a user's Account & Container Permissions.
      operationId: tagmanager.accounts.permissions.update
      x-api-path-slug: accountsaccountidpermissionspermissionid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: permissionId
        description: The GTM User ID
      responses:
        200:
          description: OK
      tags:
      - User