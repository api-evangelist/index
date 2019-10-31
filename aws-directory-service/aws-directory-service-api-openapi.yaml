swagger: "2.0"
x-collection-name: AWS Directory Service
x-complete: 1
info:
  title: AWS Directory Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddIpRoutes:
    get:
      summary: Add Ip Routes
      description: If the DNS server for your on-premises domain uses a publicly addressable
        IP address, you must add a CIDR address block to correctly route traffic to
        and from your Microsoft AD on Amazon Web Services.
      operationId: addIpRoutes
      x-api-path-slug: actionaddiproutes-get
      parameters:
      - in: query
        name: DirectoryId
        description: Identifier (ID) of the directory to which to add the address
          block
        type: string
      - in: query
        name: IpRoutes
        description: IP address blocks, using CIDR format, of the traffic to route
        type: string
      - in: query
        name: UpdateSecurityGroupForDirectoryControllers
        description: 'If set to true, updates the inbound and outbound rules of the
          security group that has the description: AWS created security group for
          directory ID directory controllers'
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Address Routes
  /?Action=AddTagsToResource:
    get:
      summary: Add Tags To Resource
      description: Adds or overwrites one or more tags for the specified directory.
      operationId: addTagsToResource
      x-api-path-slug: actionaddtagstoresource-get
      parameters:
      - in: query
        name: ResourceId
        description: Identifier (ID) for the directory to which to add the tag
        type: string
      - in: query
        name: Tags
        description: The tags to be assigned to the directory
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
  /?Action=CancelSchemaExtension:
    get:
      summary: Cancel Schema Extension
      description: Cancels an in-progress schema extension to a Microsoft AD directory.
      operationId: cancelSchemaExtension
      x-api-path-slug: actioncancelschemaextension-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory whose schema extension will be
          canceled
        type: string
      - in: query
        name: SchemaExtensionId
        description: The identifier of the schema extension that will be canceled
        type: string
      responses:
        200:
          description: OK
      tags:
      - Schemas
  /?Action=ConnectDirectory:
    get:
      summary: Connect Directory
      description: Creates an AD Connector to connect to an on-premises directory.
      operationId: connectDirectory
      x-api-path-slug: actionconnectdirectory-get
      parameters:
      - in: query
        name: ConnectSettings
        description: A DirectoryConnectSettings object that contains additional information
          for the         operation
        type: string
      - in: query
        name: Description
        description: A textual description for the directory
        type: string
      - in: query
        name: Name
        description: The fully-qualified name of the on-premises directory, such as            corp
        type: string
      - in: query
        name: Password
        description: The password for the on-premises user account
        type: string
      - in: query
        name: ShortName
        description: The NetBIOS name of the on-premises directory, such as CORP
        type: string
      - in: query
        name: Size
        description: The size of the directory
        type: string
      responses:
        200:
          description: OK
      tags:
      - Directories
  /?Action=CreateAlias:
    get:
      summary: Create Alias
      description: Creates an alias for a directory and assigns the alias to the directory.
      operationId: createAlias
      x-api-path-slug: actioncreatealias-get
      parameters:
      - in: query
        name: Alias
        description: The requested alias
        type: string
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which to create the alias
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alias
  /?Action=CreateComputer:
    get:
      summary: Create Computer
      description: Creates a computer account in the specified directory, and joins
        the computer to the directory.
      operationId: createComputer
      x-api-path-slug: actioncreatecomputer-get
      parameters:
      - in: query
        name: ComputerAttributes
        description: An array of Attribute objects that contain any LDAP attributes
          to apply to the            computer account
        type: string
      - in: query
        name: ComputerName
        description: The name of the computer account
        type: string
      - in: query
        name: DirectoryId
        description: The identifier of the directory in which to create the computer
          account
        type: string
      - in: query
        name: OrganizationalUnitDistinguishedName
        description: The fully-qualified distinguished name of the organizational
          unit to place the computer account in
        type: string
      - in: query
        name: Password
        description: A one-time password that is used to join the computer to the
          directory
        type: string
      responses:
        200:
          description: OK
      tags:
      - Computer
  /?Action=CreateConditionalForwarder:
    get:
      summary: Create Conditional Forwarder
      description: Creates a conditional forwarder associated with your AWS directory.
      operationId: createConditionalForwarder
      x-api-path-slug: actioncreateconditionalforwarder-get
      parameters:
      - in: query
        name: DirectoryId
        description: The directory ID of the AWS directory for which you are creating
          the conditional forwarder
        type: string
      - in: query
        name: DnsIpAddrs
        description: The IP addresses of the remote DNS server associated with RemoteDomainName
        type: string
      - in: query
        name: RemoteDomainName
        description: The fully qualified domain name (FQDN) of the remote domain with
          which you will set up a trust relationship
        type: string
      responses:
        200:
          description: OK
      tags:
      - Conditional Forwarder
  /?Action=CreateDirectory:
    get:
      summary: Create Directory
      description: Creates a Simple AD directory.
      operationId: createDirectory
      x-api-path-slug: actioncreatedirectory-get
      parameters:
      - in: query
        name: Description
        description: A textual description for the directory
        type: string
      - in: query
        name: Name
        description: The fully qualified name for the directory, such as corp
        type: string
      - in: query
        name: Password
        description: The password for the directory administrator
        type: string
      - in: query
        name: ShortName
        description: The short name of the directory, such as CORP
        type: string
      - in: query
        name: Size
        description: The size of the directory
        type: string
      - in: query
        name: VpcSettings
        description: A DirectoryVpcSettings object that contains additional information
          for the         operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Directories
  /?Action=CreateMicrosoftAD:
    get:
      summary: Create Microsoft A D
      description: Creates a Microsoft AD in the AWS cloud.
      operationId: createMicrosoftAD
      x-api-path-slug: actioncreatemicrosoftad-get
      parameters:
      - in: query
        name: Description
        description: A textual description for the directory
        type: string
      - in: query
        name: Name
        description: The fully qualified domain name for the directory, such as corp
        type: string
      - in: query
        name: Password
        description: The password for the default administrative user named Admin
        type: string
      - in: query
        name: ShortName
        description: The NetBIOS name for your domain
        type: string
      - in: query
        name: VpcSettings
        description: Contains VPC information for the CreateDirectory or CreateMicrosoftAD
          operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Microsoft AD
  /?Action=CreateSnapshot:
    get:
      summary: Create Snapshot
      description: Creates a snapshot of a Simple AD or Microsoft AD directory in
        the AWS cloud.
      operationId: createSnapshot
      x-api-path-slug: actioncreatesnapshot-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory of which to take a snapshot
        type: string
      - in: query
        name: Name
        description: The descriptive name to apply to the snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshot
  /?Action=CreateTrust:
    get:
      summary: Create Trust
      description: AWS Directory Service for Microsoft Active Directory allows you
        to configure trust relationships.
      operationId: createTrust
      x-api-path-slug: actioncreatetrust-get
      parameters:
      - in: query
        name: ConditionalForwarderIpAddrs
        description: The IP addresses of the remote DNS server associated with RemoteDomainName
        type: string
      - in: query
        name: DirectoryId
        description: The Directory ID of the Microsoft AD in the AWS cloud for which
          to establish the trust relationship
        type: string
      - in: query
        name: RemoteDomainName
        description: The Fully Qualified Domain Name (FQDN) of the external domain
          for which to create the trust relationship
        type: string
      - in: query
        name: TrustDirection
        description: The direction of the trust relationship
        type: string
      - in: query
        name: TrustPassword
        description: The trust password
        type: string
      - in: query
        name: TrustType
        description: The trust relationship type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Trust
  /?Action=DeleteConditionalForwarder:
    get:
      summary: Delete Conditional Forwarder
      description: Deletes a conditional forwarder that has been set up for your AWS
        directory.
      operationId: deleteConditionalForwarder
      x-api-path-slug: actiondeleteconditionalforwarder-get
      parameters:
      - in: query
        name: DirectoryId
        description: The directory ID for which you are deleting the conditional forwarder
        type: string
      - in: query
        name: RemoteDomainName
        description: The fully qualified domain name (FQDN) of the remote domain with
          which you are deleting the conditional forwarder
        type: string
      responses:
        200:
          description: OK
      tags:
      - Conditional Forwarder
  /?Action=DeleteDirectory:
    get:
      summary: Delete Directory
      description: Deletes an AWS Directory Service directory.
      operationId: deleteDirectory
      x-api-path-slug: actiondeletedirectory-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Directories
  /?Action=DeleteSnapshot:
    get:
      summary: Delete Snapshot
      description: Deletes a directory snapshot.
      operationId: deleteSnapshot
      x-api-path-slug: actiondeletesnapshot-get
      parameters:
      - in: query
        name: SnapshotId
        description: The identifier of the directory snapshot to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DeleteTrust:
    get:
      summary: Delete Trust
      description: Deletes an existing trust relationship between your Microsoft AD
        in the AWS cloud and an external domain.
      operationId: deleteTrust
      x-api-path-slug: actiondeletetrust-get
      parameters:
      - in: query
        name: DeleteAssociatedConditionalForwarder
        description: Delete a conditional forwarder as part of a DeleteTrustRequest
        type: string
      - in: query
        name: TrustId
        description: The Trust ID of the trust relationship to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Trust
  /?Action=DeregisterEventTopic:
    get:
      summary: Deregister Event Topic
      description: Removes the specified directory as a publisher to the specified
        SNS topic.
      operationId: deregisterEventTopic
      x-api-path-slug: actionderegistereventtopic-get
      parameters:
      - in: query
        name: DirectoryId
        description: The Directory ID to remove as a publisher
        type: string
      - in: query
        name: TopicName
        description: The name of the SNS topic from which to remove the directory
          as a publisher
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Topics
  /?Action=DescribeConditionalForwarders:
    get:
      summary: Describe Conditional Forwarders
      description: Obtains information about the conditional forwarders for this account.
      operationId: describeConditionalForwarders
      x-api-path-slug: actiondescribeconditionalforwarders-get
      parameters:
      - in: query
        name: DirectoryId
        description: The directory ID for which to get the list of associated conditional
          forwarders
        type: string
      - in: query
        name: RemoteDomainNames
        description: The fully qualified domain names (FQDN) of the remote domains
          for which to get the list of associated conditional forwarders
        type: string
      responses:
        200:
          description: OK
      tags:
      - Conditional Forwarder
  /?Action=DescribeDirectories:
    get:
      summary: Describe Directories
      description: Obtains information about the directories that belong to this account.
      operationId: describeDirectories
      x-api-path-slug: actiondescribedirectories-get
      parameters:
      - in: query
        name: DirectoryIds
        description: A list of identifiers of the directories for which to obtain
          the information
        type: string
      - in: query
        name: Limit
        description: The maximum number of items to return
        type: string
      - in: query
        name: NextToken
        description: The DescribeDirectoriesResult
        type: string
      responses:
        200:
          description: OK
      tags:
      - Directories
  /?Action=DescribeEventTopics:
    get:
      summary: Describe Event Topics
      description: Obtains information about which SNS topics receive status messages
        from the specified directory.
      operationId: describeEventTopics
      x-api-path-slug: actiondescribeeventtopics-get
      parameters:
      - in: query
        name: DirectoryId
        description: The Directory ID for which to get the list of associated SNS
          topics
        type: string
      - in: query
        name: TopicNames
        description: A list of SNS topic names for which to obtain the information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Topics
  /?Action=DescribeSnapshots:
    get:
      summary: Describe Snapshots
      description: Obtains information about the directory snapshots that belong to
        this account.
      operationId: describeSnapshots
      x-api-path-slug: actiondescribesnapshots-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which to retrieve snapshot
          information
        type: string
      - in: query
        name: Limit
        description: The maximum number of objects to return
        type: string
      - in: query
        name: NextToken
        description: The DescribeSnapshotsResult
        type: string
      - in: query
        name: SnapshotIds
        description: A list of identifiers of the snapshots to obtain the information
          for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DescribeTrusts:
    get:
      summary: Describe Trusts
      description: Obtains information about the trust relationships for this account.
      operationId: describeTrusts
      x-api-path-slug: actiondescribetrusts-get
      parameters:
      - in: query
        name: DirectoryId
        description: The Directory ID of the AWS directory that is a part of the requested
          trust relationship
        type: string
      - in: query
        name: Limit
        description: The maximum number of objects to return
        type: string
      - in: query
        name: NextToken
        description: The DescribeTrustsResult
        type: string
      - in: query
        name: TrustIds
        description: A list of identifiers of the trust relationships for which to
          obtain the information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Trust
  /?Action=DisableRadius:
    get:
      summary: Disable Radius
      description: Disables multi-factor authentication (MFA) with the Remote Authentication
        Dial In User Service (RADIUS) server for an AD Connector directory.
      operationId: disableRadius
      x-api-path-slug: actiondisableradius-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which to disable MFA
        type: string
      responses:
        200:
          description: OK
      tags:
      - Radius
  /?Action=DisableSso:
    get:
      summary: Disable Sso
      description: Disables single-sign on for a directory.
      operationId: disableSso
      x-api-path-slug: actiondisablesso-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which to disable single-sign
          on
        type: string
      - in: query
        name: Password
        description: The password of an alternate account to use to disable single-sign
          on
        type: string
      - in: query
        name: UserName
        description: The username of an alternate account to use to disable single-sign
          on
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSO
  /?Action=EnableRadius:
    get:
      summary: Enable Radius
      description: Enables multi-factor authentication (MFA) with the Remote Authentication
        Dial In User Service (RADIUS) server for an AD Connector directory.
      operationId: enableRadius
      x-api-path-slug: actionenableradius-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which to enable MFA
        type: string
      - in: query
        name: RadiusSettings
        description: A RadiusSettings object that contains information about the RADIUS
          server
        type: string
      responses:
        200:
          description: OK
      tags:
      - Radius
  /?Action=EnableSso:
    get:
      summary: Enable Sso
      description: Enables single sign-on for a directory.
      operationId: enableSso
      x-api-path-slug: actionenablesso-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which to enable single-sign
          on
        type: string
      - in: query
        name: Password
        description: The password of an alternate account to use to enable single-sign
          on
        type: string
      - in: query
        name: UserName
        description: The username of an alternate account to use to enable single-sign
          on
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSO
  /?Action=GetDirectoryLimits:
    get:
      summary: Get Directory Limits
      description: Obtains directory limit information for the current region.
      operationId: getDirectoryLimits
      x-api-path-slug: actiongetdirectorylimits-get
      parameters:
      - in: query
        name: DirectoryLimits
        description: A DirectoryLimits object that contains the directory limits for
          the current         region
        type: string
      responses:
        200:
          description: OK
      tags:
      - Directories
  /?Action=GetSnapshotLimits:
    get:
      summary: Get Snapshot Limits
      description: Obtains the manual snapshot limits for a directory.
      operationId: getSnapshotLimits
      x-api-path-slug: actiongetsnapshotlimits-get
      parameters:
      - in: query
        name: DirectoryId
        description: Contains the identifier of the directory to obtain the limits
          for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=ListIpRoutes:
    get:
      summary: List Ip Routes
      description: Lists the address blocks that you have added to a directory.
      operationId: listIpRoutes
      x-api-path-slug: actionlistiproutes-get
      parameters:
      - in: query
        name: DirectoryId
        description: Identifier (ID) of the directory for which you want to retrieve
          the IP addresses
        type: string
      - in: query
        name: Limit
        description: Maximum number of items to return
        type: string
      - in: query
        name: NextToken
        description: The ListIpRoutes
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Address Routes
  /?Action=ListSchemaExtensions:
    get:
      summary: List Schema Extensions
      description: Lists all schema extensions applied to a Microsoft AD Directory.
      operationId: listSchemaExtensions
      x-api-path-slug: actionlistschemaextensions-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory from which to retrieve the schema
          extension information
        type: string
      - in: query
        name: Limit
        description: The maximum number of items to return
        type: string
      - in: query
        name: NextToken
        description: The ListSchemaExtensions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Schema Extension
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: Lists all tags on a directory.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: Limit
        description: Reserved for future use
        type: string
      - in: query
        name: NextToken
        description: Reserved for future use
        type: string
      - in: query
        name: ResourceId
        description: Identifier (ID) of the directory for which you want to retrieve
          tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Tags
  /?Action=RegisterEventTopic:
    get:
      summary: Register Event Topic
      description: Associates a directory with an SNS topic.
      operationId: registerEventTopic
      x-api-path-slug: actionregistereventtopic-get
      parameters:
      - in: query
        name: DirectoryId
        description: The Directory ID that will publish status messages to the SNS
          topic
        type: string
      - in: query
        name: TopicName
        description: The SNS topic name to which the directory will publish status
          messages
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Topics
  /?Action=RemoveIpRoutes:
    get:
      summary: Remove Ip Routes
      description: Removes IP address blocks from a directory.
      operationId: removeIpRoutes
      x-api-path-slug: actionremoveiproutes-get
      parameters:
      - in: query
        name: CidrIps
        description: IP address blocks that you want to remove
        type: string
      - in: query
        name: DirectoryId
        description: Identifier (ID) of the directory from which you want to remove
          the IP addresses
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Address Routes
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes tags from a directory.
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceId
        description: Identifier (ID) of the directory from which to remove the tag
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
  /?Action=RestoreFromSnapshot:
    get:
      summary: Restore From Snapshot
      description: Restores a directory using an existing directory snapshot.
      operationId: restoreFromSnapshot
      x-api-path-slug: actionrestorefromsnapshot-get
      parameters:
      - in: query
        name: SnapshotId
        description: The identifier of the snapshot to restore from
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=StartSchemaExtension:
    get:
      summary: Start Schema Extension
      description: Applies a schema extension to a Microsoft AD directory.
      operationId: startSchemaExtension
      x-api-path-slug: actionstartschemaextension-get
      parameters:
      - in: query
        name: CreateSnapshotBeforeSchemaExtension
        description: If true, creates a snapshot of the directory before applying
          the schema extension
        type: string
      - in: query
        name: Description
        description: A description of the schema extension
        type: string
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which the schema extension
          will be applied to
        type: string
      - in: query
        name: LdifContent
        description: The LDIF file represented as a string
        type: string
      responses:
        200:
          description: OK
      tags:
      - Schema Extension
  /?Action=UpdateConditionalForwarder:
    get:
      summary: Update Conditional Forwarder
      description: Updates a conditional forwarder that has been set up for your AWS
        directory.
      operationId: updateConditionalForwarder
      x-api-path-slug: actionupdateconditionalforwarder-get
      parameters:
      - in: query
        name: DirectoryId
        description: The directory ID of the AWS directory for which to update the
          conditional forwarder
        type: string
      - in: query
        name: DnsIpAddrs
        description: The updated IP addresses of the remote DNS server associated
          with the conditional forwarder
        type: string
      - in: query
        name: RemoteDomainName
        description: The fully qualified domain name (FQDN) of the remote domain with
          which you will set up a trust relationship
        type: string
      responses:
        200:
          description: OK
      tags:
      - Conditional Forwarder
  /?Action=UpdateRadius:
    get:
      summary: Update Radius
      description: Updates the Remote Authentication Dial In User Service (RADIUS)
        server information for an AD Connector directory.
      operationId: updateRadius
      x-api-path-slug: actionupdateradius-get
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which to update the RADIUS
          server information
        type: string
      - in: query
        name: RadiusSettings
        description: A RadiusSettings object that contains information about the RADIUS
          server
        type: string
      responses:
        200:
          description: OK
      tags:
      - Radius
  /?Action=VerifyTrust:
    get:
      summary: Verify Trust
      description: AWS Directory Service for Microsoft Active Directory allows you
        to configure and verify trust relationships.
      operationId: verifyTrust
      x-api-path-slug: actionverifytrust-get
      parameters:
      - in: query
        name: TrustId
        description: The unique Trust ID of the trust relationship to verify
        type: string
      responses:
        200:
          description: OK
      tags:
      - Trust