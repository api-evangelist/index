swagger: "2.0"
x-collection-name: AWS Data Pipeline
x-complete: 1
info:
  title: AWS Data Pipeline API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ActivatePipeline:
    get:
      summary: Activate Pipeline
      description: Validates the specified pipeline and starts processing pipeline
        tasks.
      operationId: activatePipeline
      x-api-path-slug: actionactivatepipeline-get
      parameters:
      - in: query
        name: parameterValues
        description: A list of parameter values to pass to the pipeline at activation
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: startTimestamp
        description: The date and time to resume the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=AddTags:
    get:
      summary: Add Tags
      description: Adds or modifies tags for the specified pipeline.
      operationId: addTags
      x-api-path-slug: actionaddtags-get
      parameters:
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: tags
        description: The tags to add, as key/value pairs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=CreatePipeline:
    get:
      summary: Create Pipeline
      description: Creates a new, empty pipeline.
      operationId: createPipeline
      x-api-path-slug: actioncreatepipeline-get
      parameters:
      - in: query
        name: description
        description: The description for the pipeline
        type: string
      - in: query
        name: name
        description: The name for the pipeline
        type: string
      - in: query
        name: tags
        description: A list of tags to associate with the pipeline at creation
        type: string
      - in: query
        name: uniqueId
        description: A unique identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=DeactivatePipeline:
    get:
      summary: Deactivate Pipeline
      description: Deactivates the specified running pipeline.
      operationId: deactivatePipeline
      x-api-path-slug: actiondeactivatepipeline-get
      parameters:
      - in: query
        name: cancelActive
        description: Indicates whether to cancel any running objects
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=DeletePipeline:
    get:
      summary: Delete Pipeline
      description: Deletes a pipeline, its pipeline definition, and its run history.
      operationId: deletePipeline
      x-api-path-slug: actiondeletepipeline-get
      parameters:
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=DescribeObjects:
    get:
      summary: Describe Objects
      description: Gets the object definitions for a set of objects associated with
        the pipeline.
      operationId: describeObjects
      x-api-path-slug: actiondescribeobjects-get
      parameters:
      - in: query
        name: evaluateExpressions
        description: Indicates whether any expressions in the object should be evaluated
          when the object descriptions are returned
        type: string
      - in: query
        name: marker
        description: The starting point for the results to be returned
        type: string
      - in: query
        name: objectIds
        description: The IDs of the pipeline objects that contain the definitions
          to be described
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline that contains the object definitions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Objects
  /?Action=DescribePipelines:
    get:
      summary: Describe Pipelines
      description: Retrieves metadata about one or more pipelines.
      operationId: describePipelines
      x-api-path-slug: actiondescribepipelines-get
      parameters:
      - in: query
        name: pipelineIds
        description: The IDs of the pipelines to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=EvaluateExpression:
    get:
      summary: Evaluate Expression
      description: Task runners call EvaluateExpression to evaluate a string in the
        context of the specified object.
      operationId: evaluateExpression
      x-api-path-slug: actionevaluateexpression-get
      parameters:
      - in: query
        name: expression
        description: The expression to evaluate
        type: string
      - in: query
        name: objectId
        description: The ID of the object
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Expressions
  /?Action=GetPipelineDefinition:
    get:
      summary: Get Pipeline Definition
      description: Gets the definition of the specified pipeline.
      operationId: getPipelineDefinition
      x-api-path-slug: actiongetpipelinedefinition-get
      parameters:
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: version
        description: The version of the pipeline definition to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=ListPipelines:
    get:
      summary: List Pipelines
      description: Lists the pipeline identifiers for all active pipelines that you
        have permission to access.
      operationId: listPipelines
      x-api-path-slug: actionlistpipelines-get
      parameters:
      - in: query
        name: marker
        description: The starting point for the results to be returned
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=PollForTask:
    get:
      summary: Poll For Task
      description: Task runners call PollForTask to receive a task to perform from
        AWS Data Pipeline.
      operationId: pollForTask
      x-api-path-slug: actionpollfortask-get
      parameters:
      - in: query
        name: hostname
        description: The public DNS name of the calling task runner
        type: string
      - in: query
        name: instanceIdentity
        description: Identity information for the EC2 instance that is hosting the
          task runner
        type: string
      - in: query
        name: workerGroup
        description: The type of task the task runner is configured to accept and
          process
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=PutPipelineDefinition:
    get:
      summary: Put Pipeline Definition
      description: Adds tasks, schedules, and preconditions to the specified pipeline.
      operationId: putPipelineDefinition
      x-api-path-slug: actionputpipelinedefinition-get
      parameters:
      - in: query
        name: parameterObjects
        description: The parameter objects used with the pipeline
        type: string
      - in: query
        name: parameterValues
        description: The parameter values used with the pipeline
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: pipelineObjects
        description: The objects that define the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=QueryObjects:
    get:
      summary: Query Objects
      description: Queries the specified pipeline for the names of objects that match
        the specified set of conditions.
      operationId: queryObjects
      x-api-path-slug: actionqueryobjects-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of object names that QueryObjects will return
          in a single call
        type: string
      - in: query
        name: marker
        description: The starting point for the results to be returned
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: query
        description: The query that defines the objects to be returned
        type: string
      - in: query
        name: sphere
        description: Indicates whether the query applies to components or instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Objects
  /?Action=RemoveTags:
    get:
      summary: Remove Tags
      description: Removes existing tags from the specified pipeline.
      operationId: removeTags
      x-api-path-slug: actionremovetags-get
      parameters:
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: tagKeys
        description: The keys of the tags to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=ReportTaskProgress:
    get:
      summary: Report Task Progress
      description: Task runners call ReportTaskProgress when assigned a task to acknowledge
        that it has the task.
      operationId: reportTaskProgress
      x-api-path-slug: actionreporttaskprogress-get
      parameters:
      - in: query
        name: fields
        description: Key-value pairs that define the properties of the ReportTaskProgressInput
          object
        type: string
      - in: query
        name: taskId
        description: The ID of the task assigned to the task runner
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=ReportTaskRunnerHeartbeat:
    get:
      summary: Report Task Runner Heartbeat
      description: Task runners call ReportTaskRunnerHeartbeat every 15 minutes to
        indicate that they are operational.
      operationId: reportTaskRunnerHeartbeat
      x-api-path-slug: actionreporttaskrunnerheartbeat-get
      parameters:
      - in: query
        name: hostname
        description: The public DNS name of the task runner
        type: string
      - in: query
        name: taskrunnerId
        description: The ID of the task runner
        type: string
      - in: query
        name: workerGroup
        description: The type of task the task runner is configured to accept and
          process
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Runner Hearbeat
  /?Action=SetStatus:
    get:
      summary: Set Status
      description: Requests that the status of the specified physical or logical pipeline
        objects be updated in the specified pipeline.
      operationId: setStatus
      x-api-path-slug: actionsetstatus-get
      parameters:
      - in: query
        name: objectIds
        description: The IDs of the objects
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline that contains the objects
        type: string
      - in: query
        name: status
        description: The status to be set on all the objects specified in objectIds
        type: string
      responses:
        200:
          description: OK
      tags:
      - Status
  /?Action=SetTaskStatus:
    get:
      summary: Set Task Status
      description: Task runners call SetTaskStatus to notify AWS Data Pipeline that
        a task is completed and provide information about the final status.
      operationId: setTaskStatus
      x-api-path-slug: actionsettaskstatus-get
      parameters:
      - in: query
        name: errorId
        description: If an error occurred during the task, this value specifies the
          error code
        type: string
      - in: query
        name: errorMessage
        description: If an error occurred during the task, this value specifies a
          text description of the error
        type: string
      - in: query
        name: errorStackTrace
        description: If an error occurred during the task, this value specifies the
          stack trace associated with the error
        type: string
      - in: query
        name: taskId
        description: The ID of the task assigned to the task runner
        type: string
      - in: query
        name: taskStatus
        description: If FINISHED, the task successfully completed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=ValidatePipelineDefinition:
    get:
      summary: Validate Pipeline Definition
      description: Validates the specified pipeline definition to ensure that it is
        well formed and can be run without error.
      operationId: validatePipelineDefinition
      x-api-path-slug: actionvalidatepipelinedefinition-get
      parameters:
      - in: query
        name: parameterObjects
        description: The parameter objects used with the pipeline
        type: string
      - in: query
        name: parameterValues
        description: The parameter values used with the pipeline
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: pipelineObjects
        description: The objects that define the pipeline changes to validate against
          the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline