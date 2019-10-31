swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 1
info:
  title: AWS Database Migration Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddTagsToResource:
    get:
      summary: Add Tags To Resource
      description: Adds metadata tags to a DMS resource, including replication instance,
        endpoint, security group, and migration task.
      operationId: addTagsToResource
      x-api-path-slug: actionaddtagstoresource-get
      parameters:
      - in: query
        name: ResourceArn
        description: The Amazon Resource Name (ARN) of the AWS DMS resource the tag
          is to be added to
        type: string
      - in: query
        name: Tags
        description: The tag to be assigned to the DMS resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
  /?Action=CreateEndpoint:
    get:
      summary: Create Endpoint
      description: Creates an endpoint using the provided settings.
      operationId: createEndpoint
      x-api-path-slug: actioncreateendpoint-get
      parameters:
      - in: query
        name: CertificateArn
        description: The Amazon Resource Number (ARN) for the certificate
        type: string
      - in: query
        name: DatabaseName
        description: The name of the endpoint database
        type: string
      - in: query
        name: EndpointIdentifier
        description: The database endpoint identifier
        type: string
      - in: query
        name: EndpointType
        description: The type of endpoint
        type: string
      - in: query
        name: EngineName
        description: The type of engine for the endpoint
        type: string
      - in: query
        name: ExtraConnectionAttributes
        description: Additional attributes associated with the connection
        type: string
      - in: query
        name: KmsKeyId
        description: The KMS key identifier that will be used to encrypt the connection
          parameters
        type: string
      - in: query
        name: Password
        description: The password to be used to login to the endpoint database
        type: string
      - in: query
        name: Port
        description: The port used by the endpoint database
        type: string
      - in: query
        name: ServerName
        description: The name of the server where the endpoint database resides
        type: string
      - in: query
        name: SslMode
        description: The SSL mode to use for the SSL connection
        type: string
      - in: query
        name: Tags
        description: Tags to be added to the endpoint
        type: string
      - in: query
        name: Username
        description: The user name to be used to login to the endpoint database
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /?Action=CreateReplicationInstance:
    get:
      summary: Create Replication Instance
      description: Creates the replication instance using the specified parameters.
      operationId: createReplicationInstance
      x-api-path-slug: actioncreatereplicationinstance-get
      parameters:
      - in: query
        name: AllocatedStorage
        description: The amount of storage (in gigabytes) to be initially allocated
          for the replication instance
        type: string
      - in: query
        name: AutoMinorVersionUpgrade
        description: Indicates that minor engine upgrades will be applied automatically
          to the replication instance during the maintenance window
        type: string
      - in: query
        name: AvailabilityZone
        description: The EC2 Availability Zone that the replication instance will
          be created in
        type: string
      - in: query
        name: EngineVersion
        description: The engine version number of the replication instance
        type: string
      - in: query
        name: KmsKeyId
        description: The KMS key identifier that will be used to encrypt the content
          on the replication instance
        type: string
      - in: query
        name: MultiAZ
        description: Specifies if the replication instance is a Multi-AZ deployment
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range during which system maintenance can occur,
          in Universal Coordinated Time (UTC)
        type: string
      - in: query
        name: PubliclyAccessible
        description: Specifies the accessibility options for the replication instance
        type: string
      - in: query
        name: ReplicationInstanceClass
        description: The compute and memory capacity of the replication instance as
          specified by the replication instance class
        type: string
      - in: query
        name: ReplicationInstanceIdentifier
        description: The replication instance identifier
        type: string
      - in: query
        name: ReplicationSubnetGroupIdentifier
        description: A subnet group to associate with the replication instance
        type: string
      - in: query
        name: Tags
        description: Tags to be associated with the replication instance
        type: string
      - in: query
        name: VpcSecurityGroupIds
        description: Specifies the VPC security group to be used with the replication
          instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Instances
  /?Action=CreateReplicationSubnetGroup:
    get:
      summary: Create Replication Subnet Group
      description: Creates a replication subnet group given a list of the subnet IDs
        in a VPC.
      operationId: createReplicationSubnetGroup
      x-api-path-slug: actioncreatereplicationsubnetgroup-get
      parameters:
      - in: query
        name: ReplicationSubnetGroupDescription
        description: The description for the subnet group
        type: string
      - in: query
        name: ReplicationSubnetGroupIdentifier
        description: The name for the replication subnet group
        type: string
      - in: query
        name: SubnetIds
        description: The EC2 subnet IDs for the subnet group
        type: string
      - in: query
        name: Tags
        description: The tag to be assigned to the subnet group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Subnet Group
  /?Action=CreateReplicationTask:
    get:
      summary: Create Replication Task
      description: Creates a replication task using the specified parameters.
      operationId: createReplicationTask
      x-api-path-slug: actioncreatereplicationtask-get
      parameters:
      - in: query
        name: CdcStartTime
        description: The start time for the Change Data Capture (CDC) operation
        type: string
      - in: query
        name: MigrationType
        description: The migration type
        type: string
      - in: query
        name: ReplicationInstanceArn
        description: The Amazon Resource Name (ARN) of the replication instance
        type: string
      - in: query
        name: ReplicationTaskIdentifier
        description: The replication task identifier
        type: string
      - in: query
        name: ReplicationTaskSettings
        description: Settings for the task, such as target metadata settings
        type: string
      - in: query
        name: SourceEndpointArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the endpoint
        type: string
      - in: query
        name: TableMappings
        description: The path of the JSON file that contains the table mappings
        type: string
      - in: query
        name: Tags
        description: Tags to be added to the replication instance
        type: string
      - in: query
        name: TargetEndpointArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the endpoint
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Tasks
  /?Action=DeleteCertificate:
    get:
      summary: Delete Certificate
      description: Deletes the specified certificate.
      operationId: deleteCertificate
      x-api-path-slug: actiondeletecertificate-get
      parameters:
      - in: query
        name: CertificateArn
        description: The Amazon Resource Name (ARN) of the deleted certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=DeleteEndpoint:
    get:
      summary: Delete Endpoint
      description: Deletes the specified endpoint.
      operationId: deleteEndpoint
      x-api-path-slug: actiondeleteendpoint-get
      parameters:
      - in: query
        name: EndpointArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the endpoint
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /?Action=DeleteReplicationInstance:
    get:
      summary: Delete Replication Instance
      description: Deletes the specified replication instance.
      operationId: deleteReplicationInstance
      x-api-path-slug: actiondeletereplicationinstance-get
      parameters:
      - in: query
        name: ReplicationInstanceArn
        description: The Amazon Resource Name (ARN) of the replication instance to
          be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Instances
  /?Action=DeleteReplicationSubnetGroup:
    get:
      summary: Delete Replication Subnet Group
      description: Deletes a subnet group.
      operationId: deleteReplicationSubnetGroup
      x-api-path-slug: actiondeletereplicationsubnetgroup-get
      parameters:
      - in: query
        name: ReplicationSubnetGroupIdentifier
        description: The subnet group name of the replication instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Subnet Group
  /?Action=DeleteReplicationTask:
    get:
      summary: Delete Replication Task
      description: Deletes the specified replication task.
      operationId: deleteReplicationTask
      x-api-path-slug: actiondeletereplicationtask-get
      parameters:
      - in: query
        name: ReplicationTaskArn
        description: The Amazon Resource Name (ARN) of the replication task to be
          deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Tasks
  /?Action=DescribeAccountAttributes:
    get:
      summary: Describe Account Attributes
      description: Lists all of the AWS DMS attributes for a customer account.
      operationId: describeAccountAttributes
      x-api-path-slug: actiondescribeaccountattributes-get
      parameters:
      - in: query
        name: AccountQuotas
        description: Account quota information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Attributes
  /?Action=DescribeCertificates:
    get:
      summary: Describe Certificates
      description: Provides a description of the certificate.
      operationId: describeCertificates
      x-api-path-slug: actiondescribecertificates-get
      parameters:
      - in: query
        name: Filters
        description: Filters applied to the certificate described in the form of key-value
          pairs
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous         request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=DescribeConnections:
    get:
      summary: Describe Connections
      description: Describes the status of the connections that have been made between
        the replication instance and an endpoint.
      operationId: describeConnections
      x-api-path-slug: actiondescribeconnections-get
      parameters:
      - in: query
        name: Filters
        description: The filters applied to the connection
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Connections
  /?Action=DescribeEndpoints:
    get:
      summary: Describe Endpoints
      description: Returns information about the endpoints for your account in the
        current region.
      operationId: describeEndpoints
      x-api-path-slug: actiondescribeendpoints-get
      parameters:
      - in: query
        name: Filters
        description: Filters applied to the describe action
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /?Action=DescribeEndpointTypes:
    get:
      summary: Describe Endpoint Types
      description: Returns information about the type of endpoints available.
      operationId: describeEndpointTypes
      x-api-path-slug: actiondescribeendpointtypes-get
      parameters:
      - in: query
        name: Filters
        description: Filters applied to the describe action
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoint Types
  /?Action=DescribeOrderableReplicationInstances:
    get:
      summary: Describe Orderable Replication Instances
      description: Returns information about the replication instance types that can
        be created in the specified region.
      operationId: describeOrderableReplicationInstances
      x-api-path-slug: actiondescribeorderablereplicationinstances-get
      parameters:
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Instances
  /?Action=DescribeRefreshSchemasStatus:
    get:
      summary: Describe Refresh Schemas Status
      description: Returns the status of the RefreshSchemas operation.
      operationId: describeRefreshSchemasStatus
      x-api-path-slug: actiondescriberefreshschemasstatus-get
      parameters:
      - in: query
        name: EndpointArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the endpoint
        type: string
      responses:
        200:
          description: OK
      tags:
      - Schemas
  /?Action=DescribeReplicationInstances:
    get:
      summary: Describe Replication Instances
      description: Returns information about replication instances for your account
        in the current region.
      operationId: describeReplicationInstances
      x-api-path-slug: actiondescribereplicationinstances-get
      parameters:
      - in: query
        name: Filters
        description: Filters applied to the describe action
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Instances
  /?Action=DescribeReplicationSubnetGroups:
    get:
      summary: Describe Replication Subnet Groups
      description: Returns information about the replication subnet groups.
      operationId: describeReplicationSubnetGroups
      x-api-path-slug: actiondescribereplicationsubnetgroups-get
      parameters:
      - in: query
        name: Filters
        description: Filters applied to the describe action
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Instances
  /?Action=DescribeReplicationTasks:
    get:
      summary: Describe Replication Tasks
      description: Returns information about replication tasks for your account in
        the current region.
      operationId: describeReplicationTasks
      x-api-path-slug: actiondescribereplicationtasks-get
      parameters:
      - in: query
        name: Filters
        description: Filters applied to the describe action
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous     request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Tasks
  /?Action=DescribeSchemas:
    get:
      summary: Describe Schemas
      description: Returns information about the schema for the specified endpoint.
      operationId: describeSchemas
      x-api-path-slug: actiondescribeschemas-get
      parameters:
      - in: query
        name: EndpointArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the endpoint
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous     request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Schemas
  /?Action=DescribeTableStatistics:
    get:
      summary: Describe Table Statistics
      description: Returns table statistics on the database migration task, including
        table name, rows inserted, rows updated, and rows deleted.
      operationId: describeTableStatistics
      x-api-path-slug: actiondescribetablestatistics-get
      parameters:
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: ReplicationTaskArn
        description: The Amazon Resource Name (ARN) of the replication task
        type: string
      responses:
        200:
          description: OK
      tags:
      - Table Statistics
  /?Action=ImportCertificate:
    get:
      summary: Import Certificate
      description: Uploads the specified certificate.
      operationId: importCertificate
      x-api-path-slug: actionimportcertificate-get
      parameters:
      - in: query
        name: CertificateIdentifier
        description: The customer-assigned name of the certificate
        type: string
      - in: query
        name: CertificatePem
        description: 'The contents of the '
        type: string
      - in: query
        name: CertificateWallet
        description: The location of the imported Oracle Wallet certificate for use
          with SSL
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: Lists all tags for an AWS DMS resource.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: ResourceArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the AWS DMS resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
  /?Action=ModifyEndpoint:
    get:
      summary: Modify Endpoint
      description: Modifies the specified endpoint.
      operationId: modifyEndpoint
      x-api-path-slug: actionmodifyendpoint-get
      parameters:
      - in: query
        name: CertificateArn
        description: The Amazon Resource Name (ARN) of the certificate used for SSL
          connection
        type: string
      - in: query
        name: DatabaseName
        description: The name of the endpoint database
        type: string
      - in: query
        name: EndpointArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the endpoint
        type: string
      - in: query
        name: EndpointIdentifier
        description: The database endpoint identifier
        type: string
      - in: query
        name: EndpointType
        description: The type of endpoint
        type: string
      - in: query
        name: EngineName
        description: The type of engine for the endpoint
        type: string
      - in: query
        name: ExtraConnectionAttributes
        description: Additional attributes associated with the connection
        type: string
      - in: query
        name: Password
        description: The password to be used to login to the endpoint database
        type: string
      - in: query
        name: Port
        description: The port used by the endpoint database
        type: string
      - in: query
        name: ServerName
        description: The name of the server where the endpoint database resides
        type: string
      - in: query
        name: SslMode
        description: The SSL mode to be used
        type: string
      - in: query
        name: Username
        description: The user name to be used to login to the endpoint database
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /?Action=ModifyReplicationInstance:
    get:
      summary: Modify Replication Instance
      description: Modifies the replication instance to apply new settings.
      operationId: modifyReplicationInstance
      x-api-path-slug: actionmodifyreplicationinstance-get
      parameters:
      - in: query
        name: AllocatedStorage
        description: The amount of storage (in gigabytes) to be allocated for the
          replication instance
        type: string
      - in: query
        name: AllowMajorVersionUpgrade
        description: Indicates that major version upgrades are allowed
        type: string
      - in: query
        name: ApplyImmediately
        description: Indicates whether the changes should be applied immediately or
          during the next maintenance window
        type: string
      - in: query
        name: AutoMinorVersionUpgrade
        description: Indicates that minor version upgrades will be applied automatically     to
          the replication instance during the maintenance window
        type: string
      - in: query
        name: EngineVersion
        description: The engine version number of the replication instance
        type: string
      - in: query
        name: MultiAZ
        description: Specifies if the replication instance is a Multi-AZ deployment
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range (in UTC) during which system maintenance
          can occur, which might result in an outage
        type: string
      - in: query
        name: ReplicationInstanceArn
        description: The Amazon Resource Name (ARN) of the replication instance
        type: string
      - in: query
        name: ReplicationInstanceClass
        description: The compute and memory capacity of the replication instance
        type: string
      - in: query
        name: ReplicationInstanceIdentifier
        description: The replication instance identifier
        type: string
      - in: query
        name: VpcSecurityGroupIds
        description: Specifies the VPC security group to be used with the replication
          instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Instances
  /?Action=ModifyReplicationSubnetGroup:
    get:
      summary: Modify Replication Subnet Group
      description: Modifies the settings for the specified replication subnet group.
      operationId: modifyReplicationSubnetGroup
      x-api-path-slug: actionmodifyreplicationsubnetgroup-get
      parameters:
      - in: query
        name: ReplicationSubnetGroupDescription
        description: The description of the replication instance subnet group
        type: string
      - in: query
        name: ReplicationSubnetGroupIdentifier
        description: The name of the replication instance subnet group
        type: string
      - in: query
        name: SubnetIds
        description: A list of subnet IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Subnet Groups
  /?Action=ModifyReplicationTask:
    get:
      summary: Modify Replication Task
      description: Modifies the specified replication task.
      operationId: modifyReplicationTask
      x-api-path-slug: actionmodifyreplicationtask-get
      parameters:
      - in: query
        name: CdcStartTime
        description: The start time for the Change Data Capture (CDC) operation
        type: string
      - in: query
        name: MigrationType
        description: The migration type
        type: string
      - in: query
        name: ReplicationTaskArn
        description: The Amazon Resource Name (ARN) of the replication task
        type: string
      - in: query
        name: ReplicationTaskIdentifier
        description: The replication task identifier
        type: string
      - in: query
        name: ReplicationTaskSettings
        description: JSON file that contains settings for the task, such as target
          metadata settings
        type: string
      - in: query
        name: TableMappings
        description: The path of the JSON file that contains the table mappings
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Tasks
  /?Action=RefreshSchemas:
    get:
      summary: Refresh Schemas
      description: Populates the schema for the specified endpoint.
      operationId: refreshSchemas
      x-api-path-slug: actionrefreshschemas-get
      parameters:
      - in: query
        name: EndpointArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the endpoint
        type: string
      - in: query
        name: ReplicationInstanceArn
        description: The Amazon Resource Name (ARN) of the replication instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Schemas
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes metadata tags from a DMS resource.
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceArn
        description: '&gt;The Amazon Resource Name (ARN) of the AWS DMS resource the
          tag is to be removed from'
        type: string
      - in: query
        name: TagKeys
        description: The tag key (name) of the tag to be removed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
  /?Action=StartReplicationTask:
    get:
      summary: Start Replication Task
      description: Starts the replication task.
      operationId: startReplicationTask
      x-api-path-slug: actionstartreplicationtask-get
      parameters:
      - in: query
        name: CdcStartTime
        description: The start time for the Change Data Capture (CDC) operation
        type: string
      - in: query
        name: ReplicationTaskArn
        description: The Amazon Resource Number (ARN) of the replication task to be
          started
        type: string
      - in: query
        name: StartReplicationTaskType
        description: The type of replication task
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Tasks
  /?Action=StopReplicationTask:
    get:
      summary: Stop Replication Task
      description: Stops the replication task.
      operationId: stopReplicationTask
      x-api-path-slug: actionstopreplicationtask-get
      parameters:
      - in: query
        name: ReplicationTaskArn
        description: The Amazon Resource Number(ARN) of the replication task to be
          stopped
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Tasks
  /?Action=TestConnection:
    get:
      summary: Test Connection
      description: Tests the connection between the replication instance and the endpoint.
      operationId: testConnection
      x-api-path-slug: actiontestconnection-get
      parameters:
      - in: query
        name: EndpointArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the endpoint
        type: string
      - in: query
        name: ReplicationInstanceArn
        description: The Amazon Resource Name (ARN) of the replication instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Connections