swagger: "2.0"
x-collection-name: AWS WorkDocs
x-complete: 1
info:
  title: AWS WorkDocs API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AbortDocumentVersionUpload:
    get:
      summary: Abort Document Version Upload
      description: Aborts the upload of the specified document version that was previously
        initiated by.
      operationId: abortDocumentVersionUpload
      x-api-path-slug: actionabortdocumentversionupload-get
      parameters:
      - in: query
        name: DocumentId
        description: The ID of the document
        type: string
      - in: query
        name: VersionId
        description: The ID of the version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Documents
  /?Action=ActivateUser:
    get:
      summary: Activate User
      description: Activates the specified user.
      operationId: activateUser
      x-api-path-slug: actionactivateuser-get
      parameters:
      - in: query
        name: UserId
        description: The ID of the user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AddResourcePermissions:
    get:
      summary: Add Resource Permissions
      description: Creates a set of permissions for the specified folder or document.
      operationId: addResourcePermissions
      x-api-path-slug: actionaddresourcepermissions-get
      parameters:
      - in: query
        name: ResourceId
        description: The ID of the resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Permissions
  /?Action=CreateFolder:
    get:
      summary: Create Folder
      description: Creates a folder with the specified name and parent folder.
      operationId: createFolder
      x-api-path-slug: actioncreatefolder-get
      parameters:
      - in: query
        name: Name
        description: The name of the new folder
        type: string
      - in: query
        name: ParentFolderId
        description: The ID of the parent folder
        type: string
      responses:
        200:
          description: OK
      tags:
      - Folders
  /?Action=CreateNotificationSubscription:
    get:
      summary: Create Notification Subscription
      description: Configure WorkDocs to use Amazon SNS notifications.
      operationId: createNotificationSubscription
      x-api-path-slug: actioncreatenotificationsubscription-get
      parameters:
      - in: query
        name: OrganizationId
        description: The ID of the organization
        type: string
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /?Action=CreateUser:
    get:
      summary: Create User
      description: Creates a user in a Simple AD or Microsoft AD directory.
      operationId: createUser
      x-api-path-slug: actioncreateuser-get
      parameters:
      - in: query
        name: GivenName
        description: The given name of the user
        type: string
      - in: query
        name: OrganizationId
        description: The ID of the organization
        type: string
      - in: query
        name: Password
        description: The password of the user
        type: string
      - in: query
        name: StorageRule
        description: The amount of storage for the user
        type: string
      - in: query
        name: Surname
        description: The surname of the user
        type: string
      - in: query
        name: TimeZoneId
        description: The time zone ID of the user
        type: string
      - in: query
        name: Username
        description: The login name of the user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=DeactivateUser:
    get:
      summary: Deactivate User
      description: Deactivates the specified user, which revokes the user's access
        to Amazon WorkDocs.
      operationId: deactivateUser
      x-api-path-slug: actiondeactivateuser-get
      parameters:
      - in: query
        name: UserId
        description: The ID of the user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=DeleteDocument:
    get:
      summary: Delete Document
      description: Permanently deletes the specified document and its associated metadata.
      operationId: deleteDocument
      x-api-path-slug: actiondeletedocument-get
      parameters:
      - in: query
        name: DocumentId
        description: The ID of the document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Documents
  /?Action=DeleteFolder:
    get:
      summary: Delete Folder
      description: Permanently deletes the specified folder and its contents.
      operationId: deleteFolder
      x-api-path-slug: actiondeletefolder-get
      parameters:
      - in: query
        name: FolderId
        description: The ID of the folder
        type: string
      responses:
        200:
          description: OK
      tags:
      - Folders
  /?Action=DeleteFolderContents:
    get:
      summary: Delete Folder Contents
      description: Deletes the contents of the specified folder.
      operationId: deleteFolderContents
      x-api-path-slug: actiondeletefoldercontents-get
      parameters:
      - in: query
        name: FolderId
        description: The ID of the folder
        type: string
      responses:
        200:
          description: OK
      tags:
      - Folders
  /?Action=DeleteNotificationSubscription:
    get:
      summary: Delete Notification Subscription
      description: Deletes the specified subscription from the specified organization.
      operationId: deleteNotificationSubscription
      x-api-path-slug: actiondeletenotificationsubscription-get
      parameters:
      - in: query
        name: OrganizationId
        description: The ID of the organization
        type: string
      - in: query
        name: SubscriptionId
        description: The ID of the subscription
        type: string
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /?Action=DeleteUser:
    get:
      summary: Delete User
      description: Deletes the specified user from a Simple AD or Microsoft AD directory.
      operationId: deleteUser
      x-api-path-slug: actiondeleteuser-get
      parameters:
      - in: query
        name: UserId
        description: The ID of the user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=DescribeDocumentVersions:
    get:
      summary: Describe Document Versions
      description: Retrieves the document versions for the specified document.
      operationId: describeDocumentVersions
      x-api-path-slug: actiondescribedocumentversions-get
      parameters:
      - in: query
        name: DocumentId
        description: The ID of the document
        type: string
      - in: query
        name: Fields
        description: Specify SOURCE to include initialized versions and a URL for
          the source document
        type: string
      - in: query
        name: Include
        description: A comma-separated list of values
        type: string
      - in: query
        name: Limit
        description: The maximum number of versions to return with this call
        type: string
      - in: query
        name: Marker
        description: The marker for the next set of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Documents
  /?Action=DescribeFolderContents:
    get:
      summary: Describe Folder Contents
      description: Describes the contents of the specified folder, including its documents
        and sub-folders.
      operationId: describeFolderContents
      x-api-path-slug: actiondescribefoldercontents-get
      parameters:
      - in: query
        name: FolderId
        description: The ID of the folder
        type: string
      - in: query
        name: Include
        description: The contents to include
        type: string
      - in: query
        name: Limit
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: Marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: Order
        description: The order for the contents of the folder
        type: string
      - in: query
        name: Sort
        description: The sorting criteria
        type: string
      - in: query
        name: Type
        description: The type of items
        type: string
      responses:
        200:
          description: OK
      tags:
      - Folders
  /?Action=DescribeNotificationSubscriptions:
    get:
      summary: Describe Notification Subscriptions
      description: Lists the specified notification subscriptions.
      operationId: describeNotificationSubscriptions
      x-api-path-slug: actiondescribenotificationsubscriptions-get
      parameters:
      - in: query
        name: Limit
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: Marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: OrganizationId
        description: The ID of the organization
        type: string
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /?Action=DescribeResourcePermissions:
    get:
      summary: Describe Resource Permissions
      description: Describes the permissions of a specified resource.
      operationId: describeResourcePermissions
      x-api-path-slug: actiondescriberesourcepermissions-get
      parameters:
      - in: query
        name: ResourceId
        description: The ID of the resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Permissions
  /?Action=DescribeUsers:
    get:
      summary: Describe Users
      description: Describes the specified users.
      operationId: describeUsers
      x-api-path-slug: actiondescribeusers-get
      parameters:
      - in: query
        name: Fields
        description: A comma-separated list of values
        type: string
      - in: query
        name: Include
        description: The state of the users
        type: string
      - in: query
        name: Limit
        description: The maximum number of items to return
        type: string
      - in: query
        name: Marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: Order
        description: The order for the results
        type: string
      - in: query
        name: OrganizationId
        description: The ID of the organization
        type: string
      - in: query
        name: Query
        description: A query to filter users by user name
        type: string
      - in: query
        name: Sort
        description: The sorting criteria
        type: string
      - in: query
        name: UserIds
        description: The IDs of the users
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=GetDocument:
    get:
      summary: Get Document
      description: Retrieves the specified document object.
      operationId: getDocument
      x-api-path-slug: actiongetdocument-get
      parameters:
      - in: query
        name: DocumentId
        description: The ID of the document object
        type: string
      responses:
        200:
          description: OK
      tags:
      - Documents
  /?Action=GetDocumentPath:
    get:
      summary: Get Document Path
      description: Retrieves the path information (the hierarchy from the root folder)
        for the requested document.
      operationId: getDocumentPath
      x-api-path-slug: actiongetdocumentpath-get
      parameters:
      - in: query
        name: DocumentId
        description: The ID of the document
        type: string
      - in: query
        name: Fields
        description: A comma-separated list of values
        type: string
      - in: query
        name: Limit
        description: The maximum number of levels in the hierarchy to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Documents
  /?Action=GetDocumentVersion:
    get:
      summary: Get Document Version
      description: Retrieves version metadata for the specified document.
      operationId: getDocumentVersion
      x-api-path-slug: actiongetdocumentversion-get
      parameters:
      - in: query
        name: DocumentId
        description: The ID of the document
        type: string
      - in: query
        name: Fields
        description: A comma-separated list of values
        type: string
      - in: query
        name: VersionId
        description: The version ID of the document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Documents
  /?Action=GetFolder:
    get:
      summary: Get Folder
      description: Retrieves the metadata of the specified folder.
      operationId: getFolder
      x-api-path-slug: actiongetfolder-get
      parameters:
      - in: query
        name: FolderId
        description: The ID of the folder
        type: string
      responses:
        200:
          description: OK
      tags:
      - Folders
  /?Action=GetFolderPath:
    get:
      summary: Get Folder Path
      description: Retrieves the path information (the hierarchy from the root folder)
        for the specified folder.
      operationId: getFolderPath
      x-api-path-slug: actiongetfolderpath-get
      parameters:
      - in: query
        name: Fields
        description: A comma-separated list of values
        type: string
      - in: query
        name: FolderId
        description: The ID of the folder
        type: string
      - in: query
        name: Limit
        description: The maximum number of levels in the hierarchy to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Folders
  /?Action=InitiateDocumentVersionUpload:
    get:
      summary: Initiate Document Version Upload
      description: Creates a new document object and version object.
      operationId: initiateDocumentVersionUpload
      x-api-path-slug: actioninitiatedocumentversionupload-get
      parameters:
      - in: query
        name: ContentType
        description: The content type of the document
        type: string
      - in: query
        name: DocumentSizeInBytes
        description: The size of the document, in bytes
        type: string
      - in: query
        name: Id
        description: The ID of the document
        type: string
      - in: query
        name: Name
        description: The name of the document
        type: string
      - in: query
        name: ParentFolderId
        description: The ID of the parent folder
        type: string
      responses:
        200:
          description: OK
      tags:
      - Documents
  /?Action=RemoveAllResourcePermissions:
    get:
      summary: Remove All Resource Permissions
      description: Removes all the permissions from the specified resource.
      operationId: removeAllResourcePermissions
      x-api-path-slug: actionremoveallresourcepermissions-get
      parameters:
      - in: query
        name: ResourceId
        description: The ID of the resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Permissions
  /?Action=RemoveResourcePermission:
    get:
      summary: Remove Resource Permission
      description: Removes the permission for the specified principal from the specified
        resource.
      operationId: removeResourcePermission
      x-api-path-slug: actionremoveresourcepermission-get
      parameters:
      - in: query
        name: PrincipalId
        description: The principal ID of the resource
        type: string
      - in: query
        name: PrincipalType
        description: The principal type of the resource
        type: string
      - in: query
        name: ResourceId
        description: The ID of the resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Permissions
  /?Action=UpdateDocument:
    get:
      summary: Update Document
      description: Updates the specified attributes of the specified document.
      operationId: updateDocument
      x-api-path-slug: actionupdatedocument-get
      parameters:
      - in: query
        name: DocumentId
        description: The ID of the document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Documents
  /?Action=UpdateDocumentVersion:
    get:
      summary: Update Document Version
      description: Changes the status of the document version to ACTIVE.
      operationId: updateDocumentVersion
      x-api-path-slug: actionupdatedocumentversion-get
      parameters:
      - in: query
        name: DocumentId
        description: The ID of the document
        type: string
      - in: query
        name: VersionId
        description: The version ID of the document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Documents
  /?Action=UpdateFolder:
    get:
      summary: Update Folder
      description: Updates the specified attributes of the specified folder.
      operationId: updateFolder
      x-api-path-slug: actionupdatefolder-get
      parameters:
      - in: query
        name: FolderId
        description: The ID of the folder
        type: string
      responses:
        200:
          description: OK
      tags:
      - Folders
  /?Action=UpdateUser:
    get:
      summary: Update User
      description: "Updates the specified attributes of the specified user, and grants
        or revokes \n      administrative privileges to the Amazon WorkDocs site."
      operationId: updateUser
      x-api-path-slug: actionupdateuser-get
      parameters:
      - in: query
        name: UserId
        description: The ID of the user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users