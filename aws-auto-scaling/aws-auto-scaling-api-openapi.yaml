swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 1
info:
  title: AWS Auto Scaling API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AttachInstances:
    get:
      summary: Attach Instances
      description: Attaches one or more EC2 instances to the specified Auto Scaling
        group.
      operationId: attachInstances
      x-api-path-slug: actionattachinstances-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: InstanceIds.member.N
        description: One or more instance IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance
  /?Action=AttachLoadBalancers:
    get:
      summary: Attach Load Balancers
      description: Attaches one or more Classic load balancers to the specified Auto
        Scaling group.
      operationId: attachLoadBalancers
      x-api-path-slug: actionattachloadbalancers-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: LoadBalancerNames.member.N
        description: One or more load balancer names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=AttachLoadBalancerTargetGroups:
    get:
      summary: Attach Load Balancer Target Groups
      description: Attaches one or more target groups to the specified Auto Scaling
        group.
      operationId: attachLoadBalancerTargetGroups
      x-api-path-slug: actionattachloadbalancertargetgroups-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: TargetGroupARNs.member.N
        description: The Amazon Resource Names (ARN) of the target groups
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=CompleteLifecycleAction:
    get:
      summary: Complete Lifecycle Action
      description: Completes the lifecycle action for the specified token or instance
        with the specified result.
      operationId: completeLifecycleAction
      x-api-path-slug: actioncompletelifecycleaction-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group for the lifecycle hook
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: LifecycleActionResult
        description: The action for the group to take
        type: string
      - in: query
        name: LifecycleActionToken
        description: A universally unique identifier (UUID) that identifies a specific
          lifecycle action associated with an instance
        type: string
      - in: query
        name: LifecycleHookName
        description: The name of the lifecycle hook
        type: string
      responses:
        200:
          description: OK
      tags:
      - Life Cycle
  /?Action=CreateAutoScalingGroup:
    get:
      summary: Create Auto Scaling Group
      description: Creates an Auto Scaling group with the specified name and attributes.
      operationId: createAutoScalingGroup
      x-api-path-slug: actioncreateautoscalinggroup-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: AvailabilityZones.member.N
        description: One or more Availability Zones for the group
        type: string
      - in: query
        name: DefaultCooldown
        description: The amount of time, in seconds, after a scaling activity completes
          before another scaling activity can start
        type: string
      - in: query
        name: DesiredCapacity
        description: The number of EC2 instances that should be running in the group
        type: string
      - in: query
        name: HealthCheckGracePeriod
        description: The amount of time, in seconds, that Auto Scaling waits before
          checking the health status of an EC2 instance that has come into service
        type: string
      - in: query
        name: HealthCheckType
        description: The service to use for the health checks
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance used to create a launch configuration
          for the group
        type: string
      - in: query
        name: LaunchConfigurationName
        description: The name of the launch configuration
        type: string
      - in: query
        name: LoadBalancerNames.member.N
        description: One or more Classic load balancers
        type: string
      - in: query
        name: MaxSize
        description: The maximum size of the group
        type: string
      - in: query
        name: MinSize
        description: The minimum size of the group
        type: string
      - in: query
        name: NewInstancesProtectedFromScaleIn
        description: Indicates whether newly launched instances are protected from
          termination by Auto Scaling when scaling in
        type: string
      - in: query
        name: PlacementGroup
        description: The name of the placement group into which youll launch your
          instances, if any
        type: string
      - in: query
        name: Tags.member.N
        description: One or more tags
        type: string
      - in: query
        name: TargetGroupARNs.member.N
        description: The Amazon Resource Names (ARN) of the target groups
        type: string
      - in: query
        name: TerminationPolicies.member.N
        description: One or more termination policies used to select the instance
          to terminate
        type: string
      - in: query
        name: VPCZoneIdentifier
        description: A comma-separated list of subnet identifiers for your virtual
          private cloud (VPC)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Auto Scaling Groups
  /?Action=CreateLaunchConfiguration:
    get:
      summary: Create Launch Configuration
      description: Creates a launch configuration.
      operationId: createLaunchConfiguration
      x-api-path-slug: actioncreatelaunchconfiguration-get
      parameters:
      - in: query
        name: AssociatePublicIpAddress
        description: Used for groups that launch instances into a virtual private
          cloud (VPC)
        type: string
      - in: query
        name: BlockDeviceMappings.member.N
        description: One or more mappings that specify how block devices are exposed
          to the instance
        type: string
      - in: query
        name: ClassicLinkVPCId
        description: The ID of a ClassicLink-enabled VPC to link your EC2-Classic
          instances to
        type: string
      - in: query
        name: ClassicLinkVPCSecurityGroups.member.N
        description: The IDs of one or more security groups for the specified ClassicLink-enabled
          VPC
        type: string
      - in: query
        name: EbsOptimized
        description: Indicates whether the instance is optimized for Amazon EBS I/O
        type: string
      - in: query
        name: IamInstanceProfile
        description: The name or the Amazon Resource Name (ARN) of the instance profile
          associated with the IAM role for the instance
        type: string
      - in: query
        name: ImageId
        description: The ID of the Amazon Machine Image (AMI) to use to launch your
          EC2 instances
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance to use to create the launch configuration
        type: string
      - in: query
        name: InstanceMonitoring
        description: Enables detailed monitoring (true) or basic monitoring (false)
          for the Auto Scaling instances
        type: string
      - in: query
        name: InstanceType
        description: The instance type of the EC2 instance
        type: string
      - in: query
        name: KernelId
        description: The ID of the kernel associated with the AMI
        type: string
      - in: query
        name: KeyName
        description: The name of the key pair
        type: string
      - in: query
        name: LaunchConfigurationName
        description: The name of the launch configuration
        type: string
      - in: query
        name: PlacementTenancy
        description: The tenancy of the instance
        type: string
      - in: query
        name: RamdiskId
        description: The ID of the RAM disk associated with the AMI
        type: string
      - in: query
        name: SecurityGroups.member.N
        description: One or more security groups with which to associate the instances
        type: string
      - in: query
        name: SpotPrice
        description: The maximum hourly price to be paid for any Spot Instance launched
          to fulfill the request
        type: string
      - in: query
        name: UserData
        description: The user data to make available to the launched EC2 instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Launch
  /?Action=CreateOrUpdateTags:
    get:
      summary: Create Or Update Tags
      description: Creates or updates tags for the specified Auto Scaling group.
      operationId: createOrUpdateTags
      x-api-path-slug: actioncreateorupdatetags-get
      parameters:
      - in: query
        name: Tags.member.N
        description: One or more tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=DeleteAutoScalingGroup:
    get:
      summary: Delete Auto Scaling Group
      description: Deletes the specified Auto Scaling group.
      operationId: deleteAutoScalingGroup
      x-api-path-slug: actiondeleteautoscalinggroup-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group to delete
        type: string
      - in: query
        name: ForceDelete
        description: Specifies that the group will be deleted along with all instances
          associated with the group, without waiting for all instances to be terminated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Auto Scaling Groups
  /?Action=DeleteLaunchConfiguration:
    get:
      summary: Delete Launch Configuration
      description: Deletes the specified launch configuration.
      operationId: deleteLaunchConfiguration
      x-api-path-slug: actiondeletelaunchconfiguration-get
      parameters:
      - in: query
        name: LaunchConfigurationName
        description: The name of the launch configuration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Launch
  /?Action=DeleteLifecycleHook:
    get:
      summary: Delete Lifecycle Hook
      description: Deletes the specified lifecycle hook.
      operationId: deleteLifecycleHook
      x-api-path-slug: actiondeletelifecyclehook-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group for the lifecycle hook
        type: string
      - in: query
        name: LifecycleHookName
        description: The name of the lifecycle hook
        type: string
      responses:
        200:
          description: OK
      tags:
      - Life Cycle
  /?Action=DeleteNotificationConfiguration:
    get:
      summary: Delete Notification Configuration
      description: Deletes the specified notification.
      operationId: deleteNotificationConfiguration
      x-api-path-slug: actiondeletenotificationconfiguration-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: TopicARN
        description: The Amazon Resource Name (ARN) of the Amazon Simple Notification
          Service (SNS) topic
        type: string
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /?Action=DeletePolicy:
    get:
      summary: Delete Policy
      description: Deletes the specified Auto Scaling policy.
      operationId: deletePolicy
      x-api-path-slug: actiondeletepolicy-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: PolicyName
        description: The name or Amazon Resource Name (ARN) of the policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=DeleteScheduledAction:
    get:
      summary: Delete Scheduled Action
      description: Deletes the specified scheduled action.
      operationId: deleteScheduledAction
      x-api-path-slug: actiondeletescheduledaction-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: ScheduledActionName
        description: The name of the action to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scheduled Action
  /?Action=DeleteTags:
    get:
      summary: Delete Tags
      description: Deletes the specified tags.
      operationId: deleteTags
      x-api-path-slug: actiondeletetags-get
      parameters:
      - in: query
        name: Tags.member.N
        description: One or more tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=DescribeAccountLimits:
    get:
      summary: Describe Account Limits
      description: Describes the current Auto Scaling resource limits for your AWS
        account.
      operationId: describeAccountLimits
      x-api-path-slug: actiondescribeaccountlimits-get
      parameters:
      - in: query
        name: MaxNumberOfAutoScalingGroups
        description: The maximum number of groups allowed for your AWS account
        type: string
      - in: query
        name: MaxNumberOfLaunchConfigurations
        description: The maximum number of launch configurations allowed for your
          AWS account
        type: string
      - in: query
        name: NumberOfAutoScalingGroups
        description: The current number of groups for your AWS account
        type: string
      - in: query
        name: NumberOfLaunchConfigurations
        description: The current number of launch configurations for your AWS account
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Limits
  /?Action=DescribeAdjustmentTypes:
    get:
      summary: Describe Adjustment Types
      description: Describes the policy adjustment types for use with.
      operationId: describeAdjustmentTypes
      x-api-path-slug: actiondescribeadjustmenttypes-get
      parameters:
      - in: query
        name: AdjustmentTypes.member.N
        description: The policy adjustment types
        type: string
      responses:
        200:
          description: OK
      tags:
      - Adjustment Types
  /?Action=DescribeAutoScalingGroups:
    get:
      summary: Describe Auto Scaling Groups
      description: Describes one or more Auto Scaling groups.
      operationId: describeAutoScalingGroups
      x-api-path-slug: actiondescribeautoscalinggroups-get
      parameters:
      - in: query
        name: AutoScalingGroupNames.member.N
        description: The group names
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Auto Scaling Groups
  /?Action=DescribeAutoScalingInstances:
    get:
      summary: Describe Auto Scaling Instances
      description: Describes one or more Auto Scaling instances.
      operationId: describeAutoScalingInstances
      x-api-path-slug: actiondescribeautoscalinginstances-get
      parameters:
      - in: query
        name: InstanceIds.member.N
        description: The instances to describe; up to 50 instance IDs
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Auto Scaling Instances
  /?Action=DescribeAutoScalingNotificationTypes:
    get:
      summary: Describe Auto Scaling Notification Types
      description: Describes the notification types that are supported by Auto Scaling.
      operationId: describeAutoScalingNotificationTypes
      x-api-path-slug: actiondescribeautoscalingnotificationtypes-get
      parameters:
      - in: query
        name: AutoScalingNotificationTypes.member.N
        description: The notification types
        type: string
      responses:
        200:
          description: OK
      tags:
      - Auto Scaling Notifications
  /?Action=DescribeLaunchConfigurations:
    get:
      summary: Describe Launch Configurations
      description: Describes one or more launch configurations.
      operationId: describeLaunchConfigurations
      x-api-path-slug: actiondescribelaunchconfigurations-get
      parameters:
      - in: query
        name: LaunchConfigurationNames.member.N
        description: The launch configuration names
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Launch
  /?Action=DescribeLifecycleHooks:
    get:
      summary: Describe Lifecycle Hooks
      description: Describes the lifecycle hooks for the specified Auto Scaling group.
      operationId: describeLifecycleHooks
      x-api-path-slug: actiondescribelifecyclehooks-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: LifecycleHookNames.member.N
        description: The names of one or more lifecycle hooks
        type: string
      responses:
        200:
          description: OK
      tags:
      - Life Cycle
  /?Action=DescribeLifecycleHookTypes:
    get:
      summary: Describe Lifecycle Hook Types
      description: Describes the available types of lifecycle hooks.
      operationId: describeLifecycleHookTypes
      x-api-path-slug: actiondescribelifecyclehooktypes-get
      parameters:
      - in: query
        name: LifecycleHookTypes.member.N
        description: The lifecycle hook types
        type: string
      responses:
        200:
          description: OK
      tags:
      - Life Cycle
  /?Action=DescribeLoadBalancers:
    get:
      summary: Describe Load Balancers
      description: Describes the load balancers for the specified Auto Scaling group.
      operationId: describeLoadBalancers
      x-api-path-slug: actiondescribeloadbalancers-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=DescribeLoadBalancerTargetGroups:
    get:
      summary: Describe Load Balancer Target Groups
      description: Describes the target groups for the specified Auto Scaling group.
      operationId: describeLoadBalancerTargetGroups
      x-api-path-slug: actiondescribeloadbalancertargetgroups-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=DescribeMetricCollectionTypes:
    get:
      summary: Describe Metric Collection Types
      description: Describes the available CloudWatch metrics for Auto Scaling.
      operationId: describeMetricCollectionTypes
      x-api-path-slug: actiondescribemetriccollectiontypes-get
      parameters:
      - in: query
        name: Granularities.member.N
        description: The granularities for the metrics
        type: string
      - in: query
        name: Metrics.member.N
        description: One or more metrics
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metric Collection
  /?Action=DescribeNotificationConfigurations:
    get:
      summary: Describe Notification Configurations
      description: Describes the notification actions associated with the specified
        Auto Scaling group.
      operationId: describeNotificationConfigurations
      x-api-path-slug: actiondescribenotificationconfigurations-get
      parameters:
      - in: query
        name: AutoScalingGroupNames.member.N
        description: The name of the group
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /?Action=DescribePolicies:
    get:
      summary: Describe Policies
      description: Describes the policies for the specified Auto Scaling group.
      operationId: describePolicies
      x-api-path-slug: actiondescribepolicies-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to be returned with each call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: PolicyNames.member.N
        description: One or more policy names or policy ARNs to be described
        type: string
      - in: query
        name: PolicyTypes.member.N
        description: One or more policy types
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=DescribeScalingActivities:
    get:
      summary: Describe Scaling Activities
      description: Describes one or more scaling activities for the specified Auto
        Scaling group.
      operationId: describeScalingActivities
      x-api-path-slug: actiondescribescalingactivities-get
      parameters:
      - in: query
        name: ActivityIds.member.N
        description: The activity IDs of the desired scaling activities
        type: string
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scaling Activities
  /?Action=DescribeScalingProcessTypes:
    get:
      summary: Describe Scaling Process Types
      description: Describes the scaling process types for use with.
      operationId: describeScalingProcessTypes
      x-api-path-slug: actiondescribescalingprocesstypes-get
      parameters:
      - in: query
        name: Processes.member.N
        description: The names of the process types
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scaling Process
  /?Action=DescribeScheduledActions:
    get:
      summary: Describe Scheduled Actions
      description: Describes the actions scheduled for your Auto Scaling group that
        haven't run.
      operationId: describeScheduledActions
      x-api-path-slug: actiondescribescheduledactions-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: EndTime
        description: The latest scheduled start time to return
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: ScheduledActionNames.member.N
        description: Describes one or more scheduled actions
        type: string
      - in: query
        name: StartTime
        description: The earliest scheduled start time to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scheduled Actions
  /?Action=DescribeTags:
    get:
      summary: Describe Tags
      description: Describes the specified tags.
      operationId: describeTags
      x-api-path-slug: actiondescribetags-get
      parameters:
      - in: query
        name: Filters.member.N
        description: A filter used to scope the tags to return
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=DescribeTerminationPolicyTypes:
    get:
      summary: Describe Termination Policy Types
      description: Describes the termination policies supported by Auto Scaling.
      operationId: describeTerminationPolicyTypes
      x-api-path-slug: actiondescribeterminationpolicytypes-get
      parameters:
      - in: query
        name: TerminationPolicyTypes.member.N
        description: The termination policies supported by Auto Scaling (OldestInstance,
          OldestLaunchConfiguration,             NewestInstance, ClosestToNextInstanceHour,
          and Default)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Termination Policies
  /?Action=DetachInstances:
    get:
      summary: Detach Instances
      description: Removes one or more instances from the specified Auto Scaling group.
      operationId: detachInstances
      x-api-path-slug: actiondetachinstances-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: InstanceIds.member.N
        description: One or more instance IDs
        type: string
      - in: query
        name: ShouldDecrementDesiredCapacity
        description: If True, the Auto Scaling group decrements the desired capacity
          value by the number of instances detached
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instances
  /?Action=DetachLoadBalancers:
    get:
      summary: Detach Load Balancers
      description: Detaches one or more Classic load balancers from the specified
        Auto Scaling group.
      operationId: detachLoadBalancers
      x-api-path-slug: actiondetachloadbalancers-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: LoadBalancerNames.member.N
        description: One or more load balancer names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=DetachLoadBalancerTargetGroups:
    get:
      summary: Detach Load Balancer Target Groups
      description: Detaches one or more target groups from the specified Auto Scaling
        group.
      operationId: detachLoadBalancerTargetGroups
      x-api-path-slug: actiondetachloadbalancertargetgroups-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: TargetGroupARNs.member.N
        description: The Amazon Resource Names (ARN) of the target groups
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=DisableMetricsCollection:
    get:
      summary: Disable Metrics Collection
      description: Disables group metrics for the specified Auto Scaling group.
      operationId: disableMetricsCollection
      x-api-path-slug: actiondisablemetricscollection-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name or Amazon Resource Name (ARN) of the group
        type: string
      - in: query
        name: Metrics.member.N
        description: One or more of the following metrics
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metrics Collection
  /?Action=EnableMetricsCollection:
    get:
      summary: Enable Metrics Collection
      description: Enables group metrics for the specified Auto Scaling group.
      operationId: enableMetricsCollection
      x-api-path-slug: actionenablemetricscollection-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name or ARN of the Auto Scaling group
        type: string
      - in: query
        name: Granularity
        description: The granularity to associate with the metrics to collect
        type: string
      - in: query
        name: Metrics.member.N
        description: One or more of the following metrics
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metrics Collection
  /?Action=EnterStandby:
    get:
      summary: Enter Standby
      description: Moves the specified instances into Standby mode.
      operationId: enterStandby
      x-api-path-slug: actionenterstandby-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: InstanceIds.member.N
        description: One or more instances to move into Standby mode
        type: string
      - in: query
        name: ShouldDecrementDesiredCapacity
        description: Specifies whether the instances moved to Standby mode count as
          part of the Auto Scaling groups desired capacity
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stand By
  /?Action=ExecutePolicy:
    get:
      summary: Execute Policy
      description: Executes the specified policy.
      operationId: executePolicy
      x-api-path-slug: actionexecutepolicy-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name or Amazon Resource Name (ARN) of the Auto Scaling group
        type: string
      - in: query
        name: BreachThreshold
        description: The breach threshold for the alarm
        type: string
      - in: query
        name: HonorCooldown
        description: If this parameter is true, Auto Scaling waits for the cooldown
          period to complete before executing the policy
        type: string
      - in: query
        name: MetricValue
        description: The metric value to compare to BreachThreshold
        type: string
      - in: query
        name: PolicyName
        description: The name or ARN of the policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=ExitStandby:
    get:
      summary: Exit Standby
      description: Moves the specified instances out of Standby mode.
      operationId: exitStandby
      x-api-path-slug: actionexitstandby-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: InstanceIds.member.N
        description: One or more instance IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stand By
  /?Action=PutLifecycleHook:
    get:
      summary: Put Lifecycle Hook
      description: Creates or updates a lifecycle hook for the specified Auto Scaling
        Group.
      operationId: putLifecycleHook
      x-api-path-slug: actionputlifecyclehook-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group to which you want to assign
          the lifecycle hook
        type: string
      - in: query
        name: DefaultResult
        description: Defines the action the Auto Scaling group should take when the
          lifecycle hook timeout elapses or if an unexpected failure occurs
        type: string
      - in: query
        name: HeartbeatTimeout
        description: The amount of time, in seconds, that can elapse before the lifecycle
          hook times out
        type: string
      - in: query
        name: LifecycleHookName
        description: The name of the lifecycle hook
        type: string
      - in: query
        name: LifecycleTransition
        description: The instance state to which you want to attach the lifecycle
          hook
        type: string
      - in: query
        name: NotificationMetadata
        description: Contains additional information that you want to include any
          time Auto Scaling sends a message to the notification target
        type: string
      - in: query
        name: NotificationTargetARN
        description: The ARN of the notification target that Auto Scaling will use
          to notify you when an instance is in the transition state for the lifecycle
          hook
        type: string
      - in: query
        name: RoleARN
        description: The ARN of the IAM role that allows the Auto Scaling group to
          publish to the specified notification target
        type: string
      responses:
        200:
          description: OK
      tags:
      - Life Cycle
  /?Action=PutNotificationConfiguration:
    get:
      summary: Put Notification Configuration
      description: Configures an Auto Scaling group to send notifications when specified
        events take place.
      operationId: putNotificationConfiguration
      x-api-path-slug: actionputnotificationconfiguration-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: NotificationTypes.member.N
        description: The type of event that will cause the notification to be sent
        type: string
      - in: query
        name: TopicARN
        description: The Amazon Resource Name (ARN) of the Amazon Simple Notification
          Service (SNS) topic
        type: string
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /?Action=PutScalingPolicy:
    get:
      summary: Put Scaling Policy
      description: Creates or updates a policy for an Auto Scaling group.
      operationId: putScalingPolicy
      x-api-path-slug: actionputscalingpolicy-get
      parameters:
      - in: query
        name: AdjustmentType
        description: The adjustment type
        type: string
      - in: query
        name: AutoScalingGroupName
        description: The name or ARN of the group
        type: string
      - in: query
        name: Cooldown
        description: The amount of time, in seconds, after a scaling activity completes
          and before the next scaling activity can start
        type: string
      - in: query
        name: EstimatedInstanceWarmup
        description: The estimated time, in seconds, until a newly launched instance
          can contribute to the CloudWatch metrics
        type: string
      - in: query
        name: MetricAggregationType
        description: The aggregation type for the CloudWatch metrics
        type: string
      - in: query
        name: MinAdjustmentMagnitude
        description: The minimum number of instances to scale
        type: string
      - in: query
        name: MinAdjustmentStep
        description: Available for backward compatibility
        type: string
      - in: query
        name: PolicyName
        description: The name of the policy
        type: string
      - in: query
        name: PolicyType
        description: The policy type
        type: string
      - in: query
        name: ScalingAdjustment
        description: The amount by which to scale, based on the specified adjustment
          type
        type: string
      - in: query
        name: StepAdjustments.member.N
        description: A set of adjustments that enable you to scale based on the size
          of the alarm breach
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scaling Policy
  /?Action=PutScheduledUpdateGroupAction:
    get:
      summary: Put Scheduled Update Group Action
      description: Creates or updates a scheduled scaling action for an Auto Scaling
        group.
      operationId: putScheduledUpdateGroupAction
      x-api-path-slug: actionputscheduledupdategroupaction-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name or Amazon Resource Name (ARN) of the Auto Scaling group
        type: string
      - in: query
        name: DesiredCapacity
        description: The number of EC2 instances that should be running in the group
        type: string
      - in: query
        name: EndTime
        description: The time for the recurring schedule to end
        type: string
      - in: query
        name: MaxSize
        description: The maximum size for the Auto Scaling group
        type: string
      - in: query
        name: MinSize
        description: The minimum size for the Auto Scaling group
        type: string
      - in: query
        name: Recurrence
        description: The recurring schedule for this action, in Unix cron syntax format
        type: string
      - in: query
        name: ScheduledActionName
        description: The name of this scaling action
        type: string
      - in: query
        name: StartTime
        description: The time for this action to start, in YYYY-MM-DDThh:mm:ssZ format
          in UTC/GMT only             (for example, 2014-06-01T00:00:00Z)
        type: string
      - in: query
        name: Time
        description: This parameter is deprecated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scheduled Update
  /?Action=RecordLifecycleActionHeartbeat:
    get:
      summary: Record Lifecycle Action Heartbeat
      description: Records a heartbeat for the lifecycle action associated with the
        specified token or instance.
      operationId: recordLifecycleActionHeartbeat
      x-api-path-slug: actionrecordlifecycleactionheartbeat-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group for the hook
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: LifecycleActionToken
        description: A token that uniquely identifies a specific lifecycle action
          associated with an instance
        type: string
      - in: query
        name: LifecycleHookName
        description: The name of the lifecycle hook
        type: string
      responses:
        200:
          description: OK
      tags:
      - Life Cycle
  /?Action=ResumeProcesses:
    get:
      summary: Resume Processes
      description: Resumes the specified suspended Auto Scaling processes, or all
        suspended process, for the specified Auto Scaling group.
      operationId: resumeProcesses
      x-api-path-slug: actionresumeprocesses-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name or Amazon Resource Name (ARN) of the Auto Scaling group
        type: string
      - in: query
        name: ScalingProcesses.member.N
        description: One or more of the following processes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Processes
  /?Action=SetDesiredCapacity:
    get:
      summary: Set Desired Capacity
      description: Sets the size of the specified Auto Scaling group.
      operationId: setDesiredCapacity
      x-api-path-slug: actionsetdesiredcapacity-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: DesiredCapacity
        description: The number of EC2 instances that should be running in the Auto
          Scaling group
        type: string
      - in: query
        name: HonorCooldown
        description: By default, SetDesiredCapacity overrides any cooldown period
          associated with the Auto Scaling group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Desired Capacity
  /?Action=SetInstanceHealth:
    get:
      summary: Set Instance Health
      description: Sets the health status of the specified instance.
      operationId: setInstanceHealth
      x-api-path-slug: actionsetinstancehealth-get
      parameters:
      - in: query
        name: HealthStatus
        description: The health status of the instance
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: ShouldRespectGracePeriod
        description: If the Auto Scaling group of the specified instance has a HealthCheckGracePeriod             specified
          for the group, by default, this call will respect the grace period
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Health
  /?Action=SetInstanceProtection:
    get:
      summary: Set Instance Protection
      description: Updates the instance protection settings of the specified instances.
      operationId: setInstanceProtection
      x-api-path-slug: actionsetinstanceprotection-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: InstanceIds.member.N
        description: One or more instance IDs
        type: string
      - in: query
        name: ProtectedFromScaleIn
        description: Indicates whether the instance is protected from termination
          by Auto Scaling when scaling in
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Protection
  /?Action=SuspendProcesses:
    get:
      summary: Suspend Processes
      description: Suspends the specified Auto Scaling processes, or all processes,
        for the specified Auto Scaling group.
      operationId: suspendProcesses
      x-api-path-slug: actionsuspendprocesses-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name or Amazon Resource Name (ARN) of the Auto Scaling group
        type: string
      - in: query
        name: ScalingProcesses.member.N
        description: One or more of the following processes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Processes
  /?Action=TerminateInstanceInAutoScalingGroup:
    get:
      summary: Terminate Instance In Auto Scaling Group
      description: Terminates the specified instance and optionally adjusts the desired
        group size.
      operationId: terminateInstanceInAutoScalingGroup
      x-api-path-slug: actionterminateinstanceinautoscalinggroup-get
      parameters:
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: ShouldDecrementDesiredCapacity
        description: If true, terminating the instance also decrements the size of
          the Auto Scaling group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Auto Scaling
  /?Action=UpdateAutoScalingGroup:
    get:
      summary: Update Auto Scaling Group
      description: Updates the configuration for the specified Auto Scaling group.
      operationId: updateAutoScalingGroup
      x-api-path-slug: actionupdateautoscalinggroup-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: AvailabilityZones.member.N
        description: One or more Availability Zones for the group
        type: string
      - in: query
        name: DefaultCooldown
        description: The amount of time, in seconds, after a scaling activity completes
          before another scaling activity can start
        type: string
      - in: query
        name: DesiredCapacity
        description: The number of EC2 instances that should be running in the Auto
          Scaling group
        type: string
      - in: query
        name: HealthCheckGracePeriod
        description: The amount of time, in seconds, that Auto Scaling waits before
          checking the health status of an EC2 instance that has come into service
        type: string
      - in: query
        name: HealthCheckType
        description: The service to use for the health checks
        type: string
      - in: query
        name: LaunchConfigurationName
        description: The name of the launch configuration
        type: string
      - in: query
        name: MaxSize
        description: The maximum size of the Auto Scaling group
        type: string
      - in: query
        name: MinSize
        description: The minimum size of the Auto Scaling group
        type: string
      - in: query
        name: NewInstancesProtectedFromScaleIn
        description: Indicates whether newly launched instances are protected from
          termination by Auto Scaling when scaling in
        type: string
      - in: query
        name: PlacementGroup
        description: The name of the placement group into which youll launch your
          instances, if any
        type: string
      - in: query
        name: TerminationPolicies.member.N
        description: A standalone termination policy or a list of termination policies
          used to select the instance to terminate
        type: string
      - in: query
        name: VPCZoneIdentifier
        description: The ID of the subnet, if you are launching into a VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - Auto Scaling