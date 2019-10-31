swagger: "2.0"
x-collection-name: CollabNet
x-complete: 1
info:
  title: Foundation API
  version: 1.0.0
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /appconfiguration:
    patch:
      summary: Updates configuration properties
      description: Updates configuration properties.
      operationId: setConfigurations
      x-api-path-slug: appconfiguration-patch
      parameters:
      - in: body
        name: body
        description: List of configuration properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Configuration
      - Properties
  /appconfiguration/by-name/{configname}:
    get:
      summary: Get value for specified configuration property
      description: Get value for specified configuration property.
      operationId: getValueForSpecifiedConfigurationProperty
      x-api-path-slug: appconfigurationbynameconfigname-get
      parameters:
      - in: path
        name: configname
        description: configname
      responses:
        200:
          description: OK
      tags:
      - Valuespecified
      - Configuration
      - Property
  /appconfiguration/by-name/{configname}/value:
    patch:
      summary: Updates the configuration value
      description: Updates the configuration value.
      operationId: updateConfigurationValue
      x-api-path-slug: appconfigurationbynameconfignamevalue-patch
      parameters:
      - in: body
        name: body
        description: Update the configuration value
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: configname
        description: configname
      responses:
        200:
          description: OK
      tags:
      - Configuration
      - Value
  /approval-requests/summary:
    get:
      summary: Gets a summary of pending approval requests on TF server
      description: Gets a summary of pending approval requests on tf server.
      operationId: getApprovalRequestSummary
      x-api-path-slug: approvalrequestssummary-get
      parameters:
      - in: query
        name: projectId
        description: Project identifier
      responses:
        200:
          description: OK
      tags:
      - Summary
      - Of
      - Pending
      - Approval
      - Requests
      - "On"
      - TF
      - Server
  /associations:
    get:
      summary: Gets the association information for the given object/activity ids
      description: Gets the association information for the given object/activity
        ids.
      operationId: getAssociations
      x-api-path-slug: associations-get
      parameters:
      - in: query
        name: depth
        description: Number of levels
      - in: query
        name: ids
        description: Comma separated object ids
      - in: query
        name: includeDependencies
        description: Include dependency associations (parent and child)
      - in: query
        name: includeEvents
        description: Include events
      - in: query
        name: includePhantoms
        description: Include phantom events
      - in: query
        name: limit
        description: Maximum number of generic associations for an object
      responses:
        200:
          description: OK
      tags:
      - Association
      - Informationthe
      - Given
      - Object
      - Activitys
  /groups:
    get:
      summary: Gets paginated user group list
      description: Gets paginated user group list.
      operationId: getUserGroups
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
        description: Offset
      - in: query
        name: sortby
        description: Sort by column name
      responses:
        200:
          description: OK
      tags:
      - Paginated
      - User
      - Group
      - List
    post:
      summary: Creates user group
      description: Creates user group.
      operationId: createUserGroup
      x-api-path-slug: groups-post
      parameters:
      - in: body
        name: body
        description: New user group data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - User
      - Group
  /groups/by-name/{name}:
    get:
      summary: Gets group data by fullname
      description: Gets group data by fullname.
      operationId: getItemByName
      x-api-path-slug: groupsbynamename-get
      parameters:
      - in: path
        name: name
        description: Groups full name
      responses:
        200:
          description: OK
      tags:
      - Group
      - Data
      - By
      - Fullname
  /groups/{groupid}:
    get:
      summary: Gets group data by id
      description: Gets group data by id.
      operationId: getUserGroup
      x-api-path-slug: groupsgroupid-get
      parameters:
      - in: path
        name: groupid
      responses:
        200:
          description: OK
      tags:
      - Group
      - Data
      - By
    delete:
      summary: Deletes group data by id
      description: Deletes group data by id.
      operationId: deleteUserGroup
      x-api-path-slug: groupsgroupid-delete
      parameters:
      - in: path
        name: groupid
      responses:
        200:
          description: OK
      tags:
      - Group
      - Data
      - By
    patch:
      summary: Updates group data by id
      description: Updates group data by id.
      operationId: updateUserGroup
      x-api-path-slug: groupsgroupid-patch
      parameters:
      - in: body
        name: body
        description: Updated user group info
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupid
      - in: header
        name: If-Match
        description: Group version
      responses:
        200:
          description: OK
      tags:
      - Group
      - Data
      - By
  /groups/{groupid}/members:
    get:
      summary: Gets usergroup members
      description: Gets usergroup members.
      operationId: getUserGroupMembers
      x-api-path-slug: groupsgroupidmembers-get
      parameters:
      - in: path
        name: groupid
      responses:
        200:
          description: OK
      tags:
      - Usergroup
      - Members
  /groups/{groupid}/members/{username}:
    put:
      summary: Adds a user to usergroup
      description: Adds a user to usergroup.
      operationId: addUserGroupMember
      x-api-path-slug: groupsgroupidmembersusername-put
      parameters:
      - in: path
        name: groupid
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - Usergroup
    delete:
      summary: Removes a user from usergroup
      description: Removes a user from usergroup.
      operationId: removeUserGroupMember
      x-api-path-slug: groupsgroupidmembersusername-delete
      parameters:
      - in: path
        name: groupid
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Removes
      - User
      - From
      - Usergroup
  /integrationdata/by-objectid/{objectid}/by-name/{namespace}:
    get:
      summary: Gets integration data for an object by namespace name
      description: Gets integration data for an object by namespace name.
      operationId: getIntegrationDataByName
      x-api-path-slug: integrationdatabyobjectidobjectidbynamenamespace-get
      parameters:
      - in: query
        name: dataname
        description: Data name
      - in: path
        name: namespace
        description: Namespace name
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - Integration
      - Dataan
      - Object
      - By
      - Namespace
      - Name
    put:
      summary: Sets integration data for an object by namespace name
      description: Sets integration data for an object by namespace name.
      operationId: setIntegrationDataByName
      x-api-path-slug: integrationdatabyobjectidobjectidbynamenamespace-put
      parameters:
      - in: body
        name: body
        description: Integration data
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: createNamespace
        description: Create namespace if missing?
      - in: path
        name: namespace
        description: Namespace name
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Integration
      - Dataan
      - Object
      - By
      - Namespace
      - Name
    delete:
      summary: Removes integration data for an object by namespace name
      description: Removes integration data for an object by namespace name.
      operationId: removeIntegrationDataByName
      x-api-path-slug: integrationdatabyobjectidobjectidbynamenamespace-delete
      parameters:
      - in: query
        name: dataname
        description: Data name
      - in: path
        name: namespace
        description: Namespace name
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Integration
      - Dataan
      - Object
      - By
      - Namespace
      - Name
  /integrationdata/by-objectid/{objectid}/{namespaceid}:
    get:
      summary: Gets integration data for an object by namespace id
      description: Gets integration data for an object by namespace id.
      operationId: getIntegrationData
      x-api-path-slug: integrationdatabyobjectidobjectidnamespaceid-get
      parameters:
      - in: query
        name: dataname
        description: Data name
      - in: path
        name: namespaceid
        description: Namespace id
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - Integration
      - Dataan
      - Object
      - By
      - Namespace
    put:
      summary: Sets integration data for an object by namespace id
      description: Sets integration data for an object by namespace id.
      operationId: setIntegrationData
      x-api-path-slug: integrationdatabyobjectidobjectidnamespaceid-put
      parameters:
      - in: body
        name: body
        description: Integration data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaceid
        description: Namespace id
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Integration
      - Dataan
      - Object
      - By
      - Namespace
    delete:
      summary: Removes integration data for an object by namespace id
      description: Removes integration data for an object by namespace id.
      operationId: removeIntegrationData
      x-api-path-slug: integrationdatabyobjectidobjectidnamespaceid-delete
      parameters:
      - in: query
        name: dataname
        description: Data name
      - in: path
        name: namespaceid
        description: Namespace id
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Integration
      - Dataan
      - Object
      - By
      - Namespace
  /integrationdata/myself/by-name/{namespace}:
    get:
      summary: Gets integration data for current user by namespace name
      description: Gets integration data for current user by namespace name.
      operationId: getMyIntegrationDataByName
      x-api-path-slug: integrationdatamyselfbynamenamespace-get
      parameters:
      - in: query
        name: dataname
        description: Data name
      - in: path
        name: namespace
        description: Namespace name
      responses:
        200:
          description: OK
      tags:
      - Integration
      - Datacurrent
      - User
      - By
      - Namespace
      - Name
    put:
      summary: Sets integration data for current user by namespace name
      description: Sets integration data for current user by namespace name.
      operationId: setMyIntegrationDataByName
      x-api-path-slug: integrationdatamyselfbynamenamespace-put
      parameters:
      - in: body
        name: body
        description: Integration data
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: createNamespace
        description: Create namespace if missing?
      - in: path
        name: namespace
        description: Namespace name
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Integration
      - Datacurrent
      - User
      - By
      - Namespace
      - Name
    delete:
      summary: Removes integration data for current user by namespace name
      description: Removes integration data for current user by namespace name.
      operationId: removeMyIntegrationDataByName
      x-api-path-slug: integrationdatamyselfbynamenamespace-delete
      parameters:
      - in: query
        name: dataname
        description: Data name
      - in: path
        name: namespace
        description: Namespace name
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Integration
      - Datacurrent
      - User
      - By
      - Namespace
      - Name
  /integrationdata/myself/{namespaceid}:
    get:
      summary: Gets integration data for current user by namespace id
      description: Gets integration data for current user by namespace id.
      operationId: getMyIntegrationData
      x-api-path-slug: integrationdatamyselfnamespaceid-get
      parameters:
      - in: query
        name: dataname
        description: Data name
      - in: path
        name: namespaceid
        description: Namespace id
      responses:
        200:
          description: OK
      tags:
      - Integration
      - Datacurrent
      - User
      - By
      - Namespace
    put:
      summary: Sets integration data for current user by namespace id
      description: Sets integration data for current user by namespace id.
      operationId: setMyIntegrationData
      x-api-path-slug: integrationdatamyselfnamespaceid-put
      parameters:
      - in: body
        name: body
        description: Integration data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaceid
        description: Namespace id
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Integration
      - Datacurrent
      - User
      - By
      - Namespace
    delete:
      summary: Removes integration data for current user by namespace id
      description: Removes integration data for current user by namespace id.
      operationId: removeMyIntegrationData
      x-api-path-slug: integrationdatamyselfnamespaceid-delete
      parameters:
      - in: query
        name: dataname
        description: Data name
      - in: path
        name: namespaceid
        description: Namespace id
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Integration
      - Datacurrent
      - User
      - By
      - Namespace
  /integrationdata/namespaces:
    post:
      summary: Registers namespace
      description: Registers namespace.
      operationId: registerNamespace
      x-api-path-slug: integrationdatanamespaces-post
      parameters:
      - in: body
        name: body
        description: Namespace
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Registers
      - Namespace
  /integrationdata/namespaces/by-name/{namespace}:
    get:
      summary: Gets namespace info by name
      description: Gets namespace info by name.
      operationId: getNamespaceByName
      x-api-path-slug: integrationdatanamespacesbynamenamespace-get
      parameters:
      - in: path
        name: namespace
        description: Namespace name
      responses:
        200:
          description: OK
      tags:
      - Namespace
      - Info
      - By
      - Name
  /monitoring/objects/{objectid}/users:
    get:
      summary: Returns the list of monitoring users for the object(Folder/Item).
      description: Returns the list of monitoring users for the object(folder/item)..
      operationId: listUsersForObject
      x-api-path-slug: monitoringobjectsobjectidusers-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: path
        name: objectid
        description: Object id
      - in: query
        name: offset
        description: Offset
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Monitoring
      - Usersthe
      - Object(Folder
      - Item)
  /monitoring/users/by-username/{username}/objects:
    get:
      summary: Returns the list of monitoring items for the given username
      description: Returns the list of monitoring items for the given username.
      operationId: monitoringItemsForUsername
      x-api-path-slug: monitoringusersbyusernameusernameobjects-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
        description: Offset
      - in: query
        name: projectid
        description: Project Id
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Monitoring
      - Itemsthe
      - Given
      - Username
    post:
      summary: Monitors / Unmonitors the list of objects for the given username
      description: Monitors / unmonitors the list of objects for the given username.
      operationId: monitorOrUnmonitorObjectsByUsername
      x-api-path-slug: monitoringusersbyusernameusernameobjects-post
      parameters:
      - in: query
        name: action
        description: To perform action
      - in: body
        name: body
        description: Monitor / Unmonitor items
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Monitors
      - ""
      - ""
      - Unmonitors
      - List
      - Of
      - Objectsthe
      - Given
      - Username
  /monitoring/users/by-username/{username}/objects/{objectid}:
    get:
      summary: Monitoring the current object or not for the given username (true /
        false)
      description: Monitoring the current object or not for the given username (true
        / false).
      operationId: isObjectMonitoredByUsername
      x-api-path-slug: monitoringusersbyusernameusernameobjectsobjectid-get
      parameters:
      - in: path
        name: objectid
        description: Object id
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Current
      - Object
      - Notthe
      - Given
      - Username
      - (true
      - ""
      - ""
      - False)
    post:
      summary: Monitors the current object for the given username.
      description: Monitors the current object for the given username..
      operationId: monitorObjectByUsername
      x-api-path-slug: monitoringusersbyusernameusernameobjectsobjectid-post
      parameters:
      - in: path
        name: objectid
        description: Object id
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Monitors
      - Current
      - Objectthe
      - Given
      - Username
    delete:
      summary: UnMonitors the current object for the given username.
      description: Unmonitors the current object for the given username..
      operationId: unMonitorObjectByuser
      x-api-path-slug: monitoringusersbyusernameusernameobjectsobjectid-delete
      parameters:
      - in: path
        name: objectid
        description: Object id
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - UnMonitors
      - Current
      - Objectthe
      - Given
      - Username
  /monitoring/users/myself/objects:
    get:
      summary: Returns the list of monitoring items for current user
      description: Returns the list of monitoring items for current user.
      operationId: monitoringItemsForUser
      x-api-path-slug: monitoringusersmyselfobjects-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
        description: Offset
      - in: query
        name: projectid
        description: Project id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Monitoring
      - Itemscurrent
      - User
    post:
      summary: Monitors / Unmonitors the list of objects for current user.
      description: Monitors / unmonitors the list of objects for current user..
      operationId: monitorOrUnmonitorObjectsForUser
      x-api-path-slug: monitoringusersmyselfobjects-post
      parameters:
      - in: query
        name: action
        description: To perform action
      - in: body
        name: body
        description: Monitor / Unmonitor items
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitors
      - ""
      - ""
      - Unmonitors
      - List
      - Of
      - Objectscurrent
      - User
  /monitoring/users/myself/objects/{objectid}:
    get:
      summary: The logged in user is monitoring the current object or not (true /
        false)
      description: The logged in user is monitoring the current object or not (true
        / false).
      operationId: isObjectMonitored
      x-api-path-slug: monitoringusersmyselfobjectsobjectid-get
      parameters:
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - The
      - Logged
      - In
      - User
      - Is
      - Monitoring
      - Current
      - Object
      - Not
      - (true
      - ""
      - ""
      - False)
    post:
      summary: Monitors the current object for current user.
      description: Monitors the current object for current user..
      operationId: monitorObjectForUser
      x-api-path-slug: monitoringusersmyselfobjectsobjectid-post
      parameters:
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - Monitors
      - Current
      - Objectcurrent
      - User
    delete:
      summary: UnMonitors the current object for the current user,
      description: Unmonitors the current object for the current user,.
      operationId: unMonitorObject
      x-api-path-slug: monitoringusersmyselfobjectsobjectid-delete
      parameters:
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - UnMonitors
      - Current
      - Objectthe
      - Current
      - User
      - ""
  /monitoring/users/{userid}/objects:
    get:
      summary: Returns the list of monitoring items for the given userid
      description: Returns the list of monitoring items for the given userid.
      operationId: monitorSubforUserId
      x-api-path-slug: monitoringusersuseridobjects-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
        description: Offset
      - in: query
        name: projectid
        description: Project Id
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Monitoring
      - Itemsthe
      - Given
      - Userid
    post:
      summary: Monitors / Unmonitors the list of objects for the given userid.
      description: Monitors / unmonitors the list of objects for the given userid..
      operationId: monitorOrUnmonitorObjectsByUserid
      x-api-path-slug: monitoringusersuseridobjects-post
      parameters:
      - in: query
        name: action
        description: To perform action
      - in: body
        name: body
        description: Monitor / Unmonitor items
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - Monitors
      - ""
      - ""
      - Unmonitors
      - List
      - Of
      - Objectsthe
      - Given
      - Userid
  /monitoring/users/{userid}/objects/{objectid}:
    get:
      summary: Monitoring the current object or not for the given user id (true /
        false)
      description: Monitoring the current object or not for the given user id (true
        / false).
      operationId: isObjectMonitoredByUserid
      x-api-path-slug: monitoringusersuseridobjectsobjectid-get
      parameters:
      - in: path
        name: objectid
        description: Object id
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Current
      - Object
      - Notthe
      - Given
      - User
      - (true
      - ""
      - ""
      - False)
    post:
      summary: Monitors the current object for the given userid.
      description: Monitors the current object for the given userid..
      operationId: monitorObjectByUserid
      x-api-path-slug: monitoringusersuseridobjectsobjectid-post
      parameters:
      - in: path
        name: objectid
        description: Object id
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - Monitors
      - Current
      - Objectthe
      - Given
      - Userid
    delete:
      summary: UnMonitors the current object for given userid
      description: Unmonitors the current object for given userid.
      operationId: unMonitorObjectByid
      x-api-path-slug: monitoringusersuseridobjectsobjectid-delete
      parameters:
      - in: path
        name: objectid
        description: Object id
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - UnMonitors
      - Current
      - Objectgiven
      - Userid
  /myself/recent/objects:
    get:
      summary: Gets recent object list for the current user
      description: Gets recent object list for the current user.
      operationId: getMyRecentObjects
      x-api-path-slug: myselfrecentobjects-get
      parameters:
      - in: query
        name: count
        description: Max
      responses:
        200:
          description: OK
      tags:
      - Recent
      - Object
      - Listthe
      - Current
      - User
  /myself/recent/projects:
    get:
      summary: Gets recent project list for the current user
      description: Gets recent project list for the current user.
      operationId: getMyRecentProjects
      x-api-path-slug: myselfrecentprojects-get
      parameters:
      - in: query
        name: count
        description: Max
      responses:
        200:
          description: OK
      tags:
      - Recent
      - Project
      - Listthe
      - Current
      - User
  /objects/{artifactId}/comments/{commentId}/edit:
    post:
      summary: Edit a comment added by the same user, on the given artifact id
      description: Edit a comment added by the same user, on the given artifact id.
      operationId: editComment
      x-api-path-slug: objectsartifactidcommentscommentidedit-post
      parameters:
      - in: path
        name: artifactId
        description: Artifact id
      - in: body
        name: body
        description: Comment
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: commentId
        description: Comment id
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Comment
      - Added
      - By
      - Same
      - User
      - ""
      - "On"
      - Given
      - Artifact
  /objects/{objectid}/associations:
    get:
      summary: Gets the association information for the given object id
      description: Gets the association information for the given object id.
      operationId: getObjectAssociations
      x-api-path-slug: objectsobjectidassociations-get
      parameters:
      - in: query
        name: depth
        description: Number of levels
      - in: query
        name: includeDependencies
        description: Include dependency associations (parent and child)
      - in: query
        name: includeEvents
        description: Include events
      - in: query
        name: includePhantoms
        description: Include phantom events
      - in: query
        name: limit
        description: Maximum number of generic associations for an object
      - in: path
        name: objectid
        description: Object/Activity id
      responses:
        200:
          description: OK
      tags:
      - Association
      - Informationthe
      - Given
      - Object
  /objects/{objectid}/associations/{targetid}:
    put:
      summary: Creates association
      description: Creates association.
      operationId: createAssociation
      x-api-path-slug: objectsobjectidassociationstargetid-put
      parameters:
      - in: body
        name: body
        description: Association parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: objectid
        description: Origin object id
      - in: path
        name: targetid
        description: Target object id
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Association
    delete:
      summary: Deletes association
      description: Deletes association.
      operationId: deleteAssociation
      x-api-path-slug: objectsobjectidassociationstargetid-delete
      parameters:
      - in: path
        name: objectid
        description: Origin object id
      - in: path
        name: targetid
        description: Target object id
      responses:
        200:
          description: OK
      tags:
      - Association
  /objects/{objectid}/auditlog:
    get:
      summary: Gets a collection of audit transactions performed on the specified
        TeamForge object
      description: Gets a collection of audit transactions performed on the specified
        teamforge object.
      operationId: getAuditLog
      x-api-path-slug: objectsobjectidauditlog-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: path
        name: objectid
        description: Object identifier
      - in: query
        name: offset
        description: Offset
      responses:
        200:
          description: OK
      tags:
      - Collection
      - Of
      - Audit
      - Transactions
      - Performed
      - "On"
      - Specified
      - TeamForge
      - Object
  /objects/{objectid}/comments:
    get:
      summary: Gets the comments on the given object id
      description: Gets the comments on the given object id.
      operationId: getObjectComments
      x-api-path-slug: objectsobjectidcomments-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: path
        name: objectid
        description: Object id
      - in: query
        name: offset
        description: Offset
      - in: query
        name: sortby
        description: Sort by column name
      responses:
        200:
          description: OK
      tags:
      - Comments
      - "On"
      - Given
      - Object
    post:
      summary: Posts a comment on the given object id
      description: Posts a comment on the given object id.
      operationId: postComment
      x-api-path-slug: objectsobjectidcomments-post
      parameters:
      - in: body
        name: body
        description: Comment
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - Comment
      - "On"
      - Given
      - Object
  /objects/{objectid}/delivery:
    get:
      summary: Gets delivery information for the given object
      description: Gets delivery information for the given object.
      operationId: getObjectDeliveryInfo
      x-api-path-slug: objectsobjectiddelivery-get
      parameters:
      - in: path
        name: objectid
        description: Object id(commit or artifact)
      responses:
        200:
          description: OK
      tags:
      - Delivery
      - Informationthe
      - Given
      - Object
  /permission/{projectid}/{folderPath}/baseline:
    get:
      summary: Check Baseline Permission for given project
      description: Check baseline permission for given project.
      operationId: check baseline permission
      x-api-path-slug: permissionprojectidfolderpathbaseline-get
      parameters:
      - in: path
        name: folderPath
      - in: path
        name: projectPath
      responses:
        200:
          description: OK
      tags:
      - Check
      - Baseline
      - Permissiongiven
      - Project
  /projectgroups:
    get:
      summary: Gets paginated project group list
      description: Gets paginated project group list.
      operationId: getProjectGroups
      x-api-path-slug: projectgroups-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
        description: Offset
      - in: query
        name: sortby
        description: Sort by column name
      responses:
        200:
          description: OK
      tags:
      - Paginated
      - Project
      - Group
      - List
    post:
      summary: Creates project group
      description: Creates project group.
      operationId: createProjectGroup
      x-api-path-slug: projectgroups-post
      parameters:
      - in: body
        name: body
        description: New project group data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Project
      - Group
  /projectgroups/{projectgroupid}:
    get:
      summary: Gets project group information
      description: Gets project group information.
      operationId: getProjectGroup
      x-api-path-slug: projectgroupsprojectgroupid-get
      parameters:
      - in: path
        name: projectgroupid
        description: Project group identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - Group
      - Information
    delete:
      summary: Deletes a project group
      description: Deletes a project group.
      operationId: deleteProjectGroup
      x-api-path-slug: projectgroupsprojectgroupid-delete
      parameters:
      - in: query
        name: force
      - in: path
        name: projectgroupid
      responses:
        200:
          description: OK
      tags:
      - Project
      - Group
    patch:
      summary: Updates project group data
      description: Updates project group data.
      operationId: updateProjectGroup
      x-api-path-slug: projectgroupsprojectgroupid-patch
      parameters:
      - in: body
        name: body
        description: Updated project group info
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: If-Match
        description: Project version
      - in: path
        name: projectgroupid
      responses:
        200:
          description: OK
      tags:
      - Project
      - Group
      - Data
  /projectgroups/{projectgroupid}/admins:
    get:
      summary: Gets project group admins
      description: Gets project group admins.
      operationId: getProjectGroupAdmins
      x-api-path-slug: projectgroupsprojectgroupidadmins-get
      parameters:
      - in: path
        name: projectgroupid
        description: Project group identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - Group
      - Admins
  /projectgroups/{projectgroupid}/admins/{username}:
    put:
      summary: Adds project group admin
      description: Adds project group admin.
      operationId: addProjectGroupAdmin
      x-api-path-slug: projectgroupsprojectgroupidadminsusername-put
      parameters:
      - in: path
        name: projectgroupid
        description: Project group identifier
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Project
      - Group
      - Admin
    delete:
      summary: Removes project group admin
      description: Removes project group admin.
      operationId: removeProjectGroupAdmin
      x-api-path-slug: projectgroupsprojectgroupidadminsusername-delete
      parameters:
      - in: path
        name: projectgroupid
        description: Project group identifier
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Project
      - Group
      - Admin
  /projectgroups/{projectgroupid}/members:
    get:
      summary: Gets project group members
      description: Gets project group members.
      operationId: getProjectGroupMembers
      x-api-path-slug: projectgroupsprojectgroupidmembers-get
      parameters:
      - in: path
        name: projectgroupid
        description: Project group identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - Group
      - Members
  /projectgroups/{projectgroupid}/members/{username}:
    put:
      summary: Adds project group member
      description: Adds project group member.
      operationId: addProjectGroupMember
      x-api-path-slug: projectgroupsprojectgroupidmembersusername-put
      parameters:
      - in: path
        name: projectgroupid
        description: Project group identifier
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Project
      - Group
      - Member
    delete:
      summary: Removes project group member
      description: Removes project group member.
      operationId: removeProjectGroupMember
      x-api-path-slug: projectgroupsprojectgroupidmembersusername-delete
      parameters:
      - in: path
        name: projectgroupid
        description: Project group identifier
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Project
      - Group
      - Member
  /projectgroups/{projectgroupid}/projects:
    get:
      summary: Gets project group projects
      description: Gets project group projects.
      operationId: getProjectGroupProjects
      x-api-path-slug: projectgroupsprojectgroupidprojects-get
      parameters:
      - in: path
        name: projectgroupid
        description: Project group identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - Group
      - Projects
  /projectgroups/{projectgroupid}/projects/{projectid}:
    put:
      summary: Adds project to project group
      description: Adds project to project group.
      operationId: addProjectToGroup
      x-api-path-slug: projectgroupsprojectgroupidprojectsprojectid-put
      parameters:
      - in: path
        name: projectgroupid
        description: Project group identifier
      - in: path
        name: projectid
        description: Project identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - To
      - Project
      - Group
    delete:
      summary: Removes project from group
      description: Removes project from group.
      operationId: removeProjectFromGroup
      x-api-path-slug: projectgroupsprojectgroupidprojectsprojectid-delete
      parameters:
      - in: path
        name: projectgroupid
        description: Project group identifier
      - in: path
        name: projectid
        description: Project identifier
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Project
      - From
      - Group
  /projects:
    get:
      summary: Gets paginated project list.
      description: Gets paginated project list..
      operationId: getProjects
      x-api-path-slug: projects-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: fetchHierarchyPath
      - in: query
        name: offset
        description: Offset
      - in: query
        name: searchvalue
      - in: query
        name: sortby
        description: Sort by column name
      responses:
        200:
          description: OK
      tags:
      - Paginated
      - Project
      - List
    post:
      summary: Creates project
      description: Creates project.
      operationId: createProject
      x-api-path-slug: projects-post
      parameters:
      - in: body
        name: body
        description: New project data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Project
  /projects/requests:
    get:
      summary: Gets paginated project request list
      description: Gets paginated project request list.
      operationId: getProjectRequests
      x-api-path-slug: projectsrequests-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
        description: Offset
      responses:
        200:
          description: OK
      tags:
      - Paginated
      - Project
      - Request
      - List
  /projects/requests/count:
    get:
      summary: Gets the number of pending project requests
      description: Gets the number of pending project requests.
      operationId: getProjectRequestCount
      x-api-path-slug: projectsrequestscount-get
      responses:
        200:
          description: OK
      tags:
      - Number
      - Of
      - Pending
      - Project
      - Requests
  /projects/{projectid}:
    get:
      summary: Gets project information
      description: Gets project information.
      operationId: getProject
      x-api-path-slug: projectsprojectid-get
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - Information
    delete:
      summary: Deletes a project
      description: Deletes a project.
      operationId: deleteItem
      x-api-path-slug: projectsprojectid-delete
      parameters:
      - in: query
        name: force
      - in: query
        name: notify
      - in: path
        name: projectid
      responses:
        200:
          description: OK
      tags:
      - Project
    patch:
      summary: Updates project data
      description: Updates project data.
      operationId: updateProject
      x-api-path-slug: projectsprojectid-patch
      parameters:
      - in: body
        name: body
        description: Updated project info
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: If-Match
        description: Project version
      - in: path
        name: projectid
      responses:
        200:
          description: OK
      tags:
      - Project
      - Data
  /projects/{projectid}/admins:
    get:
      summary: Gets project administrators
      description: Gets project administrators.
      operationId: getProjectAdmins
      x-api-path-slug: projectsprojectidadmins-get
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - Administrators
  /projects/{projectid}/diskusage:
    get:
      summary: Gets project disk usage in bytes
      description: Gets project disk usage in bytes.
      operationId: getProjectDiskUsage
      x-api-path-slug: projectsprojectiddiskusage-get
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - Disk
      - Usage
      - In
      - Bytes
  /projects/{projectid}/lock:
    put:
      summary: Locks a project
      description: Locks a project.
      operationId: lockProject
      x-api-path-slug: projectsprojectidlock-put
      parameters:
      - in: path
        name: projectid
      responses:
        200:
          description: OK
      tags:
      - Locks
      - Project
    delete:
      summary: Unlocks a project
      description: Unlocks a project.
      operationId: unlockProject
      x-api-path-slug: projectsprojectidlock-delete
      parameters:
      - in: path
        name: projectid
      responses:
        200:
          description: OK
      tags:
      - Unlocks
      - Project
  /projects/{projectid}/members:
    get:
      summary: Gets project members
      description: Gets project members.
      operationId: getProjectMembers
      x-api-path-slug: projectsprojectidmembers-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
      - in: path
        name: projectid
        description: Project identifier
      - in: query
        name: searchvalue
        description: Filter value for project member name
      - in: query
        name: sortby
        description: Sorting column name
      responses:
        200:
          description: OK
      tags:
      - Project
      - Members
  /projects/{projectid}/roles:
    get:
      summary: Gets project role list
      description: Gets project role list.
      operationId: getProjectRoles
      x-api-path-slug: projectsprojectidroles-get
      parameters:
      - in: query
        name: includeInherited
        description: Include inherited roles? This parameter is relevant for Project
          type only
      - in: path
        name: projectid
        description: Project or project group identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - Role
      - List
    post:
      summary: Creates project role.
      description: Creates project role..
      operationId: createProjectRole
      x-api-path-slug: projectsprojectidroles-post
      parameters:
      - in: body
        name: body
        description: New role data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectid
        description: Project or project group identifier
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Project
      - Role
  /projects/{projectid}/roles/by-users:
    post:
      summary: Get roles by user
      description: Get roles by user.
      operationId: getRolesByUsers
      x-api-path-slug: projectsprojectidrolesbyusers-post
      parameters:
      - in: body
        name: body
        description: List of user Names
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectid
      responses:
        200:
          description: OK
      tags:
      - Roles
      - By
      - User
  /projects/{projectid}/roles/inherited-roles:
    get:
      summary: Gets inherited project role list
      description: Gets inherited project role list.
      operationId: getInheritedProjectRoles
      x-api-path-slug: projectsprojectidrolesinheritedroles-get
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      responses:
        200:
          description: OK
      tags:
      - Inherited
      - Project
      - Role
      - List
  /projects/{projectid}/roles/{roleid}:
    delete:
      summary: Deletes a project role
      description: Deletes a project role.
      operationId: deleteProjectRole
      x-api-path-slug: projectsprojectidrolesroleid-delete
      parameters:
      - in: path
        name: projectid
        description: Project or project group identifier
      - in: path
        name: roleid
      responses:
        200:
          description: OK
      tags:
      - Project
      - Role
    patch:
      summary: Updates project role.
      description: Updates project role..
      operationId: updateProjectRole
      x-api-path-slug: projectsprojectidrolesroleid-patch
      parameters:
      - in: body
        name: body
        description: Updated role info
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: If-Match
        description: Role version
      - in: path
        name: projectid
        description: Project or project group identifier
      - in: path
        name: roleid
        description: Role identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - Role
  /projects/{projectid}/roles/{roleid}/auto-grant:
    get:
      summary: Gets whether a role is granted automatically in a project or not.
      description: Gets whether a role is granted automatically in a project or not..
      operationId: isRoleAutoGrantInProject
      x-api-path-slug: projectsprojectidrolesroleidautogrant-get
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      - in: path
        name: roleid
        description: Role identifier
      responses:
        200:
          description: OK
      tags:
      - Whether
      - Role
      - Is
      - Granted
      - Automatically
      - In
      - Project
      - Not
    put:
      summary: Grant a role automatically in a given project
      description: Grant a role automatically in a given project.
      operationId: autoGrantRoleInProject
      x-api-path-slug: projectsprojectidrolesroleidautogrant-put
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      - in: path
        name: roleid
        description: Role identifier
      responses:
        200:
          description: OK
      tags:
      - Grant
      - Role
      - Automatically
      - In
      - Given
      - Project
    delete:
      summary: Stop granting a role automatically in a given project
      description: Stop granting a role automatically in a given project.
      operationId: removeAutoGrantRoleInProject
      x-api-path-slug: projectsprojectidrolesroleidautogrant-delete
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      - in: path
        name: roleid
        description: Role identifier
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Granting
      - Role
      - Automatically
      - In
      - Given
      - Project
  /projects/{projectid}/roles/{roleid}/members:
    get:
      summary: Gets project role members
      description: Gets project role members.
      operationId: getProjectRoleMembers
      x-api-path-slug: projectsprojectidrolesroleidmembers-get
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      - in: path
        name: roleid
        description: Role identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - Role
      - Members
  /projects/{projectid}/roles/{roleid}/members/{username}:
    put:
      summary: Add user to project role
      description: Add user to project role.
      operationId: addUserToProjectRole
      x-api-path-slug: projectsprojectidrolesroleidmembersusername-put
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      - in: path
        name: roleid
        description: Role identifier
      - in: path
        name: username
        description: username
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - Project
      - Role
    delete:
      summary: Removes user from a project role
      description: Removes user from a project role.
      operationId: removeUserFromProjectRole
      x-api-path-slug: projectsprojectidrolesroleidmembersusername-delete
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      - in: path
        name: roleid
        description: Role identifier
      - in: path
        name: username
        description: username
      responses:
        200:
          description: OK
      tags:
      - Removes
      - User
      - From
      - Project
      - Role
  /projects/{projectid}/subprojects:
    get:
      summary: Gets subproject list.
      description: Gets subproject list..
      operationId: getSubprojects
      x-api-path-slug: projectsprojectidsubprojects-get
      parameters:
      - in: query
        name: fetchHierarchyPath
      - in: path
        name: projectid
        description: Project identifier
      - in: query
        name: sortby
        description: Sort by column name
      responses:
        200:
          description: OK
      tags:
      - Subproject
      - List
  /projects/{projectid}/{username}:
    put:
      summary: Adds project member
      description: Adds project member.
      operationId: addProjectMember
      x-api-path-slug: projectsprojectidusername-put
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Project
      - Member
    delete:
      summary: Removes project member
      description: Removes project member.
      operationId: removeProjectMember
      x-api-path-slug: projectsprojectidusername-delete
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Project
      - Member
  /projecttemplates:
    get:
      summary: Gets paginated project template list.
      description: Gets paginated project template list..
      operationId: getProjectTemplates
      x-api-path-slug: projecttemplates-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
        description: Offset
      - in: query
        name: sortby
        description: Sort by column name
      responses:
        200:
          description: OK
      tags:
      - Paginated
      - Project
      - Template
      - List
  /roles:
    get:
      summary: Gets global/site role list
      description: Gets global/site role list.
      operationId: getRoles
      x-api-path-slug: roles-get
      parameters:
      - in: query
        name: projectId
        description: Context project id (to verify access permissions)
      - in: query
        name: type
        description: Role type
      responses:
        200:
          description: OK
      tags:
      - Global
      - Site
      - Role
      - List
    post:
      summary: Creates role.
      description: Creates role..
      operationId: createRole
      x-api-path-slug: roles-post
      parameters:
      - in: body
        name: body
        description: New role data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Role
  /roles/{roleid}:
    get:
      summary: Gets role data.
      description: Gets role data..
      operationId: getRole
      x-api-path-slug: rolesroleid-get
      parameters:
      - in: path
        name: roleid
        description: Role identifier
      responses:
        200:
          description: OK
      tags:
      - Role
      - Data
    delete:
      summary: Deletes a role
      description: Deletes a role.
      operationId: deleteRole
      x-api-path-slug: rolesroleid-delete
      parameters:
      - in: path
        name: roleid
      responses:
        200:
          description: OK
      tags:
      - Role
    patch:
      summary: Updates role.
      description: Updates role..
      operationId: updateRole
      x-api-path-slug: rolesroleid-patch
      parameters:
      - in: body
        name: body
        description: Updated role info
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: If-Match
        description: Role version
      - in: path
        name: roleid
        description: Role identifier
      responses:
        200:
          description: OK
      tags:
      - Role
  /roles/{roleid}/members:
    get:
      summary: Gets role members
      description: Gets role members.
      operationId: getRoleMembers
      x-api-path-slug: rolesroleidmembers-get
      parameters:
      - in: path
        name: roleid
        description: Role identifier
      responses:
        200:
          description: OK
      tags:
      - Role
      - Members
  /roles/{roleid}/members/{username}:
    put:
      summary: Add user to a role
      description: Add user to a role.
      operationId: addRoleMember
      x-api-path-slug: rolesroleidmembersusername-put
      parameters:
      - in: path
        name: roleid
        description: Role identifier
      - in: path
        name: username
        description: username
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - Role
    delete:
      summary: Removes user from a role
      description: Removes user from a role.
      operationId: removeRoleMember
      x-api-path-slug: rolesroleidmembersusername-delete
      parameters:
      - in: path
        name: roleid
        description: Role identifier
      - in: path
        name: username
        description: username
      responses:
        200:
          description: OK
      tags:
      - Removes
      - User
      - From
      - Role
  /server:
    get:
      summary: Gets TeamForge server information
      description: Gets teamforge server information.
      operationId: getTeamForgeServerInfo
      x-api-path-slug: server-get
      responses:
        200:
          description: OK
      tags:
      - TeamForge
      - Server
      - Information
  /server/health:
    get:
      summary: Gets the health of the CTF core
      description: Gets the health of the ctf core.
      operationId: getHealth
      x-api-path-slug: serverhealth-get
      parameters:
      - in: query
        name: assumeactive
      - in: query
        name: thorough
      - in: query
        name: verbose
      responses:
        200:
          description: OK
      tags:
      - Health
      - Of
      - CTF
      - Core
  /server/licensekey:
    put:
      summary: Sets/Updates license key
      description: Sets/updates license key.
      operationId: enterLicenseKey
      x-api-path-slug: serverlicensekey-put
      parameters:
      - in: body
        name: body
        description: License key
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sets
      - License
      - Key
  /server/licensetypes:
    get:
      summary: Gets valid license types
      description: Gets valid license types.
      operationId: getLicenseTypes
      x-api-path-slug: serverlicensetypes-get
      responses:
        200:
          description: OK
      tags:
      - Valid
      - License
      - Types
  /users:
    get:
      summary: Gets paginated user list
      description: Gets paginated user list.
      operationId: getUsers
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: ids
        description: List of user ids (separated by comma)
      - in: query
        name: names
        description: List of usernames (separated by comma)
      - in: query
        name: offset
        description: Offset
      - in: query
        name: search
        description: Comma separated terms to search in username, fullname fields
      - in: query
        name: sortby
        description: Sort by column name
      - in: query
        name: status
        description: User status
      responses:
        200:
          description: OK
      tags:
      - Paginated
      - User
      - List
    post:
      summary: Creates a user
      description: Creates a user.
      operationId: createUser
      x-api-path-slug: users-post
      parameters:
      - in: body
        name: body
        description: New user information
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - User
  /users/by-email/{email}:
    get:
      summary: Gets user data by email
      description: Gets user data by email.
      operationId: getUserByEmail
      x-api-path-slug: usersbyemailemail-get
      parameters:
      - in: path
        name: email
      responses:
        200:
          description: OK
      tags:
      - User
      - Data
      - By
      - Email
  /users/by-username/{username}:
    get:
      summary: Gets user data by username
      description: Gets user data by username.
      operationId: getUserByUsername
      x-api-path-slug: usersbyusernameusername-get
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - User
      - Data
      - By
      - Username
    delete:
      summary: Deletes a user by username
      description: Deletes a user by username.
      operationId: deleteUserByUsername
      x-api-path-slug: usersbyusernameusername-delete
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - User
      - By
      - Username
    patch:
      summary: Updates a user by username
      description: Updates a user by username.
      operationId: updateUserByUsername
      x-api-path-slug: usersbyusernameusername-patch
      parameters:
      - in: body
        name: body
        description: Updated user info
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: If-Match
        description: User version
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - User
      - By
      - Username
  /users/by-username/{username}/alternative-licensetypes:
    get:
      summary: Gets alternative license types by username.
      description: Gets alternative license types by username..
      operationId: getLicenseByUsername
      x-api-path-slug: usersbyusernameusernamealternativelicensetypes-get
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Alternative
      - License
      - Types
      - By
      - Username
  /users/by-username/{username}/authorization-keys:
    get:
      summary: Gets authorization keys by username
      description: Gets authorization keys by username.
      operationId: getAuthorizationKeysByUsername
      x-api-path-slug: usersbyusernameusernameauthorizationkeys-get
      parameters:
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Authorization
      - Keys
      - By
      - Username
    post:
      summary: Sets authorization keys by username
      description: Sets authorization keys by username.
      operationId: setAuthorizationKeys
      x-api-path-slug: usersbyusernameusernameauthorizationkeys-post
      parameters:
      - in: body
        name: body
        description: Authorization keys
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Authorization
      - Keys
      - By
      - Username
  /users/by-username/{username}/groups:
    get:
      summary: Gets a user's group list by username
      description: Gets a user's group list by username.
      operationId: getUserGroupsByUsername
      x-api-path-slug: usersbyusernameusernamegroups-get
      parameters:
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Users
      - Group
      - List
      - By
      - Username
  /users/by-username/{username}/groups/{groupid}:
    put:
      summary: Add user to a user group by user name
      description: Add user to a user group by user name.
      operationId: addUserToGroupByUsername
      x-api-path-slug: usersbyusernameusernamegroupsgroupid-put
      parameters:
      - in: path
        name: groupid
        description: Group id
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - User
      - Group
      - By
      - User
      - Name
  /users/by-username/{username}/password:
    patch:
      summary: Resets user password by username
      description: Resets user password by username.
      operationId: resetPasswordByUsername
      x-api-path-slug: usersbyusernameusernamepassword-patch
      parameters:
      - in: body
        name: body
        description: New password
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Resets
      - User
      - Password
      - By
      - Username
  /users/by-username/{username}/preferences:
    get:
      summary: Gets preferences by username
      description: Gets preferences by username.
      operationId: getPreferences
      x-api-path-slug: usersbyusernameusernamepreferences-get
      parameters:
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Preferences
      - By
      - Username
    patch:
      summary: Sets preferences by user name
      description: Sets preferences by user name.
      operationId: setPreferences
      x-api-path-slug: usersbyusernameusernamepreferences-patch
      parameters:
      - in: body
        name: body
        description: Preferences
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Preferences
      - By
      - User
      - Name
  /users/by-username/{username}/preferences/{preference}:
    get:
      summary: Gets preference by username
      description: Gets preference by username.
      operationId: getPreference
      x-api-path-slug: usersbyusernameusernamepreferencespreference-get
      parameters:
      - in: path
        name: preference
        description: Preference
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Preference
      - By
      - Username
  /users/by-username/{username}/profile-picture:
    post:
      summary: Uploads and sets profile picture by username
      description: Uploads and sets profile picture by username.
      operationId: setProfilePictureByUsername
      x-api-path-slug: usersbyusernameusernameprofilepicture-post
      parameters:
      - in: body
        name: body
        description: Picture
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Sets
      - Profile
      - Picture
      - By
      - Username
    delete:
      summary: Deletes profile picture by username
      description: Deletes profile picture by username.
      operationId: deleteProfilePictureByUsername
      x-api-path-slug: usersbyusernameusernameprofilepicture-delete
      parameters:
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Profile
      - Picture
      - By
      - Username
  /users/by-username/{username}/projects:
    get:
      summary: Gets a user's project list by username
      description: Gets a user's project list by username.
      operationId: getProjectsByUsername
      x-api-path-slug: usersbyusernameusernameprojects-get
      parameters:
      - in: query
        name: fetchHierarchyPath
      - in: query
        name: sortby
        description: Sort by column name
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Users
      - Project
      - List
      - By
      - Username
  /users/by-username/{username}/projects/{projectid}:
    put:
      summary: Adds a user to specified project's member list by username
      description: Adds a user to specified project's member list by username.
      operationId: addUserByUsername
      x-api-path-slug: usersbyusernameusernameprojectsprojectid-put
      parameters:
      - in: path
        name: projectid
        description: Project id
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - Specified
      - Projects
      - Member
      - List
      - By
      - Username
  /users/myself:
    get:
      summary: Gets user data for current user
      description: Gets user data for current user.
      operationId: getMyself
      x-api-path-slug: usersmyself-get
      responses:
        200:
          description: OK
      tags:
      - User
      - Datacurrent
      - User
    patch:
      summary: Updates current user data
      description: Updates current user data.
      operationId: updateMyself
      x-api-path-slug: usersmyself-patch
      parameters:
      - in: body
        name: body
        description: Updated user info
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: If-Match
        description: User version
      responses:
        200:
          description: OK
      tags:
      - Current
      - User
      - Data
  /users/myself/alternative-licensetypes:
    get:
      summary: Gets alternative license types for current user.
      description: Gets alternative license types for current user..
      operationId: getLicenseForMyself
      x-api-path-slug: usersmyselfalternativelicensetypes-get
      responses:
        200:
          description: OK
      tags:
      - Alternative
      - License
      - Typescurrent
      - User
  /users/myself/authorization-keys:
    get:
      summary: Gets authorization keys for current user
      description: Gets authorization keys for current user.
      operationId: getAuthorizationKeysForMyself
      x-api-path-slug: usersmyselfauthorizationkeys-get
      responses:
        200:
          description: OK
      tags:
      - Authorization
      - Keyscurrent
      - User
    post:
      summary: Sets authorization keys for current user
      description: Sets authorization keys for current user.
      operationId: setAuthorizationKeysForMyself
      x-api-path-slug: usersmyselfauthorizationkeys-post
      parameters:
      - in: body
        name: body
        description: Authorization keys
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Authorization
      - Keyscurrent
      - User
  /users/myself/groups:
    get:
      summary: Gets current user's group list
      description: Gets current user's group list.
      operationId: getMyUserGroups
      x-api-path-slug: usersmyselfgroups-get
      responses:
        200:
          description: OK
      tags:
      - Current
      - Users
      - Group
      - List
  /users/myself/groups/{groupid}:
    put:
      summary: Add current user to a user group
      description: Add current user to a user group.
      operationId: addMyselfToGroup
      x-api-path-slug: usersmyselfgroupsgroupid-put
      parameters:
      - in: path
        name: groupid
        description: Group id
      responses:
        200:
          description: OK
      tags:
      - Current
      - User
      - To
      - User
      - Group
  /users/myself/password:
    patch:
      summary: Resets user password for current user
      description: Resets user password for current user.
      operationId: resetPasswordForMyself
      x-api-path-slug: usersmyselfpassword-patch
      parameters:
      - in: body
        name: body
        description: New password
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Resets
      - User
      - Passwordcurrent
      - User
  /users/myself/preferences:
    get:
      summary: Gets preferences for current user
      description: Gets preferences for current user.
      operationId: getPreferencesForMyself
      x-api-path-slug: usersmyselfpreferences-get
      responses:
        200:
          description: OK
      tags:
      - Preferencescurrent
      - User
    patch:
      summary: Sets preferences for current user
      description: Sets preferences for current user.
      operationId: setPreferencesForMyself
      x-api-path-slug: usersmyselfpreferences-patch
      parameters:
      - in: body
        name: body
        description: Preferences
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Preferencescurrent
      - User
  /users/myself/preferences/{preference}:
    get:
      summary: Gets preference for current user
      description: Gets preference for current user.
      operationId: getPreferenceForMyself
      x-api-path-slug: usersmyselfpreferencespreference-get
      parameters:
      - in: path
        name: preference
        description: Preference
      responses:
        200:
          description: OK
      tags:
      - Preferencecurrent
      - User
  /users/myself/profile-picture:
    post:
      summary: Uploads and sets profile picture for current user
      description: Uploads and sets profile picture for current user.
      operationId: setProfilePictureForMyself
      x-api-path-slug: usersmyselfprofilepicture-post
      parameters:
      - in: body
        name: body
        description: Picture
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Sets
      - Profile
      - Picturecurrent
      - User
    delete:
      summary: Deletes profile picture for current user
      description: Deletes profile picture for current user.
      operationId: deleteProfilePictureForMyself
      x-api-path-slug: usersmyselfprofilepicture-delete
      responses:
        200:
          description: OK
      tags:
      - Profile
      - Picturecurrent
      - User
  /users/myself/projects:
    get:
      summary: Gets current user's project list
      description: Gets current user's project list.
      operationId: getMyProjects
      x-api-path-slug: usersmyselfprojects-get
      parameters:
      - in: query
        name: fetchHierarchyPath
      - in: query
        name: sortby
        description: Sort by column name
      responses:
        200:
          description: OK
      tags:
      - Current
      - Users
      - Project
      - List
  /users/myself/projects/{projectid}:
    put:
      summary: Adds current user to specified project's member list
      description: Adds current user to specified project's member list.
      operationId: addMyself
      x-api-path-slug: usersmyselfprojectsprojectid-put
      parameters:
      - in: path
        name: projectid
        description: Project id
      responses:
        200:
          description: OK
      tags:
      - Current
      - User
      - To
      - Specified
      - Projects
      - Member
      - List
  /users/{userid}:
    get:
      summary: Gets user data by user id
      description: Gets user data by user id.
      operationId: getUserById
      x-api-path-slug: usersuserid-get
      parameters:
      - in: path
        name: userid
      responses:
        200:
          description: OK
      tags:
      - User
      - Data
      - By
      - User
    delete:
      summary: Deletes a user by user id
      description: Deletes a user by user id.
      operationId: deleteUserById
      x-api-path-slug: usersuserid-delete
      parameters:
      - in: path
        name: userid
      responses:
        200:
          description: OK
      tags:
      - User
      - By
      - User
    patch:
      summary: Updates a user by user id
      description: Updates a user by user id.
      operationId: updateUserById
      x-api-path-slug: usersuserid-patch
      parameters:
      - in: body
        name: body
        description: Updated user info
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: If-Match
        description: User version
      - in: path
        name: userid
      responses:
        200:
          description: OK
      tags:
      - User
      - By
      - User
  /users/{userid}/alternative-licensetypes:
    get:
      summary: Gets alternative license types by userid.
      description: Gets alternative license types by userid..
      operationId: getLicenseById
      x-api-path-slug: usersuseridalternativelicensetypes-get
      parameters:
      - in: path
        name: userid
      responses:
        200:
          description: OK
      tags:
      - Alternative
      - License
      - Types
      - By
      - Userid
  /users/{userid}/authorization-keys:
    get:
      summary: Gets authorization keys by user id
      description: Gets authorization keys by user id.
      operationId: getAuthorizationKeysById
      x-api-path-slug: usersuseridauthorizationkeys-get
      parameters:
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Authorization
      - Keys
      - By
      - User
    post:
      summary: Sets authorization keys by user id
      description: Sets authorization keys by user id.
      operationId: setAuthorizationKeysById
      x-api-path-slug: usersuseridauthorizationkeys-post
      parameters:
      - in: body
        name: body
        description: Authorization keys
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Authorization
      - Keys
      - By
      - User
  /users/{userid}/groups:
    get:
      summary: Gets a user's group list by user id
      description: Gets a user's group list by user id.
      operationId: getUserGroupsByUserid
      x-api-path-slug: usersuseridgroups-get
      parameters:
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Group
      - List
      - By
      - User
  /users/{userid}/groups/{groupid}:
    put:
      summary: Add user to a user group by user id
      description: Add user to a user group by user id.
      operationId: addUserToGroupByUserid
      x-api-path-slug: usersuseridgroupsgroupid-put
      parameters:
      - in: path
        name: groupid
        description: Group id
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - User
      - Group
      - By
      - User
  /users/{userid}/password:
    patch:
      summary: Resets user password by userid
      description: Resets user password by userid.
      operationId: resetPasswordById
      x-api-path-slug: usersuseridpassword-patch
      parameters:
      - in: body
        name: body
        description: New password
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userid
      responses:
        200:
          description: OK
      tags:
      - Resets
      - User
      - Password
      - By
      - Userid
  /users/{userid}/preferences:
    get:
      summary: Gets preferences by user id
      description: Gets preferences by user id.
      operationId: getPreferencesById
      x-api-path-slug: usersuseridpreferences-get
      parameters:
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Preferences
      - By
      - User
    patch:
      summary: Sets preferences by user id
      description: Sets preferences by user id.
      operationId: setPreferencesById
      x-api-path-slug: usersuseridpreferences-patch
      parameters:
      - in: body
        name: body
        description: Preferences
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Preferences
      - By
      - User
  /users/{userid}/preferences/{preference}:
    get:
      summary: Gets preference by user id
      description: Gets preference by user id.
      operationId: getPreferenceById
      x-api-path-slug: usersuseridpreferencespreference-get
      parameters:
      - in: path
        name: preference
        description: Preference
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Preference
      - By
      - User
  /users/{userid}/profile-picture:
    post:
      summary: Uploads and sets profile picture by user id
      description: Uploads and sets profile picture by user id.
      operationId: setProfilePictureById
      x-api-path-slug: usersuseridprofilepicture-post
      parameters:
      - in: body
        name: body
        description: Picture
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Sets
      - Profile
      - Picture
      - By
      - User
    delete:
      summary: Deletes profile picture by user id
      description: Deletes profile picture by user id.
      operationId: deleteProfilePictureById
      x-api-path-slug: usersuseridprofilepicture-delete
      parameters:
      - in: path
        name: userid
        description: User ID
      responses:
        200:
          description: OK
      tags:
      - Profile
      - Picture
      - By
      - User
  /users/{userid}/projects:
    get:
      summary: Gets a user's project list by user id
      description: Gets a user's project list by user id.
      operationId: getProjectsByUserid
      x-api-path-slug: usersuseridprojects-get
      parameters:
      - in: query
        name: fetchHierarchyPath
      - in: query
        name: sortby
        description: Sort by column name
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Project
      - List
      - By
      - User
  /users/{userid}/projects/{projectid}:
    put:
      summary: Adds a user to specified project's member list by user id
      description: Adds a user to specified project's member list by user id.
      operationId: addUserById
      x-api-path-slug: usersuseridprojectsprojectid-put
      parameters:
      - in: path
        name: projectid
        description: Project id
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - Specified
      - Projects
      - Member
      - List
      - By
      - User