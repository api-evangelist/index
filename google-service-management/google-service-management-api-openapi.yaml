swagger: "2.0"
x-collection-name: Google Service Management
x-complete: 1
info:
  title: Google Service Management
  description: google-service-management-allows-service-producers-to-publish-their-services-on-google-cloud-platform-so-that-they-can-be-discovered-and-used-by-service-consumers-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: servicemanagement.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/services:
    get:
      summary: Get Services
      description: |-
        Lists managed services.

        Returns all public services. For authenticated users, also returns all
        services the calling user has "servicemanagement.services.get" permission
        for.

        **BETA:** If the caller specifies the `consumer_id`, it returns only the
        services enabled on the consumer. The `consumer_id` must have the format
        of "project:{PROJECT-ID}".
      operationId: servicemanagement.services.list
      x-api-path-slug: v1services-get
      parameters:
      - in: query
        name: consumerId
        description: Include services consumed by the specified consumer
      - in: query
        name: pageSize
        description: Requested size of the next page of data
      - in: query
        name: pageToken
        description: Token identifying which result to start with; returned by a previous
          listcall
      - in: query
        name: producerProjectId
        description: Include services produced by the specified project
      responses:
        200:
          description: OK
      tags:
      - Service
    post:
      summary: Create Service
      description: |-
        Creates a new managed service.
        Please note one producer project can own no more than 20 services.

        Operation<response: ManagedService>
      operationId: servicemanagement.services.create
      x-api-path-slug: v1services-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Service
  /v1/services/{serviceName}:
    delete:
      summary: Delete Service
      description: |-
        Deletes a managed service. This method will change the service to the
        `Soft-Delete` state for 30 days. Within this period, service producers may
        call UndeleteService to restore the service.
        After 30 days, the service will be permanently deleted.

        Operation<response: google.protobuf.Empty>
      operationId: servicemanagement.services.delete
      x-api-path-slug: v1servicesservicename-delete
      parameters:
      - in: path
        name: serviceName
        description: The name of the service
      responses:
        200:
          description: OK
      tags:
      - Service
    get:
      summary: Get Service
      description: |-
        Gets a managed service. Authentication is required unless the service is
        public.
      operationId: servicemanagement.services.get
      x-api-path-slug: v1servicesservicename-get
      parameters:
      - in: path
        name: serviceName
        description: The name of the service
      responses:
        200:
          description: OK
      tags:
      - Service
  /v1/services/{serviceName}/config:
    get:
      summary: Create Service Configuration
      description: Gets a service configuration (version) for a managed service.
      operationId: servicemanagement.services.getConfig
      x-api-path-slug: v1servicesservicenameconfig-get
      parameters:
      - in: query
        name: configId
        description: The id of the service configuration resource
      - in: path
        name: serviceName
        description: The name of the service
      - in: query
        name: view
        description: Specifies which parts of the Service Config should be returned
          in theresponse
      responses:
        200:
          description: OK
      tags:
      - Service Configuration
  /v1/services/{serviceName}/configs:
    get:
      summary: Create Service Configurations
      description: |-
        Lists the history of the service configuration for a managed service,
        from the newest to the oldest.
      operationId: servicemanagement.services.configs.list
      x-api-path-slug: v1servicesservicenameconfigs-get
      parameters:
      - in: query
        name: pageSize
        description: The max number of items to include in the response list
      - in: query
        name: pageToken
        description: The token of the page to retrieve
      - in: path
        name: serviceName
        description: The name of the service
      responses:
        200:
          description: OK
      tags:
      - Service Configuration
    post:
      summary: Create Service Configuration
      description: |-
        Creates a new service configuration (version) for a managed service.
        This method only stores the service configuration. To roll out the service
        configuration to backend systems please call
        CreateServiceRollout.
      operationId: servicemanagement.services.configs.create
      x-api-path-slug: v1servicesservicenameconfigs-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: serviceName
        description: The name of the service
      responses:
        200:
          description: OK
      tags:
      - Service Configuration
  /v1/services/{serviceName}/configs/{configId}:
    get:
      summary: Get Service Configuration
      description: Gets a service configuration (version) for a managed service.
      operationId: servicemanagement.services.configs.get
      x-api-path-slug: v1servicesservicenameconfigsconfigid-get
      parameters:
      - in: path
        name: configId
        description: The id of the service configuration resource
      - in: path
        name: serviceName
        description: The name of the service
      - in: query
        name: view
        description: Specifies which parts of the Service Config should be returned
          in theresponse
      responses:
        200:
          description: OK
      tags:
      - Service Configuration
  /v1/services/{serviceName}/configs:submit:
    post:
      summary: Create Service Configuration
      description: |-
        Creates a new service configuration (version) for a managed service based
        on
        user-supplied configuration source files (for example: OpenAPI
        Specification). This method stores the source configurations as well as the
        generated service configuration. To rollout the service configuration to
        other services,
        please call CreateServiceRollout.

        Operation<response: SubmitConfigSourceResponse>
      operationId: servicemanagement.services.configs.submit
      x-api-path-slug: v1servicesservicenameconfigssubmit-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: serviceName
        description: The name of the service
      responses:
        200:
          description: OK
      tags:
      - Service Configuration
  /v1/services/{serviceName}/rollouts:
    get:
      summary: Get History
      description: |-
        Lists the history of the service configuration rollouts for a managed
        service, from the newest to the oldest.
      operationId: servicemanagement.services.rollouts.list
      x-api-path-slug: v1servicesservicenamerollouts-get
      parameters:
      - in: query
        name: pageSize
        description: The max number of items to include in the response list
      - in: query
        name: pageToken
        description: The token of the page to retrieve
      - in: path
        name: serviceName
        description: The name of the service
      responses:
        200:
          description: OK
      tags:
      - Service History
    post:
      summary: Create new Service Configuration
      description: |-
        Creates a new service configuration rollout. Based on rollout, the
        Google Service Management will roll out the service configurations to
        different backend services. For example, the logging configuration will be
        pushed to Google Cloud Logging.

        Please note that any previous pending and running Rollouts and associated
        Operations will be automatically cancelled so that the latest Rollout will
        not be blocked by previous Rollouts.

        Operation<response: Rollout>
      operationId: servicemanagement.services.rollouts.create
      x-api-path-slug: v1servicesservicenamerollouts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: serviceName
        description: The name of the service
      responses:
        200:
          description: OK
      tags:
      - Service Configuration
  /v1/services/{serviceName}/rollouts/{rolloutId}:
    get:
      summary: Get Service Configuration
      description: Gets a service configuration rollout.
      operationId: servicemanagement.services.rollouts.get
      x-api-path-slug: v1servicesservicenamerolloutsrolloutid-get
      parameters:
      - in: path
        name: rolloutId
        description: The id of the rollout resource
      - in: path
        name: serviceName
        description: The name of the service
      responses:
        200:
          description: OK
      tags:
      - Service Configuration
  /v1/services/{serviceName}:disable:
    post:
      summary: Disable Service
      description: |-
        Disables a service for a project, so it can no longer be
        be used for the project. It prevents accidental usage that may cause
        unexpected billing charges or security leaks.

        Operation<response: DisableServiceResponse>
      operationId: servicemanagement.services.disable
      x-api-path-slug: v1servicesservicenamedisable-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: serviceName
        description: Name of the service to disable
      responses:
        200:
          description: OK
      tags:
      - Service
  /v1/services/{serviceName}:enable:
    post:
      summary: Enable Service
      description: |-
        Enables a service for a project, so it can be used
        for the project. See
        [Cloud Auth Guide](https://cloud.google.com/docs/authentication) for
        more information.

        Operation<response: EnableServiceResponse>
      operationId: servicemanagement.services.enable
      x-api-path-slug: v1servicesservicenameenable-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: serviceName
        description: Name of the service to enable
      responses:
        200:
          description: OK
      tags:
      - Service
  /v1/services/{serviceName}:undelete:
    post:
      summary: Undelete Service
      description: |-
        Revives a previously deleted managed service. The method restores the
        service using the configuration at the time the service was deleted.
        The target service must exist and must have been deleted within the
        last 30 days.

        Operation<response: UndeleteServiceResponse>
      operationId: servicemanagement.services.undelete
      x-api-path-slug: v1servicesservicenameundelete-post
      parameters:
      - in: path
        name: serviceName
        description: The name of the service
      responses:
        200:
          description: OK
      tags:
      - Service
  /v1/services:generateConfigReport:
    post:
      summary: Generate Configuration Report
      description: |-
        Generates and returns a report (errors, warnings and changes from
        existing configurations) associated with
        GenerateConfigReportRequest.new_value

        If GenerateConfigReportRequest.old_value is specified,
        GenerateConfigReportRequest will contain a single ChangeReport based on the
        comparison between GenerateConfigReportRequest.new_value and
        GenerateConfigReportRequest.old_value.
        If GenerateConfigReportRequest.old_value is not specified, this method
        will compare GenerateConfigReportRequest.new_value with the last pushed
        service configuration.
      operationId: servicemanagement.services.generateConfigReport
      x-api-path-slug: v1servicesgenerateconfigreport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Report
  /v1/{name}:
    get:
      summary: Get Service State
      description: |-
        Gets the latest state of a long-running operation.  Clients can use this
        method to poll the operation result at intervals as recommended by the API
        service.
      operationId: servicemanagement.operations.get
      x-api-path-slug: v1name-get
      parameters:
      - in: path
        name: name
        description: The name of the operation resource
      responses:
        200:
          description: OK
      tags:
      - Service
  /v1/{resource}:getIamPolicy:
    post:
      summary: Get IAM Policy
      description: |-
        Gets the access control policy for a resource.
        Returns an empty policy if the resource exists and does not have a policy
        set.
      operationId: servicemanagement.services.getIamPolicy
      x-api-path-slug: v1resourcegetiampolicy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy is being requested'
      responses:
        200:
          description: OK
      tags:
      - IAM
  /v1/{resource}:setIamPolicy:
    post:
      summary: Set IAM Policy
      description: |-
        Sets the access control policy on the specified resource. Replaces any
        existing policy.
      operationId: servicemanagement.services.setIamPolicy
      x-api-path-slug: v1resourcesetiampolicy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy is being specified'
      responses:
        200:
          description: OK
      tags:
      - IAM
  /v1/{resource}:testIamPermissions:
    post:
      summary: Test Permissions
      description: |-
        Returns permissions that a caller has on the specified resource.
        If the resource does not exist, this will return an empty set of
        permissions, not a NOT_FOUND error.

        Note: This operation is designed to be used for building permission-aware
        UIs and command-line tools, not for authorization checking. This operation
        may "fail open" without warning.
      operationId: servicemanagement.services.testIamPermissions
      x-api-path-slug: v1resourcetestiampermissions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy detail is being
          requested'
      responses:
        200:
          description: OK
      tags:
      - Test