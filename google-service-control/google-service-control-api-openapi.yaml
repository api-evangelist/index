swagger: "2.0"
x-collection-name: Google Service Control
x-complete: 1
info:
  title: Google Service Control
  description: google-service-control-provides-control-plane-functionality-to-managed-services-such-as-logging-monitoring-and-status-checks-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: servicecontrol.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/services/{serviceName}:allocateQuota:
    post:
      summary: Allocate Quota
      description: |-
        Attempts to allocate quota for the specified consumer. It should be called
        before the operation is executed.

        This method requires the `servicemanagement.services.quota`
        permission on the specified service. For more information, see
        [Google Cloud IAM](https://cloud.google.com/iam).
      operationId: servicecontrol.services.allocateQuota
      x-api-path-slug: v1servicesservicenameallocatequota-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: serviceName
        description: Name of the service as specified in the service configuration
      responses:
        200:
          description: OK
      tags:
      - Service Quota
  /v1/services/{serviceName}:check:
    post:
      summary: Check Operation
      description: |-
        Checks an operation with Google Service Control to decide whether
        the given operation should proceed. It should be called before the
        operation is executed.

        If feasible, the client should cache the check results and reuse them for
        60 seconds. In case of server errors, the client can rely on the cached
        results for longer time.

        NOTE: the `CheckRequest` has the size limit of 64KB.

        This method requires the `servicemanagement.services.check` permission
        on the specified service. For more information, see
        [Google Cloud IAM](https://cloud.google.com/iam).
      operationId: servicecontrol.services.check
      x-api-path-slug: v1servicesservicenamecheck-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: serviceName
        description: The service name as specified in its service configuration
      responses:
        200:
          description: OK
      tags:
      - Service Operation
  /v1/services/{serviceName}:endReconciliation:
    post:
      summary: End Reconciliation
      description: |-
        Signals the quota controller that service ends the ongoing usage
        reconciliation.

        This method requires the `servicemanagement.services.quota`
        permission on the specified service. For more information, see
        [Google Cloud IAM](https://cloud.google.com/iam).
      operationId: servicecontrol.services.endReconciliation
      x-api-path-slug: v1servicesservicenameendreconciliation-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: serviceName
        description: Name of the service as specified in the service configuration
      responses:
        200:
          description: OK
      tags:
      - Service Reconcilliation
  /v1/services/{serviceName}:releaseQuota:
    post:
      summary: Release Quota
      description: |-
        Releases previously allocated quota done through AllocateQuota method.

        This method requires the `servicemanagement.services.quota`
        permission on the specified service. For more information, see
        [Google Cloud IAM](https://cloud.google.com/iam).
      operationId: servicecontrol.services.releaseQuota
      x-api-path-slug: v1servicesservicenamereleasequota-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: serviceName
        description: Name of the service as specified in the service configuration
      responses:
        200:
          description: OK
      tags:
      - Service Quota
  /v1/services/{serviceName}:report:
    post:
      summary: Report
      description: |-
        Reports operation results to Google Service Control, such as logs and
        metrics. It should be called after an operation is completed.

        If feasible, the client should aggregate reporting data for up to 5
        seconds to reduce API traffic. Limiting aggregation to 5 seconds is to
        reduce data loss during client crashes. Clients should carefully choose
        the aggregation time window to avoid data loss risk more than 0.01%
        for business and compliance reasons.

        NOTE: the `ReportRequest` has the size limit of 1MB.

        This method requires the `servicemanagement.services.report` permission
        on the specified service. For more information, see
        [Google Cloud IAM](https://cloud.google.com/iam).
      operationId: servicecontrol.services.report
      x-api-path-slug: v1servicesservicenamereport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: serviceName
        description: The service name as specified in its service configuration
      responses:
        200:
          description: OK
      tags:
      - Report
  /v1/services/{serviceName}:startReconciliation:
    post:
      summary: Start Reconciliation
      description: |-
        Unlike rate quota, allocation quota does not get refilled periodically.
        So, it is possible that the quota usage as seen by the service differs from
        what the One Platform considers the usage is. This is expected to happen
        only rarely, but over time this can accumulate. Services can invoke
        StartReconciliation and EndReconciliation to correct this usage drift, as
        described below:
        1. Service sends StartReconciliation with a timestamp in future for each
           metric that needs to be reconciled. The timestamp being in future allows
           to account for in-flight AllocateQuota and ReleaseQuota requests for the
           same metric.
        2. One Platform records this timestamp and starts tracking subsequent
           AllocateQuota and ReleaseQuota requests until EndReconciliation is
           called.
        3. At or after the time specified in the StartReconciliation, service
           sends EndReconciliation with the usage that needs to be reconciled to.
        4. One Platform adjusts its own record of usage for that metric to the
           value specified in EndReconciliation by taking in to account any
           allocation or release between StartReconciliation and EndReconciliation.

        Signals the quota controller that the service wants to perform a usage
        reconciliation as specified in the request.

        This method requires the `servicemanagement.services.quota`
        permission on the specified service. For more information, see
        [Google Cloud IAM](https://cloud.google.com/iam).
      operationId: servicecontrol.services.startReconciliation
      x-api-path-slug: v1servicesservicenamestartreconciliation-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: serviceName
        description: Name of the service as specified in the service configuration
      responses:
        200:
          description: OK
      tags:
      - Service Reconcilliation