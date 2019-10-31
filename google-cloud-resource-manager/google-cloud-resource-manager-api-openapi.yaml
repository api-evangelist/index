swagger: "2.0"
x-collection-name: Google Cloud Resource Manager
x-complete: 1
info:
  title: Google Cloud Resource Manager
  description: the-google-cloud-resource-manager-api-provides-methods-for-creating-reading-and-updating-project-metadata-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: cloudresourcemanager.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/liens:
    get:
      summary: List Liens
      description: |-
        List all Liens applied to the `parent` resource.

        Callers of this method will require permission on the `parent` resource.
        For example, a Lien with a `parent` of `projects/1234` requires permission
        `resourcemanager.projects.get`.
      operationId: cloudresourcemanager.liens.list
      x-api-path-slug: v1liens-get
      parameters:
      - in: query
        name: pageSize
        description: The maximum number of items to return
      - in: query
        name: pageToken
        description: The `next_page_token` value returned from a previous List request,
          if any
      - in: query
        name: parent
        description: The name of the resource to list all attached Liens
      responses:
        200:
          description: OK
      tags:
      - Lien
    post:
      summary: Create Lien
      description: |-
        Create a Lien which applies to the resource denoted by the `parent` field.

        Callers of this method will require permission on the `parent` resource.
        For example, applying to `projects/1234` requires permission
        `resourcemanager.projects.updateLiens`.

        NOTE: Some resources may limit the number of Liens which may be applied.
      operationId: cloudresourcemanager.liens.create
      x-api-path-slug: v1liens-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Lien
  /v1/organizations:search:
    post:
      summary: Search Organization
      description: |-
        Searches Organization resources that are visible to the user and satisfy
        the specified filter. This method returns Organizations in an unspecified
        order. New Organizations do not necessarily appear at the end of the
        results.
      operationId: cloudresourcemanager.organizations.search
      x-api-path-slug: v1organizationssearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organization
  /v1/projects:
    get:
      summary: List Projects
      description: |-
        Lists Projects that are visible to the user and satisfy the
        specified filter. This method returns Projects in an unspecified order.
        New Projects do not necessarily appear at the end of the list.
      operationId: cloudresourcemanager.projects.list
      x-api-path-slug: v1projects-get
      parameters:
      - in: query
        name: filter
        description: An expression for filtering the results of the request
      - in: query
        name: pageSize
        description: The maximum number of Projects to return in the response
      - in: query
        name: pageToken
        description: A pagination token returned from a previous call to ListProjectsthat
          indicates from where listing should continue
      responses:
        200:
          description: OK
      tags:
      - Project
    post:
      summary: Create Project
      description: |-
        Request that a new Project be created. The result is an Operation which
        can be used to track the creation process. It is automatically deleted
        after a few hours, so there is no need to call DeleteOperation.

        Our SLO permits Project creation to take up to 30 seconds at the 90th
        percentile. As of 2016-08-29, we are observing 6 seconds 50th percentile
        latency. 95th percentile latency is around 11 seconds. We recommend
        polling at the 5th second with an exponential backoff.
      operationId: cloudresourcemanager.projects.create
      x-api-path-slug: v1projects-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Project
  /v1/projects/{projectId}:
    delete:
      summary: Delete Project
      description: |-
        Marks the Project identified by the specified
        `project_id` (for example, `my-project-123`) for deletion.
        This method will only affect the Project if the following criteria are met:

        + The Project does not have a billing account associated with it.
        + The Project has a lifecycle state of
        ACTIVE.

        This method changes the Project's lifecycle state from
        ACTIVE
        to DELETE_REQUESTED.
        The deletion starts at an unspecified time,
        at which point the Project is no longer accessible.

        Until the deletion completes, you can check the lifecycle state
        checked by retrieving the Project with GetProject,
        and the Project remains visible to ListProjects.
        However, you cannot update the project.

        After the deletion completes, the Project is not retrievable by
        the  GetProject and
        ListProjects methods.

        The caller must have modify permissions for this Project.
      operationId: cloudresourcemanager.projects.delete
      x-api-path-slug: v1projectsprojectid-delete
      parameters:
      - in: path
        name: projectId
        description: The Project ID (for example, `foo-bar-123`)
      responses:
        200:
          description: OK
      tags:
      - Project
    get:
      summary: Get Project
      description: |-
        Retrieves the Project identified by the specified
        `project_id` (for example, `my-project-123`).

        The caller must have read permissions for this Project.
      operationId: cloudresourcemanager.projects.get
      x-api-path-slug: v1projectsprojectid-get
      parameters:
      - in: path
        name: projectId
        description: The Project ID (for example, `my-project-123`)
      responses:
        200:
          description: OK
      tags:
      - Project
    put:
      summary: Update Project
      description: |-
        Updates the attributes of the Project identified by the specified
        `project_id` (for example, `my-project-123`).

        The caller must have modify permissions for this Project.
      operationId: cloudresourcemanager.projects.update
      x-api-path-slug: v1projectsprojectid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: The project ID (for example, `my-project-123`)
      responses:
        200:
          description: OK
      tags:
      - Project
  /v1/projects/{projectId}:getAncestry:
    post:
      summary: Get Project Ancestry
      description: |-
        Gets a list of ancestors in the resource hierarchy for the Project
        identified by the specified `project_id` (for example, `my-project-123`).

        The caller must have read permissions for this Project.
      operationId: cloudresourcemanager.projects.getAncestry
      x-api-path-slug: v1projectsprojectidgetancestry-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: The Project ID (for example, `my-project-123`)
      responses:
        200:
          description: OK
      tags:
      - Project
  /v1/projects/{projectId}:undelete:
    post:
      summary: Restore Project
      description: |-
        Restores the Project identified by the specified
        `project_id` (for example, `my-project-123`).
        You can only use this method for a Project that has a lifecycle state of
        DELETE_REQUESTED.
        After deletion starts, the Project cannot be restored.

        The caller must have modify permissions for this Project.
      operationId: cloudresourcemanager.projects.undelete
      x-api-path-slug: v1projectsprojectidundelete-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: The project ID (for example, `foo-bar-123`)
      responses:
        200:
          description: OK
      tags:
      - Project
  /v1/projects/{resource}:getIamPolicy:
    post:
      summary: Get IAM Policy
      description: |-
        Returns the IAM access control policy for the specified Project.
        Permission is denied if the policy or the resource does not exist.
      operationId: cloudresourcemanager.projects.getIamPolicy
      x-api-path-slug: v1projectsresourcegetiampolicy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy is being requested'
      responses:
        200:
          description: OK
      tags:
      - IAM
  /v1/projects/{resource}:setIamPolicy:
    post:
      summary: Set IAM Policy
      description: |-
        Sets the IAM access control policy for the specified Project. Replaces
        any existing policy.

        The following constraints apply when using `setIamPolicy()`:

        + Project does not support `allUsers` and `allAuthenticatedUsers` as
        `members` in a `Binding` of a `Policy`.

        + The owner role can be granted only to `user` and `serviceAccount`.

        + Service accounts can be made owners of a project directly
        without any restrictions. However, to be added as an owner, a user must be
        invited via Cloud Platform console and must accept the invitation.

        + A user cannot be granted the owner role using `setIamPolicy()`. The user
        must be granted the owner role using the Cloud Platform Console and must
        explicitly accept the invitation.

        + Invitations to grant the owner role cannot be sent using
        `setIamPolicy()`;
        they must be sent only using the Cloud Platform Console.

        + Membership changes that leave the project without any owners that have
        accepted the Terms of Service (ToS) will be rejected.

        + There must be at least one owner who has accepted the Terms of
        Service (ToS) agreement in the policy. Calling `setIamPolicy()` to
        to remove the last ToS-accepted owner from the policy will fail. This
        restriction also applies to legacy projects that no longer have owners
        who have accepted the ToS. Edits to IAM policies will be rejected until
        the lack of a ToS-accepting owner is rectified.

        + Calling this method requires enabling the App Engine Admin API.

        Note: Removing service accounts from policies or changing their roles
        can render services completely inoperable. It is important to understand
        how the service account is being used before removing or updating its
        roles.
      operationId: cloudresourcemanager.projects.setIamPolicy
      x-api-path-slug: v1projectsresourcesetiampolicy-post
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
  /v1/projects/{resource}:testIamPermissions:
    post:
      summary: Test IAM Policy
      description: Returns permissions that a caller has on the specified Project.
      operationId: cloudresourcemanager.projects.testIamPermissions
      x-api-path-slug: v1projectsresourcetestiampermissions-post
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
      - IAM
  /v1/{name}:
    delete:
      summary: Delete Lien
      description: |-
        Delete a Lien by `name`.

        Callers of this method will require permission on the `parent` resource.
        For example, a Lien with a `parent` of `projects/1234` requires permission
        `resourcemanager.projects.updateLiens`.
      operationId: cloudresourcemanager.liens.delete
      x-api-path-slug: v1name-delete
      parameters:
      - in: path
        name: name
        description: The name/identifier of the Lien to delete
      responses:
        200:
          description: OK
      tags:
      - Lien
    get:
      summary: Get Operation
      description: |-
        Gets the latest state of a long-running operation.  Clients can use this
        method to poll the operation result at intervals as recommended by the API
        service.
      operationId: cloudresourcemanager.operations.get
      x-api-path-slug: v1name-get
      parameters:
      - in: path
        name: name
        description: The name of the operation resource
      responses:
        200:
          description: OK
      tags:
      - Operation
  /v1/{resource}:getIamPolicy:
    post:
      summary: Get Organization IAM Policy
      description: |-
        Gets the access control policy for an Organization resource. May be empty
        if no such policy or resource exists. The `resource` field should be the
        organization's resource name, e.g. "organizations/123".
      operationId: cloudresourcemanager.organizations.getIamPolicy
      x-api-path-slug: v1resourcegetiampolicy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy is being requested'
      responses:
        200:
          description: OK
      tags:
      - Organization
  /v1/{resource}:setIamPolicy:
    post:
      summary: Set Organization IAM Policy
      description: |-
        Sets the access control policy on an Organization resource. Replaces any
        existing policy. The `resource` field should be the organization's resource
        name, e.g. "organizations/123".
      operationId: cloudresourcemanager.organizations.setIamPolicy
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
      - Organization
  /v1/{resource}:testIamPermissions:
    post:
      summary: TEst Organization IAM Permissions
      description: |-
        Returns permissions that a caller has on the specified Organization.
        The `resource` field should be the organization's resource name,
        e.g. "organizations/123".
      operationId: cloudresourcemanager.organizations.testIamPermissions
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
      - Organization