swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/groups/{id}/access_requests:
    get:
      summary: Get Groups Access Requests
      description: This feature was introduced in GitLab 8.11.
      operationId: getV3GroupsIdAccessRequests
      x-api-path-slug: v3groupsidaccess-requests-get
      parameters:
      - in: path
        name: id
        description: The group ID
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Access
      - Requests
    post:
      summary: Post Groups Access Requests
      description: This feature was introduced in GitLab 8.11.
      operationId: postV3GroupsIdAccessRequests
      x-api-path-slug: v3groupsidaccess-requests-post
      parameters:
      - in: path
        name: id
        description: The group ID
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Access
      - Requests
  /v3/groups/{id}/access_requests/{user_id}/approve:
    put:
      summary: Put Groups Access Requests User Approve
      description: This feature was introduced in GitLab 8.11.
      operationId: putV3GroupsIdAccessRequestsUserIdApprove
      x-api-path-slug: v3groupsidaccess-requestsuser-idapprove-put
      parameters:
      - in: formData
        name: access_level
        description: 'A valid access level (defaults: `30`, developer access level)'
      - in: path
        name: id
        description: The group ID
      - in: path
        name: user_id
        description: The user ID of the access requester
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Access
      - Requests
      - User
      - Approve
  /v3/groups/{id}/access_requests/{user_id}:
    delete:
      summary: Delete Groups Access Requests User
      description: This feature was introduced in GitLab 8.11.
      operationId: deleteV3GroupsIdAccessRequestsUserId
      x-api-path-slug: v3groupsidaccess-requestsuser-id-delete
      parameters:
      - in: path
        name: id
        description: The group ID
      - in: path
        name: user_id
        description: The user ID of the access requester
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Access
      - Requests
      - User
  /v3/groups:
    get:
      summary: Get Groups
      description: Get a groups list
      operationId: getV3Groups
      x-api-path-slug: v3groups-get
      parameters:
      - in: query
        name: all_available
        description: Show all group that you have access to
      - in: query
        name: order_by
        description: Order by name or path
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: search
        description: Search for a specific group
      - in: formData
        name: skip_groups
        description: Array of group ids to exclude from list
      - in: query
        name: sort
        description: Sort by asc (ascending) or desc (descending)
      - in: query
        name: statistics
        description: Include project statistics
      responses:
        200:
          description: OK
      tags:
      - Groups
    post:
      summary: Post Groups
      description: Create a group. Available only for users who can create groups.
      operationId: postV3Groups
      x-api-path-slug: v3groups-post
      parameters:
      - in: formData
        name: description
        description: The description of the group
      - in: formData
        name: lfs_enabled
        description: Enable/disable LFS for the projects in this group
      - in: formData
        name: name
        description: The name of the group
      - in: formData
        name: path
        description: The path of the group
      - in: formData
        name: request_access_enabled
        description: Allow users to request member access
      - in: formData
        name: visibility_level
        description: The visibility level of the group
      responses:
        200:
          description: OK
      tags:
      - Groups
  /v3/groups/owned:
    get:
      summary: Get Groups Owned
      description: Get list of owned groups for authenticated user
      operationId: getV3GroupsOwned
      x-api-path-slug: v3groupsowned-get
      parameters:
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: statistics
        description: Include project statistics
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Owned
  /v3/groups/{id}:
    put:
      summary: Put Groups
      description: Update a group. Available only for users who can administrate groups.
      operationId: putV3GroupsId
      x-api-path-slug: v3groupsid-put
      parameters:
      - in: formData
        name: description
        description: The description of the group
      - in: path
        name: id
        description: The ID of a group
      - in: formData
        name: lfs_enabled
        description: Enable/disable LFS for the projects in this group
      - in: formData
        name: name
        description: The name of the group
      - in: formData
        name: path
        description: The path of the group
      - in: formData
        name: request_access_enabled
        description: Allow users to request member access
      - in: formData
        name: visibility_level
        description: The visibility level of the group
      responses:
        200:
          description: OK
      tags:
      - Groups
    get:
      summary: Get Groups
      description: Get a single group, with containing projects.
      operationId: getV3GroupsId
      x-api-path-slug: v3groupsid-get
      parameters:
      - in: path
        name: id
        description: The ID of a group
      responses:
        200:
          description: OK
      tags:
      - Groups
    delete:
      summary: Delete Groups
      description: Remove a group.
      operationId: deleteV3GroupsId
      x-api-path-slug: v3groupsid-delete
      parameters:
      - in: path
        name: id
        description: The ID of a group
      responses:
        200:
          description: OK
      tags:
      - Groups
  /v3/groups/{id}/projects:
    get:
      summary: Get Groups Projects
      description: Get a list of projects in this group.
      operationId: getV3GroupsIdProjects
      x-api-path-slug: v3groupsidprojects-get
      parameters:
      - in: query
        name: archived
        description: Limit by archived status
      - in: path
        name: id
        description: The ID of a group
      - in: query
        name: order_by
        description: Return projects ordered by field
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: search
        description: Return list of authorized projects matching the search criteria
      - in: query
        name: simple
        description: Return only the ID, URL, name, and path of each project
      - in: query
        name: sort
        description: Return projects sorted in ascending and descending order
      - in: query
        name: visibility
        description: Limit by visibility
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Projects
  /v3/groups/{id}/projects/{project_id}:
    post:
      summary: Post Groups Projects Project
      description: Transfer a project to the group namespace. Available only for admin.
      operationId: postV3GroupsIdProjectsProjectId
      x-api-path-slug: v3groupsidprojectsproject-id-post
      parameters:
      - in: path
        name: id
        description: The ID of a group
      - in: path
        name: project_id
        description: The ID or path of the project
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Projects
      - Project
  /v3/groups/{id}/issues:
    get:
      summary: Get Groups Issues
      description: Get a list of group issues
      operationId: getV3GroupsIdIssues
      x-api-path-slug: v3groupsidissues-get
      parameters:
      - in: path
        name: id
        description: The ID of a group
      - in: query
        name: labels
        description: Comma-separated list of label names
      - in: query
        name: milestone
        description: Return issues for a specific milestone
      - in: query
        name: order_by
        description: Return issues ordered by `created_at` or `updated_at` fields
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: sort
        description: Return issues sorted in `asc` or `desc` order
      - in: query
        name: state
        description: Return opened, closed, or all issues
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Issues
  /v3/groups/{id}/members:
    get:
      summary: Get Groups Members
      description: Gets a list of group or project members viewable by the authenticated
        user.
      operationId: getV3GroupsIdMembers
      x-api-path-slug: v3groupsidmembers-get
      parameters:
      - in: path
        name: id
        description: The group ID
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: query
        description: A query string to search for members
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Members
    post:
      summary: Post Groups Members
      description: Adds a member to a group or project.
      operationId: postV3GroupsIdMembers
      x-api-path-slug: v3groupsidmembers-post
      parameters:
      - in: formData
        name: access_level
        description: 'A valid access level (defaults: `30`, developer access level)'
      - in: formData
        name: expires_at
        description: Date string in the format YEAR-MONTH-DAY
      - in: path
        name: id
        description: The group ID
      - in: formData
        name: user_id
        description: The user ID of the new member
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Members
  /v3/groups/{id}/members/{user_id}:
    get:
      summary: Get Groups Members User
      description: Gets a member of a group or project.
      operationId: getV3GroupsIdMembersUserId
      x-api-path-slug: v3groupsidmembersuser-id-get
      parameters:
      - in: path
        name: id
        description: The group ID
      - in: path
        name: user_id
        description: The user ID of the member
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Members
      - User
    put:
      summary: Put Groups Members User
      description: Updates a member of a group or project.
      operationId: putV3GroupsIdMembersUserId
      x-api-path-slug: v3groupsidmembersuser-id-put
      parameters:
      - in: formData
        name: access_level
        description: A valid access level
      - in: formData
        name: expires_at
        description: Date string in the format YEAR-MONTH-DAY
      - in: path
        name: id
        description: The group ID
      - in: path
        name: user_id
        description: The user ID of the new member
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Members
      - User
    delete:
      summary: Delete Groups Members User
      description: Removes a user from a group or project.
      operationId: deleteV3GroupsIdMembersUserId
      x-api-path-slug: v3groupsidmembersuser-id-delete
      parameters:
      - in: path
        name: id
        description: The group ID
      - in: path
        name: user_id
        description: The user ID of the member
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Members
      - User
  /v3/groups/{id}/notification_settings:
    get:
      summary: Get Groups Notification Settings
      description: This feature was introduced in GitLab 8.12
      operationId: getV3GroupsIdNotificationSettings
      x-api-path-slug: v3groupsidnotification-settings-get
      parameters:
      - in: path
        name: id
        description: The group ID or project ID or project NAMESPACE/PROJECT_NAME
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Notification
      - Settings
    put:
      summary: Put Groups Notification Settings
      description: This feature was introduced in GitLab 8.12
      operationId: putV3GroupsIdNotificationSettings
      x-api-path-slug: v3groupsidnotification-settings-put
      parameters:
      - in: formData
        name: close_issue
        description: Enable/disable this notification
      - in: formData
        name: close_merge_request
        description: Enable/disable this notification
      - in: formData
        name: failed_pipeline
        description: Enable/disable this notification
      - in: path
        name: id
        description: The group ID or project ID or project NAMESPACE/PROJECT_NAME
      - in: formData
        name: level
        description: The group notification level
      - in: formData
        name: merge_merge_request
        description: Enable/disable this notification
      - in: formData
        name: new_issue
        description: Enable/disable this notification
      - in: formData
        name: new_merge_request
        description: Enable/disable this notification
      - in: formData
        name: new_note
        description: Enable/disable this notification
      - in: formData
        name: reassign_issue
        description: Enable/disable this notification
      - in: formData
        name: reassign_merge_request
        description: Enable/disable this notification
      - in: formData
        name: reopen_issue
        description: Enable/disable this notification
      - in: formData
        name: reopen_merge_request
        description: Enable/disable this notification
      - in: formData
        name: success_pipeline
        description: Enable/disable this notification
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Notification
      - Settings
  /v3/projects/{id}/access_requests:
    get:
      summary: Get Projects Access Requests
      description: This feature was introduced in GitLab 8.11.
      operationId: getV3ProjectsIdAccessRequests
      x-api-path-slug: v3projectsidaccess-requests-get
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Access
      - Requests
    post:
      summary: Post Projects Access Requests
      description: This feature was introduced in GitLab 8.11.
      operationId: postV3ProjectsIdAccessRequests
      x-api-path-slug: v3projectsidaccess-requests-post
      parameters:
      - in: path
        name: id
        description: The project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Access
      - Requests
  /v3/projects/{id}/access_requests/{user_id}/approve:
    put:
      summary: Put Projects Access Requests User Approve
      description: This feature was introduced in GitLab 8.11.
      operationId: putV3ProjectsIdAccessRequestsUserIdApprove
      x-api-path-slug: v3projectsidaccess-requestsuser-idapprove-put
      parameters:
      - in: formData
        name: access_level
        description: 'A valid access level (defaults: `30`, developer access level)'
      - in: path
        name: id
        description: The project ID
      - in: path
        name: user_id
        description: The user ID of the access requester
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Access
      - Requests
      - User
      - Approve
  /v3/projects/{id}/access_requests/{user_id}:
    delete:
      summary: Delete Projects Access Requests User
      description: This feature was introduced in GitLab 8.11.
      operationId: deleteV3ProjectsIdAccessRequestsUserId
      x-api-path-slug: v3projectsidaccess-requestsuser-id-delete
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: path
        name: user_id
        description: The user ID of the access requester
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Access
      - Requests
      - User
  /v3/projects/{id}/issues/{issue_id}/award_emoji:
    get:
      summary: Get Projects Issues Issue Award Emoji
      description: Get projects issues issue award emoji.
      operationId: getV3ProjectsIdIssuesIssueIdAwardEmoji
      x-api-path-slug: v3projectsidissuesissue-idaward-emoji-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: issue_id
        description: The ID of an Issue, Merge Request or Snippet
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Award
      - Emoji
    post:
      summary: Post Projects Issues Issue Award Emoji
      description: Post projects issues issue award emoji.
      operationId: postV3ProjectsIdIssuesIssueIdAwardEmoji
      x-api-path-slug: v3projectsidissuesissue-idaward-emoji-post
      parameters:
      - in: path
        name: id
      - in: path
        name: issue_id
      - in: formData
        name: name
        description: The name of a award_emoji (without colons)
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Award
      - Emoji
  /v3/projects/{id}/issues/{issue_id}/award_emoji/{award_id}:
    get:
      summary: Get Projects Issues Issue Award Emoji Award
      description: Get projects issues issue award emoji award.
      operationId: getV3ProjectsIdIssuesIssueIdAwardEmojiAwardId
      x-api-path-slug: v3projectsidissuesissue-idaward-emojiaward-id-get
      parameters:
      - in: path
        name: award_id
        description: The ID of the award
      - in: path
        name: id
      - in: path
        name: issue_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Award
      - Emoji
      - Award
    delete:
      summary: Delete Projects Issues Issue Award Emoji Award
      description: Delete projects issues issue award emoji award.
      operationId: deleteV3ProjectsIdIssuesIssueIdAwardEmojiAwardId
      x-api-path-slug: v3projectsidissuesissue-idaward-emojiaward-id-delete
      parameters:
      - in: path
        name: award_id
        description: The ID of an award emoji
      - in: path
        name: id
      - in: path
        name: issue_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Award
      - Emoji
      - Award
  /v3/projects/{id}/issues/{issue_id}/notes/{note_id}/award_emoji:
    get:
      summary: Get Projects Issues Issue Notes Note Award Emoji
      description: Get projects issues issue notes note award emoji.
      operationId: getV3ProjectsIdIssuesIssueIdNotesNoteIdAwardEmoji
      x-api-path-slug: v3projectsidissuesissue-idnotesnote-idaward-emoji-get
      parameters:
      - in: path
        name: id
      - in: path
        name: issue_id
      - in: path
        name: note_id
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Notes
      - Note
      - Award
      - Emoji
    post:
      summary: Post Projects Issues Issue Notes Note Award Emoji
      description: Post projects issues issue notes note award emoji.
      operationId: postV3ProjectsIdIssuesIssueIdNotesNoteIdAwardEmoji
      x-api-path-slug: v3projectsidissuesissue-idnotesnote-idaward-emoji-post
      parameters:
      - in: path
        name: id
      - in: path
        name: issue_id
      - in: formData
        name: name
        description: The name of a award_emoji (without colons)
      - in: path
        name: note_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Notes
      - Note
      - Award
      - Emoji
  /v3/projects/{id}/issues/{issue_id}/notes/{note_id}/award_emoji/{award_id}:
    get:
      summary: Get Projects Issues Issue Notes Note Award Emoji Award
      description: Get projects issues issue notes note award emoji award.
      operationId: getV3ProjectsIdIssuesIssueIdNotesNoteIdAwardEmojiAwardId
      x-api-path-slug: v3projectsidissuesissue-idnotesnote-idaward-emojiaward-id-get
      parameters:
      - in: path
        name: award_id
        description: The ID of the award
      - in: path
        name: id
      - in: path
        name: issue_id
      - in: path
        name: note_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Notes
      - Note
      - Award
      - Emoji
      - Award
    delete:
      summary: Delete Projects Issues Issue Notes Note Award Emoji Award
      description: Delete projects issues issue notes note award emoji award.
      operationId: deleteV3ProjectsIdIssuesIssueIdNotesNoteIdAwardEmojiAwardId
      x-api-path-slug: v3projectsidissuesissue-idnotesnote-idaward-emojiaward-id-delete
      parameters:
      - in: path
        name: award_id
        description: The ID of an award emoji
      - in: path
        name: id
      - in: path
        name: issue_id
      - in: path
        name: note_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Notes
      - Note
      - Award
      - Emoji
      - Award
  /v3/projects/{id}/merge_requests/{merge_request_id}/award_emoji:
    get:
      summary: Get Projects Merge Requests Merge Request Award Emoji
      description: Get projects merge requests merge request award emoji.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdAwardEmoji
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idaward-emoji-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of an Issue, Merge Request or Snippet
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Award
      - Emoji
    post:
      summary: Post Projects Merge Requests Merge Request Award Emoji
      description: Post projects merge requests merge request award emoji.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdAwardEmoji
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idaward-emoji-post
      parameters:
      - in: path
        name: id
      - in: path
        name: merge_request_id
      - in: formData
        name: name
        description: The name of a award_emoji (without colons)
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Award
      - Emoji
  /v3/projects/{id}/merge_requests/{merge_request_id}/award_emoji/{award_id}:
    get:
      summary: Get Projects Merge Requests Merge Request Award Emoji Award
      description: Get projects merge requests merge request award emoji award.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdAwardEmojiAwardId
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idaward-emojiaward-id-get
      parameters:
      - in: path
        name: award_id
        description: The ID of the award
      - in: path
        name: id
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Award
      - Emoji
      - Award
    delete:
      summary: Delete Projects Merge Requests Merge Request Award Emoji Award
      description: Delete projects merge requests merge request award emoji award.
      operationId: deleteV3ProjectsIdMergeRequestsMergeRequestIdAwardEmojiAwardId
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idaward-emojiaward-id-delete
      parameters:
      - in: path
        name: award_id
        description: The ID of an award emoji
      - in: path
        name: id
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Award
      - Emoji
      - Award
  /v3/projects/{id}/merge_requests/{merge_request_id}/notes/{note_id}/award_emoji:
    get:
      summary: Get Projects Merge Requests Merge Request Notes Note Award Emoji
      description: Get projects merge requests merge request notes note award emoji.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdNotesNoteIdAwardEmoji
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idnotesnote-idaward-emoji-get
      parameters:
      - in: path
        name: id
      - in: path
        name: merge_request_id
      - in: path
        name: note_id
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Notes
      - Note
      - Award
      - Emoji
    post:
      summary: Post Projects Merge Requests Merge Request Notes Note Award Emoji
      description: Post projects merge requests merge request notes note award emoji.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdNotesNoteIdAwardEmoji
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idnotesnote-idaward-emoji-post
      parameters:
      - in: path
        name: id
      - in: path
        name: merge_request_id
      - in: formData
        name: name
        description: The name of a award_emoji (without colons)
      - in: path
        name: note_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Notes
      - Note
      - Award
      - Emoji
  /v3/projects/{id}/merge_requests/{merge_request_id}/notes/{note_id}/award_emoji/{award_id}:
    get:
      summary: Get Projects Merge Requests Merge Request Notes Note Award Emoji Award
      description: Get projects merge requests merge request notes note award emoji
        award.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdNotesNoteIdAwardEmojiAwardId
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idnotesnote-idaward-emojiaward-id-get
      parameters:
      - in: path
        name: award_id
        description: The ID of the award
      - in: path
        name: id
      - in: path
        name: merge_request_id
      - in: path
        name: note_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Notes
      - Note
      - Award
      - Emoji
      - Award
    delete:
      summary: Delete Projects Merge Requests Merge Request Notes Note Award Emoji
        Award
      description: Delete projects merge requests merge request notes note award emoji
        award.
      operationId: deleteV3ProjectsIdMergeRequestsMergeRequestIdNotesNoteIdAwardEmojiAwardId
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idnotesnote-idaward-emojiaward-id-delete
      parameters:
      - in: path
        name: award_id
        description: The ID of an award emoji
      - in: path
        name: id
      - in: path
        name: merge_request_id
      - in: path
        name: note_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Notes
      - Note
      - Award
      - Emoji
      - Award
  /v3/projects/{id}/snippets/{snippet_id}/award_emoji:
    get:
      summary: Get Projects Snippets Snippet Award Emoji
      description: Get projects snippets snippet award emoji.
      operationId: getV3ProjectsIdSnippetsSnippetIdAwardEmoji
      x-api-path-slug: v3projectsidsnippetssnippet-idaward-emoji-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: path
        name: snippet_id
        description: The ID of an Issue, Merge Request or Snippet
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Snippet
      - Award
      - Emoji
    post:
      summary: Post Projects Snippets Snippet Award Emoji
      description: Post projects snippets snippet award emoji.
      operationId: postV3ProjectsIdSnippetsSnippetIdAwardEmoji
      x-api-path-slug: v3projectsidsnippetssnippet-idaward-emoji-post
      parameters:
      - in: path
        name: id
      - in: formData
        name: name
        description: The name of a award_emoji (without colons)
      - in: path
        name: snippet_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Snippet
      - Award
      - Emoji
  /v3/projects/{id}/snippets/{snippet_id}/award_emoji/{award_id}:
    get:
      summary: Get Projects Snippets Snippet Award Emoji Award
      description: Get projects snippets snippet award emoji award.
      operationId: getV3ProjectsIdSnippetsSnippetIdAwardEmojiAwardId
      x-api-path-slug: v3projectsidsnippetssnippet-idaward-emojiaward-id-get
      parameters:
      - in: path
        name: award_id
        description: The ID of the award
      - in: path
        name: id
      - in: path
        name: snippet_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Snippet
      - Award
      - Emoji
      - Award
    delete:
      summary: Delete Projects Snippets Snippet Award Emoji Award
      description: Delete projects snippets snippet award emoji award.
      operationId: deleteV3ProjectsIdSnippetsSnippetIdAwardEmojiAwardId
      x-api-path-slug: v3projectsidsnippetssnippet-idaward-emojiaward-id-delete
      parameters:
      - in: path
        name: award_id
        description: The ID of an award emoji
      - in: path
        name: id
      - in: path
        name: snippet_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Snippet
      - Award
      - Emoji
      - Award
  /v3/projects/{id}/snippets/{snippet_id}/notes/{note_id}/award_emoji:
    get:
      summary: Get Projects Snippets Snippet Notes Note Award Emoji
      description: Get projects snippets snippet notes note award emoji.
      operationId: getV3ProjectsIdSnippetsSnippetIdNotesNoteIdAwardEmoji
      x-api-path-slug: v3projectsidsnippetssnippet-idnotesnote-idaward-emoji-get
      parameters:
      - in: path
        name: id
      - in: path
        name: note_id
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: path
        name: snippet_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Snippet
      - Notes
      - Note
      - Award
      - Emoji
    post:
      summary: Post Projects Snippets Snippet Notes Note Award Emoji
      description: Post projects snippets snippet notes note award emoji.
      operationId: postV3ProjectsIdSnippetsSnippetIdNotesNoteIdAwardEmoji
      x-api-path-slug: v3projectsidsnippetssnippet-idnotesnote-idaward-emoji-post
      parameters:
      - in: path
        name: id
      - in: formData
        name: name
        description: The name of a award_emoji (without colons)
      - in: path
        name: note_id
      - in: path
        name: snippet_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Snippet
      - Notes
      - Note
      - Award
      - Emoji
  /v3/projects/{id}/snippets/{snippet_id}/notes/{note_id}/award_emoji/{award_id}:
    get:
      summary: Get Projects Snippets Snippet Notes Note Award Emoji Award
      description: Get projects snippets snippet notes note award emoji award.
      operationId: getV3ProjectsIdSnippetsSnippetIdNotesNoteIdAwardEmojiAwardId
      x-api-path-slug: v3projectsidsnippetssnippet-idnotesnote-idaward-emojiaward-id-get
      parameters:
      - in: path
        name: award_id
        description: The ID of the award
      - in: path
        name: id
      - in: path
        name: note_id
      - in: path
        name: snippet_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Snippet
      - Notes
      - Note
      - Award
      - Emoji
      - Award
    delete:
      summary: Delete Projects Snippets Snippet Notes Note Award Emoji Award
      description: Delete projects snippets snippet notes note award emoji award.
      operationId: deleteV3ProjectsIdSnippetsSnippetIdNotesNoteIdAwardEmojiAwardId
      x-api-path-slug: v3projectsidsnippetssnippet-idnotesnote-idaward-emojiaward-id-delete
      parameters:
      - in: path
        name: award_id
        description: The ID of an award emoji
      - in: path
        name: id
      - in: path
        name: note_id
      - in: path
        name: snippet_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Snippet
      - Notes
      - Note
      - Award
      - Emoji
      - Award
  /v3/projects/{id}/boards:
    get:
      summary: Get Projects Boards
      description: This feature was introduced in 8.13
      operationId: getV3ProjectsIdBoards
      x-api-path-slug: v3projectsidboards-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Boards
  /v3/projects/{id}/repository/branches:
    get:
      summary: Get Projects Repository Branches
      description: Get a project repository branches
      operationId: getV3ProjectsIdRepositoryBranches
      x-api-path-slug: v3projectsidrepositorybranches-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Branches
    post:
      summary: Post Projects Repository Branches
      description: Post projects repository branches.
      operationId: postV3ProjectsIdRepositoryBranches
      x-api-path-slug: v3projectsidrepositorybranches-post
      parameters:
      - in: formData
        name: branch_name
        description: The name of the branch
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: ref
        description: Create branch from commit sha or existing branch
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Branches
  /v3/projects/{id}/repository/branches/{branch}:
    get:
      summary: Get Projects Repository Branches Branch
      description: Get projects repository branches branch.
      operationId: getV3ProjectsIdRepositoryBranchesBranch
      x-api-path-slug: v3projectsidrepositorybranchesbranch-get
      parameters:
      - in: path
        name: branch
        description: The name of the branch
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Branches
      - Branch
    delete:
      summary: Delete Projects Repository Branches Branch
      description: Delete projects repository branches branch.
      operationId: deleteV3ProjectsIdRepositoryBranchesBranch
      x-api-path-slug: v3projectsidrepositorybranchesbranch-delete
      parameters:
      - in: path
        name: branch
        description: The name of the branch
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Branches
      - Branch
  /v3/projects/{id}/repository/branches/{branch}/protect:
    put:
      summary: Put Projects Repository Branches Branch Protect
      description: Put projects repository branches branch protect.
      operationId: putV3ProjectsIdRepositoryBranchesBranchProtect
      x-api-path-slug: v3projectsidrepositorybranchesbranchprotect-put
      parameters:
      - in: path
        name: branch
        description: The name of the branch
      - in: formData
        name: developers_can_merge
        description: Flag if developers can merge to that branch
      - in: formData
        name: developers_can_push
        description: Flag if developers can push to that branch
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Branches
      - Branch
      - Protect
  /v3/projects/{id}/repository/branches/{branch}/unprotect:
    put:
      summary: Put Projects Repository Branches Branch Unprotect
      description: Put projects repository branches branch unprotect.
      operationId: putV3ProjectsIdRepositoryBranchesBranchUnprotect
      x-api-path-slug: v3projectsidrepositorybranchesbranchunprotect-put
      parameters:
      - in: path
        name: branch
        description: The name of the branch
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Branches
      - Branch
      - Unprotect
  /v3/projects/{id}/repository/merged_branches:
    delete:
      summary: Delete Projects Repository Merged Branches
      description: Delete projects repository merged branches.
      operationId: deleteV3ProjectsIdRepositoryMergedBranches
      x-api-path-slug: v3projectsidrepositorymerged-branches-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Merged
      - Branches
  /v3/projects/{id}/builds:
    get:
      summary: Get Projects Builds
      description: Get a project builds
      operationId: getV3ProjectsIdBuilds
      x-api-path-slug: v3projectsidbuilds-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: scope
        description: The scope of builds to show
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Builds
  /v3/projects/{id}/repository/commits/{sha}/builds:
    get:
      summary: Get Projects Repository Commits Sha Builds
      description: Get builds for a specific commit of a project
      operationId: getV3ProjectsIdRepositoryCommitsShaBuilds
      x-api-path-slug: v3projectsidrepositorycommitsshabuilds-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: scope
        description: The scope of builds to show
      - in: path
        name: sha
        description: The SHA id of a commit
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Commits
      - Sha
      - Builds
  /v3/projects/{id}/builds/{build_id}:
    get:
      summary: Get Projects Builds Build
      description: Get a specific build of a project
      operationId: getV3ProjectsIdBuildsBuildId
      x-api-path-slug: v3projectsidbuildsbuild-id-get
      parameters:
      - in: path
        name: build_id
        description: The ID of a build
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Builds
      - Build
  /v3/projects/{id}/builds/{build_id}/artifacts:
    get:
      summary: Get Projects Builds Build Artifacts
      description: This feature was introduced in GitLab 8.5
      operationId: getV3ProjectsIdBuildsBuildIdArtifacts
      x-api-path-slug: v3projectsidbuildsbuild-idartifacts-get
      parameters:
      - in: path
        name: build_id
        description: The ID of a build
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Builds
      - Build
      - Artifacts
  /v3/projects/{id}/builds/artifacts/{ref_name}/download:
    get:
      summary: Get Projects Builds Artifacts Ref Name Download
      description: Get projects builds artifacts ref name download.
      operationId: getV3ProjectsIdBuildsArtifactsRefNameDownload
      x-api-path-slug: v3projectsidbuildsartifactsref-namedownload-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: job
        description: The name for the build
      - in: path
        name: ref_name
        description: The ref from repository
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Builds
      - Artifacts
      - Ref
      - Name
      - Download
  /v3/projects/{id}/builds/{build_id}/trace:
    get:
      summary: Get Projects Builds Build Trace
      description: Get a trace of a specific build of a project
      operationId: getV3ProjectsIdBuildsBuildIdTrace
      x-api-path-slug: v3projectsidbuildsbuild-idtrace-get
      parameters:
      - in: path
        name: build_id
        description: The ID of a build
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Builds
      - Build
      - Trace
  /v3/projects/{id}/builds/{build_id}/cancel:
    post:
      summary: Post Projects Builds Build Cancel
      description: Cancel a specific build of a project
      operationId: postV3ProjectsIdBuildsBuildIdCancel
      x-api-path-slug: v3projectsidbuildsbuild-idcancel-post
      parameters:
      - in: path
        name: build_id
        description: The ID of a build
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Builds
      - Build
      - Cancel
  /v3/projects/{id}/builds/{build_id}/retry:
    post:
      summary: Post Projects Builds Build Retry
      description: Retry a specific build of a project
      operationId: postV3ProjectsIdBuildsBuildIdRetry
      x-api-path-slug: v3projectsidbuildsbuild-idretry-post
      parameters:
      - in: path
        name: build_id
        description: The ID of a build
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Builds
      - Build
      - Retry
  /v3/projects/{id}/builds/{build_id}/erase:
    post:
      summary: Post Projects Builds Build Erase
      description: Erase build (remove artifacts and build trace)
      operationId: postV3ProjectsIdBuildsBuildIdErase
      x-api-path-slug: v3projectsidbuildsbuild-iderase-post
      parameters:
      - in: path
        name: build_id
        description: The ID of a build
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Builds
      - Build
      - Erase
  /v3/projects/{id}/builds/{build_id}/artifacts/keep:
    post:
      summary: Post Projects Builds Build Artifacts Keep
      description: Keep the artifacts to prevent them from being deleted
      operationId: postV3ProjectsIdBuildsBuildIdArtifactsKeep
      x-api-path-slug: v3projectsidbuildsbuild-idartifactskeep-post
      parameters:
      - in: path
        name: build_id
        description: The ID of a build
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Builds
      - Build
      - Artifacts
      - Keep
  /v3/projects/{id}/builds/{build_id}/play:
    post:
      summary: Post Projects Builds Build Play
      description: This feature was added in GitLab 8.11
      operationId: postV3ProjectsIdBuildsBuildIdPlay
      x-api-path-slug: v3projectsidbuildsbuild-idplay-post
      parameters:
      - in: path
        name: build_id
        description: The ID of a Build
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Builds
      - Build
      - Play
  /v3/projects/{id}/repository/commits:
    get:
      summary: Get Projects Repository Commits
      description: Get a project repository commits
      operationId: getV3ProjectsIdRepositoryCommits
      x-api-path-slug: v3projectsidrepositorycommits-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: page
        description: The page for pagination
      - in: query
        name: path
        description: The file path
      - in: query
        name: per_page
        description: The number of results per page
      - in: query
        name: ref_name
        description: The name of a repository branch or tag, if not given the default
          branch is used
      - in: query
        name: since
        description: Only commits after or in this date will be returned
      - in: query
        name: until
        description: Only commits before or in this date will be returned
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Commits
    post:
      summary: Post Projects Repository Commits
      description: This feature was introduced in GitLab 8.13
      operationId: postV3ProjectsIdRepositoryCommits
      x-api-path-slug: v3projectsidrepositorycommits-post
      parameters:
      - in: formData
        name: actions
        description: Actions to perform in commit
      - in: formData
        name: author_email
        description: Author email for commit
      - in: formData
        name: author_name
        description: Author name for commit
      - in: formData
        name: branch_name
        description: The name of branch
      - in: formData
        name: commit_message
        description: Commit message
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Commits
  /v3/projects/{id}/repository/commits/{sha}:
    get:
      summary: Get Projects Repository Commits Sha
      description: Get projects repository commits sha.
      operationId: getV3ProjectsIdRepositoryCommitsSha
      x-api-path-slug: v3projectsidrepositorycommitssha-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: sha
        description: A commit sha, or the name of a branch or tag
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Commits
      - Sha
  /v3/projects/{id}/repository/commits/{sha}/diff:
    get:
      summary: Get Projects Repository Commits Sha Diff
      description: Get the diff for a specific commit of a project
      operationId: getV3ProjectsIdRepositoryCommitsShaDiff
      x-api-path-slug: v3projectsidrepositorycommitsshadiff-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: sha
        description: A commit sha, or the name of a branch or tag
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Commits
      - Sha
      - Diff
  /v3/projects/{id}/repository/commits/{sha}/comments:
    get:
      summary: Get Projects Repository Commits Sha Comments
      description: Get projects repository commits sha comments.
      operationId: getV3ProjectsIdRepositoryCommitsShaComments
      x-api-path-slug: v3projectsidrepositorycommitsshacomments-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: path
        name: sha
        description: A commit sha, or the name of a branch or tag
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Commits
      - Sha
      - Comments
    post:
      summary: Post Projects Repository Commits Sha Comments
      description: Post projects repository commits sha comments.
      operationId: postV3ProjectsIdRepositoryCommitsShaComments
      x-api-path-slug: v3projectsidrepositorycommitsshacomments-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: line
        description: The line number
      - in: formData
        name: line_type
        description: The type of the line
      - in: formData
        name: note
        description: The text of the comment
      - in: formData
        name: path
        description: The file path
      - in: path
        name: sha
        description: The commits SHA
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Commits
      - Sha
      - Comments
  /v3/projects/{id}/repository/commits/{sha}/cherry_pick:
    post:
      summary: Post Projects Repository Commits Sha Cherry Pick
      description: Post projects repository commits sha cherry pick.
      operationId: postV3ProjectsIdRepositoryCommitsShaCherryPick
      x-api-path-slug: v3projectsidrepositorycommitsshacherry-pick-post
      parameters:
      - in: formData
        name: branch
        description: The name of the branch
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: sha
        description: A commit sha to be cherry picked
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Commits
      - Sha
      - Cherry
      - Pick
  /v3/projects/{id}/repository/commits/{sha}/statuses:
    get:
      summary: Get Projects Repository Commits Sha Statuses
      description: Get projects repository commits sha statuses.
      operationId: getV3ProjectsIdRepositoryCommitsShaStatuses
      x-api-path-slug: v3projectsidrepositorycommitsshastatuses-get
      parameters:
      - in: query
        name: all
        description: 'Show all statuses, default: false'
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: name
        description: The name
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: ref
        description: The ref
      - in: path
        name: sha
        description: The commit hash
      - in: query
        name: stage
        description: The stage
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Commits
      - Sha
      - Statuses
  /v3/projects/{id}/statuses/{sha}:
    post:
      summary: Post Projects Statuses Sha
      description: Post projects statuses sha.
      operationId: postV3ProjectsIdStatusesSha
      x-api-path-slug: v3projectsidstatusessha-post
      parameters:
      - in: formData
        name: context
        description: A string label to differentiate this status from the status of
          other systems
      - in: formData
        name: description
        description: A short description of the status
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: name
        description: A string label to differentiate this status from the status of
          other systems
      - in: formData
        name: ref
        description: The ref
      - in: path
        name: sha
        description: The commit hash
      - in: formData
        name: state
        description: The state of the status
      - in: formData
        name: target_url
        description: The target URL to associate with this status
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Statuses
      - Sha
  /v3/projects/{id}/keys:
    get:
      summary: Get Projects Keys
      description: Get a specific project's deploy keys
      operationId: getV3ProjectsIdKeys
      x-api-path-slug: v3projectsidkeys-get
      parameters:
      - in: path
        name: id
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Keys
    post:
      summary: Post Projects Keys
      description: Add new deploy key to currently authenticated user
      operationId: postV3ProjectsIdKeys
      x-api-path-slug: v3projectsidkeys-post
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: formData
        name: key
        description: The new deploy key
      - in: formData
        name: title
        description: The name of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Keys
  /v3/projects/{id}/keys/{key_id}:
    get:
      summary: Get Projects Keys Key
      description: Get projects keys key.
      operationId: getV3ProjectsIdKeysKeyId
      x-api-path-slug: v3projectsidkeyskey-id-get
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Keys
      - Key
    delete:
      summary: Delete Projects Keys Key
      description: Delete deploy key for a project
      operationId: deleteV3ProjectsIdKeysKeyId
      x-api-path-slug: v3projectsidkeyskey-id-delete
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Keys
      - Key
  /v3/projects/{id}/keys/{key_id}/enable:
    post:
      summary: Post Projects Keys Key Enable
      description: This feature was added in GitLab 8.11
      operationId: postV3ProjectsIdKeysKeyIdEnable
      x-api-path-slug: v3projectsidkeyskey-idenable-post
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Keys
      - Key
      - Enable
  /v3/projects/{id}/keys/{key_id}/disable:
    delete:
      summary: Delete Projects Keys Key Disable
      description: This feature was added in GitLab 8.11
      operationId: deleteV3ProjectsIdKeysKeyIdDisable
      x-api-path-slug: v3projectsidkeyskey-iddisable-delete
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Keys
      - Key
      - Disable
  /v3/projects/{id}/deploy_keys:
    get:
      summary: Get Projects Deploy Keys
      description: Get a specific project's deploy keys
      operationId: getV3ProjectsIdDeployKeys
      x-api-path-slug: v3projectsiddeploy-keys-get
      parameters:
      - in: path
        name: id
        description: The ID of the project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
    post:
      summary: Post Projects Deploy Keys
      description: Add new deploy key to currently authenticated user
      operationId: postV3ProjectsIdDeployKeys
      x-api-path-slug: v3projectsiddeploy-keys-post
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: formData
        name: key
        description: The new deploy key
      - in: formData
        name: title
        description: The name of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
  /v3/projects/{id}/deploy_keys/{key_id}:
    get:
      summary: Get Projects Deploy Keys Key
      description: Get projects deploy keys key.
      operationId: getV3ProjectsIdDeployKeysKeyId
      x-api-path-slug: v3projectsiddeploy-keyskey-id-get
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
      - Key
    delete:
      summary: Delete Projects Deploy Keys Key
      description: Delete projects deploy keys key.
      operationId: deleteV3ProjectsIdDeployKeysKeyId
      x-api-path-slug: v3projectsiddeploy-keyskey-id-delete
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
      - Key
  /v3/projects/{id}/deploy_keys/{key_id}/enable:
    post:
      summary: Post Projects Deploy Keys Key Enable
      description: This feature was added in GitLab 8.11
      operationId: postV3ProjectsIdDeployKeysKeyIdEnable
      x-api-path-slug: v3projectsiddeploy-keyskey-idenable-post
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
      - Key
      - Enable
  /v3/projects/{id}/deploy_keys/{key_id}/disable:
    delete:
      summary: Delete Projects Deploy Keys Key Disable
      description: Delete projects deploy keys key disable.
      operationId: deleteV3ProjectsIdDeployKeysKeyIdDisable
      x-api-path-slug: v3projectsiddeploy-keyskey-iddisable-delete
      parameters:
      - in: path
        name: id
        description: The ID of the project
      - in: path
        name: key_id
        description: The ID of the deploy key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deploy
      - Keys
      - Key
      - Disable
  /v3/projects/{id}/deployments:
    get:
      summary: Get Projects Deployments
      description: This feature was introduced in GitLab 8.11.
      operationId: getV3ProjectsIdDeployments
      x-api-path-slug: v3projectsiddeployments-get
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deployments
  /v3/projects/{id}/deployments/{deployment_id}:
    get:
      summary: Get Projects Deployments Deployment
      description: This feature was introduced in GitLab 8.11.
      operationId: getV3ProjectsIdDeploymentsDeploymentId
      x-api-path-slug: v3projectsiddeploymentsdeployment-id-get
      parameters:
      - in: path
        name: deployment_id
        description: The deployment ID
      - in: path
        name: id
        description: The project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Deployments
      - Deployment
  /v3/projects/{id}/environments:
    get:
      summary: Get Projects Environments
      description: This feature was introduced in GitLab 8.11.
      operationId: getV3ProjectsIdEnvironments
      x-api-path-slug: v3projectsidenvironments-get
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Environments
    post:
      summary: Post Projects Environments
      description: This feature was introduced in GitLab 8.11.
      operationId: postV3ProjectsIdEnvironments
      x-api-path-slug: v3projectsidenvironments-post
      parameters:
      - in: formData
        name: external_url
        description: URL on which this deployment is viewable
      - in: path
        name: id
        description: The project ID
      - in: formData
        name: name
        description: The name of the environment to be created
      - in: formData
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Environments
  /v3/projects/{id}/environments/{environment_id}:
    put:
      summary: Put Projects Environments Environment
      description: This feature was introduced in GitLab 8.11.
      operationId: putV3ProjectsIdEnvironmentsEnvironmentId
      x-api-path-slug: v3projectsidenvironmentsenvironment-id-put
      parameters:
      - in: path
        name: environment_id
        description: The environment ID
      - in: formData
        name: external_url
        description: The new URL on which this deployment is viewable
      - in: path
        name: id
        description: The project ID
      - in: formData
        name: name
        description: The new environment name
      - in: formData
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Environments
      - Environment
    delete:
      summary: Delete Projects Environments Environment
      description: This feature was introduced in GitLab 8.11.
      operationId: deleteV3ProjectsIdEnvironmentsEnvironmentId
      x-api-path-slug: v3projectsidenvironmentsenvironment-id-delete
      parameters:
      - in: path
        name: environment_id
        description: The environment ID
      - in: path
        name: id
        description: The project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Environments
      - Environment
  /v3/projects/{id}/repository/files:
    get:
      summary: Get Projects Repository Files
      description: Get projects repository files.
      operationId: getV3ProjectsIdRepositoryFiles
      x-api-path-slug: v3projectsidrepositoryfiles-get
      parameters:
      - in: query
        name: file_path
        description: The path to the file
      - in: path
        name: id
        description: The project ID
      - in: query
        name: ref
        description: The name of branch, tag, or commit
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Files
    post:
      summary: Post Projects Repository Files
      description: Post projects repository files.
      operationId: postV3ProjectsIdRepositoryFiles
      x-api-path-slug: v3projectsidrepositoryfiles-post
      parameters:
      - in: formData
        name: author_email
        description: The email of the author
      - in: formData
        name: author_name
        description: The name of the author
      - in: formData
        name: branch_name
        description: The name of branch
      - in: formData
        name: commit_message
        description: Commit Message
      - in: formData
        name: content
        description: File content
      - in: formData
        name: encoding
        description: File encoding
      - in: formData
        name: file_path
        description: The path to new file
      - in: path
        name: id
        description: The project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Files
    put:
      summary: Put Projects Repository Files
      description: Update existing file in repository
      operationId: putV3ProjectsIdRepositoryFiles
      x-api-path-slug: v3projectsidrepositoryfiles-put
      parameters:
      - in: formData
        name: author_email
        description: The email of the author
      - in: formData
        name: author_name
        description: The name of the author
      - in: formData
        name: branch_name
        description: The name of branch
      - in: formData
        name: commit_message
        description: Commit Message
      - in: formData
        name: content
        description: File content
      - in: formData
        name: encoding
        description: File encoding
      - in: formData
        name: file_path
        description: The path to new file
      - in: path
        name: id
        description: The project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Files
    delete:
      summary: Delete Projects Repository Files
      description: Delete an existing file in repository
      operationId: deleteV3ProjectsIdRepositoryFiles
      x-api-path-slug: v3projectsidrepositoryfiles-delete
      parameters:
      - in: query
        name: author_email
        description: The email of the author
      - in: query
        name: author_name
        description: The name of the author
      - in: query
        name: branch_name
        description: The name of branch
      - in: query
        name: commit_message
        description: Commit Message
      - in: query
        name: file_path
        description: The path to new file
      - in: path
        name: id
        description: The project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Files
  /v3/projects/{id}/issues/{issue_id}/time_estimate:
    post:
      summary: Post Projects Issues Issue Time Estimate
      description: Post projects issues issue time estimate.
      operationId: postV3ProjectsIdIssuesIssueIdTimeEstimate
      x-api-path-slug: v3projectsidissuesissue-idtime-estimate-post
      parameters:
      - in: formData
        name: duration
        description: The duration to be parsed
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: issue_id
        description: The ID of a project issue
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Time
      - Estimate
  /v3/projects/{id}/issues/{issue_id}/reset_time_estimate:
    post:
      summary: Post Projects Issues Issue Reset Time Estimate
      description: Post projects issues issue reset time estimate.
      operationId: postV3ProjectsIdIssuesIssueIdResetTimeEstimate
      x-api-path-slug: v3projectsidissuesissue-idreset-time-estimate-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: issue_id
        description: The ID of a project issue
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Reset
      - Time
      - Estimate
  /v3/projects/{id}/issues/{issue_id}/add_spent_time:
    post:
      summary: Post Projects Issues Issue Add Spent Time
      description: Post projects issues issue add spent time.
      operationId: postV3ProjectsIdIssuesIssueIdAddSpentTime
      x-api-path-slug: v3projectsidissuesissue-idadd-spent-time-post
      parameters:
      - in: formData
        name: duration
        description: The duration to be parsed
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: issue_id
        description: The ID of a project issue
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - ""
      - Spent
      - Time
  /v3/projects/{id}/issues/{issue_id}/reset_spent_time:
    post:
      summary: Post Projects Issues Issue Reset Spent Time
      description: Post projects issues issue reset spent time.
      operationId: postV3ProjectsIdIssuesIssueIdResetSpentTime
      x-api-path-slug: v3projectsidissuesissue-idreset-spent-time-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: issue_id
        description: The ID of a project issue
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Reset
      - Spent
      - Time
  /v3/projects/{id}/issues/{issue_id}/time_stats:
    get:
      summary: Get Projects Issues Issue Time Stats
      description: Get projects issues issue time stats.
      operationId: getV3ProjectsIdIssuesIssueIdTimeStats
      x-api-path-slug: v3projectsidissuesissue-idtime-stats-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: issue_id
        description: The ID of a project issue
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Time
      - Stats
  /v3/projects/{id}/issues:
    get:
      summary: Get Projects Issues
      description: Get a list of project issues
      operationId: getV3ProjectsIdIssues
      x-api-path-slug: v3projectsidissues-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: iid
        description: Return the issue having the given `iid`
      - in: query
        name: labels
        description: Comma-separated list of label names
      - in: query
        name: milestone
        description: Return issues for a specific milestone
      - in: query
        name: order_by
        description: Return issues ordered by `created_at` or `updated_at` fields
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: sort
        description: Return issues sorted in `asc` or `desc` order
      - in: query
        name: state
        description: Return opened, closed, or all issues
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
    post:
      summary: Post Projects Issues
      description: Create a new project issue
      operationId: postV3ProjectsIdIssues
      x-api-path-slug: v3projectsidissues-post
      parameters:
      - in: formData
        name: assignee_id
        description: The ID of a user to assign issue
      - in: formData
        name: confidential
        description: Boolean parameter if the issue should be confidential
      - in: formData
        name: created_at
        description: Date time when the issue was created
      - in: formData
        name: description
        description: The description of an issue
      - in: formData
        name: due_date
        description: Date time string in the format YEAR-MONTH-DAY
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: labels
        description: Comma-separated list of label names
      - in: formData
        name: merge_request_for_resolving_discussions
        description: The IID of a merge request for which to resolve discussions
      - in: formData
        name: milestone_id
        description: The ID of a milestone to assign issue
      - in: formData
        name: title
        description: The title of an issue
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
  /v3/projects/{id}/issues/{issue_id}:
    get:
      summary: Get Projects Issues Issue
      description: Get a single project issue
      operationId: getV3ProjectsIdIssuesIssueId
      x-api-path-slug: v3projectsidissuesissue-id-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: issue_id
        description: The ID of a project issue
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
    put:
      summary: Put Projects Issues Issue
      description: Put projects issues issue.
      operationId: putV3ProjectsIdIssuesIssueId
      x-api-path-slug: v3projectsidissuesissue-id-put
      parameters:
      - in: formData
        name: assignee_id
        description: The ID of a user to assign issue
      - in: formData
        name: confidential
        description: Boolean parameter if the issue should be confidential
      - in: formData
        name: created_at
      - in: formData
        name: description
        description: The description of an issue
      - in: formData
        name: due_date
        description: Date time string in the format YEAR-MONTH-DAY
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: issue_id
        description: The ID of a project issue
      - in: formData
        name: labels
        description: Comma-separated list of label names
      - in: formData
        name: milestone_id
        description: The ID of a milestone to assign issue
      - in: formData
        name: state_event
        description: State of the issue
      - in: formData
        name: title
        description: The title of an issue
      - in: formData
        name: updated_at
        description: Date time when the issue was updated
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
    delete:
      summary: Delete Projects Issues Issue
      description: Delete projects issues issue.
      operationId: deleteV3ProjectsIdIssuesIssueId
      x-api-path-slug: v3projectsidissuesissue-id-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: issue_id
        description: The ID of a project issue
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
  /v3/projects/{id}/issues/{issue_id}/move:
    post:
      summary: Post Projects Issues Issue Move
      description: Post projects issues issue move.
      operationId: postV3ProjectsIdIssuesIssueIdMove
      x-api-path-slug: v3projectsidissuesissue-idmove-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: issue_id
        description: The ID of a project issue
      - in: formData
        name: to_project_id
        description: The ID of the new project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Move
  /v3/projects/{id}/labels:
    get:
      summary: Get Projects Labels
      description: Get all labels of the project
      operationId: getV3ProjectsIdLabels
      x-api-path-slug: v3projectsidlabels-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Labels
    post:
      summary: Post Projects Labels
      description: Post projects labels.
      operationId: postV3ProjectsIdLabels
      x-api-path-slug: v3projectsidlabels-post
      parameters:
      - in: formData
        name: color
        description: 'The color of the label given in 6-digit hex notation with leading
          # sign (e'
      - in: formData
        name: description
        description: The description of label to be created
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: name
        description: The name of the label to be created
      - in: formData
        name: priority
        description: The priority of the label
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Labels
    delete:
      summary: Delete Projects Labels
      description: Delete an existing label
      operationId: deleteV3ProjectsIdLabels
      x-api-path-slug: v3projectsidlabels-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: name
        description: The name of the label to be deleted
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Labels
    put:
      summary: Put Projects Labels
      description: Update an existing label. At least one optional parameter is required.
      operationId: putV3ProjectsIdLabels
      x-api-path-slug: v3projectsidlabels-put
      parameters:
      - in: formData
        name: color
        description: 'The new color of the label given in 6-digit hex notation with
          leading # sign (e'
      - in: formData
        name: description
        description: The new description of label
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: name
        description: The name of the label to be updated
      - in: formData
        name: new_name
        description: The new name of the label
      - in: formData
        name: priority
        description: The priority of the label
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Labels
  /v3/projects/{id}/members:
    get:
      summary: Get Projects Members
      description: Gets a list of group or project members viewable by the authenticated
        user.
      operationId: getV3ProjectsIdMembers
      x-api-path-slug: v3projectsidmembers-get
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: query
        description: A query string to search for members
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Members
    post:
      summary: Post Projects Members
      description: Adds a member to a group or project.
      operationId: postV3ProjectsIdMembers
      x-api-path-slug: v3projectsidmembers-post
      parameters:
      - in: formData
        name: access_level
        description: 'A valid access level (defaults: `30`, developer access level)'
      - in: formData
        name: expires_at
        description: Date string in the format YEAR-MONTH-DAY
      - in: path
        name: id
        description: The project ID
      - in: formData
        name: user_id
        description: The user ID of the new member
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Members
  /v3/projects/{id}/members/{user_id}:
    get:
      summary: Get Projects Members User
      description: Gets a member of a group or project.
      operationId: getV3ProjectsIdMembersUserId
      x-api-path-slug: v3projectsidmembersuser-id-get
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: path
        name: user_id
        description: The user ID of the member
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Members
      - User
    put:
      summary: Put Projects Members User
      description: Updates a member of a group or project.
      operationId: putV3ProjectsIdMembersUserId
      x-api-path-slug: v3projectsidmembersuser-id-put
      parameters:
      - in: formData
        name: access_level
        description: A valid access level
      - in: formData
        name: expires_at
        description: Date string in the format YEAR-MONTH-DAY
      - in: path
        name: id
        description: The project ID
      - in: path
        name: user_id
        description: The user ID of the new member
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Members
      - User
    delete:
      summary: Delete Projects Members User
      description: Removes a user from a group or project.
      operationId: deleteV3ProjectsIdMembersUserId
      x-api-path-slug: v3projectsidmembersuser-id-delete
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: path
        name: user_id
        description: The user ID of the member
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Members
      - User
  /v3/projects/{id}/merge_requests/{merge_request_id}/versions:
    get:
      summary: Get Projects Merge Requests Merge Request Versions
      description: Get projects merge requests merge request versions.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdVersions
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idversions-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a merge request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Versions
  /v3/projects/{id}/merge_requests/{merge_request_id}/versions/{version_id}:
    get:
      summary: Get Projects Merge Requests Merge Request Versions Version
      description: Get projects merge requests merge request versions version.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdVersionsVersionId
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idversionsversion-id-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a merge request
      - in: path
        name: version_id
        description: The ID of a merge request diff version
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Versions
      - Version
  /v3/projects/{id}/merge_requests/{merge_request_id}/time_estimate:
    post:
      summary: Post Projects Merge Requests Merge Request Time Estimate
      description: Post projects merge requests merge request time estimate.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdTimeEstimate
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idtime-estimate-post
      parameters:
      - in: formData
        name: duration
        description: The duration to be parsed
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a project merge_request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Time
      - Estimate
  /v3/projects/{id}/merge_requests/{merge_request_id}/reset_time_estimate:
    post:
      summary: Post Projects Merge Requests Merge Request Reset Time Estimate
      description: Post projects merge requests merge request reset time estimate.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdResetTimeEstimate
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idreset-time-estimate-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a project merge_request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Reset
      - Time
      - Estimate
  /v3/projects/{id}/merge_requests/{merge_request_id}/add_spent_time:
    post:
      summary: Post Projects Merge Requests Merge Request Add Spent Time
      description: Post projects merge requests merge request add spent time.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdAddSpentTime
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idadd-spent-time-post
      parameters:
      - in: formData
        name: duration
        description: The duration to be parsed
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a project merge_request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - ""
      - Spent
      - Time
  /v3/projects/{id}/merge_requests/{merge_request_id}/reset_spent_time:
    post:
      summary: Post Projects Merge Requests Merge Request Reset Spent Time
      description: Post projects merge requests merge request reset spent time.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdResetSpentTime
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idreset-spent-time-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a project merge_request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Reset
      - Spent
      - Time
  /v3/projects/{id}/merge_requests/{merge_request_id}/time_stats:
    get:
      summary: Get Projects Merge Requests Merge Request Time Stats
      description: Get projects merge requests merge request time stats.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdTimeStats
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idtime-stats-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a project merge_request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Time
      - Stats
  /v3/projects/{id}/merge_requests:
    get:
      summary: Get Projects Merge Requests
      description: Get projects merge requests.
      operationId: getV3ProjectsIdMergeRequests
      x-api-path-slug: v3projectsidmerge-requests-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: iid
        description: The IID of the merge requests
      - in: query
        name: order_by
        description: Return merge requests ordered by `created_at` or `updated_at`
          fields
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: sort
        description: Return merge requests sorted in `asc` or `desc` order
      - in: query
        name: state
        description: Return opened, closed, merged, or all merge requests
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
    post:
      summary: Post Projects Merge Requests
      description: Post projects merge requests.
      operationId: postV3ProjectsIdMergeRequests
      x-api-path-slug: v3projectsidmerge-requests-post
      parameters:
      - in: formData
        name: assignee_id
        description: The ID of a user to assign the merge request
      - in: formData
        name: description
        description: The description of the merge request
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: labels
        description: Comma-separated list of label names
      - in: formData
        name: milestone_id
        description: The ID of a milestone to assign the merge request
      - in: formData
        name: remove_source_branch
        description: Remove source branch when merging
      - in: formData
        name: source_branch
        description: The source branch
      - in: formData
        name: target_branch
        description: The target branch
      - in: formData
        name: target_project_id
        description: The target project of the merge request defaults to the :id of
          the project
      - in: formData
        name: title
        description: The title of the merge request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
  /v3/projects/{id}/merge_requests/{merge_request_id}:
    delete:
      summary: Delete Projects Merge Requests Merge Request
      description: Delete projects merge requests merge request.
      operationId: deleteV3ProjectsIdMergeRequestsMergeRequestId
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-id-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a merge request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
    get:
      summary: Get Projects Merge Requests Merge Request
      description: Get projects merge requests merge request.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestId
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-id-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
    put:
      summary: Put Projects Merge Requests Merge Request
      description: Put projects merge requests merge request.
      operationId: putV3ProjectsIdMergeRequestsMergeRequestId
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-id-put
      parameters:
      - in: formData
        name: assignee_id
        description: The ID of a user to assign the merge request
      - in: formData
        name: description
        description: The description of the merge request
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: labels
        description: Comma-separated list of label names
      - in: path
        name: merge_request_id
      - in: formData
        name: milestone_id
        description: The ID of a milestone to assign the merge request
      - in: formData
        name: remove_source_branch
        description: Remove source branch when merging
      - in: formData
        name: state_event
        description: Status of the merge request
      - in: formData
        name: target_branch
        description: The target branch
      - in: formData
        name: title
        description: The title of the merge request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
  /v3/projects/{id}/merge_request/{merge_request_id}:
    get:
      summary: Get Projects Merge Request Merge Request
      description: This endpoint is deprecated and will be removed in GitLab 9.0.
      operationId: getV3ProjectsIdMergeRequestMergeRequestId
      x-api-path-slug: v3projectsidmerge-requestmerge-request-id-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of a merge request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
    put:
      summary: Put Projects Merge Request Merge Request
      description: Put projects merge request merge request.
      operationId: putV3ProjectsIdMergeRequestMergeRequestId
      x-api-path-slug: v3projectsidmerge-requestmerge-request-id-put
      parameters:
      - in: formData
        name: assignee_id
        description: The ID of a user to assign the merge request
      - in: formData
        name: description
        description: The description of the merge request
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: labels
        description: Comma-separated list of label names
      - in: path
        name: merge_request_id
      - in: formData
        name: milestone_id
        description: The ID of a milestone to assign the merge request
      - in: formData
        name: remove_source_branch
        description: Remove source branch when merging
      - in: formData
        name: state_event
        description: Status of the merge request
      - in: formData
        name: target_branch
        description: The target branch
      - in: formData
        name: title
        description: The title of the merge request
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
  /v3/projects/{id}/merge_request/{merge_request_id}/commits:
    get:
      summary: Get Projects Merge Request Merge Request Commits
      description: Get projects merge request merge request commits.
      operationId: getV3ProjectsIdMergeRequestMergeRequestIdCommits
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idcommits-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Commits
  /v3/projects/{id}/merge_request/{merge_request_id}/changes:
    get:
      summary: Get Projects Merge Request Merge Request Changes
      description: Get projects merge request merge request changes.
      operationId: getV3ProjectsIdMergeRequestMergeRequestIdChanges
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idchanges-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Changes
  /v3/projects/{id}/merge_request/{merge_request_id}/merge:
    put:
      summary: Put Projects Merge Request Merge Request Merge
      description: Put projects merge request merge request merge.
      operationId: putV3ProjectsIdMergeRequestMergeRequestIdMerge
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idmerge-put
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: merge_commit_message
        description: Custom merge commit message
      - in: path
        name: merge_request_id
      - in: formData
        name: merge_when_build_succeeds
        description: When true, this merge request will be merged when the pipeline
          succeeds
      - in: formData
        name: sha
        description: When present, must have the HEAD SHA of the source branch
      - in: formData
        name: should_remove_source_branch
        description: When true, the source branch will be deleted if possible
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Merge
  /v3/projects/{id}/merge_request/{merge_request_id}/cancel_merge_when_build_succeeds:
    post:
      summary: Post Projects Merge Request Merge Request Cancel Merge When Build Succeeds
      description: Post projects merge request merge request cancel merge when build
        succeeds.
      operationId: postV3ProjectsIdMergeRequestMergeRequestIdCancelMergeWhenBuildSucceeds
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idcancel-merge-when-build-succeeds-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Cancel
      - Merge
      - When
      - Build
      - Succeeds
  /v3/projects/{id}/merge_request/{merge_request_id}/comments:
    get:
      summary: Get Projects Merge Request Merge Request Comments
      description: Get projects merge request merge request comments.
      operationId: getV3ProjectsIdMergeRequestMergeRequestIdComments
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idcomments-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Comments
    post:
      summary: Post Projects Merge Request Merge Request Comments
      description: Post projects merge request merge request comments.
      operationId: postV3ProjectsIdMergeRequestMergeRequestIdComments
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idcomments-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      - in: formData
        name: note
        description: The text of the comment
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Comments
  /v3/projects/{id}/merge_request/{merge_request_id}/closes_issues:
    get:
      summary: Get Projects Merge Request Merge Request Closes Issues
      description: Get projects merge request merge request closes issues.
      operationId: getV3ProjectsIdMergeRequestMergeRequestIdClosesIssues
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idcloses-issues-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Closes
      - Issues
  /v3/projects/{id}/merge_requests/{merge_request_id}/commits:
    get:
      summary: Get Projects Merge Requests Merge Request Commits
      description: Get projects merge requests merge request commits.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdCommits
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idcommits-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Commits
  /v3/projects/{id}/merge_requests/{merge_request_id}/changes:
    get:
      summary: Get Projects Merge Requests Merge Request Changes
      description: Get projects merge requests merge request changes.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdChanges
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idchanges-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Changes
  /v3/projects/{id}/merge_requests/{merge_request_id}/merge:
    put:
      summary: Put Projects Merge Requests Merge Request Merge
      description: Put projects merge requests merge request merge.
      operationId: putV3ProjectsIdMergeRequestsMergeRequestIdMerge
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idmerge-put
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: merge_commit_message
        description: Custom merge commit message
      - in: path
        name: merge_request_id
      - in: formData
        name: merge_when_build_succeeds
        description: When true, this merge request will be merged when the pipeline
          succeeds
      - in: formData
        name: sha
        description: When present, must have the HEAD SHA of the source branch
      - in: formData
        name: should_remove_source_branch
        description: When true, the source branch will be deleted if possible
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Merge
  /v3/projects/{id}/merge_requests/{merge_request_id}/cancel_merge_when_build_succeeds:
    post:
      summary: Post Projects Merge Requests Merge Request Cancel Merge When Build
        Succeeds
      description: Post projects merge requests merge request cancel merge when build
        succeeds.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdCancelMergeWhenBuildSucceeds
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idcancel-merge-when-build-succeeds-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Cancel
      - Merge
      - When
      - Build
      - Succeeds
  /v3/projects/{id}/merge_requests/{merge_request_id}/comments:
    get:
      summary: Get Projects Merge Requests Merge Request Comments
      description: Get projects merge requests merge request comments.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdComments
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idcomments-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Comments
    post:
      summary: Post Projects Merge Requests Merge Request Comments
      description: Post projects merge requests merge request comments.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdComments
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idcomments-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      - in: formData
        name: note
        description: The text of the comment
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Comments
  /v3/projects/{id}/merge_requests/{merge_request_id}/closes_issues:
    get:
      summary: Get Projects Merge Requests Merge Request Closes Issues
      description: Get projects merge requests merge request closes issues.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdClosesIssues
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idcloses-issues-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Closes
      - Issues
  /v3/projects/{id}/milestones:
    get:
      summary: Get Projects Milestones
      description: Get a list of project milestones
      operationId: getV3ProjectsIdMilestones
      x-api-path-slug: v3projectsidmilestones-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: iid
        description: The IID of the milestone
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: state
        description: Return active, closed, or all milestones
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Milestones
    post:
      summary: Post Projects Milestones
      description: Create a new project milestone
      operationId: postV3ProjectsIdMilestones
      x-api-path-slug: v3projectsidmilestones-post
      parameters:
      - in: formData
        name: description
        description: The description of the milestone
      - in: formData
        name: due_date
        description: The due date of the milestone
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: start_date
        description: The start date of the milestone
      - in: formData
        name: title
        description: The title of the milestone
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Milestones
  /v3/projects/{id}/milestones/{milestone_id}:
    get:
      summary: Get Projects Milestones Milestone
      description: Get projects milestones milestone.
      operationId: getV3ProjectsIdMilestonesMilestoneId
      x-api-path-slug: v3projectsidmilestonesmilestone-id-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: milestone_id
        description: The ID of a project milestone
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Milestones
      - Milestone
    put:
      summary: Put Projects Milestones Milestone
      description: Update an existing project milestone
      operationId: putV3ProjectsIdMilestonesMilestoneId
      x-api-path-slug: v3projectsidmilestonesmilestone-id-put
      parameters:
      - in: formData
        name: description
        description: The description of the milestone
      - in: formData
        name: due_date
        description: The due date of the milestone
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: milestone_id
        description: The ID of a project milestone
      - in: formData
        name: start_date
        description: The start date of the milestone
      - in: formData
        name: state_event
        description: The state event of the milestone
      - in: formData
        name: title
        description: The title of the milestone
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Milestones
      - Milestone
  /v3/projects/{id}/milestones/{milestone_id}/issues:
    get:
      summary: Get Projects Milestones Milestone Issues
      description: Get all issues for a single project milestone
      operationId: getV3ProjectsIdMilestonesMilestoneIdIssues
      x-api-path-slug: v3projectsidmilestonesmilestone-idissues-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: milestone_id
        description: The ID of a project milestone
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Milestones
      - Milestone
      - Issues
  /v3/projects/{id}/issues/{noteable_id}/notes:
    get:
      summary: Get Projects Issues Noteable Notes
      description: Get a list of project +noteable+ notes
      operationId: getV3ProjectsIdIssuesNoteableIdNotes
      x-api-path-slug: v3projectsidissuesnoteable-idnotes-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: noteable_id
        description: The ID of the noteable
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Noteable
      - Notes
    post:
      summary: Post Projects Issues Noteable Notes
      description: Post projects issues noteable notes.
      operationId: postV3ProjectsIdIssuesNoteableIdNotes
      x-api-path-slug: v3projectsidissuesnoteable-idnotes-post
      parameters:
      - in: formData
        name: body
        description: The content of a note
      - in: formData
        name: created_at
        description: The creation date of the note
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: noteable_id
        description: The ID of the noteable
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Noteable
      - Notes
  /v3/projects/{id}/issues/{noteable_id}/notes/{note_id}:
    get:
      summary: Get Projects Issues Noteable Notes Note
      description: Get projects issues noteable notes note.
      operationId: getV3ProjectsIdIssuesNoteableIdNotesNoteId
      x-api-path-slug: v3projectsidissuesnoteable-idnotesnote-id-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: noteable_id
        description: The ID of the noteable
      - in: path
        name: note_id
        description: The ID of a note
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Noteable
      - Notes
      - Note
    put:
      summary: Put Projects Issues Noteable Notes Note
      description: Put projects issues noteable notes note.
      operationId: putV3ProjectsIdIssuesNoteableIdNotesNoteId
      x-api-path-slug: v3projectsidissuesnoteable-idnotesnote-id-put
      parameters:
      - in: formData
        name: body
        description: The content of a note
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: noteable_id
        description: The ID of the noteable
      - in: path
        name: note_id
        description: The ID of a note
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Noteable
      - Notes
      - Note
    delete:
      summary: Delete Projects Issues Noteable Notes Note
      description: Delete projects issues noteable notes note.
      operationId: deleteV3ProjectsIdIssuesNoteableIdNotesNoteId
      x-api-path-slug: v3projectsidissuesnoteable-idnotesnote-id-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: noteable_id
        description: The ID of the noteable
      - in: path
        name: note_id
        description: The ID of a note
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Noteable
      - Notes
      - Note
  /v3/projects/{id}/merge_requests/{noteable_id}/notes:
    get:
      summary: Get Projects Merge Requests Noteable Notes
      description: Get projects merge requests noteable notes.
      operationId: getV3ProjectsIdMergeRequestsNoteableIdNotes
      x-api-path-slug: v3projectsidmerge-requestsnoteable-idnotes-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: noteable_id
        description: The ID of the noteable
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Noteable
      - Notes
    post:
      summary: Post Projects Merge Requests Noteable Notes
      description: Post projects merge requests noteable notes.
      operationId: postV3ProjectsIdMergeRequestsNoteableIdNotes
      x-api-path-slug: v3projectsidmerge-requestsnoteable-idnotes-post
      parameters:
      - in: formData
        name: body
        description: The content of a note
      - in: formData
        name: created_at
        description: The creation date of the note
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: noteable_id
        description: The ID of the noteable
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Noteable
      - Notes
  /v3/projects/{id}/merge_requests/{noteable_id}/notes/{note_id}:
    get:
      summary: Get Projects Merge Requests Noteable Notes Note
      description: Get projects merge requests noteable notes note.
      operationId: getV3ProjectsIdMergeRequestsNoteableIdNotesNoteId
      x-api-path-slug: v3projectsidmerge-requestsnoteable-idnotesnote-id-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: noteable_id
        description: The ID of the noteable
      - in: path
        name: note_id
        description: The ID of a note
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Noteable
      - Notes
      - Note
    put:
      summary: Put Projects Merge Requests Noteable Notes Note
      description: Put projects merge requests noteable notes note.
      operationId: putV3ProjectsIdMergeRequestsNoteableIdNotesNoteId
      x-api-path-slug: v3projectsidmerge-requestsnoteable-idnotesnote-id-put
      parameters:
      - in: formData
        name: body
        description: The content of a note
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: noteable_id
        description: The ID of the noteable
      - in: path
        name: note_id
        description: The ID of a note
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Noteable
      - Notes
      - Note
    delete:
      summary: Delete Projects Merge Requests Noteable Notes Note
      description: Delete projects merge requests noteable notes note.
      operationId: deleteV3ProjectsIdMergeRequestsNoteableIdNotesNoteId
      x-api-path-slug: v3projectsidmerge-requestsnoteable-idnotesnote-id-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: noteable_id
        description: The ID of the noteable
      - in: path
        name: note_id
        description: The ID of a note
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Noteable
      - Notes
      - Note
  /v3/projects/{id}/snippets/{noteable_id}/notes:
    get:
      summary: Get Projects Snippets Noteable Notes
      description: Get a list of project +noteable+ notes
      operationId: getV3ProjectsIdSnippetsNoteableIdNotes
      x-api-path-slug: v3projectsidsnippetsnoteable-idnotes-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: noteable_id
        description: The ID of the noteable
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Noteable
      - Notes
    post:
      summary: Post Projects Snippets Noteable Notes
      description: Post projects snippets noteable notes.
      operationId: postV3ProjectsIdSnippetsNoteableIdNotes
      x-api-path-slug: v3projectsidsnippetsnoteable-idnotes-post
      parameters:
      - in: formData
        name: body
        description: The content of a note
      - in: formData
        name: created_at
        description: The creation date of the note
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: noteable_id
        description: The ID of the noteable
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Noteable
      - Notes
  /v3/projects/{id}/snippets/{noteable_id}/notes/{note_id}:
    get:
      summary: Get Projects Snippets Noteable Notes Note
      description: Get projects snippets noteable notes note.
      operationId: getV3ProjectsIdSnippetsNoteableIdNotesNoteId
      x-api-path-slug: v3projectsidsnippetsnoteable-idnotesnote-id-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: noteable_id
        description: The ID of the noteable
      - in: path
        name: note_id
        description: The ID of a note
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Noteable
      - Notes
      - Note
    put:
      summary: Put Projects Snippets Noteable Notes Note
      description: Put projects snippets noteable notes note.
      operationId: putV3ProjectsIdSnippetsNoteableIdNotesNoteId
      x-api-path-slug: v3projectsidsnippetsnoteable-idnotesnote-id-put
      parameters:
      - in: formData
        name: body
        description: The content of a note
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: noteable_id
        description: The ID of the noteable
      - in: path
        name: note_id
        description: The ID of a note
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Noteable
      - Notes
      - Note
    delete:
      summary: Delete Projects Snippets Noteable Notes Note
      description: Delete projects snippets noteable notes note.
      operationId: deleteV3ProjectsIdSnippetsNoteableIdNotesNoteId
      x-api-path-slug: v3projectsidsnippetsnoteable-idnotesnote-id-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: noteable_id
        description: The ID of the noteable
      - in: path
        name: note_id
        description: The ID of a note
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Noteable
      - Notes
      - Note
  /v3/projects/{id}/notification_settings:
    get:
      summary: Get Projects Notification Settings
      description: This feature was introduced in GitLab 8.12
      operationId: getV3ProjectsIdNotificationSettings
      x-api-path-slug: v3projectsidnotification-settings-get
      parameters:
      - in: path
        name: id
        description: The group ID or project ID or project NAMESPACE/PROJECT_NAME
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Notification
      - Settings
    put:
      summary: Put Projects Notification Settings
      description: This feature was introduced in GitLab 8.12
      operationId: putV3ProjectsIdNotificationSettings
      x-api-path-slug: v3projectsidnotification-settings-put
      parameters:
      - in: formData
        name: close_issue
        description: Enable/disable this notification
      - in: formData
        name: close_merge_request
        description: Enable/disable this notification
      - in: formData
        name: failed_pipeline
        description: Enable/disable this notification
      - in: path
        name: id
        description: The group ID or project ID or project NAMESPACE/PROJECT_NAME
      - in: formData
        name: level
        description: The project notification level
      - in: formData
        name: merge_merge_request
        description: Enable/disable this notification
      - in: formData
        name: new_issue
        description: Enable/disable this notification
      - in: formData
        name: new_merge_request
        description: Enable/disable this notification
      - in: formData
        name: new_note
        description: Enable/disable this notification
      - in: formData
        name: reassign_issue
        description: Enable/disable this notification
      - in: formData
        name: reassign_merge_request
        description: Enable/disable this notification
      - in: formData
        name: reopen_issue
        description: Enable/disable this notification
      - in: formData
        name: reopen_merge_request
        description: Enable/disable this notification
      - in: formData
        name: success_pipeline
        description: Enable/disable this notification
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Notification
      - Settings
  /v3/projects/{id}/pipelines:
    get:
      summary: Get Projects Pipelines
      description: This feature was introduced in GitLab 8.11.
      operationId: getV3ProjectsIdPipelines
      x-api-path-slug: v3projectsidpipelines-get
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: scope
        description: Either running, branches, or tags
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Pipelines
  /v3/projects/{id}/pipeline:
    post:
      summary: Post Projects Pipeline
      description: This feature was introduced in GitLab 8.14
      operationId: postV3ProjectsIdPipeline
      x-api-path-slug: v3projectsidpipeline-post
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: formData
        name: ref
        description: Reference
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Pipeline
  /v3/projects/{id}/pipelines/{pipeline_id}:
    get:
      summary: Get Projects Pipelines Pipeline
      description: This feature was introduced in GitLab 8.11
      operationId: getV3ProjectsIdPipelinesPipelineId
      x-api-path-slug: v3projectsidpipelinespipeline-id-get
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: path
        name: pipeline_id
        description: The pipeline ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Pipelines
      - Pipeline
  /v3/projects/{id}/pipelines/{pipeline_id}/retry:
    post:
      summary: Post Projects Pipelines Pipeline Retry
      description: This feature was introduced in GitLab 8.11.
      operationId: postV3ProjectsIdPipelinesPipelineIdRetry
      x-api-path-slug: v3projectsidpipelinespipeline-idretry-post
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: path
        name: pipeline_id
        description: The pipeline ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Pipelines
      - Pipeline
      - Retry
  /v3/projects/{id}/pipelines/{pipeline_id}/cancel:
    post:
      summary: Post Projects Pipelines Pipeline Cancel
      description: This feature was introduced in GitLab 8.11.
      operationId: postV3ProjectsIdPipelinesPipelineIdCancel
      x-api-path-slug: v3projectsidpipelinespipeline-idcancel-post
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: path
        name: pipeline_id
        description: The pipeline ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Pipelines
      - Pipeline
      - Cancel
  /v3/projects/{id}/hooks:
    get:
      summary: Get Projects Hooks
      description: Get projects hooks.
      operationId: getV3ProjectsIdHooks
      x-api-path-slug: v3projectsidhooks-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Hooks
    post:
      summary: Post Projects Hooks
      description: Post projects hooks.
      operationId: postV3ProjectsIdHooks
      x-api-path-slug: v3projectsidhooks-post
      parameters:
      - in: formData
        name: build_events
        description: Trigger hook on build events
      - in: formData
        name: enable_ssl_verification
        description: Do SSL verification when triggering the hook
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: issues_events
        description: Trigger hook on issues events
      - in: formData
        name: merge_requests_events
        description: Trigger hook on merge request events
      - in: formData
        name: note_events
        description: Trigger hook on note(comment) events
      - in: formData
        name: pipeline_events
        description: Trigger hook on pipeline events
      - in: formData
        name: push_events
        description: Trigger hook on push events
      - in: formData
        name: tag_push_events
        description: Trigger hook on tag push events
      - in: formData
        name: token
        description: Secret token to validate received payloads; this will not be
          returned in the response
      - in: formData
        name: url
        description: The URL to send the request to
      - in: formData
        name: wiki_page_events
        description: Trigger hook on wiki events
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Hooks
  /v3/projects/{id}/hooks/{hook_id}:
    get:
      summary: Get Projects Hooks Hook
      description: Get projects hooks hook.
      operationId: getV3ProjectsIdHooksHookId
      x-api-path-slug: v3projectsidhookshook-id-get
      parameters:
      - in: path
        name: hook_id
        description: The ID of a project hook
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Hooks
      - Hook
    put:
      summary: Put Projects Hooks Hook
      description: Update an existing project hook
      operationId: putV3ProjectsIdHooksHookId
      x-api-path-slug: v3projectsidhookshook-id-put
      parameters:
      - in: formData
        name: build_events
        description: Trigger hook on build events
      - in: formData
        name: enable_ssl_verification
        description: Do SSL verification when triggering the hook
      - in: path
        name: hook_id
        description: The ID of the hook to update
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: issues_events
        description: Trigger hook on issues events
      - in: formData
        name: merge_requests_events
        description: Trigger hook on merge request events
      - in: formData
        name: note_events
        description: Trigger hook on note(comment) events
      - in: formData
        name: pipeline_events
        description: Trigger hook on pipeline events
      - in: formData
        name: push_events
        description: Trigger hook on push events
      - in: formData
        name: tag_push_events
        description: Trigger hook on tag push events
      - in: formData
        name: token
        description: Secret token to validate received payloads; this will not be
          returned in the response
      - in: formData
        name: url
        description: The URL to send the request to
      - in: formData
        name: wiki_page_events
        description: Trigger hook on wiki events
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Hooks
      - Hook
    delete:
      summary: Delete Projects Hooks Hook
      description: Delete projects hooks hook.
      operationId: deleteV3ProjectsIdHooksHookId
      x-api-path-slug: v3projectsidhookshook-id-delete
      parameters:
      - in: path
        name: hook_id
        description: The ID of the hook to delete
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Hooks
      - Hook
  /v3/projects/visible:
    get:
      summary: Get Projects Visible
      description: Get a list of visible projects for authenticated user
      operationId: getV3ProjectsVisible
      x-api-path-slug: v3projectsvisible-get
      parameters:
      - in: query
        name: archived
        description: Limit by archived status
      - in: query
        name: order_by
        description: Return projects ordered by field
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: search
        description: Return list of authorized projects matching the search criteria
      - in: query
        name: simple
        description: Return only the ID, URL, name, and path of each project
      - in: query
        name: sort
        description: Return projects sorted in ascending and descending order
      - in: query
        name: visibility
        description: Limit by visibility
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Visible
  /v3/projects:
    get:
      summary: Get Projects
      description: Get a projects list for authenticated user
      operationId: getV3Projects
      x-api-path-slug: v3projects-get
      parameters:
      - in: query
        name: archived
        description: Limit by archived status
      - in: query
        name: order_by
        description: Return projects ordered by field
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: search
        description: Return list of authorized projects matching the search criteria
      - in: query
        name: simple
        description: Return only the ID, URL, name, and path of each project
      - in: query
        name: sort
        description: Return projects sorted in ascending and descending order
      - in: query
        name: visibility
        description: Limit by visibility
      responses:
        200:
          description: OK
      tags:
      - Projects
    post:
      summary: Post Projects
      description: Create new project
      operationId: postV3Projects
      x-api-path-slug: v3projects-post
      parameters:
      - in: formData
        name: builds_enabled
        description: Flag indication if builds are enabled
      - in: formData
        name: container_registry_enabled
        description: Flag indication if the container registry is enabled for that
          project
      - in: formData
        name: description
        description: The description of the project
      - in: formData
        name: import_url
        description: URL from which the project is imported
      - in: formData
        name: issues_enabled
        description: Flag indication if the issue tracker is enabled
      - in: formData
        name: lfs_enabled
        description: Flag indication if Git LFS is enabled for that project
      - in: formData
        name: merge_requests_enabled
        description: Flag indication if merge requests are enabled
      - in: formData
        name: name
        description: The name of the project
      - in: formData
        name: namespace_id
        description: Namespace ID for the new project
      - in: formData
        name: only_allow_merge_if_all_discussions_are_resolved
        description: Only allow to merge if all discussions are resolved
      - in: formData
        name: only_allow_merge_if_build_succeeds
        description: Only allow to merge if builds succeed
      - in: formData
        name: path
        description: The path of the repository
      - in: formData
        name: public
        description: Create a public project
      - in: formData
        name: public_builds
        description: Perform public builds
      - in: formData
        name: request_access_enabled
        description: Allow users to request member access
      - in: formData
        name: shared_runners_enabled
        description: Flag indication if shared runners are enabled for that project
      - in: formData
        name: snippets_enabled
        description: Flag indication if snippets are enabled
      - in: formData
        name: visibility_level
        description: Create a public project
      - in: formData
        name: wiki_enabled
        description: Flag indication if the wiki is enabled
      responses:
        200:
          description: OK
      tags:
      - Projects
  /v3/projects/owned:
    get:
      summary: Get Projects Owned
      description: Get an owned projects list for authenticated user
      operationId: getV3ProjectsOwned
      x-api-path-slug: v3projectsowned-get
      parameters:
      - in: query
        name: archived
        description: Limit by archived status
      - in: query
        name: order_by
        description: Return projects ordered by field
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: search
        description: Return list of authorized projects matching the search criteria
      - in: query
        name: simple
        description: Return only the ID, URL, name, and path of each project
      - in: query
        name: sort
        description: Return projects sorted in ascending and descending order
      - in: query
        name: statistics
        description: Include project statistics
      - in: query
        name: visibility
        description: Limit by visibility
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Owned
  /v3/projects/starred:
    get:
      summary: Get Projects Starred
      description: Gets starred project for the authenticated user
      operationId: getV3ProjectsStarred
      x-api-path-slug: v3projectsstarred-get
      parameters:
      - in: query
        name: archived
        description: Limit by archived status
      - in: query
        name: order_by
        description: Return projects ordered by field
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: search
        description: Return list of authorized projects matching the search criteria
      - in: query
        name: simple
        description: Return only the ID, URL, name, and path of each project
      - in: query
        name: sort
        description: Return projects sorted in ascending and descending order
      - in: query
        name: visibility
        description: Limit by visibility
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Starred
  /v3/projects/all:
    get:
      summary: Get Projects All
      description: Get all projects for admin user
      operationId: getV3ProjectsAll
      x-api-path-slug: v3projectsall-get
      parameters:
      - in: query
        name: archived
        description: Limit by archived status
      - in: query
        name: order_by
        description: Return projects ordered by field
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: search
        description: Return list of authorized projects matching the search criteria
      - in: query
        name: simple
        description: Return only the ID, URL, name, and path of each project
      - in: query
        name: sort
        description: Return projects sorted in ascending and descending order
      - in: query
        name: statistics
        description: Include project statistics
      - in: query
        name: visibility
        description: Limit by visibility
      responses:
        200:
          description: OK
      tags:
      - Projects
  /v3/projects/search/{query}:
    get:
      summary: Get Projects Search Query
      description: Search for projects the current user has access to
      operationId: getV3ProjectsSearchQuery
      x-api-path-slug: v3projectssearchquery-get
      parameters:
      - in: query
        name: order_by
        description: Return projects ordered by field
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: path
        name: query
        description: The project name to be searched
      - in: query
        name: sort
        description: Return projects sorted in ascending and descending order
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Search
      - Query
  /v3/projects/user/{user_id}:
    post:
      summary: Post Projects User User
      description: Create new project for a specified user. Only available to admin
        users.
      operationId: postV3ProjectsUserUserId
      x-api-path-slug: v3projectsuseruser-id-post
      parameters:
      - in: formData
        name: builds_enabled
        description: Flag indication if builds are enabled
      - in: formData
        name: container_registry_enabled
        description: Flag indication if the container registry is enabled for that
          project
      - in: formData
        name: default_branch
        description: The default branch of the project
      - in: formData
        name: description
        description: The description of the project
      - in: formData
        name: import_url
        description: URL from which the project is imported
      - in: formData
        name: issues_enabled
        description: Flag indication if the issue tracker is enabled
      - in: formData
        name: lfs_enabled
        description: Flag indication if Git LFS is enabled for that project
      - in: formData
        name: merge_requests_enabled
        description: Flag indication if merge requests are enabled
      - in: formData
        name: name
        description: The name of the project
      - in: formData
        name: namespace_id
        description: Namespace ID for the new project
      - in: formData
        name: only_allow_merge_if_all_discussions_are_resolved
        description: Only allow to merge if all discussions are resolved
      - in: formData
        name: only_allow_merge_if_build_succeeds
        description: Only allow to merge if builds succeed
      - in: formData
        name: public
        description: Create a public project
      - in: formData
        name: public_builds
        description: Perform public builds
      - in: formData
        name: request_access_enabled
        description: Allow users to request member access
      - in: formData
        name: shared_runners_enabled
        description: Flag indication if shared runners are enabled for that project
      - in: formData
        name: snippets_enabled
        description: Flag indication if snippets are enabled
      - in: path
        name: user_id
        description: The ID of a user
      - in: formData
        name: visibility_level
        description: Create a public project
      - in: formData
        name: wiki_enabled
        description: Flag indication if the wiki is enabled
      responses:
        200:
          description: OK
      tags:
      - Projects
      - User
      - User
  /v3/projects/{id}:
    get:
      summary: Get Projects
      description: Get a single project
      operationId: getV3ProjectsId
      x-api-path-slug: v3projectsid-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
    put:
      summary: Put Projects
      description: Update an existing project
      operationId: putV3ProjectsId
      x-api-path-slug: v3projectsid-put
      parameters:
      - in: formData
        name: builds_enabled
        description: Flag indication if builds are enabled
      - in: formData
        name: container_registry_enabled
        description: Flag indication if the container registry is enabled for that
          project
      - in: formData
        name: default_branch
        description: The default branch of the project
      - in: formData
        name: description
        description: The description of the project
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: issues_enabled
        description: Flag indication if the issue tracker is enabled
      - in: formData
        name: lfs_enabled
        description: Flag indication if Git LFS is enabled for that project
      - in: formData
        name: merge_requests_enabled
        description: Flag indication if merge requests are enabled
      - in: formData
        name: name
        description: The name of the project
      - in: formData
        name: only_allow_merge_if_all_discussions_are_resolved
        description: Only allow to merge if all discussions are resolved
      - in: formData
        name: only_allow_merge_if_build_succeeds
        description: Only allow to merge if builds succeed
      - in: formData
        name: path
        description: The path of the repository
      - in: formData
        name: public
        description: Create a public project
      - in: formData
        name: public_builds
        description: Perform public builds
      - in: formData
        name: request_access_enabled
        description: Allow users to request member access
      - in: formData
        name: shared_runners_enabled
        description: Flag indication if shared runners are enabled for that project
      - in: formData
        name: snippets_enabled
        description: Flag indication if snippets are enabled
      - in: formData
        name: visibility_level
        description: Create a public project
      - in: formData
        name: wiki_enabled
        description: Flag indication if the wiki is enabled
      responses:
        200:
          description: OK
      tags:
      - Projects
    delete:
      summary: Delete Projects
      description: Remove a project
      operationId: deleteV3ProjectsId
      x-api-path-slug: v3projectsid-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
  /v3/projects/{id}/events:
    get:
      summary: Get Projects Events
      description: Get events for a single project
      operationId: getV3ProjectsIdEvents
      x-api-path-slug: v3projectsidevents-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Events
  /v3/projects/fork/{id}:
    post:
      summary: Post Projects Fork
      description: Fork new project for the current user or provided namespace.
      operationId: postV3ProjectsForkId
      x-api-path-slug: v3projectsforkid-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: namespace
        description: The ID or name of the namespace that the project will be forked
          into
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Fork
  /v3/projects/{id}/archive:
    post:
      summary: Post Projects Archive
      description: Post projects archive.
      operationId: postV3ProjectsIdArchive
      x-api-path-slug: v3projectsidarchive-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Archive
  /v3/projects/{id}/unarchive:
    post:
      summary: Post Projects Unarchive
      description: Post projects unarchive.
      operationId: postV3ProjectsIdUnarchive
      x-api-path-slug: v3projectsidunarchive-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Unarchive
  /v3/projects/{id}/star:
    post:
      summary: Post Projects Star
      description: Post projects star.
      operationId: postV3ProjectsIdStar
      x-api-path-slug: v3projectsidstar-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Star
    delete:
      summary: Delete Projects Star
      description: Delete projects star.
      operationId: deleteV3ProjectsIdStar
      x-api-path-slug: v3projectsidstar-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Star
  /v3/projects/{id}/fork/{forked_from_id}:
    post:
      summary: Post Projects Fork Forked From
      description: Mark this project as forked from another
      operationId: postV3ProjectsIdForkForkedFromId
      x-api-path-slug: v3projectsidforkforked-from-id-post
      parameters:
      - in: path
        name: forked_from_id
        description: The ID of the project it was forked from
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Fork
      - Forked
      - From
  /v3/projects/{id}/fork:
    delete:
      summary: Delete Projects Fork
      description: Remove a forked_from relationship
      operationId: deleteV3ProjectsIdFork
      x-api-path-slug: v3projectsidfork-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Fork
  /v3/projects/{id}/share:
    post:
      summary: Post Projects Share
      description: Share the project with a group
      operationId: postV3ProjectsIdShare
      x-api-path-slug: v3projectsidshare-post
      parameters:
      - in: formData
        name: expires_at
        description: Share expiration date
      - in: formData
        name: group_access
        description: The group access level
      - in: formData
        name: group_id
        description: The ID of a group
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Share
  /v3/projects/{id}/share/{group_id}:
    delete:
      summary: Delete Projects Share Group
      description: Delete projects share group.
      operationId: deleteV3ProjectsIdShareGroupId
      x-api-path-slug: v3projectsidsharegroup-id-delete
      parameters:
      - in: path
        name: group_id
        description: The ID of the group
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Share
      - Group
  /v3/projects/{id}/uploads:
    post:
      summary: Post Projects Uploads
      description: Post projects uploads.
      operationId: postV3ProjectsIdUploads
      x-api-path-slug: v3projectsiduploads-post
      parameters:
      - in: formData
        name: file
        description: The file to be uploaded
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Uploads
  /v3/projects/{id}/users:
    get:
      summary: Get Projects Users
      description: Get the users list of a project
      operationId: getV3ProjectsIdUsers
      x-api-path-slug: v3projectsidusers-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: search
        description: Return list of users matching the search criteria
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Users
  /v3/projects/{id}/snippets:
    get:
      summary: Get Projects Snippets
      description: Get all project snippets
      operationId: getV3ProjectsIdSnippets
      x-api-path-slug: v3projectsidsnippets-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
    post:
      summary: Post Projects Snippets
      description: Create a new project snippet
      operationId: postV3ProjectsIdSnippets
      x-api-path-slug: v3projectsidsnippets-post
      parameters:
      - in: formData
        name: code
        description: The content of the snippet
      - in: formData
        name: file_name
        description: The file name of the snippet
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: title
        description: The title of the snippet
      - in: formData
        name: visibility_level
        description: The visibility level of the snippet
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
  /v3/projects/{id}/snippets/{snippet_id}:
    get:
      summary: Get Projects Snippets Snippet
      description: Get projects snippets snippet.
      operationId: getV3ProjectsIdSnippetsSnippetId
      x-api-path-slug: v3projectsidsnippetssnippet-id-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: snippet_id
        description: The ID of a project snippet
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Snippet
    put:
      summary: Put Projects Snippets Snippet
      description: Update an existing project snippet
      operationId: putV3ProjectsIdSnippetsSnippetId
      x-api-path-slug: v3projectsidsnippetssnippet-id-put
      parameters:
      - in: formData
        name: code
        description: The content of the snippet
      - in: formData
        name: file_name
        description: The file name of the snippet
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: snippet_id
        description: The ID of a project snippet
      - in: formData
        name: title
        description: The title of the snippet
      - in: formData
        name: visibility_level
        description: The visibility level of the snippet
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Snippet
    delete:
      summary: Delete Projects Snippets Snippet
      description: Delete projects snippets snippet.
      operationId: deleteV3ProjectsIdSnippetsSnippetId
      x-api-path-slug: v3projectsidsnippetssnippet-id-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: snippet_id
        description: The ID of a project snippet
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Snippet
  /v3/projects/{id}/snippets/{snippet_id}/raw:
    get:
      summary: Get Projects Snippets Snippet Raw
      description: Get projects snippets snippet raw.
      operationId: getV3ProjectsIdSnippetsSnippetIdRaw
      x-api-path-slug: v3projectsidsnippetssnippet-idraw-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: snippet_id
        description: The ID of a project snippet
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Snippets
      - Snippet
      - Raw
  /v3/projects/{id}/repository/tree:
    get:
      summary: Get Projects Repository Tree
      description: Get a project repository tree
      operationId: getV3ProjectsIdRepositoryTree
      x-api-path-slug: v3projectsidrepositorytree-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: path
        description: The path of the tree
      - in: query
        name: recursive
        description: Used to get a recursive tree
      - in: query
        name: ref_name
        description: The name of a repository branch or tag, if not given the default
          branch is used
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Tree
  /v3/projects/{id}/repository/blobs/{sha}:
    get:
      summary: Get Projects Repository Blobs Sha
      description: Get projects repository blobs sha.
      operationId: getV3ProjectsIdRepositoryBlobsSha
      x-api-path-slug: v3projectsidrepositoryblobssha-get
      parameters:
      - in: query
        name: filepath
        description: The path to the file to display
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: sha
        description: The commit, branch name, or tag name
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Blobs
      - Sha
  /v3/projects/{id}/repository/commits/{sha}/blob:
    get:
      summary: Get Projects Repository Commits Sha Blob
      description: Get projects repository commits sha blob.
      operationId: getV3ProjectsIdRepositoryCommitsShaBlob
      x-api-path-slug: v3projectsidrepositorycommitsshablob-get
      parameters:
      - in: query
        name: filepath
        description: The path to the file to display
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: sha
        description: The commit, branch name, or tag name
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Commits
      - Sha
      - Blob
  /v3/projects/{id}/repository/raw_blobs/{sha}:
    get:
      summary: Get Projects Repository Raw Blobs Sha
      description: Get projects repository raw blobs sha.
      operationId: getV3ProjectsIdRepositoryRawBlobsSha
      x-api-path-slug: v3projectsidrepositoryraw-blobssha-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: sha
        description: The commit, branch name, or tag name
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Raw
      - Blobs
      - Sha
  /v3/projects/{id}/repository/archive:
    get:
      summary: Get Projects Repository Archive
      description: Get an archive of the repository
      operationId: getV3ProjectsIdRepositoryArchive
      x-api-path-slug: v3projectsidrepositoryarchive-get
      parameters:
      - in: query
        name: format
        description: The archive format
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: sha
        description: The commit sha of the archive to be downloaded
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Archive
  /v3/projects/{id}/repository/compare:
    get:
      summary: Get Projects Repository Compare
      description: Compare two branches, tags, or commits
      operationId: getV3ProjectsIdRepositoryCompare
      x-api-path-slug: v3projectsidrepositorycompare-get
      parameters:
      - in: query
        name: from
        description: The commit, branch name, or tag name to start comparison
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: to
        description: The commit, branch name, or tag name to stop comparison
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Compare
  /v3/projects/{id}/repository/contributors:
    get:
      summary: Get Projects Repository Contributors
      description: Get projects repository contributors.
      operationId: getV3ProjectsIdRepositoryContributors
      x-api-path-slug: v3projectsidrepositorycontributors-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Contributors
  /v3/projects/{id}/runners:
    get:
      summary: Get Projects Runners
      description: Get runners available for project
      operationId: getV3ProjectsIdRunners
      x-api-path-slug: v3projectsidrunners-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: scope
        description: The scope of specific runners to show
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Runners
    post:
      summary: Post Projects Runners
      description: Enable a runner for a project
      operationId: postV3ProjectsIdRunners
      x-api-path-slug: v3projectsidrunners-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: runner_id
        description: The ID of the runner
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Runners
  /v3/projects/{id}/runners/{runner_id}:
    delete:
      summary: Delete Projects Runners Runner
      description: Delete projects runners runner.
      operationId: deleteV3ProjectsIdRunnersRunnerId
      x-api-path-slug: v3projectsidrunnersrunner-id-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: runner_id
        description: The ID of the runner
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Runners
      - Runner
  /v3/projects/{id}/services/asana:
    put:
      summary: Put Projects Services Asana
      description: Set asana service for project
      operationId: putV3ProjectsIdServicesAsana
      x-api-path-slug: v3projectsidservicesasana-put
      parameters:
      - in: formData
        name: api_key
        description: User API token
      - in: path
        name: id
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: restrict_to_branch
        description: Comma-separated list of branches which will be automatically
          inspected
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Asana
  /v3/projects/{id}/services/assembla:
    put:
      summary: Put Projects Services Assembla
      description: Set assembla service for project
      operationId: putV3ProjectsIdServicesAssembla
      x-api-path-slug: v3projectsidservicesassembla-put
      parameters:
      - in: path
        name: id
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: subdomain
        description: Subdomain setting
      - in: formData
        name: token
        description: The authentication token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Assembla
  /v3/projects/{id}/services/bamboo:
    put:
      summary: Put Projects Services Bamboo
      description: Set bamboo service for project
      operationId: putV3ProjectsIdServicesBamboo
      x-api-path-slug: v3projectsidservicesbamboo-put
      parameters:
      - in: formData
        name: bamboo_url
        description: Bamboo root URL like https://bamboo
      - in: formData
        name: build_key
        description: Bamboo build plan key like
      - in: path
        name: id
      - in: formData
        name: password
        description: Passord of the user
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: username
        description: A user with API access, if applicable
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Bamboo
  /v3/projects/{id}/services/bugzilla:
    put:
      summary: Put Projects Services Bugzilla
      description: Set bugzilla service for project
      operationId: putV3ProjectsIdServicesBugzilla
      x-api-path-slug: v3projectsidservicesbugzilla-put
      parameters:
      - in: formData
        name: description
        description: Description
      - in: path
        name: id
      - in: formData
        name: issues_url
        description: Issues URL
      - in: formData
        name: new_issue_url
        description: New issue URL
      - in: formData
        name: project_url
        description: Project URL
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: title
        description: Title
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Bugzilla
  /v3/projects/{id}/services/buildkite:
    put:
      summary: Put Projects Services Buildkite
      description: Set buildkite service for project
      operationId: putV3ProjectsIdServicesBuildkite
      x-api-path-slug: v3projectsidservicesbuildkite-put
      parameters:
      - in: formData
        name: enable_ssl_verification
        description: Enable SSL verification for communication
      - in: path
        name: id
      - in: formData
        name: project_url
        description: The buildkite project URL
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: token
        description: Buildkite project GitLab token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Buildkite
  /v3/projects/{id}/services/builds-email:
    put:
      summary: Put Projects Services Builds Email
      description: Set builds-email service for project
      operationId: putV3ProjectsIdServicesBuildsEmail
      x-api-path-slug: v3projectsidservicesbuildsemail-put
      parameters:
      - in: formData
        name: add_pusher
        description: Add pusher to recipients list
      - in: formData
        name: build_events
        description: Event will be triggered when a build status changes
      - in: path
        name: id
      - in: formData
        name: notify_only_broken_builds
        description: Notify only broken builds
      - in: formData
        name: recipients
        description: Comma-separated list of recipient email addresses
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Builds
      - Email
  /v3/projects/{id}/services/campfire:
    put:
      summary: Put Projects Services Campfire
      description: Set campfire service for project
      operationId: putV3ProjectsIdServicesCampfire
      x-api-path-slug: v3projectsidservicescampfire-put
      parameters:
      - in: path
        name: id
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: room
        description: Campfire room
      - in: formData
        name: subdomain
        description: Campfire subdomain
      - in: formData
        name: token
        description: Campfire token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Campfire
  /v3/projects/{id}/services/custom-issue-tracker:
    put:
      summary: Put Projects Services Custom Issue Tracker
      description: Set custom-issue-tracker service for project
      operationId: putV3ProjectsIdServicesCustomIssueTracker
      x-api-path-slug: v3projectsidservicescustomissuetracker-put
      parameters:
      - in: formData
        name: description
        description: Description
      - in: path
        name: id
      - in: formData
        name: issues_url
        description: Issues URL
      - in: formData
        name: new_issue_url
        description: New issue URL
      - in: formData
        name: project_url
        description: Project URL
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: title
        description: Title
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Custom
      - Issue
      - Tracker
  /v3/projects/{id}/services/drone-ci:
    put:
      summary: Put Projects Services Drone Ci
      description: Set drone-ci service for project
      operationId: putV3ProjectsIdServicesDroneCi
      x-api-path-slug: v3projectsidservicesdroneci-put
      parameters:
      - in: formData
        name: drone_url
        description: Drone CI URL
      - in: formData
        name: enable_ssl_verification
        description: Enable SSL verification for communication
      - in: path
        name: id
      - in: formData
        name: merge_request_events
        description: Event will be triggered when a merge request is created/updated/merged
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: tag_push_events
        description: Event will be triggered when a new tag is pushed to the repository
      - in: formData
        name: token
        description: Drone CI token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Drone
      - Ci
  /v3/projects/{id}/services/emails-on-push:
    put:
      summary: Put Projects Services Emails On Push
      description: Set emails-on-push service for project
      operationId: putV3ProjectsIdServicesEmailsOnPush
      x-api-path-slug: v3projectsidservicesemailsonpush-put
      parameters:
      - in: formData
        name: disable_diffs
        description: Disable code diffs
      - in: path
        name: id
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: recipients
        description: Comma-separated list of recipient email addresses
      - in: formData
        name: send_from_committer_email
        description: Send from committer
      - in: formData
        name: tag_push_events
        description: Event will be triggered when a new tag is pushed to the repository
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Emails
      - "On"
      - Push
  /v3/projects/{id}/services/external-wiki:
    put:
      summary: Put Projects Services External Wiki
      description: Set external-wiki service for project
      operationId: putV3ProjectsIdServicesExternalWiki
      x-api-path-slug: v3projectsidservicesexternalwiki-put
      parameters:
      - in: formData
        name: external_wiki_url
        description: The URL of the external Wiki
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - External
      - Wiki
  /v3/projects/{id}/services/flowdock:
    put:
      summary: Put Projects Services Flowdock
      description: Set flowdock service for project
      operationId: putV3ProjectsIdServicesFlowdock
      x-api-path-slug: v3projectsidservicesflowdock-put
      parameters:
      - in: path
        name: id
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: token
        description: Flowdock token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Flowdock
  /v3/projects/{id}/services/gemnasium:
    put:
      summary: Put Projects Services Gemnasium
      description: Set gemnasium service for project
      operationId: putV3ProjectsIdServicesGemnasium
      x-api-path-slug: v3projectsidservicesgemnasium-put
      parameters:
      - in: formData
        name: api_key
        description: Your personal API key on gemnasium
      - in: path
        name: id
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: token
        description: The projects slug on gemnasium
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Gemnasium
  /v3/projects/{id}/services/hipchat:
    put:
      summary: Put Projects Services Hipchat
      description: Set hipchat service for project
      operationId: putV3ProjectsIdServicesHipchat
      x-api-path-slug: v3projectsidserviceshipchat-put
      parameters:
      - in: formData
        name: api_version
        description: Leave blank for default (v2)
      - in: formData
        name: build_events
        description: Event will be triggered when a build status changes
      - in: formData
        name: color
        description: The room color
      - in: formData
        name: confidential_issue_events
        description: Event will be triggered when a confidential issue is created/updated/closed
      - in: path
        name: id
      - in: formData
        name: issue_events
        description: Event will be triggered when an issue is created/updated/closed
      - in: formData
        name: merge_request_events
        description: Event will be triggered when a merge request is created/updated/merged
      - in: formData
        name: note_events
        description: Event will be triggered when someone adds a comment
      - in: formData
        name: notify
        description: Enable notifications
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: room
        description: The room name or ID
      - in: formData
        name: server
        description: Leave blank for default
      - in: formData
        name: tag_push_events
        description: Event will be triggered when a new tag is pushed to the repository
      - in: formData
        name: token
        description: The room token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Hipchat
  /v3/projects/{id}/services/irker:
    put:
      summary: Put Projects Services Irker
      description: Set irker service for project
      operationId: putV3ProjectsIdServicesIrker
      x-api-path-slug: v3projectsidservicesirker-put
      parameters:
      - in: formData
        name: colorize_messages
        description: Colorize messages
      - in: formData
        name: default_irc_uri
        description: 'Default: irc://irc'
      - in: path
        name: id
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: recipients
        description: Recipients/channels separated by whitespaces
      - in: formData
        name: server_host
        description: Server host
      - in: formData
        name: server_port
        description: Server port
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Irker
  /v3/projects/{id}/services/jira:
    put:
      summary: Put Projects Services Jira
      description: Set jira service for project
      operationId: putV3ProjectsIdServicesJira
      x-api-path-slug: v3projectsidservicesjira-put
      parameters:
      - in: formData
        name: commit_events
        description: Event will be triggered when a commit is created/updated
      - in: path
        name: id
      - in: formData
        name: jira_issue_transition_id
        description: The ID of a transition that moves issues to a closed state
      - in: formData
        name: merge_request_events
        description: Event will be triggered when a merge request is created/updated/merged
      - in: formData
        name: password
        description: The password of the user created to be used with GitLab/JIRA
      - in: formData
        name: project_key
        description: The short identifier for your JIRA project, all uppercase, e
      - in: formData
        name: url
        description: The URL to the JIRA project which is being linked to this GitLab
          project, e
      - in: formData
        name: username
        description: The username of the user created to be used with GitLab/JIRA
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Jira
  /v3/projects/{id}/services/kubernetes:
    put:
      summary: Put Projects Services Kubernetes
      description: Set kubernetes service for project
      operationId: putV3ProjectsIdServicesKubernetes
      x-api-path-slug: v3projectsidserviceskubernetes-put
      parameters:
      - in: formData
        name: api_url
        description: The URL to the Kubernetes cluster API, e
      - in: formData
        name: ca_pem
        description: A custom certificate authority bundle to verify the Kubernetes
          cluster with (PEM format)
      - in: path
        name: id
      - in: formData
        name: namespace
        description: The Kubernetes namespace to use
      - in: formData
        name: token
        description: The service token to authenticate against the Kubernetes cluster
          with
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Kubernetes
  /v3/projects/{id}/services/mattermost-slash-commands:
    put:
      summary: Put Projects Services Mattermost Slash Commands
      description: Set mattermost-slash-commands service for project
      operationId: putV3ProjectsIdServicesMattermostSlashCommands
      x-api-path-slug: v3projectsidservicesmattermostslashcommands-put
      parameters:
      - in: path
        name: id
      - in: formData
        name: token
        description: The Mattermost token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Mattermost
      - Slash
      - Commands
  /v3/projects/{id}/services/slack-slash-commands:
    put:
      summary: Put Projects Services Slack Slash Commands
      description: Set slack-slash-commands service for project
      operationId: putV3ProjectsIdServicesSlackSlashCommands
      x-api-path-slug: v3projectsidservicesslackslashcommands-put
      parameters:
      - in: path
        name: id
      - in: formData
        name: token
        description: The Slack token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Slack
      - Slash
      - Commands
  /v3/projects/{id}/services/pipelines-email:
    put:
      summary: Put Projects Services Pipelines Email
      description: Set pipelines-email service for project
      operationId: putV3ProjectsIdServicesPipelinesEmail
      x-api-path-slug: v3projectsidservicespipelinesemail-put
      parameters:
      - in: path
        name: id
      - in: formData
        name: notify_only_broken_builds
        description: Notify only broken builds
      - in: formData
        name: pipeline_events
      - in: formData
        name: recipients
        description: Comma-separated list of recipient email addresses
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Pipelines
      - Email
  /v3/projects/{id}/services/pivotaltracker:
    put:
      summary: Put Projects Services Pivotaltracker
      description: Set pivotaltracker service for project
      operationId: putV3ProjectsIdServicesPivotaltracker
      x-api-path-slug: v3projectsidservicespivotaltracker-put
      parameters:
      - in: path
        name: id
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: restrict_to_branch
        description: Comma-separated list of branches which will be automatically
          inspected
      - in: formData
        name: token
        description: The Pivotaltracker token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Pivotaltracker
  /v3/projects/{id}/services/pushover:
    put:
      summary: Put Projects Services Pushover
      description: Set pushover service for project
      operationId: putV3ProjectsIdServicesPushover
      x-api-path-slug: v3projectsidservicespushover-put
      parameters:
      - in: formData
        name: api_key
        description: The application key
      - in: formData
        name: device
        description: Leave blank for all active devices
      - in: path
        name: id
      - in: formData
        name: priority
        description: The priority
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: sound
        description: The sound of the notification
      - in: formData
        name: user_key
        description: The user key
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Pushover
  /v3/projects/{id}/services/redmine:
    put:
      summary: Put Projects Services Redmine
      description: Set redmine service for project
      operationId: putV3ProjectsIdServicesRedmine
      x-api-path-slug: v3projectsidservicesredmine-put
      parameters:
      - in: formData
        name: description
        description: The description of the tracker
      - in: path
        name: id
      - in: formData
        name: issues_url
        description: The issues URL
      - in: formData
        name: new_issue_url
        description: The new issue URL
      - in: formData
        name: project_url
        description: The project URL
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Redmine
  /v3/projects/{id}/services/slack:
    put:
      summary: Put Projects Services Slack
      description: Set slack service for project
      operationId: putV3ProjectsIdServicesSlack
      x-api-path-slug: v3projectsidservicesslack-put
      parameters:
      - in: formData
        name: build_events
        description: Event will be triggered when a build status changes
      - in: formData
        name: channel
        description: The channel name
      - in: formData
        name: confidential_issue_events
        description: Event will be triggered when a confidential issue is created/updated/closed
      - in: path
        name: id
      - in: formData
        name: issue_events
        description: Event will be triggered when an issue is created/updated/closed
      - in: formData
        name: merge_request_events
        description: Event will be triggered when a merge request is created/updated/merged
      - in: formData
        name: new_issue_url
        description: The user name
      - in: formData
        name: note_events
        description: Event will be triggered when someone adds a comment
      - in: formData
        name: pipeline_events
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: tag_push_events
        description: Event will be triggered when a new tag is pushed to the repository
      - in: formData
        name: webhook
        description: The Slack webhook
      - in: formData
        name: wiki_page_events
        description: Event will be triggered when a wiki page is created/updated
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Slack
  /v3/projects/{id}/services/mattermost:
    put:
      summary: Put Projects Services Mattermost
      description: Set mattermost service for project
      operationId: putV3ProjectsIdServicesMattermost
      x-api-path-slug: v3projectsidservicesmattermost-put
      parameters:
      - in: formData
        name: build_events
        description: Event will be triggered when a build status changes
      - in: formData
        name: confidential_issue_events
        description: Event will be triggered when a confidential issue is created/updated/closed
      - in: path
        name: id
      - in: formData
        name: issue_events
        description: Event will be triggered when an issue is created/updated/closed
      - in: formData
        name: merge_request_events
        description: Event will be triggered when a merge request is created/updated/merged
      - in: formData
        name: note_events
        description: Event will be triggered when someone adds a comment
      - in: formData
        name: pipeline_events
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: tag_push_events
        description: Event will be triggered when a new tag is pushed to the repository
      - in: formData
        name: webhook
        description: The Mattermost webhook
      - in: formData
        name: wiki_page_events
        description: Event will be triggered when a wiki page is created/updated
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Mattermost
  /v3/projects/{id}/services/teamcity:
    put:
      summary: Put Projects Services Teamcity
      description: Set teamcity service for project
      operationId: putV3ProjectsIdServicesTeamcity
      x-api-path-slug: v3projectsidservicesteamcity-put
      parameters:
      - in: formData
        name: build_type
        description: Build configuration ID
      - in: path
        name: id
      - in: formData
        name: password
        description: The password of the user
      - in: formData
        name: push_events
        description: Event will be triggered by a push to the repository
      - in: formData
        name: teamcity_url
        description: TeamCity root URL like https://teamcity
      - in: formData
        name: username
        description: A user with permissions to trigger a manual build
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Teamcity
  /v3/projects/{id}/services/{service_slug}:
    delete:
      summary: Delete Projects Services Service Slug
      description: Delete projects services service slug.
      operationId: deleteV3ProjectsIdServicesServiceSlug
      x-api-path-slug: v3projectsidservicesservice-slug-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: service_slug
        description: The name of the service
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Service
      - Slug
    get:
      summary: Get Projects Services Service Slug
      description: Get the service settings for project
      operationId: getV3ProjectsIdServicesServiceSlug
      x-api-path-slug: v3projectsidservicesservice-slug-get
      parameters:
      - in: path
        name: id
      - in: path
        name: service_slug
        description: The name of the service
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Service
      - Slug
  /v3/projects/{id}/services/mattermost_slash_commands/trigger:
    post:
      summary: Post Projects Services Mattermost Slash Commands Trigger
      description: Post projects services mattermost slash commands trigger.
      operationId: postV3ProjectsIdServicesMattermostSlashCommandsTrigger
      x-api-path-slug: v3projectsidservicesmattermost-slash-commandstrigger-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: token
        description: The Mattermost token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Mattermost
      - Slash
      - Commands
      - Trigger
  /v3/projects/{id}/services/slack_slash_commands/trigger:
    post:
      summary: Post Projects Services Slack Slash Commands Trigger
      description: Post projects services slack slash commands trigger.
      operationId: postV3ProjectsIdServicesSlackSlashCommandsTrigger
      x-api-path-slug: v3projectsidservicesslack-slash-commandstrigger-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: token
        description: The Slack token
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Slack
      - Slash
      - Commands
      - Trigger
  /v3/projects/{id}/merge_request/{subscribable_id}/subscription:
    post:
      summary: Post Projects Merge Request Subscribable Subscription
      description: Post projects merge request subscribable subscription.
      operationId: postV3ProjectsIdMergeRequestSubscribableIdSubscription
      x-api-path-slug: v3projectsidmerge-requestsubscribable-idsubscription-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Subscribable
      - Subscription
    delete:
      summary: Delete Projects Merge Request Subscribable Subscription
      description: Delete projects merge request subscribable subscription.
      operationId: deleteV3ProjectsIdMergeRequestSubscribableIdSubscription
      x-api-path-slug: v3projectsidmerge-requestsubscribable-idsubscription-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Subscribable
      - Subscription
  /v3/projects/{id}/merge_requests/{subscribable_id}/subscription:
    post:
      summary: Post Projects Merge Requests Subscribable Subscription
      description: Post projects merge requests subscribable subscription.
      operationId: postV3ProjectsIdMergeRequestsSubscribableIdSubscription
      x-api-path-slug: v3projectsidmerge-requestssubscribable-idsubscription-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Subscribable
      - Subscription
    delete:
      summary: Delete Projects Merge Requests Subscribable Subscription
      description: Delete projects merge requests subscribable subscription.
      operationId: deleteV3ProjectsIdMergeRequestsSubscribableIdSubscription
      x-api-path-slug: v3projectsidmerge-requestssubscribable-idsubscription-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Subscribable
      - Subscription
  /v3/projects/{id}/issues/{subscribable_id}/subscription:
    post:
      summary: Post Projects Issues Subscribable Subscription
      description: Post projects issues subscribable subscription.
      operationId: postV3ProjectsIdIssuesSubscribableIdSubscription
      x-api-path-slug: v3projectsidissuessubscribable-idsubscription-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Subscribable
      - Subscription
    delete:
      summary: Delete Projects Issues Subscribable Subscription
      description: Delete projects issues subscribable subscription.
      operationId: deleteV3ProjectsIdIssuesSubscribableIdSubscription
      x-api-path-slug: v3projectsidissuessubscribable-idsubscription-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Subscribable
      - Subscription
  /v3/projects/{id}/labels/{subscribable_id}/subscription:
    post:
      summary: Post Projects Labels Subscribable Subscription
      description: Post projects labels subscribable subscription.
      operationId: postV3ProjectsIdLabelsSubscribableIdSubscription
      x-api-path-slug: v3projectsidlabelssubscribable-idsubscription-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Labels
      - Subscribable
      - Subscription
    delete:
      summary: Delete Projects Labels Subscribable Subscription
      description: Delete projects labels subscribable subscription.
      operationId: deleteV3ProjectsIdLabelsSubscribableIdSubscription
      x-api-path-slug: v3projectsidlabelssubscribable-idsubscription-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: subscribable_id
        description: The ID of a resource
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Labels
      - Subscribable
      - Subscription
  /v3/projects/{id}/repository/tags:
    get:
      summary: Get Projects Repository Tags
      description: Get a project repository tags
      operationId: getV3ProjectsIdRepositoryTags
      x-api-path-slug: v3projectsidrepositorytags-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Tags
    post:
      summary: Post Projects Repository Tags
      description: Post projects repository tags.
      operationId: postV3ProjectsIdRepositoryTags
      x-api-path-slug: v3projectsidrepositorytags-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: message
        description: Specifying a message creates an annotated tag
      - in: formData
        name: ref
        description: The commit sha or branch name
      - in: formData
        name: release_description
        description: Specifying release notes stored in the GitLab database
      - in: formData
        name: tag_name
        description: The name of the tag
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Tags
  /v3/projects/{id}/repository/tags/{tag_name}:
    get:
      summary: Get Projects Repository Tags Tag Name
      description: Get projects repository tags tag name.
      operationId: getV3ProjectsIdRepositoryTagsTagName
      x-api-path-slug: v3projectsidrepositorytagstag-name-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: tag_name
        description: The name of the tag
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Tags
      - Tag
      - Name
    delete:
      summary: Delete Projects Repository Tags Tag Name
      description: Delete projects repository tags tag name.
      operationId: deleteV3ProjectsIdRepositoryTagsTagName
      x-api-path-slug: v3projectsidrepositorytagstag-name-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: tag_name
        description: The name of the tag
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Tags
      - Tag
      - Name
  /v3/projects/{id}/repository/tags/{tag_name}/release:
    post:
      summary: Post Projects Repository Tags Tag Name Release
      description: Post projects repository tags tag name release.
      operationId: postV3ProjectsIdRepositoryTagsTagNameRelease
      x-api-path-slug: v3projectsidrepositorytagstag-namerelease-post
      parameters:
      - in: formData
        name: description
        description: Release notes with markdown support
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: tag_name
        description: The name of the tag
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Tags
      - Tag
      - Name
      - Release
    put:
      summary: Put Projects Repository Tags Tag Name Release
      description: Put projects repository tags tag name release.
      operationId: putV3ProjectsIdRepositoryTagsTagNameRelease
      x-api-path-slug: v3projectsidrepositorytagstag-namerelease-put
      parameters:
      - in: formData
        name: description
        description: Release notes with markdown support
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: tag_name
        description: The name of the tag
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Tags
      - Tag
      - Name
      - Release
  /v3/projects/{id}/merge_requests/{merge_request_id}/todo:
    post:
      summary: Post Projects Merge Requests Merge Request Todo
      description: Post projects merge requests merge request todo.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdTodo
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idtodo-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of an issuable
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Todo
  /v3/projects/{id}/issues/{issue_id}/todo:
    post:
      summary: Post Projects Issues Issue Todo
      description: Post projects issues issue todo.
      operationId: postV3ProjectsIdIssuesIssueIdTodo
      x-api-path-slug: v3projectsidissuesissue-idtodo-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: issue_id
        description: The ID of an issuable
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Todo
  /v3/projects/{id}/(ref/{ref}/)trigger/builds:
    post:
      summary: Post Projects (ref Ref )trigger Builds
      description: Post projects (ref ref )trigger builds.
      operationId: postV3ProjectsId(refRef)triggerBuilds
      x-api-path-slug: v3projectsidrefreftriggerbuilds-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: ref
        description: The commit sha or name of a branch or tag
      - in: formData
        name: token
        description: The unique token of trigger
      responses:
        200:
          description: OK
      tags:
      - Projects
      - (ref
      - Ref
      - )trigger
      - Builds
  /v3/projects/{id}/triggers:
    get:
      summary: Get Projects Triggers
      description: Get projects triggers.
      operationId: getV3ProjectsIdTriggers
      x-api-path-slug: v3projectsidtriggers-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Triggers
    post:
      summary: Post Projects Triggers
      description: Post projects triggers.
      operationId: postV3ProjectsIdTriggers
      x-api-path-slug: v3projectsidtriggers-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Triggers
  /v3/projects/{id}/triggers/{token}:
    get:
      summary: Get Projects Triggers Token
      description: Get specific trigger of a project
      operationId: getV3ProjectsIdTriggersToken
      x-api-path-slug: v3projectsidtriggerstoken-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: token
        description: The unique token of trigger
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Triggers
      - Token
    delete:
      summary: Delete Projects Triggers Token
      description: Delete projects triggers token.
      operationId: deleteV3ProjectsIdTriggersToken
      x-api-path-slug: v3projectsidtriggerstoken-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: token
        description: The unique token of trigger
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Triggers
      - Token
  /v3/projects/{id}/variables:
    get:
      summary: Get Projects Variables
      description: Get projects variables.
      operationId: getV3ProjectsIdVariables
      x-api-path-slug: v3projectsidvariables-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Variables
    post:
      summary: Post Projects Variables
      description: Create a new variable in a project
      operationId: postV3ProjectsIdVariables
      x-api-path-slug: v3projectsidvariables-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: key
        description: The key of the variable
      - in: formData
        name: value
        description: The value of the variable
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Variables
  /v3/projects/{id}/variables/{key}:
    get:
      summary: Get Projects Variables Key
      description: Get a specific variable from a project
      operationId: getV3ProjectsIdVariablesKey
      x-api-path-slug: v3projectsidvariableskey-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: key
        description: The key of the variable
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Variables
      - Key
    put:
      summary: Put Projects Variables Key
      description: Update an existing variable from a project
      operationId: putV3ProjectsIdVariablesKey
      x-api-path-slug: v3projectsidvariableskey-put
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: key
        description: The key of the variable
      - in: formData
        name: value
        description: The value of the variable
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Variables
      - Key
    delete:
      summary: Delete Projects Variables Key
      description: Delete an existing variable from a project
      operationId: deleteV3ProjectsIdVariablesKey
      x-api-path-slug: v3projectsidvariableskey-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: key
        description: The key of the variable
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Variables
      - Key
  /v3/projects/{id}/boards/{board_id}/lists:
    get:
      summary: Get Projects Boards Board Lists
      description: Does not include `backlog` and `done` lists. This feature was introduced
        in 8.13
      operationId: getV3ProjectsIdBoardsBoardIdLists
      x-api-path-slug: v3projectsidboardsboard-idlists-get
      parameters:
      - in: path
        name: board_id
        description: The ID of a board
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Boards
      - Board
      - Lists
    post:
      summary: Post Projects Boards Board Lists
      description: This feature was introduced in 8.13
      operationId: postV3ProjectsIdBoardsBoardIdLists
      x-api-path-slug: v3projectsidboardsboard-idlists-post
      parameters:
      - in: path
        name: board_id
        description: The ID of a board
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: label_id
        description: The ID of an existing label
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Boards
      - Board
      - Lists
  /v3/projects/{id}/boards/{board_id}/lists/{list_id}:
    get:
      summary: Get Projects Boards Board Lists List
      description: Get projects boards board lists list.
      operationId: getV3ProjectsIdBoardsBoardIdListsListId
      x-api-path-slug: v3projectsidboardsboard-idlistslist-id-get
      parameters:
      - in: path
        name: board_id
        description: The ID of a board
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: list_id
        description: The ID of a list
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Boards
      - Board
      - Lists
      - List
    put:
      summary: Put Projects Boards Board Lists List
      description: Put projects boards board lists list.
      operationId: putV3ProjectsIdBoardsBoardIdListsListId
      x-api-path-slug: v3projectsidboardsboard-idlistslist-id-put
      parameters:
      - in: path
        name: board_id
        description: The ID of a board
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: list_id
        description: The ID of a list
      - in: formData
        name: position
        description: The position of the list
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Boards
      - Board
      - Lists
      - List
    delete:
      summary: Delete Projects Boards Board Lists List
      description: Delete projects boards board lists list.
      operationId: deleteV3ProjectsIdBoardsBoardIdListsListId
      x-api-path-slug: v3projectsidboardsboard-idlistslist-id-delete
      parameters:
      - in: path
        name: board_id
        description: The ID of a board
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: list_id
        description: The ID of a board list
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Boards
      - Board
      - Lists
      - List
  /v3/internal/allowed:
    post:
      summary: Post Internal Allowed
      description: Post internal allowed.
      operationId: postV3InternalAllowed
      x-api-path-slug: v3internalallowed-post
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Owed
  /v3/internal/lfs_authenticate:
    post:
      summary: Post Internal Lfs Authenticate
      description: Post internal lfs authenticate.
      operationId: postV3InternalLfsAuthenticate
      x-api-path-slug: v3internallfs-authenticate-post
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Lfs
      - Authenticate
  /v3/internal/merge_request_urls:
    get:
      summary: Get Internal Merge Request Urls
      description: Get internal merge request urls.
      operationId: getV3InternalMergeRequestUrls
      x-api-path-slug: v3internalmerge-request-urls-get
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Merge
      - Request
      - Urls
  /v3/internal/discover:
    get:
      summary: Get Internal Discover
      description: Get internal discover.
      operationId: getV3InternalDiscover
      x-api-path-slug: v3internaldiscover-get
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Discover
  /v3/internal/check:
    get:
      summary: Get Internal Check
      description: Get internal check.
      operationId: getV3InternalCheck
      x-api-path-slug: v3internalcheck-get
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Check
  /v3/internal/broadcast_message:
    get:
      summary: Get Internal Broadcast Message
      description: Get internal broadcast message.
      operationId: getV3InternalBroadcastMessage
      x-api-path-slug: v3internalbroadcast-message-get
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Broadcast
      - Message
  /v3/internal/two_factor_recovery_codes:
    post:
      summary: Post Internal Two Factor Recovery Codes
      description: Post internal two factor recovery codes.
      operationId: postV3InternalTwoFactorRecoveryCodes
      x-api-path-slug: v3internaltwo-factor-recovery-codes-post
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Two
      - Factor
      - Recovery
      - Codes
  /v3/issues:
    get:
      summary: Get Issues
      description: Get currently authenticated user's issues
      operationId: getV3Issues
      x-api-path-slug: v3issues-get
      parameters:
      - in: query
        name: labels
        description: Comma-separated list of label names
      - in: query
        name: milestone
        description: Return issues for a specific milestone
      - in: query
        name: order_by
        description: Return issues ordered by `created_at` or `updated_at` fields
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: sort
        description: Return issues sorted in `asc` or `desc` order
      - in: query
        name: state
        description: Return opened, closed, or all issues
      responses:
        200:
          description: OK
      tags:
      - Issues
  /v3/keys/{id}:
    get:
      summary: Get Keys
      description: Get single ssh key by id. Only available to admin users
      operationId: getV3KeysId
      x-api-path-slug: v3keysid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Keys
  /v3/ci/lint:
    post:
      summary: Post Ci Lint
      description: Validation of .gitlab-ci.yml content
      operationId: postV3CiLint
      x-api-path-slug: v3cilint-post
      parameters:
      - in: formData
        name: content
        description: 'Content of '
      responses:
        200:
          description: OK
      tags:
      - Ci
      - Lint
  /v3/namespaces:
    get:
      summary: Get Namespaces
      description: Get a namespaces list
      operationId: getV3Namespaces
      x-api-path-slug: v3namespaces-get
      parameters:
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: search
        description: Search query for namespaces
      responses:
        200:
          description: OK
      tags:
      - Namespaces
  /v3/notification_settings:
    get:
      summary: Get Notification Settings
      description: This feature was introduced in GitLab 8.12
      operationId: getV3NotificationSettings
      x-api-path-slug: v3notification-settings-get
      responses:
        200:
          description: OK
      tags:
      - Notification
      - Settings
    put:
      summary: Put Notification Settings
      description: This feature was introduced in GitLab 8.12
      operationId: putV3NotificationSettings
      x-api-path-slug: v3notification-settings-put
      parameters:
      - in: formData
        name: close_issue
        description: Enable/disable this notification
      - in: formData
        name: close_merge_request
        description: Enable/disable this notification
      - in: formData
        name: failed_pipeline
        description: Enable/disable this notification
      - in: formData
        name: level
        description: The global notification level
      - in: formData
        name: merge_merge_request
        description: Enable/disable this notification
      - in: formData
        name: new_issue
        description: Enable/disable this notification
      - in: formData
        name: new_merge_request
        description: Enable/disable this notification
      - in: formData
        name: new_note
        description: Enable/disable this notification
      - in: formData
        name: notification_email
        description: The email address to send notifications
      - in: formData
        name: reassign_issue
        description: Enable/disable this notification
      - in: formData
        name: reassign_merge_request
        description: Enable/disable this notification
      - in: formData
        name: reopen_issue
        description: Enable/disable this notification
      - in: formData
        name: reopen_merge_request
        description: Enable/disable this notification
      - in: formData
        name: success_pipeline
        description: Enable/disable this notification
      responses:
        200:
          description: OK
      tags:
      - Notification
      - Settings
  /v3/runners:
    get:
      summary: Get Runners
      description: Get runners available for user
      operationId: getV3Runners
      x-api-path-slug: v3runners-get
      parameters:
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: scope
        description: The scope of specific runners to show
      responses:
        200:
          description: OK
      tags:
      - Runners
  /v3/runners/all:
    get:
      summary: Get Runners All
      description: Get all runners - shared and specific
      operationId: getV3RunnersAll
      x-api-path-slug: v3runnersall-get
      parameters:
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: scope
        description: The scope of specific runners to show
      responses:
        200:
          description: OK
      tags:
      - Runners
  /v3/runners/{id}:
    get:
      summary: Get Runners
      description: Get runner's details
      operationId: getV3RunnersId
      x-api-path-slug: v3runnersid-get
      parameters:
      - in: path
        name: id
        description: The ID of the runner
      responses:
        200:
          description: OK
      tags:
      - Runners
    put:
      summary: Put Runners
      description: Update runner's details
      operationId: putV3RunnersId
      x-api-path-slug: v3runnersid-put
      parameters:
      - in: formData
        name: active
        description: The state of a runner
      - in: formData
        name: description
        description: The description of the runner
      - in: path
        name: id
        description: The ID of the runner
      - in: formData
        name: locked
        description: Flag indicating the runner is locked
      - in: formData
        name: run_untagged
        description: Flag indicating the runner can execute untagged jobs
      - in: formData
        name: tag_list
        description: The list of tags for a runner
      responses:
        200:
          description: OK
      tags:
      - Runners
    delete:
      summary: Delete Runners
      description: Remove a runner
      operationId: deleteV3RunnersId
      x-api-path-slug: v3runnersid-delete
      parameters:
      - in: path
        name: id
        description: The ID of the runner
      responses:
        200:
          description: OK
      tags:
      - Runners
  /v3/snippets:
    get:
      summary: Get Snippets
      description: This feature was introduced in GitLab 8.15.
      operationId: getV3Snippets
      x-api-path-slug: v3snippets-get
      parameters:
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Snippets
    post:
      summary: Post Snippets
      description: This feature was introduced in GitLab 8.15.
      operationId: postV3Snippets
      x-api-path-slug: v3snippets-post
      parameters:
      - in: formData
        name: content
        description: The content of a snippet
      - in: formData
        name: file_name
        description: The name of a snippet file
      - in: formData
        name: title
        description: The title of a snippet
      - in: formData
        name: visibility_level
        description: The visibility level of the snippet
      responses:
        200:
          description: OK
      tags:
      - Snippets
  /v3/snippets/public:
    get:
      summary: Get Snippets Public
      description: This feature was introduced in GitLab 8.15.
      operationId: getV3SnippetsPublic
      x-api-path-slug: v3snippetspublic-get
      parameters:
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Public
  /v3/snippets/{id}:
    get:
      summary: Get Snippets
      description: This feature was introduced in GitLab 8.15.
      operationId: getV3SnippetsId
      x-api-path-slug: v3snippetsid-get
      parameters:
      - in: path
        name: id
        description: The ID of a snippet
      responses:
        200:
          description: OK
      tags:
      - Snippets
    put:
      summary: Put Snippets
      description: This feature was introduced in GitLab 8.15.
      operationId: putV3SnippetsId
      x-api-path-slug: v3snippetsid-put
      parameters:
      - in: formData
        name: content
        description: The content of a snippet
      - in: formData
        name: file_name
        description: The name of a snippet file
      - in: path
        name: id
        description: The ID of a snippet
      - in: formData
        name: title
        description: The title of a snippet
      - in: formData
        name: visibility_level
        description: The visibility level of the snippet
      responses:
        200:
          description: OK
      tags:
      - Snippets
    delete:
      summary: Delete Snippets
      description: This feature was introduced in GitLab 8.15.
      operationId: deleteV3SnippetsId
      x-api-path-slug: v3snippetsid-delete
      parameters:
      - in: path
        name: id
        description: The ID of a snippet
      responses:
        200:
          description: OK
      tags:
      - Snippets
  /v3/snippets/{id}/raw:
    get:
      summary: Get Snippets Raw
      description: This feature was introduced in GitLab 8.15.
      operationId: getV3SnippetsIdRaw
      x-api-path-slug: v3snippetsidraw-get
      parameters:
      - in: path
        name: id
        description: The ID of a snippet
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Raw
  /v3/hooks:
    get:
      summary: Get Hooks
      description: Get the list of system hooks
      operationId: getV3Hooks
      x-api-path-slug: v3hooks-get
      responses:
        200:
          description: OK
      tags:
      - Hooks
    post:
      summary: Post Hooks
      description: Create a new system hook
      operationId: postV3Hooks
      x-api-path-slug: v3hooks-post
      parameters:
      - in: formData
        name: enable_ssl_verification
        description: Do SSL verification when triggering the hook
      - in: formData
        name: push_events
        description: Trigger hook on push events
      - in: formData
        name: tag_push_events
        description: Trigger hook on tag push events
      - in: formData
        name: token
        description: The token used to validate payloads
      - in: formData
        name: url
        description: The URL to send the request to
      responses:
        200:
          description: OK
      tags:
      - Hooks
  /v3/hooks/{id}:
    get:
      summary: Get Hooks
      description: Test a hook
      operationId: getV3HooksId
      x-api-path-slug: v3hooksid-get
      parameters:
      - in: path
        name: id
        description: The ID of the system hook
      responses:
        200:
          description: OK
      tags:
      - Hooks
    delete:
      summary: Delete Hooks
      description: Delete a hook
      operationId: deleteV3HooksId
      x-api-path-slug: v3hooksid-delete
      parameters:
      - in: path
        name: id
        description: The ID of the system hook
      responses:
        200:
          description: OK
      tags:
      - Hooks
  /v3/todos:
    get:
      summary: Get Todos
      description: Get a todo list
      operationId: getV3Todos
      x-api-path-slug: v3todos-get
      parameters:
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Todos
    delete:
      summary: Delete Todos
      description: Mark all todos as done
      operationId: deleteV3Todos
      x-api-path-slug: v3todos-delete
      responses:
        200:
          description: OK
      tags:
      - Todos
  /v3/todos/{id}:
    delete:
      summary: Delete Todos
      description: Mark a todo as done
      operationId: deleteV3TodosId
      x-api-path-slug: v3todosid-delete
      parameters:
      - in: path
        name: id
        description: The ID of the todo being marked as done
      responses:
        200:
          description: OK
      tags:
      - Todos
  /v3/users:
    get:
      summary: Get Users
      description: Get the list of users
      operationId: getV3Users
      x-api-path-slug: v3users-get
      parameters:
      - in: query
        name: active
        description: Filters only active users
      - in: query
        name: blocked
        description: Filters only blocked users
      - in: query
        name: external
        description: Filters only external users
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: search
        description: Search for a username
      - in: query
        name: username
        description: Get a single user with a specific username
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Post Users
      description: Create a user. Available only for admins.
      operationId: postV3Users
      x-api-path-slug: v3users-post
      parameters:
      - in: formData
        name: admin
        description: Flag indicating the user is an administrator
      - in: formData
        name: bio
        description: The biography of the user
      - in: formData
        name: can_create_group
        description: Flag indicating the user can create groups
      - in: formData
        name: confirm
        description: Flag indicating the account needs to be confirmed
      - in: formData
        name: email
        description: The email of the user
      - in: formData
        name: external
        description: Flag indicating the user is an external user
      - in: formData
        name: extern_uid
        description: The external authentication provider UID
      - in: formData
        name: linkedin
        description: The LinkedIn username
      - in: formData
        name: location
        description: The location of the user
      - in: formData
        name: name
        description: The name of the user
      - in: formData
        name: organization
        description: The organization of the user
      - in: formData
        name: password
        description: The password of the new user
      - in: formData
        name: projects_limit
        description: The number of projects a user can create
      - in: formData
        name: provider
        description: The external provider
      - in: formData
        name: skype
        description: The Skype username
      - in: formData
        name: twitter
        description: The Twitter username
      - in: formData
        name: username
        description: The username of the user
      - in: formData
        name: website_url
        description: The website of the user
      responses:
        200:
          description: OK
      tags:
      - Users
  /v3/users/{id}:
    get:
      summary: Get Users
      description: Get a single user
      operationId: getV3UsersId
      x-api-path-slug: v3usersid-get
      parameters:
      - in: path
        name: id
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Users
    put:
      summary: Put Users
      description: Update a user. Available only for admins.
      operationId: putV3UsersId
      x-api-path-slug: v3usersid-put
      parameters:
      - in: formData
        name: admin
        description: Flag indicating the user is an administrator
      - in: formData
        name: bio
        description: The biography of the user
      - in: formData
        name: can_create_group
        description: Flag indicating the user can create groups
      - in: formData
        name: confirm
        description: Flag indicating the account needs to be confirmed
      - in: formData
        name: email
        description: The email of the user
      - in: formData
        name: external
        description: Flag indicating the user is an external user
      - in: formData
        name: extern_uid
        description: The external authentication provider UID
      - in: path
        name: id
        description: The ID of the user
      - in: formData
        name: linkedin
        description: The LinkedIn username
      - in: formData
        name: location
        description: The location of the user
      - in: formData
        name: name
        description: The name of the user
      - in: formData
        name: organization
        description: The organization of the user
      - in: formData
        name: password
        description: The password of the new user
      - in: formData
        name: projects_limit
        description: The number of projects a user can create
      - in: formData
        name: provider
        description: The external provider
      - in: formData
        name: skype
        description: The Skype username
      - in: formData
        name: twitter
        description: The Twitter username
      - in: formData
        name: username
        description: The username of the user
      - in: formData
        name: website_url
        description: The website of the user
      responses:
        200:
          description: OK
      tags:
      - Users
    delete:
      summary: Delete Users
      description: Delete a user. Available only for admins.
      operationId: deleteV3UsersId
      x-api-path-slug: v3usersid-delete
      parameters:
      - in: path
        name: id
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Users
  /v3/users/{id}/keys:
    post:
      summary: Post Users Keys
      description: Add an SSH key to a specified user. Available only for admins.
      operationId: postV3UsersIdKeys
      x-api-path-slug: v3usersidkeys-post
      parameters:
      - in: path
        name: id
        description: The ID of the user
      - in: formData
        name: key
        description: The new SSH key
      - in: formData
        name: title
        description: The title of the new SSH key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Keys
    get:
      summary: Get Users Keys
      description: Get the SSH keys of a specified user. Available only for admins.
      operationId: getV3UsersIdKeys
      x-api-path-slug: v3usersidkeys-get
      parameters:
      - in: path
        name: id
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Keys
  /v3/users/{id}/keys/{key_id}:
    delete:
      summary: Delete Users Keys Key
      description: Delete an existing SSH key from a specified user. Available only
        for admins.
      operationId: deleteV3UsersIdKeysKeyId
      x-api-path-slug: v3usersidkeyskey-id-delete
      parameters:
      - in: path
        name: id
        description: The ID of the user
      - in: path
        name: key_id
        description: The ID of the SSH key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Keys
      - Key
  /v3/users/{id}/emails:
    post:
      summary: Post Users Emails
      description: Add an email address to a specified user. Available only for admins.
      operationId: postV3UsersIdEmails
      x-api-path-slug: v3usersidemails-post
      parameters:
      - in: formData
        name: email
        description: The email of the user
      - in: path
        name: id
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Emails
    get:
      summary: Get Users Emails
      description: Get the emails addresses of a specified user. Available only for
        admins.
      operationId: getV3UsersIdEmails
      x-api-path-slug: v3usersidemails-get
      parameters:
      - in: path
        name: id
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Emails
  /v3/users/{id}/emails/{email_id}:
    delete:
      summary: Delete Users Emails Email
      description: Delete an email address of a specified user. Available only for
        admins.
      operationId: deleteV3UsersIdEmailsEmailId
      x-api-path-slug: v3usersidemailsemail-id-delete
      parameters:
      - in: path
        name: email_id
        description: The ID of the email
      - in: path
        name: id
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Emails
      - Email
  /v3/users/{id}/block:
    put:
      summary: Put Users Block
      description: Block a user. Available only for admins.
      operationId: putV3UsersIdBlock
      x-api-path-slug: v3usersidblock-put
      parameters:
      - in: path
        name: id
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Block
  /v3/users/{id}/unblock:
    put:
      summary: Put Users Unblock
      description: Unblock a user. Available only for admins.
      operationId: putV3UsersIdUnblock
      x-api-path-slug: v3usersidunblock-put
      parameters:
      - in: path
        name: id
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Unblock
  /v3/users/{id}/events:
    get:
      summary: Get Users Events
      description: This feature was introduced in GitLab 8.13.
      operationId: getV3UsersIdEvents
      x-api-path-slug: v3usersidevents-get
      parameters:
      - in: path
        name: id
        description: The ID of the user
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Users
      - Events
  /v3/user:
    get:
      summary: Get User
      description: Get the currently authenticated user
      operationId: getV3User
      x-api-path-slug: v3user-get
      responses:
        200:
          description: OK
      tags:
      - User
  /v3/user/keys:
    get:
      summary: Get User Keys
      description: Get the currently authenticated user's SSH keys
      operationId: getV3UserKeys
      x-api-path-slug: v3userkeys-get
      responses:
        200:
          description: OK
      tags:
      - User
      - Keys
    post:
      summary: Post User Keys
      description: Add a new SSH key to the currently authenticated user
      operationId: postV3UserKeys
      x-api-path-slug: v3userkeys-post
      parameters:
      - in: formData
        name: key
        description: The new SSH key
      - in: formData
        name: title
        description: The title of the new SSH key
      responses:
        200:
          description: OK
      tags:
      - User
      - Keys
  /v3/user/keys/{key_id}:
    get:
      summary: Get User Keys Key
      description: Get a single key owned by currently authenticated user
      operationId: getV3UserKeysKeyId
      x-api-path-slug: v3userkeyskey-id-get
      parameters:
      - in: path
        name: key_id
        description: The ID of the SSH key
      responses:
        200:
          description: OK
      tags:
      - User
      - Keys
      - Key
    delete:
      summary: Delete User Keys Key
      description: Delete an SSH key from the currently authenticated user
      operationId: deleteV3UserKeysKeyId
      x-api-path-slug: v3userkeyskey-id-delete
      parameters:
      - in: path
        name: key_id
        description: The ID of the SSH key
      responses:
        200:
          description: OK
      tags:
      - User
      - Keys
      - Key
  /v3/user/emails:
    get:
      summary: Get User Emails
      description: Get the currently authenticated user's email addresses
      operationId: getV3UserEmails
      x-api-path-slug: v3useremails-get
      responses:
        200:
          description: OK
      tags:
      - User
      - Emails
    post:
      summary: Post User Emails
      description: Add new email address to the currently authenticated user
      operationId: postV3UserEmails
      x-api-path-slug: v3useremails-post
      parameters:
      - in: formData
        name: email
        description: The new email
      responses:
        200:
          description: OK
      tags:
      - User
      - Emails
  /v3/user/emails/{email_id}:
    get:
      summary: Get User Emails Email
      description: Get a single email address owned by the currently authenticated
        user
      operationId: getV3UserEmailsEmailId
      x-api-path-slug: v3useremailsemail-id-get
      parameters:
      - in: path
        name: email_id
        description: The ID of the email
      responses:
        200:
          description: OK
      tags:
      - User
      - Emails
      - Email
    delete:
      summary: Delete User Emails Email
      description: Delete an email address from the currently authenticated user
      operationId: deleteV3UserEmailsEmailId
      x-api-path-slug: v3useremailsemail-id-delete
      parameters:
      - in: path
        name: email_id
        description: The ID of the email
      responses:
        200:
          description: OK
      tags:
      - User
      - Emails
      - Email
  /v3/deploy_keys:
    get:
      summary: Get Deploy Keys
      description: Get deploy keys.
      operationId: getV3DeployKeys
      x-api-path-slug: v3deploy-keys-get
      responses:
        200:
          description: OK
      tags:
      - Deploy
      - Keys
  /v3/session:
    post:
      summary: Post Session
      description: Login to get token
      operationId: postV3Session
      x-api-path-slug: v3session-post
      parameters:
      - in: formData
        name: email
        description: The email of the user
      - in: formData
        name: login
        description: The username
      - in: formData
        name: password
        description: The password of the user
      responses:
        200:
          description: OK
      tags:
      - Session
  /v3/application/settings:
    get:
      summary: Get Application Settings
      description: Get the current application settings
      operationId: getV3ApplicationSettings
      x-api-path-slug: v3applicationsettings-get
      responses:
        200:
          description: OK
      tags:
      - Application
      - Settings
    put:
      summary: Put Application Settings
      description: Modify application settings
      operationId: putV3ApplicationSettings
      x-api-path-slug: v3applicationsettings-put
      parameters:
      - in: formData
        name: admin_notification_email
        description: Abuse reports will be sent to this address if it is set
      - in: formData
        name: after_sign_out_path
        description: We will redirect users to this page after they sign out
      - in: formData
        name: after_sign_up_text
        description: Text shown after sign up
      - in: formData
        name: akismet_api_key
        description: Generate API key at http://www
      - in: formData
        name: akismet_enabled
        description: Helps prevent bots from creating issues
      - in: formData
        name: container_registry_token_expire_delay
        description: Authorization token duration (minutes)
      - in: formData
        name: default_branch_protection
        description: Determine if developers can push to master
      - in: formData
        name: default_group_visibility
        description: The default group visibility
      - in: formData
        name: default_projects_limit
        description: The maximum number of personal projects
      - in: formData
        name: default_project_visibility
        description: The default project visibility
      - in: formData
        name: default_snippet_visibility
        description: The default snippet visibility
      - in: formData
        name: disabled_oauth_sign_in_sources
        description: Disable certain OAuth sign-in sources
      - in: formData
        name: domain_blacklist
        description: Users with e-mail addresses that match these domain(s) will NOT
          be able to sign-up
      - in: formData
        name: domain_blacklist_enabled
        description: Enable domain blacklist for sign ups
      - in: formData
        name: domain_whitelist
        description: ONLY users with e-mail addresses that match these domain(s) will
          be able to sign-up
      - in: formData
        name: email_author_in_body
        description: Some email servers do not support overriding the email sender
          name
      - in: formData
        name: enabled_git_access_protocol
        description: Allow only the selected protocols to be used for Git access
      - in: formData
        name: gravatar_enabled
        description: Flag indicating if the Gravatar service is enabled
      - in: formData
        name: help_page_text
        description: Custom text displayed on the help page
      - in: formData
        name: home_page_url
        description: We will redirect non-logged in users to this page
      - in: formData
        name: housekeeping_bitmaps_enabled
        description: Creating pack file bitmaps makes housekeeping take a little longer
          but bitmaps should accelerate git clone performance
      - in: formData
        name: housekeeping_enabled
        description: Enable automatic repository housekeeping (git repack, git gc)
      - in: formData
        name: housekeeping_full_repack_period
        description: Number of Git pushes after which a full git repack is run
      - in: formData
        name: housekeeping_gc_period
        description: Number of Git pushes after which git gc is run
      - in: formData
        name: housekeeping_incremental_repack_period
        description: Number of Git pushes after which an incremental git repack is
          run
      - in: formData
        name: html_emails_enabled
        description: By default GitLab sends emails in HTML and plain text formats
          so mail clients can choose what format to use
      - in: formData
        name: import_sources
        description: Enabled sources for code import during project creation
      - in: formData
        name: koding_enabled
        description: Enable Koding
      - in: formData
        name: koding_url
        description: The Koding team URL
      - in: formData
        name: max_artifacts_size
        description: Set the maximum file size each builds artifacts can have
      - in: formData
        name: max_attachment_size
        description: Maximum attachment size in MB
      - in: formData
        name: metrics_enabled
        description: Enable the InfluxDB metrics
      - in: formData
        name: metrics_host
        description: The InfluxDB host
      - in: formData
        name: metrics_method_call_threshold
        description: A method call is only tracked when it takes longer to complete
          than the given amount of milliseconds
      - in: formData
        name: metrics_packet_size
        description: The amount of points to store in a single UDP packet
      - in: formData
        name: metrics_pool_size
        description: The amount of InfluxDB connections to open
      - in: formData
        name: metrics_port
        description: The UDP port to use for connecting to InfluxDB
      - in: formData
        name: metrics_sample_interval
        description: The sampling interval in seconds
      - in: formData
        name: metrics_timeout
        description: The amount of seconds after which an InfluxDB connection will
          time out
      - in: formData
        name: plantuml_enabled
        description: Enable PlantUML
      - in: formData
        name: plantuml_url
        description: The PlantUML server URL
      - in: formData
        name: recaptcha_enabled
        description: Helps prevent bots from creating accounts
      - in: formData
        name: recaptcha_private_key
        description: Generate private key at http://www
      - in: formData
        name: recaptcha_site_key
        description: Generate site key at http://www
      - in: formData
        name: repository_checks_enabled
        description: GitLab will periodically run git fsck in all project and wiki
          repositories to look for silent disk corruption issues
      - in: formData
        name: repository_storage
        description: Storage paths for new projects
      - in: formData
        name: require_two_factor_authentication
        description: Require all users to setup Two-factor authentication
      - in: formData
        name: restricted_visibility_levels
        description: Selected levels cannot be used by non-admin users for projects
          or snippets
      - in: formData
        name: send_user_confirmation_email
        description: Send confirmation email on sign-up
      - in: formData
        name: sentry_dsn
        description: Sentry Data Source Name
      - in: formData
        name: sentry_enabled
        description: 'Sentry is an error reporting and logging tool which is currently
          not shipped with GitLab, get it here: https://getsentry'
      - in: formData
        name: session_expire_delay
        description: Session duration in minutes
      - in: formData
        name: shared_runners_enabled
        description: Enable shared runners for new projects
      - in: formData
        name: shared_runners_text
        description: Shared runners text
      - in: formData
        name: sidekiq_throttling_enabled
        description: Enable Sidekiq Job Throttling
      - in: formData
        name: sidekiq_throttling_factor
        description: The factor by which the queues should be throttled
      - in: formData
        name: sidekiq_throttling_queus
        description: Choose which queues you wish to throttle
      - in: formData
        name: signin_enabled
        description: Flag indicating if sign in is enabled
      - in: formData
        name: signup_enabled
        description: Flag indicating if sign up is enabled
      - in: formData
        name: sign_in_text
        description: The sign in text of the GitLab application
      - in: formData
        name: two_factor_grace_period
        description: Amount of time (in hours) that users are allowed to skip forced
          configuration of two-factor authentication
      - in: formData
        name: user_default_external
        description: Newly registered users will by default be external
      - in: formData
        name: user_oauth_applications
        description: Allow users to register any application to use GitLab as an OAuth
          provider
      - in: formData
        name: version_check_enabled
        description: Let GitLab inform you when an update is available
      responses:
        200:
          description: OK
      tags:
      - Application
      - Settings
  /v3/sidekiq/queue_metrics:
    get:
      summary: Get Sekiq Queue Metrics
      description: Get the Sidekiq queue metrics
      operationId: getV3SidekiqQueueMetrics
      x-api-path-slug: v3sidekiqqueue-metrics-get
      responses:
        200:
          description: OK
      tags:
      - Sekiq
      - Queue
      - Metrics
  /v3/sidekiq/process_metrics:
    get:
      summary: Get Sekiq Process Metrics
      description: Get the Sidekiq process metrics
      operationId: getV3SidekiqProcessMetrics
      x-api-path-slug: v3sidekiqprocess-metrics-get
      responses:
        200:
          description: OK
      tags:
      - Sekiq
      - Process
      - Metrics
  /v3/sidekiq/job_stats:
    get:
      summary: Get Sekiq Job Stats
      description: Get the Sidekiq job statistics
      operationId: getV3SidekiqJobStats
      x-api-path-slug: v3sidekiqjob-stats-get
      responses:
        200:
          description: OK
      tags:
      - Sekiq
      - Job
      - Stats
  /v3/sidekiq/compound_metrics:
    get:
      summary: Get Sekiq Compound Metrics
      description: Get the Sidekiq Compound metrics. Includes queue, process, and
        job statistics
      operationId: getV3SidekiqCompoundMetrics
      x-api-path-slug: v3sidekiqcompound-metrics-get
      responses:
        200:
          description: OK
      tags:
      - Sekiq
      - Compound
      - Metrics
  /v3/licenses:
    get:
      summary: Get Licenses
      description: This feature was introduced in GitLab 8.7. This endpoint is deprecated
        and will be removed in GitLab 9.0.
      operationId: getV3Licenses
      x-api-path-slug: v3licenses-get
      parameters:
      - in: query
        name: popular
        description: If passed, returns only popular licenses
      responses:
        200:
          description: OK
      tags:
      - Licenses
  /v3/licenses/{name}:
    get:
      summary: Get Licenses Name
      description: This feature was introduced in GitLab 8.7. This endpoint is deprecated
        and will be removed in GitLab 9.0.
      operationId: getV3LicensesName
      x-api-path-slug: v3licensesname-get
      parameters:
      - in: path
        name: name
        description: The name of the template
      responses:
        200:
          description: OK
      tags:
      - Licenses
      - Name
  /v3/templates/licenses:
    get:
      summary: Get Templates Licenses
      description: This feature was introduced in GitLab 8.7.
      operationId: getV3TemplatesLicenses
      x-api-path-slug: v3templateslicenses-get
      parameters:
      - in: query
        name: popular
        description: If passed, returns only popular licenses
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Licenses
  /v3/templates/licenses/{name}:
    get:
      summary: Get Templates Licenses Name
      description: This feature was introduced in GitLab 8.7.
      operationId: getV3TemplatesLicensesName
      x-api-path-slug: v3templateslicensesname-get
      parameters:
      - in: path
        name: name
        description: The name of the template
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Licenses
      - Name
  /v3/templates/gitignores:
    get:
      summary: Get Templates Gitignores
      description: This feature was introduced in GitLab 8.8.
      operationId: getV3TemplatesGitignores
      x-api-path-slug: v3templatesgitignores-get
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Gitignores
  /v3/templates/gitignores/{name}:
    get:
      summary: Get Templates Gitignores Name
      description: This feature was introduced in GitLab 8.8.
      operationId: getV3TemplatesGitignoresName
      x-api-path-slug: v3templatesgitignoresname-get
      parameters:
      - in: path
        name: name
        description: The name of the template
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Gitignores
      - Name
  /v3/templates/gitlab_ci_ymls:
    get:
      summary: Get Templates Gitlab Ci Ymls
      description: This feature was introduced in GitLab 8.9.
      operationId: getV3TemplatesGitlabCiYmls
      x-api-path-slug: v3templatesgitlab-ci-ymls-get
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Gitlab
      - Ci
      - Ymls
  /v3/templates/gitlab_ci_ymls/{name}:
    get:
      summary: Get Templates Gitlab Ci Ymls Name
      description: This feature was introduced in GitLab 8.9.
      operationId: getV3TemplatesGitlabCiYmlsName
      x-api-path-slug: v3templatesgitlab-ci-ymlsname-get
      parameters:
      - in: path
        name: name
        description: The name of the template
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Gitlab
      - Ci
      - Ymls
      - Name
  /v3/templates/dockerfiles:
    get:
      summary: Get Templates Dockerfiles
      description: This feature was introduced in GitLab 8.15.
      operationId: getV3TemplatesDockerfiles
      x-api-path-slug: v3templatesdockerfiles-get
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Dockerfiles
  /v3/templates/dockerfiles/{name}:
    get:
      summary: Get Templates Dockerfiles Name
      description: This feature was introduced in GitLab 8.15.
      operationId: getV3TemplatesDockerfilesName
      x-api-path-slug: v3templatesdockerfilesname-get
      parameters:
      - in: path
        name: name
        description: The name of the template
      responses:
        200:
          description: OK
      tags:
      - Templates
      - Dockerfiles
      - Name
  /v3/gitignores:
    get:
      summary: Get Gitignores
      description: This feature was introduced in GitLab 8.8. This endpoint is deprecated
        and will be removed in GitLab 9.0.
      operationId: getV3Gitignores
      x-api-path-slug: v3gitignores-get
      responses:
        200:
          description: OK
      tags:
      - Gitignores
  /v3/gitignores/{name}:
    get:
      summary: Get Gitignores Name
      description: This feature was introduced in GitLab 8.8. This endpoint is deprecated
        and will be removed in GitLab 9.0.
      operationId: getV3GitignoresName
      x-api-path-slug: v3gitignoresname-get
      parameters:
      - in: path
        name: name
        description: The name of the template
      responses:
        200:
          description: OK
      tags:
      - Gitignores
      - Name
  /v3/gitlab_ci_ymls:
    get:
      summary: Get Gitlab Ci Ymls
      description: This feature was introduced in GitLab 8.9. This endpoint is deprecated
        and will be removed in GitLab 9.0.
      operationId: getV3GitlabCiYmls
      x-api-path-slug: v3gitlab-ci-ymls-get
      responses:
        200:
          description: OK
      tags:
      - Gitlab
      - Ci
      - Ymls
  /v3/gitlab_ci_ymls/{name}:
    get:
      summary: Get Gitlab Ci Ymls Name
      description: This feature was introduced in GitLab 8.9. This endpoint is deprecated
        and will be removed in GitLab 9.0.
      operationId: getV3GitlabCiYmlsName
      x-api-path-slug: v3gitlab-ci-ymlsname-get
      parameters:
      - in: path
        name: name
        description: The name of the template
      responses:
        200:
          description: OK
      tags:
      - Gitlab
      - Ci
      - Ymls
      - Name
  /v3/dockerfiles:
    get:
      summary: Get Dockerfiles
      description: This feature was introduced in GitLab 8.15. This endpoint is deprecated
        and will be removed in GitLab 9.0.
      operationId: getV3Dockerfiles
      x-api-path-slug: v3dockerfiles-get
      responses:
        200:
          description: OK
      tags:
      - Dockerfiles
  /v3/dockerfiles/{name}:
    get:
      summary: Get Dockerfiles Name
      description: This feature was introduced in GitLab 8.15. This endpoint is deprecated
        and will be removed in GitLab 9.0.
      operationId: getV3DockerfilesName
      x-api-path-slug: v3dockerfilesname-get
      parameters:
      - in: path
        name: name
        description: The name of the template
      responses:
        200:
          description: OK
      tags:
      - Dockerfiles
      - Name
  /v3/version:
    get:
      summary: Get Version
      description: This feature was introduced in GitLab 8.13.
      operationId: getV3Version
      x-api-path-slug: v3version-get
      responses:
        200:
          description: OK
      tags:
      - Version