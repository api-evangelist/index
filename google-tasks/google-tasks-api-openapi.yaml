swagger: "2.0"
x-collection-name: Google Tasks
x-complete: 1
info:
  title: Tasks
  description: lets-you-manage-your-tasks-and-task-lists-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tasks/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lists/{tasklist}/clear:
    post:
      summary: Add Lists Task List Clear
      description: Clears all completed tasks from the specified task list. The affected
        tasks will be marked as 'hidden' and no longer be returned by default when
        retrieving all tasks for a task list.
      operationId: tasks.tasks.clear
      x-api-path-slug: liststasklistclear-post
      parameters:
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Task
      - List
      - Clear
  /lists/{tasklist}/tasks:
    get:
      summary: Get Lists Task List Tasks
      description: Returns all tasks in the specified task list.
      operationId: tasks.tasks.list
      x-api-path-slug: liststasklisttasks-get
      parameters:
      - in: query
        name: completedMax
        description: Upper bound for a tasks completion date (as a RFC 3339 timestamp)
          to filter by
      - in: query
        name: completedMin
        description: Lower bound for a tasks completion date (as a RFC 3339 timestamp)
          to filter by
      - in: query
        name: dueMax
        description: Upper bound for a tasks due date (as a RFC 3339 timestamp) to
          filter by
      - in: query
        name: dueMin
        description: Lower bound for a tasks due date (as a RFC 3339 timestamp) to
          filter by
      - in: query
        name: maxResults
        description: Maximum number of task lists returned on one page
      - in: query
        name: pageToken
        description: Token specifying the result page to return
      - in: query
        name: showCompleted
        description: Flag indicating whether completed tasks are returned in the result
      - in: query
        name: showDeleted
        description: Flag indicating whether deleted tasks are returned in the result
      - in: query
        name: showHidden
        description: Flag indicating whether hidden tasks are returned in the result
      - in: path
        name: tasklist
        description: Task list identifier
      - in: query
        name: updatedMin
        description: Lower bound for a tasks last modification time (as a RFC 3339
          timestamp) to filter by
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Task
      - List
      - Tasks
    post:
      summary: Add Lists Task List Tasks
      description: Creates a new task on the specified task list.
      operationId: tasks.tasks.insert
      x-api-path-slug: liststasklisttasks-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: parent
        description: Parent task identifier
      - in: query
        name: previous
        description: Previous sibling task identifier
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Task
      - List
      - Tasks
  /lists/{tasklist}/tasks/{task}:
    delete:
      summary: Delete Lists Task List Tasks Task
      description: Deletes the specified task from the task list.
      operationId: tasks.tasks.delete
      x-api-path-slug: liststasklisttaskstask-delete
      parameters:
      - in: path
        name: task
        description: Task identifier
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Task
      - List
      - Tasks
      - Task
    get:
      summary: Get Lists Task List Tasks Task
      description: Returns the specified task.
      operationId: tasks.tasks.get
      x-api-path-slug: liststasklisttaskstask-get
      parameters:
      - in: path
        name: task
        description: Task identifier
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Task
      - List
      - Tasks
      - Task
    patch:
      summary: Patch Lists Task List Tasks Task
      description: Updates the specified task. This method supports patch semantics.
      operationId: tasks.tasks.patch
      x-api-path-slug: liststasklisttaskstask-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: task
        description: Task identifier
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Task
      - List
      - Tasks
      - Task
    put:
      summary: Put Lists Task List Tasks Task
      description: Updates the specified task.
      operationId: tasks.tasks.update
      x-api-path-slug: liststasklisttaskstask-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: task
        description: Task identifier
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Task
      - List
      - Tasks
      - Task
  /lists/{tasklist}/tasks/{task}/move:
    post:
      summary: Add Lists Task List Tasks Task Move
      description: Moves the specified task to another position in the task list.
        This can include putting it as a child task under a new parent and/or move
        it to a different position among its sibling tasks.
      operationId: tasks.tasks.move
      x-api-path-slug: liststasklisttaskstaskmove-post
      parameters:
      - in: query
        name: parent
        description: New parent task identifier
      - in: query
        name: previous
        description: New previous sibling task identifier
      - in: path
        name: task
        description: Task identifier
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Task
      - List
      - Tasks
      - Task
      - Move
  /users/@me/lists:
    get:
      summary: Get Users @me Lists
      description: Returns all the authenticated user's task lists.
      operationId: tasks.tasklists.list
      x-api-path-slug: usersmelists-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of task lists returned on one page
      - in: query
        name: pageToken
        description: Token specifying the result page to return
      responses:
        200:
          description: OK
      tags:
      - Users
      - '@me'
      - Lists
    post:
      summary: Add Users @me Lists
      description: Creates a new task list and adds it to the authenticated user's
        task lists.
      operationId: tasks.tasklists.insert
      x-api-path-slug: usersmelists-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
      - '@me'
      - Lists
  /users/@me/lists/{tasklist}:
    delete:
      summary: Delete Users Task List
      description: Deletes the authenticated user's specified task list.
      operationId: tasks.tasklists.delete
      x-api-path-slug: usersmeliststasklist-delete
      parameters:
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Users
      - Task
      - List
    get:
      summary: Get Users Task List
      description: Returns the authenticated user's specified task list.
      operationId: tasks.tasklists.get
      x-api-path-slug: usersmeliststasklist-get
      parameters:
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Users
      - Task
      - List
    patch:
      summary: Patch Users Task List
      description: Updates the authenticated user's specified task list. This method
        supports patch semantics.
      operationId: tasks.tasklists.patch
      x-api-path-slug: usersmeliststasklist-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Users
      - Task
      - List
    put:
      summary: Put Users Task List
      description: Updates the authenticated user's specified task list.
      operationId: tasks.tasklists.update
      x-api-path-slug: usersmeliststasklist-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Users
      - Task
      - List