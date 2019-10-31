swagger: "2.0"
x-collection-name: Google Cloud Dataproc
x-complete: 1
info:
  title: Google Cloud Dataproc
  description: manages-hadoopbased-clusters-and-jobs-on-google-cloud-platform-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: dataproc.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/projects/{projectId}/regions/{region}/clusters:
    get:
      summary: Get Region Clusters
      description: Lists all regions/{region}/clusters in a project.
      operationId: dataproc.projects.regions.clusters.list
      x-api-path-slug: v1projectsprojectidregionsregionclusters-get
      parameters:
      - in: query
        name: filter
        description: Optional A filter constraining the clusters to list
      - in: query
        name: pageSize
        description: Optional The standard List page size
      - in: query
        name: pageToken
        description: Optional The standard List page token
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          cluster belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      responses:
        200:
          description: OK
      tags:
      - Cluster
    post:
      summary: Create Cluster
      description: Creates a cluster in a project.
      operationId: dataproc.projects.regions.clusters.create
      x-api-path-slug: v1projectsprojectidregionsregionclusters-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          cluster belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      responses:
        200:
          description: OK
      tags:
      - Cluster
  /v1/projects/{projectId}/regions/{region}/clusters/{clusterName}:
    delete:
      summary: Delete Cluster
      description: Deletes a cluster in a project.
      operationId: dataproc.projects.regions.clusters.delete
      x-api-path-slug: v1projectsprojectidregionsregionclustersclustername-delete
      parameters:
      - in: path
        name: clusterName
        description: Required The cluster name
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          cluster belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      responses:
        200:
          description: OK
      tags:
      - Cluster
    get:
      summary: Get Cluster
      description: Gets the resource representation for a cluster in a project.
      operationId: dataproc.projects.regions.clusters.get
      x-api-path-slug: v1projectsprojectidregionsregionclustersclustername-get
      parameters:
      - in: path
        name: clusterName
        description: Required The cluster name
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          cluster belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      responses:
        200:
          description: OK
      tags:
      - Cluster
    patch:
      summary: Update Cluster
      description: Updates a cluster in a project.
      operationId: dataproc.projects.regions.clusters.patch
      x-api-path-slug: v1projectsprojectidregionsregionclustersclustername-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: clusterName
        description: Required The cluster name
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project the cluster
          belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      - in: query
        name: updateMask
        description: Required Specifies the path, relative to Cluster, of the field
          to update
      responses:
        200:
          description: OK
      tags:
      - Cluster
  /v1/projects/{projectId}/regions/{region}/clusters/{clusterName}:diagnose:
    post:
      summary: Get Cluster Diagnostic
      description: Gets cluster diagnostic information. After the operation completes,
        the Operation.response field contains DiagnoseClusterOutputLocation.
      operationId: dataproc.projects.regions.clusters.diagnose
      x-api-path-slug: v1projectsprojectidregionsregionclustersclusternamediagnose-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: clusterName
        description: Required The cluster name
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          cluster belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      responses:
        200:
          description: OK
      tags:
      - Cluster
  /v1/projects/{projectId}/regions/{region}/jobs:
    get:
      summary: Get Region Jobs
      description: Lists regions/{region}/jobs in a project.
      operationId: dataproc.projects.regions.jobs.list
      x-api-path-slug: v1projectsprojectidregionsregionjobs-get
      parameters:
      - in: query
        name: clusterName
        description: Optional If set, the returned jobs list includes only jobs that
          were submitted to the named cluster
      - in: query
        name: filter
        description: Optional A filter constraining the jobs to list
      - in: query
        name: jobStateMatcher
        description: Optional Specifies enumerated categories of jobs to list (default
          = match ALL jobs)
      - in: query
        name: pageSize
        description: Optional The number of results to return in each response
      - in: query
        name: pageToken
        description: Optional The page token, returned by a previous call, to request
          the next page of results
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          job belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1/projects/{projectId}/regions/{region}/jobs/{jobId}:
    delete:
      summary: Delete Job
      description: Deletes the job from the project. If the job is active, the delete
        fails, and the response returns FAILED_PRECONDITION.
      operationId: dataproc.projects.regions.jobs.delete
      x-api-path-slug: v1projectsprojectidregionsregionjobsjobid-delete
      parameters:
      - in: path
        name: jobId
        description: Required The job ID
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          job belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      responses:
        200:
          description: OK
      tags:
      - Job
    get:
      summary: Get Job
      description: Gets the resource representation for a job in a project.
      operationId: dataproc.projects.regions.jobs.get
      x-api-path-slug: v1projectsprojectidregionsregionjobsjobid-get
      parameters:
      - in: path
        name: jobId
        description: Required The job ID
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          job belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      responses:
        200:
          description: OK
      tags:
      - Job
    patch:
      summary: Update Job
      description: Updates a job in a project.
      operationId: dataproc.projects.regions.jobs.patch
      x-api-path-slug: v1projectsprojectidregionsregionjobsjobid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: jobId
        description: Required The job ID
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          job belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      - in: query
        name: updateMask
        description: Required Specifies the path, relative to Job, of the field to
          update
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1/projects/{projectId}/regions/{region}/jobs/{jobId}:cancel:
    post:
      summary: Cancel Job
      description: Starts a job cancellation request. To access the job resource after
        cancellation, call regions/{region}/jobs.list or regions/{region}/jobs.get.
      operationId: dataproc.projects.regions.jobs.cancel
      x-api-path-slug: v1projectsprojectidregionsregionjobsjobidcancel-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: jobId
        description: Required The job ID
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          job belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1/projects/{projectId}/regions/{region}/jobs:submit:
    post:
      summary: Submit Job
      description: Submits a job to a cluster.
      operationId: dataproc.projects.regions.jobs.submit
      x-api-path-slug: v1projectsprojectidregionsregionjobssubmit-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          job belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1/{name}:
    delete:
      summary: Delete Operation
      description: Deletes a long-running operation. This method indicates that the
        client is no longer interested in the operation result. It does not cancel
        the operation. If the server doesn't support this method, it returns google.rpc.Code.UNIMPLEMENTED.
      operationId: dataproc.projects.regions.operations.delete
      x-api-path-slug: v1name-delete
      parameters:
      - in: path
        name: name
        description: The name of the operation resource to be deleted
      responses:
        200:
          description: OK
      tags:
      - Operation
    get:
      summary: Get Operation State
      description: Gets the latest state of a long-running operation. Clients can
        use this method to poll the operation result at intervals as recommended by
        the API service.
      operationId: dataproc.projects.regions.operations.get
      x-api-path-slug: v1name-get
      parameters:
      - in: path
        name: name
        description: The name of the operation resource
      responses:
        200:
          description: OK
      tags:
      - Operation
  /v1/{name}:cancel:
    post:
      summary: Start Cancellation
      description: Starts asynchronous cancellation on a long-running operation. The
        server makes a best effort to cancel the operation, but success is not guaranteed.
        If the server doesn't support this method, it returns google.rpc.Code.UNIMPLEMENTED.
        Clients can use Operations.GetOperation or other methods to check whether
        the cancellation succeeded or whether the operation completed despite cancellation.
        On successful cancellation, the operation is not deleted; instead, it becomes
        an operation with an Operation.error value with a google.rpc.Status.code of
        1, corresponding to Code.CANCELLED.
      operationId: dataproc.projects.regions.operations.cancel
      x-api-path-slug: v1namecancel-post
      parameters:
      - in: path
        name: name
        description: The name of the operation resource to be cancelled
      responses:
        200:
          description: OK
      tags:
      - Operation