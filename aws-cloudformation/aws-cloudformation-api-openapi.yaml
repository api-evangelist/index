swagger: "2.0"
x-collection-name: AWS CloudFormation
x-complete: 1
info:
  title: AWS CloudFormation API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CancelUpdateStack:
    get:
      summary: Cancel Update Stack
      description: Cancels an update on the specified stack.
      operationId: cancelUpdateStack
      x-api-path-slug: actioncancelupdatestack-get
      parameters:
      - in: query
        name: StackName
        description: The name or the unique stack ID that is associated with the stack
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stacks
  /?Action=ContinueUpdateRollback:
    get:
      summary: Continue Update Rollback
      description: |-
        For a specified stack that is in the UPDATE_ROLLBACK_FAILED state, continues rolling it back
                 to the UPDATE_ROLLBACK_COMPLETE state.
      operationId: continueUpdateRollback
      x-api-path-slug: actioncontinueupdaterollback-get
      parameters:
      - in: query
        name: ResourcesToSkip.member.N
        description: A list of the logical IDs of the resources that AWS CloudFormation
          skips during the continue update rollback operation
        type: string
      - in: query
        name: RoleARN
        description: The Amazon Resource Name (ARN) of an AWS Identity and Access
          Management (IAM) role that AWS CloudFormation         assumes to roll back
          the stack
        type: string
      - in: query
        name: StackName
        description: The name or the unique ID of the stack that you want to continue
          rolling back
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rollback
  /?Action=CreateChangeSet:
    get:
      summary: Create Change Set
      description: Creates a list of changes for a stack.
      operationId: createChangeSet
      x-api-path-slug: actioncreatechangeset-get
      parameters:
      - in: query
        name: Capabilities.member.N
        description: A list of values that you must specify before AWS CloudFormation
          can update certain stacks
        type: string
      - in: query
        name: ChangeSetName
        description: The name of the change set
        type: string
      - in: query
        name: ChangeSetType
        description: The type of change set operation
        type: string
      - in: query
        name: ClientToken
        description: A unique identifier for this CreateChangeSet request
        type: string
      - in: query
        name: Description
        description: A description to help you identify this change set
        type: string
      - in: query
        name: NotificationARNs.member.N
        description: The Amazon Resource Names (ARNs) of Amazon Simple Notification
          Service (Amazon SNS) topics that AWS CloudFormation associates with the
          stack
        type: string
      - in: query
        name: Parameters.member.N
        description: A list of Parameter structures that specify input parameters
          for the change set
        type: string
      - in: query
        name: ResourceTypes.member.N
        description: The template resource types that you have permissions to work
          with if you execute this change set, such as AWS::EC2::Instance, AWS::EC2::*,
          or Custom::MyCustomInstance
        type: string
      - in: query
        name: RoleARN
        description: The Amazon Resource Name (ARN) of an AWS Identity and Access
          Management (IAM) role that AWS CloudFormation         assumes when executing
          the change set
        type: string
      - in: query
        name: StackName
        description: The name or the unique ID of the stack for which you are creating
          a change set
        type: string
      - in: query
        name: Tags.member.N
        description: Key-value pairs to associate with this stack
        type: string
      - in: query
        name: TemplateBody
        description: A structure that contains the body of the revised template, with
          a minimum length of 1 byte and a maximum length of 51,200 bytes
        type: string
      - in: query
        name: TemplateURL
        description: The location of the file that contains the revised template
        type: string
      - in: query
        name: UsePreviousTemplate
        description: Whether to reuse the template that is associated with the stack
          to create the change set
        type: string
      responses:
        200:
          description: OK
      tags:
      - Change Sets
  /?Action=CreateStack:
    get:
      summary: Create Stack
      description: Creates a stack as specified in the template.
      operationId: createStack
      x-api-path-slug: actioncreatestack-get
      parameters:
      - in: query
        name: Capabilities.member.N
        description: A list of values that you must specify before AWS CloudFormation
          can create certain stacks
        type: string
      - in: query
        name: DisableRollback
        description: Set to true to disable rollback of the stack if stack creation
          failed
        type: string
      - in: query
        name: NotificationARNs.member.N
        description: The Simple Notification Service (SNS) topic ARNs to publish stack
          related events
        type: string
      - in: query
        name: OnFailure
        description: Determines what action will be taken if stack creation fails
        type: string
      - in: query
        name: Parameters.member.N
        description: A list of Parameter structures that specify input parameters
          for the stack
        type: string
      - in: query
        name: ResourceTypes.member.N
        description: The template resource types that you have permissions to work
          with for this create stack action, such as AWS::EC2::Instance, AWS::EC2::*,
          or Custom::MyCustomInstance
        type: string
      - in: query
        name: RoleARN
        description: The Amazon Resource Name (ARN) of an AWS Identity and Access
          Management (IAM) role that AWS CloudFormation         assumes to create
          the stack
        type: string
      - in: query
        name: StackName
        description: The name that is associated with the stack
        type: string
      - in: query
        name: StackPolicyBody
        description: Structure containing the stack policy body
        type: string
      - in: query
        name: StackPolicyURL
        description: Location of a file containing the stack policy
        type: string
      - in: query
        name: Tags.member.N
        description: Key-value pairs to associate with this stack
        type: string
      - in: query
        name: TemplateBody
        description: Structure containing the template body with a minimum length
          of 1 byte and a maximum length of 51,200 bytes
        type: string
      - in: query
        name: TemplateURL
        description: Location of file containing the template body
        type: string
      - in: query
        name: TimeoutInMinutes
        description: The amount of time that can pass before the stack status becomes
          CREATE_FAILED; if DisableRollback         is not set or is set to false,
          the stack will be rolled back
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stacks
  /?Action=DeleteChangeSet:
    get:
      summary: Delete Change Set
      description: Deletes the specified change set.
      operationId: deleteChangeSet
      x-api-path-slug: actiondeletechangeset-get
      parameters:
      - in: query
        name: ChangeSetName
        description: The name or Amazon Resource Name (ARN) of the change set that
          you want to delete
        type: string
      - in: query
        name: StackName
        description: If you specified the name of a change set to delete, specify
          the stack name or ID (ARN) that is associated with it
        type: string
      responses:
        200:
          description: OK
      tags:
      - Change Sets
  /?Action=DeleteStack:
    get:
      summary: Delete Stack
      description: Deletes a specified stack.
      operationId: deleteStack
      x-api-path-slug: actiondeletestack-get
      parameters:
      - in: query
        name: RetainResources.member.N
        description: For stacks in the DELETE_FAILED state, a list of resource logical
          IDs that are associated with          the resources you want to retain
        type: string
      - in: query
        name: RoleARN
        description: The Amazon Resource Name (ARN) of an AWS Identity and Access
          Management (IAM) role that AWS CloudFormation         assumes to delete
          the stack
        type: string
      - in: query
        name: StackName
        description: The name or the unique stack ID that is associated with the stack
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stacks
  /?Action=DescribeAccountLimits:
    get:
      summary: Describe Account Limits
      description: Retrieves your account's AWS CloudFormation limits, such as the
        maximum number of stacks that you can create in your account.
      operationId: describeAccountLimits
      x-api-path-slug: actiondescribeaccountlimits-get
      parameters:
      - in: query
        name: NextToken
        description: A string that identifies the next page of limits that you want
          to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Limits
  /?Action=DescribeChangeSet:
    get:
      summary: Describe Change Set
      description: Returns the inputs for the change set and a list of changes that
        AWS CloudFormation will make if you execute the change set.
      operationId: describeChangeSet
      x-api-path-slug: actiondescribechangeset-get
      parameters:
      - in: query
        name: ChangeSetName
        description: The name or Amazon Resource Name (ARN) of the change set that
          you want to describe
        type: string
      - in: query
        name: NextToken
        description: A string (provided by the DescribeChangeSet response output)
          that identifies the next page of information that you want to retrieve
        type: string
      - in: query
        name: StackName
        description: If you specified the name of a change set, specify the stack
          name or ID (ARN) of the change set you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Change Sets
  /?Action=DescribeStackEvents:
    get:
      summary: Describe Stack Events
      description: Returns all stack related events for a specified stack in reverse
        chronological order.
      operationId: describeStackEvents
      x-api-path-slug: actiondescribestackevents-get
      parameters:
      - in: query
        name: NextToken
        description: A string that identifies the next page of events that you want
          to retrieve
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack Events
  /?Action=DescribeStackResource:
    get:
      summary: Describe Stack Resource
      description: Returns a description of the specified resource in the specified
        stack.
      operationId: describeStackResource
      x-api-path-slug: actiondescribestackresource-get
      parameters:
      - in: query
        name: LogicalResourceId
        description: The logical name of the resource as specified in the template
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack Resources
  /?Action=DescribeStackResources:
    get:
      summary: Describe Stack Resources
      description: Returns AWS resource descriptions for running and deleted stacks.
      operationId: describeStackResources
      x-api-path-slug: actiondescribestackresources-get
      parameters:
      - in: query
        name: LogicalResourceId
        description: The logical name of the resource as specified in the template
        type: string
      - in: query
        name: PhysicalResourceId
        description: The name or unique identifier that corresponds to a physical
          instance ID of a resource supported by AWS CloudFormation
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack Resources
  /?Action=DescribeStacks:
    get:
      summary: Describe Stacks
      description: Returns the description for the specified stack; if no stack name
        was specified, then it returns the description for all the stacks created.
      operationId: describeStacks
      x-api-path-slug: actiondescribestacks-get
      parameters:
      - in: query
        name: NextToken
        description: A string that identifies the next page of stacks that you want
          to retrieve
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stacks
  /?Action=EstimateTemplateCost:
    get:
      summary: Estimate Template Cost
      description: Returns the estimated monthly cost of a template.
      operationId: estimateTemplateCost
      x-api-path-slug: actionestimatetemplatecost-get
      parameters:
      - in: query
        name: Parameters.member.N
        description: A list of Parameter structures that specify input parameters
        type: string
      - in: query
        name: TemplateBody
        description: Structure containing the template body with a minimum length
          of 1 byte and a maximum length of 51,200 bytes
        type: string
      - in: query
        name: TemplateURL
        description: Location of file containing the template body
        type: string
      responses:
        200:
          description: OK
      tags:
      - Template Cost
  /?Action=ExecuteChangeSet:
    get:
      summary: Execute Change Set
      description: Updates a stack using the input information that was provided when
        the specified change set was created.
      operationId: executeChangeSet
      x-api-path-slug: actionexecutechangeset-get
      parameters:
      - in: query
        name: ChangeSetName
        description: The name or ARN of the change set that you want use to update
          the specified stack
        type: string
      - in: query
        name: StackName
        description: If you specified the name of a change set, specify the stack
          name or ID (ARN) that is associated with the change set you want to execute
        type: string
      responses:
        200:
          description: OK
      tags:
      - Change Sets
  /?Action=GetStackPolicy:
    get:
      summary: Get Stack Policy
      description: Returns the stack policy for a specified stack.
      operationId: getStackPolicy
      x-api-path-slug: actiongetstackpolicy-get
      parameters:
      - in: query
        name: StackName
        description: The name or unique stack ID that is associated with the stack
          whose policy you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack Policies
  /?Action=GetTemplate:
    get:
      summary: Get Template
      description: Returns the template body for a specified stack.
      operationId: getTemplate
      x-api-path-slug: actiongettemplate-get
      parameters:
      - in: query
        name: ChangeSetName
        description: The name or Amazon Resource Name (ARN) of a change set for which
          AWS CloudFormation returns the associated template
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      - in: query
        name: TemplateStage
        description: For templates that include transforms, the stage of the template
          that AWS CloudFormation returns
        type: string
      responses:
        200:
          description: OK
      tags:
      - Templates
  /?Action=GetTemplateSummary:
    get:
      summary: Get Template Summary
      description: Returns information about a new or existing template.
      operationId: getTemplateSummary
      x-api-path-slug: actiongettemplatesummary-get
      parameters:
      - in: query
        name: StackName
        description: The name or the stack ID that is associated with the stack, which
          are not always interchangeable
        type: string
      - in: query
        name: TemplateBody
        description: Structure containing the template body with a minimum length
          of 1 byte and a maximum length of 51,200 bytes
        type: string
      - in: query
        name: TemplateURL
        description: Location of file containing the template body
        type: string
      responses:
        200:
          description: OK
      tags:
      - Templates
  /?Action=ListChangeSets:
    get:
      summary: List Change Sets
      description: Returns the ID and status of each active change set for a stack.
      operationId: listChangeSets
      x-api-path-slug: actionlistchangesets-get
      parameters:
      - in: query
        name: NextToken
        description: A string (provided by the ListChangeSets response output) that
          identifies the next page of change sets that you want to retrieve
        type: string
      - in: query
        name: StackName
        description: The name or the Amazon Resource Name (ARN) of the stack for which
          you want to list change sets
        type: string
      responses:
        200:
          description: OK
      tags:
      - Change Sets
  /?Action=ListExports:
    get:
      summary: List Exports
      description: Lists all exported output values in the account and region in which
        you call this action.
      operationId: listExports
      x-api-path-slug: actionlistexports-get
      parameters:
      - in: query
        name: NextToken
        description: A string (provided by the ListExports response output) that        identifies
          the next page of exported output values that you asked to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Exports
  /?Action=ListImports:
    get:
      summary: List Imports
      description: Lists all stacks that are importing an exported output value.
      operationId: listImports
      x-api-path-slug: actionlistimports-get
      parameters:
      - in: query
        name: ExportName
        description: The name of the exported output value
        type: string
      - in: query
        name: NextToken
        description: A string (provided by the ListImports response output) that         identifies
          the next page of stacks that are importing the specified exported output
          value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Imports
  /?Action=ListStackResources:
    get:
      summary: List Stack Resources
      description: Returns descriptions of all resources of the specified stack.
      operationId: listStackResources
      x-api-path-slug: actionliststackresources-get
      parameters:
      - in: query
        name: NextToken
        description: A string that identifies the next page of stack resources that
          you want to retrieve
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack Resources
  /?Action=ListStacks:
    get:
      summary: List Stacks
      description: Returns the summary information for stacks whose status matches
        the specified StackStatusFilter.
      operationId: listStacks
      x-api-path-slug: actionliststacks-get
      parameters:
      - in: query
        name: NextToken
        description: A string that identifies the next page of stacks that you want
          to retrieve
        type: string
      - in: query
        name: StackStatusFilter.member.N
        description: Stack status to use as a filter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stacks
  /?Action=SetStackPolicy:
    get:
      summary: Set Stack Policy
      description: Sets a stack policy for a specified stack.
      operationId: setStackPolicy
      x-api-path-slug: actionsetstackpolicy-get
      parameters:
      - in: query
        name: StackName
        description: The name or unique stack ID that you want to associate a policy
          with
        type: string
      - in: query
        name: StackPolicyBody
        description: Structure containing the stack policy body
        type: string
      - in: query
        name: StackPolicyURL
        description: Location of a file containing the stack policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack Policies
  /?Action=SignalResource:
    get:
      summary: Signal Resource
      description: Sends a signal to the specified resource with a success or failure
        status.
      operationId: signalResource
      x-api-path-slug: actionsignalresource-get
      parameters:
      - in: query
        name: LogicalResourceId
        description: The logical ID of the resource that you want to signal
        type: string
      - in: query
        name: StackName
        description: The stack name or unique stack ID that includes the resource
          that you want to signal
        type: string
      - in: query
        name: Status
        description: The status of the signal, which is either success or failure
        type: string
      - in: query
        name: UniqueId
        description: A unique ID of the signal
        type: string
      responses:
        200:
          description: OK
      tags:
      - Signal Resources
  /?Action=UpdateStack:
    get:
      summary: Update Stack
      description: Updates a stack as specified in the template.
      operationId: updateStack
      x-api-path-slug: actionupdatestack-get
      parameters:
      - in: query
        name: Capabilities.member.N
        description: A list of values that you must specify before AWS CloudFormation
          can update certain stacks
        type: string
      - in: query
        name: NotificationARNs.member.N
        description: Amazon Simple Notification Service topic Amazon Resource Names
          (ARNs) that AWS CloudFormation associates with the stack
        type: string
      - in: query
        name: Parameters.member.N
        description: A list of Parameter structures that specify input parameters
          for the stack
        type: string
      - in: query
        name: ResourceTypes.member.N
        description: The template resource types that you have permissions to work
          with for this update stack action, such as AWS::EC2::Instance, AWS::EC2::*,
          or Custom::MyCustomInstance
        type: string
      - in: query
        name: RoleARN
        description: The Amazon Resource Name (ARN) of an AWS Identity and Access
          Management (IAM) role that AWS CloudFormation         assumes to update
          the stack
        type: string
      - in: query
        name: StackName
        description: The name or unique stack ID of the stack to update
        type: string
      - in: query
        name: StackPolicyBody
        description: Structure containing a new stack policy body
        type: string
      - in: query
        name: StackPolicyDuringUpdateBody
        description: Structure containing the temporary overriding stack policy body
        type: string
      - in: query
        name: StackPolicyDuringUpdateURL
        description: Location of a file containing the temporary overriding stack
          policy
        type: string
      - in: query
        name: StackPolicyURL
        description: Location of a file containing the updated stack policy
        type: string
      - in: query
        name: Tags.member.N
        description: Key-value pairs to associate with this stack
        type: string
      - in: query
        name: TemplateBody
        description: Structure containing the template body with a minimum length
          of 1 byte and a maximum length of 51,200 bytes
        type: string
      - in: query
        name: TemplateURL
        description: Location of file containing the template body
        type: string
      - in: query
        name: UsePreviousTemplate
        description: Reuse the existing template that is associated with the stack
          that you are updating
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stacks
  /?Action=ValidateTemplate:
    get:
      summary: Validate Template
      description: Validates a specified template.
      operationId: validateTemplate
      x-api-path-slug: actionvalidatetemplate-get
      parameters:
      - in: query
        name: TemplateBody
        description: Structure containing the template body with a minimum length
          of 1 byte and a maximum length of 51,200 bytes
        type: string
      - in: query
        name: TemplateURL
        description: Location of file containing the template body
        type: string
      responses:
        200:
          description: OK
      tags:
      - Templates