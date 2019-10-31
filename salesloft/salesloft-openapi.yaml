swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 1
info:
  title: SalesLoft
  description: salesloft-helps-transform-sales-teams-into-modern-sales-organizations---converting-more-target-accounts-into-customer-accounts
  version: v2
host: api.salesloft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/accounts.json:
    get:
      summary: List accounts
      description: |-
        Fetches multiple account records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.accounts.json.get
      x-api-path-slug: v2accounts-json-get
      parameters:
      - in: query
        name: domain
        description: Domain of the accounts to fetch
      - in: query
        name: ids
        description: IDs of accounts to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, last_contacted_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Accounts
    post:
      summary: Create an account
      description: |-
        Creates an account.

        "domain" must be unique on the current team.
      operationId: v2.accounts.json.post
      x-api-path-slug: v2accounts-json-post
      parameters:
      - in: formData
        name: city
        description: City
      - in: formData
        name: company_stage_id
        description: ID of the CompanyStage assigned to this Account
      - in: formData
        name: company_type
        description: Type of the Accounts company
      - in: formData
        name: conversational_name
        description: Conversational name of the Account
      - in: formData
        name: country
        description: Country
      - in: formData
        name: custom_fields
        description: Custom fields are defined by the users team
      - in: formData
        name: description
        description: Description
      - in: formData
        name: domain
        description: Website domain, not a fully qualified URI
      - in: formData
        name: do_not_contact
        description: Whether this company can not be contacted
      - in: formData
        name: founded
        description: Date or year of founding
      - in: formData
        name: industry
        description: Industry
      - in: formData
        name: linkedin_url
        description: Full LinkedIn url
      - in: formData
        name: locale
        description: Time locale
      - in: formData
        name: name
        description: Account Full Name
      - in: formData
        name: owner_id
        description: ID of the User that owns this Account
      - in: formData
        name: phone
        description: Phone number without formatting
      - in: formData
        name: postal_code
        description: Postal code
      - in: formData
        name: revenue_range
        description: Estimated revenue range
      - in: formData
        name: size
        description: Estimated number of people in employment
      - in: formData
        name: state
        description: State
      - in: formData
        name: street
        description: Street name and number
      - in: formData
        name: tags
        description: All tags applied to this Account
      - in: formData
        name: twitter_handle
        description: Twitter handle, with @
      - in: formData
        name: website
        description: Website
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Account
  /v2/accounts/{id}.json:
    delete:
      summary: Delete an account
      description: |-
        Deletes an account. This operation is not reversible without contacting support.
        This operation can be called multiple times successfully.

        Deleting an account will remove all connected people from that account.
      operationId: v2.accounts.id.json.delete
      x-api-path-slug: v2accountsid-json-delete
      parameters:
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Account
    get:
      summary: Fetch an account
      description: Fetches an account, by ID only.
      operationId: v2.accounts.id.json.get
      x-api-path-slug: v2accountsid-json-get
      parameters:
      - in: path
        name: id
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Account
    put:
      summary: Update an existing Account
      description: |-
        Updates an account.

        "domain" must be unique on the current team.
      operationId: v2.accounts.id.json.put
      x-api-path-slug: v2accountsid-json-put
      parameters:
      - in: formData
        name: city
        description: City
      - in: formData
        name: company_stage_id
        description: ID of the CompanyStage assigned to this Account
      - in: formData
        name: company_type
        description: Type of the Accounts company
      - in: formData
        name: conversational_name
        description: Conversational name of the Account
      - in: formData
        name: country
        description: Country
      - in: formData
        name: custom_fields
        description: Custom fields are defined by the users team
      - in: formData
        name: description
        description: Description
      - in: formData
        name: domain
        description: Website domain, not a fully qualified URI
      - in: formData
        name: do_not_contact
        description: Whether this company can not be contacted
      - in: formData
        name: founded
        description: Date or year of founding
      - in: path
        name: id
        description: Account ID
      - in: formData
        name: industry
        description: Industry
      - in: formData
        name: linkedin_url
        description: Full LinkedIn url
      - in: formData
        name: locale
        description: Time locale
      - in: formData
        name: name
        description: Account Full Name
      - in: formData
        name: owner_id
        description: ID of the User that owns this Account
      - in: formData
        name: phone
        description: Phone number without formatting
      - in: formData
        name: postal_code
        description: Postal code
      - in: formData
        name: revenue_range
        description: Estimated revenue range
      - in: formData
        name: size
        description: Estimated number of people in employment
      - in: formData
        name: state
        description: State
      - in: formData
        name: street
        description: Street name and number
      - in: formData
        name: tags
        description: All tags applied to this Account
      - in: formData
        name: twitter_handle
        description: Twitter handle, with @
      - in: formData
        name: website
        description: Website
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Existing
      - Account
  /v2/action_details/call_instructions.json:
    get:
      summary: List call instructions
      description: |-
        Fetches multiple call instruction records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.action_details.call_instructions.json.get
      x-api-path-slug: v2action-detailscall-instructions-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of call instructions to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Call
      - Instructions
  /v2/action_details/call_instructions/{id}.json:
    get:
      summary: Fetch a call instructions
      description: Fetches a call instruction, by ID only.
      operationId: v2.action_details.call_instructions.id.json.get
      x-api-path-slug: v2action-detailscall-instructionsid-json-get
      parameters:
      - in: path
        name: id
        description: Call instructions ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Call
      - Instructions
  /v2/actions.json:
    get:
      summary: List actions
      description: |-
        Fetches multiple action records. The records can be filtered, paged, and sorted according to
        the respective parameters. Only actions that are currently "in_progess" will be returned by
        this endpoint.
      operationId: v2.actions.json.get
      x-api-path-slug: v2actions-json-get
      parameters:
      - in: query
        name: due_on
        description: Equality filters that are applied to the due_on field
      - in: query
        name: ids
        description: IDs of actions to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: step_id
        description: Fetch actions by step ID
      - in: query
        name: type
        description: Filter actions by type
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Actions
  /v2/actions/{id}.json:
    get:
      summary: Fetch an action
      description: |-
        Fetches an action, by ID only.
        This endpoint will only return actions that are in_progress or pending_activity.
        Once an action is complete, the request for that action will return a 404 status code.
      operationId: v2.actions.id.json.get
      x-api-path-slug: v2actionsid-json-get
      parameters:
      - in: path
        name: id
        description: Action ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Action
  /v2/activities/calls.json:
    get:
      summary: List calls
      description: |-
        Fetches multiple call records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.activities.calls.json.get
      x-api-path-slug: v2activitiescalls-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of calls to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Calls
  /v2/activities/calls/{id}.json:
    get:
      summary: Fetch a call
      description: Fetches a call, by ID only.
      operationId: v2.activities.calls.id.json.get
      x-api-path-slug: v2activitiescallsid-json-get
      parameters:
      - in: path
        name: id
        description: Call ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Call
  /v2/activities/emails.json:
    get:
      summary: List emails
      description: |-
        Fetches multiple email records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.activities.emails.json.get
      x-api-path-slug: v2activitiesemails-json-get
      parameters:
      - in: query
        name: bounced
        description: Filters emails by whether they have bounced or not
      - in: query
        name: ids
        description: IDs of emails to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Emails
  /v2/activities/emails/{id}.json:
    get:
      summary: Fetch an email
      description: Fetches an email, by ID only.
      operationId: v2.activities.emails.id.json.get
      x-api-path-slug: v2activitiesemailsid-json-get
      parameters:
      - in: path
        name: id
        description: Email ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Email
  /v2/cadence_memberships.json:
    get:
      summary: List cadence memberships
      description: |-
        Fetches multiple cadence membership records. The records can be filtered, paged, and sorted according to
        the respective parameters. A cadence membership is the association between a person and their current and
        historical time on a cadence. Cadence membership records are mutable and change over time. If a person is
        added to a cadence and re-added to the same cadence in the future, there is a single membership record.
      operationId: v2.cadence_memberships.json.get
      x-api-path-slug: v2cadence-memberships-json-get
      parameters:
      - in: query
        name: cadence_id
        description: ID of the cadence to find cadence memberships for
      - in: query
        name: ids
        description: IDs of cadence memberships to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: person_id
        description: ID of the person to find cadence memberships for
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Cadence
      - Memberships
    post:
      summary: Create a cadence membership
      description: |-
        Adds a person to a cadence. person_id and cadence_id are required, and must be visible to the authenticated user. user_id will
        default to the authenticated user, but can be set to any visible user on the authenticated team.

        A person cannot be added to a cadence on behalf of a teammate unless the cadence is a team cadence, or the cadence is owned by
        the teammate.
      operationId: v2.cadence_memberships.json.post
      x-api-path-slug: v2cadence-memberships-json-post
      parameters:
      - in: query
        name: cadence_id
        description: ID of the cadence to create a cadence membership for
      - in: query
        name: person_id
        description: ID of the person to create a cadence membership for
      - in: query
        name: user_id
        description: ID of the user to create a cadence membership for
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Cadence
      - Membership
  /v2/cadence_memberships/{id}.json:
    delete:
      summary: Delete a cadence membership
      description: ""
      operationId: v2.cadence_memberships.id.json.delete
      x-api-path-slug: v2cadence-membershipsid-json-delete
      parameters:
      - in: path
        name: id
        description: CadenceMembership ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Cadence
      - Membership
    get:
      summary: Fetch a cadence membership
      description: Fetches a cadence membership, by ID only.
      operationId: v2.cadence_memberships.id.json.get
      x-api-path-slug: v2cadence-membershipsid-json-get
      parameters:
      - in: path
        name: id
        description: CadenceMembership ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Cadence
      - Membership
  /v2/cadences.json:
    get:
      summary: List cadences
      description: |-
        Fetches multiple cadence records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.cadences.json.get
      x-api-path-slug: v2cadences-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of cadences to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: team_cadence
        description: Filters cadences by whether they are a team cadence or not
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Cadences
  /v2/cadences/{id}.json:
    get:
      summary: Fetch a cadence
      description: Fetches a cadence, by ID only.
      operationId: v2.cadences.id.json.get
      x-api-path-slug: v2cadencesid-json-get
      parameters:
      - in: path
        name: id
        description: Cadence ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Cadence
  /v2/call_data_records.json:
    get:
      summary: List call data records
      description: |-
        Fetches multiple call data records. The records can be filtered, paged, and sorted according to
        the respective parameters.

        Call data records are records of all inbound and outbound calls through SalesLoft. A call data record may
        be associated with a call, but does not have to be.
      operationId: v2.call_data_records.json.get
      x-api-path-slug: v2call-data-records-json-get
      parameters:
      - in: query
        name: has_call
        description: Return only call data records which have or do not have a call
          logged for them
      - in: query
        name: ids
        description: IDs of call data records to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Call
      - Data
      - Records
  /v2/call_data_records/{id}.json:
    get:
      summary: Fetch a call data record
      description: Fetches a call data record, by ID only.
      operationId: v2.call_data_records.id.json.get
      x-api-path-slug: v2call-data-recordsid-json-get
      parameters:
      - in: path
        name: id
        description: CallDataRecord ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Call
      - Data
      - Record
  /v2/crm_activities.json:
    get:
      summary: List crm activities
      description: |-
        Fetches multiple crm activity records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.crm_activities.json.get
      x-api-path-slug: v2crm-activities-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of crm activities to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Crm
      - Activities
  /v2/crm_activities/{id}.json:
    get:
      summary: Fetch a crm activity
      description: Fetches a crm activity, by ID only.
      operationId: v2.crm_activities.id.json.get
      x-api-path-slug: v2crm-activitiesid-json-get
      parameters:
      - in: path
        name: id
        description: Crm activity ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Crm
      - Activity
  /v2/custom_fields.json:
    get:
      summary: List custom fields
      description: |-
        Fetches multiple custom field records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.custom_fields.json.get
      x-api-path-slug: v2custom-fields-json-get
      parameters:
      - in: query
        name: field_type
        description: Type of field to fetch
      - in: query
        name: ids
        description: IDs of custom fields to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, name'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Custom
      - Fields
    post:
      summary: Create a custom field
      description: Creates a custom field.
      operationId: v2.custom_fields.json.post
      x-api-path-slug: v2custom-fields-json-post
      parameters:
      - in: formData
        name: field_type
        description: The field type of the custom field
      - in: formData
        name: name
        description: The name of the custom field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Custom
      - Field
  /v2/custom_fields/{id}.json:
    delete:
      summary: Delete a custom field
      description: Deletes a custom field.
      operationId: v2.custom_fields.id.json.delete
      x-api-path-slug: v2custom-fieldsid-json-delete
      parameters:
      - in: path
        name: id
        description: Custom Field ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Custom
      - Field
    get:
      summary: Fetch a custom field
      description: Fetches a custom field, by ID only.
      operationId: v2.custom_fields.id.json.get
      x-api-path-slug: v2custom-fieldsid-json-get
      parameters:
      - in: path
        name: id
        description: Custom Field ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Custom
      - Field
    put:
      summary: Update a custom field
      description: Update a custom field.
      operationId: v2.custom_fields.id.json.put
      x-api-path-slug: v2custom-fieldsid-json-put
      parameters:
      - in: formData
        name: field_type
        description: The field type of the custom field
      - in: path
        name: id
        description: Custom Field ID
      - in: formData
        name: name
        description: The name of the custom field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Custom
      - Field
  /v2/email_templates.json:
    get:
      summary: List email templates
      description: |-
        Fetches multiple email template records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.email_templates.json.get
      x-api-path-slug: v2email-templates-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of email templates to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: linked_to_team_template
        description: Filters email templates by whether they are linked to a team
          template or not
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, last_used_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Email
      - Templates
  /v2/email_templates/{id}.json:
    get:
      summary: Fetch an email template
      description: Fetches an email template, by ID only.
      operationId: v2.email_templates.id.json.get
      x-api-path-slug: v2email-templatesid-json-get
      parameters:
      - in: path
        name: id
        description: EmailTemplate ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Email
      - Template
  /v2/imports.json:
    get:
      summary: List imports
      description: Fetches multiple imports.
      operationId: v2.imports.json.get
      x-api-path-slug: v2imports-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of imports to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: user_ids
        description: ID of users to fetch imports for
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Imports
    post:
      summary: Create an import
      description: Creates an import.
      operationId: v2.imports.json.post
      x-api-path-slug: v2imports-json-post
      parameters:
      - in: formData
        name: name
        description: Name, recommended to be easily identifiable to a user
      - in: formData
        name: user_id
        description: ID of the User that owns this Import
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Import
  /v2/imports/{id}.json:
    delete:
      summary: Delete an import
      description: |-
        Deletes an import, by ID only. The associated people can be deleted as part of the deletion process.

        Admin users can access imports for the entire team, but non-admin users can only access their own imports.
      operationId: v2.imports.id.json.delete
      x-api-path-slug: v2importsid-json-delete
      parameters:
      - in: path
        name: id
        description: Import ID
      - in: query
        name: undo
        description: Whether to delete people on this Import
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Import
    get:
      summary: Fetch an import
      description: |-
        Fetches an import, by ID only.

        Admin users can access imports for the entire team, but non-admin users can only access their own imports.
      operationId: v2.imports.id.json.get
      x-api-path-slug: v2importsid-json-get
      parameters:
      - in: path
        name: id
        description: Import ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Import
    put:
      summary: Update an import
      description: |-
        Updates an import, by ID only.

        Admin users can access imports for the entire team, but non-admin users can only access their own imports.
      operationId: v2.imports.id.json.put
      x-api-path-slug: v2importsid-json-put
      parameters:
      - in: path
        name: id
        description: Import ID
      - in: formData
        name: name
        description: Name, recommended to be easily identifiable to a user
      - in: formData
        name: user_id
        description: ID of the User that owns this Import
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Import
  /v2/me.json:
    get:
      summary: Fetch current user
      description: |-
        Authenticated user information. This endpoint does not accept any parameters as it is
        represents your authenticated user. The "Users" resource provides user information
        for other users on the team.
      operationId: v2.me.json.get
      x-api-path-slug: v2me-json-get
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Current
      - User
  /v2/notes.json:
    get:
      summary: List notes
      description: |-
        Fetches multiple note records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.notes.json.get
      x-api-path-slug: v2notes-json-get
      parameters:
      - in: query
        name: associated_with_id
        description: ID of the item with which the note is associated
      - in: query
        name: associated_with_type
        description: Case insensitive type of item with which the note is associated
      - in: query
        name: ids
        description: IDs of notes to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Notes
    post:
      summary: Create a note
      description: Creates a note.
      operationId: v2.notes.json.post
      x-api-path-slug: v2notes-json-post
      parameters:
      - in: formData
        name: associated_with_id
        description: ID of the item with which the note is associated
      - in: formData
        name: associated_with_type
        description: Case insensitive type of item with which the note is associated
      - in: formData
        name: call_id
        description: ID of the call with which the note is associated
      - in: formData
        name: content
        description: The content of the note
      - in: formData
        name: skip_crm_sync
        description: Boolean indicating if the CRM sync should be skipped
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Note
  /v2/notes/{id}.json:
    get:
      summary: Fetch a note
      description: Fetches a note, by ID only.
      operationId: v2.notes.id.json.get
      x-api-path-slug: v2notesid-json-get
      parameters:
      - in: path
        name: id
        description: Note ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Note
    put:
      summary: Update a note
      description: Updates a note. Any changes to the note or associated records will
        not reflect in Salesforce.com.
      operationId: v2.notes.id.json.put
      x-api-path-slug: v2notesid-json-put
      parameters:
      - in: formData
        name: call_id
        description: ID of the call with which the note is associated
      - in: formData
        name: content
        description: The content of the note
      - in: path
        name: id
        description: Note ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Note
  /v2/people.json:
    get:
      summary: List people
      description: |-
        Fetches multiple person records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.people.json.get
      x-api-path-slug: v2people-json-get
      parameters:
      - in: query
        name: email_addresses
        description: Filters people by email address
      - in: query
        name: ids
        description: IDs of people to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, last_contacted_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - People
    post:
      summary: Create a person
      description: |-
        Creates a person. Either email_address or phone/last_name must be provided as a unique lookup
        on the team.
      operationId: v2.people.json.post
      x-api-path-slug: v2people-json-post
      parameters:
      - in: formData
        name: account_id
        description: ID of the Account to link this person to
      - in: formData
        name: autotag_date
        description: Whether the date should be added to this person as a tag
      - in: formData
        name: city
        description: City
      - in: formData
        name: country
        description: Country
      - in: formData
        name: custom_fields
        description: Custom fields are defined by the users team
      - in: formData
        name: do_not_contact
        description: Whether this person can not be contacted
      - in: formData
        name: email_address
        description: Email address
      - in: formData
        name: first_name
        description: First name
      - in: formData
        name: home_phone
        description: Home phone without formatting
      - in: formData
        name: import_id
        description: ID of the Import this person is a part of
      - in: formData
        name: last_name
        description: Last name
      - in: formData
        name: linkedin_url
        description: Linkedin URL
      - in: formData
        name: locale
        description: Time locale of the person
      - in: formData
        name: mobile_phone
        description: Mobile phone without formatting
      - in: formData
        name: owner_id
        description: ID of the User that owns this person
      - in: formData
        name: personal_email_address
        description: Personal email address
      - in: formData
        name: personal_website
        description: The website of this person
      - in: formData
        name: person_company_industry
        description: Company industry
      - in: formData
        name: person_company_name
        description: Company name
      - in: formData
        name: person_company_website
        description: Company website
      - in: formData
        name: person_stage_id
        description: ID of the PersonStage of this person
      - in: formData
        name: phone
        description: Phone without formatting
      - in: formData
        name: phone_extension
        description: Phone extension without formatting
      - in: formData
        name: secondary_email_address
        description: Alternate email address
      - in: formData
        name: state
        description: State
      - in: formData
        name: tags
        description: All tags applied to this person
      - in: formData
        name: title
        description: Job title
      - in: formData
        name: twitter_handle
        description: The twitter handle of this person
      - in: formData
        name: work_city
        description: Work location - city
      - in: formData
        name: work_country
        description: Work location - country
      - in: formData
        name: work_state
        description: Work location - state
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Person
  /v2/people/{id}.json:
    delete:
      summary: Delete a person
      description: |-
        Deletes a person. This operation is not reversible without contacting support.
        This operation can be called multiple times successfully.
      operationId: v2.people.id.json.delete
      x-api-path-slug: v2peopleid-json-delete
      parameters:
      - in: path
        name: id
        description: Person id
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Person
    get:
      summary: Fetch a person
      description: Fetches a person, by ID only.
      operationId: v2.people.id.json.get
      x-api-path-slug: v2peopleid-json-get
      parameters:
      - in: path
        name: id
        description: Person ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Person
    put:
      summary: Update a person
      description: Updates a person.
      operationId: v2.people.id.json.put
      x-api-path-slug: v2peopleid-json-put
      parameters:
      - in: formData
        name: account_id
        description: ID of the Account to link this person to
      - in: formData
        name: city
        description: City
      - in: formData
        name: country
        description: Country
      - in: formData
        name: custom_fields
        description: Custom fields are defined by the users team
      - in: formData
        name: do_not_contact
        description: Whether this person can not be contacted
      - in: formData
        name: email_address
        description: Email address
      - in: formData
        name: first_name
        description: First name
      - in: formData
        name: home_phone
        description: Home phone without formatting
      - in: path
        name: id
        description: Person id
      - in: formData
        name: import_id
        description: ID of the Import this person is a part of
      - in: formData
        name: last_name
        description: Last name
      - in: formData
        name: linkedin_url
        description: Linkedin URL
      - in: formData
        name: locale
        description: Time locale of the person
      - in: formData
        name: mobile_phone
        description: Mobile phone without formatting
      - in: formData
        name: owner_id
        description: ID of the User that owns this person
      - in: formData
        name: personal_email_address
        description: Personal email address
      - in: formData
        name: personal_website
        description: The website of this person
      - in: formData
        name: person_company_industry
        description: Company industry
      - in: formData
        name: person_company_name
        description: Company name
      - in: formData
        name: person_company_website
        description: Company website
      - in: formData
        name: person_stage_id
        description: ID of the PersonStage of this person
      - in: formData
        name: phone
        description: Phone without formatting
      - in: formData
        name: phone_extension
        description: Phone extension without formatting
      - in: formData
        name: secondary_email_address
        description: Alternate email address
      - in: formData
        name: state
        description: State
      - in: formData
        name: tags
        description: All tags applied to this person
      - in: formData
        name: title
        description: Job title
      - in: formData
        name: twitter_handle
        description: The twitter handle of this person
      - in: formData
        name: work_city
        description: Work location - city
      - in: formData
        name: work_country
        description: Work location - country
      - in: formData
        name: work_state
        description: Work location - state
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Person
  /v2/person_stages.json:
    get:
      summary: List person stages
      description: |-
        Fetches multiple person stage records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.person_stages.json.get
      x-api-path-slug: v2person-stages-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of person stages to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Person
      - Stages
    post:
      summary: Create a person stage
      description: Creates a person stage.
      operationId: v2.person_stages.json.post
      x-api-path-slug: v2person-stages-json-post
      parameters:
      - in: formData
        name: name
        description: The name of the new stage
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Person
      - Stage
  /v2/person_stages/{id}.json:
    delete:
      summary: Delete an person stage
      description: |-
        Deletes a person stage. This operation is not reversible without contacting support.
        This operation can be called multiple times successfully.
      operationId: v2.person_stages.id.json.delete
      x-api-path-slug: v2person-stagesid-json-delete
      parameters:
      - in: path
        name: id
        description: Stage ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Person
      - Stage
    get:
      summary: Fetch a person stage
      description: Fetches a person stage, by ID only.
      operationId: v2.person_stages.id.json.get
      x-api-path-slug: v2person-stagesid-json-get
      parameters:
      - in: path
        name: id
        description: Stage ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Person
      - Stage
    put:
      summary: Update a person stage
      description: Updates a person stage.
      operationId: v2.person_stages.id.json.put
      x-api-path-slug: v2person-stagesid-json-put
      parameters:
      - in: path
        name: id
        description: Stage ID
      - in: formData
        name: name
        description: The name of the stage
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Person
      - Stage
  /v2/phone_numbers/caller_ids.json:
    get:
      summary: List caller ids
      description: |-
        Each entry is a possible caller ID match for the number. Multiple
        entries may be returned if the phone number is present on more than one
        person in the system.  Phone number should be in E.164 format.
      operationId: v2.phone_numbers.caller_ids.json.get
      x-api-path-slug: v2phone-numberscaller-ids-json-get
      parameters:
      - in: query
        name: phone_number
        description: E
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Caller
      - Ids
  /v2/phone_numbers/recording_settings/{id}.json:
    get:
      summary: Fetch recording setting
      description: |-
        Fetches the recording status for a given phone number, based on Do Not Record and Recording Governance for your team.
        Phone number should be in E.164 format.
      operationId: v2.phone_numbers.recording_settings.id.json.get
      x-api-path-slug: v2phone-numbersrecording-settingsid-json-get
      parameters:
      - in: path
        name: id
        description: E
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Recording
      - Setting
  /v2/steps.json:
    get:
      summary: List steps
      description: |-
        Fetches multiple step records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.steps.json.get
      x-api-path-slug: v2steps-json-get
      parameters:
      - in: query
        name: cadence_id
        description: Filter by cadence ID
      - in: query
        name: has_due_actions
        description: Filter by whether a step has due actions
      - in: query
        name: ids
        description: IDs of steps to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: type
        description: Filter by step type
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Steps
  /v2/steps/{id}.json:
    get:
      summary: Fetch a step
      description: Fetches a step, by ID only.
      operationId: v2.steps.id.json.get
      x-api-path-slug: v2stepsid-json-get
      parameters:
      - in: path
        name: id
        description: Step ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Step
  /v2/successes.json:
    get:
      summary: List successes
      description: |-
        Fetches multiple success records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.successes.json.get
      x-api-path-slug: v2successes-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of successes to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, succeeded_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Successes
  /v2/team.json:
    get:
      summary: Fetch current team
      description: Fetches the team of the authenticated user.
      operationId: v2.team.json.get
      x-api-path-slug: v2team-json-get
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Current
      - Team
  /v2/team_templates.json:
    get:
      summary: List team templates
      description: |-
        Fetches multiple team template records. The records can be filtered, paged, and sorted according to
        the respective parameters.

        Team templates are templates that are available team-wide. Admins may use
        team templates to create original content for the entire team, monitor version control to ensure templates are always up to date,
        and track template performance across the entire organization. All metrics on a team template reflect usage across the team; individual metrics can be found with the email_templates API endpoint.
      operationId: v2.team_templates.json.get
      x-api-path-slug: v2team-templates-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of team templates to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, last_used_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Team
      - Templates
  /v2/team_templates/{id}.json:
    get:
      summary: Fetch a team template
      description: Fetches a team template, by ID only.
      operationId: v2.team_templates.id.json.get
      x-api-path-slug: v2team-templatesid-json-get
      parameters:
      - in: path
        name: id
        description: Team Template ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Team
      - Template
  /v2/users.json:
    get:
      summary: List users
      description: |-
        Non Admin: Lists only your user, or all on team depending on group visibility policy
        Team Admin: Lists users associated with your team
      operationId: v2.users.json.get
      x-api-path-slug: v2users-json-get
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Users
  /v2/users/{id}.json:
    get:
      summary: Fetch a user
      description: Fetches a user, by ID only.
      operationId: v2.users.id.json.get
      x-api-path-slug: v2usersid-json-get
      parameters:
      - in: path
        name: id
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - User