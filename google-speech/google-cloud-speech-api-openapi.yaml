swagger: "2.0"
x-collection-name: Google Speech
x-complete: 1
info:
  title: Google Cloud Speech
  description: google-cloud-speech-api-
  contact:
    name: Google
    url: https://google.com
  version: v1beta1
host: speech.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1beta1/operations:
    get:
      summary: Get Operations
      description: |-
        Lists operations that match the specified filter in the request. If the
        server doesn't support this method, it returns `UNIMPLEMENTED`.

        NOTE: the `name` binding below allows API services to override the binding
        to use different resource name schemes, such as `users/*/operations`.
      operationId: speech.operations.list
      x-api-path-slug: v1beta1operations-get
      parameters:
      - in: query
        name: filter
        description: The standard list filter
      - in: query
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
      - Operation
  /v1beta1/operations/{name}:
    delete:
      summary: Delete Operation
      description: |-
        Deletes a long-running operation. This method indicates that the client is
        no longer interested in the operation result. It does not cancel the
        operation. If the server doesn't support this method, it returns
        `google.rpc.Code.UNIMPLEMENTED`.
      operationId: speech.operations.delete
      x-api-path-slug: v1beta1operationsname-delete
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
      summary: Delete Operation
      description: |-
        Gets the latest state of a long-running operation.  Clients can use this
        method to poll the operation result at intervals as recommended by the API
        service.
      operationId: speech.operations.get
      x-api-path-slug: v1beta1operationsname-get
      parameters:
      - in: path
        name: name
        description: The name of the operation resource
      responses:
        200:
          description: OK
      tags:
      - Operation
  /v1beta1/operations/{name}:cancel:
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
      operationId: speech.operations.cancel
      x-api-path-slug: v1beta1operationsnamecancel-post
      parameters:
      - in: path
        name: name
        description: The name of the operation resource to be cancelled
      responses:
        200:
          description: OK
      tags:
      - Operation
  /v1beta1/speech:asyncrecognize:
    post:
      summary: Perform Asynchronous Speech Recognition
      description: |-
        Performs asynchronous speech recognition: receive results via the
        [google.longrunning.Operations]
        (/speech/reference/rest/v1beta1/operations#Operation)
        interface. Returns either an
        `Operation.error` or an `Operation.response` which contains
        an `AsyncRecognizeResponse` message.
      operationId: speech.speech.asyncrecognize
      x-api-path-slug: v1beta1speechasyncrecognize-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Speech Recognition
  /v1beta1/speech:syncrecognize:
    post:
      summary: Perform Synchronous Speech Recognition
      description: |-
        Performs synchronous speech recognition: receive results after all audio
        has been sent and processed.
      operationId: speech.speech.syncrecognize
      x-api-path-slug: v1beta1speechsyncrecognize-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Speech Recognition