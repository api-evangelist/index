swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 1
info:
  title: AWS RDS API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddRoleToDBCluster:
    get:
      summary: Add Role To D B Cluster
      description: Associates an Identity and Access Management (IAM) role from an
        Aurora DB cluster.
      operationId: addroletodbcluster
      x-api-path-slug: actionaddroletodbcluster-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The name of the DB cluster to associate the IAM role with
        type: string
      - in: query
        name: RoleArn
        description: The Amazon Resource Name (ARN) of the IAM role to associate with
          the Aurora DB cluster, for example            arn:aws:iam::123456789012:role/AuroraAccessRole
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=AddSourceIdentifierToSubscription:
    get:
      summary: Add Source Identifier To Subscription
      description: Adds a source identifier to an existing RDS event notification
        subscription.
      operationId: addsourceidentifiertosubscription
      x-api-path-slug: actionaddsourceidentifiertosubscription-get
      parameters:
      - in: query
        name: SourceIdentifier
        description: The identifier of the event source to be added
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the RDS event notification subscription you want
          to add a source identifier to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=AddTagsToResource:
    get:
      summary: Add Tags To Resource
      description: Adds metadata tags to an Amazon RDS resource.
      operationId: addtagstoresource
      x-api-path-slug: actionaddtagstoresource-get
      parameters:
      - in: query
        name: ResourceName
        description: The Amazon RDS resource the tags will be added to
        type: string
      - in: query
        name: Tags.Tag.N
        description: The tags to be assigned to the Amazon RDS resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=ApplyPendingMaintenanceAction:
    get:
      summary: Apply Pending Maintenance Action
      description: Applies a pending maintenance action to a resource (for example,
        to a DB instance).
      operationId: applypendingmaintenanceaction
      x-api-path-slug: actionapplypendingmaintenanceaction-get
      parameters:
      - in: query
        name: ApplyAction
        description: The pending maintenance action to apply to this resource
        type: string
      - in: query
        name: OptInType
        description: A value that specifies the type of opt-in request, or undoes
          an opt-in request
        type: string
      - in: query
        name: ResourceIdentifier
        description: The RDS Amazon Resource Name (ARN) of the resource that the       pending
          maintenance action applies to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance Actions
  /?Action=AuthorizeDBSecurityGroupIngress:
    get:
      summary: Authorize D B Security Group Ingress
      description: Enables ingress to a DBSecurityGroup using one of two forms of
        authorization.
      operationId: authorizedbsecuritygroupingress
      x-api-path-slug: actionauthorizedbsecuritygroupingress-get
      parameters:
      - in: query
        name: CIDRIP
        description: The IP range to authorize
        type: string
      - in: query
        name: DBSecurityGroupName
        description: The name of the DB security group to add authorization to
        type: string
      - in: query
        name: EC2SecurityGroupId
        description: Id of the EC2 security group to authorize
        type: string
      - in: query
        name: EC2SecurityGroupName
        description: Name of the EC2 security group to authorize
        type: string
      - in: query
        name: EC2SecurityGroupOwnerId
        description: AWS account number of the owner of the EC2 security group        specified
          in the EC2SecurityGroupName parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Groups
  /?Action=CopyDBClusterParameterGroup:
    get:
      summary: Copy D B Cluster Parameter Group
      description: Copies the specified DB cluster parameter group.
      operationId: copydbclusterparametergroup
      x-api-path-slug: actioncopydbclusterparametergroup-get
      parameters:
      - in: query
        name: SourceDBClusterParameterGroupIdentifier
        description: The identifier or Amazon Resource Name (ARN) for the source DB
          cluster parameter group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TargetDBClusterParameterGroupDescription
        description: A description for the copied DB cluster parameter group
        type: string
      - in: query
        name: TargetDBClusterParameterGroupIdentifier
        description: The identifier for the copied DB cluster parameter group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=CopyDBClusterSnapshot:
    get:
      summary: Copy D B Cluster Snapshot
      description: Creates a snapshot of a DB cluster.
      operationId: copydbclustersnapshot
      x-api-path-slug: actioncopydbclustersnapshot-get
      parameters:
      - in: query
        name: SourceDBClusterSnapshotIdentifier
        description: The identifier of the DB cluster snapshot to copy
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TargetDBClusterSnapshotIdentifier
        description: The identifier of the new DB cluster snapshot to create from
          the source DB cluster snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=CopyDBParameterGroup:
    get:
      summary: Copy D B Parameter Group
      description: Copies the specified DB parameter group.
      operationId: copydbparametergroup
      x-api-path-slug: actioncopydbparametergroup-get
      parameters:
      - in: query
        name: SourceDBParameterGroupIdentifier
        description: The identifier or ARN for the source DB parameter group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TargetDBParameterGroupDescription
        description: A description for the copied DB parameter group
        type: string
      - in: query
        name: TargetDBParameterGroupIdentifier
        description: The identifier for the copied DB parameter group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter Groups
  /?Action=CopyDBSnapshot:
    get:
      summary: Copy D B Snapshot
      description: Copies the specified DB snapshot.
      operationId: copydbsnapshot
      x-api-path-slug: actioncopydbsnapshot-get
      parameters:
      - in: query
        name: CopyTags
        description: True to copy all tags from the source DB snapshot to the target
          DB snapshot; otherwise false
        type: string
      - in: query
        name: KmsKeyId
        description: The AWS KMS key ID for an encrypted DB snapshot
        type: string
      - in: query
        name: PreSignedUrl
        description: The URL that contains a Signature Version 4 signed request for
          the CopyDBSnapshot API action in the AWS region that contains the             source
          DB snapshot to copy
        type: string
      - in: query
        name: SourceDBSnapshotIdentifier
        description: The identifier for the source DB snapshot
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TargetDBSnapshotIdentifier
        description: The identifier for the copied snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=CopyOptionGroup:
    get:
      summary: Copy Option Group
      description: Copies the specified option group.
      operationId: copyoptiongroup
      x-api-path-slug: actioncopyoptiongroup-get
      parameters:
      - in: query
        name: SourceOptionGroupIdentifier
        description: The identifier or ARN for the source option group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TargetOptionGroupDescription
        description: The description for the copied option group
        type: string
      - in: query
        name: TargetOptionGroupIdentifier
        description: The identifier for the copied option group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Option Groups
  /?Action=CreateDBCluster:
    get:
      summary: Create D B Cluster
      description: Creates a new Amazon Aurora DB cluster.
      operationId: createdbcluster
      x-api-path-slug: actioncreatedbcluster-get
      parameters:
      - in: query
        name: AvailabilityZones.AvailabilityZone.N
        description: A list of EC2 Availability Zones that instances in the DB cluster
          can be created in
        type: string
      - in: query
        name: BackupRetentionPeriod
        description: The number of days for which automated backups are retained
        type: string
      - in: query
        name: CharacterSetName
        description: A value that indicates that the DB cluster should be associated
          with the specified CharacterSet
        type: string
      - in: query
        name: DatabaseName
        description: The name for your database of up to 8 alpha-numeric characters
        type: string
      - in: query
        name: DBClusterIdentifier
        description: The DB cluster identifier
        type: string
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group to associate            with
          this DB cluster
        type: string
      - in: query
        name: DBSubnetGroupName
        description: A DB subnet group to associate with this DB cluster
        type: string
      - in: query
        name: Engine
        description: The name of the database engine to be used for this DB cluster
        type: string
      - in: query
        name: EngineVersion
        description: The version number of the database engine to use
        type: string
      - in: query
        name: KmsKeyId
        description: The KMS key identifier for an encrypted DB cluster
        type: string
      - in: query
        name: MasterUsername
        description: The name of the master user for the DB cluster
        type: string
      - in: query
        name: MasterUserPassword
        description: The password for the master database user
        type: string
      - in: query
        name: OptionGroupName
        description: A value that indicates that the DB cluster should be associated
          with the specified option group
        type: string
      - in: query
        name: Port
        description: The port number on which the instances in the DB cluster accept
          connections
        type: string
      - in: query
        name: PreferredBackupWindow
        description: The daily time range during which automated backups are created        if
          automated backups are enabled        using the BackupRetentionPeriod parameter
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range during which system maintenance can occur,
          in Universal Coordinated Time (UTC)
        type: string
      - in: query
        name: ReplicationSourceIdentifier
        description: The Amazon Resource Name (ARN) of the source DB cluster if this
          DB cluster is created as a Read Replica
        type: string
      - in: query
        name: StorageEncrypted
        description: Specifies whether the DB cluster is encrypted
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of EC2 VPC security groups to associate with this DB cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=CreateDBClusterParameterGroup:
    get:
      summary: Create D B Cluster Parameter Group
      description: Creates a new DB cluster parameter group.
      operationId: createdbclusterparametergroup
      x-api-path-slug: actioncreatedbclusterparametergroup-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group
        type: string
      - in: query
        name: DBParameterGroupFamily
        description: The DB cluster parameter group family name
        type: string
      - in: query
        name: Description
        description: The description for the DB cluster parameter group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=CreateDBClusterSnapshot:
    get:
      summary: Create D B Cluster Snapshot
      description: Creates a snapshot of a DB cluster.
      operationId: createdbclustersnapshot
      x-api-path-slug: actioncreatedbclustersnapshot-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The identifier of the DB cluster to create a snapshot for
        type: string
      - in: query
        name: DBClusterSnapshotIdentifier
        description: The identifier of the DB cluster snapshot
        type: string
      - in: query
        name: Tags.Tag.N
        description: The tags to be assigned to the DB cluster snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=CreateDBInstance:
    get:
      summary: Create D B Instance
      description: Creates a new DB instance.
      operationId: createdbinstance
      x-api-path-slug: actioncreatedbinstance-get
      parameters:
      - in: query
        name: AllocatedStorage
        description: The amount of storage (in gigabytes) to be initially allocated
          for the database instance
        type: string
      - in: query
        name: AutoMinorVersionUpgrade
        description: Indicates that minor engine upgrades will be applied automatically
          to the DB instance during the maintenance window
        type: string
      - in: query
        name: AvailabilityZone
        description: The EC2 Availability Zone that the database instance will be
          created in
        type: string
      - in: query
        name: BackupRetentionPeriod
        description: The number of days for which automated backups are retained
        type: string
      - in: query
        name: CharacterSetName
        description: For supported engines, indicates that the DB instance should
          be associated with the specified CharacterSet
        type: string
      - in: query
        name: CopyTagsToSnapshot
        description: True to copy all tags from the DB instance to snapshots of the
          DB instance; otherwise false
        type: string
      - in: query
        name: DBClusterIdentifier
        description: The identifier of the DB cluster that the instance will belong
          to
        type: string
      - in: query
        name: DBInstanceClass
        description: The compute and memory capacity of the DB instance
        type: string
      - in: query
        name: DBInstanceIdentifier
        description: The DB instance identifier
        type: string
      - in: query
        name: DBName
        description: The meaning of this parameter differs according to the database
          engine you use
        type: string
      - in: query
        name: DBParameterGroupName
        description: The name of the DB parameter group to associate with this DB
          instance
        type: string
      - in: query
        name: DBSecurityGroups.DBSecurityGroupName.N
        description: A list of DB security groups to associate with this DB instance
        type: string
      - in: query
        name: DBSubnetGroupName
        description: A DB subnet group to associate with this DB instance
        type: string
      - in: query
        name: Domain
        description: Specify the Active Directory Domain to create the instance in
        type: string
      - in: query
        name: DomainIAMRoleName
        description: Specify the name of the IAM role to be used when making API calls
          to the Directory Service
        type: string
      - in: query
        name: Engine
        description: The name of the database engine to be used for this instance
        type: string
      - in: query
        name: EngineVersion
        description: The version number of the database engine to use
        type: string
      - in: query
        name: Iops
        description: The amount of Provisioned IOPS (input/output operations per second)
          to be initially allocated for the DB instance
        type: string
      - in: query
        name: KmsKeyId
        description: The KMS key identifier for an encrypted DB instance
        type: string
      - in: query
        name: LicenseModel
        description: License model information for this DB instance
        type: string
      - in: query
        name: MasterUsername
        description: The name of master user for the client DB instance
        type: string
      - in: query
        name: MasterUserPassword
        description: The password for the master database user
        type: string
      - in: query
        name: MonitoringInterval
        description: The interval, in seconds, between points when Enhanced Monitoring
          metrics are collected for the DB instance
        type: string
      - in: query
        name: MonitoringRoleArn
        description: The ARN for the IAM role that permits RDS to send enhanced monitoring
          metrics to CloudWatch Logs
        type: string
      - in: query
        name: MultiAZ
        description: Specifies if the DB instance is a Multi-AZ deployment
        type: string
      - in: query
        name: OptionGroupName
        description: Indicates that the DB instance should be associated with the
          specified option group
        type: string
      - in: query
        name: Port
        description: The port number on which the database accepts connections
        type: string
      - in: query
        name: PreferredBackupWindow
        description: The daily time range during which automated backups are created        if
          automated backups are enabled,        using the BackupRetentionPeriod parameter
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range during which system maintenance can occur,
          in Universal Coordinated Time (UTC)
        type: string
      - in: query
        name: PromotionTier
        description: A value that specifies the order in which an Aurora Replica is
          promoted to the primary instance       after a failure of the existing primary
          instance
        type: string
      - in: query
        name: PubliclyAccessible
        description: Specifies the accessibility options for the DB instance
        type: string
      - in: query
        name: StorageEncrypted
        description: Specifies whether the DB instance is encrypted
        type: string
      - in: query
        name: StorageType
        description: Specifies the storage type to be associated with the DB instance
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TdeCredentialArn
        description: The ARN from the Key Store with which to associate the instance
          for TDE encryption
        type: string
      - in: query
        name: TdeCredentialPassword
        description: The password for the given ARN from the Key Store in order to
          access the device
        type: string
      - in: query
        name: Timezone
        description: The time zone of the DB instance
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of EC2 VPC security groups to associate with this DB instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=CreateDBInstanceReadReplica:
    get:
      summary: Create D B Instance Read Replica
      description: Creates a DB instance for a DB instance running MySQL, MariaDB,
        or PostgreSQL that acts as a Read Replica of a source DB instance.
      operationId: createdbinstancereadreplica
      x-api-path-slug: actioncreatedbinstancereadreplica-get
      parameters:
      - in: query
        name: AutoMinorVersionUpgrade
        description: Indicates that minor engine upgrades will be applied automatically
          to the Read Replica during the maintenance window
        type: string
      - in: query
        name: AvailabilityZone
        description: The Amazon EC2 Availability Zone that the Read Replica will be
          created in
        type: string
      - in: query
        name: CopyTagsToSnapshot
        description: True to copy all tags from the Read Replica to snapshots of the
          Read Replica; otherwise false
        type: string
      - in: query
        name: DBInstanceClass
        description: The compute and memory capacity of the Read Replica
        type: string
      - in: query
        name: DBInstanceIdentifier
        description: The DB instance identifier of the Read Replica
        type: string
      - in: query
        name: DBSubnetGroupName
        description: Specifies a DB subnet group for the DB instance
        type: string
      - in: query
        name: Iops
        description: The amount of Provisioned IOPS (input/output operations per second)
          to be initially allocated for the DB instance
        type: string
      - in: query
        name: MonitoringInterval
        description: The interval, in seconds, between points when Enhanced Monitoring
          metrics are collected for the Read Replica
        type: string
      - in: query
        name: MonitoringRoleArn
        description: The ARN for the IAM role that permits RDS to send enhanced monitoring
          metrics to CloudWatch Logs
        type: string
      - in: query
        name: OptionGroupName
        description: The option group the DB instance will be associated with
        type: string
      - in: query
        name: Port
        description: The port number that the DB instance uses for connections
        type: string
      - in: query
        name: PubliclyAccessible
        description: Specifies the accessibility options for the DB instance
        type: string
      - in: query
        name: SourceDBInstanceIdentifier
        description: The identifier of the DB instance that will act as the source
          for the Read Replica
        type: string
      - in: query
        name: StorageType
        description: Specifies the storage type to be associated with the Read Replica
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=CreateDBParameterGroup:
    get:
      summary: Create D B Parameter Group
      description: Creates a new DB parameter group.
      operationId: createdbparametergroup
      x-api-path-slug: actioncreatedbparametergroup-get
      parameters:
      - in: query
        name: DBParameterGroupFamily
        description: The DB parameter group family name
        type: string
      - in: query
        name: DBParameterGroupName
        description: The name of the DB parameter group
        type: string
      - in: query
        name: Description
        description: The description for the DB parameter group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter Groups
  /?Action=CreateDBSecurityGroup:
    get:
      summary: Create D B Security Group
      description: Creates a new DB security group.
      operationId: createdbsecuritygroup
      x-api-path-slug: actioncreatedbsecuritygroup-get
      parameters:
      - in: query
        name: DBSecurityGroupDescription
        description: The description for the DB security group
        type: string
      - in: query
        name: DBSecurityGroupName
        description: The name for the DB security group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Groups
  /?Action=CreateDBSnapshot:
    get:
      summary: Create D B Snapshot
      description: Creates a DBSnapshot.
      operationId: createdbsnapshot
      x-api-path-slug: actioncreatedbsnapshot-get
      parameters:
      - in: query
        name: DBInstanceIdentifier
        description: The DB instance identifier
        type: string
      - in: query
        name: DBSnapshotIdentifier
        description: The identifier for the DB snapshot
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=CreateDBSubnetGroup:
    get:
      summary: Create D B Subnet Group
      description: Creates a new DB subnet group.
      operationId: createdbsubnetgroup
      x-api-path-slug: actioncreatedbsubnetgroup-get
      parameters:
      - in: query
        name: DBSubnetGroupDescription
        description: The description for the DB subnet group
        type: string
      - in: query
        name: DBSubnetGroupName
        description: The name for the DB subnet group
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: The EC2 Subnet IDs for the DB subnet group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnet Groups
  /?Action=CreateEventSubscription:
    get:
      summary: Create Event Subscription
      description: Creates an RDS event notification subscription.
      operationId: createeventsubscription
      x-api-path-slug: actioncreateeventsubscription-get
      parameters:
      - in: query
        name: Enabled
        description: A Boolean value; set to true to activate the subscription, set
          to false to create the subscription but not active it
        type: string
      - in: query
        name: EventCategories.EventCategory.N
        description: A list of event categories for a SourceType that you want to
          subscribe to
        type: string
      - in: query
        name: SnsTopicArn
        description: The Amazon Resource Name (ARN) of the SNS topic created for event
          notification
        type: string
      - in: query
        name: SourceIds.SourceId.N
        description: The list of identifiers of the event sources for which events
          will be returned
        type: string
      - in: query
        name: SourceType
        description: The type of source that will be generating the events
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the subscription
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=CreateOptionGroup:
    get:
      summary: Create Option Group
      description: Creates a new option group.
      operationId: createoptiongroup
      x-api-path-slug: actioncreateoptiongroup-get
      parameters:
      - in: query
        name: EngineName
        description: Specifies the name of the engine that this option group should
          be associated with
        type: string
      - in: query
        name: MajorEngineVersion
        description: Specifies the major version of the engine that this option group
          should be associated with
        type: string
      - in: query
        name: OptionGroupDescription
        description: The description of the option group
        type: string
      - in: query
        name: OptionGroupName
        description: Specifies the name of the option group to be created
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Option Groups
  /?Action=DeleteDBCluster:
    get:
      summary: Delete D B Cluster
      description: The DeleteDBCluster action deletes a previously provisioned DB
        cluster.
      operationId: deletedbcluster
      x-api-path-slug: actiondeletedbcluster-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The DB cluster identifier for the DB cluster to be deleted
        type: string
      - in: query
        name: FinalDBSnapshotIdentifier
        description: The DB cluster snapshot identifier of the new DB cluster snapshot
          created when SkipFinalSnapshot      is set to false
        type: string
      - in: query
        name: SkipFinalSnapshot
        description: Determines whether a final DB cluster snapshot is created before
          the DB cluster is deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DeleteDBClusterParameterGroup:
    get:
      summary: Delete D B Cluster Parameter Group
      description: Deletes a specified DB cluster parameter group.
      operationId: deletedbclusterparametergroup
      x-api-path-slug: actiondeletedbclusterparametergroup-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=DeleteDBClusterSnapshot:
    get:
      summary: Delete D B Cluster Snapshot
      description: Deletes a DB cluster snapshot.
      operationId: deletedbclustersnapshot
      x-api-path-slug: actiondeletedbclustersnapshot-get
      parameters:
      - in: query
        name: DBClusterSnapshotIdentifier
        description: The identifier of the DB cluster snapshot to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=DeleteDBInstance:
    get:
      summary: Delete D B Instance
      description: The DeleteDBInstance action deletes a previously provisioned DB
        instance.
      operationId: deletedbinstance
      x-api-path-slug: actiondeletedbinstance-get
      parameters:
      - in: query
        name: DBInstanceIdentifier
        description: The DB instance identifier for the DB instance to be deleted
        type: string
      - in: query
        name: FinalDBSnapshotIdentifier
        description: The DBSnapshotIdentifier of the new DBSnapshot created when SkipFinalSnapshot        is
          set to false
        type: string
      - in: query
        name: SkipFinalSnapshot
        description: Determines whether a final DB snapshot is created before the
          DB instance is deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=DeleteDBParameterGroup:
    get:
      summary: Delete D B Parameter Group
      description: Deletes a specified DBParameterGroup.
      operationId: deletedbparametergroup
      x-api-path-slug: actiondeletedbparametergroup-get
      parameters:
      - in: query
        name: DBParameterGroupName
        description: The name of the DB parameter group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter Groups
  /?Action=DeleteDBSecurityGroup:
    get:
      summary: Delete D B Security Group
      description: Deletes a DB security group.
      operationId: deletedbsecuritygroup
      x-api-path-slug: actiondeletedbsecuritygroup-get
      parameters:
      - in: query
        name: DBSecurityGroupName
        description: The name of the DB security group to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Groups
  /?Action=DeleteDBSnapshot:
    get:
      summary: Delete D B Snapshot
      description: Deletes a DBSnapshot.
      operationId: deletedbsnapshot
      x-api-path-slug: actiondeletedbsnapshot-get
      parameters:
      - in: query
        name: DBSnapshotIdentifier
        description: The DBSnapshot identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DeleteDBSubnetGroup:
    get:
      summary: Delete D B Subnet Group
      description: Deletes a DB subnet group.
      operationId: deletedbsubnetgroup
      x-api-path-slug: actiondeletedbsubnetgroup-get
      parameters:
      - in: query
        name: DBSubnetGroupName
        description: The name of the database subnet group to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnet Groups
  /?Action=DeleteEventSubscription:
    get:
      summary: Delete Event Subscription
      description: Deletes an RDS event notification subscription.
      operationId: deleteeventsubscription
      x-api-path-slug: actiondeleteeventsubscription-get
      parameters:
      - in: query
        name: SubscriptionName
        description: The name of the RDS event notification subscription you want
          to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=DeleteOptionGroup:
    get:
      summary: Delete Option Group
      description: Deletes an existing option group.
      operationId: deleteoptiongroup
      x-api-path-slug: actiondeleteoptiongroup-get
      parameters:
      - in: query
        name: OptionGroupName
        description: The name of the option group to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Option Groups
  /?Action=DescribeAccountAttributes:
    get:
      summary: Describe Account Attributes
      description: Lists all of the attributes for a customer account.
      operationId: describeaccountattributes
      x-api-path-slug: actiondescribeaccountattributes-get
      parameters:
      - in: query
        name: AccountQuotas.AccountQuota.N
        description: A list of AccountQuota objects
        type: string
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /?Action=DescribeCertificates:
    get:
      summary: Describe Certificates
      description: Lists the set of CA certificates provided by Amazon RDS for this
        AWS account.
      operationId: describecertificates
      x-api-path-slug: actiondescribecertificates-get
      parameters:
      - in: query
        name: CertificateIdentifier
        description: The user-supplied certificate identifier
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeCertificates
          request
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
  /?Action=DescribeDBClusterParameterGroups:
    get:
      summary: Describe D B Cluster Parameter Groups
      description: Returns a list of DBClusterParameterGroup descriptions.
      operationId: describedbclusterparametergroups
      x-api-path-slug: actiondescribedbclusterparametergroups-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of a specific DB cluster parameter group to return details
          for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeDBClusterParameterGroups
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=DescribeDBClusterParameters:
    get:
      summary: Describe D B Cluster Parameters
      description: Returns the detailed parameter list for a particular DB cluster
        parameter group.
      operationId: describedbclusterparameters
      x-api-path-slug: actiondescribedbclusterparameters-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of a specific DB cluster parameter group to return parameter
          details for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      DescribeDBClusterParameters
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: Source
        description: A value that indicates to return only parameters for a specific
          source
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameters
  /?Action=DescribeDBClusters:
    get:
      summary: Describe D B Clusters
      description: Returns information about provisioned Aurora DB clusters.
      operationId: describedbclusters
      x-api-path-slug: actiondescribedbclusters-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The user-supplied DB cluster identifier
        type: string
      - in: query
        name: Filters.Filter.N
        description: A filter that specifies one or more DB clusters to describe
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous            DescribeDBClusters
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DescribeDBClusterSnapshotAttributes:
    get:
      summary: Describe D B Cluster Snapshot Attributes
      description: Returns a list of DB cluster snapshot attribute names and values
        for a manual DB cluster snapshot.
      operationId: describedbclustersnapshotattributes
      x-api-path-slug: actiondescribedbclustersnapshotattributes-get
      parameters:
      - in: query
        name: DBClusterSnapshotIdentifier
        description: The identifier for the DB cluster snapshot to describe the attributes
          for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=DescribeDBClusterSnapshots:
    get:
      summary: Describe D B Cluster Snapshots
      description: Returns information about DB cluster snapshots.
      operationId: describedbclustersnapshots
      x-api-path-slug: actiondescribedbclustersnapshots-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The ID of the DB cluster to retrieve the list of DB cluster snapshots
          for
        type: string
      - in: query
        name: DBClusterSnapshotIdentifier
        description: A specific DB cluster snapshot identifier to describe
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: IncludePublic
        description: Set this value to true to include manual DB cluster snapshots
          that are public and can be copied             or restored by any AWS account,
          otherwise set this value to false
        type: string
      - in: query
        name: IncludeShared
        description: Set this value to true to include shared manual DB cluster snapshots             from
          other AWS accounts that this AWS account has been given             permission
          to copy or restore, otherwise set this value to false
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous            DescribeDBClusterSnapshots
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: SnapshotType
        description: The type of DB cluster snapshots to be returned
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=DescribeDBEngineVersions:
    get:
      summary: Describe D B Engine Versions
      description: Returns a list of the available DB engines.
      operationId: describedbengineversions
      x-api-path-slug: actiondescribedbengineversions-get
      parameters:
      - in: query
        name: DBParameterGroupFamily
        description: The name of a specific DB parameter group family to return details
          for
        type: string
      - in: query
        name: DefaultOnly
        description: Indicates that only the default version of the specified engine
          or engine and major version combination is returned
        type: string
      - in: query
        name: Engine
        description: The database engine to return
        type: string
      - in: query
        name: EngineVersion
        description: The database engine version to return
        type: string
      - in: query
        name: Filters.Filter.N
        description: Not currently supported
        type: string
      - in: query
        name: ListSupportedCharacterSets
        description: If this parameter is specified           and the requested engine
          supports the CharacterSetName parameter for CreateDBInstance,           the
          response includes a list of supported character sets for each engine version
        type: string
      - in: query
        name: ListSupportedTimezones
        description: If this parameter is specified             and the requested
          engine supports the TimeZone parameter for CreateDBInstance,             the
          response includes a list of supported time zones for each engine version
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Engines
  /?Action=DescribeDBInstances:
    get:
      summary: Describe D B Instances
      description: Returns information about provisioned RDS instances.
      operationId: describedbinstances
      x-api-path-slug: actiondescribedbinstances-get
      parameters:
      - in: query
        name: DBInstanceIdentifier
        description: The user-supplied instance identifier
        type: string
      - in: query
        name: Filters.Filter.N
        description: A filter that specifies one or more DB instances to describe
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeDBInstances
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=DescribeDBLogFiles:
    get:
      summary: Describe D B Log Files
      description: Returns a list of DB log files for the DB instance.
      operationId: describedblogfiles
      x-api-path-slug: actiondescribedblogfiles-get
      parameters:
      - in: query
        name: DBInstanceIdentifier
        description: The customer-assigned name of the DB instance that contains the
          log files you want to list
        type: string
      - in: query
        name: FileLastWritten
        description: Filters the available log files for files written since the specified
          date, in POSIX timestamp format with milliseconds
        type: string
      - in: query
        name: FilenameContains
        description: Filters the available log files for log file names that contain
          the specified string
        type: string
      - in: query
        name: FileSize
        description: Filters the available log files for files larger than the specified
          size
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: The pagination token provided in the previous request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Blog Files
  /?Action=DescribeDBParameterGroups:
    get:
      summary: Describe D B Parameter Groups
      description: Returns a list of DBParameterGroup descriptions.
      operationId: describedbparametergroups
      x-api-path-slug: actiondescribedbparametergroups-get
      parameters:
      - in: query
        name: DBParameterGroupName
        description: The name of a specific DB parameter group to return details for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeDBParameterGroups
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter Groups
  /?Action=DescribeDBParameters:
    get:
      summary: Describe D B Parameters
      description: Returns the detailed parameter list for a particular DB parameter
        group.
      operationId: describedbparameters
      x-api-path-slug: actiondescribedbparameters-get
      parameters:
      - in: query
        name: DBParameterGroupName
        description: The name of a specific DB parameter group to return details for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeDBParameters
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: Source
        description: The parameter types to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameters
  /?Action=DescribeDBSecurityGroups:
    get:
      summary: Describe D B Security Groups
      description: Returns a list of DBSecurityGroup descriptions.
      operationId: describedbsecuritygroups
      x-api-path-slug: actiondescribedbsecuritygroups-get
      parameters:
      - in: query
        name: DBSecurityGroupName
        description: The name of the DB security group to return details for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeDBSecurityGroups
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Groups
  /?Action=DescribeDBSnapshotAttributes:
    get:
      summary: Describe D B Snapshot Attributes
      description: Returns a list of DB snapshot attribute names and values for a
        manual DB snapshot.
      operationId: describedbsnapshotattributes
      x-api-path-slug: actiondescribedbsnapshotattributes-get
      parameters:
      - in: query
        name: DBSnapshotIdentifier
        description: The identifier for the DB snapshot to describe the attributes
          for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DescribeDBSnapshots:
    get:
      summary: Describe D B Snapshots
      description: Returns information about DB snapshots.
      operationId: describedbsnapshots
      x-api-path-slug: actiondescribedbsnapshots-get
      parameters:
      - in: query
        name: DBInstanceIdentifier
        description: The ID of the DB instance to retrieve the list of DB snapshots
          for
        type: string
      - in: query
        name: DBSnapshotIdentifier
        description: A specific DB snapshot identifier to describe
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: IncludePublic
        description: Set this value to true to include manual DB snapshots that are
          public and can be copied or restored           by any AWS account, otherwise
          set this value to false
        type: string
      - in: query
        name: IncludeShared
        description: Set this value to true to include shared manual DB snapshots
          from other           AWS accounts that this AWS account has been given permission
          to copy or restore, otherwise set this value to false
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeDBSnapshots
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: SnapshotType
        description: The type of snapshots to be returned
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DescribeDBSubnetGroups:
    get:
      summary: Describe D B Subnet Groups
      description: Returns a list of DBSubnetGroup descriptions.
      operationId: describedbsubnetgroups
      x-api-path-slug: actiondescribedbsubnetgroups-get
      parameters:
      - in: query
        name: DBSubnetGroupName
        description: The name of the DB subnet group to return details for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous DescribeDBSubnetGroups
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnet Groups
  /?Action=DescribeEngineDefaultClusterParameters:
    get:
      summary: Describe Engine Default Cluster Parameters
      description: Returns the default engine and system parameter information for
        the cluster database engine.
      operationId: describeenginedefaultclusterparameters
      x-api-path-slug: actiondescribeenginedefaultclusterparameters-get
      parameters:
      - in: query
        name: DBParameterGroupFamily
        description: The name of the DB cluster parameter group family to return engine
          parameter information for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      DescribeEngineDefaultClusterParameters
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Default Cluster Parameters
  /?Action=DescribeEngineDefaultParameters:
    get:
      summary: Describe Engine Default Parameters
      description: Returns the default engine and system parameter information for
        the specified database engine.
      operationId: describeenginedefaultparameters
      x-api-path-slug: actiondescribeenginedefaultparameters-get
      parameters:
      - in: query
        name: DBParameterGroupFamily
        description: The name of the DB parameter group family
        type: string
      - in: query
        name: Filters.Filter.N
        description: Not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeEngineDefaultParameters
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Default Parameters
  /?Action=DescribeEventCategories:
    get:
      summary: Describe Event Categories
      description: Displays a list of categories for all event source types, or, if
        specified, for a specified source type.
      operationId: describeeventcategories
      x-api-path-slug: actiondescribeeventcategories-get
      parameters:
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: SourceType
        description: The type of source that will be generating the events
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Categories
  /?Action=DescribeEvents:
    get:
      summary: Describe Events
      description: Returns events related to DB instances, DB security groups, DB
        snapshots, and DB parameter groups for the past 14 days.
      operationId: describeevents
      x-api-path-slug: actiondescribeevents-get
      parameters:
      - in: query
        name: Duration
        description: The number of minutes to retrieve events for
        type: string
      - in: query
        name: EndTime
        description: The end of the time interval for which to retrieve events,        specified
          in ISO 8601 format
        type: string
      - in: query
        name: EventCategories.EventCategory.N
        description: A list of event categories that trigger notifications for a event
          notification subscription
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeEvents
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: SourceIdentifier
        description: The identifier of the event source for which events will be returned
        type: string
      - in: query
        name: SourceType
        description: The event source to retrieve events for
        type: string
      - in: query
        name: StartTime
        description: The beginning of the time interval to retrieve events for,        specified
          in ISO 8601 format
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
  /?Action=DescribeEventSubscriptions:
    get:
      summary: Describe Event Subscriptions
      description: Lists all the subscription descriptions for a customer account.
      operationId: describeeventsubscriptions
      x-api-path-slug: actiondescribeeventsubscriptions-get
      parameters:
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous            DescribeOrderableDBInstanceOptions
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the RDS event notification subscription you want
          to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=DescribeOptionGroupOptions:
    get:
      summary: Describe Option Group Options
      description: Describes all available options.
      operationId: describeoptiongroupoptions
      x-api-path-slug: actiondescribeoptiongroupoptions-get
      parameters:
      - in: query
        name: EngineName
        description: A required parameter
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: MajorEngineVersion
        description: If specified, filters the results to include only options for
          the specified major engine version
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Option Groups
  /?Action=DescribeOptionGroups:
    get:
      summary: Describe Option Groups
      description: Describes the available option groups.
      operationId: describeoptiongroups
      x-api-path-slug: actiondescribeoptiongroups-get
      parameters:
      - in: query
        name: EngineName
        description: Filters the list of option groups to only include groups associated
          with a specific database engine
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: MajorEngineVersion
        description: Filters the list of option groups to only include groups associated
          with a specific database engine version
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous DescribeOptionGroups
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: OptionGroupName
        description: The name of the option group to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Option Groups
  /?Action=DescribeOrderableDBInstanceOptions:
    get:
      summary: Describe Orderable D B Instance Options
      description: Returns a list of orderable DB instance options for the specified
        engine.
      operationId: describeorderabledbinstanceoptions
      x-api-path-slug: actiondescribeorderabledbinstanceoptions-get
      parameters:
      - in: query
        name: DBInstanceClass
        description: The DB instance class filter value
        type: string
      - in: query
        name: Engine
        description: The name of the engine to retrieve DB instance options for
        type: string
      - in: query
        name: EngineVersion
        description: The engine version filter value
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: LicenseModel
        description: The license model filter value
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous            DescribeOrderableDBInstanceOptions
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: Vpc
        description: The VPC filter value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=DescribePendingMaintenanceActions:
    get:
      summary: Describe Pending Maintenance Actions
      description: Returns a list of resources (for example, DB instances) that have
        at least one pending maintenance action.
      operationId: describependingmaintenanceactions
      x-api-path-slug: actiondescribependingmaintenanceactions-get
      parameters:
      - in: query
        name: Filters.Filter.N
        description: A filter that specifies one or more resources to return pending
          maintenance actions for
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous            DescribePendingMaintenanceActions
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: ResourceIdentifier
        description: The ARN of a resource to return pending maintenance actions for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance Actions
  /?Action=DescribeReservedDBInstances:
    get:
      summary: Describe Reserved D B Instances
      description: Returns information about reserved DB instances for this account,
        or about a specified reserved DB instance.
      operationId: describereserveddbinstances
      x-api-path-slug: actiondescribereserveddbinstances-get
      parameters:
      - in: query
        name: DBInstanceClass
        description: The DB instance class filter value
        type: string
      - in: query
        name: Duration
        description: The duration filter value, specified in years or seconds
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: MultiAZ
        description: The Multi-AZ filter value
        type: string
      - in: query
        name: OfferingType
        description: The offering type filter value
        type: string
      - in: query
        name: ProductDescription
        description: The product description filter value
        type: string
      - in: query
        name: ReservedDBInstanceId
        description: The reserved DB instance identifier filter value
        type: string
      - in: query
        name: ReservedDBInstancesOfferingId
        description: The offering identifier filter value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=DescribeReservedDBInstancesOfferings:
    get:
      summary: Describe Reserved D B Instances Offerings
      description: Lists available reserved DB instance offerings.
      operationId: describereserveddbinstancesofferings
      x-api-path-slug: actiondescribereserveddbinstancesofferings-get
      parameters:
      - in: query
        name: DBInstanceClass
        description: The DB instance class filter value
        type: string
      - in: query
        name: Duration
        description: Duration filter value, specified in years or seconds
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: MultiAZ
        description: The Multi-AZ filter value
        type: string
      - in: query
        name: OfferingType
        description: The offering type filter value
        type: string
      - in: query
        name: ProductDescription
        description: Product description filter value
        type: string
      - in: query
        name: ReservedDBInstancesOfferingId
        description: The offering identifier filter value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=DescribeSourceRegions:
    get:
      summary: Describe Source Regions
      description: "Returns a list of the source AWS regions where the current AWS
        region can create a Read Replica \n            or copy a DB snapshot from."
      operationId: describesourceregions
      x-api-path-slug: actiondescribesourceregions-get
      parameters:
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous DescribeSourceRegions
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: RegionName
        description: The source region name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Source Regions
  /?Action=DownloadDBLogFilePortion:
    get:
      summary: Download D B Log File Portion
      description: Downloads all or a portion of the specified log file, up to 1 MB
        in size.
      operationId: downloaddblogfileportion
      x-api-path-slug: actiondownloaddblogfileportion-get
      parameters:
      - in: query
        name: DBInstanceIdentifier
        description: The customer-assigned name of the DB instance that contains the
          log files you want to list
        type: string
      - in: query
        name: LogFileName
        description: The name of the log file to be downloaded
        type: string
      - in: query
        name: Marker
        description: The pagination token provided in the previous request or 0
        type: string
      - in: query
        name: NumberOfLines
        description: The number of lines to download
        type: string
      responses:
        200:
          description: OK
      tags:
      - Log Files
  /?Action=FailoverDBCluster:
    get:
      summary: Failover D B Cluster
      description: Forces a failover for a DB cluster.
      operationId: failoverdbcluster
      x-api-path-slug: actionfailoverdbcluster-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: A DB cluster identifier to force a failover for
        type: string
      - in: query
        name: TargetDBInstanceIdentifier
        description: The name of the instance to promote to the primary instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: Lists all tags on an Amazon RDS resource.
      operationId: listtagsforresource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: ResourceName
        description: The Amazon RDS resource with tags to be listed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=ModifyDBCluster:
    get:
      summary: Modify D B Cluster
      description: Modify a setting for an Amazon Aurora DB cluster.
      operationId: modifydbcluster
      x-api-path-slug: actionmodifydbcluster-get
      parameters:
      - in: query
        name: ApplyImmediately
        description: A value that specifies whether the modifications in this request
          and      any pending modifications are asynchronously applied      as soon
          as possible, regardless of the      PreferredMaintenanceWindow setting for
          the DB cluster
        type: string
      - in: query
        name: BackupRetentionPeriod
        description: The number of days for which automated backups are retained
        type: string
      - in: query
        name: DBClusterIdentifier
        description: The DB cluster identifier for the cluster being modified
        type: string
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group to use for the DB
          cluster
        type: string
      - in: query
        name: MasterUserPassword
        description: The new password for the master database user
        type: string
      - in: query
        name: NewDBClusterIdentifier
        description: The new DB cluster identifier for the DB cluster when renaming
          a DB cluster
        type: string
      - in: query
        name: OptionGroupName
        description: A value that indicates that the DB cluster should be associated
          with the specified option group
        type: string
      - in: query
        name: Port
        description: The port number on which the DB cluster accepts connections
        type: string
      - in: query
        name: PreferredBackupWindow
        description: The daily time range during which automated backups are created            if
          automated backups are enabled,            using the BackupRetentionPeriod
          parameter
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range during which system maintenance can occur,
          in Universal Coordinated Time (UTC)
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A lst of VPC security groups that the DB cluster will belong
          to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=ModifyDBClusterParameterGroup:
    get:
      summary: Modify D B Cluster Parameter Group
      description: Modifies the parameters of a DB cluster parameter group.
      operationId: modifydbclusterparametergroup
      x-api-path-slug: actionmodifydbclusterparametergroup-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group to modify
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: A list of parameters in the DB cluster parameter group to modify
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=ModifyDBClusterSnapshotAttribute:
    get:
      summary: Modify D B Cluster Snapshot Attribute
      description: Adds an attribute and values to, or removes an attribute and values
        from, a manual DB cluster snapshot.
      operationId: modifydbclustersnapshotattribute
      x-api-path-slug: actionmodifydbclustersnapshotattribute-get
      parameters:
      - in: query
        name: AttributeName
        description: The name of the DB cluster snapshot attribute to modify
        type: string
      - in: query
        name: DBClusterSnapshotIdentifier
        description: The identifier for the DB cluster snapshot to modify the attributes
          for
        type: string
      - in: query
        name: ValuesToAdd.AttributeValue.N
        description: A list of DB cluster snapshot attributes to add to the attribute
          specified by AttributeName
        type: string
      - in: query
        name: ValuesToRemove.AttributeValue.N
        description: A list of DB cluster snapshot attributes to remove from the attribute
          specified by AttributeName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=ModifyDBInstance:
    get:
      summary: Modify D B Instance
      description: Modifies settings for a DB instance.
      operationId: modifydbinstance
      x-api-path-slug: actionmodifydbinstance-get
      parameters:
      - in: query
        name: AllocatedStorage
        description: The new storage capacity of the RDS instance
        type: string
      - in: query
        name: AllowMajorVersionUpgrade
        description: Indicates that major version upgrades are allowed
        type: string
      - in: query
        name: ApplyImmediately
        description: Specifies whether the modifications in this request and        any
          pending modifications are asynchronously applied        as soon as possible,
          regardless of the        PreferredMaintenanceWindow setting for the DB instance
        type: string
      - in: query
        name: AutoMinorVersionUpgrade
        description: Indicates that minor version upgrades will be applied automatically    to
          the DB instance during the maintenance window
        type: string
      - in: query
        name: BackupRetentionPeriod
        description: The number of days to retain automated backups
        type: string
      - in: query
        name: CACertificateIdentifier
        description: Indicates the certificate that needs to be associated with the
          instance
        type: string
      - in: query
        name: CopyTagsToSnapshot
        description: True to copy all tags from the DB instance to snapshots of the
          DB instance; otherwise false
        type: string
      - in: query
        name: DBInstanceClass
        description: The new compute and memory capacity of the DB instance
        type: string
      - in: query
        name: DBInstanceIdentifier
        description: The DB instance identifier
        type: string
      - in: query
        name: DBParameterGroupName
        description: The name of the DB parameter group to apply to the DB instance
        type: string
      - in: query
        name: DBPortNumber
        description: The port number on which the database accepts connections
        type: string
      - in: query
        name: DBSecurityGroups.DBSecurityGroupName.N
        description: A list of DB security groups to authorize on this DB instance
        type: string
      - in: query
        name: DBSubnetGroupName
        description: The new DB subnet group for the DB instance
        type: string
      - in: query
        name: Domain
        description: The Active Directory Domain to move the instance to
        type: string
      - in: query
        name: DomainIAMRoleName
        description: The name of the IAM role to use when making API calls to the
          Directory Service
        type: string
      - in: query
        name: EngineVersion
        description: The version number of the database engine to upgrade to
        type: string
      - in: query
        name: Iops
        description: The new Provisioned IOPS (I/O operations per second) value for
          the RDS instance
        type: string
      - in: query
        name: LicenseModel
        description: The license model for the DB instance
        type: string
      - in: query
        name: MasterUserPassword
        description: The new password for the DB instance master user
        type: string
      - in: query
        name: MonitoringInterval
        description: The interval, in seconds, between points when Enhanced Monitoring
          metrics are collected for the DB instance
        type: string
      - in: query
        name: MonitoringRoleArn
        description: The ARN for the IAM role that permits RDS to send enhanced monitoring
          metrics to CloudWatch Logs
        type: string
      - in: query
        name: MultiAZ
        description: Specifies if the DB instance is a Multi-AZ deployment
        type: string
      - in: query
        name: NewDBInstanceIdentifier
        description: The new DB instance identifier for the DB instance when renaming
          a DB            instance
        type: string
      - in: query
        name: OptionGroupName
        description: Indicates that the DB instance should be associated with the
          specified option group
        type: string
      - in: query
        name: PreferredBackupWindow
        description: The daily time range during which automated backups are created        if
          automated backups are enabled,        as determined by the BackupRetentionPeriod
          parameter
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range (in UTC) during which system maintenance
          can occur, which might result in an outage
        type: string
      - in: query
        name: PromotionTier
        description: A value that specifies the order in which an Aurora Replica is
          promoted to the primary instance       after a failure of the existing primary
          instance
        type: string
      - in: query
        name: PubliclyAccessible
        description: Boolean value that indicates if the DB instance has a publicly
          resolvable DNS name
        type: string
      - in: query
        name: StorageType
        description: Specifies the storage type to be associated with the DB instance
        type: string
      - in: query
        name: TdeCredentialArn
        description: The ARN from the Key Store with which to associate the instance
          for TDE encryption
        type: string
      - in: query
        name: TdeCredentialPassword
        description: The password for the given ARN from the Key Store in order to
          access the device
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of EC2 VPC security groups to authorize on this DB instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=ModifyDBParameterGroup:
    get:
      summary: Modify D B Parameter Group
      description: Modifies the parameters of a DB parameter group.
      operationId: modifydbparametergroup
      x-api-path-slug: actionmodifydbparametergroup-get
      parameters:
      - in: query
        name: DBParameterGroupName
        description: The name of the DB parameter group
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: An array of parameter names, values, and the apply method for
          the parameter update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter Groups
  /?Action=ModifyDBSnapshotAttribute:
    get:
      summary: Modify D B Snapshot Attribute
      description: Adds an attribute and values to, or removes an attribute and values
        from, a manual DB snapshot.
      operationId: modifydbsnapshotattribute
      x-api-path-slug: actionmodifydbsnapshotattribute-get
      parameters:
      - in: query
        name: AttributeName
        description: The name of the DB snapshot attribute to modify
        type: string
      - in: query
        name: DBSnapshotIdentifier
        description: The identifier for the DB snapshot to modify the attributes for
        type: string
      - in: query
        name: ValuesToAdd.AttributeValue.N
        description: A list of DB snapshot attributes to add to the attribute specified
          by AttributeName
        type: string
      - in: query
        name: ValuesToRemove.AttributeValue.N
        description: A list of DB snapshot attributes to remove from the attribute
          specified by AttributeName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=ModifyDBSubnetGroup:
    get:
      summary: Modify D B Subnet Group
      description: Modifies an existing DB subnet group.
      operationId: modifydbsubnetgroup
      x-api-path-slug: actionmodifydbsubnetgroup-get
      parameters:
      - in: query
        name: DBSubnetGroupDescription
        description: The description for the DB subnet group
        type: string
      - in: query
        name: DBSubnetGroupName
        description: The name for the DB subnet group
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: The EC2 subnet IDs for the DB subnet group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnet Groups
  /?Action=ModifyEventSubscription:
    get:
      summary: Modify Event Subscription
      description: Modifies an existing RDS event notification subscription.
      operationId: modifyeventsubscription
      x-api-path-slug: actionmodifyeventsubscription-get
      parameters:
      - in: query
        name: Enabled
        description: A Boolean value; set to true to activate the subscription
        type: string
      - in: query
        name: EventCategories.EventCategory.N
        description: A list of event categories for a SourceType that you want to
          subscribe to
        type: string
      - in: query
        name: SnsTopicArn
        description: The Amazon Resource Name (ARN) of the SNS topic created for event
          notification
        type: string
      - in: query
        name: SourceType
        description: The type of source that will be generating the events
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the RDS event notification subscription
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=ModifyOptionGroup:
    get:
      summary: Modify Option Group
      description: Modifies an existing option group.
      operationId: modifyoptiongroup
      x-api-path-slug: actionmodifyoptiongroup-get
      parameters:
      - in: query
        name: ApplyImmediately
        description: Indicates whether the changes should be applied immediately,
          or during the next maintenance window for each instance associated with
          the option group
        type: string
      - in: query
        name: OptionGroupName
        description: The name of the option group to be modified
        type: string
      - in: query
        name: OptionsToInclude.OptionConfiguration.N
        description: Options in this list are added to the option group or, if already
          present, the specified configuration is used to update the existing configuration
        type: string
      - in: query
        name: OptionsToRemove.member.N
        description: Options in this list are removed from the option group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Option Groups
  /?Action=PromoteReadReplica:
    get:
      summary: Promote Read Replica
      description: Promotes a Read Replica DB instance to a standalone DB instance.
      operationId: promotereadreplica
      x-api-path-slug: actionpromotereadreplica-get
      parameters:
      - in: query
        name: BackupRetentionPeriod
        description: The number of days to retain automated backups
        type: string
      - in: query
        name: DBInstanceIdentifier
        description: The DB instance identifier
        type: string
      - in: query
        name: PreferredBackupWindow
        description: The daily time range during which automated backups are created        if
          automated backups are enabled,        using the BackupRetentionPeriod parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replicas
  /?Action=PromoteReadReplicaDBCluster:
    get:
      summary: Promote Read Replica D B Cluster
      description: Promotes a Read Replica DB cluster to a standalone DB cluster.
      operationId: promotereadreplicadbcluster
      x-api-path-slug: actionpromotereadreplicadbcluster-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The identifier of the DB cluster Read Replica to promote
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replicas
  /?Action=PurchaseReservedDBInstancesOffering:
    get:
      summary: Purchase Reserved D B Instances Offering
      description: Purchases a reserved DB instance offering.
      operationId: purchasereserveddbinstancesoffering
      x-api-path-slug: actionpurchasereserveddbinstancesoffering-get
      parameters:
      - in: query
        name: DBInstanceCount
        description: The number of instances to reserve
        type: string
      - in: query
        name: ReservedDBInstanceId
        description: Customer-specified identifier to track this reservation
        type: string
      - in: query
        name: ReservedDBInstancesOfferingId
        description: The ID of the Reserved DB instance offering to purchase
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=RebootDBInstance:
    get:
      summary: Reboot D B Instance
      description: Rebooting a DB instance restarts the database engine service.
      operationId: rebootdbinstance
      x-api-path-slug: actionrebootdbinstance-get
      parameters:
      - in: query
        name: DBInstanceIdentifier
        description: The DB instance identifier
        type: string
      - in: query
        name: ForceFailover
        description: When true, the reboot will be conducted through a MultiAZ failover
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=RemoveRoleFromDBCluster:
    get:
      summary: Remove Role From D B Cluster
      description: Disassociates an Identity and Access Management (IAM) role from
        an Aurora DB cluster.
      operationId: removerolefromdbcluster
      x-api-path-slug: actionremoverolefromdbcluster-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The name of the DB cluster to disassociate the IAM role rom
        type: string
      - in: query
        name: RoleArn
        description: The Amazon Resource Name (ARN) of the IAM role to disassociate
          from the Aurora DB cluster, for example        arn:aws:iam::123456789012:role/AuroraAccessRole
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=RemoveSourceIdentifierFromSubscription:
    get:
      summary: Remove Source Identifier From Subscription
      description: Removes a source identifier from an existing RDS event notification
        subscription.
      operationId: removesourceidentifierfromsubscription
      x-api-path-slug: actionremovesourceidentifierfromsubscription-get
      parameters:
      - in: query
        name: SourceIdentifier
        description: The source identifier to be removed from the subscription, such
          as the DB instance identifier             for a DB instance or the name
          of a security group
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the RDS event notification subscription you want
          to remove a source identifier from
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes metadata tags from an Amazon RDS resource.
      operationId: removetagsfromresource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceName
        description: The Amazon RDS resource the tags will be removed from
        type: string
      - in: query
        name: TagKeys.member.N
        description: The tag key (name) of the tag to be removed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=ResetDBClusterParameterGroup:
    get:
      summary: Reset D B Cluster Parameter Group
      description: Modifies the parameters of a DB cluster parameter group to the
        default value.
      operationId: resetdbclusterparametergroup
      x-api-path-slug: actionresetdbclusterparametergroup-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group to reset
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: A list of parameter names in the DB cluster parameter group to
          reset to the default values
        type: string
      - in: query
        name: ResetAllParameters
        description: A value that is set to true to reset all parameters in the DB
          cluster parameter group       to their default values, and false otherwise
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=ResetDBParameterGroup:
    get:
      summary: Reset D B Parameter Group
      description: Modifies the parameters of a DB parameter group to the engine/system
        default value.
      operationId: resetdbparametergroup
      x-api-path-slug: actionresetdbparametergroup-get
      parameters:
      - in: query
        name: DBParameterGroupName
        description: The name of the DB parameter group
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: An array of parameter names, values, and the apply method for
          the parameter update
        type: string
      - in: query
        name: ResetAllParameters
        description: Specifies whether (true) or not (false) to reset all parameters        in
          the DB parameter group to default values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter Groups
  /?Action=RestoreDBClusterFromS3:
    get:
      summary: Restore D B Cluster From S3
      description: Creates an Amazon Aurora DB cluster from data stored in an Amazon
        S3 bucket.
      operationId: restoredbclusterfroms3
      x-api-path-slug: actionrestoredbclusterfroms3-get
      parameters:
      - in: query
        name: AvailabilityZones.AvailabilityZone.N
        description: A list of EC2 Availability Zones that instances in the restored
          DB cluster can be created in
        type: string
      - in: query
        name: BackupRetentionPeriod
        description: The number of days for which automated backups of the restored
          DB cluster are retained
        type: string
      - in: query
        name: CharacterSetName
        description: A value that indicates that the restored DB cluster should be
          associated with the specified CharacterSet
        type: string
      - in: query
        name: DatabaseName
        description: The database name for the restored DB cluster
        type: string
      - in: query
        name: DBClusterIdentifier
        description: The name of the DB cluster to create from the source data in
          the S3 bucket
        type: string
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group to associate            with
          the restored DB cluster
        type: string
      - in: query
        name: DBSubnetGroupName
        description: A DB subnet group to associate with the restored DB cluster
        type: string
      - in: query
        name: Engine
        description: The name of the database engine to be used for the restored DB
          cluster
        type: string
      - in: query
        name: EngineVersion
        description: The version number of the database engine to use
        type: string
      - in: query
        name: KmsKeyId
        description: The KMS key identifier for an encrypted DB cluster
        type: string
      - in: query
        name: MasterUsername
        description: The name of the master user for the restored DB cluster
        type: string
      - in: query
        name: MasterUserPassword
        description: The password for the master database user
        type: string
      - in: query
        name: OptionGroupName
        description: A value that indicates that the restored DB cluster should be
          associated with the specified option group
        type: string
      - in: query
        name: Port
        description: The port number on which the instances in the restored DB cluster
          accept connections
        type: string
      - in: query
        name: PreferredBackupWindow
        description: The daily time range during which automated backups are created            if
          automated backups are enabled            using the BackupRetentionPeriod
          parameter
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range during which system maintenance can occur,
          in Universal Coordinated Time (UTC)
        type: string
      - in: query
        name: S3BucketName
        description: The name of the Amazon S3 bucket that contains the data used
          to create the Amazon Aurora DB cluster
        type: string
      - in: query
        name: S3IngestionRoleArn
        description: The Amazon Resource Name (ARN) of the AWS Identity and Access
          Management (IAM) role that authorizes        Amazon RDS to access the Amazon
          S3 bucket on your behalf
        type: string
      - in: query
        name: S3Prefix
        description: The prefix for all of the file names that contain the data used
          to create the Amazon Aurora DB cluster
        type: string
      - in: query
        name: SourceEngine
        description: The identifier for the database engine that was backed up to
          create the files stored in the            Amazon S3 bucket
        type: string
      - in: query
        name: SourceEngineVersion
        description: The version of the database that the backup files were created
          from
        type: string
      - in: query
        name: StorageEncrypted
        description: Specifies whether the restored DB cluster is encrypted
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of EC2 VPC security groups to associate with the restored
          DB cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=RestoreDBClusterFromSnapshot:
    get:
      summary: Restore D B Cluster From Snapshot
      description: Creates a new DB cluster from a DB cluster snapshot.
      operationId: restoredbclusterfromsnapshot
      x-api-path-slug: actionrestoredbclusterfromsnapshot-get
      parameters:
      - in: query
        name: AvailabilityZones.AvailabilityZone.N
        description: Provides the list of EC2 Availability Zones that instances in
          the restored DB cluster can be created in
        type: string
      - in: query
        name: DatabaseName
        description: The database name for the restored DB cluster
        type: string
      - in: query
        name: DBClusterIdentifier
        description: The name of the DB cluster to create from the DB cluster snapshot
        type: string
      - in: query
        name: DBSubnetGroupName
        description: The name of the DB subnet group to use for the new DB cluster
        type: string
      - in: query
        name: Engine
        description: The database engine to use for the new DB cluster
        type: string
      - in: query
        name: EngineVersion
        description: The version of the database engine to use for the new DB cluster
        type: string
      - in: query
        name: KmsKeyId
        description: The KMS key identifier to use when restoring an encrypted DB
          cluster from a DB cluster snapshot
        type: string
      - in: query
        name: OptionGroupName
        description: The name of the option group to use for the restored DB cluster
        type: string
      - in: query
        name: Port
        description: The port number on which the new DB cluster accepts connections
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The identifier for the DB cluster snapshot to restore from
        type: string
      - in: query
        name: Tags.Tag.N
        description: The tags to be assigned to the restored DB cluster
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of VPC security groups that the new DB cluster will belong
          to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=RestoreDBClusterToPointInTime:
    get:
      summary: Restore D B Cluster To Point In Time
      description: Restores a DB cluster to an arbitrary point in time.
      operationId: restoredbclustertopointintime
      x-api-path-slug: actionrestoredbclustertopointintime-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The name of the new DB cluster to be created
        type: string
      - in: query
        name: DBSubnetGroupName
        description: The DB subnet group name to use for the new DB cluster
        type: string
      - in: query
        name: KmsKeyId
        description: The KMS key identifier to use when restoring an encrypted DB
          cluster from an encrypted DB cluster
        type: string
      - in: query
        name: OptionGroupName
        description: The name of the option group for the new DB cluster
        type: string
      - in: query
        name: Port
        description: The port number on which the new DB cluster accepts connections
        type: string
      - in: query
        name: RestoreToTime
        description: The date and time to restore the DB cluster to
        type: string
      - in: query
        name: SourceDBClusterIdentifier
        description: The identifier of the source DB cluster from which to restore
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: UseLatestRestorableTime
        description: A value that is set to true to restore the DB cluster to the
          latest       restorable backup time, and false otherwise
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A lst of VPC security groups that the new DB cluster belongs
          to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=RestoreDBInstanceFromDBSnapshot:
    get:
      summary: Restore D B Instance From D B Snapshot
      description: Creates a new DB instance from a DB snapshot.
      operationId: restoredbinstancefromdbsnapshot
      x-api-path-slug: actionrestoredbinstancefromdbsnapshot-get
      parameters:
      - in: query
        name: AutoMinorVersionUpgrade
        description: Indicates that minor version upgrades will be applied automatically
          to the DB instance during the maintenance window
        type: string
      - in: query
        name: AvailabilityZone
        description: The EC2 Availability Zone that the database instance will be
          created in
        type: string
      - in: query
        name: CopyTagsToSnapshot
        description: True to copy all tags from the restored DB instance to snapshots
          of the DB instance; otherwise false
        type: string
      - in: query
        name: DBInstanceClass
        description: The compute and memory capacity of the Amazon RDS DB instance
        type: string
      - in: query
        name: DBInstanceIdentifier
        description: Name of the DB instance to create from the DB snapshot
        type: string
      - in: query
        name: DBName
        description: The database name for the restored DB instance
        type: string
      - in: query
        name: DBSnapshotIdentifier
        description: The identifier for the DB snapshot to restore from
        type: string
      - in: query
        name: DBSubnetGroupName
        description: The DB subnet group name to use for the new instance
        type: string
      - in: query
        name: Domain
        description: Specify the Active Directory Domain to restore the instance in
        type: string
      - in: query
        name: DomainIAMRoleName
        description: Specify the name of the IAM role to be used when making API calls
          to the Directory Service
        type: string
      - in: query
        name: Engine
        description: The database engine to use for the new instance
        type: string
      - in: query
        name: Iops
        description: Specifies the amount of provisioned IOPS for the DB instance,
          expressed in I/O operations per second
        type: string
      - in: query
        name: LicenseModel
        description: License model information for the restored DB instance
        type: string
      - in: query
        name: MultiAZ
        description: Specifies if the DB instance is a Multi-AZ deployment
        type: string
      - in: query
        name: OptionGroupName
        description: The name of the option group to be used for the restored DB instance
        type: string
      - in: query
        name: Port
        description: The port number on which the database accepts connections
        type: string
      - in: query
        name: PubliclyAccessible
        description: Specifies the accessibility options for the DB instance
        type: string
      - in: query
        name: StorageType
        description: Specifies the storage type to be associated with the DB instance
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TdeCredentialArn
        description: The ARN from the Key Store with which to associate the instance
          for TDE encryption
        type: string
      - in: query
        name: TdeCredentialPassword
        description: The password for the given ARN from the Key Store in order to
          access the device
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=RestoreDBInstanceToPointInTime:
    get:
      summary: Restore D B Instance To Point In Time
      description: Restores a DB instance to an arbitrary point in time.
      operationId: restoredbinstancetopointintime
      x-api-path-slug: actionrestoredbinstancetopointintime-get
      parameters:
      - in: query
        name: AutoMinorVersionUpgrade
        description: Indicates that minor version upgrades will be applied automatically
          to the DB instance during the maintenance window
        type: string
      - in: query
        name: AvailabilityZone
        description: The EC2 Availability Zone that the database instance will be
          created in
        type: string
      - in: query
        name: CopyTagsToSnapshot
        description: True to copy all tags from the restored DB instance to snapshots
          of the DB instance; otherwise false
        type: string
      - in: query
        name: DBInstanceClass
        description: The compute and memory capacity of the Amazon RDS DB instance
        type: string
      - in: query
        name: DBName
        description: The database name for the restored DB instance
        type: string
      - in: query
        name: DBSubnetGroupName
        description: The DB subnet group name to use for the new instance
        type: string
      - in: query
        name: Domain
        description: Specify the Active Directory Domain to restore the instance in
        type: string
      - in: query
        name: DomainIAMRoleName
        description: Specify the name of the IAM role to be used when making API calls
          to the Directory Service
        type: string
      - in: query
        name: Engine
        description: The database engine to use for the new instance
        type: string
      - in: query
        name: Iops
        description: The amount of Provisioned IOPS (input/output operations per second)
          to be initially allocated for the DB instance
        type: string
      - in: query
        name: LicenseModel
        description: License model information for the restored DB instance
        type: string
      - in: query
        name: MultiAZ
        description: Specifies if the DB instance is a Multi-AZ deployment
        type: string
      - in: query
        name: OptionGroupName
        description: The name of the option group to be used for the restored DB instance
        type: string
      - in: query
        name: Port
        description: The port number on which the database accepts connections
        type: string
      - in: query
        name: PubliclyAccessible
        description: Specifies the accessibility options for the DB instance
        type: string
      - in: query
        name: RestoreTime
        description: The date and time to restore from
        type: string
      - in: query
        name: SourceDBInstanceIdentifier
        description: The identifier of the source DB instance from which to restore
        type: string
      - in: query
        name: StorageType
        description: Specifies the storage type to be associated with the DB instance
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TargetDBInstanceIdentifier
        description: The name of the new database instance to be created
        type: string
      - in: query
        name: TdeCredentialArn
        description: The ARN from the Key Store with which to associate the instance
          for TDE encryption
        type: string
      - in: query
        name: TdeCredentialPassword
        description: The password for the given ARN from the Key Store in order to
          access the device
        type: string
      - in: query
        name: UseLatestRestorableTime
        description: Specifies whether (true) or not (false) the        DB instance
          is restored from the latest backup time
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=RevokeDBSecurityGroupIngress:
    get:
      summary: Revoke D B Security Group Ingress
      description: Revokes ingress from a DBSecurityGroup for previously authorized
        IP ranges or EC2 or VPC Security Groups.
      operationId: revokedbsecuritygroupingress
      x-api-path-slug: actionrevokedbsecuritygroupingress-get
      parameters:
      - in: query
        name: CIDRIP
        description: The IP range to revoke access from
        type: string
      - in: query
        name: DBSecurityGroupName
        description: The name of the DB security group to revoke ingress from
        type: string
      - in: query
        name: EC2SecurityGroupId
        description: The id of the EC2 security group to revoke access from
        type: string
      - in: query
        name: EC2SecurityGroupName
        description: The name of the EC2 security group to revoke access from
        type: string
      - in: query
        name: EC2SecurityGroupOwnerId
        description: The AWS Account Number of the owner of the EC2 security group        specified
          in the EC2SecurityGroupName parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Groups