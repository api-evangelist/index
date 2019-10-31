swagger: "2.0"
x-collection-name: Google Cloud Machine Learning Engine
x-complete: 1
info:
  title: Google Cloud Machine Learning Engine
  description: an-api-to-enable-creating-and-using-machine-learning-models-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: ml.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:
    delete:
      summary: Delete Model Version
      description: |-
        Deletes a model version.

        Each model can have multiple versions deployed and in use at any given
        time. Use this method to remove a single version.

        Note: You cannot delete the version that is set as the default version
        of the model unless it is the only remaining version.
      operationId: ml.projects.models.versions.delete
      x-api-path-slug: v1name-delete
      parameters:
      - in: path
        name: name
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Version
    get:
      summary: Get Model Version
      description: |-
        Gets information about a model version.

        Models can have multiple versions. You can call
        [projects.models.versions.list](/ml/reference/rest/v1/projects.models.versions/list)
        to get the same information that this method returns for all of the
        versions of a model.
      operationId: ml.projects.models.versions.get
      x-api-path-slug: v1name-get
      parameters:
      - in: path
        name: name
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Version
  /v1/{name}/operations:
    get:
      summary: Get Operations
      description: |-
        Lists operations that match the specified filter in the request. If the
        server doesn't support this method, it returns `UNIMPLEMENTED`.

        NOTE: the `name` binding below allows API services to override the binding
        to use different resource name schemes, such as `users/*/operations`.
      operationId: ml.projects.operations.list
      x-api-path-slug: v1nameoperations-get
      parameters:
      - in: query
        name: filter
        description: The standard list filter
      - in: path
        name: name
        description: The name of the operation collection
      - in: query
        name: pageSize
        description: The standard list page size
      - in: query
        name: pageToken
        description: The standard list page token
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Operation
  /v1/{name}:cancel:
    post:
      summary: Cancel Operation
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
      operationId: ml.projects.operations.cancel
      x-api-path-slug: v1namecancel-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The name of the operation resource to be cancelled
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Operation
  /v1/{name}:getConfig:
    get:
      summary: Get Operation
      description: |-
        Get the service account information associated with your project. You need
        this information in order to grant the service account persmissions for
        the Google Cloud Storage location where you put your model training code
        for training the model with Google Cloud Machine Learning.
      operationId: ml.projects.getConfig
      x-api-path-slug: v1namegetconfig-get
      parameters:
      - in: path
        name: name
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Operation
  /v1/{name}:predict:
    post:
      summary: Predict Operation
      description: |-
        Performs prediction on the data in the request.

        **** REMOVE FROM GENERATED DOCUMENTATION
      operationId: ml.projects.predict
      x-api-path-slug: v1namepredict-post
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
      - Machine Learning
      - Operation
  /v1/{name}:setDefault:
    post:
      summary: Set Default Version
      description: |-
        Designates a version to be the default for the model.

        The default version is used for prediction requests made against the model
        that don't specify a version.

        The first version to be created for a model is automatically set as the
        default. You must make any subsequent changes to the default version
        setting manually using this method.
      operationId: ml.projects.models.versions.setDefault
      x-api-path-slug: v1namesetdefault-post
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
      - Machine Learning
      - Version
  /v1/{parent}/jobs:
    get:
      summary: List Jobs
      description: Lists the jobs in the project.
      operationId: ml.projects.jobs.list
      x-api-path-slug: v1parentjobs-get
      parameters:
      - in: query
        name: filter
        description: Optional
      - in: query
        name: pageSize
        description: Optional
      - in: query
        name: pageToken
        description: Optional
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Job
    post:
      summary: Create Job
      description: Creates a training or a batch prediction job.
      operationId: ml.projects.jobs.create
      x-api-path-slug: v1parentjobs-post
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
      - Machine Learning
      - Job
  /v1/{parent}/models:
    get:
      summary: List Models
      description: |-
        Lists the models in a project.

        Each project can contain multiple models, and each model can have multiple
        versions.
      operationId: ml.projects.models.list
      x-api-path-slug: v1parentmodels-get
      parameters:
      - in: query
        name: pageSize
        description: Optional
      - in: query
        name: pageToken
        description: Optional
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Model
    post:
      summary: Create Models
      description: |-
        Creates a model which will later contain one or more versions.

        You must add at least one version before you can request predictions from
        the model. Add versions by calling
        [projects.models.versions.create](/ml/reference/rest/v1/projects.models.versions/create).
      operationId: ml.projects.models.create
      x-api-path-slug: v1parentmodels-post
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
      - Machine Learning
      - Model
  /v1/{parent}/versions:
    get:
      summary: Get Version
      description: |-
        Gets basic information about all the versions of a model.

        If you expect that a model has a lot of versions, or if you need to handle
        only a limited number of results at a time, you can request that the list
        be retrieved in batches (called pages):
      operationId: ml.projects.models.versions.list
      x-api-path-slug: v1parentversions-get
      parameters:
      - in: query
        name: pageSize
        description: Optional
      - in: query
        name: pageToken
        description: Optional
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Version
    post:
      summary: Create Version
      description: |-
        Creates a new version of a model from a trained TensorFlow model.

        If the version created in the cloud by this call is the first deployed
        version of the specified model, it will be made the default version of the
        model. When you add a version to a model that already has one or more
        versions, the default version does not automatically change. If you want a
        new version to be the default, you must call
        [projects.models.versions.setDefault](/ml/reference/rest/v1/projects.models.versions/setDefault).
      operationId: ml.projects.models.versions.create
      x-api-path-slug: v1parentversions-post
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
      - Machine Learning
      - Version