swagger: "2.0"
x-collection-name: Google Task Queue
x-complete: 1
info:
  title: TaskQueue
  description: accesses-a-google-app-engine-pull-task-queue-over-rest-
  contact:
    name: Google
    url: https://google.com
  version: v1beta2
host: www.googleapis.com
basePath: /taskqueue/v1beta2/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/taskqueues/{taskqueue}:
    get:
      summary: Get Task Queues
      description: Get detailed information about a TaskQueue.
      operationId: taskqueue.taskqueues.get
      x-api-path-slug: projecttaskqueuestaskqueue-get
      parameters:
      - in: query
        name: getStats
        description: Whether to get stats
      - in: path
        name: project
        description: The project under which the queue lies
      - in: path
        name: taskqueue
        description: The id of the taskqueue to get the properties of
      responses:
        200:
          description: OK
      tags:
      - Task Queues
  /{project}/taskqueues/{taskqueue}/tasks:
    get:
      summary: Get Tasks
      description: List Tasks in a TaskQueue
      operationId: taskqueue.tasks.list
      x-api-path-slug: projecttaskqueuestaskqueuetasks-get
      parameters:
      - in: path
        name: project
        description: The project under which the queue lies
      - in: path
        name: taskqueue
        description: The id of the taskqueue to list tasks from
      responses:
        200:
          description: OK
      tags:
      - Task
    post:
      summary: Insert Task
      description: Insert a new task in a TaskQueue
      operationId: taskqueue.tasks.insert
      x-api-path-slug: projecttaskqueuestaskqueuetasks-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: The project under which the queue lies
      - in: path
        name: taskqueue
        description: The taskqueue to insert the task into
      responses:
        200:
          description: OK
      tags:
      - Task
  /{project}/taskqueues/{taskqueue}/tasks/lease:
    post:
      summary: Lease Task
      description: Lease 1 or more tasks from a TaskQueue.
      operationId: taskqueue.tasks.lease
      x-api-path-slug: projecttaskqueuestaskqueuetaskslease-post
      parameters:
      - in: query
        name: groupByTag
        description: When true, all returned tasks will have the same tag
      - in: query
        name: leaseSecs
        description: The lease in seconds
      - in: query
        name: numTasks
        description: The number of tasks to lease
      - in: path
        name: project
        description: The project under which the queue lies
      - in: query
        name: tag
        description: The tag allowed for tasks in the response
      - in: path
        name: taskqueue
        description: The taskqueue to lease a task from
      responses:
        200:
          description: OK
      tags:
      - Task
  /{project}/taskqueues/{taskqueue}/tasks/{task}:
    delete:
      summary: Delete Task
      description: Delete a task from a TaskQueue.
      operationId: taskqueue.tasks.delete
      x-api-path-slug: projecttaskqueuestaskqueuetaskstask-delete
      parameters:
      - in: path
        name: project
        description: The project under which the queue lies
      - in: path
        name: task
        description: The id of the task to delete
      - in: path
        name: taskqueue
        description: The taskqueue to delete a task from
      responses:
        200:
          description: OK
      tags:
      - Task
    get:
      summary: Get Task
      description: Get a particular task from a TaskQueue.
      operationId: taskqueue.tasks.get
      x-api-path-slug: projecttaskqueuestaskqueuetaskstask-get
      parameters:
      - in: path
        name: project
        description: The project under which the queue lies
      - in: path
        name: task
        description: The task to get properties of
      - in: path
        name: taskqueue
        description: The taskqueue in which the task belongs
      responses:
        200:
          description: OK
      tags:
      - Task
    patch:
      summary: Update Task
      description: Update tasks that are leased out of a TaskQueue. This method supports
        patch semantics.
      operationId: taskqueue.tasks.patch
      x-api-path-slug: projecttaskqueuestaskqueuetaskstask-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: newLeaseSeconds
        description: The new lease in seconds
      - in: path
        name: project
        description: The project under which the queue lies
      - in: path
        name: task
      - in: path
        name: taskqueue
      responses:
        200:
          description: OK
      tags:
      - Task
    post:
      summary: Update Task
      description: Update tasks that are leased out of a TaskQueue.
      operationId: taskqueue.tasks.update
      x-api-path-slug: projecttaskqueuestaskqueuetaskstask-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: newLeaseSeconds
        description: The new lease in seconds
      - in: path
        name: project
        description: The project under which the queue lies
      - in: path
        name: task
      - in: path
        name: taskqueue
      responses:
        200:
          description: OK
      tags:
      - Task