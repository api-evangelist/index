swagger: "2.0"
x-collection-name: Automox
x-complete: 1
info:
  title: Automox API
  description: the-automox-api-is-a-powerful-interface-that-allows-you-to-integrate-automox-reporting-data-into-you-applications-and-control-the-various-settings-of-your-account-all-endpoints-are-only-accessible-via-https-and-are-located-atapi-automox-com--for-instance-you-can-see-events-associated-with-your-account-by-accessing-the-following-url-with-your-idreplace-apikey-with-your-own--httpsconsole-automox-comapieventsapi-keyapikey-limitsbe-nice--if-youre-sending-too-many-requests-too-quickly-well-send-back-a429-error-code-too-many-requests-you-are-limited-to-5000-requests-per-hour-per-api-key-overall--practically-this-means-you-should-when-possible-authenticateusers-so-that-limits-are-well-outside-the-reach-of-a-given-user-
  termsOfService: https://www.automox.com/
  contact:
    name: support@automox.com
  version: 1.0.0
host: console.automox.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events:
    get:
      summary: Get Events
      description: Gets all `Event` objects for the authenticated user.
      operationId: gets-all-event-objects-for-the-authenticated-user
      x-api-path-slug: events-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /events/{id}:
    get:
      summary: Get Events
      description: Gets a specific `Event` object for the authenticated user.
      operationId: gets-a-specific-event-object-for-the-authenticated-user
      x-api-path-slug: eventsid-get
      parameters:
      - in: path
        name: id
        description: event ID
      responses:
        200:
          description: OK
      tags:
      - Events
  /orgs:
    get:
      summary: Get Orgs
      description: Gets all organizations for the api key
      operationId: gets-all-organizations-for-the-api-key
      x-api-path-slug: orgs-get
      responses:
        200:
          description: OK
      tags:
      - Orgs
  /orgs/{id}/packages:
    get:
      summary: Get Orgs Packages
      description: Returns all software packages discovered on all servers (endpoints)
        of an organization
      operationId: returns-all-software-packages-discovered-on-all-servers-endpoints-of-an-organization
      x-api-path-slug: orgsidpackages-get
      parameters:
      - in: path
        name: id
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Orgs
      - Packages
  /policies:
    get:
      summary: Get Policies
      description: Gets all `Policy` objects for authenticated user
      operationId: gets-all-policy-objects-for-authenticated-user
      x-api-path-slug: policies-get
      parameters:
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Policies
  /policies/{id}:
    get:
      summary: Get Policies
      description: Gets a specific `Policy` object for the authenticated user.
      operationId: gets-a-specific-policy-object-for-the-authenticated-user
      x-api-path-slug: policiesid-get
      parameters:
      - in: path
        name: id
        description: Policy ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Policies
    put:
      summary: Put Policies
      description: Updates a `Policy` object
      operationId: updates-a-policy-object
      x-api-path-slug: policiesid-put
      parameters:
      - in: path
        name: id
        description: Policy ID
      - in: query
        name: o
        description: Organization ID
      - in: body
        name: policy
        description: Updated policy object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Policies
  /policies/{id}/action:
    post:
      summary: Post Policies Action
      description: Schedule a policy for immediate remediation
      operationId: schedule-a-policy-for-immediate-remediation
      x-api-path-slug: policiesidaction-post
      parameters:
      - in: formData
        name: action
        description: Remediation action type [remediateAll]
      - in: path
        name: id
        description: Policy ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Policies
      - Action
  /policysets:
    get:
      summary: Get Policysets
      description: Gets all `Policy Set` objects for authenticated user
      operationId: gets-all-policy-set-objects-for-authenticated-user
      x-api-path-slug: policysets-get
      parameters:
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Policysets
  /policystats:
    get:
      summary: Get Policystats
      description: Gets all `Policy Stats` objects for authenticated user
      operationId: gets-all-policy-stats-objects-for-authenticated-user
      x-api-path-slug: policystats-get
      parameters:
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Policystats
  /servers:
    get:
      summary: Get Servers
      description: Gets all `Server` objects for authenticated user
      operationId: gets-all-server-objects-for-authenticated-user
      x-api-path-slug: servers-get
      parameters:
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
  /servers/{id}:
    get:
      summary: Get Servers
      description: Gets a specific `Server` object for the authenticated user.
      operationId: gets-a-specific-server-object-for-the-authenticated-user
      x-api-path-slug: serversid-get
      parameters:
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
    put:
      summary: Put Servers
      description: Updates a `Server` object
      operationId: updates-a-server-object
      x-api-path-slug: serversid-put
      parameters:
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      - in: body
        name: server
        description: Updated server object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Servers
    delete:
      summary: Delete Servers
      description: ""
      operationId: ""
      x-api-path-slug: serversid-delete
      parameters:
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
  /servers/{id}/packages:
    get:
      summary: Get Servers Packages
      description: Returns the command queue for the specified server (endpoint)
      operationId: returns-the-command-queue-for-the-specified-server-endpoint
      x-api-path-slug: serversidpackages-get
      parameters:
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
      - Packages
  /servers/{id}/queues:
    get:
      summary: Get Servers Queues
      description: Returns the command queue for the specified server (endpoint)
      operationId: returns-the-command-queue-for-the-specified-server-endpoint
      x-api-path-slug: serversidqueues-get
      parameters:
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
      - Queues
    post:
      summary: Post Servers Queues
      description: Issue a command to an endpoint. Can be used to install a specific
        set of patches or reboot an endpoint
      operationId: issue-a-command-to-an-endpoint-can-be-used-to-install-a-specific-set-of-patches-or-reboot-an-endpoin
      x-api-path-slug: serversidqueues-post
      parameters:
      - in: body
        name: command
        description: Command object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
      - Queues
  /servergroups:
    get:
      summary: Get Servergroups
      description: Gets all `Server Group` objects for authenticated user
      operationId: gets-all-server-group-objects-for-authenticated-user
      x-api-path-slug: servergroups-get
      parameters:
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servergroups
    post:
      summary: Post Servergroups
      description: Updates a `Server Group` object
      operationId: updates-a-server-group-object
      x-api-path-slug: servergroups-post
      parameters:
      - in: body
        name: servergroup
        description: Updated server object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Servergroups
  /servergroups/{id}:
    get:
      summary: Get Servergroups
      description: Gets a specific `Server Group` object for the authenticated user.
      operationId: gets-a-specific-server-group-object-for-the-authenticated-user
      x-api-path-slug: servergroupsid-get
      parameters:
      - in: path
        name: id
        description: Server Group ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servergroups
    put:
      summary: Put Servergroups
      description: Updates a `Server Group` object
      operationId: updates-a-server-group-object
      x-api-path-slug: servergroupsid-put
      parameters:
      - in: path
        name: id
        description: Server Group ID
      - in: query
        name: o
        description: Organization ID
      - in: body
        name: servergroup
        description: Updated server object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Servergroups
    delete:
      summary: Delete Servergroups
      description: ""
      operationId: ""
      x-api-path-slug: servergroupsid-delete
      parameters:
      - in: path
        name: id
        description: Server Group ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servergroups
  /software_version:
    get:
      summary: Get Software Version
      description: Retrieves software packages and patches for an organization, specific
        policy, or just those that need [approval | attention | exceptions | pending
        update].
      operationId: retrieves-software-packages-and-patches-for-an-organization-specific-policy-or-just-those-that-need-
      x-api-path-slug: software-version-get
      parameters:
      - in: query
        name: exceptions
        description: Retrieve software that applies to exception endpoints
      - in: query
        name: l
        description: Result Limit
      - in: query
        name: needsApproval
        description: Retrieve software that needs approval
      - in: query
        name: needsAttention
        description: Retrieve software that needs attention
      - in: query
        name: o
        description: Organization ID
      - in: query
        name: p
        description: Page Number
      - in: query
        name: pendingUpdate
        description: Retrieve software that is pending update
      - in: query
        name: policyId
        description: Return results for a specific Policy ID
      responses:
        200:
          description: OK
      tags:
      - Software
      - Version
  /software:
    get:
      summary: Get Software
      description: Retrieves software packages and patches for an organization, allows
        filtering the list of software by name
      operationId: retrieves-software-packages-and-patches-for-an-organization-allows-filtering-the-list-of-software-by
      x-api-path-slug: software-get
      parameters:
      - in: query
        name: groupID
        description: Return software for a given group ID
      - in: query
        name: limit
        description: Limit number of results returned
      - in: query
        name: name
        description: Name of software package (wildcards ok) i
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Software
  /approvals/{id}:
    put:
      summary: Put Approvals
      description: Update a manual approval record. Set `manual_approval` attribute
        of `approval` object to `true` to approve a patch; set it to `false` to reject
        a patch
      operationId: update-a-manual-approval-record-set-manual-approval-attribute-of-approval-object-to-true-to-approve-
      x-api-path-slug: approvalsid-put
      parameters:
      - in: body
        name: approval
        description: Approval object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Approval ID
      responses:
        200:
          description: OK
      tags:
      - Approvals
  /users:
    get:
      summary: Get Users
      description: Gets all `User` objects for the authenticated user.
      operationId: gets-all-user-objects-for-the-authenticated-user
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{id}/queues:
    get:
      summary: Get Users Queues
      description: Gets all commands executed for specified user id
      operationId: gets-all-commands-executed-for-specified-user-id
      x-api-path-slug: usersidqueues-get
      parameters:
      - in: path
        name: id
        description: User ID or `self` for current user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Queues
  /reports/prepatch:
    get:
      summary: Get Reports Prepatch
      description: Retrieve the prepatch report
      operationId: retrieve-the-prepatch-report
      x-api-path-slug: reportsprepatch-get
      parameters:
      - in: query
        name: startDate
        description: Report Start Date - `YYYY-MM-DD`
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Prepatch
  /reports/noncompliance:
    get:
      summary: Get Reports Noncompliance
      description: Retrieve the non compliant devices report
      operationId: retrieve-the-non-compliant-devices-report
      x-api-path-slug: reportsnoncompliance-get
      parameters:
      - in: query
        name: startDate
        description: Report Start Date - `YYYY-MM-DD`
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Noncompliance