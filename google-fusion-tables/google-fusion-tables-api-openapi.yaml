swagger: "2.0"
x-collection-name: Google Fusion Tables
x-complete: 1
info:
  title: Fusion Tables
  description: api-for-working-with-fusion-tables-data-
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /fusiontables/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /query:
    get:
      summary: Execute SQL Statement
      description: "Executes a SQL statement which can be any of \n- SELECT\n- SHOW\n-
        DESCRIBE"
      operationId: fusiontables.query.sqlGet
      x-api-path-slug: query-get
      parameters:
      - in: query
        name: hdrs
        description: Whether column names are included (in the first row)
      - in: query
        name: sql
        description: A SQL statement which can be any of - SELECT- SHOW- DESCRIBE
      - in: query
        name: typed
        description: 'Whether typed values are returned in the (JSON) response: numbers
          for numeric values and parsed geometries for KML values'
      responses:
        200:
          description: OK
      tags:
      - Query
    post:
      summary: Execute Fusion Table SQL Statement
      description: "Executes a Fusion Tables SQL statement, which can be any of \n-
        SELECT\n- INSERT\n- UPDATE\n- DELETE\n- SHOW\n- DESCRIBE\n- CREATE statement."
      operationId: fusiontables.query.sql
      x-api-path-slug: query-post
      parameters:
      - in: query
        name: hdrs
        description: Whether column names are included in the first row
      - in: query
        name: sql
        description: A Fusion Tables SQL statement, which can be any of - SELECT-
          INSERT- UPDATE- DELETE- SHOW- DESCRIBE- CREATE
      - in: query
        name: typed
        description: 'Whether typed values are returned in the (JSON) response: numbers
          for numeric values and parsed geometries for KML values'
      responses:
        200:
          description: OK
      tags:
      - Query
  /tables:
    get:
      summary: Get Tables
      description: Retrieves a list of tables a user owns.
      operationId: fusiontables.table.list
      x-api-path-slug: tables-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of tables to return
      - in: query
        name: pageToken
        description: Continuation token specifying which result page to return
      responses:
        200:
          description: OK
      tags:
      - Table
    post:
      summary: Create Table
      description: Creates a new table.
      operationId: fusiontables.table.insert
      x-api-path-slug: tables-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Table
  /tables/import:
    post:
      summary: Import Table
      description: Imports a new table.
      operationId: fusiontables.table.importTable
      x-api-path-slug: tablesimport-post
      parameters:
      - in: query
        name: delimiter
        description: The delimiter used to separate cell values
      - in: query
        name: encoding
        description: The encoding of the content
      - in: query
        name: name
        description: The name to be assigned to the new table
      responses:
        200:
          description: OK
      tags:
      - Table
  /tables/{tableId}:
    delete:
      summary: Delete Table
      description: Deletes a table.
      operationId: fusiontables.table.delete
      x-api-path-slug: tablestableid-delete
      parameters:
      - in: path
        name: tableId
        description: ID of the table to be deleted
      responses:
        200:
          description: OK
      tags:
      - Table
    get:
      summary: Get Table
      description: Retrieves a specific table by its ID.
      operationId: fusiontables.table.get
      x-api-path-slug: tablestableid-get
      parameters:
      - in: path
        name: tableId
        description: Identifier for the table being requested
      responses:
        200:
          description: OK
      tags:
      - Table
    patch:
      summary: Update Table
      description: Updates an existing table. Unless explicitly requested, only the
        name, description, and attribution will be updated. This method supports patch
        semantics.
      operationId: fusiontables.table.patch
      x-api-path-slug: tablestableid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: replaceViewDefinition
        description: Whether the view definition is also updated
      - in: path
        name: tableId
        description: ID of the table that is being updated
      responses:
        200:
          description: OK
      tags:
      - Table
    put:
      summary: Update Table
      description: Updates an existing table. Unless explicitly requested, only the
        name, description, and attribution will be updated.
      operationId: fusiontables.table.update
      x-api-path-slug: tablestableid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: replaceViewDefinition
        description: Whether the view definition is also updated
      - in: path
        name: tableId
        description: ID of the table that is being updated
      responses:
        200:
          description: OK
      tags:
      - Table
  /tables/{tableId}/columns:
    get:
      summary: Get Columns
      description: Retrieves a list of columns.
      operationId: fusiontables.column.list
      x-api-path-slug: tablestableidcolumns-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of columns to return
      - in: query
        name: pageToken
        description: Continuation token specifying which result page to return
      - in: path
        name: tableId
        description: Table whose columns are being listed
      responses:
        200:
          description: OK
      tags:
      - Column
    post:
      summary: Add Column
      description: Adds a new column to the table.
      operationId: fusiontables.column.insert
      x-api-path-slug: tablestableidcolumns-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tableId
        description: Table for which a new column is being added
      responses:
        200:
          description: OK
      tags:
      - Column
  /tables/{tableId}/columns/{columnId}:
    delete:
      summary: Delete Column
      description: Deletes the specified column.
      operationId: fusiontables.column.delete
      x-api-path-slug: tablestableidcolumnscolumnid-delete
      parameters:
      - in: path
        name: columnId
        description: Name or identifier for the column being deleted
      - in: path
        name: tableId
        description: Table from which the column is being deleted
      responses:
        200:
          description: OK
      tags:
      - Column
    get:
      summary: Get Column
      description: Retrieves a specific column by its ID.
      operationId: fusiontables.column.get
      x-api-path-slug: tablestableidcolumnscolumnid-get
      parameters:
      - in: path
        name: columnId
        description: Name or identifier for the column that is being requested
      - in: path
        name: tableId
        description: Table to which the column belongs
      responses:
        200:
          description: OK
      tags:
      - Column
    patch:
      summary: Update Column
      description: Updates the name or type of an existing column. This method supports
        patch semantics.
      operationId: fusiontables.column.patch
      x-api-path-slug: tablestableidcolumnscolumnid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: columnId
        description: Name or identifier for the column that is being updated
      - in: path
        name: tableId
        description: Table for which the column is being updated
      responses:
        200:
          description: OK
      tags:
      - Column
    put:
      summary: Update Column
      description: Updates the name or type of an existing column.
      operationId: fusiontables.column.update
      x-api-path-slug: tablestableidcolumnscolumnid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: columnId
        description: Name or identifier for the column that is being updated
      - in: path
        name: tableId
        description: Table for which the column is being updated
      responses:
        200:
          description: OK
      tags:
      - Column
  /tables/{tableId}/copy:
    post:
      summary: Copy Table
      description: Copies a table.
      operationId: fusiontables.table.copy
      x-api-path-slug: tablestableidcopy-post
      parameters:
      - in: query
        name: copyPresentation
        description: Whether to also copy tabs, styles, and templates
      - in: path
        name: tableId
        description: ID of the table that is being copied
      responses:
        200:
          description: OK
      tags:
      - Table
  /tables/{tableId}/import:
    post:
      summary: import Rows
      description: Imports more rows into a table.
      operationId: fusiontables.table.importRows
      x-api-path-slug: tablestableidimport-post
      parameters:
      - in: query
        name: delimiter
        description: The delimiter used to separate cell values
      - in: query
        name: encoding
        description: The encoding of the content
      - in: query
        name: endLine
        description: The index of the line up to which data will be imported
      - in: query
        name: isStrict
        description: Whether the imported CSV must have the same number of values
          for each row
      - in: query
        name: startLine
        description: The index of the first line from which to start importing, inclusive
      - in: path
        name: tableId
        description: The table into which new rows are being imported
      responses:
        200:
          description: OK
      tags:
      - Table
  /tables/{tableId}/replace:
    post:
      summary: Replace Rows
      description: Replaces rows of an existing table. Current rows remain visible
        until all replacement rows are ready.
      operationId: fusiontables.table.replaceRows
      x-api-path-slug: tablestableidreplace-post
      parameters:
      - in: query
        name: delimiter
        description: The delimiter used to separate cell values
      - in: query
        name: encoding
        description: The encoding of the content
      - in: query
        name: endLine
        description: The index of the line up to which data will be imported
      - in: query
        name: isStrict
        description: Whether the imported CSV must have the same number of column
          values for each row
      - in: query
        name: startLine
        description: The index of the first line from which to start importing, inclusive
      - in: path
        name: tableId
        description: Table whose rows will be replaced
      responses:
        200:
          description: OK
      tags:
      - Table
  /tables/{tableId}/styles:
    get:
      summary: Get Styels
      description: Retrieves a list of styles.
      operationId: fusiontables.style.list
      x-api-path-slug: tablestableidstyles-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of styles to return
      - in: query
        name: pageToken
        description: Continuation token specifying which result page to return
      - in: path
        name: tableId
        description: Table whose styles are being listed
      responses:
        200:
          description: OK
      tags:
      - Table Style
    post:
      summary: Create Style
      description: Adds a new style for the table.
      operationId: fusiontables.style.insert
      x-api-path-slug: tablestableidstyles-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tableId
        description: Table for which a new style is being added
      responses:
        200:
          description: OK
      tags:
      - Table Style
  /tables/{tableId}/styles/{styleId}:
    delete:
      summary: Delete Style
      description: Deletes a style.
      operationId: fusiontables.style.delete
      x-api-path-slug: tablestableidstylesstyleid-delete
      parameters:
      - in: path
        name: styleId
        description: Identifier (within a table) for the style being deleted
      - in: path
        name: tableId
        description: Table from which the style is being deleted
      responses:
        200:
          description: OK
      tags:
      - Table Style
    get:
      summary: DelGetete Style
      description: Gets a specific style.
      operationId: fusiontables.style.get
      x-api-path-slug: tablestableidstylesstyleid-get
      parameters:
      - in: path
        name: styleId
        description: Identifier (integer) for a specific style in a table
      - in: path
        name: tableId
        description: Table to which the requested style belongs
      responses:
        200:
          description: OK
      tags:
      - Table Style
    patch:
      summary: Update Style
      description: Updates an existing style. This method supports patch semantics.
      operationId: fusiontables.style.patch
      x-api-path-slug: tablestableidstylesstyleid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: styleId
        description: Identifier (within a table) for the style being updated
      - in: path
        name: tableId
        description: Table whose style is being updated
      responses:
        200:
          description: OK
      tags:
      - Table Style
    put:
      summary: Update Style
      description: Updates an existing style.
      operationId: fusiontables.style.update
      x-api-path-slug: tablestableidstylesstyleid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: styleId
        description: Identifier (within a table) for the style being updated
      - in: path
        name: tableId
        description: Table whose style is being updated
      responses:
        200:
          description: OK
      tags:
      - Table Style
  /tables/{tableId}/tasks:
    get:
      summary: Get Tasks
      description: Retrieves a list of tasks.
      operationId: fusiontables.task.list
      x-api-path-slug: tablestableidtasks-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of tasks to return
      - in: query
        name: pageToken
        description: Continuation token specifying which result page to return
      - in: query
        name: startIndex
        description: Index of the first result returned in the current page
      - in: path
        name: tableId
        description: Table whose tasks are being listed
      responses:
        200:
          description: OK
      tags:
      - Task
  /tables/{tableId}/tasks/{taskId}:
    delete:
      summary: Delete Task
      description: Deletes a specific task by its ID, unless that task has already
        started running.
      operationId: fusiontables.task.delete
      x-api-path-slug: tablestableidtaskstaskid-delete
      parameters:
      - in: path
        name: tableId
        description: Table from which the task is being deleted
      - in: path
        name: taskId
        description: The identifier of the task to delete
      responses:
        200:
          description: OK
      tags:
      - Task
    get:
      summary: Get Task
      description: Retrieves a specific task by its ID.
      operationId: fusiontables.task.get
      x-api-path-slug: tablestableidtaskstaskid-get
      parameters:
      - in: path
        name: tableId
        description: Table to which the task belongs
      - in: path
        name: taskId
        description: The identifier of the task to get
      responses:
        200:
          description: OK
      tags:
      - Task
  /tables/{tableId}/templates:
    get:
      summary: Get Templates
      description: Retrieves a list of templates.
      operationId: fusiontables.template.list
      x-api-path-slug: tablestableidtemplates-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of templates to return
      - in: query
        name: pageToken
        description: Continuation token specifying which results page to return
      - in: path
        name: tableId
        description: Identifier for the table whose templates are being requested
      responses:
        200:
          description: OK
      tags:
      - Template
    post:
      summary: Create Template
      description: Creates a new template for the table.
      operationId: fusiontables.template.insert
      x-api-path-slug: tablestableidtemplates-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tableId
        description: Table for which a new template is being created
      responses:
        200:
          description: OK
      tags:
      - Template
  /tables/{tableId}/templates/{templateId}:
    delete:
      summary: Delete Template
      description: Deletes a template
      operationId: fusiontables.template.delete
      x-api-path-slug: tablestableidtemplatestemplateid-delete
      parameters:
      - in: path
        name: tableId
        description: Table from which the template is being deleted
      - in: path
        name: templateId
        description: Identifier for the template which is being deleted
      responses:
        200:
          description: OK
      tags:
      - Template
    get:
      summary: Get Template
      description: Retrieves a specific template by its id
      operationId: fusiontables.template.get
      x-api-path-slug: tablestableidtemplatestemplateid-get
      parameters:
      - in: path
        name: tableId
        description: Table to which the template belongs
      - in: path
        name: templateId
        description: Identifier for the template that is being requested
      responses:
        200:
          description: OK
      tags:
      - Template
    patch:
      summary: Update Template
      description: Updates an existing template. This method supports patch semantics.
      operationId: fusiontables.template.patch
      x-api-path-slug: tablestableidtemplatestemplateid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tableId
        description: Table to which the updated template belongs
      - in: path
        name: templateId
        description: Identifier for the template that is being updated
      responses:
        200:
          description: OK
      tags:
      - Template
    put:
      summary: Update Template
      description: Updates an existing template
      operationId: fusiontables.template.update
      x-api-path-slug: tablestableidtemplatestemplateid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tableId
        description: Table to which the updated template belongs
      - in: path
        name: templateId
        description: Identifier for the template that is being updated
      responses:
        200:
          description: OK
      tags:
      - Template