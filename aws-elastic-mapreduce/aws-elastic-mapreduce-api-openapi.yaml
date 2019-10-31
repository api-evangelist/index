swagger: "2.0"
x-collection-name: AWS Elastic MapReduce
x-complete: 1
info:
  title: AWS Elastic MapReduce API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddInstanceGroups:
    get:
      summary: Add Instance Groups
      description: Adds one or more instance groups to a running cluster.
      operationId: addInstanceGroups
      x-api-path-slug: actionaddinstancegroups-get
      parameters:
      - in: query
        name: InstanceGroups
        description: Instance groups to add
        type: string
      - in: query
        name: JobFlowId
        description: Job flow in which to add the instance groups
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Groups
  /?Action=AddJobFlowSteps:
    get:
      summary: Add Job Flow Steps
      description: AddJobFlowSteps adds new steps to a running job flow.
      operationId: addJobFlowSteps
      x-api-path-slug: actionaddjobflowsteps-get
      parameters:
      - in: query
        name: JobFlowId
        description: A string that uniquely identifies the job flow
        type: string
      - in: query
        name: Steps
        description: A list of StepConfig to be executed by the job flow
        type: string
      responses:
        200:
          description: OK
      tags:
      - Job Flow Steps
  /?Action=AddTags:
    get:
      summary: Add Tags
      description: Adds tags to an Amazon EMR resource.
      operationId: addTags
      x-api-path-slug: actionaddtags-get
      parameters:
      - in: query
        name: ResourceId
        description: The Amazon EMR resource identifier to which tags will be added
        type: string
      - in: query
        name: Tags
        description: A list of tags to associate with a cluster and propagate to EC2
          instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=CancelSteps:
    get:
      summary: Cancel Steps
      description: Cancels a pending step or steps in a running cluster.
      operationId: cancelSteps
      x-api-path-slug: actioncancelsteps-get
      parameters:
      - in: query
        name: ClusterId
        description: The ClusterID for which specified steps will be canceled
        type: string
      - in: query
        name: StepIds
        description: The list of StepIDs to cancel
        type: string
      responses:
        200:
          description: OK
      tags:
      - Steps
  /?Action=CreateSecurityConfiguration:
    get:
      summary: Create Security Configuration
      description: Creates a security configuration, which is stored in the service
        and can be specified when a cluster is created.
      operationId: createSecurityConfiguration
      x-api-path-slug: actioncreatesecurityconfiguration-get
      parameters:
      - in: query
        name: Name
        description: The name of the security configuration
        type: string
      - in: query
        name: SecurityConfiguration
        description: The security configuration details in JSON format
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Configurations
  /?Action=DeleteSecurityConfiguration:
    get:
      summary: Delete Security Configuration
      description: Deletes a security configuration.
      operationId: deleteSecurityConfiguration
      x-api-path-slug: actiondeletesecurityconfiguration-get
      parameters:
      - in: query
        name: Name
        description: The name of the security configuration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Configurations
  /?Action=DescribeCluster:
    get:
      summary: Describe Cluster
      description: Provides cluster-level details including status, hardware and software
        configuration, VPC settings, and so on.
      operationId: describeCluster
      x-api-path-slug: actiondescribecluster-get
      parameters:
      - in: query
        name: ClusterId
        description: The identifier of the cluster to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DescribeJobFlows:
    get:
      summary: Describe Job Flows
      description: This API is deprecated and will eventually be removed.
      operationId: describeJobFlows
      x-api-path-slug: actiondescribejobflows-get
      parameters:
      - in: query
        name: CreatedAfter
        description: Return only job flows created after this date and time
        type: string
      - in: query
        name: CreatedBefore
        description: Return only job flows created before this date and time
        type: string
      - in: query
        name: JobFlowIds
        description: Return only job flows whose job flow ID is contained in this
          list
        type: string
      - in: query
        name: JobFlowStates
        description: Return only job flows whose state is contained in this list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Job Flows
  /?Action=DescribeSecurityConfiguration:
    get:
      summary: Describe Security Configuration
      description: Provides the details of a security configuration by returning the
        configuration JSON.
      operationId: describeSecurityConfiguration
      x-api-path-slug: actiondescribesecurityconfiguration-get
      parameters:
      - in: query
        name: Name
        description: The name of the security configuration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Configurations
  /?Action=DescribeStep:
    get:
      summary: Describe Step
      description: Provides more detail about the cluster step.
      operationId: describeStep
      x-api-path-slug: actiondescribestep-get
      parameters:
      - in: query
        name: ClusterId
        description: The identifier of the cluster with steps to describe
        type: string
      - in: query
        name: StepId
        description: The identifier of the step to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Steps
  /?Action=ListBootstrapActions:
    get:
      summary: List Bootstrap Actions
      description: Provides information about the bootstrap actions associated with
        a cluster.
      operationId: listBootstrapActions
      x-api-path-slug: actionlistbootstrapactions-get
      parameters:
      - in: query
        name: ClusterId
        description: The cluster identifier for the bootstrap actions to list
        type: string
      - in: query
        name: Marker
        description: The pagination token that indicates the next set of results to
          retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bootstrap Actions
  /?Action=ListClusters:
    get:
      summary: List Clusters
      description: Provides the status of all clusters visible to this AWS account.
      operationId: listClusters
      x-api-path-slug: actionlistclusters-get
      parameters:
      - in: query
        name: ClusterStates
        description: The cluster state filters to apply when listing clusters
        type: string
      - in: query
        name: CreatedAfter
        description: The creation date and time beginning value filter for listing
          clusters
        type: string
      - in: query
        name: CreatedBefore
        description: The creation date and time end value filter for listing clusters
        type: string
      - in: query
        name: Marker
        description: The pagination token that indicates the next set of results to
          retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=ListInstanceGroups:
    get:
      summary: List Instance Groups
      description: Provides all available details about the instance groups in a cluster.
      operationId: listInstanceGroups
      x-api-path-slug: actionlistinstancegroups-get
      parameters:
      - in: query
        name: ClusterId
        description: The identifier of the cluster for which to list the instance
          groups
        type: string
      - in: query
        name: Marker
        description: The pagination token that indicates the next set of results to
          retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Groups
  /?Action=ListInstances:
    get:
      summary: List Instances
      description: "Provides information about the cluster instances that Amazon EMR
        provisions on behalf of a user \n         when it creates the cluster."
      operationId: listInstances
      x-api-path-slug: actionlistinstances-get
      parameters:
      - in: query
        name: ClusterId
        description: The identifier of the cluster for which to list the instances
        type: string
      - in: query
        name: InstanceGroupId
        description: The identifier of the instance group for which to list the instances
        type: string
      - in: query
        name: InstanceGroupTypes
        description: The type of instance group for which to list the instances
        type: string
      - in: query
        name: InstanceStates
        description: A list of instance states that will filter the instances returned
          with this request
        type: string
      - in: query
        name: Marker
        description: The pagination token that indicates the next set of results to
          retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=ListSecurityConfigurations:
    get:
      summary: List Security Configurations
      description: Lists all the security configurations visible to this account,
        providing their creation dates and times, and their names.
      operationId: listSecurityConfigurations
      x-api-path-slug: actionlistsecurityconfigurations-get
      parameters:
      - in: query
        name: Marker
        description: The pagination token that indicates the set of results to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Configurations
  /?Action=ListSteps:
    get:
      summary: List Steps
      description: Provides a list of steps for the cluster in reverse order unless
        you specify stepIds with the request.
      operationId: listSteps
      x-api-path-slug: actionliststeps-get
      parameters:
      - in: query
        name: ClusterId
        description: The identifier of the cluster for which to list the steps
        type: string
      - in: query
        name: Marker
        description: The pagination token that indicates the next set of results to
          retrieve
        type: string
      - in: query
        name: StepIds
        description: The filter to limit the step list based on the identifier of
          the steps
        type: string
      - in: query
        name: StepStates
        description: The filter to limit the step list based on certain states
        type: string
      responses:
        200:
          description: OK
      tags:
      - Steps
  /?Action=ModifyInstanceGroups:
    get:
      summary: Modify Instance Groups
      description: ModifyInstanceGroups modifies the number of nodes and configuration
        settings of an instance group.
      operationId: modifyInstanceGroups
      x-api-path-slug: actionmodifyinstancegroups-get
      parameters:
      - in: query
        name: ClusterId
        description: The ID of the cluster to which the instance group belongs
        type: string
      - in: query
        name: InstanceGroups
        description: Instance groups to change
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Groups
  /?Action=PutAutoScalingPolicy:
    get:
      summary: Put Auto Scaling Policy
      description: Creates or updates an automatic scaling policy for a core instance
        group or task instance group in an Amazon EMR cluster.
      operationId: putAutoScalingPolicy
      x-api-path-slug: actionputautoscalingpolicy-get
      parameters:
      - in: query
        name: AutoScalingPolicy
        description: Specifies the definition of the automatic scaling policy
        type: string
      - in: query
        name: ClusterId
        description: Specifies the ID of a cluster
        type: string
      - in: query
        name: InstanceGroupId
        description: Specifies the ID of the instance group to which the automatic
          scaling policy is applied
        type: string
      responses:
        200:
          description: OK
      tags:
      - Auto Scaling Policies
  /?Action=RemoveAutoScalingPolicy:
    get:
      summary: Remove Auto Scaling Policy
      description: Removes an automatic scaling policy from a specified instance group
        within an EMR cluster.
      operationId: removeAutoScalingPolicy
      x-api-path-slug: actionremoveautoscalingpolicy-get
      parameters:
      - in: query
        name: ClusterId
        description: Specifies the ID of a cluster
        type: string
      - in: query
        name: InstanceGroupId
        description: Specifies the ID of the instance group to which the scaling policy
          is applied
        type: string
      responses:
        200:
          description: OK
      tags:
      - Auto Scaling Policies
  /?Action=RemoveTags:
    get:
      summary: Remove Tags
      description: Removes tags from an Amazon EMR resource.
      operationId: removeTags
      x-api-path-slug: actionremovetags-get
      parameters:
      - in: query
        name: ResourceId
        description: The Amazon EMR resource identifier from which tags will be removed
        type: string
      - in: query
        name: TagKeys
        description: A list of tag keys to remove from a resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=RunJobFlow:
    get:
      summary: Run Job Flow
      description: RunJobFlow creates and starts running a new job flow.
      operationId: runJobFlow
      x-api-path-slug: actionrunjobflow-get
      parameters:
      - in: query
        name: AdditionalInfo
        description: A JSON string for selecting additional features
        type: string
      - in: query
        name: AmiVersion
        description: Note
        type: string
      - in: query
        name: Applications
        description: Note
        type: string
      - in: query
        name: AutoScalingRole
        description: An IAM role for automatic scaling policies
        type: string
      - in: query
        name: BootstrapActions
        description: A list of bootstrap actions that will be run before Hadoop is
          started on the cluster nodes
        type: string
      - in: query
        name: Configurations
        description: Note
        type: string
      - in: query
        name: Instances
        description: A specification of the number and type of Amazon EC2 instances
          on which to run the job flow
        type: string
      - in: query
        name: JobFlowRole
        description: Also called instance profile and EC2 role
        type: string
      - in: query
        name: LogUri
        description: The location in Amazon S3 to write the log files of the job flow
        type: string
      - in: query
        name: Name
        description: The name of the job flow
        type: string
      - in: query
        name: NewSupportedProducts
        description: Note
        type: string
      - in: query
        name: ReleaseLabel
        description: Note
        type: string
      - in: query
        name: ScaleDownBehavior
        description: Specifies the way that individual Amazon EC2 instances terminate
          when an automatic scale-in activity occurs or an instance group is resized
        type: string
      - in: query
        name: SecurityConfiguration
        description: The name of a security configuration to apply to the cluster
        type: string
      - in: query
        name: ServiceRole
        description: The IAM role that will be assumed by the Amazon EMR service to
          access AWS resources on your behalf
        type: string
      - in: query
        name: Steps
        description: A list of steps to be executed by the job flow
        type: string
      - in: query
        name: SupportedProducts
        description: Note
        type: string
      - in: query
        name: Tags
        description: A list of tags to associate with a cluster and propagate to Amazon
          EC2 instances
        type: string
      - in: query
        name: VisibleToAllUsers
        description: Whether the job flow is visible to all IAM users of the AWS account
          associated with the job flow
        type: string
      responses:
        200:
          description: OK
      tags:
      - Job Flows
  /?Action=SetTerminationProtection:
    get:
      summary: Set Termination Protection
      description: SetTerminationProtection locks a job flow so the EC2 instances
        in the cluster cannot be terminated by user intervention, an API call, or
        in the event of a job-flow error.
      operationId: setTerminationProtection
      x-api-path-slug: actionsetterminationprotection-get
      parameters:
      - in: query
        name: JobFlowIds
        description: A list of strings that uniquely identify the job flows to protect
        type: string
      - in: query
        name: TerminationProtected
        description: A Boolean that indicates whether to protect the job flow and
          prevent the Amazon EC2 instances in the cluster from shutting down due to
          API calls, user intervention, or job-flow error
        type: string
      responses:
        200:
          description: OK
      tags:
      - Termination Protection
  /?Action=SetVisibleToAllUsers:
    get:
      summary: Set Visible To All Users
      description: Sets whether all AWS Identity and Access Management (IAM) users
        under your account can access the specified job flows.
      operationId: setVisibleToAllUsers
      x-api-path-slug: actionsetvisibletoallusers-get
      parameters:
      - in: query
        name: JobFlowIds
        description: Identifiers of the job flows to receive the new visibility setting
        type: string
      - in: query
        name: VisibleToAllUsers
        description: Whether the specified job flows are visible to all IAM users
          of the AWS account associated with the job flow
        type: string
      responses:
        200:
          description: OK
      tags:
      - Visible To All Users
  /?Action=TerminateJobFlows:
    get:
      summary: Terminate Job Flows
      description: TerminateJobFlows shuts a list of job flows down.
      operationId: terminateJobFlows
      x-api-path-slug: actionterminatejobflows-get
      parameters:
      - in: query
        name: JobFlowIds
        description: A list of job flows to be shutdown
        type: string
      responses:
        200:
          description: OK
      tags:
      - Job Flows