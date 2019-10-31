swagger: "2.0"
x-collection-name: Google Drive
x-complete: 1
info:
  title: Google Drive
  description: manages-files-in-drive-including-uploading-downloading-searching-detecting-changes-and-updating-sharing-permissions-
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /drive/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /about:
    get:
      summary: Get About
      description: Gets information about the user, the user's Drive, and system capabilities.
      operationId: drive.about.get
      x-api-path-slug: about-get
      responses:
        200:
          description: OK
      tags:
      - About
  /changes:
    get:
      summary: Get Changes
      description: Lists the changes for a user or Team Drive.
      operationId: drive.changes.list
      x-api-path-slug: changes-get
      parameters:
      - in: query
        name: includeCorpusRemovals
        description: Whether changes should include the file resource if the file
          is still accessible by the user at the time of the request, even when a
          file was removed from the list of changes and there will be no further change
          entries for this file
      - in: query
        name: includeRemoved
        description: Whether to include changes indicating that items have been removed
          from the list of changes, for example by deletion or loss of access
      - in: query
        name: includeTeamDriveItems
        description: Whether Team Drive files or changes should be included in results
      - in: query
        name: pageSize
        description: The maximum number of changes to return per page
      - in: query
        name: pageToken
        description: The token for continuing a previous list request on the next
          page
      - in: query
        name: restrictToMyDrive
        description: Whether to restrict the results to changes inside the My Drive
          hierarchy
      - in: query
        name: spaces
        description: A comma-separated list of spaces to query within the user corpus
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: teamDriveId
        description: The Team Drive from which changes will be returned
      responses:
        200:
          description: OK
      tags:
      - Change
  /changes/startPageToken:
    get:
      summary: Get Start Page Token Changes
      description: Gets the starting pageToken for listing future changes.
      operationId: drive.changes.getStartPageToken
      x-api-path-slug: changesstartpagetoken-get
      parameters:
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: teamDriveId
        description: The ID of the Team Drive for which the starting pageToken for
          listing future changes from that Team Drive will be returned
      responses:
        200:
          description: OK
      tags:
      - Change
  /changes/watch:
    post:
      summary: Watch Changes
      description: Subscribes to changes for a user.
      operationId: drive.changes.watch
      x-api-path-slug: changeswatch-post
      parameters:
      - in: query
        name: includeCorpusRemovals
        description: Whether changes should include the file resource if the file
          is still accessible by the user at the time of the request, even when a
          file was removed from the list of changes and there will be no further change
          entries for this file
      - in: query
        name: includeRemoved
        description: Whether to include changes indicating that items have been removed
          from the list of changes, for example by deletion or loss of access
      - in: query
        name: includeTeamDriveItems
        description: Whether Team Drive files or changes should be included in results
      - in: query
        name: pageSize
        description: The maximum number of changes to return per page
      - in: query
        name: pageToken
        description: The token for continuing a previous list request on the next
          page
      - in: body
        name: resource
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: restrictToMyDrive
        description: Whether to restrict the results to changes inside the My Drive
          hierarchy
      - in: query
        name: spaces
        description: A comma-separated list of spaces to query within the user corpus
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: teamDriveId
        description: The Team Drive from which changes will be returned
      responses:
        200:
          description: OK
      tags:
      - Change
  /channels/stop:
    post:
      summary: Stop Watching Changes
      description: Stop watching resources through this channel
      operationId: drive.channels.stop
      x-api-path-slug: channelsstop-post
      parameters:
      - in: body
        name: resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Change
  /files:
    get:
      summary: Get Files
      description: Lists or searches files.
      operationId: drive.files.list
      x-api-path-slug: files-get
      parameters:
      - in: query
        name: corpora
        description: Comma-separated list of bodies of items (files/documents) to
          which the query applies
      - in: query
        name: corpus
        description: The source of files to list
      - in: query
        name: includeTeamDriveItems
        description: Whether Team Drive items should be included in results
      - in: query
        name: orderBy
        description: A comma-separated list of sort keys
      - in: query
        name: pageSize
        description: The maximum number of files to return per page
      - in: query
        name: pageToken
        description: The token for continuing a previous list request on the next
          page
      - in: query
        name: q
        description: A query for filtering the file results
      - in: query
        name: spaces
        description: A comma-separated list of spaces to query within the corpus
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: teamDriveId
        description: ID of Team Drive to search
      responses:
        200:
          description: OK
      tags:
      - File
    post:
      summary: Create File
      description: Creates a new file.
      operationId: drive.files.create
      x-api-path-slug: files-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: ignoreDefaultVisibility
        description: Whether to ignore the domains default visibility settings for
          the created file
      - in: query
        name: keepRevisionForever
        description: Whether to set the keepForever field in the new head revision
      - in: query
        name: ocrLanguage
        description: A language hint for OCR processing during image import (ISO 639-1
          code)
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: useContentAsIndexableText
        description: Whether to use the uploaded content as indexable text
      responses:
        200:
          description: OK
      tags:
      - File
  /files/generateIds:
    get:
      summary: Generate File IDs
      description: Generates a set of file IDs which can be provided in create requests.
      operationId: drive.files.generateIds
      x-api-path-slug: filesgenerateids-get
      parameters:
      - in: query
        name: count
        description: The number of IDs to return
      - in: query
        name: space
        description: The space in which the IDs can be used to create new files
      responses:
        200:
          description: OK
      tags:
      - File
  /files/trash:
    delete:
      summary: Empty Trash
      description: Permanently deletes all of the user's trashed files.
      operationId: drive.files.emptyTrash
      x-api-path-slug: filestrash-delete
      responses:
        200:
          description: OK
      tags:
      - File
  /files/{fileId}:
    delete:
      summary: Delete File
      description: Permanently deletes a file owned by the user without moving it
        to the trash. If the file belongs to a Team Drive the user must be an organizer
        on the parent. If the target is a folder, all descendants owned by the user
        are also deleted.
      operationId: drive.files.delete
      x-api-path-slug: filesfileid-delete
      parameters:
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      responses:
        200:
          description: OK
      tags:
      - File
    get:
      summary: Get File
      description: Gets a file's metadata or content by ID.
      operationId: drive.files.get
      x-api-path-slug: filesfileid-get
      parameters:
      - in: query
        name: acknowledgeAbuse
        description: Whether the user is acknowledging the risk of downloading known
          malware or other abusive files
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      responses:
        200:
          description: OK
      tags:
      - File
    patch:
      summary: Update File
      description: Updates a file's metadata and/or content with patch semantics.
      operationId: drive.files.update
      x-api-path-slug: filesfileid-patch
      parameters:
      - in: query
        name: addParents
        description: A comma-separated list of parent IDs to add
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: keepRevisionForever
        description: Whether to set the keepForever field in the new head revision
      - in: query
        name: ocrLanguage
        description: A language hint for OCR processing during image import (ISO 639-1
          code)
      - in: query
        name: removeParents
        description: A comma-separated list of parent IDs to remove
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: useContentAsIndexableText
        description: Whether to use the uploaded content as indexable text
      responses:
        200:
          description: OK
      tags:
      - File
  /files/{fileId}/comments:
    get:
      summary: Get File Comments
      description: Lists a file's comments.
      operationId: drive.comments.list
      x-api-path-slug: filesfileidcomments-get
      parameters:
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: includeDeleted
        description: Whether to include deleted comments
      - in: query
        name: pageSize
        description: The maximum number of comments to return per page
      - in: query
        name: pageToken
        description: The token for continuing a previous list request on the next
          page
      - in: query
        name: startModifiedTime
        description: The minimum value of modifiedTime for the result comments (RFC
          3339 date-time)
      responses:
        200:
          description: OK
      tags:
      - Comment
    post:
      summary: Create File Comment
      description: Creates a new comment on a file.
      operationId: drive.comments.create
      x-api-path-slug: filesfileidcomments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: fileId
        description: The ID of the file
      responses:
        200:
          description: OK
      tags:
      - Comment
  /files/{fileId}/comments/{commentId}:
    delete:
      summary: Delete File Comment
      description: Deletes a comment.
      operationId: drive.comments.delete
      x-api-path-slug: filesfileidcommentscommentid-delete
      parameters:
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      responses:
        200:
          description: OK
      tags:
      - Comment
    get:
      summary: Get File Comment
      description: Gets a comment by ID.
      operationId: drive.comments.get
      x-api-path-slug: filesfileidcommentscommentid-get
      parameters:
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: includeDeleted
        description: Whether to return deleted comments
      responses:
        200:
          description: OK
      tags:
      - Comment
    patch:
      summary: Update File Comment
      description: Updates a comment with patch semantics.
      operationId: drive.comments.update
      x-api-path-slug: filesfileidcommentscommentid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      responses:
        200:
          description: OK
      tags:
      - Comment
  /files/{fileId}/comments/{commentId}/replies:
    get:
      summary: Get File Comment Replies
      description: Lists a comment's replies.
      operationId: drive.replies.list
      x-api-path-slug: filesfileidcommentscommentidreplies-get
      parameters:
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: includeDeleted
        description: Whether to include deleted replies
      - in: query
        name: pageSize
        description: The maximum number of replies to return per page
      - in: query
        name: pageToken
        description: The token for continuing a previous list request on the next
          page
      responses:
        200:
          description: OK
      tags:
      - Comment
    post:
      summary: Create File Comment Reply
      description: Creates a new reply to a comment.
      operationId: drive.replies.create
      x-api-path-slug: filesfileidcommentscommentidreplies-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      responses:
        200:
          description: OK
      tags:
      - Comment
  /files/{fileId}/comments/{commentId}/replies/{replyId}:
    delete:
      summary: Delete File Comment Reply
      description: Deletes a reply.
      operationId: drive.replies.delete
      x-api-path-slug: filesfileidcommentscommentidrepliesreplyid-delete
      parameters:
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      - in: path
        name: replyId
        description: The ID of the reply
      responses:
        200:
          description: OK
      tags:
      - Comment
    get:
      summary: Get File Comment Reply
      description: Gets a reply by ID.
      operationId: drive.replies.get
      x-api-path-slug: filesfileidcommentscommentidrepliesreplyid-get
      parameters:
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: includeDeleted
        description: Whether to return deleted replies
      - in: path
        name: replyId
        description: The ID of the reply
      responses:
        200:
          description: OK
      tags:
      - Comment
    patch:
      summary: Update File Comment Reply
      description: Updates a reply with patch semantics.
      operationId: drive.replies.update
      x-api-path-slug: filesfileidcommentscommentidrepliesreplyid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      - in: path
        name: replyId
        description: The ID of the reply
      responses:
        200:
          description: OK
      tags:
      - Comment
  /files/{fileId}/copy:
    post:
      summary: Copy File
      description: Creates a copy of a file and applies any requested updates with
        patch semantics.
      operationId: drive.files.copy
      x-api-path-slug: filesfileidcopy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: ignoreDefaultVisibility
        description: Whether to ignore the domains default visibility settings for
          the created file
      - in: query
        name: keepRevisionForever
        description: Whether to set the keepForever field in the new head revision
      - in: query
        name: ocrLanguage
        description: A language hint for OCR processing during image import (ISO 639-1
          code)
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      responses:
        200:
          description: OK
      tags:
      - File
  /files/{fileId}/export:
    get:
      summary: Export File
      description: Exports a Google Doc to the requested MIME type and returns the
        exported content.
      operationId: drive.files.export
      x-api-path-slug: filesfileidexport-get
      parameters:
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: mimeType
        description: The MIME type of the format requested for this export
      responses:
        200:
          description: OK
      tags:
      - File
  /files/{fileId}/permissions:
    get:
      summary: Get File Permissions
      description: Lists a file's or Team Drive's permissions.
      operationId: drive.permissions.list
      x-api-path-slug: filesfileidpermissions-get
      parameters:
      - in: path
        name: fileId
        description: The ID of the file or Team Drive
      - in: query
        name: pageSize
        description: The maximum number of permissions to return per page
      - in: query
        name: pageToken
        description: The token for continuing a previous list request on the next
          page
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: useDomainAdminAccess
        description: Whether the request should be treated as if it was issued by
          a domain administrator; if set to true, then the requester will be granted
          access if they are an administrator of the domain to which the item belongs
      responses:
        200:
          description: OK
      tags:
      - Permission
    post:
      summary: Create File Permission
      description: Creates a permission for a file or Team Drive.
      operationId: drive.permissions.create
      x-api-path-slug: filesfileidpermissions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: emailMessage
        description: A custom message to include in the notification email
      - in: path
        name: fileId
        description: The ID of the file or Team Drive
      - in: query
        name: sendNotificationEmail
        description: Whether to send a notification email when sharing to users or
          groups
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: transferOwnership
        description: Whether to transfer ownership to the specified user and downgrade
          the current owner to a writer
      - in: query
        name: useDomainAdminAccess
        description: Whether the request should be treated as if it was issued by
          a domain administrator; if set to true, then the requester will be granted
          access if they are an administrator of the domain to which the item belongs
      responses:
        200:
          description: OK
      tags:
      - Permission
  /files/{fileId}/permissions/{permissionId}:
    delete:
      summary: Delete File Permission
      description: Deletes a permission.
      operationId: drive.permissions.delete
      x-api-path-slug: filesfileidpermissionspermissionid-delete
      parameters:
      - in: path
        name: fileId
        description: The ID of the file or Team Drive
      - in: path
        name: permissionId
        description: The ID of the permission
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: useDomainAdminAccess
        description: Whether the request should be treated as if it was issued by
          a domain administrator; if set to true, then the requester will be granted
          access if they are an administrator of the domain to which the item belongs
      responses:
        200:
          description: OK
      tags:
      - Permission
    get:
      summary: Get File Permission
      description: Gets a permission by ID.
      operationId: drive.permissions.get
      x-api-path-slug: filesfileidpermissionspermissionid-get
      parameters:
      - in: path
        name: fileId
        description: The ID of the file
      - in: path
        name: permissionId
        description: The ID of the permission
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: useDomainAdminAccess
        description: Whether the request should be treated as if it was issued by
          a domain administrator; if set to true, then the requester will be granted
          access if they are an administrator of the domain to which the item belongs
      responses:
        200:
          description: OK
      tags:
      - Permission
    patch:
      summary: Update File Permission
      description: Updates a permission with patch semantics.
      operationId: drive.permissions.update
      x-api-path-slug: filesfileidpermissionspermissionid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: fileId
        description: The ID of the file or Team Drive
      - in: path
        name: permissionId
        description: The ID of the permission
      - in: query
        name: removeExpiration
        description: Whether to remove the expiration date
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: transferOwnership
        description: Whether to transfer ownership to the specified user and downgrade
          the current owner to a writer
      - in: query
        name: useDomainAdminAccess
        description: Whether the request should be treated as if it was issued by
          a domain administrator; if set to true, then the requester will be granted
          access if they are an administrator of the domain to which the item belongs
      responses:
        200:
          description: OK
      tags:
      - Permission
  /files/{fileId}/revisions:
    get:
      summary: Get File Revisions
      description: Lists a file's revisions.
      operationId: drive.revisions.list
      x-api-path-slug: filesfileidrevisions-get
      parameters:
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: pageSize
        description: The maximum number of revisions to return per page
      - in: query
        name: pageToken
        description: The token for continuing a previous list request on the next
          page
      responses:
        200:
          description: OK
      tags:
      - Revision
  /files/{fileId}/revisions/{revisionId}:
    delete:
      summary: Delete File Revision
      description: Permanently deletes a revision. This method is only applicable
        to files with binary content in Drive.
      operationId: drive.revisions.delete
      x-api-path-slug: filesfileidrevisionsrevisionid-delete
      parameters:
      - in: path
        name: fileId
        description: The ID of the file
      - in: path
        name: revisionId
        description: The ID of the revision
      responses:
        200:
          description: OK
      tags:
      - Revision
    get:
      summary: Get File Revision
      description: Gets a revision's metadata or content by ID.
      operationId: drive.revisions.get
      x-api-path-slug: filesfileidrevisionsrevisionid-get
      parameters:
      - in: query
        name: acknowledgeAbuse
        description: Whether the user is acknowledging the risk of downloading known
          malware or other abusive files
      - in: path
        name: fileId
        description: The ID of the file
      - in: path
        name: revisionId
        description: The ID of the revision
      responses:
        200:
          description: OK
      tags:
      - Revision
    patch:
      summary: Update File Revision
      description: Updates a revision with patch semantics.
      operationId: drive.revisions.update
      x-api-path-slug: filesfileidrevisionsrevisionid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: fileId
        description: The ID of the file
      - in: path
        name: revisionId
        description: The ID of the revision
      responses:
        200:
          description: OK
      tags:
      - Revision
  /files/{fileId}/watch:
    post:
      summary: Watch File
      description: Subscribes to changes to a file
      operationId: drive.files.watch
      x-api-path-slug: filesfileidwatch-post
      parameters:
      - in: query
        name: acknowledgeAbuse
        description: Whether the user is acknowledging the risk of downloading known
          malware or other abusive files
      - in: path
        name: fileId
        description: The ID of the file
      - in: body
        name: resource
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      responses:
        200:
          description: OK
      tags:
      - File
  /teamdrives:
    get:
      summary: Get Team Drives
      description: Lists the user's Team Drives.
      operationId: drive.teamdrives.list
      x-api-path-slug: teamdrives-get
      parameters:
      - in: query
        name: pageSize
        description: Maximum number of Team Drives to return
      - in: query
        name: pageToken
        description: Page token for Team Drives
      - in: query
        name: q
        description: Query string for searching Team Drives
      - in: query
        name: useDomainAdminAccess
        description: Whether the request should be treated as if it was issued by
          a domain administrator; if set to true, then all Team Drives of the domain
          in which the requester is an administrator are returned
      responses:
        200:
          description: OK
      tags:
      - Team Drive
    post:
      summary: Create Team Drive
      description: Creates a new Team Drive.
      operationId: drive.teamdrives.create
      x-api-path-slug: teamdrives-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: requestId
        description: An ID, such as a random UUID, which uniquely identifies this
          users request for idempotent creation of a Team Drive
      responses:
        200:
          description: OK
      tags:
      - Team Drive
  /teamdrives/{teamDriveId}:
    delete:
      summary: Delete Team Drive
      description: Permanently deletes a Team Drive for which the user is an organizer.
        The Team Drive cannot contain any untrashed items.
      operationId: drive.teamdrives.delete
      x-api-path-slug: teamdrivesteamdriveid-delete
      parameters:
      - in: path
        name: teamDriveId
        description: The ID of the Team Drive
      responses:
        200:
          description: OK
      tags:
      - Team Drive
    get:
      summary: CrGeteate Team Drive
      description: Gets a Team Drive's metadata by ID.
      operationId: drive.teamdrives.get
      x-api-path-slug: teamdrivesteamdriveid-get
      parameters:
      - in: path
        name: teamDriveId
        description: The ID of the Team Drive
      - in: query
        name: useDomainAdminAccess
        description: Whether the request should be treated as if it was issued by
          a domain administrator; if set to true, then the requester will be granted
          access if they are an administrator of the domain to which the Team Drive
          belongs
      responses:
        200:
          description: OK
      tags:
      - Team Drive
    patch:
      summary: Update Team Drive
      description: Updates a Team Drive's metadata
      operationId: drive.teamdrives.update
      x-api-path-slug: teamdrivesteamdriveid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: teamDriveId
        description: The ID of the Team Drive
      responses:
        200:
          description: OK
      tags:
      - Team Drive