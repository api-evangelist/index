swagger: "2.0"
x-collection-name: Google Cloud Spanner
x-complete: 1
info:
  title: Cloud Spanner
  description: cloud-spanner-is-a-managed-missioncritical-globally-consistent-and-scalable-relational-database-service-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: spanner.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{database}:
    delete:
      summary: Delete Database
      description: Drops (aka deletes) a Cloud Spanner database.
      operationId: spanner.projects.instances.databases.dropDatabase
      x-api-path-slug: v1database-delete
      parameters:
      - in: path
        name: database
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Database
  /v1/{database}/ddl:
    get:
      summary: Get Database Schema
      description: |-
        Returns the schema of a Cloud Spanner database as a list of formatted
        DDL statements. This method does not show pending schema updates, those may
        be queried using the Operations API.
      operationId: spanner.projects.instances.databases.getDdl
      x-api-path-slug: v1databaseddl-get
      parameters:
      - in: path
        name: database
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Database Schema
    patch:
      summary: Update Database Schema
      description: |-
        Updates the schema of a Cloud Spanner database by
        creating/altering/dropping tables, columns, indexes, etc. The returned
        long-running operation will have a name of
        the format `<database_name>/operations/<operation_id>` and can be used to
        track execution of the schema change(s). The
        metadata field type is
        UpdateDatabaseDdlMetadata.  The operation has no response.
      operationId: spanner.projects.instances.databases.updateDdl
      x-api-path-slug: v1databaseddl-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: database
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Database Schema
  /v1/{database}/sessions:
    post:
      summary: Create Session
      description: |-
        Creates a new session. A session can be used to perform
        transactions that read and/or modify data in a Cloud Spanner database.
        Sessions are meant to be reused for many consecutive
        transactions.

        Sessions can only execute one transaction at a time. To execute
        multiple concurrent read-write/write-only transactions, create
        multiple sessions. Note that standalone reads and queries use a
        transaction internally, and count toward the one transaction
        limit.

        Cloud Spanner limits the number of sessions that can exist at any given
        time; thus, it is a good idea to delete idle and/or unneeded sessions.
        Aside from explicit deletes, Cloud Spanner can delete sessions for
        which no operations are sent for more than an hour, or due to
        internal errors. If a session is deleted, requests to it
        return `NOT_FOUND`.

        Idle sessions can be kept alive by sending a trivial SQL query
        periodically, e.g., `"SELECT 1"`.
      operationId: spanner.projects.instances.databases.sessions.create
      x-api-path-slug: v1databasesessions-post
      parameters:
      - in: path
        name: database
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Session
  /v1/{name}:
    delete:
      summary: End Session
      description: Ends a session, releasing server resources associated with it.
      operationId: spanner.projects.instances.databases.sessions.delete
      x-api-path-slug: v1name-delete
      parameters:
      - in: path
        name: name
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Session
    get:
      summary: Get Session
      description: |-
        Gets a session. Returns `NOT_FOUND` if the session does not exist.
        This is mainly useful for determining whether a session is still
        alive.
      operationId: spanner.projects.instances.databases.sessions.get
      x-api-path-slug: v1name-get
      parameters:
      - in: path
        name: name
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Session
    patch:
      summary: Update Instance
      description: |-
        Updates an instance, and begins allocating or releasing resources
        as requested. The returned long-running
        operation can be used to track the
        progress of updating the instance. If the named instance does not
        exist, returns `NOT_FOUND`.

        Immediately upon completion of this request:

          * For resource types for which a decrease in the instance's allocation
            has been requested, billing is based on the newly-requested level.

        Until completion of the returned operation:

          * Cancelling the operation sets its metadata's
            cancel_time, and begins
            restoring resources to their pre-request values. The operation
            is guaranteed to succeed at undoing all resource changes,
            after which point it terminates with a `CANCELLED` status.
          * All other attempts to modify the instance are rejected.
          * Reading the instance via the API continues to give the pre-request
            resource levels.

        Upon completion of the returned operation:

          * Billing begins for all successfully-allocated resources (some types
            may have lower than the requested levels).
          * All newly-reserved resources are available for serving the instance's
            tables.
          * The instance's new resource levels are readable via the API.

        The returned long-running operation will
        have a name of the format `<instance_name>/operations/<operation_id>` and
        can be used to track the instance modification.  The
        metadata field type is
        UpdateInstanceMetadata.
        The response field type is
        Instance, if successful.

        Authorization requires `spanner.instances.update` permission on
        resource name.
      operationId: spanner.projects.instances.patch
      x-api-path-slug: v1name-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Instance
  /v1/{name}:cancel:
    post:
      summary: Cancel Instance
      description: |-
        Starts asynchronous cancellation on a long-running operation.  The server
        makes a best effort to cancel the operation, but success is not
        guaranteed.  If the server doesn't support this method, it returns
        `google.rpc.Code.UNIMPLEMENTED`.  Clients can use
        Operations.GetOperation or
        other methods to check whether the cancellation succeeded or whether the
        operation completed despite cancellation. On successful cancellation,
        the operation is not deleted; instead, it becomes an operation with
        an Operation.error value with a google.rpc.Status.code of 1,
        corresponding to `Code.CANCELLED`.
      operationId: spanner.projects.instances.databases.operations.cancel
      x-api-path-slug: v1namecancel-post
      parameters:
      - in: path
        name: name
        description: The name of the operation resource to be cancelled
      responses:
        200:
          description: OK
      tags:
      - Instance
  /v1/{parent}/databases:
    get:
      summary: Get Databases
      description: Lists Cloud Spanner databases.
      operationId: spanner.projects.instances.databases.list
      x-api-path-slug: v1parentdatabases-get
      parameters:
      - in: query
        name: pageSize
        description: Number of databases to be returned in the response
      - in: query
        name: pageToken
        description: If non-empty, `page_token` should contain anext_page_token from
          aprevious ListDatabasesResponse
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Database
    post:
      summary: Create Database
      description: |-
        Creates a new Cloud Spanner database and starts to prepare it for serving.
        The returned long-running operation will
        have a name of the format `<database_name>/operations/<operation_id>` and
        can be used to track preparation of the database. The
        metadata field type is
        CreateDatabaseMetadata. The
        response field type is
        Database, if successful.
      operationId: spanner.projects.instances.databases.create
      x-api-path-slug: v1parentdatabases-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Database
  /v1/{parent}/instanceConfigs:
    get:
      summary: Get Instance Configurations
      description: Lists the supported instance configurations for a given project.
      operationId: spanner.projects.instanceConfigs.list
      x-api-path-slug: v1parentinstanceconfigs-get
      parameters:
      - in: query
        name: pageSize
        description: Number of instance configurations to be returned in the response
      - in: query
        name: pageToken
        description: If non-empty, `page_token` should contain anext_page_tokenfrom
          a previous ListInstanceConfigsResponse
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Instance
  /v1/{parent}/instances:
    get:
      summary: Get Instances
      description: Lists all instances in the given project.
      operationId: spanner.projects.instances.list
      x-api-path-slug: v1parentinstances-get
      parameters:
      - in: query
        name: filter
        description: An expression for filtering the results of the request
      - in: query
        name: pageSize
        description: Number of instances to be returned in the response
      - in: query
        name: pageToken
        description: If non-empty, `page_token` should contain anext_page_token from
          aprevious ListInstancesResponse
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Instance
    post:
      summary: Create instance
      description: |-
        Creates an instance and begins preparing it to begin serving. The
        returned long-running operation
        can be used to track the progress of preparing the new
        instance. The instance name is assigned by the caller. If the
        named instance already exists, `CreateInstance` returns
        `ALREADY_EXISTS`.

        Immediately upon completion of this request:

          * The instance is readable via the API, with all requested attributes
            but no allocated resources. Its state is `CREATING`.

        Until completion of the returned operation:

          * Cancelling the operation renders the instance immediately unreadable
            via the API.
          * The instance can be deleted.
          * All other attempts to modify the instance are rejected.

        Upon completion of the returned operation:

          * Billing for all successfully-allocated resources begins (some types
            may have lower than the requested levels).
          * Databases can be created in the instance.
          * The instance's allocated resource levels are readable via the API.
          * The instance's state becomes `READY`.

        The returned long-running operation will
        have a name of the format `<instance_name>/operations/<operation_id>` and
        can be used to track creation of the instance.  The
        metadata field type is
        CreateInstanceMetadata.
        The response field type is
        Instance, if successful.
      operationId: spanner.projects.instances.create
      x-api-path-slug: v1parentinstances-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Instance
  /v1/{resource}:getIamPolicy:
    post:
      summary: Get IAM Policy
      description: |-
        Gets the access control policy for a database resource. Returns an empty
        policy if a database exists but does not have a policy set.

        Authorization requires `spanner.databases.getIamPolicy` permission on
        resource.
      operationId: spanner.projects.instances.databases.getIamPolicy
      x-api-path-slug: v1resourcegetiampolicy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The Cloud Spanner resource for which the policy is
          being retrieved'
      responses:
        200:
          description: OK
      tags:
      - IAM
  /v1/{resource}:setIamPolicy:
    post:
      summary: Set IAM Policy
      description: |-
        Sets the access control policy on a database resource. Replaces any
        existing policy.

        Authorization requires `spanner.databases.setIamPolicy` permission on
        resource.
      operationId: spanner.projects.instances.databases.setIamPolicy
      x-api-path-slug: v1resourcesetiampolicy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The Cloud Spanner resource for which the policy is
          being set'
      responses:
        200:
          description: OK
      tags:
      - IAM
  /v1/{resource}:testIamPermissions:
    post:
      summary: Test IAM Permissions
      description: |-
        Returns permissions that the caller has on the specified database resource.

        Attempting this RPC on a non-existent Cloud Spanner database will result in
        a NOT_FOUND error if the user has `spanner.databases.list` permission on
        the containing Cloud Spanner instance. Otherwise returns an empty set of
        permissions.
      operationId: spanner.projects.instances.databases.testIamPermissions
      x-api-path-slug: v1resourcetestiampermissions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The Cloud Spanner resource for which permissions are
          being tested'
      responses:
        200:
          description: OK
      tags:
      - IAM
  /v1/{session}:beginTransaction:
    post:
      summary: Begin Transaction
      description: |-
        Begins a new transaction. This step can often be skipped:
        Read, ExecuteSql and
        Commit can begin a new transaction as a
        side-effect.
      operationId: spanner.projects.instances.databases.sessions.beginTransaction
      x-api-path-slug: v1sessionbegintransaction-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: session
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Transaction
  /v1/{session}:commit:
    post:
      summary: Commit Transaction
      description: |-
        Commits a transaction. The request includes the mutations to be
        applied to rows in the database.

        `Commit` might return an `ABORTED` error. This can occur at any time;
        commonly, the cause is conflicts with concurrent
        transactions. However, it can also happen for a variety of other
        reasons. If `Commit` returns `ABORTED`, the caller should re-attempt
        the transaction from the beginning, re-using the same session.
      operationId: spanner.projects.instances.databases.sessions.commit
      x-api-path-slug: v1sessioncommit-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: session
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Transaction
  /v1/{session}:executeSql:
    post:
      summary: Execute SQL
      description: |-
        Executes an SQL query, returning all rows in a single reply. This
        method cannot be used to return a result set larger than 10 MiB;
        if the query yields more data than that, the query fails with
        a `FAILED_PRECONDITION` error.

        Queries inside read-write transactions might return `ABORTED`. If
        this occurs, the application should restart the transaction from
        the beginning. See Transaction for more details.

        Larger result sets can be fetched in streaming fashion by calling
        ExecuteStreamingSql instead.
      operationId: spanner.projects.instances.databases.sessions.executeSql
      x-api-path-slug: v1sessionexecutesql-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: session
        description: Required
      responses:
        200:
          description: OK
      tags:
      - SQL
  /v1/{session}:executeStreamingSql:
    post:
      summary: Execute Streaming SQL
      description: |-
        Like ExecuteSql, except returns the result
        set as a stream. Unlike ExecuteSql, there
        is no limit on the size of the returned result set. However, no
        individual row in the result set can exceed 100 MiB, and no
        column value can exceed 10 MiB.
      operationId: spanner.projects.instances.databases.sessions.executeStreamingSql
      x-api-path-slug: v1sessionexecutestreamingsql-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: session
        description: Required
      responses:
        200:
          description: OK
      tags:
      - SQL
  /v1/{session}:read:
    post:
      summary: Read Rows
      description: |-
        Reads rows from the database using key lookups and scans, as a
        simple key/value style alternative to
        ExecuteSql.  This method cannot be used to
        return a result set larger than 10 MiB; if the read matches more
        data than that, the read fails with a `FAILED_PRECONDITION`
        error.

        Reads inside read-write transactions might return `ABORTED`. If
        this occurs, the application should restart the transaction from
        the beginning. See Transaction for more details.

        Larger result sets can be yielded in streaming fashion by calling
        StreamingRead instead.
      operationId: spanner.projects.instances.databases.sessions.read
      x-api-path-slug: v1sessionread-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: session
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Row
  /v1/{session}:rollback:
    post:
      summary: Rollback Transaction
      description: |-
        Rolls back a transaction, releasing any locks it holds. It is a good
        idea to call this for any transaction that includes one or more
        Read or ExecuteSql requests and
        ultimately decides not to commit.

        `Rollback` returns `OK` if it successfully aborts the transaction, the
        transaction was already aborted, or the transaction is not
        found. `Rollback` never returns `ABORTED`.
      operationId: spanner.projects.instances.databases.sessions.rollback
      x-api-path-slug: v1sessionrollback-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: session
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Transaction
  /v1/{session}:streamingRead:
    post:
      summary: Streaming Read
      description: |-
        Like Read, except returns the result set as a
        stream. Unlike Read, there is no limit on the
        size of the returned result set. However, no individual row in
        the result set can exceed 100 MiB, and no column value can exceed
        10 MiB.
      operationId: spanner.projects.instances.databases.sessions.streamingRead
      x-api-path-slug: v1sessionstreamingread-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: session
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Streaming