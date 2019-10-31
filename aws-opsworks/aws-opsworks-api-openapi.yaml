swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 1
info:
  title: AWS OpsWorks API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AssignInstance:
    get:
      summary: Assign Instance
      description: Assign a registered instance to a layer.
      operationId: assignInstance
      x-api-path-slug: actionassigninstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      - in: query
        name: LayerIds
        description: The layer ID, which must correspond to a custom layer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Assign
      - Instance
  /?Action=AssignVolume:
    get:
      summary: Assign Volume
      description: Assigns one of the stack's registered Amazon EBS volumes to a specified
        instance.
      operationId: assignVolume
      x-api-path-slug: actionassignvolume-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      - in: query
        name: VolumeId
        description: The volume ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Assign
      - Volume
  /?Action=AssociateElasticIp:
    get:
      summary: Associate Elastic IP
      description: Associates one of the stack's registered Elastic IP addresses with
        a specified instance.
      operationId: associateElasticIp
      x-api-path-slug: actionassociateelasticip-get
      parameters:
      - in: query
        name: ElasticIp
        description: The Elastic IP address
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Associate
      - Elastic
      - IP Addresses
  /?Action=AttachElasticLoadBalancer:
    get:
      summary: Attach Elastic Load Balancer
      description: Attaches an Elastic Load Balancing load balancer to a specified
        layer.
      operationId: attachElasticLoadBalancer
      x-api-path-slug: actionattachelasticloadbalancer-get
      parameters:
      - in: query
        name: ElasticLoadBalancerName
        description: The Elastic Load Balancing instances name
        type: string
      - in: query
        name: LayerId
        description: The ID of the layer that the Elastic Load Balancing instance
          is to be attached to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attach
      - Elastic
      - Load
      - Balancer
  /?Action=CloneStack:
    get:
      summary: Clone Stack
      description: Creates a clone of a specified stack.
      operationId: cloneStack
      x-api-path-slug: actionclonestack-get
      parameters:
      - in: query
        name: AgentVersion
        description: The default AWS OpsWorks Stacks agent version
        type: string
      - in: query
        name: Attributes
        description: A list of stack attributes and values as key/value pairs to be
          added to the cloned stack
        type: string
      - in: query
        name: ChefConfiguration
        description: A ChefConfiguration object that specifies whether to enable Berkshelf
          and the      Berkshelf version on Chef 11
        type: string
      - in: query
        name: CloneAppIds
        description: A list of source stack app IDs to be included in the cloned stack
        type: string
      - in: query
        name: ClonePermissions
        description: Whether to clone the source stacks permissions
        type: string
      - in: query
        name: ConfigurationManager
        description: The configuration manager
        type: string
      - in: query
        name: CustomCookbooksSource
        description: Contains the information required to retrieve an app or cookbook
          from a repository
        type: string
      - in: query
        name: CustomJson
        description: A string that contains user-defined, custom JSON
        type: string
      - in: query
        name: DefaultAvailabilityZone
        description: The cloned stacks default Availability Zone, which must be in
          the specified region
        type: string
      - in: query
        name: DefaultInstanceProfileArn
        description: The Amazon Resource Name (ARN) of an IAM profile that is the
          default profile for all of the stacks EC2 instances
        type: string
      - in: query
        name: DefaultOs
        description: The stacks operating system, which must be set to one of the
          following
        type: string
      - in: query
        name: DefaultRootDeviceType
        description: The default root device type
        type: string
      - in: query
        name: DefaultSshKeyName
        description: A default Amazon EC2 key pair name
        type: string
      - in: query
        name: DefaultSubnetId
        description: The stacks default VPC subnet ID
        type: string
      - in: query
        name: HostnameTheme
        description: The stacks host name theme, with spaces are replaced by underscores
        type: string
      - in: query
        name: Name
        description: The cloned stack name
        type: string
      - in: query
        name: Region
        description: The cloned stack AWS region, such as ap-northeast-2
        type: string
      - in: query
        name: ServiceRoleArn
        description: The stack AWS Identity and Access Management (IAM) role, which
          allows AWS OpsWorks Stacks to work with AWS      resources on your behalf
        type: string
      - in: query
        name: SourceStackId
        description: The source stack ID
        type: string
      - in: query
        name: UseCustomCookbooks
        description: Whether to use custom cookbooks
        type: string
      - in: query
        name: UseOpsworksSecurityGroups
        description: Whether to associate the AWS OpsWorks Stacks built-in security
          groups with the stacks layers
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC that the cloned stack is to be launched into
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clone
      - Stack
  /?Action=CreateApp:
    get:
      summary: Create App
      description: Creates an app for a specified stack.
      operationId: createApp
      x-api-path-slug: actioncreateapp-get
      parameters:
      - in: query
        name: AppSource
        description: A Source object that specifies the app repository
        type: string
      - in: query
        name: Attributes
        description: One or more user-defined key/value pairs to be added to the stack
          attributes
        type: string
      - in: query
        name: DataSources
        description: The apps data source
        type: string
      - in: query
        name: Description
        description: A description of the app
        type: string
      - in: query
        name: Domains
        description: The app virtual host settings, with multiple domains separated
          by commas
        type: string
      - in: query
        name: EnableSsl
        description: Whether to enable SSL for the app
        type: string
      - in: query
        name: Environment
        description: An array of EnvironmentVariable objects that specify environment
          variables to be      associated with the app
        type: string
      - in: query
        name: Name
        description: The app name
        type: string
      - in: query
        name: Shortname
        description: The apps short name
        type: string
      - in: query
        name: SslConfiguration
        description: An SslConfiguration object with the SSL configuration
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      - in: query
        name: Type
        description: The app type
        type: string
      responses:
        200:
          description: OK
      tags:
      - App
  /?Action=CreateDeployment:
    get:
      summary: Create Deployment
      description: Runs deployment or stack commands.
      operationId: createDeployment
      x-api-path-slug: actioncreatedeployment-get
      parameters:
      - in: query
        name: AppId
        description: The app ID
        type: string
      - in: query
        name: Command
        description: A DeploymentCommand object that specifies the deployment command
          and any      associated arguments
        type: string
      - in: query
        name: Comment
        description: A user-defined comment
        type: string
      - in: query
        name: CustomJson
        description: A string that contains user-defined, custom JSON
        type: string
      - in: query
        name: InstanceIds
        description: The instance IDs for the deployment targets
        type: string
      - in: query
        name: LayerIds
        description: The layer IDs for the deployment targets
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment
  /?Action=CreateInstance:
    get:
      summary: Create Instance
      description: Creates an instance in a specified stack.
      operationId: createInstance
      x-api-path-slug: actioncreateinstance-get
      parameters:
      - in: query
        name: AgentVersion
        description: The default AWS OpsWorks Stacks agent version
        type: string
      - in: query
        name: AmiId
        description: A custom AMI ID to be used to create the instance
        type: string
      - in: query
        name: Architecture
        description: The instance architecture
        type: string
      - in: query
        name: AutoScalingType
        description: For load-based or time-based instances, the type
        type: string
      - in: query
        name: AvailabilityZone
        description: The instance Availability Zone
        type: string
      - in: query
        name: BlockDeviceMappings
        description: An array of BlockDeviceMapping objects that specify the instances
          block      devices
        type: string
      - in: query
        name: EbsOptimized
        description: Whether to create an Amazon EBS-optimized instance
        type: string
      - in: query
        name: Hostname
        description: The instance host name
        type: string
      - in: query
        name: InstallUpdatesOnBoot
        description: Whether to install operating system and package updates when
          the instance boots
        type: string
      - in: query
        name: InstanceType
        description: The instance type, such as t2
        type: string
      - in: query
        name: LayerIds
        description: An array that contains the instances layer IDs
        type: string
      - in: query
        name: Os
        description: The instances operating system, which must be set to one of the
          following
        type: string
      - in: query
        name: RootDeviceType
        description: The instance root device type
        type: string
      - in: query
        name: SshKeyName
        description: The instances Amazon EC2 key-pair name
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      - in: query
        name: SubnetId
        description: The ID of the instances subnet
        type: string
      - in: query
        name: Tenancy
        description: The instances tenancy option
        type: string
      - in: query
        name: VirtualizationType
        description: The instances virtualization type, paravirtual or hvm
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
  /?Action=CreateLayer:
    get:
      summary: Create Layer
      description: Creates a layer.
      operationId: createLayer
      x-api-path-slug: actioncreatelayer-get
      parameters:
      - in: query
        name: Attributes
        description: One or more user-defined key-value pairs to be added to the stack
          attributes
        type: string
      - in: query
        name: AutoAssignElasticIps
        description: Whether to automatically assign an Elastic IP        address
          to the layers instances
        type: string
      - in: query
        name: AutoAssignPublicIps
        description: For stacks that are running in a VPC, whether to automatically
          assign a public IP address to      the layers instances
        type: string
      - in: query
        name: CustomInstanceProfileArn
        description: The ARN of an IAM profile to be used for the layers EC2 instances
        type: string
      - in: query
        name: CustomJson
        description: A JSON-formatted string containing custom stack configuration
          and deployment attributes     to be installed on the layers instances
        type: string
      - in: query
        name: CustomRecipes
        description: A LayerCustomRecipes object that specifies the layer custom recipes
        type: string
      - in: query
        name: CustomSecurityGroupIds
        description: An array containing the layer custom security group IDs
        type: string
      - in: query
        name: EnableAutoHealing
        description: Whether to disable auto healing for the layer
        type: string
      - in: query
        name: InstallUpdatesOnBoot
        description: Whether to install operating system and package updates when
          the instance boots
        type: string
      - in: query
        name: LifecycleEventConfiguration
        description: A LifeCycleEventConfiguration object that you can use to configure
          the Shutdown event to      specify an execution timeout and enable or disable
          Elastic Load Balancer connection      draining
        type: string
      - in: query
        name: Name
        description: The layer name, which is used by the console
        type: string
      - in: query
        name: Packages
        description: An array of Package objects that describes the layer packages
        type: string
      - in: query
        name: Shortname
        description: For custom layers only, use this parameter to specify the layers
          short name, which is used internally by AWS OpsWorks Stacks and by Chef
          recipes
        type: string
      - in: query
        name: StackId
        description: The layer stack ID
        type: string
      - in: query
        name: Type
        description: The layer type
        type: string
      - in: query
        name: UseEbsOptimizedInstances
        description: Whether to use Amazon EBS-optimized instances
        type: string
      - in: query
        name: VolumeConfigurations
        description: A VolumeConfigurations object that describes the layers Amazon
          EBS volumes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Layer
  /?Action=CreateStack:
    get:
      summary: Create Stack
      description: Creates a new stack.
      operationId: createStack
      x-api-path-slug: actioncreatestack-get
      parameters:
      - in: query
        name: AgentVersion
        description: The default AWS OpsWorks Stacks agent version
        type: string
      - in: query
        name: Attributes
        description: One or more user-defined key-value pairs to be added to the stack
          attributes
        type: string
      - in: query
        name: ChefConfiguration
        description: A ChefConfiguration object that specifies whether to enable Berkshelf
          and the      Berkshelf version on Chef 11
        type: string
      - in: query
        name: ConfigurationManager
        description: The configuration manager
        type: string
      - in: query
        name: CustomCookbooksSource
        description: Contains the information required to retrieve an app or cookbook
          from a repository
        type: string
      - in: query
        name: CustomJson
        description: A string that contains user-defined, custom JSON
        type: string
      - in: query
        name: DefaultAvailabilityZone
        description: The stacks default Availability Zone, which must be in the specified
          region
        type: string
      - in: query
        name: DefaultInstanceProfileArn
        description: The Amazon Resource Name (ARN) of an IAM profile that is the
          default profile for all of the stacks EC2 instances
        type: string
      - in: query
        name: DefaultOs
        description: The stacks default operating system, which is installed on every
          instance unless you specify a different operating system when you create
          the instance
        type: string
      - in: query
        name: DefaultRootDeviceType
        description: The default root device type
        type: string
      - in: query
        name: DefaultSshKeyName
        description: A default Amazon EC2 key pair name
        type: string
      - in: query
        name: DefaultSubnetId
        description: The stacks default VPC subnet ID
        type: string
      - in: query
        name: HostnameTheme
        description: The stacks host name theme, with spaces replaced by underscores
        type: string
      - in: query
        name: Name
        description: The stack name
        type: string
      - in: query
        name: Region
        description: The stacks AWS region, such as ap-south-1
        type: string
      - in: query
        name: ServiceRoleArn
        description: The stacks AWS Identity and Access Management (IAM) role, which
          allows AWS OpsWorks Stacks to work with AWS      resources on your behalf
        type: string
      - in: query
        name: UseCustomCookbooks
        description: Whether the stack uses custom cookbooks
        type: string
      - in: query
        name: UseOpsworksSecurityGroups
        description: Whether to associate the AWS OpsWorks Stacks built-in security
          groups with the stacks layers
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC that the stack is to be launched into
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack
  /?Action=CreateUserProfile:
    get:
      summary: Create User Profile
      description: Creates a new user profile.
      operationId: createUserProfile
      x-api-path-slug: actioncreateuserprofile-get
      parameters:
      - in: query
        name: AllowSelfManagement
        description: Whether users can specify their own SSH public key through the
          My Settings page
        type: string
      - in: query
        name: IamUserArn
        description: The users IAM ARN; this can also be a federated users ARN
        type: string
      - in: query
        name: SshPublicKey
        description: The users public SSH key
        type: string
      - in: query
        name: SshUsername
        description: The users SSH user name
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Profile
  /?Action=DeleteApp:
    get:
      summary: Delete App
      description: Deletes a specified app.
      operationId: deleteApp
      x-api-path-slug: actiondeleteapp-get
      parameters:
      - in: query
        name: AppId
        description: The app ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - App
  /?Action=DeleteInstance:
    get:
      summary: Delete Instance
      description: Deletes a specified instance, which terminates the associated Amazon
        EC2 instance.
      operationId: deleteInstance
      x-api-path-slug: actiondeleteinstance-get
      parameters:
      - in: query
        name: DeleteElasticIp
        description: Whether to delete the instance Elastic IP address
        type: string
      - in: query
        name: DeleteVolumes
        description: Whether to delete the instances Amazon EBS volumes
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
  /?Action=DeleteLayer:
    get:
      summary: Delete Layer
      description: Deletes a specified layer.
      operationId: deleteLayer
      x-api-path-slug: actiondeletelayer-get
      parameters:
      - in: query
        name: LayerId
        description: The layer ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Layer
  /?Action=DeleteStack:
    get:
      summary: Delete Stack
      description: Deletes a specified stack.
      operationId: deleteStack
      x-api-path-slug: actiondeletestack-get
      parameters:
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack
  /?Action=DeleteUserProfile:
    get:
      summary: Delete User Profile
      description: Deletes a user profile.
      operationId: deleteUserProfile
      x-api-path-slug: actiondeleteuserprofile-get
      parameters:
      - in: query
        name: IamUserArn
        description: The users IAM ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Profile
  /?Action=DeregisterEcsCluster:
    get:
      summary: Deregister Ecs Cluster
      description: Deregisters a specified Amazon ECS cluster from a stack.
      operationId: deregisterEcsCluster
      x-api-path-slug: actionderegisterecscluster-get
      parameters:
      - in: query
        name: EcsClusterArn
        description: The clusters ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Ecs
      - Cluster
  /?Action=DeregisterElasticIp:
    get:
      summary: Deregister Elastic IP
      description: Deregisters a specified Elastic IP address.
      operationId: deregisterElasticIp
      x-api-path-slug: actionderegisterelasticip-get
      parameters:
      - in: query
        name: ElasticIp
        description: The Elastic IP address
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Elastic
      - IP Addresses
  /?Action=DeregisterInstance:
    get:
      summary: Deregister Instance
      description: Deregister a registered Amazon EC2 or on-premises instance.
      operationId: deregisterInstance
      x-api-path-slug: actionderegisterinstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Instance
  /?Action=DeregisterRdsDbInstance:
    get:
      summary: Deregister Rds Db Instance
      description: Deregisters an Amazon RDS instance.
      operationId: deregisterRdsDbInstance
      x-api-path-slug: actionderegisterrdsdbinstance-get
      parameters:
      - in: query
        name: RdsDbInstanceArn
        description: The Amazon RDS instances ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Rds
      - Db
      - Instance
  /?Action=DeregisterVolume:
    get:
      summary: Deregister Volume
      description: Deregisters an Amazon EBS volume.
      operationId: deregisterVolume
      x-api-path-slug: actionderegistervolume-get
      parameters:
      - in: query
        name: VolumeId
        description: The AWS OpsWorks Stacks volume ID, which is the GUID that AWS
          OpsWorks Stacks assigned to the instance when you registered the volume
          with the stack, not the Amazon EC2 volume ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Volume
  /?Action=DescribeAgentVersions:
    get:
      summary: Describe Agent Versions
      description: Describes the available AWS OpsWorks Stacks agent versions.
      operationId: describeAgentVersions
      x-api-path-slug: actiondescribeagentversions-get
      parameters:
      - in: query
        name: ConfigurationManager
        description: The configuration manager
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Agent
      - Versions
  /?Action=DescribeApps:
    get:
      summary: Describe Apps
      description: Requests a description of a specified set of apps.
      operationId: describeApps
      x-api-path-slug: actiondescribeapps-get
      parameters:
      - in: query
        name: AppIds
        description: An array of app IDs for the apps to be described
        type: string
      - in: query
        name: StackId
        description: The app stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Apps
  /?Action=DescribeCommands:
    get:
      summary: Describe Commands
      description: Describes the results of specified commands.
      operationId: describeCommands
      x-api-path-slug: actiondescribecommands-get
      parameters:
      - in: query
        name: CommandIds
        description: An array of command IDs
        type: string
      - in: query
        name: DeploymentId
        description: The deployment ID
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Commands
  /?Action=DescribeDeployments:
    get:
      summary: Describe Deployments
      description: Requests a description of a specified set of deployments.
      operationId: describeDeployments
      x-api-path-slug: actiondescribedeployments-get
      parameters:
      - in: query
        name: AppId
        description: The app ID
        type: string
      - in: query
        name: DeploymentIds
        description: An array of deployment IDs to be described
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Deployments
  /?Action=DescribeEcsClusters:
    get:
      summary: Describe Ecs Clusters
      description: Describes Amazon ECS clusters that are registered with a stack.
      operationId: describeEcsClusters
      x-api-path-slug: actiondescribeecsclusters-get
      parameters:
      - in: query
        name: EcsClusterArns
        description: A list of ARNs, one for each cluster to be described
        type: string
      - in: query
        name: MaxResults
        description: To receive a paginated response, use this parameter to specify
          the maximum number      of results to be returned with a single call
        type: string
      - in: query
        name: NextToken
        description: If the previous paginated request did not return all of the remaining
          results,      the response objectsNextToken parameter value is set to a
          token
        type: string
      - in: query
        name: StackId
        description: A stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Ecs
      - Clusters
  /?Action=DescribeElasticIps:
    get:
      summary: Describes Elastic IPs
      description: Describes Elastic IPs
      operationId: describeElasticIps
      x-api-path-slug: actiondescribeelasticips-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      - in: query
        name: Ips
        description: An array of Elastic IP addresses to be described
        type: string
      - in: query
        name: StackId
        description: A stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describes
      - Elastic
      - IP Addressess
  /?Action=DescribeElasticLoadBalancers:
    get:
      summary: Describe Elastic Load Balancers
      description: Describes a stack's Elastic Load Balancing instances.
      operationId: describeElasticLoadBalancers
      x-api-path-slug: actiondescribeelasticloadbalancers-get
      parameters:
      - in: query
        name: LayerIds
        description: A list of layer IDs
        type: string
      - in: query
        name: StackId
        description: A stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Elastic
      - Load
      - Balancers
  /?Action=DescribeInstances:
    get:
      summary: Describe Instances
      description: Requests a description of a set of instances.
      operationId: describeInstances
      x-api-path-slug: actiondescribeinstances-get
      parameters:
      - in: query
        name: InstanceIds
        description: An array of instance IDs to be described
        type: string
      - in: query
        name: LayerId
        description: A layer ID
        type: string
      - in: query
        name: StackId
        description: A stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Instances
  /?Action=DescribeLayers:
    get:
      summary: Describe Layers
      description: Requests a description of one or more layers in a specified stack.
      operationId: describeLayers
      x-api-path-slug: actiondescribelayers-get
      parameters:
      - in: query
        name: LayerIds
        description: An array of layer IDs that specify the layers to be described
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Layers
  /?Action=DescribeLoadBasedAutoScaling:
    get:
      summary: Describe Load Based Auto Scaling
      description: Describes load-based auto scaling configurations for specified
        layers.
      operationId: describeLoadBasedAutoScaling
      x-api-path-slug: actiondescribeloadbasedautoscaling-get
      parameters:
      - in: query
        name: LayerIds
        description: An array of layer IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Load
      - Based
      - Auto
      - Scaling
  /?Action=DescribeMyUserProfile:
    get:
      summary: Describe My User Profile
      description: Describes a user's SSH information.
      operationId: describeMyUserProfile
      x-api-path-slug: actiondescribemyuserprofile-get
      parameters:
      - in: query
        name: UserProfile
        description: A UserProfile object that describes the users SSH information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - My
      - User
      - Profile
  /?Action=DescribePermissions:
    get:
      summary: Describe Permissions
      description: Describes the permissions for a specified stack.
      operationId: describePermissions
      x-api-path-slug: actiondescribepermissions-get
      parameters:
      - in: query
        name: IamUserArn
        description: The users IAM ARN
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Permissions
  /?Action=DescribeRaidArrays:
    get:
      summary: Describe Raid Arrays
      description: Describe an instance's RAID arrays.
      operationId: describeRaidArrays
      x-api-path-slug: actiondescriberaidarrays-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      - in: query
        name: RaidArrayIds
        description: An array of RAID array IDs
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Raid
      - Arrays
  /?Action=DescribeRdsDbInstances:
    get:
      summary: Describe Rds Db Instances
      description: Describes Amazon RDS instances.
      operationId: describeRdsDbInstances
      x-api-path-slug: actiondescriberdsdbinstances-get
      parameters:
      - in: query
        name: RdsDbInstanceArns
        description: An array containing the ARNs of the instances to be described
        type: string
      - in: query
        name: StackId
        description: The stack ID that the instances are registered with
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Rds
      - Db
      - Instances
  /?Action=DescribeServiceErrors:
    get:
      summary: Describe Service Errors
      description: Describes AWS OpsWorks Stacks service errors.
      operationId: describeServiceErrors
      x-api-path-slug: actiondescribeserviceerrors-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      - in: query
        name: ServiceErrorIds
        description: An array of service error IDs
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Service
      - Errors
  /?Action=DescribeStackProvisioningParameters:
    get:
      summary: Describe Stack Provisioning Parameters
      description: Requests a description of a stack's provisioning parameters.
      operationId: describeStackProvisioningParameters
      x-api-path-slug: actiondescribestackprovisioningparameters-get
      parameters:
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Stack
      - Provisioning
      - Parameters
  /?Action=DescribeStacks:
    get:
      summary: Describe Stacks
      description: Requests a description of one or more stacks.
      operationId: describeStacks
      x-api-path-slug: actiondescribestacks-get
      parameters:
      - in: query
        name: StackIds
        description: An array of stack IDs that specify the stacks to be described
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Stacks
  /?Action=DescribeStackSummary:
    get:
      summary: Describe Stack Summary
      description: |-
        Describes the number of layers and apps in a specified stack, and the number of instances in
              each state, such as running_setup or online.
      operationId: describeStackSummary
      x-api-path-slug: actiondescribestacksummary-get
      parameters:
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Stack
      - Summary
  /?Action=DescribeTimeBasedAutoScaling:
    get:
      summary: Describe Time Based Auto Scaling
      description: Describes time-based auto scaling configurations for specified
        instances.
      operationId: describeTimeBasedAutoScaling
      x-api-path-slug: actiondescribetimebasedautoscaling-get
      parameters:
      - in: query
        name: InstanceIds
        description: An array of instance IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Time
      - Based
      - Auto
      - Scaling
  /?Action=DescribeUserProfiles:
    get:
      summary: Describe User Profiles
      description: Describe specified users.
      operationId: describeUserProfiles
      x-api-path-slug: actiondescribeuserprofiles-get
      parameters:
      - in: query
        name: IamUserArns
        description: An array of IAM or federated user ARNs that identify the users
          to be described
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - User
      - Profiles
  /?Action=DescribeVolumes:
    get:
      summary: Describe Volumes
      description: Describes an instance's Amazon EBS volumes.
      operationId: describeVolumes
      x-api-path-slug: actiondescribevolumes-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      - in: query
        name: RaidArrayId
        description: The RAID array ID
        type: string
      - in: query
        name: StackId
        description: A stack ID
        type: string
      - in: query
        name: VolumeIds
        description: Am array of volume IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Volumes
  /?Action=DetachElasticLoadBalancer:
    get:
      summary: Detach Elastic Load Balancer
      description: Detaches a specified Elastic Load Balancing instance from its layer.
      operationId: detachElasticLoadBalancer
      x-api-path-slug: actiondetachelasticloadbalancer-get
      parameters:
      - in: query
        name: ElasticLoadBalancerName
        description: The Elastic Load Balancing instances name
        type: string
      - in: query
        name: LayerId
        description: The ID of the layer that the Elastic Load Balancing instance
          is attached to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Detach
      - Elastic
      - Load
      - Balancer
  /?Action=DisassociateElasticIp:
    get:
      summary: Disassociate Elastic Ip
      description: Disassociates an Elastic IP address from its instance.
      operationId: disassociateElasticIp
      x-api-path-slug: actiondisassociateelasticip-get
      parameters:
      - in: query
        name: ElasticIp
        description: The Elastic IP address
        type: string
      responses:
        200:
          description: OK
      tags:
      - Disassociate
      - Elastic
      - Ip
  /?Action=GetHostnameSuggestion:
    get:
      summary: Get Hostname Suggestion
      description: Gets a generated host name for the specified layer, based on the
        current host name theme.
      operationId: getHostnameSuggestion
      x-api-path-slug: actiongethostnamesuggestion-get
      parameters:
      - in: query
        name: LayerId
        description: The layer ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Hostname
      - Suggestion
  /?Action=GrantAccess:
    get:
      summary: Grant Access
      description: NoteThis action can be used only with Windows stacks.
      operationId: grantAccess
      x-api-path-slug: actiongrantaccess-get
      parameters:
      - in: query
        name: InstanceId
        description: The instances AWS OpsWorks Stacks ID
        type: string
      - in: query
        name: ValidForInMinutes
        description: The length of time (in minutes) that the grant is valid
        type: string
      responses:
        200:
          description: OK
      tags:
      - Grant
      - Access
  /?Action=RebootInstance:
    get:
      summary: Reboot Instance
      description: Reboots a specified instance.
      operationId: rebootInstance
      x-api-path-slug: actionrebootinstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reboot
      - Instance
  /?Action=RegisterEcsCluster:
    get:
      summary: Register Ecs Cluster
      description: Registers a specified Amazon ECS cluster with a stack.
      operationId: registerEcsCluster
      x-api-path-slug: actionregisterecscluster-get
      parameters:
      - in: query
        name: EcsClusterArn
        description: The clusters ARN
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Ecs
      - Cluster
  /?Action=RegisterElasticIp:
    get:
      summary: Register Elastic Ip
      description: Registers an Elastic IP address with a specified stack.
      operationId: registerElasticIp
      x-api-path-slug: actionregisterelasticip-get
      parameters:
      - in: query
        name: ElasticIp
        description: The Elastic IP address
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Elastic
      - Ip
  /?Action=RegisterInstance:
    get:
      summary: Register Instance
      description: Registers instances that were created outside of AWS OpsWorks Stacks
        with a specified stack.
      operationId: registerInstance
      x-api-path-slug: actionregisterinstance-get
      parameters:
      - in: query
        name: Hostname
        description: The instances hostname
        type: string
      - in: query
        name: InstanceIdentity
        description: An InstanceIdentity object that contains the instances identity
        type: string
      - in: query
        name: PrivateIp
        description: The instances private IP address
        type: string
      - in: query
        name: PublicIp
        description: The instances public IP address
        type: string
      - in: query
        name: RsaPublicKey
        description: The instances public RSA key
        type: string
      - in: query
        name: RsaPublicKeyFingerprint
        description: The instances public RSA key fingerprint
        type: string
      - in: query
        name: StackId
        description: The ID of the stack that the instance is to be registered with
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Instance
  /?Action=RegisterRdsDbInstance:
    get:
      summary: Register Rds Db Instance
      description: Registers an Amazon RDS instance with a stack.
      operationId: registerRdsDbInstance
      x-api-path-slug: actionregisterrdsdbinstance-get
      parameters:
      - in: query
        name: DbPassword
        description: The database password
        type: string
      - in: query
        name: DbUser
        description: The databases master user name
        type: string
      - in: query
        name: RdsDbInstanceArn
        description: The Amazon RDS instances ARN
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Rds
      - Db
      - Instance
  /?Action=RegisterVolume:
    get:
      summary: Register Volume
      description: Registers an Amazon EBS volume with a specified stack.
      operationId: registerVolume
      x-api-path-slug: actionregistervolume-get
      parameters:
      - in: query
        name: Ec2VolumeId
        description: The Amazon EBS volume ID
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Volume
  /?Action=SetLoadBasedAutoScaling:
    get:
      summary: Set Load Based Auto Scaling
      description: Specify the load-based auto scaling configuration for a specified
        layer.
      operationId: setLoadBasedAutoScaling
      x-api-path-slug: actionsetloadbasedautoscaling-get
      parameters:
      - in: query
        name: DownScaling
        description: An AutoScalingThresholds object with the downscaling threshold
          configuration
        type: string
      - in: query
        name: Enable
        description: Enables load-based auto scaling for the layer
        type: string
      - in: query
        name: LayerId
        description: The layer ID
        type: string
      - in: query
        name: UpScaling
        description: An AutoScalingThresholds object with the upscaling threshold
          configuration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Set
      - Load
      - Based
      - Auto
      - Scaling
  /?Action=SetPermission:
    get:
      summary: Set Permission
      description: Specifies a user's permissions.
      operationId: setPermission
      x-api-path-slug: actionsetpermission-get
      parameters:
      - in: query
        name: AllowSsh
        description: The user is allowed to use SSH to communicate with the instance
        type: string
      - in: query
        name: AllowSudo
        description: The user is allowed to use sudo to elevate privileges
        type: string
      - in: query
        name: IamUserArn
        description: The users IAM ARN
        type: string
      - in: query
        name: Level
        description: The users permission level, which must be set to one of the following
          strings
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Set
      - Permission
  /?Action=SetTimeBasedAutoScaling:
    get:
      summary: Set Time Based Auto Scaling
      description: Specify the time-based auto scaling configuration for a specified
        instance.
      operationId: setTimeBasedAutoScaling
      x-api-path-slug: actionsettimebasedautoscaling-get
      parameters:
      - in: query
        name: AutoScalingSchedule
        description: An AutoScalingSchedule with the instance schedule
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Set
      - Time
      - Based
      - Auto
      - Scaling
  /?Action=StartInstance:
    get:
      summary: Start Instance
      description: Starts a specified instance.
      operationId: startInstance
      x-api-path-slug: actionstartinstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Start
      - Instance
  /?Action=StartStack:
    get:
      summary: Start Stack
      description: Starts a stack's instances.
      operationId: startStack
      x-api-path-slug: actionstartstack-get
      parameters:
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Start
      - Stack
  /?Action=StopInstance:
    get:
      summary: Stop Instance
      description: Stops a specified instance.
      operationId: stopInstance
      x-api-path-slug: actionstopinstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Instance
  /?Action=StopStack:
    get:
      summary: Stop Stack
      description: Stops a specified stack.
      operationId: stopStack
      x-api-path-slug: actionstopstack-get
      parameters:
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Stack
  /?Action=UnassignInstance:
    get:
      summary: Unassign Instance
      description: Unassigns a registered instance from all of it's layers.
      operationId: unassignInstance
      x-api-path-slug: actionunassigninstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Unassign
      - Instance
  /?Action=UnassignVolume:
    get:
      summary: Unassign Volume
      description: Unassigns an assigned Amazon EBS volume.
      operationId: unassignVolume
      x-api-path-slug: actionunassignvolume-get
      parameters:
      - in: query
        name: VolumeId
        description: The volume ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Unassign
      - Volume
  /?Action=UpdateApp:
    get:
      summary: Update App
      description: Updates a specified app.
      operationId: updateApp
      x-api-path-slug: actionupdateapp-get
      parameters:
      - in: query
        name: AppId
        description: The app ID
        type: string
      - in: query
        name: AppSource
        description: A Source object that specifies the app repository
        type: string
      - in: query
        name: Attributes
        description: One or more user-defined key/value pairs to be added to the stack
          attributes
        type: string
      - in: query
        name: DataSources
        description: The apps data sources
        type: string
      - in: query
        name: Description
        description: A description of the app
        type: string
      - in: query
        name: Domains
        description: The apps virtual host settings, with multiple domains separated
          by commas
        type: string
      - in: query
        name: EnableSsl
        description: Whether SSL is enabled for the app
        type: string
      - in: query
        name: Environment
        description: An array of EnvironmentVariable objects that specify environment
          variables to be      associated with the app
        type: string
      - in: query
        name: Name
        description: The app name
        type: string
      - in: query
        name: SslConfiguration
        description: An SslConfiguration object with the SSL configuration
        type: string
      - in: query
        name: Type
        description: The app type
        type: string
      responses:
        200:
          description: OK
      tags:
      - App
  /?Action=UpdateElasticIp:
    get:
      summary: Update Elastic Ip
      description: Updates a registered Elastic IP address's name.
      operationId: updateElasticIp
      x-api-path-slug: actionupdateelasticip-get
      parameters:
      - in: query
        name: ElasticIp
        description: The address
        type: string
      - in: query
        name: Name
        description: The new name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Elastic
      - Ip
  /?Action=UpdateInstance:
    get:
      summary: Update Instance
      description: Updates a specified instance.
      operationId: updateInstance
      x-api-path-slug: actionupdateinstance-get
      parameters:
      - in: query
        name: AgentVersion
        description: The default AWS OpsWorks Stacks agent version
        type: string
      - in: query
        name: AmiId
        description: The ID of the AMI that was used to create the instance
        type: string
      - in: query
        name: Architecture
        description: The instance architecture
        type: string
      - in: query
        name: AutoScalingType
        description: For load-based or time-based instances, the type
        type: string
      - in: query
        name: EbsOptimized
        description: This property cannot be updated
        type: string
      - in: query
        name: Hostname
        description: The instance host name
        type: string
      - in: query
        name: InstallUpdatesOnBoot
        description: Whether to install operating system and package updates when
          the instance boots
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      - in: query
        name: InstanceType
        description: The instance type, such as t2
        type: string
      - in: query
        name: LayerIds
        description: The instances layer IDs
        type: string
      - in: query
        name: Os
        description: The instances operating system, which must be set to one of the
          following
        type: string
      - in: query
        name: SshKeyName
        description: The instances Amazon EC2 key name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
  /?Action=UpdateLayer:
    get:
      summary: Update Layer
      description: Updates a specified layer.
      operationId: updateLayer
      x-api-path-slug: actionupdatelayer-get
      parameters:
      - in: query
        name: Attributes
        description: One or more user-defined key/value pairs to be added to the stack
          attributes
        type: string
      - in: query
        name: AutoAssignElasticIps
        description: Whether to automatically assign an Elastic IP        address
          to the layers instances
        type: string
      - in: query
        name: AutoAssignPublicIps
        description: For stacks that are running in a VPC, whether to automatically
          assign a public IP address to      the layers instances
        type: string
      - in: query
        name: CustomInstanceProfileArn
        description: The ARN of an IAM profile to be used for all of the layers EC2
          instances
        type: string
      - in: query
        name: CustomJson
        description: A JSON-formatted string containing custom stack configuration
          and deployment attributes      to be installed on the layers instances
        type: string
      - in: query
        name: CustomRecipes
        description: A LayerCustomRecipes object that specifies the layers custom
          recipes
        type: string
      - in: query
        name: CustomSecurityGroupIds
        description: An array containing the layers custom security group IDs
        type: string
      - in: query
        name: EnableAutoHealing
        description: Whether to disable auto healing for the layer
        type: string
      - in: query
        name: InstallUpdatesOnBoot
        description: Whether to install operating system and package updates when
          the instance boots
        type: string
      - in: query
        name: LayerId
        description: The layer ID
        type: string
      - in: query
        name: LifecycleEventConfiguration
        type: string
      - in: query
        name: Name
        description: The layer name, which is used by the console
        type: string
      - in: query
        name: Packages
        description: An array of Package objects that describe the layers packages
        type: string
      - in: query
        name: Shortname
        description: For custom layers only, use this parameter to specify the layers
          short name, which is used internally by AWS OpsWorks Stacks and by Chef
        type: string
      - in: query
        name: UseEbsOptimizedInstances
        description: Whether to use Amazon EBS-optimized instances
        type: string
      - in: query
        name: VolumeConfigurations
        description: A VolumeConfigurations object that describes the layers Amazon
          EBS volumes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Layer
  /?Action=UpdateMyUserProfile:
    get:
      summary: Update My User Profile
      description: Updates a user's SSH public key.
      operationId: updateMyUserProfile
      x-api-path-slug: actionupdatemyuserprofile-get
      parameters:
      - in: query
        name: SshPublicKey
        description: The users SSH public key
        type: string
      responses:
        200:
          description: OK
      tags:
      - My
      - User
      - Profile
  /?Action=UpdateRdsDbInstance:
    get:
      summary: Update Rds Db Instance
      description: Updates an Amazon RDS instance.
      operationId: updateRdsDbInstance
      x-api-path-slug: actionupdaterdsdbinstance-get
      parameters:
      - in: query
        name: DbPassword
        description: The database password
        type: string
      - in: query
        name: DbUser
        description: The master user name
        type: string
      - in: query
        name: RdsDbInstanceArn
        description: The Amazon RDS instances ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rds
      - Db
      - Instance
  /?Action=UpdateStack:
    get:
      summary: Update Stack
      description: Updates a specified stack.
      operationId: updateStack
      x-api-path-slug: actionupdatestack-get
      parameters:
      - in: query
        name: AgentVersion
        description: The default AWS OpsWorks Stacks agent version
        type: string
      - in: query
        name: Attributes
        description: One or more user-defined key-value pairs to be added to the stack
          attributes
        type: string
      - in: query
        name: ChefConfiguration
        description: A ChefConfiguration object that specifies whether to enable Berkshelf
          and the      Berkshelf version on Chef 11
        type: string
      - in: query
        name: ConfigurationManager
        description: The configuration manager
        type: string
      - in: query
        name: CustomCookbooksSource
        description: Contains the information required to retrieve an app or cookbook
          from a repository
        type: string
      - in: query
        name: CustomJson
        description: A string that contains user-defined, custom JSON
        type: string
      - in: query
        name: DefaultAvailabilityZone
        description: The stacks default Availability Zone, which must be in the      stacks
          region
        type: string
      - in: query
        name: DefaultInstanceProfileArn
        description: The ARN of an IAM profile that is the default profile for all
          of the stacks EC2 instances
        type: string
      - in: query
        name: DefaultOs
        description: 'The stacks operating system, which must be set to one of the
          following:'
        type: string
      - in: query
        name: DefaultRootDeviceType
        description: The default root device type
        type: string
      - in: query
        name: DefaultSshKeyName
        description: A default Amazon EC2 key-pair name
        type: string
      - in: query
        name: DefaultSubnetId
        description: The stacks default VPC subnet ID
        type: string
      - in: query
        name: HostnameTheme
        description: The stacks new host name theme, with spaces replaced by underscores
        type: string
      - in: query
        name: Name
        description: The stacks new name
        type: string
      - in: query
        name: ServiceRoleArn
        description: Do not use this parameter
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      - in: query
        name: UseCustomCookbooks
        description: Whether the stack uses custom cookbooks
        type: string
      - in: query
        name: UseOpsworksSecurityGroups
        description: Whether to associate the AWS OpsWorks Stacks built-in security
          groups with the stacks layers
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack
  /?Action=UpdateUserProfile:
    get:
      summary: Update User Profile
      description: Updates a specified user profile.
      operationId: updateUserProfile
      x-api-path-slug: actionupdateuserprofile-get
      parameters:
      - in: query
        name: AllowSelfManagement
        description: Whether users can specify their own SSH public key through the
          My Settings page
        type: string
      - in: query
        name: IamUserArn
        description: The user IAM ARN
        type: string
      - in: query
        name: SshPublicKey
        description: The users new SSH public key
        type: string
      - in: query
        name: SshUsername
        description: The users SSH user name
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Profile
  /?Action=UpdateVolume:
    get:
      summary: Update Volume
      description: Updates an Amazon EBS volume's name or mount point.
      operationId: updateVolume
      x-api-path-slug: actionupdatevolume-get
      parameters:
      - in: query
        name: MountPoint
        description: The new mount point
        type: string
      - in: query
        name: Name
        description: The new name
        type: string
      - in: query
        name: VolumeId
        description: The volume ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Volume