swagger: "2.0"
x-collection-name: Google Cloud SQL
x-complete: 1
info:
  title: Cloud SQL Administration
  description: creates-and-configures-cloud-sql-instances-which-provide-fullymanaged-mysql-databases-
  contact:
    name: Google
    url: https://google.com
  version: v1beta4
host: www.googleapis.com
basePath: /sql/v1beta4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /flags:
    get:
      summary: Get Flags
      description: List all available database flags for Google Cloud SQL instances.
      operationId: sql.flags.list
      x-api-path-slug: flags-get
      parameters:
      - in: query
        name: databaseVersion
        description: Database version for flag retrieval
      responses:
        200:
          description: OK
      tags:
      - Flags
  /projects/{project}/instances:
    get:
      summary: Get Projects Project Instances
      description: Lists instances under a given project in the alphabetical order
        of the instance name.
      operationId: sql.instances.list
      x-api-path-slug: projectsprojectinstances-get
      parameters:
      - in: query
        name: filter
        description: A filter expression for filtering listed instances
      - in: query
        name: maxResults
        description: The maximum number of results to return per response
      - in: query
        name: pageToken
        description: A previously-returned page token representing part of the larger
          set of results to view
      - in: path
        name: project
        description: Project ID of the project for which to list Cloud SQL instances
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
    post:
      summary: Add Projects Project Instances
      description: Creates a new Cloud SQL instance.
      operationId: sql.instances.insert
      x-api-path-slug: projectsprojectinstances-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID of the project to which the newly created Cloud SQL
          instances should belong
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
  /projects/{project}/instances/{instance}:
    delete:
      summary: Delete Projects Project Instances Instance
      description: Deletes a Cloud SQL instance.
      operationId: sql.instances.delete
      x-api-path-slug: projectsprojectinstancesinstance-delete
      parameters:
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance to be deleted
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
    get:
      summary: Get Projects Project Instances Instance
      description: Retrieves a resource containing information about a Cloud SQL instance.
      operationId: sql.instances.get
      x-api-path-slug: projectsprojectinstancesinstance-get
      parameters:
      - in: path
        name: instance
        description: Database instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
    patch:
      summary: Patch Projects Project Instances Instance
      description: 'Updates settings of a Cloud SQL instance. Caution: This is not
        a partial update, so you must include values for all the settings that you
        want to retain. For partial updates, use patch.. This method supports patch
        semantics.'
      operationId: sql.instances.patch
      x-api-path-slug: projectsprojectinstancesinstance-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
    put:
      summary: Put Projects Project Instances Instance
      description: 'Updates settings of a Cloud SQL instance. Caution: This is not
        a partial update, so you must include values for all the settings that you
        want to retain. For partial updates, use patch.'
      operationId: sql.instances.update
      x-api-path-slug: projectsprojectinstancesinstance-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Put
      - Projects
      - Project
      - Instances
      - Instance
  /projects/{project}/instances/{instance}/backupRuns:
    get:
      summary: Get Projects Project Instances Instance Backupruns
      description: Lists all backup runs associated with a given instance and configuration
        in the reverse chronological order of the enqueued time.
      operationId: sql.backupRuns.list
      x-api-path-slug: projectsprojectinstancesinstancebackupruns-get
      parameters:
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: query
        name: maxResults
        description: Maximum number of backup runs per response
      - in: query
        name: pageToken
        description: A previously-returned page token representing part of the larger
          set of results to view
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Backupruns
    post:
      summary: Add Projects Project Instances Instance Backupruns
      description: Creates a new backup run on demand. This method is applicable only
        to Second Generation instances.
      operationId: sql.backupRuns.insert
      x-api-path-slug: projectsprojectinstancesinstancebackupruns-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Backupruns
  /projects/{project}/instances/{instance}/backupRuns/{id}:
    delete:
      summary: Delete Projects Project Instances Instance Backupruns
      description: Deletes the backup taken by a backup run.
      operationId: sql.backupRuns.delete
      x-api-path-slug: projectsprojectinstancesinstancebackuprunsid-delete
      parameters:
      - in: path
        name: id
        description: The ID of the Backup Run to delete
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Backupruns
    get:
      summary: Get Projects Project Instances Instance Backupruns
      description: Retrieves a resource containing information about a backup run.
      operationId: sql.backupRuns.get
      x-api-path-slug: projectsprojectinstancesinstancebackuprunsid-get
      parameters:
      - in: path
        name: id
        description: The ID of this Backup Run
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Backupruns
  /projects/{project}/instances/{instance}/clone:
    post:
      summary: Add Projects Project Instances Instance Clone
      description: Creates a Cloud SQL instance as a clone of the source instance.
        The API is not ready for Second Generation instances yet.
      operationId: sql.instances.clone
      x-api-path-slug: projectsprojectinstancesinstanceclone-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: The ID of the Cloud SQL instance to be cloned (source)
      - in: path
        name: project
        description: Project ID of the source as well as the clone Cloud SQL instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Clone
  /projects/{project}/instances/{instance}/createEphemeral:
    post:
      summary: Add Projects Project Instances Instance Createephemeral
      description: Generates a short-lived X509 certificate containing the provided
        public key and signed by a private key specific to the target instance. Users
        may use the certificate to authenticate as themselves when connecting to the
        database.
      operationId: sql.sslCerts.createEphemeral
      x-api-path-slug: projectsprojectinstancesinstancecreateephemeral-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the Cloud SQL project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Createephemeral
  /projects/{project}/instances/{instance}/databases:
    get:
      summary: Get Projects Project Instances Instance Databases
      description: Lists databases in the specified Cloud SQL instance.
      operationId: sql.databases.list
      x-api-path-slug: projectsprojectinstancesinstancedatabases-get
      parameters:
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project for which to list Cloud SQL instances
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Databases
    post:
      summary: Add Projects Project Instances Instance Databases
      description: Inserts a resource containing information about a database inside
        a Cloud SQL instance.
      operationId: sql.databases.insert
      x-api-path-slug: projectsprojectinstancesinstancedatabases-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Database instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Databases
  /projects/{project}/instances/{instance}/databases/{database}:
    delete:
      summary: Delete Projects Project Instances Instance Databases Database
      description: Deletes a database from a Cloud SQL instance.
      operationId: sql.databases.delete
      x-api-path-slug: projectsprojectinstancesinstancedatabasesdatabase-delete
      parameters:
      - in: path
        name: database
        description: Name of the database to be deleted in the instance
      - in: path
        name: instance
        description: Database instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Databases
      - Database
    get:
      summary: Get Projects Project Instances Instance Databases Database
      description: Retrieves a resource containing information about a database inside
        a Cloud SQL instance.
      operationId: sql.databases.get
      x-api-path-slug: projectsprojectinstancesinstancedatabasesdatabase-get
      parameters:
      - in: path
        name: database
        description: Name of the database in the instance
      - in: path
        name: instance
        description: Database instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Databases
      - Database
    patch:
      summary: Patch Projects Project Instances Instance Databases Database
      description: Updates a resource containing information about a database inside
        a Cloud SQL instance. This method supports patch semantics.
      operationId: sql.databases.patch
      x-api-path-slug: projectsprojectinstancesinstancedatabasesdatabase-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: database
        description: Name of the database to be updated in the instance
      - in: path
        name: instance
        description: Database instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Databases
      - Database
    put:
      summary: Put Projects Project Instances Instance Databases Database
      description: Updates a resource containing information about a database inside
        a Cloud SQL instance.
      operationId: sql.databases.update
      x-api-path-slug: projectsprojectinstancesinstancedatabasesdatabase-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: database
        description: Name of the database to be updated in the instance
      - in: path
        name: instance
        description: Database instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Put
      - Projects
      - Project
      - Instances
      - Instance
      - Databases
      - Database
  /projects/{project}/instances/{instance}/export:
    post:
      summary: Add Projects Project Instances Instance Export
      description: Exports data from a Cloud SQL instance to a Google Cloud Storage
        bucket as a MySQL dump file.
      operationId: sql.instances.export
      x-api-path-slug: projectsprojectinstancesinstanceexport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance to be exported
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Export
  /projects/{project}/instances/{instance}/failover:
    post:
      summary: Add Projects Project Instances Instance Failover
      description: Failover the instance to its failover replica instance.
      operationId: sql.instances.failover
      x-api-path-slug: projectsprojectinstancesinstancefailover-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: ID of the project that contains the read replica
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Failover
  /projects/{project}/instances/{instance}/import:
    post:
      summary: Add Projects Project Instances Instance Import
      description: Imports data into a Cloud SQL instance from a MySQL dump file in
        Google Cloud Storage.
      operationId: sql.instances.import
      x-api-path-slug: projectsprojectinstancesinstanceimport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Import
  /projects/{project}/instances/{instance}/promoteReplica:
    post:
      summary: Add Projects Project Instances Instance Promotereplica
      description: Promotes the read replica instance to be a stand-alone Cloud SQL
        instance.
      operationId: sql.instances.promoteReplica
      x-api-path-slug: projectsprojectinstancesinstancepromotereplica-post
      parameters:
      - in: path
        name: instance
        description: Cloud SQL read replica instance name
      - in: path
        name: project
        description: ID of the project that contains the read replica
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Promotereplica
  /projects/{project}/instances/{instance}/resetSslConfig:
    post:
      summary: Add Projects Project Instances Instance Resetsslconfig
      description: Deletes all client certificates and generates a new server SSL
        certificate for the instance. The changes will not take effect until the instance
        is restarted. Existing instances without a server certificate will need to
        call this once to set a server certificate.
      operationId: sql.instances.resetSslConfig
      x-api-path-slug: projectsprojectinstancesinstanceresetsslconfig-post
      parameters:
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Resetsslconfig
  /projects/{project}/instances/{instance}/restart:
    post:
      summary: Add Projects Project Instances Instance Restart
      description: Restarts a Cloud SQL instance.
      operationId: sql.instances.restart
      x-api-path-slug: projectsprojectinstancesinstancerestart-post
      parameters:
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance to be restarted
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Restart
  /projects/{project}/instances/{instance}/restoreBackup:
    post:
      summary: Add Projects Project Instances Instance Restorebackup
      description: Restores a backup of a Cloud SQL instance.
      operationId: sql.instances.restoreBackup
      x-api-path-slug: projectsprojectinstancesinstancerestorebackup-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Restorebackup
  /projects/{project}/instances/{instance}/sslCerts:
    get:
      summary: Get Projects Project Instances Instance Sslcerts
      description: Lists all of the current SSL certificates for the instance.
      operationId: sql.sslCerts.list
      x-api-path-slug: projectsprojectinstancesinstancesslcerts-get
      parameters:
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project for which to list Cloud SQL instances
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Sslcerts
    post:
      summary: Add Projects Project Instances Instance Sslcerts
      description: Creates an SSL certificate and returns it along with the private
        key and server certificate authority. The new certificate will not be usable
        until the instance is restarted.
      operationId: sql.sslCerts.insert
      x-api-path-slug: projectsprojectinstancesinstancesslcerts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project to which the newly created Cloud SQL
          instances should belong
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Sslcerts
  /projects/{project}/instances/{instance}/sslCerts/{sha1Fingerprint}:
    delete:
      summary: Delete Projects Project Instances Instance Sslcerts Sha1fingerprint
      description: Deletes the SSL certificate. The change will not take effect until
        the instance is restarted.
      operationId: sql.sslCerts.delete
      x-api-path-slug: projectsprojectinstancesinstancesslcertssha1fingerprint-delete
      parameters:
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance to be deleted
      - in: path
        name: sha1Fingerprint
        description: Sha1 FingerPrint
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Sslcerts
      - Sha1fingerprint
    get:
      summary: Get Projects Project Instances Instance Sslcerts Sha1fingerprint
      description: Retrieves a particular SSL certificate. Does not include the private
        key (required for usage). The private key must be saved from the response
        to initial creation.
      operationId: sql.sslCerts.get
      x-api-path-slug: projectsprojectinstancesinstancesslcertssha1fingerprint-get
      parameters:
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      - in: path
        name: sha1Fingerprint
        description: Sha1 FingerPrint
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Sslcerts
      - Sha1fingerprint
  /projects/{project}/instances/{instance}/startReplica:
    post:
      summary: Add Projects Project Instances Instance Startreplica
      description: Starts the replication in the read replica instance.
      operationId: sql.instances.startReplica
      x-api-path-slug: projectsprojectinstancesinstancestartreplica-post
      parameters:
      - in: path
        name: instance
        description: Cloud SQL read replica instance name
      - in: path
        name: project
        description: ID of the project that contains the read replica
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Startreplica
  /projects/{project}/instances/{instance}/stopReplica:
    post:
      summary: Add Projects Project Instances Instance Stopreplica
      description: Stops the replication in the read replica instance.
      operationId: sql.instances.stopReplica
      x-api-path-slug: projectsprojectinstancesinstancestopreplica-post
      parameters:
      - in: path
        name: instance
        description: Cloud SQL read replica instance name
      - in: path
        name: project
        description: ID of the project that contains the read replica
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Stopreplica
  /projects/{project}/instances/{instance}/truncateLog:
    post:
      summary: Add Projects Project Instances Instance Truncatelog
      description: Truncate MySQL general and slow query log tables
      operationId: sql.instances.truncateLog
      x-api-path-slug: projectsprojectinstancesinstancetruncatelog-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the Cloud SQL project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Truncatelog
  /projects/{project}/instances/{instance}/users:
    delete:
      summary: Delete Projects Project Instances Instance Users
      description: Deletes a user from a Cloud SQL instance.
      operationId: sql.users.delete
      x-api-path-slug: projectsprojectinstancesinstanceusers-delete
      parameters:
      - in: query
        name: host
        description: Host of the user in the instance
      - in: path
        name: instance
        description: Database instance ID
      - in: query
        name: name
        description: Name of the user in the instance
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Users
    get:
      summary: Get Projects Project Instances Instance Users
      description: Lists users in the specified Cloud SQL instance.
      operationId: sql.users.list
      x-api-path-slug: projectsprojectinstancesinstanceusers-get
      parameters:
      - in: path
        name: instance
        description: Database instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Users
    post:
      summary: Add Projects Project Instances Instance Users
      description: Creates a new user in a Cloud SQL instance.
      operationId: sql.users.insert
      x-api-path-slug: projectsprojectinstancesinstanceusers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Database instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Users
    put:
      summary: Put Projects Project Instances Instance Users
      description: Updates an existing user in a Cloud SQL instance.
      operationId: sql.users.update
      x-api-path-slug: projectsprojectinstancesinstanceusers-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: host
        description: Host of the user in the instance
      - in: path
        name: instance
        description: Database instance ID
      - in: query
        name: name
        description: Name of the user in the instance
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Put
      - Projects
      - Project
      - Instances
      - Instance
      - Users
  /projects/{project}/operations:
    get:
      summary: Get Projects Project Operations
      description: Lists all instance operations that have been performed on the given
        Cloud SQL instance in the reverse chronological order of the start time.
      operationId: sql.operations.list
      x-api-path-slug: projectsprojectoperations-get
      parameters:
      - in: query
        name: instance
        description: Cloud SQL instance ID
      - in: query
        name: maxResults
        description: Maximum number of operations per response
      - in: query
        name: pageToken
        description: A previously-returned page token representing part of the larger
          set of results to view
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Operations
  /projects/{project}/operations/{operation}:
    get:
      summary: Get Projects Project Operations Operation
      description: Retrieves an instance operation that has been performed on an instance.
      operationId: sql.operations.get
      x-api-path-slug: projectsprojectoperationsoperation-get
      parameters:
      - in: path
        name: operation
        description: Instance operation ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Operations
      - Operation
  /projects/{project}/tiers:
    get:
      summary: Get Projects Project Tiers
      description: Lists all available service tiers for Google Cloud SQL, for example
        D1, D2. For related information, see Pricing.
      operationId: sql.tiers.list
      x-api-path-slug: projectsprojecttiers-get
      parameters:
      - in: path
        name: project
        description: Project ID of the project for which to list tiers
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Tiers