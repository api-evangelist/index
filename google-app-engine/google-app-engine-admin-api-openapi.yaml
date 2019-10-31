swagger: "2.0"
x-collection-name: Google App Engine
x-complete: 1
info:
  title: Google App Engine Admin
  description: provisions-and-manages-app-engine-applications-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: appengine.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/apps:
    post:
      summary: Create App
      description: 'Creates an App Engine application for a Google Cloud Platform
        project. Required fields: id - The ID of the target Cloud Platform project.
        location - The region (https://cloud.google.com/appengine/docs/locations)
        where you want the App Engine application located.For more information about
        App Engine applications, see Managing Projects, Applications, and Billing
        (https://cloud.google.com/appengine/docs/python/console/).'
      operationId: appengine.apps.create
      x-api-path-slug: v1apps-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Application
  /v1/apps/{appsId}:
    get:
      summary: Get App
      description: Gets information about an application.
      operationId: appengine.apps.get
      x-api-path-slug: v1appsappsid-get
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      responses:
        200:
          description: OK
      tags:
      - Application
    patch:
      summary: Update App
      description: 'Updates the specified Application resource. You can update the
        following fields: auth_domain - Google authentication domain for controlling
        user access to the application. default_cookie_expiration - Cookie expiration
        policy for the application.'
      operationId: appengine.apps.patch
      x-api-path-slug: v1appsappsid-patch
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: updateMask
        description: Standard field mask for the set of fields to be updated
      responses:
        200:
          description: OK
      tags:
      - Application
  /v1/apps/{appsId}/locations:
    get:
      summary: Get App Locations
      description: Lists information about the supported locations for this service.
      operationId: appengine.apps.locations.list
      x-api-path-slug: v1appsappsidlocations-get
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: query
        name: filter
        description: The standard list filter
      - in: query
        name: pageSize
        description: The standard list page size
      - in: query
        name: pageToken
        description: The standard list page token
      responses:
        200:
          description: OK
      tags:
      - Application Location
  /v1/apps/{appsId}/locations/{locationsId}:
    get:
      summary: Get App Location
      description: Get information about a location.
      operationId: appengine.apps.locations.get
      x-api-path-slug: v1appsappsidlocationslocationsid-get
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: path
        name: locationsId
        description: Part of `name`
      responses:
        200:
          description: OK
      tags:
      - Application Location
  /v1/apps/{appsId}/operations:
    get:
      summary: Get Operations
      description: 'Lists operations that match the specified filter in the request.
        If the server doesn''t support this method, it returns UNIMPLEMENTED.NOTE:
        the name binding below allows API services to override the binding to use
        different resource name schemes, such as users/*/operations.'
      operationId: appengine.apps.operations.list
      x-api-path-slug: v1appsappsidoperations-get
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: query
        name: filter
        description: The standard list filter
      - in: query
        name: pageSize
        description: The standard list page size
      - in: query
        name: pageToken
        description: The standard list page token
      responses:
        200:
          description: OK
      tags:
      - Operation
  /v1/apps/{appsId}/operations/{operationsId}:
    get:
      summary: Get State
      description: Gets the latest state of a long-running operation. Clients can
        use this method to poll the operation result at intervals as recommended by
        the API service.
      operationId: appengine.apps.operations.get
      x-api-path-slug: v1appsappsidoperationsoperationsid-get
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: path
        name: operationsId
        description: Part of `name`
      responses:
        200:
          description: OK
      tags:
      - State
  /v1/apps/{appsId}/services:
    get:
      summary: Get Services
      description: Lists all the services in the application.
      operationId: appengine.apps.services.list
      x-api-path-slug: v1appsappsidservices-get
      parameters:
      - in: path
        name: appsId
        description: Part of `parent`
      - in: query
        name: pageSize
        description: Maximum results to return per page
      - in: query
        name: pageToken
        description: Continuation token for fetching the next page of results
      responses:
        200:
          description: OK
      tags:
      - Service
  /v1/apps/{appsId}/services/{servicesId}:
    delete:
      summary: Delete Service
      description: Deletes the specified service and all enclosed versions.
      operationId: appengine.apps.services.delete
      x-api-path-slug: v1appsappsidservicesservicesid-delete
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: path
        name: servicesId
        description: Part of `name`
      responses:
        200:
          description: OK
      tags:
      - Service
    get:
      summary: Get Configuration
      description: Gets the current configuration of the specified service.
      operationId: appengine.apps.services.get
      x-api-path-slug: v1appsappsidservicesservicesid-get
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: path
        name: servicesId
        description: Part of `name`
      responses:
        200:
          description: OK
      tags:
      - Configuration
    patch:
      summary: Update Configuration
      description: Updates the configuration of the specified service.
      operationId: appengine.apps.services.patch
      x-api-path-slug: v1appsappsidservicesservicesid-patch
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: migrateTraffic
        description: Set to true to gradually shift traffic to one or more versions
          that you specify
      - in: path
        name: servicesId
        description: Part of `name`
      - in: query
        name: updateMask
        description: Standard field mask for the set of fields to be updated
      responses:
        200:
          description: OK
      tags:
      - Configuration
  /v1/apps/{appsId}/services/{servicesId}/versions:
    get:
      summary: Get Versions
      description: Lists the versions of a service.
      operationId: appengine.apps.services.versions.list
      x-api-path-slug: v1appsappsidservicesservicesidversions-get
      parameters:
      - in: path
        name: appsId
        description: Part of `parent`
      - in: query
        name: pageSize
        description: Maximum results to return per page
      - in: query
        name: pageToken
        description: Continuation token for fetching the next page of results
      - in: path
        name: servicesId
        description: Part of `parent`
      - in: query
        name: view
        description: Controls the set of fields returned in the List response
      responses:
        200:
          description: OK
      tags:
      - Version
    post:
      summary: Deploy Version
      description: Deploys code and resource files to a new version.
      operationId: appengine.apps.services.versions.create
      x-api-path-slug: v1appsappsidservicesservicesidversions-post
      parameters:
      - in: path
        name: appsId
        description: Part of `parent`
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: servicesId
        description: Part of `parent`
      responses:
        200:
          description: OK
      tags:
      - Version
  /v1/apps/{appsId}/services/{servicesId}/versions/{versionsId}:
    delete:
      summary: Delete Version
      description: Deletes an existing Version resource.
      operationId: appengine.apps.services.versions.delete
      x-api-path-slug: v1appsappsidservicesservicesidversionsversionsid-delete
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: path
        name: servicesId
        description: Part of `name`
      - in: path
        name: versionsId
        description: Part of `name`
      responses:
        200:
          description: OK
      tags:
      - Version
    get:
      summary: Get Version
      description: Gets the specified Version resource. By default, only a BASIC_VIEW
        will be returned. Specify the FULL_VIEW parameter to get the full resource.
      operationId: appengine.apps.services.versions.get
      x-api-path-slug: v1appsappsidservicesservicesidversionsversionsid-get
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: path
        name: servicesId
        description: Part of `name`
      - in: path
        name: versionsId
        description: Part of `name`
      - in: query
        name: view
        description: Controls the set of fields returned in the Get response
      responses:
        200:
          description: OK
      tags:
      - Version
    patch:
      summary: Update Version
      description: 'Updates the specified Version resource. You can specify the following
        fields depending on the App Engine environment and type of scaling that the
        version resource uses: serving_status (https://cloud.google.com/appengine/docs/admin-api/reference/rest/v1/apps.services.versions#Version.FIELDS.serving_status):
        For Version resources that use basic scaling, manual scaling, or run in the
        App Engine flexible environment. instance_class (https://cloud.google.com/appengine/docs/admin-api/reference/rest/v1/apps.services.versions#Version.FIELDS.instance_class):
        For Version resources that run in the App Engine standard environment. automatic_scaling.min_idle_instances
        (https://cloud.google.com/appengine/docs/admin-api/reference/rest/v1/apps.services.versions#Version.FIELDS.automatic_scaling):
        For Version resources that use automatic scaling and run in the App Engine
        standard environment. automatic_scaling.max_idle_instances (https://cloud.google.com/appengine/docs/admin-api/reference/rest/v1/apps.services.versions#Version.FIELDS.automatic_scaling):
        For Version resources that use automatic scaling and run in the App Engine
        standard environment.'
      operationId: appengine.apps.services.versions.patch
      x-api-path-slug: v1appsappsidservicesservicesidversionsversionsid-patch
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: servicesId
        description: Part of `name`
      - in: query
        name: updateMask
        description: Standard field mask for the set of fields to be updated
      - in: path
        name: versionsId
        description: Part of `name`
      responses:
        200:
          description: OK
      tags:
      - Version
  /v1/apps/{appsId}/services/{servicesId}/versions/{versionsId}/instances:
    get:
      summary: Get Instances
      description: 'Lists the instances of a version.Tip: To aggregate details about
        instances over time, see the Stackdriver Monitoring API (https://cloud.google.com/monitoring/api/ref_v3/rest/v3/projects.timeSeries/list).'
      operationId: appengine.apps.services.versions.instances.list
      x-api-path-slug: v1appsappsidservicesservicesidversionsversionsidinstances-get
      parameters:
      - in: path
        name: appsId
        description: Part of `parent`
      - in: query
        name: pageSize
        description: Maximum results to return per page
      - in: query
        name: pageToken
        description: Continuation token for fetching the next page of results
      - in: path
        name: servicesId
        description: Part of `parent`
      - in: path
        name: versionsId
        description: Part of `parent`
      responses:
        200:
          description: OK
      tags:
      - Instance
  /v1/apps/{appsId}/services/{servicesId}/versions/{versionsId}/instances/{instancesId}:
    delete:
      summary: Stop Instance
      description: Stops a running instance.
      operationId: appengine.apps.services.versions.instances.delete
      x-api-path-slug: v1appsappsidservicesservicesidversionsversionsidinstancesinstancesid-delete
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: path
        name: instancesId
        description: Part of `name`
      - in: path
        name: servicesId
        description: Part of `name`
      - in: path
        name: versionsId
        description: Part of `name`
      responses:
        200:
          description: OK
      tags:
      - Instance
    get:
      summary: Get Instance
      description: Gets instance information.
      operationId: appengine.apps.services.versions.instances.get
      x-api-path-slug: v1appsappsidservicesservicesidversionsversionsidinstancesinstancesid-get
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: path
        name: instancesId
        description: Part of `name`
      - in: path
        name: servicesId
        description: Part of `name`
      - in: path
        name: versionsId
        description: Part of `name`
      responses:
        200:
          description: OK
      tags:
      - Instance
  /v1/apps/{appsId}/services/{servicesId}/versions/{versionsId}/instances/{instancesId}:debug:
    post:
      summary: Enable Debugging
      description: Enables debugging on a VM instance. This allows you to use the
        SSH command to connect to the virtual machine where the instance lives. While
        in "debug mode", the instance continues to serve live traffic. You should
        delete the instance when you are done debugging and then allow the system
        to take over and determine if another instance should be started.Only applicable
        for instances in App Engine flexible environment.
      operationId: appengine.apps.services.versions.instances.debug
      x-api-path-slug: v1appsappsidservicesservicesidversionsversionsidinstancesinstancesiddebug-post
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instancesId
        description: Part of `name`
      - in: path
        name: servicesId
        description: Part of `name`
      - in: path
        name: versionsId
        description: Part of `name`
      responses:
        200:
          description: OK
      tags:
      - Debugging
  /v1/apps/{appsId}:repair:
    post:
      summary: Repair App
      description: Recreates the required App Engine features for the specified App
        Engine application, for example a Cloud Storage bucket or App Engine service
        account. Use this method if you receive an error message about a missing feature,
        for example, Error retrieving the App Engine service account.
      operationId: appengine.apps.repair
      x-api-path-slug: v1appsappsidrepair-post
      parameters:
      - in: path
        name: appsId
        description: Part of `name`
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - App