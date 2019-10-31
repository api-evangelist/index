swagger: "2.0"
x-collection-name: Backupify
x-complete: 1
info:
  title: Backupify
  description: the-backupify-api-allows-you-to-integrate-the-leading-saas-backup-solution-into-your-software-making-it-easy-to-give-your-customers-the-data-protection-they-need--
  version: 1.0.0
host: api.backupify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /oauth/token:
    post:
      summary: Retrieve an Access Token authenticated using the provided client_id
        and client_secret.
      description: All actions and visibility is limited in scope to items that are
        descendents of the authenticated vendor and the backup_definitions owned thereby.
        At this time, all Access Tokens are scoped with full write capabilities.
      operationId: postOauthToken
      x-api-path-slug: oauthtoken-post
      parameters:
      - in: formData
        name: client_id
        description: API Client ID
      - in: formData
        name: client_secret
        description: API Client secret
      - in: formData
        name: grant_type
        description: String identifying the grant type to be used for token retrieval
      - in: formData
        name: scope
        description: A space separated list of operational scopes available to the
          returned token
      responses:
        200:
          description: OK
      tags:
      - Oauth
      - Token
  /v1/authenticate_customer:
    get:
      summary: A simple method to test authentication of a customer access token.
      description: A simple method to test authentication of a customer access token..
      operationId: getV1AuthenticateCustomer
      x-api-path-slug: v1authenticate-customer-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted for customer
      responses:
        200:
          description: OK
      tags:
      - V1
      - Authenticate
      - Customer
  /v1/authenticate_vendor:
    get:
      summary: A simple method to test authentication of a vendor access token. The
        response body is empty JSON object.
      description: A simple method to test authentication of a vendor access token.
        the response body is empty json object..
      operationId: getV1AuthenticateVendor
      x-api-path-slug: v1authenticate-vendor-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client_credentials for vendor
      responses:
        200:
          description: OK
      tags:
      - V1
      - Authenticate
      - Vendor
  /v1/backup_definitions:
    get:
      summary: Retrieve an index of all backup_definitions
      description: This will retrieve a list of backup_defintions from all vendors.
        To view backup_defintions for a particular vendor, see the vendors API. Records
        are returned in ascending order (by id), with a default of 20 per page. Links
        to the next, previous, first, and last pages can be found in the response
        headers.
      operationId: getV1BackupDefinitions
      x-api-path-slug: v1backup-definitions-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: query
        name: vendor_id
        description: Limit backup_definitions returned to those owned by the specified
          vendor_id
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
    post:
      summary: Create a new backup_definition
      description: Create a new backup_definition.
      operationId: postV1BackupDefinitions
      x-api-path-slug: v1backup-definitions-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: formData
        name: backup_definition[description]
        description: Description of the backup_definition
      - in: formData
        name: backup_definition[name]
        description: Name for the backup_definition
      - in: formData
        name: backup_definition[published]
        description: Boolean flag indicating whether the backup definition is published
          and available for use
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
  /v1/backup_definitions/{backup_definition_id}:
    get:
      summary: Retrieve a backup_definition by backup_definition_id
      description: Only backup_definitions you have permission to view will be returned
      operationId: getV1BackupDefinitionsBackupDefinition
      x-api-path-slug: v1backup-definitionsbackup-definition-id-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_definition_id
        description: ID of the backup_definition to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
      - Backup
      - Definition
      - Id
    put:
      summary: Update the specified backup_definition
      description: Only backup_definitions you have permission to change can be modified
      operationId: putV1BackupDefinitionsBackupDefinition
      x-api-path-slug: v1backup-definitionsbackup-definition-id-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: formData
        name: backup_definition[description]
        description: Description of the backup_definition
      - in: formData
        name: backup_definition[name]
        description: Name for the backup_definition
      - in: formData
        name: backup_definition[published]
        description: Boolean flag indicating whether the backup definition is published
          and available for use
      - in: path
        name: backup_definition_id
        description: ID of the backup_definition to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
      - Backup
      - Definition
      - Id
  /v1/backup_definitions/{backup_definition_id}/variables:
    get:
      summary: Retrieve a list of variables for the specified backup_definition
      description: You can only retrieve variables for backup_definitions you have
        access to. Records are returned in ascending order (by id), with a default
        of 20 per page. Links to the next, previous, first, and last pages can be
        found in the response headers.
      operationId: getV1BackupDefinitionsBackupDefinitionVariables
      x-api-path-slug: v1backup-definitionsbackup-definition-idvariables-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_definition_id
        description: ID of the backup_definition to retrieve variables for
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
      - Backup
      - Definition
      - Id
      - Variables
    post:
      summary: Create a new variable for the specified key for the specified backup_definition
      description: It is only possible to create variables for backup_definitions
        you have permission to manage.
      operationId: postV1BackupDefinitionsBackupDefinitionVariables
      x-api-path-slug: v1backup-definitionsbackup-definition-idvariables-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_definition_id
        description: ID of the backup_definition to create a variable for
      - in: formData
        name: variable[default_value]
        description: A default value that can be used when no instance specific value
          is provided
      - in: formData
        name: variable[description]
        description: Description offering additional information or detail about the
          variable
      - in: formData
        name: variable[key]
        description: The symbolic name or identifier to access the defined variable
          by
      - in: formData
        name: variable[name]
        description: A human-friendly name for the variable
      - in: formData
        name: variable[optional]
        description: Flag indicating whether this variable is optional or if a value
          is required
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
      - Backup
      - Definition
      - Id
      - Variables
  /v1/backup_definitions/{backup_definition_id}/variables/{key}:
    get:
      summary: Retrieve a specific variable by key for the specified backup_definition
      description: You can only retrieve variables for backup_definitions you have
        access to
      operationId: getV1BackupDefinitionsBackupDefinitionVariablesKey
      x-api-path-slug: v1backup-definitionsbackup-definition-idvariableskey-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_definition_id
        description: ID of the backup_definition to retrieve a variable for
      - in: path
        name: key
        description: The key, symbolic name, or identifier of the variable to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
      - Backup
      - Definition
      - Id
      - Variables
      - Key
    put:
      summary: Update a specific variable by key for the specified backup_definition
      description: You can only update variables for backup_definitions you have access
        to. Additionally, it is not possible to update a variable's key. Requests
        including a modified key name will result in an error.
      operationId: putV1BackupDefinitionsBackupDefinitionVariablesKey
      x-api-path-slug: v1backup-definitionsbackup-definition-idvariableskey-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_definition_id
        description: ID of the backup_definition to retrieve a variable for
      - in: path
        name: key
        description: The key, symbolic name, or identifier of the variable to update
      - in: formData
        name: name
        description: The human-friendly name to use for the variable
      - in: formData
        name: variable[default_value]
        description: A default value that can be used when no instance specific value
          is provided
      - in: formData
        name: variable[description]
        description: Description offering additional information or detail about the
          variable
      - in: formData
        name: variable[optional]
        description: Flag indicating whether this variable is optional or if a value
          is required
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Definitions
      - Backup
      - Definition
      - Id
      - Variables
      - Key
  /v1/backup_instances:
    get:
      summary: Retrieves a list of backup_instances associated with the specified
        backup_definition
      description: It is only possible to retrieve backup_instances for customers
        you are authorized to access. Records are returned in ascending order (by
        id), with a default of 20 per page. Links to the next, previous, first, and
        last pages can be found in the response headers.
      operationId: getV1BackupInstances
      x-api-path-slug: v1backup-instances-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: query
        name: backup_definition_id
        description: ID of the backup_definition to retrieve backup_instances for
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
    post:
      summary: Create a new backup_instance from the specified backup_definition for
        the specified customer
      description: Create a new backup_instance from the specified backup_definition
        for the specified customer.
      operationId: postV1BackupInstances
      x-api-path-slug: v1backup-instances-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: formData
        name: backup_instance[backup_definition_id]
        description: ID of the backup_definition to create a backup_instance for
      - in: formData
        name: backup_instance[backup_frequency]
        description: Frequency with which scheduled backups are performed
      - in: formData
        name: backup_instance[customer_id]
        description: ID of the customer to create the backup_instance for
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
  /v1/backup_instances/{backup_instance_id}:
    get:
      summary: Retrieve a backup_instance by backup_instance_id
      description: Only backup_instances you have permission to view will be returned
      operationId: getV1BackupInstancesBackupInstance
      x-api-path-slug: v1backup-instancesbackup-instance-id-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
    put:
      summary: Modify the specified backup_instance
      description: Only backup_instances you have permission to change can be modified
      operationId: putV1BackupInstancesBackupInstance
      x-api-path-slug: v1backup-instancesbackup-instance-id-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: formData
        name: backup_instance[backup_frequency]
        description: Frequency with which scheduled backups will be performed
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
  /v1/backup_instances/{backup_instance_id}/backups:
    get:
      summary: Retrieve a list of all backups for the specified backup_instance.
      description: Only backups belonging to backup_instances you have permission
        to manage can be retrieved. Records are returned in ascending order (by id),
        with a default of 20 per page. Links to the next, previous, first, and last
        pages can be found in the response headers.
      operationId: getV1BackupInstancesBackupInstanceBackups
      x-api-path-slug: v1backup-instancesbackup-instance-idbackups-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to backup
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Backups
    post:
      summary: Perform an immediate backup of the specified backup_instance
      description: Only backup_instances you have permission to manage can be backed
        up
      operationId: postV1BackupInstancesBackupInstanceBackups
      x-api-path-slug: v1backup-instancesbackup-instance-idbackups-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to backup
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Backups
  /v1/backup_instances/{backup_instance_id}/backups/active:
    get:
      summary: Retrieve the active backup for the specified backup_instance if one
        exists
      description: Only backups belonging to backup_instances you have permission
        to access can be retrieved
      operationId: getV1BackupInstancesBackupInstanceBackupsActive
      x-api-path-slug: v1backup-instancesbackup-instance-idbackupsactive-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance the requested backup belongs to
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Backups
      - Active
  /v1/backup_instances/{backup_instance_id}/backups/{backup_id}:
    get:
      summary: Retrieve the specified backup for the specified backup_instance
      description: Only backups belonging to backup_instances you have permission
        to access can be retrieved
      operationId: getV1BackupInstancesBackupInstanceBackupsBackup
      x-api-path-slug: v1backup-instancesbackup-instance-idbackupsbackup-id-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_id
        description: ID of the backup to retrieve
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance the requested backup belongs to
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Backups
      - Backup
      - Id
  /v1/backup_instances/{backup_instance_id}/endpoints:
    get:
      summary: Retrieve a list of endpoints for the specified backup_instance
      description: You can only retrieve endpoints for backup_instances you have access
        to. Records are returned in ascending order (by id), with a default of 20
        per page. Links to the next, previous, first, and last pages can be found
        in the response headers.
      operationId: getV1BackupInstancesBackupInstanceEndpoints
      x-api-path-slug: v1backup-instancesbackup-instance-idendpoints-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an endpoint for
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Endpoints
  /v1/backup_instances/{backup_instance_id}/endpoints/{endpoint_name}:
    get:
      summary: Retrieve a specific endpoint by name for the specified backup_instance
      description: You can only retrieve endpoints for backup_instances you have access
        to
      operationId: getV1BackupInstancesBackupInstanceEndpointsEndpointName
      x-api-path-slug: v1backup-instancesbackup-instance-idendpointsendpoint-name-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an endpoint for
      - in: path
        name: endpoint_name
        description: The name of the endpoint to retrieve as defined by the backup_definition
          of the specified backup_instance
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Endpoints
      - Endpoint
      - Name
  /v1/backup_instances/{backup_instance_id}/endpoints/{endpoint_name}/records:
    get:
      summary: Retrieve a list of records stored for the specified endpoint and backup_instance
      description: You can only retrieve records for endpoints that belong to backup_instances
        you have access to. Records are returned in ascending order (by id), with
        a default of 20 per page. Links to the next, previous, first, and last pages
        can be found in the response headers.
      operationId: getV1BackupInstancesBackupInstanceEndpointsEndpointNameRecords
      x-api-path-slug: v1backup-instancesbackup-instance-idendpointsendpoint-namerecords-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an endpoint for
      - in: path
        name: endpoint_name
        description: ID of the endpoint to retrieve records for
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Endpoints
      - Endpoint
      - Name
      - Records
  /v1/backup_instances/{backup_instance_id}/endpoints/{endpoint_name}/records/{record_id}:
    get:
      summary: Retrieve a specific record by id for the specified endpoint and backup_instance
      description: You can only retrieve records for endpoints of backup_instances
        you have access to
      operationId: getV1BackupInstancesBackupInstanceEndpointsEndpointNameRecordsRecord
      x-api-path-slug: v1backup-instancesbackup-instance-idendpointsendpoint-namerecordsrecord-id-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an endpoint for
      - in: path
        name: endpoint_name
        description: The name of the endpoint to retrieve the record from
      - in: path
        name: record_id
        description: The id of the endpoint record to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Endpoints
      - Endpoint
      - Name
      - Records
      - Record
      - Id
  /v1/backup_instances/{backup_instance_id}/endpoints/{endpoint_name}/records/{record_id}/blob:
    get:
      summary: Retrieve the blob associated with the specified record for the specified
        endpoint and backup_instance
      description: Retrieve the blob associated with the specified record for the
        specified endpoint and backup_instance.
      operationId: getV1BackupInstancesBackupInstanceEndpointsEndpointNameRecordsRecordBlob
      x-api-path-slug: v1backup-instancesbackup-instance-idendpointsendpoint-namerecordsrecord-idblob-get
      parameters:
      - in: header
        name: Access-Token
        description: Access Token granted from client credentials authorizing vendor
          to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an endpoint for
      - in: path
        name: endpoint_name
        description: The name of the endpoint to retrieve the record from
      - in: path
        name: record_id
        description: The id of the endpoint record the blob belongs to
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Endpoints
      - Endpoint
      - Name
      - Records
      - Record
      - Id
      - Blob
  /v1/backup_instances/{backup_instance_id}/exports:
    get:
      summary: Retrieve a list of exports for the specified backup_instance
      description: You can only retrieve exports for backup_instances you have access
        to. Records are returned in ascending order (by id), with a default of 20
        per page. Links to the next, previous, first, and last pages can be found
        in the response headers.
      operationId: getV1BackupInstancesBackupInstanceExports
      x-api-path-slug: v1backup-instancesbackup-instance-idexports-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve exports for
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Exports
    post:
      summary: Perform an export of the most recent backup of the specified backup_instance
      description: Perform an export of the most recent backup of the specified backup_instance.
      operationId: postV1BackupInstancesBackupInstanceExports
      x-api-path-slug: v1backup-instancesbackup-instance-idexports-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to export
      - in: formData
        name: export_run[backup_run_id]
        description: ID of a specific backup_run to export
      - in: formData
        name: export_run[content_types]
        description: Comma separated list of blob content-types to export
      - in: formData
        name: export_run[export_datetime]
        description: 'Date (format: YYYY-MM-DD) from which to export'
      - in: formData
        name: export_run[export_formats]
        description: Comma separated list of export format options
      - in: formData
        name: export_run[force_full]
        description: Flag to force a full export, as opposed to re-authorizing an
          old export if the data is the same
      - in: formData
        name: export_run[send_confirmation]
        description: Flag to send a confirmation email w/export link upon completion
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Exports
  /v1/backup_instances/{backup_instance_id}/exports/{export_id}:
    get:
      summary: Retrieve a specific export for the specified backup_instance
      description: You can only retrieve exports for backup_instances you have access
        to
      operationId: getV1BackupInstancesBackupInstanceExportsExport
      x-api-path-slug: v1backup-instancesbackup-instance-idexportsexport-id-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an export for
      - in: path
        name: export_id
        description: ID of the export to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Exports
      - Export
      - Id
  /v1/backup_instances/{backup_instance_id}/exports/{export_id}/reauth:
    post:
      summary: Retrieve an updated exported_data_url for a specific export for the
        specified backup_instance
      description: Retrieve an updated exported_data_url for a specific export for
        the specified backup_instance.
      operationId: postV1BackupInstancesBackupInstanceExportsExportReauth
      x-api-path-slug: v1backup-instancesbackup-instance-idexportsexport-idreauth-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an export for
      - in: path
        name: export_id
        description: ID of the export to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Exports
      - Export
      - Id
      - Reauth
  /v1/backup_instances/{backup_instance_id}/logs:
    get:
      summary: Returns the logs for a given backup instance
      description: Returns the logs for a given backup instance.
      operationId: getV1BackupInstancesBackupInstanceLogs
      x-api-path-slug: v1backup-instancesbackup-instance-idlogs-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to pull logs for
      - in: query
        name: date
        description: 'Date (format: YYYY-MM-DD) for which to fetch logs (default:
          today)'
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Logs
  /v1/backup_instances/{backup_instance_id}/logs/{scroll_id}:
    get:
      summary: Returns the logs for a given backup instance
      description: Returns the logs for a given backup instance.
      operationId: getV1BackupInstancesBackupInstanceLogsScroll
      x-api-path-slug: v1backup-instancesbackup-instance-idlogsscroll-id-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to pull logs for
      - in: path
        name: scroll_id
        description: scroll_id for pagination
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Logs
      - Scroll
      - Id
  /v1/backup_instances/{backup_instance_id}/variables:
    get:
      summary: Retrieve a list of variables for the specified backup_instance
      description: You can only retrieve variables for backup_instances you have access
        to. Records are returned in ascending order (by id), with a default of 20
        per page. Links to the next, previous, first, and last pages can be found
        in the response headers.
      operationId: getV1BackupInstancesBackupInstanceVariables
      x-api-path-slug: v1backup-instancesbackup-instance-idvariables-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve variables for
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Variables
    post:
      summary: Create a custom variable value for the specified key for the specified
        backup_instance
      description: The key specified must refer to the key of a previously defined
        backup_definition variable. It is only possible to create variables for backup_instances
        you have permission to manage.
      operationId: postV1BackupInstancesBackupInstanceVariables
      x-api-path-slug: v1backup-instancesbackup-instance-idvariables-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to create a variable for
      - in: formData
        name: variable[key]
        description: The key, as defined by the backup_definition, to set a value
          for
      - in: formData
        name: variable[value]
        description: The value or information to store for the specified key
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Variables
  /v1/backup_instances/{backup_instance_id}/variables/{key}:
    get:
      summary: Retrieve a specific variable by key for the specified backup_instance
      description: You can only retrieve variables for backup_instances you have access
        to
      operationId: getV1BackupInstancesBackupInstanceVariablesKey
      x-api-path-slug: v1backup-instancesbackup-instance-idvariableskey-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve a variable for
      - in: path
        name: key
        description: The key of the variable to retrieve as defined by the backup_definition
          of the specified backup_instance
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Variables
      - Key
    put:
      summary: Update the value of a variable by key for the specified backup_instance
      description: You can only alter variables for backup_instances you have access
        to manage
      operationId: putV1BackupInstancesBackupInstanceVariablesKey
      x-api-path-slug: v1backup-instancesbackup-instance-idvariableskey-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to update a variable for
      - in: path
        name: key
        description: The key of the variable to update as defined by the backup_definition
          of the specified backup_instance
      - in: formData
        name: variable[value]
        description: The updated data to store at the specified key
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Variables
      - Key
  /v1/customers:
    get:
      summary: Retrieve a list of customers associated with the authenticated vendor
      description: Requires Access Token granted from client credentials. Records
        are returned in ascending order (by id), with a default of 20 per page. Links
        to the next, previous, first, and last pages can be found in the response
        headers.
      operationId: getV1Customers
      x-api-path-slug: v1customers-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      responses:
        200:
          description: OK
      tags:
      - V1
      - Customers
    post:
      summary: Create a new customer instance identified by the given {name} identifier
      description: Create a new customer instance identified by the given {name} identifier.
      operationId: postV1Customers
      x-api-path-slug: v1customers-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: formData
        name: customer[email]
        description: Email address associated with the customer
      - in: formData
        name: customer[name]
        description: Vendor provided ID uniquely identifying customer
      responses:
        200:
          description: OK
      tags:
      - V1
      - Customers
  /v1/customers/{customer_id}:
    get:
      summary: Retrieves the customer identified by customer_id
      description: Requires Access Token granted from client credentials.
      operationId: getV1CustomersCustomer
      x-api-path-slug: v1customerscustomer-id-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: customer_id
        description: ID of the customer to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Customers
      - Customer
      - Id
    put:
      summary: Update a customer instance identified by the given customer_id
      description: Update a customer instance identified by the given customer_id.
      operationId: putV1CustomersCustomer
      x-api-path-slug: v1customerscustomer-id-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: formData
        name: customer[name]
        description: Vendor provided ID uniquely identifying customer
      - in: path
        name: customer_id
        description: ID of the customer to modify
      responses:
        200:
          description: OK
      tags:
      - V1
      - Customers
      - Customer
      - Id
  /v1/customers/{customer_id}/backup_instances:
    get:
      summary: Retrieves a list of backup_instances associated with the specified
        customer
      description: It is only possible to retrieve backup_instances for customers
        you are authorized to access. Records are returned in ascending order (by
        id), with a default of 20 per page. Links to the next, previous, first, and
        last pages can be found in the response headers.
      operationId: getV1CustomersCustomerBackupInstances
      x-api-path-slug: v1customerscustomer-idbackup-instances-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: customer_id
        description: ID of the customer to retrieve backup_instances for
      responses:
        200:
          description: OK
      tags:
      - V1
      - Customers
      - Customer
      - Id
      - Backup
      - Instances
  /v1/ping:
    get:
      summary: A simple method that returns a 200 response if the connection succeeds
      description: A simple method that returns a 200 response if the connection succeeds.
      operationId: getV1Ping
      x-api-path-slug: v1ping-get
      responses:
        200:
          description: OK
      tags:
      - V1
      - Ping
  /v1/vendors/me:
    get:
      summary: Provides information about the currently authenticated vendor user
      description: Provides information about the currently authenticated vendor user.
      operationId: getV1VendorsMe
      x-api-path-slug: v1vendorsme-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      responses:
        200:
          description: OK
      tags:
      - V1
      - Vendors
      - Me