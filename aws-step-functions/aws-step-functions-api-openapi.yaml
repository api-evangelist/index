swagger: "2.0"
x-collection-name: AWS Step Functions
x-complete: 1
info:
  title: AWS Step Functions API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateActivity:
    get:
      summary: Create Activity
      description: Creates an activity.
      operationId: createActivity
      x-api-path-slug: actioncreateactivity-get
      parameters:
      - in: query
        name: name
        description: The name of the activity to create
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activity
  /?Action=CreateStateMachine:
    get:
      summary: Create State Machine
      description: Creates a state machine.
      operationId: createStateMachine
      x-api-path-slug: actioncreatestatemachine-get
      parameters:
      - in: query
        name: definition
        description: The Amazon States Language definition of the state machine
        type: string
      - in: query
        name: name
        description: The name of the state machine
        type: string
      - in: query
        name: roleArn
        description: The Amazon Resource Name (ARN) of the IAM role to use for this
          state machine
        type: string
      responses:
        200:
          description: OK
      tags:
      - State Machine
  /?Action=DeleteActivity:
    get:
      summary: Delete Activity
      description: Deletes an activity.
      operationId: deleteActivity
      x-api-path-slug: actiondeleteactivity-get
      parameters:
      - in: query
        name: activityArn
        description: The Amazon Resource Name (ARN) of the activity to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activity
  /?Action=DeleteStateMachine:
    get:
      summary: Delete State Machine
      description: Deletes a state machine.
      operationId: deleteStateMachine
      x-api-path-slug: actiondeletestatemachine-get
      parameters:
      - in: query
        name: stateMachineArn
        description: The Amazon Resource Name (ARN) of the state machine to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - State Machine
  /?Action=DescribeActivity:
    get:
      summary: Describe Activity
      description: Describes an activity.
      operationId: describeActivity
      x-api-path-slug: actiondescribeactivity-get
      parameters:
      - in: query
        name: activityArn
        description: The Amazon Resource Name (ARN) of the activity to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activity
  /?Action=DescribeExecution:
    get:
      summary: Describe Execution
      description: Describes an execution.
      operationId: describeExecution
      x-api-path-slug: actiondescribeexecution-get
      parameters:
      - in: query
        name: executionArn
        description: The Amazon Resource Name (ARN) of the execution to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Execution
  /?Action=DescribeStateMachine:
    get:
      summary: Describe State Machine
      description: Describes a state machine.
      operationId: describeStateMachine
      x-api-path-slug: actiondescribestatemachine-get
      parameters:
      - in: query
        name: stateMachineArn
        description: The Amazon Resource Name (ARN) of the state machine to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - State Machine
  /?Action=GetActivityTask:
    get:
      summary: Get Activity Task
      description: "Used by workers to retrieve a task (with the specified activity
        ARN) which has been scheduled \n    for execution by a running state machine."
      operationId: getActivityTask
      x-api-path-slug: actiongetactivitytask-get
      parameters:
      - in: query
        name: activityArn
        description: The Amazon Resource Name (ARN) of the activity to retrieve tasks
          from (assigned when you create the task      using CreateActivity
        type: string
      - in: query
        name: workerName
        description: You can provide an arbitrary name in order to identify the worker
          that the task is assigned to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activity Task
  /?Action=GetExecutionHistory:
    get:
      summary: Get Execution History
      description: Returns the history of the specified execution as a list of events.
      operationId: getExecutionHistory
      x-api-path-slug: actiongetexecutionhistory-get
      parameters:
      - in: query
        name: executionArn
        description: The Amazon Resource Name (ARN) of the execution
        type: string
      - in: query
        name: maxResults
        description: The maximum number of results that will be returned per call
        type: string
      - in: query
        name: nextToken
        description: If a nextToken was returned by a previous call, there are more
          results available
        type: string
      - in: query
        name: reverseOrder
        description: Lists events in descending order of their timeStamp
        type: string
      responses:
        200:
          description: OK
      tags:
      - Execution
  /?Action=ListActivities:
    get:
      summary: List Activities
      description: Lists the existing activities.
      operationId: listActivities
      x-api-path-slug: actionlistactivities-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of results that will be returned per call
        type: string
      - in: query
        name: nextToken
        description: If a nextToken was returned by a previous call, there are more
          results available
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activity
  /?Action=ListExecutions:
    get:
      summary: List Executions
      description: Lists the executions of a state machine that meet the filtering
        criteria.
      operationId: listExecutions
      x-api-path-slug: actionlistexecutions-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of results that will be returned per call
        type: string
      - in: query
        name: nextToken
        description: If a nextToken was returned by a previous call, there are more
          results available
        type: string
      - in: query
        name: stateMachineArn
        description: The Amazon Resource Name (ARN) of the state machine whose executions
          will be listed
        type: string
      - in: query
        name: statusFilter
        description: If specified, only list the executions whose current execution
          status matches the given filter
        type: string
      responses:
        200:
          description: OK
      tags:
      - State Machine
  /?Action=ListStateMachines:
    get:
      summary: List State Machines
      description: Lists the existing state machines.
      operationId: listStateMachines
      x-api-path-slug: actionliststatemachines-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of results that will be returned per call
        type: string
      - in: query
        name: nextToken
        description: If a nextToken was returned by a previous call, there are more
          results available
        type: string
      responses:
        200:
          description: OK
      tags:
      - State Machine
  /?Action=SendTaskFailure:
    get:
      summary: Send Task Failure
      description: Used by workers to report that the task identified by the taskToken
        failed.
      operationId: sendTaskFailure
      x-api-path-slug: actionsendtaskfailure-get
      parameters:
      - in: query
        name: cause
        description: A more detailed explanation of the cause of the failure
        type: string
      - in: query
        name: error
        description: An arbitrary error code that identifies the cause of the failure
        type: string
      - in: query
        name: taskToken
        description: The token that represents this task
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=SendTaskHeartbeat:
    get:
      summary: Send Task Heartbeat
      description: "Used by workers to report to the service that the task represented
        by the specified taskToken \n    is still making progress."
      operationId: sendTaskHeartbeat
      x-api-path-slug: actionsendtaskheartbeat-get
      parameters:
      - in: query
        name: taskToken
        description: The token that represents this task
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=SendTaskSuccess:
    get:
      summary: Send Task Success
      description: Used by workers to report that the task identified by the taskToken
        completed successfully.
      operationId: sendTaskSuccess
      x-api-path-slug: actionsendtasksuccess-get
      parameters:
      - in: query
        name: output
        description: The JSON output of the task
        type: string
      - in: query
        name: taskToken
        description: The token that represents this task
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=StartExecution:
    get:
      summary: Start Execution
      description: Starts a state machine execution.
      operationId: startExecution
      x-api-path-slug: actionstartexecution-get
      parameters:
      - in: query
        name: input
        description: The JSON input data for the execution
        type: string
      - in: query
        name: name
        description: The name of the execution
        type: string
      - in: query
        name: stateMachineArn
        description: The Amazon Resource Name (ARN) of the state machine to execute
        type: string
      responses:
        200:
          description: OK
      tags:
      - State Machine
  /?Action=StopExecution:
    get:
      summary: Stop Execution
      description: Stops an execution.
      operationId: stopExecution
      x-api-path-slug: actionstopexecution-get
      parameters:
      - in: query
        name: cause
        description: A more detailed explanation of the cause of the termination
        type: string
      - in: query
        name: error
        description: An arbitrary error code that identifies the cause of the termination
        type: string
      - in: query
        name: executionArn
        description: The Amazon Resource Name (ARN) of the execution to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Execution