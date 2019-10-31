swagger: "2.0"
x-collection-name: Learnifier
x-complete: 1
info:
  title: Learnifier
  version: 1.1.0
host: learnifier.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /coursedesigns:
    get:
      summary: Lists all global course design templates
      description: Lists all global course design templates. Only api callers that
        have full access can call this method.
      operationId: coursedesigns.get
      x-api-path-slug: coursedesigns-get
      responses:
        200:
          description: OK
      tags:
      - Courses
  /extorgunit:
    get:
      summary: Get Organization Unit with External Id
      description: Returns information about the organization unit with the specified
        external id.
      operationId: extorgunit.get
      x-api-path-slug: extorgunit-get
      parameters:
      - in: query
        name: extid
        description: The external id of the organization unit
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /extparticipation:
    get:
      summary: Gets a participation by external id
      description: Gets a participation by external id.
      operationId: extparticipation.get
      x-api-path-slug: extparticipation-get
      parameters:
      - in: query
        name: extid
        description: The external id of the participation
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Participation
  /extproject:
    get:
      summary: Gets Organization Unit by external id
      description: Gets an Organization Unit by external id
      operationId: extproject.get
      x-api-path-slug: extproject-get
      parameters:
      - in: query
        name: extid
        description: The external id of the organization unit
      responses:
        200:
          description: OK
      tags:
      - Projects
  /extuser:
    get:
      summary: Gets a user by external id
      description: Gets a user by external id.
      operationId: extuser.get
      x-api-path-slug: extuser-get
      parameters:
      - in: query
        name: extid
        description: The external id of the user
      responses:
        200:
          description: OK
      tags:
      - Users
  /globalusergroups:
    get:
      summary: List Global User Groups.
      description: Returns a list of Global User Groups. Global User Groups are set
        up for the realm, and will generate groups that can be used on the client
        level.
      operationId: globalusergroups.get
      x-api-path-slug: globalusergroups-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /globalusergroups/{groupid}/members:
    get:
      summary: List of all users in group.
      description: Returns a list of all members in User Groups that are based on
        the Global Group with this groupid.
      operationId: globalusergroups.groupid.members.get
      x-api-path-slug: globalusergroupsgroupidmembers-get
      parameters:
      - in: path
        name: groupid
        description: ID of group
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /orgunits:
    get:
      summary: Organization Units
      description: |-
        The orgunits endpoint returns information about the available organization units (orgunits).
        The response includes the display name, internal and external id and client number.
      operationId: orgunits.get
      x-api-path-slug: orgunits-get
      responses:
        200:
          description: OK
      tags:
      - Organizations
    post:
      summary: Adds an Organization Unit
      description: Adds an Organization Unit
      operationId: orgunits.post
      x-api-path-slug: orgunits-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /orgunits/{orgid}:
    get:
      summary: Get Organization Unit
      description: |-
        Returns information about the specified organization unit.
        The response includes the display name, internal and external id and client number.
      operationId: orgunits.orgid.get
      x-api-path-slug: orgunitsorgid-get
      parameters:
      - in: path
        name: orgid
        description: Id of the organization unit
      responses:
        200:
          description: OK
      tags:
      - Organizations
    patch:
      summary: Updates an Organization Unit
      description: Adds an Organization Unit
      operationId: orgunits.orgid.patch
      x-api-path-slug: orgunitsorgid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orgid
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /orgunits/{orgid}/projects:
    get:
      summary: Organization Unit Projects
      description: Returns the available projects for the organization unit
      operationId: orgunits.orgid.projects.get
      x-api-path-slug: orgunitsorgidprojects-get
      parameters:
      - in: path
        name: orgid
        description: Id of the organization unit
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Projects
    post:
      summary: Create project
      description: Creates a new project
      operationId: orgunits.orgid.projects.post
      x-api-path-slug: orgunitsorgidprojects-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orgid
        description: Id of the organization unit
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Projects
  /orgunits/{orgid}/projects/{projectid}:
    delete:
      summary: Deletes the project
      description: Deletes the project. The project can only be deleted if the project
        do not contain any participants.
      operationId: orgunits.orgid.projects.projectid.delete
      x-api-path-slug: orgunitsorgidprojectsprojectid-delete
      parameters:
      - in: path
        name: orgid
        description: Id of the organization unit
      - in: path
        name: projectid
        description: Id of the project
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Projects
      - Projectid
    get:
      summary: Project information
      description: Returns project information
      operationId: orgunits.orgid.projects.projectid.get
      x-api-path-slug: orgunitsorgidprojectsprojectid-get
      parameters:
      - in: path
        name: orgid
        description: Id of the organization unit
      - in: path
        name: projectid
        description: Id of the project
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Projects
      - Projectid
    patch:
      summary: Update project information
      description: Updates information about a project. Values are only updated if
        the fields are specified in the input
      operationId: orgunits.orgid.projects.projectid.patch
      x-api-path-slug: orgunitsorgidprojectsprojectid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orgid
        description: Id of the organization unit
      - in: path
        name: projectid
        description: Id of the project
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Projects
      - Projectid
  /orgunits/{orgid}/projects/{projectid}/participants:
    get:
      summary: Project participants
      description: Returns project participants
      operationId: orgunits.orgid.projects.projectid.participants.get
      x-api-path-slug: orgunitsorgidprojectsprojectidparticipants-get
      parameters:
      - in: path
        name: orgid
        description: Id of the organization unit
      - in: path
        name: projectid
        description: Id of the project
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Projects
      - Projectid
      - Participants
    post:
      summary: Add participant
      description: Add a user to the project. Participant information is created for
        the user. In the body object, only one of either email or userid must be specified.
        The participant needs to be activated before it the user can access it.
      operationId: orgunits.orgid.projects.projectid.participants.post
      x-api-path-slug: orgunitsorgidprojectsprojectidparticipants-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orgid
        description: Id of the organization unit
      - in: path
        name: projectid
        description: Id of the project
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Projects
      - Projectid
      - Participants
  /orgunits/{orgid}/projects/{projectid}/participants/${participantId}:
    delete:
      summary: Deletes a participant
      description: "Deletes a participant. The user itself will still remain but any
        state related to the project will be deleted. \nIt might not be possible due
        to constraints from the products in the project to delete the participant.
        However\nthis can only be determined at the time of the delete. If a delete
        fails the participant will have their inError\nflag set."
      operationId: orgunits.orgid.projects.projectid.participants._participantId.delete
      x-api-path-slug: orgunitsorgidprojectsprojectidparticipantsparticipantid-delete
      parameters:
      - in: path
        name: orgid
        description: Id of the organization unit
      - in: path
        name: participantId
        description: Participant id
      - in: path
        name: projectid
        description: Id of the project
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Projects
      - Projectid
      - Participants
      - $participantId
  /orgunits/{orgid}/projects/{projectid}/participants/${participantId}/activate:
    post:
      summary: Activate participant
      description: Activates a participant so that it can be used
      operationId: orgunits.orgid.projects.projectid.participants._participantId.activate.post
      x-api-path-slug: orgunitsorgidprojectsprojectidparticipantsparticipantidactivate-post
      parameters:
      - in: path
        name: orgid
        description: Id of the organization unit
      - in: path
        name: participantId
        description: Id of the participant
      - in: path
        name: projectid
        description: Id of the project
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Projects
      - Projectid
      - Participants
      - $participantId
      - Activate
  /orgunits/{orgid}/projects/{projectid}/participants/${participantId}/loginlink:
    post:
      summary: Participant login link
      description: |-
        Returns a single sign on link for the participant. The link is only usable once and should be used directly. The link expires after a few minutes.

        This operation requires the *login link* permission.
      operationId: orgunits.orgid.projects.projectid.participants._participantId.loginlink.post
      x-api-path-slug: orgunitsorgidprojectsprojectidparticipantsparticipantidloginlink-post
      parameters:
      - in: path
        name: orgid
        description: Id of the organization unit
      - in: path
        name: participantId
        description: Id of the participant
      - in: path
        name: projectid
        description: Id of the project
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Projects
      - Projectid
      - Participants
      - $participantId
      - Loginlink
  /orgunits/{orgid}/projects/{projectid}/teammembers:
    get:
      summary: Project team members
      description: Returns the project team members. A team member is a ....
      operationId: orgunits.orgid.projects.projectid.teammembers.get
      x-api-path-slug: orgunitsorgidprojectsprojectidteammembers-get
      parameters:
      - in: path
        name: orgid
        description: Id of the organization unit
      - in: path
        name: projectid
        description: Id of the project
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Projects
      - Projectid
      - Team
      - Members
  /orgunits/{orgid}/usergroups:
    get:
      summary: List User Groups.
      description: Returns a list of User Groups for the org unit.
      operationId: orgunits.orgid.usergroups.get
      x-api-path-slug: orgunitsorgidusergroups-get
      parameters:
      - in: path
        name: orgid
        description: ID of organization
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Users
      - Groups
    post:
      summary: Create a User Group.
      description: Create a User Group.
      operationId: orgunits.orgid.usergroups.post
      x-api-path-slug: orgunitsorgidusergroups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orgid
        description: ID of organization
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Users
      - Groups
  /orgunits/{orgid}/usergroups/{groupid}:
    get:
      summary: Get user group
      description: Returns single User Group.
      operationId: orgunits.orgid.usergroups.groupid.get
      x-api-path-slug: orgunitsorgidusergroupsgroupid-get
      parameters:
      - in: path
        name: groupid
        description: ID of group
      - in: path
        name: orgid
        description: ID of organization
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Users
      - Groups
      - Groupid
  /orgunits/{orgid}/usergroups/{groupid}/members:
    get:
      summary: List of all users in group.
      description: Returns a list of all members in User Groups that are based on
        the Global Group with this groupid.
      operationId: orgunits.orgid.usergroups.groupid.members.get
      x-api-path-slug: orgunitsorgidusergroupsgroupidmembers-get
      parameters:
      - in: path
        name: groupid
        description: ID of group
      - in: path
        name: orgid
        description: ID of organization
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Uses
      - Groups
      - Members
    post:
      summary: Add user group member.
      description: Adds a user to user group.
      operationId: orgunits.orgid.usergroups.groupid.members.post
      x-api-path-slug: orgunitsorgidusergroupsgroupidmembers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupid
        description: ID of group
      - in: path
        name: orgid
        description: ID of organization
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Uses
      - Groups
      - Members
  /orgunits/{orgid}/usergroups/{groupid}/members/{uuid}:
    delete:
      summary: Remove user group member.
      description: Removes a user from a user group.
      operationId: orgunits.orgid.usergroups.groupid.members.uuid.delete
      x-api-path-slug: orgunitsorgidusergroupsgroupidmembersuuid-delete
      parameters:
      - in: path
        name: groupid
        description: ID of group
      - in: path
        name: orgid
        description: ID of organization
      - in: path
        name: uuid
        description: UUID of user to remove from group
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Uses
      - Groups
      - Members
  /users:
    get:
      summary: Lists all users
      description: Lists all users. Only api callers that have full access can call
        this method.
      operationId: users.get
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of users to return
      - in: query
        name: offset
        description: The offset to start listing users from
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Adds a user
      description: Adds a user. No two users can have the same email address. Email
        is saved WITH case but compared regardless of case. Email can be changed for
        a user assuming it doesn't cause a conflict.
      operationId: users.post
      x-api-path-slug: users-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{userid}:
    get:
      summary: User information
      description: Returns information about a user
      operationId: users.userid.get
      x-api-path-slug: usersuserid-get
      parameters:
      - in: path
        name: userid
        description: A user id
      responses:
        200:
          description: OK
      tags:
      - Users
    patch:
      summary: Updates user information
      description: Updates a user. All values that have a key defined in the input
        will be set. So if a value should not be updated omit it totally from the
        input, otherwise it will be unset.
      operationId: users.userid.patch
      x-api-path-slug: usersuserid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userid
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{userid}/pic?key={APIKEY}:
    get:
      summary: User profile picture
      description: |-
        Returns a thumbnail picture of the user. This can either be a selected picture or an auto generated image. This method doesn't require a full sign in. The api key is sufficient.
        The image is square and is likely, but not necessary, to be in 128x128 PNG format. However the format will always be either PNG, JPEG or GIF.
      operationId: users.userid.pic_key_APIKEY.get
      x-api-path-slug: usersuseridpickeyapikey-get
      parameters:
      - in: path
        name: APIKEY
      - in: path
        name: userid
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{userid}/projectParticipations:
    get:
      summary: Returns information about the projects the user is a participant in.
      description: Returns information about the projects the user is a participant
        in. Only the projects that the current token have access to will be listed.
      operationId: users.userid.projectParticipations.get
      x-api-path-slug: usersuseridprojectparticipations-get
      parameters:
      - in: path
        name: userid
        description: A user id
      responses:
        200:
          description: OK
      tags:
      - Users