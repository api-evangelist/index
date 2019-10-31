swagger: "2.0"
x-collection-name: 123FormBuilder
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: api.123contactform.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ping:
    get:
      summary: Ping status
      description: This indicates if our servers are up and running.
      operationId: this-indicates-if-our-servers-are-up-and-running
      x-api-path-slug: ping-get
      responses:
        200:
          description: OK
      tags:
      - Ping
      - Status
  /token:
    post:
      summary: User login
      description: "Allows you to authenticate users. \n\nRequired parameters:\n-
        username OR email\n- password OR passhash"
      operationId: allows-you-to-authenticate-users-required-parameters-username-or-email-password-or-passhash
      x-api-path-slug: token-post
      parameters:
      - in: query
        name: email
      - in: query
        name: passhash
        description: MD5 password
      - in: query
        name: password
        description: Plain text password
      - in: query
        name: username
      responses:
        200:
          description: OK
      tags:
      - User
      - Login
  /token/refresh:
    post:
      summary: Refresh token
      description: Refresh token
      operationId: refresh-token
      x-api-path-slug: tokenrefresh-post
      parameters:
      - in: formData
        name: JWT
        description: JWT authentication token
      responses:
        200:
          description: OK
      tags:
      - Refresh
      - Token
  /token/invalidate:
    post:
      summary: Invalidate token
      description: Invalidate token
      operationId: invalidate-token
      x-api-path-slug: tokeninvalidate-post
      parameters:
      - in: formData
        name: JWT
        description: JWT authentication token
      responses:
        200:
          description: OK
      tags:
      - Invalidate
      - Token
  /forms:
    get:
      summary: List forms
      description: The forms endpoint returns information about the forms. The response
        includes submissions and other details about each form.
      operationId: the-forms-endpoint-returns-information-about-the-forms-the-response-includes-submissions-and-other-d
      x-api-path-slug: forms-get
      parameters:
      - in: query
        name: JWT
        description: JWT authentication token
      - in: query
        name: page
        description: Page number
      - in: query
        name: per_page
        description: The number of forms to get per page in a request
      - in: query
        name: search
        description: Filter form name
      responses:
        200:
          description: OK
      tags:
      - List
      - Forms
    post:
      summary: Create a new form
      description: Create a new form
      operationId: create-a-new-form
      x-api-path-slug: forms-post
      parameters:
      - in: formData
        name: active
        description: Form activity status
      - in: formData
        name: active_date_from
        description: If activity status is 1, this field is required
      - in: formData
        name: active_date_to
        description: If activity status is 1, this field is required
      - in: formData
        name: active_days
        description: If activity status is 4, this field is required
      - in: formData
        name: group_id
        description: The ID of the group in which you want to create the form
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: name
        description: The name of the new form
      responses:
        200:
          description: OK
      tags:
      - New
      - Form
  /forms/bulk:
    delete:
      summary: Delete multiple forms
      description: Delete multiple forms
      operationId: delete-multiple-forms
      x-api-path-slug: formsbulk-delete
      parameters:
      - in: formData
        name: form_ids
        description: The IDs of the forms separated by comma
      - in: formData
        name: JWT
        description: JWT authentication token
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Forms
  /forms/{form_id}:
    get:
      summary: Get form details
      description: Get the details of a single form
      operationId: get-the-details-of-a-single-form
      x-api-path-slug: formsform-id-get
      parameters:
      - in: path
        name: form_id
        description: The ID of the form
      - in: query
        name: JWT
        description: JWT authentication token
      responses:
        200:
          description: OK
      tags:
      - Form
      - Details
    put:
      summary: Update form details
      description: Update form details
      operationId: update-form-details
      x-api-path-slug: formsform-id-put
      parameters:
      - in: formData
        name: active
        description: Form activity status
      - in: formData
        name: active_date_from
        description: If activity status is 1, this field is required
      - in: formData
        name: active_date_to
        description: If activity status is 1, this field is required
      - in: formData
        name: active_days
        description: If activity status is 4, this field is required
      - in: path
        name: form_id
        description: The ID of the form
      - in: formData
        name: group_id
        description: The ID of the group in which you want to create the form
      - in: query
        name: JWT
        description: JWT authentication token
      - in: formData
        name: name
        description: Change the name of the form
      responses:
        200:
          description: OK
      tags:
      - Form
      - Details
    delete:
      summary: Delete a form
      description: Delete a form
      operationId: delete-a-form
      x-api-path-slug: formsform-id-delete
      parameters:
      - in: path
        name: form_id
        description: The ID of the form
      - in: formData
        name: JWT
        description: JWT authentication token
      responses:
        200:
          description: OK
      tags:
      - Form
  /forms/{form_id}/fields:
    get:
      summary: Get form fields
      description: Get the details of a single form and its fields
      operationId: get-the-details-of-a-single-form-and-its-fields
      x-api-path-slug: formsform-idfields-get
      parameters:
      - in: path
        name: form_id
        description: The ID of the form
      - in: query
        name: JWT
        description: JWT authentication token
      responses:
        200:
          description: OK
      tags:
      - Form
      - Fields
  /forms/{form_id}/submissions:
    get:
      summary: Get submissions
      description: Get all submissions received through a form
      operationId: get-all-submissions-received-through-a-form
      x-api-path-slug: formsform-idsubmissions-get
      parameters:
      - in: path
        name: form_id
        description: The ID of the form
      - in: query
        name: include_recipients
        description: Returns the recipient(s) who should receive the submissions
      - in: query
        name: JWT
        description: JWT authentication token
      - in: query
        name: page
        description: Page number
      - in: query
        name: per_page
        description: The number of submissions to get per page in a request
      - in: query
        name: start_date
        description: List submissions starting with a specific date
      - in: query
        name: start_submission_id
        description: List all submissions starting with the specified submission ID
      responses:
        200:
          description: OK
      tags:
      - Submissions
  /forms/{form_id}/submissions/{submission_id}:
    get:
      summary: Get submission details
      description: Get the details of a single submission
      operationId: get-the-details-of-a-single-submission
      x-api-path-slug: formsform-idsubmissionssubmission-id-get
      parameters:
      - in: path
        name: form_id
        description: The ID of the form
      - in: query
        name: include_recipients
        description: Returns the recipient(s) who should receive the submission
      - in: query
        name: JWT
        description: JWT authentication token
      - in: path
        name: submission_id
        description: The ID of the submission
      responses:
        200:
          description: OK
      tags:
      - Submission
      - Details
    put:
      summary: Update Submission
      description: Update Submission
      operationId: update-submission
      x-api-path-slug: formsform-idsubmissionssubmission-id-put
      parameters:
      - in: query
        name: approved
        description: Approval status
      - in: path
        name: form_id
        description: The ID of the form
      - in: query
        name: JWT
        description: JWT authentication token
      - in: query
        name: payed
        description: Payment status
      - in: path
        name: submission_id
        description: The ID of the submission
      responses:
        200:
          description: OK
      tags:
      - Submission
    delete:
      summary: Delete one form submission
      description: Delete one form submission
      operationId: delete-one-form-submission
      x-api-path-slug: formsform-idsubmissionssubmission-id-delete
      parameters:
      - in: path
        name: form_id
        description: The ID of the form
      - in: query
        name: JWT
        description: JWT authentication token
      - in: path
        name: submission_id
        description: The ID of the submission
      responses:
        200:
          description: OK
      tags:
      - Form
      - Submission
  /groups:
    get:
      summary: Get all user groups
      description: Get all user groups
      operationId: get-all-user-groups
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: JWT
        description: JWT authentication token
      - in: query
        name: page
        description: Page number
      - in: query
        name: per_page
        description: The number of groups to get per page in a request
      responses:
        200:
          description: OK
      tags:
      - User
      - Groups
    post:
      summary: Create a new group
      description: Create a new group
      operationId: create-a-new-group
      x-api-path-slug: groups-post
      parameters:
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: name
        description: Form name
      - in: formData
        name: parent_id
        description: Indicates the ID of the parent group
      - in: formData
        name: webhook_url
        description: The URL of the WebHook
      responses:
        200:
          description: OK
      tags:
      - New
      - Group
  /groups/{group_id}:
    get:
      summary: Get group details
      description: Get information about a specific group.
      operationId: get-information-about-a-specific-group
      x-api-path-slug: groupsgroup-id-get
      parameters:
      - in: path
        name: group_id
        description: The ID of the group
      - in: query
        name: JWT
        description: JWT authentication token
      responses:
        200:
          description: OK
      tags:
      - Group
      - Details
    put:
      summary: Update group data
      description: Updates the details of a group.
      operationId: updates-the-details-of-a-group
      x-api-path-slug: groupsgroup-id-put
      parameters:
      - in: path
        name: group_id
        description: The ID of the group you want to edit
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: name
        description: This is required when the webhook_url or parent_id is missing
      - in: formData
        name: parent_id
        description: Indicates the ID of the parent group
      - in: formData
        name: webhook_url
        description: This is required when the name or parent_id is missing
      responses:
        200:
          description: OK
      tags:
      - Group
      - Data
  /groups/{group_id}/forms:
    get:
      summary: Get all forms in a group
      description: Displays a list of all of the forms within a specific group.
      operationId: displays-a-list-of-all-of-the-forms-within-a-specific-group
      x-api-path-slug: groupsgroup-idforms-get
      parameters:
      - in: path
        name: group_id
        description: The ID of the group
      - in: query
        name: JWT
        description: JWT authentication token
      responses:
        200:
          description: OK
      tags:
      - Forms
      - In
      - Group
  /groups/{group_id}/share:
    post:
      summary: Share a group with a user
      description: This may not be available for your account. It is specific to certain
        users.
      operationId: this-may-not-be-available-for-your-account-it-is-specific-to-certain-users
      x-api-path-slug: groupsgroup-idshare-post
      parameters:
      - in: path
        name: group_id
        description: The ID of the group you want to share
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: subuser_email
        description: The username with whom you want to share this group
      - in: formData
        name: subuser_id
        description: The ID of the user with whom you want to share this group
      responses:
        200:
          description: OK
      tags:
      - Share
      - Group
      - User
  /groups/{group_id}/unshare:
    post:
      summary: Unshare a group from a user
      description: This may not be available for your account. It is specific to certain
        users.
      operationId: this-may-not-be-available-for-your-account-it-is-specific-to-certain-users
      x-api-path-slug: groupsgroup-idunshare-post
      parameters:
      - in: path
        name: group_id
        description: The ID of the group you want to unshare
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: subuser_email
        description: The username from whom you want to unshare the group
      - in: formData
        name: subuser_id
        description: The ID of the subuser from whom you want to unshare the group
      responses:
        200:
          description: OK
      tags:
      - Unshare
      - Group
      - From
      - User
  /users:
    get:
      summary: Get info about master user and subusers
      description: Get info about master user and subusers
      operationId: get-info-about-master-user-and-subusers
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: JWT
        description: JWT authentication token
      - in: query
        name: page
        description: Page number
      - in: query
        name: per_page
        description: The number of groups to get per page in a request
      responses:
        200:
          description: OK
      tags:
      - Info
      - About
      - Master
      - User
      - Subusers
    post:
      summary: Create a new subuser
      description: Create a new subuser
      operationId: create-a-new-subuser
      x-api-path-slug: users-post
      parameters:
      - in: formData
        name: admin
        description: Indicates if the subuser is admin or not
      - in: formData
        name: allow_create_form
        description: Allow or restrict subuser access to creating new forms
      - in: formData
        name: allow_delete_form
        description: Allow subusers to delete forms
      - in: formData
        name: allow_duplicate_form
        description: Allow subusers to duplicate forms
      - in: formData
        name: can_manage_groups
        description: Allow admin subusers to manage groups
      - in: formData
        name: can_manage_users
        description: Allow admin subusers to manage users
      - in: formData
        name: company_name
        description: The name of the company to which the subuser belongs
      - in: formData
        name: email
        description: Email address of the account
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: name
        description: Username of the account
      - in: formData
        name: passhash
        description: MD5 password
      - in: formData
        name: password
        description: Plain text password
      responses:
        200:
          description: OK
      tags:
      - New
      - Subuser
  /users/{identifier}:
    put:
      summary: Update user
      description: Update user information
      operationId: update-user-information
      x-api-path-slug: usersidentifier-put
      parameters:
      - in: formData
        name: admin
        description: Indicates if the subuser is admin or not
      - in: formData
        name: allow_create_form
        description: Allow or restrict subuser access to creating new forms
      - in: formData
        name: allow_delete_form
        description: Allow subusers to delete forms
      - in: formData
        name: allow_duplicate_form
        description: Allow subusers to duplicate forms
      - in: formData
        name: can_manage_groups
        description: Allow admin subusers to manage groups
      - in: formData
        name: can_manage_users
        description: Allow admin subusers to manage users
      - in: formData
        name: company_name
        description: The name of the company to which the subuser belongs
      - in: formData
        name: email
        description: Email address of the account
      - in: path
        name: identifier
        description: The ID or username of the user to be modified
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: passhash
        description: MD5 password
      - in: formData
        name: password
        description: Plain text password
      responses:
        200:
          description: OK
      tags:
      - User
  /accounts:
    post:
      summary: Create new account
      description: Creates a new account (standalone user). This is available only
        upon request.
      operationId: creates-a-new-account-standalone-user-this-is-available-only-upon-request
      x-api-path-slug: accounts-post
      parameters:
      - in: formData
        name: company_name
        description: The company name associated with the account
      - in: formData
        name: email
        description: The email address associated with the account
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: name
        description: The username associated with the account
      - in: formData
        name: password
        description: The password associated with the account
      - in: formData
        name: password_repeat
        description: Password repeat
      - in: formData
        name: plan
        description: 'The service plan of the account: 0 - Free (default value), 1
          - Gold, 2 - Platinum, 3 - Diamond'
      responses:
        200:
          description: OK
      tags:
      - New
      - Account
  /accounts/{user_id}:
    put:
      summary: Update account
      description: Updates an account. You can only update the users that you have
        created using your account token.
      operationId: updates-an-account-you-can-only-update-the-users-that-you-have-created-using-your-account-token
      x-api-path-slug: accountsuser-id-put
      parameters:
      - in: formData
        name: company_name
        description: The company name associated with the account
      - in: formData
        name: email
        description: The email address associated with the account
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: password
        description: The password associated with the account
      - in: formData
        name: password_repeat
        description: Password repeat
      - in: formData
        name: plan
        description: 'The service plan of the account: 0 - Free (default value), 1
          - Gold, 2 - Platinum, 3 - Diamond'
      - in: path
        name: user_id
        description: The ID of the account that you want to update
      responses:
        200:
          description: OK
      tags:
      - Account