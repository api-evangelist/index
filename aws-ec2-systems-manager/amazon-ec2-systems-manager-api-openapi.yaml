swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 1
info:
  title: AWS EC2 Systems Manager API
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
      description: Adds or overwrites one or more tags for the specified resource.
      operationId: addTagsToResource
      x-api-path-slug: actionaddtagstoresource-get
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID you want to tag
        type: string
      - in: query
        name: ResourceType
        description: Specifies the type of resource you are tagging
        type: string
      - in: query
        name: Tags
        description: One or more tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resources
  /?Action=CancelCommand:
    get:
      summary: Cancel Command
      description: Attempts to cancel the command specified by the Command ID.
      operationId: cancelCommand
      x-api-path-slug: actioncancelcommand-get
      parameters:
      - in: query
        name: CommandId
        description: The ID of the command you want to cancel
        type: string
      - in: query
        name: InstanceIds
        description: (Optional) A list of instance IDs on which you want to cancel
          the command
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Command
  /?Action=CreateActivation:
    get:
      summary: Create Activation
      description: |-
        Registers your on-premises server or virtual machine with Amazon EC2 so that you can manage
           these resources using Run Command.
      operationId: createActivation
      x-api-path-slug: actioncreateactivation-get
      parameters:
      - in: query
        name: DefaultInstanceName
        description: The name of the registered, managed instance as it will appear
          in the Amazon EC2 console or   when you use the AWS command line tools to
          list EC2 resources
        type: string
      - in: query
        name: Description
        description: A user-defined description of the resource that you want to register
          with Amazon EC2
        type: string
      - in: query
        name: ExpirationDate
        description: The date by which this activation request should expire
        type: string
      - in: query
        name: IamRole
        description: The Amazon Identity and Access Management (IAM) role that you
          want to assign to the   managed instance
        type: string
      - in: query
        name: RegistrationLimit
        description: Specify the maximum number of managed instances you want to register
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activation
  /?Action=CreateAssociation:
    get:
      summary: Create Association
      description: Associates the specified SSM document with the specified instances
        or targets.
      operationId: createAssociation
      x-api-path-slug: actioncreateassociation-get
      parameters:
      - in: query
        name: DocumentVersion
        description: The document version you want to associate with the target(s)
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      - in: query
        name: Name
        description: The name of the SSM document
        type: string
      - in: query
        name: OutputLocation
        description: An Amazon S3 bucket where you want to store the output details
          of the request
        type: string
      - in: query
        name: Parameters
        description: The parameters for the documents runtime configuration
        type: string
      - in: query
        name: ScheduleExpression
        description: A cron expression when the association will be applied to the
          target(s)
        type: string
      - in: query
        name: Targets
        description: The targets (either instances or tags) for the association
        type: string
      responses:
        200:
          description: OK
      tags:
      - Association
  /?Action=CreateAssociationBatch:
    get:
      summary: Create Association Batch
      description: Associates the specified SSM document with the specified instances
        or targets.
      operationId: createAssociationBatch
      x-api-path-slug: actioncreateassociationbatch-get
      parameters:
      - in: query
        name: Entries
        description: One or more associations
        type: string
      responses:
        200:
          description: OK
      tags:
      - Association
      - Batch
  /?Action=CreateDocument:
    get:
      summary: Create Document
      description: Creates an SSM document.
      operationId: createDocument
      x-api-path-slug: actioncreatedocument-get
      parameters:
      - in: query
        name: Content
        description: A valid JSON string
        type: string
      - in: query
        name: DocumentType
        description: The type of document to create
        type: string
      - in: query
        name: Name
        description: A name for the SSM document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Document
  /?Action=CreateMaintenanceWindow:
    get:
      summary: Create Maintenance Window
      description: Creates a new Maintenance Window.
      operationId: createMaintenanceWindow
      x-api-path-slug: actioncreatemaintenancewindow-get
      parameters:
      - in: query
        name: AllowUnassociatedTargets
        description: Whether targets must be registered with the Maintenance Window
          before tasks can be   defined for those targets
        type: string
      - in: query
        name: ClientToken
        description: User-provided idempotency token
        type: string
      - in: query
        name: Cutoff
        description: The number of hours before the end of the Maintenance Window
          that Systems Manager stops   scheduling new tasks for execution
        type: string
      - in: query
        name: Duration
        description: The duration of the Maintenance Window in hours
        type: string
      - in: query
        name: Name
        description: The name of the Maintenance Window
        type: string
      - in: query
        name: Schedule
        description: The schedule of the Maintenance Window in the form of a cron
          or rate   expression
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Window
  /?Action=CreatePatchBaseline:
    get:
      summary: Create Patch Baseline
      description: Creates a patch baseline.
      operationId: createPatchBaseline
      x-api-path-slug: actioncreatepatchbaseline-get
      parameters:
      - in: query
        name: ApprovalRules
        description: A set of rules used to include patches in the baseline
        type: string
      - in: query
        name: ApprovedPatches
        description: A list of explicitly approved patches for the baseline
        type: string
      - in: query
        name: ClientToken
        description: Caller-provided idempotency token
        type: string
      - in: query
        name: Description
        description: A description of the patch baseline
        type: string
      - in: query
        name: GlobalFilters
        description: A set of global filters used to exclude patches from the baseline
        type: string
      - in: query
        name: Name
        description: The name of the patch baseline
        type: string
      - in: query
        name: RejectedPatches
        description: A list of explicitly rejected patches for the baseline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Baseline
  /?Action=DeleteActivation:
    get:
      summary: Delete Activation
      description: Deletes an activation.
      operationId: deleteActivation
      x-api-path-slug: actiondeleteactivation-get
      parameters:
      - in: query
        name: ActivationId
        description: The ID of the activation that you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activation
  /?Action=DeleteAssociation:
    get:
      summary: Delete Association
      description: Disassociates the specified SSM document from the specified instance.
      operationId: deleteAssociation
      x-api-path-slug: actiondeleteassociation-get
      parameters:
      - in: query
        name: AssociationId
        description: The association ID that you want to delete
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: Name
        description: The name of the SSM document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Association
  /?Action=DeleteDocument:
    get:
      summary: Delete Document
      description: Deletes the SSM document and all instance associations to the document.
      operationId: deleteDocument
      x-api-path-slug: actiondeletedocument-get
      parameters:
      - in: query
        name: Name
        description: The name of the SSM document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Document
  /?Action=DeleteMaintenanceWindow:
    get:
      summary: Delete Maintenance Window
      description: Deletes a Maintenance Window.
      operationId: deleteMaintenanceWindow
      x-api-path-slug: actiondeletemaintenancewindow-get
      parameters:
      - in: query
        name: WindowId
        description: The ID of the Maintenance Window to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Window
  /?Action=DeleteParameter:
    get:
      summary: Delete Parameter
      description: Delete a parameter from the system.
      operationId: deleteParameter
      x-api-path-slug: actiondeleteparameter-get
      parameters:
      - in: query
        name: Name
        description: The name of the parameter to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter
  /?Action=DeletePatchBaseline:
    get:
      summary: Delete Patch Baseline
      description: Deletes a patch baseline.
      operationId: deletePatchBaseline
      x-api-path-slug: actiondeletepatchbaseline-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Baseline
  /?Action=DeregisterManagedInstance:
    get:
      summary: Deregister Managed Instance
      description: Removes the server or virtual machine from the list of registered
        servers.
      operationId: deregisterManagedInstance
      x-api-path-slug: actionderegistermanagedinstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The ID assigned to the managed instance when you registered it
          using the activation   process
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Managed
      - Instance
  /?Action=DeregisterPatchBaselineForPatchGroup:
    get:
      summary: Deregister Patch Baseline For Patch Group
      description: Removes a patch group from a patch baseline.
      operationId: deregisterPatchBaselineForPatchGroup
      x-api-path-slug: actionderegisterpatchbaselineforpatchgroup-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline to deregister the patch group from
        type: string
      - in: query
        name: PatchGroup
        description: The name of the patch group that should be deregistered from
          the patch baseline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - BaselineGroup
  /?Action=DeregisterTargetFromMaintenanceWindow:
    get:
      summary: Deregister Target From Maintenance Window
      description: Removes a target from a Maintenance Window.
      operationId: deregisterTargetFromMaintenanceWindow
      x-api-path-slug: actionderegistertargetfrommaintenancewindow-get
      parameters:
      - in: query
        name: WindowId
        description: The ID of the Maintenance Window the target should be removed
          from
        type: string
      - in: query
        name: WindowTargetId
        description: The ID of the target definition to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Target
      - From
      - Maintenance
      - Window
  /?Action=DeregisterTaskFromMaintenanceWindow:
    get:
      summary: Deregister Task From Maintenance Window
      description: Removes a task from a Maintenance Window.
      operationId: deregisterTaskFromMaintenanceWindow
      x-api-path-slug: actionderegistertaskfrommaintenancewindow-get
      parameters:
      - in: query
        name: WindowId
        description: The ID of the Maintenance Window the task should be removed from
        type: string
      - in: query
        name: WindowTaskId
        description: The ID of the task to remove from the Maintenance Window
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Task
      - From
      - Maintenance
      - Window
  /?Action=DescribeActivations:
    get:
      summary: Describe Activations
      description: |-
        Details about the activation, including: the date and time the activation was created,
           the expiration date, the IAM role assigned to the instances in the activation, and the number of
           instances activated by this registration.
      operationId: describeActivations
      x-api-path-slug: actiondescribeactivations-get
      parameters:
      - in: query
        name: Filters
        description: A filter to view information about your activations
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: A token to start the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activations
  /?Action=DescribeAssociation:
    get:
      summary: Describe Association
      description: Describes the associations for the specified SSM document or instance.
      operationId: describeAssociation
      x-api-path-slug: actiondescribeassociation-get
      parameters:
      - in: query
        name: AssociationId
        description: The association ID for which you want information
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      - in: query
        name: Name
        description: The name of the SSM document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Association
  /?Action=DescribeAutomationExecutions:
    get:
      summary: Describe Automation Executions
      description: Provides details about all active and terminated Automation executions.
      operationId: describeAutomationExecutions
      x-api-path-slug: actiondescribeautomationexecutions-get
      parameters:
      - in: query
        name: Filters
        description: Filters used to limit the scope of executions that are requested
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Automation
      - Executions
  /?Action=DescribeAvailablePatches:
    get:
      summary: Describe Available Patches
      description: Lists all patches that could possibly be included in a patch baseline.
      operationId: describeAvailablePatches
      x-api-path-slug: actiondescribeavailablepatches-get
      parameters:
      - in: query
        name: Filters
        description: Filters used to scope down the returned patches
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of patches to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Available
      - Patches
  /?Action=DescribeDocument:
    get:
      summary: Describe Document
      description: Describes the specified SSM document.
      operationId: describeDocument
      x-api-path-slug: actiondescribedocument-get
      parameters:
      - in: query
        name: DocumentVersion
        description: The document version for which you want information
        type: string
      - in: query
        name: Name
        description: The name of the SSM document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Document
  /?Action=DescribeDocumentPermission:
    get:
      summary: Describe Document Permission
      description: Describes the permissions for an SSM document.
      operationId: describeDocumentPermission
      x-api-path-slug: actiondescribedocumentpermission-get
      parameters:
      - in: query
        name: Name
        description: The name of the document for which you are the owner
        type: string
      - in: query
        name: PermissionType
        description: The permission type for the document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Document
      - Permission
  /?Action=DescribeEffectiveInstanceAssociations:
    get:
      summary: Describe Effective Instance Associations
      description: All associations for the instance(s).
      operationId: describeEffectiveInstanceAssociations
      x-api-path-slug: actiondescribeeffectiveinstanceassociations-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID for which you want to view all associations
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Effective
      - Instance
      - Associations
  /?Action=DescribeEffectivePatchesForPatchBaseline:
    get:
      summary: Describe Effective Patches For Patch Baseline
      description: Retrieves the current effective patches (the patch and the approval
        state) for the specified patch baseline.
      operationId: describeEffectivePatchesForPatchBaseline
      x-api-path-slug: actiondescribeeffectivepatchesforpatchbaseline-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline to retrieve the effective patches
          for
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of patches to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Effective
      - PatchesBaseline
  /?Action=DescribeInstanceAssociationsStatus:
    get:
      summary: Describe Instance Associations Status
      description: The status of the associations for the instance(s).
      operationId: describeInstanceAssociationsStatus
      x-api-path-slug: actiondescribeinstanceassociationsstatus-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance IDs for which you want association status information
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
      - Associations
      - Status
  /?Action=DescribeInstanceInformation:
    get:
      summary: Describe Instance Information
      description: Describes one or more of your instances.
      operationId: describeInstanceInformation
      x-api-path-slug: actiondescribeinstanceinformation-get
      parameters:
      - in: query
        name: Filters
        description: One or more filters
        type: string
      - in: query
        name: InstanceInformationFilterList
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
      - Information
  /?Action=DescribeInstancePatches:
    get:
      summary: Describe Instance Patches
      description: Retrieves information about the patches on the specified instance
        and their state relative to the patch baseline being used for the instance.
      operationId: describeInstancePatches
      x-api-path-slug: actiondescribeinstancepatches-get
      parameters:
      - in: query
        name: Filters
        description: 'Each entry in the array is a structure containing:'
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance whose patch state information should be
          retrieved
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of patches to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
      - Patches
  /?Action=DescribeInstancePatchStates:
    get:
      summary: Describe Instance Patch States
      description: Retrieves the high-level patch state of one or more instances.
      operationId: describeInstancePatchStates
      x-api-path-slug: actiondescribeinstancepatchstates-get
      parameters:
      - in: query
        name: InstanceIds
        description: The ID of the instance whose patch state information should be
          retrieved
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of instances to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
      - States
  /?Action=DescribeInstancePatchStatesForPatchGroup:
    get:
      summary: Describe Instance Patch States For Patch Group
      description: Retrieves the high-level patch state for the instances in the specified
        patch group.
      operationId: describeInstancePatchStatesForPatchGroup
      x-api-path-slug: actiondescribeinstancepatchstatesforpatchgroup-get
      parameters:
      - in: query
        name: Filters
        description: 'Each entry in the array is a structure containing:'
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of patches to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: PatchGroup
        description: The name of the patch group for which the patch state information
          should be retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
      - StatesGroup
  /?Action=DescribeMaintenanceWindowExecutions:
    get:
      summary: Describe Maintenance Window Executions
      description: |-
        Lists the executions of a Maintenance Window (meaning, information about when the
           Maintenance Window was scheduled to be active and information about tasks registered and run with
           the Maintenance Window).
      operationId: describeMaintenanceWindowExecutions
      x-api-path-slug: actiondescribemaintenancewindowexecutions-get
      parameters:
      - in: query
        name: Filters
        description: 'Each entry in the array is a structure containing:'
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: WindowId
        description: The ID of the Maintenance Window whose executions should be retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Window
      - Executions
  /?Action=DescribeMaintenanceWindowExecutionTaskInvocations:
    get:
      summary: Describe Maintenance Window Execution Task Invocations
      description: |-
        Retrieves the individual task executions (one per target) for a particular task executed
           as part of a Maintenance Window execution.
      operationId: describeMaintenanceWindowExecutionTaskInvocations
      x-api-path-slug: actiondescribemaintenancewindowexecutiontaskinvocations-get
      parameters:
      - in: query
        name: Filters
        description: Optional filters used to scope down the returned task invocations
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: TaskId
        description: The ID of the specific task in the Maintenance Window task that
          should be   retrieved
        type: string
      - in: query
        name: WindowExecutionId
        description: The ID of the Maintenance Window execution the task is part of
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Window
      - Execution
      - Task
      - Invocations
  /?Action=DescribeMaintenanceWindowExecutionTasks:
    get:
      summary: Describe Maintenance Window Execution Tasks
      description: For a given Maintenance Window execution, lists the tasks that
        were executed.
      operationId: describeMaintenanceWindowExecutionTasks
      x-api-path-slug: actiondescribemaintenancewindowexecutiontasks-get
      parameters:
      - in: query
        name: Filters
        description: Optional filters used to scope down the returned tasks
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: WindowExecutionId
        description: The ID of the Maintenance Window execution whose task executions
          should be   retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Window
      - Execution
      - Tasks
  /?Action=DescribeMaintenanceWindows:
    get:
      summary: Describe Maintenance Windows
      description: Retrieves the Maintenance Windows in an AWS account.
      operationId: describeMaintenanceWindows
      x-api-path-slug: actiondescribemaintenancewindows-get
      parameters:
      - in: query
        name: Filters
        description: Optional filters used to narrow down the scope of the returned
          Maintenance Windows
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Windows
  /?Action=DescribeMaintenanceWindowTargets:
    get:
      summary: Describe Maintenance Window Targets
      description: Lists the targets registered with the Maintenance Window.
      operationId: describeMaintenanceWindowTargets
      x-api-path-slug: actiondescribemaintenancewindowtargets-get
      parameters:
      - in: query
        name: Filters
        description: Optional filters that can be used to narrow down the scope of
          the returned window   targets
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: WindowId
        description: The ID of the Maintenance Window whose targets should be retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Window
      - Targets
  /?Action=DescribeMaintenanceWindowTasks:
    get:
      summary: Describe Maintenance Window Tasks
      description: Lists the tasks in a Maintenance Window.
      operationId: describeMaintenanceWindowTasks
      x-api-path-slug: actiondescribemaintenancewindowtasks-get
      parameters:
      - in: query
        name: Filters
        description: Optional filters used to narrow down the scope of the returned
          tasks
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: WindowId
        description: The ID of the Maintenance Window whose tasks should be retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Window
      - Tasks
  /?Action=DescribeParameters:
    get:
      summary: Describe Parameters
      description: Get information about a parameter.
      operationId: describeParameters
      x-api-path-slug: actiondescribeparameters-get
      parameters:
      - in: query
        name: Filters
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameters
  /?Action=DescribePatchBaselines:
    get:
      summary: Describe Patch Baselines
      description: Lists the patch baselines in your AWS account.
      operationId: describePatchBaselines
      x-api-path-slug: actiondescribepatchbaselines-get
      parameters:
      - in: query
        name: Filters
        description: 'Each element in the array is a structure containing:'
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of patch baselines to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Baselines
  /?Action=DescribePatchGroups:
    get:
      summary: Describe Patch Groups
      description: Lists all patch groups that have been registered with patch baselines.
      operationId: describePatchGroups
      x-api-path-slug: actiondescribepatchgroups-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of patch groups to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=DescribePatchGroupState:
    get:
      summary: Describe Patch Group State
      description: Returns high-level aggregated patch compliance state for a patch
        group.
      operationId: describePatchGroupState
      x-api-path-slug: actiondescribepatchgroupstate-get
      parameters:
      - in: query
        name: PatchGroup
        description: The name of the patch group whose patch snapshot should be retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - State
  /?Action=GetAutomationExecution:
    get:
      summary: Get Automation Execution
      description: Get detailed information about a particular Automation execution.
      operationId: getAutomationExecution
      x-api-path-slug: actiongetautomationexecution-get
      parameters:
      - in: query
        name: AutomationExecutionId
        description: The unique identifier for an existing automation execution to
          examine
        type: string
      responses:
        200:
          description: OK
      tags:
      - Automation
      - Execution
  /?Action=GetCommandInvocation:
    get:
      summary: Get Command Invocation
      description: Returns detailed information about command execution for an invocation
        or plugin.
      operationId: getCommandInvocation
      x-api-path-slug: actiongetcommandinvocation-get
      parameters:
      - in: query
        name: CommandId
        description: (Required) The parent command ID of the invocation plugin
        type: string
      - in: query
        name: InstanceId
        description: (Required) The ID of the managed instance targeted by the command
        type: string
      - in: query
        name: PluginName
        description: (Optional) The name of the plugin for which you want detailed
          results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Command
      - Invocation
  /?Action=GetDefaultPatchBaseline:
    get:
      summary: Get Default Patch Baseline
      description: Retrieves the default patch baseline.
      operationId: getDefaultPatchBaseline
      x-api-path-slug: actiongetdefaultpatchbaseline-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the default patch baseline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Default
      - Baseline
  /?Action=GetDeployablePatchSnapshotForInstance:
    get:
      summary: Get Deployable Patch Snapshot For Instance
      description: Retrieves the current snapshot for the patch baseline the instance
        uses.
      operationId: getDeployablePatchSnapshotForInstance
      x-api-path-slug: actiongetdeployablepatchsnapshotforinstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The ID of the instance for which the appropriate patch snapshot
          should be retrieved
        type: string
      - in: query
        name: SnapshotId
        description: The user-defined snapshot ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployable
      - SnapshotInstance
  /?Action=GetDocument:
    get:
      summary: Get Document
      description: Gets the contents of the specified SSM document.
      operationId: getDocument
      x-api-path-slug: actiongetdocument-get
      parameters:
      - in: query
        name: DocumentVersion
        description: The document version for which you want information
        type: string
      - in: query
        name: Name
        description: The name of the SSM document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Document
  /?Action=GetInventory:
    get:
      summary: Get Inventory
      description: Query inventory information.
      operationId: getInventory
      x-api-path-slug: actiongetinventory-get
      parameters:
      - in: query
        name: Filters
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: ResultAttributes
        description: The list of inventory item types to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Inventory
  /?Action=GetInventorySchema:
    get:
      summary: Get Inventory Schema
      description: |-
        Return a list of inventory type names for the account, or return a list of attribute
           names for a specific Inventory item type.
      operationId: getInventorySchema
      x-api-path-slug: actiongetinventoryschema-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: TypeName
        description: The type of inventory item to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Inventory
      - Schema
  /?Action=GetMaintenanceWindow:
    get:
      summary: Get Maintenance Window
      description: Retrieves a Maintenance Window.
      operationId: getMaintenanceWindow
      x-api-path-slug: actiongetmaintenancewindow-get
      parameters:
      - in: query
        name: WindowId
        description: The ID of the desired Maintenance Window
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Window
  /?Action=GetMaintenanceWindowExecution:
    get:
      summary: Get Maintenance Window Execution
      description: |-
        Retrieves details about a specific task executed as part of a Maintenance Window
           execution.
      operationId: getMaintenanceWindowExecution
      x-api-path-slug: actiongetmaintenancewindowexecution-get
      parameters:
      - in: query
        name: WindowExecutionId
        description: The ID of the Maintenance Window execution that includes the
          task
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Window
      - Execution
  /?Action=GetMaintenanceWindowExecutionTask:
    get:
      summary: Get Maintenance Window Execution Task
      description: |-
        Retrieves the details about a specific task executed as part of a Maintenance Window
           execution.
      operationId: getMaintenanceWindowExecutionTask
      x-api-path-slug: actiongetmaintenancewindowexecutiontask-get
      parameters:
      - in: query
        name: TaskId
        description: The ID of the specific task execution in the Maintenance Window
          task that should be   retrieved
        type: string
      - in: query
        name: WindowExecutionId
        description: The ID of the Maintenance Window execution that includes the
          task
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Window
      - Execution
      - Task
  /?Action=GetParameterHistory:
    get:
      summary: Get Parameter History
      description: Query a list of all parameters used by the AWS account.
      operationId: getParameterHistory
      x-api-path-slug: actiongetparameterhistory-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: Name
        description: The name of a parameter you want to query
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: WithDecryption
        description: Return decrypted values for secure string parameters
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter
      - History
  /?Action=GetParameters:
    get:
      summary: Get Parameters
      description: Get a list of parameters used by the AWS account.
      operationId: getParameters
      x-api-path-slug: actiongetparameters-get
      parameters:
      - in: query
        name: Names
        description: Names of the parameters for which you want to query information
        type: string
      - in: query
        name: WithDecryption
        description: Return decrypted secure string value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameters
  /?Action=GetPatchBaseline:
    get:
      summary: Get Patch Baseline
      description: Retrieves information about a patch baseline.
      operationId: getPatchBaseline
      x-api-path-slug: actiongetpatchbaseline-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Baseline
  /?Action=GetPatchBaselineForPatchGroup:
    get:
      summary: Get Patch Baseline For Patch Group
      description: Retrieves the patch baseline that should be used for the specified
        patch group.
      operationId: getPatchBaselineForPatchGroup
      x-api-path-slug: actiongetpatchbaselineforpatchgroup-get
      parameters:
      - in: query
        name: PatchGroup
        description: The name of the patch group whose patch baseline should be retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - BaselineGroup
  /?Action=ListAssociations:
    get:
      summary: List Associations
      description: Lists the associations for the specified SSM document or instance.
      operationId: listAssociations
      x-api-path-slug: actionlistassociations-get
      parameters:
      - in: query
        name: AssociationFilterList
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Associations
  /?Action=ListCommandInvocations:
    get:
      summary: List Command Invocations
      description: An invocation is copy of a command sent to a specific instance.
      operationId: listCommandInvocations
      x-api-path-slug: actionlistcommandinvocations-get
      parameters:
      - in: query
        name: CommandId
        description: (Optional) The invocations for a specific command ID
        type: string
      - in: query
        name: Details
        description: (Optional) If set this returns the response of the command executions
          and any command   output
        type: string
      - in: query
        name: Filters
        description: (Optional) One or more filters
        type: string
      - in: query
        name: InstanceId
        description: (Optional) The command execution details for a specific instance
          ID
        type: string
      - in: query
        name: MaxResults
        description: (Optional) The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: (Optional) The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Command
      - Invocations
  /?Action=ListCommands:
    get:
      summary: List Commands
      description: Lists the commands requested by users of the AWS account.
      operationId: listCommands
      x-api-path-slug: actionlistcommands-get
      parameters:
      - in: query
        name: CommandId
        description: (Optional) If provided, lists only the specified command
        type: string
      - in: query
        name: Filters
        description: (Optional) One or more filters
        type: string
      - in: query
        name: InstanceId
        description: (Optional) Lists commands issued against this instance ID
        type: string
      - in: query
        name: MaxResults
        description: (Optional) The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: (Optional) The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Commands
  /?Action=ListDocuments:
    get:
      summary: List Documents
      description: Describes one or more of your SSM documents.
      operationId: listDocuments
      x-api-path-slug: actionlistdocuments-get
      parameters:
      - in: query
        name: DocumentFilterList
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Documents
  /?Action=ListDocumentVersions:
    get:
      summary: List Document Versions
      description: List all versions for a document.
      operationId: listDocumentVersions
      x-api-path-slug: actionlistdocumentversions-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: Name
        description: The name of the document about which you want version information
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Document
      - Versions
  /?Action=ListInventoryEntries:
    get:
      summary: List Inventory Entries
      description: A list of inventory items returned by the request.
      operationId: listInventoryEntries
      x-api-path-slug: actionlistinventoryentries-get
      parameters:
      - in: query
        name: Filters
        description: One or more filters
        type: string
      - in: query
        name: InstanceId
        description: The instance ID for which you want inventory information
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: TypeName
        description: The type of inventory item for which you want information
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Inventory
      - Entries
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: Returns a list of the tags assigned to the specified resource.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID for which you want to see a list of tags
        type: string
      - in: query
        name: ResourceType
        description: Returns a list of tags for a specific resource type
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - TagsResource
  /?Action=ModifyDocumentPermission:
    get:
      summary: Modify Document Permission
      description: Share a document publicly or privately.
      operationId: modifyDocumentPermission
      x-api-path-slug: actionmodifydocumentpermission-get
      parameters:
      - in: query
        name: AccountIdsToAdd
        description: The AWS user accounts that should have access to the document
        type: string
      - in: query
        name: AccountIdsToRemove
        description: The AWS user accounts that should no longer have access to the
          document
        type: string
      - in: query
        name: Name
        description: The name of the document that you want to share
        type: string
      - in: query
        name: PermissionType
        description: The permission type for the document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Modify
      - Document
      - Permission
  /?Action=PutInventory:
    get:
      summary: Put Inventory
      description: Bulk update custom inventory items on one more instance.
      operationId: putInventory
      x-api-path-slug: actionputinventory-get
      parameters:
      - in: query
        name: InstanceId
        description: One or more instance IDs where you want to add or update inventory
          items
        type: string
      - in: query
        name: Items
        description: The inventory items that you want to add or update on instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Inventory
  /?Action=PutParameter:
    get:
      summary: Put Parameter
      description: Add one or more paramaters to the system.
      operationId: putParameter
      x-api-path-slug: actionputparameter-get
      parameters:
      - in: query
        name: Description
        description: Information about the parameter that you want to add to the system
        type: string
      - in: query
        name: KeyId
        description: The parameter key ID that you want to add to the system
        type: string
      - in: query
        name: Name
        description: The name of the parameter that you want to add to the system
        type: string
      - in: query
        name: Overwrite
        description: Overwrite an existing parameter
        type: string
      - in: query
        name: Type
        description: The type of parameter that you want to add to the system
        type: string
      - in: query
        name: Value
        description: The parameter value that you want to add to the system
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter
  /?Action=RegisterDefaultPatchBaseline:
    get:
      summary: Register Default Patch Baseline
      description: Defines the default patch baseline.
      operationId: registerDefaultPatchBaseline
      x-api-path-slug: actionregisterdefaultpatchbaseline-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline that should be the default patch
          baseline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Default
      - Baseline
  /?Action=RegisterPatchBaselineForPatchGroup:
    get:
      summary: Register Patch Baseline For Patch Group
      description: Registers a patch baseline for a patch group.
      operationId: registerPatchBaselineForPatchGroup
      x-api-path-slug: actionregisterpatchbaselineforpatchgroup-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline to register the patch group with
        type: string
      - in: query
        name: PatchGroup
        description: The name of the patch group that should be registered with the
          patch baseline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - BaselineGroup
  /?Action=RegisterTargetWithMaintenanceWindow:
    get:
      summary: Register Target With Maintenance Window
      description: Registers a target with a Maintenance Window.
      operationId: registerTargetWithMaintenanceWindow
      x-api-path-slug: actionregistertargetwithmaintenancewindow-get
      parameters:
      - in: query
        name: ClientToken
        description: User-provided idempotency token
        type: string
      - in: query
        name: OwnerInformation
        description: User-provided value that will be included in any CloudWatch events
          raised while running   tasks for these targets in this Maintenance Window
        type: string
      - in: query
        name: ResourceType
        description: The type of target being registered with the Maintenance Window
        type: string
      - in: query
        name: Targets
        description: The targets (either instances or tags)
        type: string
      - in: query
        name: WindowId
        description: The ID of the Maintenance Window the target should be registered
          with
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - TargetMaintenance
      - Window
  /?Action=RegisterTaskWithMaintenanceWindow:
    get:
      summary: Register Task With Maintenance Window
      description: Adds a new task to a Maintenance Window.
      operationId: registerTaskWithMaintenanceWindow
      x-api-path-slug: actionregistertaskwithmaintenancewindow-get
      parameters:
      - in: query
        name: ClientToken
        description: User-provided idempotency token
        type: string
      - in: query
        name: LoggingInfo
        description: A structure containing information about an Amazon S3 bucket
          to write instance-level logs to
        type: string
      - in: query
        name: MaxConcurrency
        description: The maximum number of targets this task can be run for in parallel
        type: string
      - in: query
        name: MaxErrors
        description: The maximum number of errors allowed before this task stops being
          scheduled
        type: string
      - in: query
        name: Priority
        description: The priority of the task in the Maintenance Window, the lower
          the number the higher the   priority
        type: string
      - in: query
        name: ServiceRoleArn
        description: The role that should be assumed when executing the task
        type: string
      - in: query
        name: Targets
        description: The targets (either instances or tags)
        type: string
      - in: query
        name: TaskArn
        description: The ARN of the task to execute
        type: string
      - in: query
        name: TaskParameters
        description: The parameters that should be passed to the task when it is executed
        type: string
      - in: query
        name: TaskType
        description: The type of task being registered
        type: string
      - in: query
        name: WindowId
        description: The id of the Maintenance Window the task should be added to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - TaskMaintenance
      - Window
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes all tags from the specified resource.
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID for which you want to remove tags
        type: string
      - in: query
        name: ResourceType
        description: The type of resource of which you want to remove a tag
        type: string
      - in: query
        name: TagKeys
        description: Tag keys that you want to remove from the specified resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Tags
      - From
      - Resource
  /?Action=SendCommand:
    get:
      summary: Send Command
      description: Executes commands on one or more remote instances.
      operationId: sendCommand
      x-api-path-slug: actionsendcommand-get
      parameters:
      - in: query
        name: Comment
        description: User-specified information about the command, such as a brief
          description of what the   command should do
        type: string
      - in: query
        name: DocumentHash
        description: The Sha256 or Sha1 hash created by the system when the document
          was created
        type: string
      - in: query
        name: DocumentHashType
        description: Sha256 or Sha1
        type: string
      - in: query
        name: DocumentName
        description: Required
        type: string
      - in: query
        name: InstanceIds
        description: Required
        type: string
      - in: query
        name: MaxConcurrency
        description: (Optional) The maximum number of instances that are allowed to
          execute the command at the   same time
        type: string
      - in: query
        name: MaxErrors
        description: The maximum number of errors allowed without the command failing
        type: string
      - in: query
        name: NotificationConfig
        description: Configurations for sending notifications
        type: string
      - in: query
        name: OutputS3BucketName
        description: The name of the S3 bucket where command execution responses should
          be stored
        type: string
      - in: query
        name: OutputS3KeyPrefix
        description: The directory structure within the S3 bucket where the responses
          should be   stored
        type: string
      - in: query
        name: OutputS3Region
        description: (Optional) The region where the Amazon Simple Storage Service
          (Amazon S3) output bucket is located
        type: string
      - in: query
        name: Parameters
        description: The required and optional parameters specified in the SSM document
          being   executed
        type: string
      - in: query
        name: ServiceRoleArn
        description: The IAM role that Systems Manager uses to send notifications
        type: string
      - in: query
        name: Targets
        description: (Optional) An array of search criteria that targets instances
          using a    Key;Value combination that you specify
        type: string
      - in: query
        name: TimeoutSeconds
        description: If this time is reached and the command has not already started
          executing, it will not   execute
        type: string
      responses:
        200:
          description: OK
      tags:
      - Send
      - Command
  /?Action=StartAutomationExecution:
    get:
      summary: Start Automation Execution
      description: Initiates execution of an Automation document.
      operationId: startAutomationExecution
      x-api-path-slug: actionstartautomationexecution-get
      parameters:
      - in: query
        name: DocumentName
        description: The name of the Automation document to use for this execution
        type: string
      - in: query
        name: DocumentVersion
        description: The version of the Automation document to use for this execution
        type: string
      - in: query
        name: Parameters
        description: A key-value map of execution parameters, which match the declared
          parameters in the Automation document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Start
      - Automation
      - Execution
  /?Action=StopAutomationExecution:
    get:
      summary: Stop Automation Execution
      description: Stop an Automation that is currently executing.
      operationId: stopAutomationExecution
      x-api-path-slug: actionstopautomationexecution-get
      parameters:
      - in: query
        name: AutomationExecutionId
        description: The execution ID of the Automation to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Automation
      - Execution
  /?Action=UpdateAssociation:
    get:
      summary: Update Association
      description: Updates an association.
      operationId: updateAssociation
      x-api-path-slug: actionupdateassociation-get
      parameters:
      - in: query
        name: AssociationId
        description: The ID of the association you want to update
        type: string
      - in: query
        name: DocumentVersion
        description: The document version you want update for the association
        type: string
      - in: query
        name: OutputLocation
        description: An Amazon S3 bucket where you want to store the results of this
          request
        type: string
      - in: query
        name: Parameters
        description: The parameters you want to update for the association
        type: string
      - in: query
        name: ScheduleExpression
        description: The cron expression used to schedule the association that you
          want to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Association
  /?Action=UpdateAssociationStatus:
    get:
      summary: Update Association Status
      description: |-
        Updates the status of the SSM document associated with the specified
           instance.
      operationId: updateAssociationStatus
      x-api-path-slug: actionupdateassociationstatus-get
      parameters:
      - in: query
        name: AssociationStatus
        description: The association status
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: Name
        description: The name of the SSM document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Association
      - Status
  /?Action=UpdateDocument:
    get:
      summary: Update Document
      description: The document you want to update.
      operationId: updateDocument
      x-api-path-slug: actionupdatedocument-get
      parameters:
      - in: query
        name: Content
        description: The content in a document that you want to update
        type: string
      - in: query
        name: DocumentVersion
        description: The version of the document that you want to update
        type: string
      - in: query
        name: Name
        description: The name of the document that you want to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Document
  /?Action=UpdateDocumentDefaultVersion:
    get:
      summary: Update Document Default Version
      description: Set the default version of a document.
      operationId: updateDocumentDefaultVersion
      x-api-path-slug: actionupdatedocumentdefaultversion-get
      parameters:
      - in: query
        name: DocumentVersion
        description: The version of a custom document that you want to set as the
          default version
        type: string
      - in: query
        name: Name
        description: The name of a custom document that you want to set as the default
          version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Document
      - Default
      - Version
  /?Action=UpdateMaintenanceWindow:
    get:
      summary: Update Maintenance Window
      description: Updates an existing Maintenance Window.
      operationId: updateMaintenanceWindow
      x-api-path-slug: actionupdatemaintenancewindow-get
      parameters:
      - in: query
        name: AllowUnassociatedTargets
        description: Whether targets must be registered with the Maintenance Window
          before tasks can be   defined for those targets
        type: string
      - in: query
        name: Cutoff
        description: The number of hours before the end of the Maintenance Window
          that Systems Manager stops   scheduling new tasks for execution
        type: string
      - in: query
        name: Duration
        description: The duration of the Maintenance Window in hours
        type: string
      - in: query
        name: Enabled
        description: Whether the Maintenance Window is enabled
        type: string
      - in: query
        name: Name
        description: The name of the Maintenance Window
        type: string
      - in: query
        name: Schedule
        description: The schedule of the Maintenance Window in the form of a cron
          or rate   expression
        type: string
      - in: query
        name: WindowId
        description: The ID of the Maintenance Window to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Window
  /?Action=UpdateManagedInstanceRole:
    get:
      summary: Update Managed Instance Role
      description: |-
        Assigns or changes an Amazon Identity and Access Management (IAM) role to the managed
           instance.
      operationId: updateManagedInstanceRole
      x-api-path-slug: actionupdatemanagedinstancerole-get
      parameters:
      - in: query
        name: IamRole
        description: The IAM role you want to assign or change
        type: string
      - in: query
        name: InstanceId
        description: The ID of the managed instance where you want to update the role
        type: string
      responses:
        200:
          description: OK
      tags:
      - Managed
      - Instance
      - Role
  /?Action=UpdatePatchBaseline:
    get:
      summary: Update Patch Baseline
      description: Modifies an existing patch baseline.
      operationId: updatePatchBaseline
      x-api-path-slug: actionupdatepatchbaseline-get
      parameters:
      - in: query
        name: ApprovalRules
        description: A set of rules used to include patches in the baseline
        type: string
      - in: query
        name: ApprovedPatches
        description: A list of explicitly approved patches for the baseline
        type: string
      - in: query
        name: BaselineId
        description: The ID of the patch baseline to update
        type: string
      - in: query
        name: Description
        description: A description of the patch baseline
        type: string
      - in: query
        name: GlobalFilters
        description: A set of global filters used to exclude patches from the baseline
        type: string
      - in: query
        name: Name
        description: The name of the patch baseline
        type: string
      - in: query
        name: RejectedPatches
        description: A list of explicitly rejected patches for the baseline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Baseline