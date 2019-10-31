swagger: "2.0"
x-collection-name: AWS Code Pipeline
x-complete: 1
info:
  title: AWS Code Pipeline API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AcknowledgeJob:
    get:
      summary: Acknowledge Job
      description: |-
        Returns information about a specified job and whether that job has been received by
                    the job worker.
      operationId: acknowledgeJob
      x-api-path-slug: actionacknowledgejob-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: jobId
        description: The unique system-generated ID of the job for which you want
          to confirm            receipt
        type: string
      - in: query
        name: nonce
        description: A system-generated random number that AWS CodePipeline uses to
          ensure that the job            is being worked on by only one job worker
        type: string
      - in: query
        name: SnapshotId
        description: The ID of the EBS snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Acknowledge
      - Job
  /?Action=AcknowledgeThirdPartyJob:
    get:
      summary: Acknowledge Third Party Job
      description: Confirms a job worker has received the specified job.
      operationId: acknowledgeThirdPartyJob
      x-api-path-slug: actionacknowledgethirdpartyjob-get
      parameters:
      - in: query
        name: clientToken
        description: The clientToken portion of the clientId and clientToken pair
          used to verify that            the calling entity is allowed access to the
          job and its details
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: jobId
        description: The unique system-generated ID of the job
        type: string
      - in: query
        name: nonce
        description: A system-generated random number that AWS CodePipeline uses to
          ensure that the job            is being worked on by only one job worker
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Acknowledge
      - Third
      - Party
      - Job
  /?Action=CreateCustomActionType:
    get:
      summary: Create Custom Action Type
      description: |-
        Creates a new custom action that can be used in all pipelines associated with the
                    AWS account.
      operationId: createCustomActionType
      x-api-path-slug: actioncreatecustomactiontype-get
      parameters:
      - in: query
        name: Attribute
        description: The snapshot attribute you would like to view
        type: string
      - in: query
        name: category
        description: The category of the custom action, such as a build action or
          a test            action
        type: string
      - in: query
        name: configurationProperties
        description: The configuration properties for the custom action
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: inputArtifactDetails
        description: Returns information about the details of an artifact
        type: string
      - in: query
        name: outputArtifactDetails
        description: Returns information about the details of an artifact
        type: string
      - in: query
        name: provider
        description: The provider of the service used in the custom action, such as
          AWS            CodeDeploy
        type: string
      - in: query
        name: settings
        description: Returns information about the settings for an action type
        type: string
      - in: query
        name: SnapshotId
        description: The ID of the EBS snapshot
        type: string
      - in: query
        name: version
        description: The version identifier of the custom action
        type: string
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Action
      - Type
  /?Action=CreatePipeline:
    get:
      summary: Create Pipeline
      description: Creates a pipeline.
      operationId: createPipeline
      x-api-path-slug: actioncreatepipeline-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of snapshot results returned by DescribeSnapshots
          in      paginated output
        type: string
      - in: query
        name: NextToken
        description: The NextToken value returned from a previous paginated        DescribeSnapshots
          request where MaxResults was used and the      results exceeded the value
          of that parameter
        type: string
      - in: query
        name: Owner.N
        description: Returns the snapshots owned by the specified owner
        type: string
      - in: query
        name: pipeline
        description: Represents the structure of actions and stages to be performed
          in the            pipeline
        type: string
      - in: query
        name: RestorableBy.N
        description: One or more AWS accounts IDs that can create volumes from the
          snapshot
        type: string
      - in: query
        name: SnapshotId.N
        description: One or more snapshot IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=DeleteCustomActionType:
    get:
      summary: Delete Custom Action Type
      description: Marks a custom action as deleted.
      operationId: deleteCustomActionType
      x-api-path-slug: actiondeletecustomactiontype-get
      parameters:
      - in: query
        name: Attribute
        description: The instance attribute
        type: string
      - in: query
        name: category
        description: The category of the custom action that you want to delete, such
          as source or            deploy
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: provider
        description: The provider of the service used in the custom action, such as
          AWS            CodeDeploy
        type: string
      - in: query
        name: version
        description: The version of the custom action to delete
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Action
      - Type
  /?Action=DeletePipeline:
    get:
      summary: Delete Pipeline
      description: Deletes the specified pipeline.
      operationId: deletePipeline
      x-api-path-slug: actiondeletepipeline-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of volume results returned by DescribeVolumes
          in paginated      output
        type: string
      - in: query
        name: name
        description: The name of the pipeline to be deleted
        type: string
      - in: query
        name: NextToken
        description: The NextToken value returned from a previous paginated        DescribeVolumes
          request where MaxResults was used and the results      exceeded the value
          of that parameter
        type: string
      - in: query
        name: VolumeId.N
        description: One or more volume IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=DisableStageTransition:
    get:
      summary: Disable Stage Transition
      description: |-
        Prevents artifacts in a pipeline from transitioning to the next stage in the
                    pipeline.
      operationId: disableStageTransition
      x-api-path-slug: actiondisablestagetransition-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of volume results returned by DescribeVolumeStatus
          in      paginated output
        type: string
      - in: query
        name: NextToken
        description: The NextToken value to include in a future DescribeVolumeStatus      request
        type: string
      - in: query
        name: pipelineName
        description: The name of the pipeline in which you want to disable the flow
          of artifacts from            one stage to another
        type: string
      - in: query
        name: reason
        description: The reason given to the user why a stage is disabled, such as
          waiting for manual            approval or manual tests
        type: string
      - in: query
        name: stageName
        description: The name of the stage where you want to disable the inbound or
          outbound transition            of artifacts
        type: string
      - in: query
        name: transitionType
        description: Specifies whether artifacts will be prevented from transitioning
          into the stage and            being processed by the actions in that stage
          (inbound), or prevented from transitioning            from the stage after
          they have been processed by the actions in that stage            (outbound)
        type: string
      - in: query
        name: VolumeId.N
        description: One or more volume IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Disable
      - Stage
      - Transition
  /?Action=EnableStageTransition:
    get:
      summary: Enable Stage Transition
      description: Enables artifacts in a pipeline to transition to a stage in a pipeline.
      operationId: enableStageTransition
      x-api-path-slug: actionenablestagetransition-get
      parameters:
      - in: query
        name: Device
        description: The device name
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Force
        description: Forces detachment if the previous detachment attempt did not
          occur cleanly (for example,      logging into an instance, unmounting the
          volume, and detaching normally)
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: pipelineName
        description: The name of the pipeline in which you want to enable the flow
          of artifacts from one            stage to another
        type: string
      - in: query
        name: stageName
        description: The name of the stage where you want to enable the transition
          of artifacts, either            into the stage (inbound) or from that stage
          to the next stage (outbound)
        type: string
      - in: query
        name: transitionType
        description: Specifies whether artifacts will be allowed to enter the stage
          and be processed by            the actions in that stage (inbound) or whether
          already-processed artifacts will be            allowed to transition to
          the next stage (outbound)
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Enable
      - Stage
      - Transition
  /?Action=GetJobDetails:
    get:
      summary: Get Job Details
      description: Returns information about a job.
      operationId: getJobDetails
      x-api-path-slug: actiongetjobdetails-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: jobId
        description: The unique system-generated ID for the job
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Job
      - Details
  /?Action=GetPipeline:
    get:
      summary: Get Pipeline
      description: Returns the metadata, structure, stages, and actions of a pipeline.
      operationId: getPipeline
      x-api-path-slug: actiongetpipeline-get
      parameters:
      - in: query
        name: Attribute
        description: The snapshot attribute to modify
        type: string
      - in: query
        name: CreateVolumePermission
        description: A JSON representation of the snapshot attribute modification
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: name
        description: The name of the pipeline for which you want to get information
        type: string
      - in: query
        name: OperationType
        description: The type of operation to perform to the attribute
        type: string
      - in: query
        name: SnapshotId
        description: The ID of the snapshot
        type: string
      - in: query
        name: UserGroup.N
        description: The group to modify for the snapshot
        type: string
      - in: query
        name: UserId.N
        description: The account ID to modify for the snapshot
        type: string
      - in: query
        name: version
        description: The version number of the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=GetPipelineExecution:
    get:
      summary: Get Pipeline Execution
      description: |-
        Returns information about an execution of a pipeline, including details about
                    artifacts, the pipeline execution ID, and the name, version, and status of the
                    pipeline.
      operationId: getPipelineExecution
      x-api-path-slug: actiongetpipelineexecution-get
      parameters:
      - in: query
        name: AutoEnableIO
        description: Indicates whether the volume should be auto-enabled for I/O operations
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: pipelineExecutionId
        description: The ID of the pipeline execution about which you want to get
          execution            details
        type: string
      - in: query
        name: pipelineName
        description: The name of the pipeline about which you want to get execution
          details
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
      - Execution
  /?Action=GetPipelineState:
    get:
      summary: Get Pipeline State
      description: |-
        Returns information about the state of a pipeline, including the stages and
                    actions.
      operationId: getPipelineState
      x-api-path-slug: actiongetpipelinestate-get
      parameters:
      - in: query
        name: Attribute
        description: The attribute to reset
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: name
        description: The name of the pipeline about which you want to get information
        type: string
      - in: query
        name: SnapshotId
        description: The ID of the snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
      - State
  /?Action=GetThirdPartyJobDetails:
    get:
      summary: Get Third Party Job Details
      description: Requests the details of a job for a third party action.
      operationId: getThirdPartyJobDetails
      x-api-path-slug: actiongetthirdpartyjobdetails-get
      parameters:
      - in: query
        name: clientToken
        description: The clientToken portion of the clientId and clientToken pair
          used to verify that            the calling entity is allowed access to the
          job and its details
        type: string
      - in: query
        name: Domain
        description: Set to vpc to allocate the address for use with instances in
          a VPC
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: jobId
        description: The unique system-generated ID used for identifying the job
        type: string
      responses:
        200:
          description: OK
      tags:
      - Third
      - Party
      - Job
      - Details
  /?Action=ListActionTypes:
    get:
      summary: List Action Types
      description: |-
        Gets a summary of all AWS CodePipeline action types associated with your
                    account.
      operationId: listActionTypes
      x-api-path-slug: actionlistactiontypes-get
      parameters:
      - in: query
        name: actionOwnerFilter
        description: Filters the list of action types to those created by a specified
          entity
        type: string
      - in: query
        name: AllocationId
        description: '[EC2-VPC] The allocation ID'
        type: string
      - in: query
        name: AllowReassociation
        description: '[EC2-VPC] For a VPC in an EC2-Classic account, specify true
          to allow an Elastic IP address that is already associated with an instance
          or network interface to be reassociated with the specified instance or network
          interface'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: NetworkInterfaceId
        description: '[EC2-VPC] The ID of the network interface'
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous list action
          types call, which can            be used to return the next set of action
          types in the list
        type: string
      - in: query
        name: PrivateIpAddress
        description: '[EC2-VPC] The primary or secondary private IP address to associate
          with the Elastic IP address'
        type: string
      - in: query
        name: PublicIp
        description: The Elastic IP address
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Action
      - Types
  /?Action=ListPipelines:
    get:
      summary: List Pipelines
      description: Gets a summary of all of the pipelines associated with your account.
      operationId: listPipelines
      x-api-path-slug: actionlistpipelines-get
      parameters:
      - in: query
        name: AllocationId.N
        description: '[EC2-VPC] One or more allocation IDs'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous list pipelines
          call, which can be            used to return the next set of pipelines in
          the list
        type: string
      - in: query
        name: PublicIp.N
        description: '[EC2-Classic] One or more Elastic IP addresses'
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Pipelines
  /?Action=PollForJobs:
    get:
      summary: Poll For Jobs
      description: Returns information about any jobs for AWS CodePipeline to act
        upon.
      operationId: pollForJobs
      x-api-path-slug: actionpollforjobs-get
      parameters:
      - in: query
        name: actionTypeId
        description: Represents information about an action type
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: maxBatchSize
        description: The maximum number of jobs to return in a poll for jobs call
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return for the request in a
          single page
        type: string
      - in: query
        name: NextToken
        description: The token to use to retrieve the next page of results
        type: string
      - in: query
        name: PublicIp.N
        description: One or more Elastic IP addresses
        type: string
      - in: query
        name: queryParam
        description: A map of property names and values
        type: string
      responses:
        200:
          description: OK
      tags:
      - PollJobs
  /?Action=PollForThirdPartyJobs:
    get:
      summary: Poll For Third Party Jobs
      description: Determines whether there are any third party jobs for a job worker
        to act on.
      operationId: pollForThirdPartyJobs
      x-api-path-slug: actionpollforthirdpartyjobs-get
      parameters:
      - in: query
        name: actionTypeId
        description: Represents information about an action type
        type: string
      - in: query
        name: AssociationId
        description: '[EC2-VPC] The association ID'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: maxBatchSize
        description: The maximum number of jobs to return in a poll for jobs call
        type: string
      - in: query
        name: PublicIp
        description: '[EC2-Classic] The Elastic IP address'
        type: string
      responses:
        200:
          description: OK
      tags:
      - PollThird
      - Party
      - Jobs
  /?Action=PutActionRevision:
    get:
      summary: Put Action Revision
      description: Provides information to AWS CodePipeline about new revisions to
        a source.
      operationId: putActionRevision
      x-api-path-slug: actionputactionrevision-get
      parameters:
      - in: query
        name: actionName
        description: The name of the action that will process the revision
        type: string
      - in: query
        name: actionRevision
        description: Represents information about the version (or revision) of an
          action
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: pipelineName
        description: The name of the pipeline that will start processing the revision
          to the            source
        type: string
      - in: query
        name: PublicIp
        description: The Elastic IP address
        type: string
      - in: query
        name: stageName
        description: The name of the stage that contains the action that will act
          upon the            revision
        type: string
      responses:
        200:
          description: OK
      tags:
      - Put
      - Action
      - Revision
  /?Action=PutApprovalResult:
    get:
      summary: Put Approval Result
      description: Provides the response to a manual approval request to AWS CodePipeline.
      operationId: putApprovalResult
      x-api-path-slug: actionputapprovalresult-get
      parameters:
      - in: query
        name: actionName
        description: The name of the action for which approval is requested
        type: string
      - in: query
        name: AllocationId
        description: '[EC2-VPC] The allocation ID'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: pipelineName
        description: The name of the pipeline that contains the action
        type: string
      - in: query
        name: PublicIp
        description: '[EC2-Classic] The Elastic IP address'
        type: string
      - in: query
        name: result
        description: Represents information about the result of the approval request
        type: string
      - in: query
        name: stageName
        description: The name of the stage that contains the action
        type: string
      - in: query
        name: token
        description: The system-generated token used to identify a unique approval
          request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Put
      - Approval
      - Result
  /?Action=PutJobFailureResult:
    get:
      summary: Put Job Failure Result
      description: Represents the failure of a job as returned to the pipeline by
        a job worker.
      operationId: putJobFailureResult
      x-api-path-slug: actionputjobfailureresult-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: failureDetails
        description: The details about the failure of a job
        type: string
      - in: query
        name: jobId
        description: The unique system-generated ID of the job that failed
        type: string
      - in: query
        name: PublicIp
        description: The Elastic IP address
        type: string
      responses:
        200:
          description: OK
      tags:
      - Put
      - Job
      - Failure
      - Result
  /?Action=PutJobSuccessResult:
    get:
      summary: Put Job Success Result
      description: Represents the success of a job as returned to the pipeline by
        a job worker.
      operationId: putJobSuccessResult
      x-api-path-slug: actionputjobsuccessresult-get
      parameters:
      - in: query
        name: continuationToken
        description: A token generated by a job worker, such as an AWS CodeDeploy
          deployment ID, that a            successful job provides to identify a custom
          action in progress
        type: string
      - in: query
        name: currentRevision
        description: The ID of the current revision of the artifact successfully worked
          upon by the            job
        type: string
      - in: query
        name: executionDetails
        description: The execution details of the successful job, such as the actions
          taken by the job            worker
        type: string
      - in: query
        name: Ipv6AddressCount
        description: The number of IPv6 addresses to assign to the network interface
        type: string
      - in: query
        name: Ipv6Addresses.N
        description: One or more specific IPv6 addresses to be assigned to the network
          interface
        type: string
      - in: query
        name: jobId
        description: The unique system-generated ID of the job that succeeded
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      responses:
        200:
          description: OK
      tags:
      - Put
      - Job
      - Success
      - Result
  /?Action=PutThirdPartyJobFailureResult:
    get:
      summary: Put Third Party Job Failure Result
      description: |-
        Represents the failure of a third party job as returned to the pipeline by a job
                    worker.
      operationId: putThirdPartyJobFailureResult
      x-api-path-slug: actionputthirdpartyjobfailureresult-get
      parameters:
      - in: query
        name: AllowReassignment
        description: Indicates whether to allow an IP address that is already assigned
          to another network interface or instance to be reassigned to the specified
          network interface
        type: string
      - in: query
        name: clientToken
        description: The clientToken portion of the clientId and clientToken pair
          used to verify that            the calling entity is allowed access to the
          job and its details
        type: string
      - in: query
        name: failureDetails
        description: Represents information about failure details
        type: string
      - in: query
        name: jobId
        description: The ID of the job that failed
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      - in: query
        name: PrivateIpAddress.N
        description: One or more IP addresses to be assigned as a secondary private
          IP address to the network interface
        type: string
      - in: query
        name: SecondaryPrivateIpAddressCount
        description: The number of secondary IP addresses to assign to the network
          interface
        type: string
      responses:
        200:
          description: OK
      tags:
      - Put
      - Third
      - Party
      - Job
      - Failure
      - Result
  /?Action=PutThirdPartyJobSuccessResult:
    get:
      summary: Put Third Party Job Success Result
      description: |-
        Represents the success of a third party job as returned to the pipeline by a job
                    worker.
      operationId: putThirdPartyJobSuccessResult
      x-api-path-slug: actionputthirdpartyjobsuccessresult-get
      parameters:
      - in: query
        name: clientToken
        description: The clientToken portion of the clientId and clientToken pair
          used to verify that            the calling entity is allowed access to the
          job and its details
        type: string
      - in: query
        name: continuationToken
        description: A token generated by a job worker, such as an AWS CodeDeploy
          deployment ID, that a            successful job provides to identify a partner
          action in progress
        type: string
      - in: query
        name: currentRevision
        description: Represents information about a current revision
        type: string
      - in: query
        name: DeviceIndex
        description: The index of the device for the network interface attachment
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: executionDetails
        description: The details of the actions taken and results produced on an artifact
          as it passes            through stages in the pipeline
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: jobId
        description: The ID of the job that successfully completed
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      responses:
        200:
          description: OK
      tags:
      - Put
      - Third
      - Party
      - Job
      - Success
      - Result
  /?Action=RetryStageExecution:
    get:
      summary: Retry Stage Execution
      description: |-
        Resumes the pipeline execution by retrying the last failed actions in a
                    stage.
      operationId: retryStageExecution
      x-api-path-slug: actionretrystageexecution-get
      parameters:
      - in: query
        name: Description
        description: A description for the network interface
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Ipv6AddressCount
        description: The number of IPv6 addresses to assign to a network interface
        type: string
      - in: query
        name: Ipv6Addresses.N
        description: One or more specific IPv6 addresses from the IPv6 CIDR block
          range of your subnet
        type: string
      - in: query
        name: pipelineExecutionId
        description: The ID of the pipeline execution in the failed stage to be retried
        type: string
      - in: query
        name: pipelineName
        description: The name of the pipeline that contains the failed stage
        type: string
      - in: query
        name: PrivateIpAddress
        description: The primary private IPv4 address of the network interface
        type: string
      - in: query
        name: PrivateIpAddresses.N
        description: One or more private IPv4 addresses
        type: string
      - in: query
        name: retryMode
        description: The scope of the retry attempt
        type: string
      - in: query
        name: SecondaryPrivateIpAddressCount
        description: The number of secondary private IPv4 addresses to assign to a
          network interface
        type: string
      - in: query
        name: SecurityGroupId.N
        description: The IDs of one or more security groups
        type: string
      - in: query
        name: stageName
        description: The name of the failed stage to be retried
        type: string
      - in: query
        name: SubnetId
        description: The ID of the subnet to associate with the network interface
        type: string
      responses:
        200:
          description: OK
      tags:
      - Retry
      - Stage
      - Execution
  /?Action=StartPipelineExecution:
    get:
      summary: Start Pipeline Execution
      description: Starts the specified pipeline.
      operationId: startPipelineExecution
      x-api-path-slug: actionstartpipelineexecution-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: name
        description: The name of the pipeline to start
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      responses:
        200:
          description: OK
      tags:
      - Start
      - Pipeline
      - Execution
  /?Action=UpdatePipeline:
    get:
      summary: Update Pipeline
      description: Updates a specified pipeline with edits or changes to its structure.
      operationId: updatePipeline
      x-api-path-slug: actionupdatepipeline-get
      parameters:
      - in: query
        name: Attribute
        description: The attribute of the network interface
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      - in: query
        name: pipeline
        description: The name of the pipeline to be updated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline