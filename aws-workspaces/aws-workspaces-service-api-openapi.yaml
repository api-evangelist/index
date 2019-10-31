swagger: "2.0"
x-collection-name: AWS WorkSpaces
x-complete: 1
info:
  title: AWS WorkSpaces Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateTags:
    get:
      summary: Create Tags
      description: Creates tags for a WorkSpace.
      operationId: createTags
      x-api-path-slug: actioncreatetags-get
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID of the request
        type: string
      - in: query
        name: Tags
        description: The tags of the request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=CreateWorkspaces:
    get:
      summary: Create Workspaces
      description: Creates one or more WorkSpaces.
      operationId: createWorkspaces
      x-api-path-slug: actioncreateworkspaces-get
      parameters:
      - in: query
        name: Workspaces
        description: An array of structures that specify the WorkSpaces to create
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""
  /?Action=DeleteTags:
    get:
      summary: Delete Tags
      description: Deletes tags from a WorkSpace.
      operationId: deleteTags
      x-api-path-slug: actiondeletetags-get
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID of the request
        type: string
      - in: query
        name: TagKeys
        description: The tag keys of the request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=DescribeTags:
    get:
      summary: Describe Tags
      description: Describes tags for a WorkSpace.
      operationId: describeTags
      x-api-path-slug: actiondescribetags-get
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID of the request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=DescribeWorkspaceBundles:
    get:
      summary: Describe Workspace Bundles
      description: Obtains information about the WorkSpace bundles that are available
        to your account in the specified region.
      operationId: describeWorkspaceBundles
      x-api-path-slug: actiondescribeworkspacebundles-get
      parameters:
      - in: query
        name: BundleIds
        description: An array of strings that contains the identifiers of the bundles
          to retrieve
        type: string
      - in: query
        name: NextToken
        description: The NextToken value from a previous call to this operation
        type: string
      - in: query
        name: Owner
        description: The owner of the bundles to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspace Bundles
  /?Action=DescribeWorkspaceDirectories:
    get:
      summary: Describe Workspace Directories
      description: Retrieves information about the AWS Directory Service directories
        in the region that are registered with Amazon WorkSpaces and are available
        to your account.
      operationId: describeWorkspaceDirectories
      x-api-path-slug: actiondescribeworkspacedirectories-get
      parameters:
      - in: query
        name: DirectoryIds
        description: An array of strings that contains the directory identifiers to
          retrieve information for
        type: string
      - in: query
        name: NextToken
        description: The NextToken value from a previous call to this operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspace Directories
  /?Action=DescribeWorkspaces:
    get:
      summary: Describe Workspaces
      description: Obtains information about the specified WorkSpaces.
      operationId: describeWorkspaces
      x-api-path-slug: actiondescribeworkspaces-get
      parameters:
      - in: query
        name: BundleId
        description: The identifier of a bundle to obtain the WorkSpaces for
        type: string
      - in: query
        name: DirectoryId
        description: Specifies the directory identifier to which to limit the WorkSpaces
        type: string
      - in: query
        name: Limit
        description: The maximum number of items to return
        type: string
      - in: query
        name: NextToken
        description: The NextToken value from a previous call to this operation
        type: string
      - in: query
        name: UserName
        description: Used with the DirectoryId parameter to specify the directory
          user for whom to         obtain the WorkSpace
        type: string
      - in: query
        name: WorkspaceIds
        description: An array of strings that contain the identifiers of the WorkSpaces
          for which to retrieve information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspaces
  /?Action=DescribeWorkspacesConnectionStatus:
    get:
      summary: Describe Workspaces Connection Status
      description: Describes the connection status of a specified WorkSpace.
      operationId: describeWorkspacesConnectionStatus
      x-api-path-slug: actiondescribeworkspacesconnectionstatus-get
      parameters:
      - in: query
        name: NextToken
        description: The next token of the request
        type: string
      - in: query
        name: WorkspaceIds
        description: An array of strings that contain the identifiers of the WorkSpaces
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspaces
  /?Action=ModifyWorkspaceProperties:
    get:
      summary: Modify Workspace Properties
      description: Modifies the WorkSpace properties, including the running mode and
        AutoStop time.
      operationId: modifyWorkspaceProperties
      x-api-path-slug: actionmodifyworkspaceproperties-get
      parameters:
      - in: query
        name: WorkspaceId
        description: The ID of the WorkSpace
        type: string
      - in: query
        name: WorkspaceProperties
        description: The WorkSpace properties of the request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspaces
  /?Action=RebootWorkspaces:
    get:
      summary: Reboot Workspaces
      description: Reboots the specified WorkSpaces.
      operationId: rebootWorkspaces
      x-api-path-slug: actionrebootworkspaces-get
      parameters:
      - in: query
        name: RebootWorkspaceRequests
        description: An array of structures that specify the WorkSpaces to reboot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspaces
  /?Action=RebuildWorkspaces:
    get:
      summary: Rebuild Workspaces
      description: Rebuilds the specified WorkSpaces.
      operationId: rebuildWorkspaces
      x-api-path-slug: actionrebuildworkspaces-get
      parameters:
      - in: query
        name: RebuildWorkspaceRequests
        description: An array of structures that specify the WorkSpaces to rebuild
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspaces
  /?Action=StartWorkspaces:
    get:
      summary: Start Workspaces
      description: Starts the specified WorkSpaces.
      operationId: startWorkspaces
      x-api-path-slug: actionstartworkspaces-get
      parameters:
      - in: query
        name: StartWorkspaceRequests
        description: The requests
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspaces
  /?Action=StopWorkspaces:
    get:
      summary: Stop Workspaces
      description: Stops the specified WorkSpaces.
      operationId: stopWorkspaces
      x-api-path-slug: actionstopworkspaces-get
      parameters:
      - in: query
        name: StopWorkspaceRequests
        description: The requests
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspaces
  /?Action=TerminateWorkspaces:
    get:
      summary: Terminate Workspaces
      description: Terminates the specified WorkSpaces.
      operationId: terminateWorkspaces
      x-api-path-slug: actionterminateworkspaces-get
      parameters:
      - in: query
        name: TerminateWorkspaceRequests
        description: An array of structures that specify the WorkSpaces to terminate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Workspaces