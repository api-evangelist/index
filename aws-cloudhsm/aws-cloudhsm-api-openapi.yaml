swagger: "2.0"
x-collection-name: AWS CloudHSM
x-complete: 1
info:
  title: AWS CloudHSM API
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
      description: Adds or overwrites one or more tags for the specified AWS CloudHSM
        resource.
      operationId: addTagsToResource
      x-api-path-slug: actionaddtagstoresource-get
      parameters:
      - in: query
        name: ResourceArn
        description: The Amazon Resource Name (ARN) of the AWS CloudHSM resource to
          tag
        type: string
      - in: query
        name: TagList
        description: One or more tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=CreateHapg:
    get:
      summary: Create Hapg
      description: Creates a high-availability partition group.
      operationId: createHapg
      x-api-path-slug: actioncreatehapg-get
      parameters:
      - in: query
        name: Label
        description: The label of the new high-availability partition group
        type: string
      responses:
        200:
          description: OK
      tags:
      - High-Availability Partition Group
  /?Action=CreateHsm:
    get:
      summary: Create HSM
      description: Creates an uninitialized HSM instance.
      operationId: createHsm
      x-api-path-slug: actioncreatehsm-get
      parameters:
      - in: query
        name: ClientToken
        description: A user-defined token to ensure idempotence
        type: string
      - in: query
        name: EniIp
        description: The IP address to assign to the HSMs ENI
        type: string
      - in: query
        name: ExternalId
        description: The external ID from IamRoleArn, if present
        type: string
      - in: query
        name: IamRoleArn
        description: The ARN of an IAM role to enable the AWS CloudHSM service to
          allocate an ENI on your      behalf
        type: string
      - in: query
        name: SshKey
        description: The SSH public key to install on the HSM
        type: string
      - in: query
        name: SubnetId
        description: The identifier of the subnet in your VPC in which to place the
          HSM
        type: string
      - in: query
        name: SubscriptionType
        description: Specifies the type of subscription for the HSM
        type: string
      - in: query
        name: SyslogIp
        description: The IP address for the syslog monitoring server
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Instances
  /?Action=CreateLunaClient:
    get:
      summary: Create Luna Client
      description: Creates an HSM client.
      operationId: createLunaClient
      x-api-path-slug: actioncreatelunaclient-get
      parameters:
      - in: query
        name: Certificate
        description: The contents of a Base64-Encoded X
        type: string
      - in: query
        name: Label
        description: The label for the client
        type: string
      responses:
        200:
          description: OK
      tags:
      - Luna Clients
  /?Action=DeleteHapg:
    get:
      summary: Delete HAPG
      description: Deletes a high-availability partition group.
      operationId: deleteHapg
      x-api-path-slug: actiondeletehapg-get
      parameters:
      - in: query
        name: HapgArn
        description: The ARN of the high-availability partition group to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - High-Availability Partition Group
  /?Action=DeleteHsm:
    get:
      summary: Delete HSM
      description: Deletes an HSM.
      operationId: deleteHsm
      x-api-path-slug: actiondeletehsm-get
      parameters:
      - in: query
        name: HsmArn
        description: The ARN of the HSM to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Instances
  /?Action=DeleteLunaClient:
    get:
      summary: Delete Luna Client
      description: Deletes a client.
      operationId: deleteLunaClient
      x-api-path-slug: actiondeletelunaclient-get
      parameters:
      - in: query
        name: ClientArn
        description: The ARN of the client to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Luna Clients
  /?Action=DescribeHapg:
    get:
      summary: Describe HAPG
      description: Retrieves information about a high-availability partition group.
      operationId: describeHapg
      x-api-path-slug: actiondescribehapg-get
      parameters:
      - in: query
        name: HapgArn
        description: The ARN of the high-availability partition group to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - High-Availability Partition Group
  /?Action=DescribeHsm:
    get:
      summary: Describe HSM
      description: Retrieves information about an HSM.
      operationId: describeHsm
      x-api-path-slug: actiondescribehsm-get
      parameters:
      - in: query
        name: HsmArn
        description: The ARN of the HSM
        type: string
      - in: query
        name: HsmSerialNumber
        description: The serial number of the HSM
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Instances
  /?Action=DescribeLunaClient:
    get:
      summary: Describe Luna Client
      description: Retrieves information about an HSM client.
      operationId: describeLunaClient
      x-api-path-slug: actiondescribelunaclient-get
      parameters:
      - in: query
        name: CertificateFingerprint
        description: The certificate fingerprint
        type: string
      - in: query
        name: ClientArn
        description: The ARN of the client
        type: string
      responses:
        200:
          description: OK
      tags:
      - Luna Clients
  /?Action=GetConfig:
    get:
      summary: Get Config
      description: |-
        Gets the configuration files necessary to connect to all high availability partition
              groups the client is associated with.
      operationId: getConfig
      x-api-path-slug: actiongetconfig-get
      parameters:
      - in: query
        name: ClientArn
        description: The ARN of the client
        type: string
      - in: query
        name: ClientVersion
        description: The client version
        type: string
      - in: query
        name: HapgList
        description: A list of ARNs that identify the high-availability partition
          groups that are associated      with the client
        type: string
      responses:
        200:
          description: OK
      tags:
      - Config
  /?Action=ListAvailableZones:
    get:
      summary: List Available Zones
      description: Lists the Availability Zones that have available AWS CloudHSM capacity.
      operationId: listAvailableZones
      x-api-path-slug: actionlistavailablezones-get
      parameters:
      - in: query
        name: AZList
        description: The list of Availability Zones that have available AWS CloudHSM
          capacity
        type: string
      responses:
        200:
          description: OK
      tags:
      - Zones
  /?Action=ListHapgs:
    get:
      summary: List HAPG
      description: Lists the high-availability partition groups for the account.
      operationId: listHapgs
      x-api-path-slug: actionlisthapgs-get
      parameters:
      - in: query
        name: NextToken
        description: The NextToken value from a previous call to ListHapgs
        type: string
      responses:
        200:
          description: OK
      tags:
      - High-Availability Partition Group
  /?Action=ListHsms:
    get:
      summary: List HSM
      description: |-
        Retrieves the identifiers of all of the HSMs provisioned for the current
              customer.
      operationId: listHsms
      x-api-path-slug: actionlisthsms-get
      parameters:
      - in: query
        name: NextToken
        description: The NextToken value from a previous call to ListHsms
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Instances
  /?Action=ListLunaClients:
    get:
      summary: List Luna Clients
      description: Lists all of the clients.
      operationId: listLunaClients
      x-api-path-slug: actionlistlunaclients-get
      parameters:
      - in: query
        name: NextToken
        description: The NextToken value from a previous call to ListLunaClients
        type: string
      responses:
        200:
          description: OK
      tags:
      - Luna Clients
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: Returns a list of all tags for the specified AWS CloudHSM resource.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: ResourceArn
        description: The Amazon Resource Name (ARN) of the AWS CloudHSM resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=ModifyHapg:
    get:
      summary: Modify HAPG
      description: Modifies an existing high-availability partition group.
      operationId: modifyHapg
      x-api-path-slug: actionmodifyhapg-get
      parameters:
      - in: query
        name: HapgArn
        description: The ARN of the high-availability partition group to modify
        type: string
      - in: query
        name: Label
        description: The new label for the high-availability partition group
        type: string
      - in: query
        name: PartitionSerialList
        description: The list of partition serial numbers to make members of the high-availability
          partition      group
        type: string
      responses:
        200:
          description: OK
      tags:
      - High-Availability Partition Group
  /?Action=ModifyHsm:
    get:
      summary: Modify HSM
      description: Modifies an HSM.
      operationId: modifyHsm
      x-api-path-slug: actionmodifyhsm-get
      parameters:
      - in: query
        name: EniIp
        description: The new IP address for the elastic network interface (ENI) attached
          to the      HSM
        type: string
      - in: query
        name: ExternalId
        description: The new external ID
        type: string
      - in: query
        name: HsmArn
        description: The ARN of the HSM to modify
        type: string
      - in: query
        name: IamRoleArn
        description: The new IAM role ARN
        type: string
      - in: query
        name: SubnetId
        description: The new identifier of the subnet that the HSM is in
        type: string
      - in: query
        name: SyslogIp
        description: The new IP address for the syslog monitoring server
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Instances
  /?Action=ModifyLunaClient:
    get:
      summary: Modify Luna Client
      description: Modifies the certificate used by the client.
      operationId: modifyLunaClient
      x-api-path-slug: actionmodifylunaclient-get
      parameters:
      - in: query
        name: Certificate
        description: The new certificate for the client
        type: string
      - in: query
        name: ClientArn
        description: The ARN of the client
        type: string
      responses:
        200:
          description: OK
      tags:
      - Luna Clients
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes one or more tags from the specified AWS CloudHSM resource.
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceArn
        description: The Amazon Resource Name (ARN) of the AWS CloudHSM resource
        type: string
      - in: query
        name: TagKeyList
        description: The tag key or keys to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags