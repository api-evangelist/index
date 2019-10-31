swagger: "2.0"
x-collection-name: Google Stackdriver Monitoring
x-complete: 1
info:
  title: Google Stackdriver Monitoring
  description: google-stackdriver-provides-powerful-monitoring-logging-and-diagnostics--it-equips-you-with-insight-into-the-health-performance-and-availability-of-cloudpowered-applications-enabling-you-to-find-and-fix-issues-faster--it-is-natively-integrated-with-google-cloud-platform-amazon-web-services-and-popular-open-source-packages--stackdriver-provides-a-wide-variety-of-metrics-dashboards-alerting-log-management-reporting-and-tracing-capabilities-
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/metricDescriptors:
    get:
      summary: Get Project Metric Descriptors
      description: List metric descriptors that match the query. If the query is not
        set, then all of the metric descriptors will be returned. Large responses
        will be paginated, use the nextPageToken returned in the response to request
        subsequent pages of results by setting the pageToken query parameter to the
        value of the nextPageToken.
      operationId: cloudmonitoring.metricDescriptors.list
      x-api-path-slug: projectmetricdescriptors-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: count
        description: Maximum number of metric descriptors per page
      - in: query
        name: pageToken
        description: The pagination token, which is used to page through large result
          sets
      - in: path
        name: project
        description: The project id
      - in: query
        name: query
        description: The query used to search against existing metrics
      responses:
        200:
          description: OK
      tags:
      - Monitoring
    post:
      summary: Post Project Metric Descriptors
      description: Create a new metric.
      operationId: cloudmonitoring.metricDescriptors.create
      x-api-path-slug: projectmetricdescriptors-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: The project id
      responses:
        200:
          description: OK
      tags:
      - Monitoring
  /{project}/metricDescriptors/{metric}:
    delete:
      summary: Delete Project Metric Descriptors Metric
      description: Delete an existing metric.
      operationId: cloudmonitoring.metricDescriptors.delete
      x-api-path-slug: projectmetricdescriptorsmetric-delete
      parameters:
      - in: path
        name: metric
        description: Name of the metric
      - in: path
        name: project
        description: The project ID to which the metric belongs
      responses:
        200:
          description: OK
      tags:
      - Monitoring
  /{project}/timeseries/{metric}:
    get:
      summary: Get Project Timeseries Metric
      description: List the data points of the time series that match the metric and
        labels values and that have data points in the interval. Large responses are
        paginated; use the nextPageToken returned in the response to request subsequent
        pages of results by setting the pageToken query parameter to the value of
        the nextPageToken.
      operationId: cloudmonitoring.timeseries.list
      x-api-path-slug: projecttimeseriesmetric-get
      parameters:
      - in: query
        name: aggregator
        description: The aggregation function that will reduce the data points in
          each window to a single point
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: count
        description: Maximum number of data points per page, which is used for pagination
          of results
      - in: query
        name: labels
        description: 'A collection of labels for the matching time series, which are
          represented as:  - key==value: key equals the value - key=~value: key regex
          matches the value - key!=value: key does not equal the value - key!~value:
          key regex does not match the value  For example, to list all of the time
          series descriptors for the region us-central1, you could specify:label=cloud'
      - in: path
        name: metric
        description: Metric names are protocol-free URLs as listed in the Supported
          Metrics page
      - in: query
        name: oldest
        description: Start of the time interval (exclusive), which is expressed as
          an RFC 3339 timestamp
      - in: query
        name: pageToken
        description: The pagination token, which is used to page through large result
          sets
      - in: path
        name: project
        description: The project ID to which this time series belongs
      - in: query
        name: timespan
        description: 'Length of the time interval to query, which is an alternative
          way to declare the interval: (youngest - timespan, youngest]'
      - in: query
        name: window
        description: The sampling window
      - in: query
        name: youngest
        description: End of the time interval (inclusive), which is expressed as an
          RFC 3339 timestamp
      responses:
        200:
          description: OK
      tags:
      - Monitoring
  /{project}/timeseries:write:
    post:
      summary: Post Project Timeseries Write
      description: Put data points to one or more time series for one or more metrics.
        If a time series does not exist, a new time series will be created. It is
        not allowed to write a time series point that is older than the existing youngest
        point of that time series. Points that are older than the existing youngest
        point of that time series will be discarded silently. Therefore, users should
        make sure that points of a time series are written sequentially in the order
        of their end time.
      operationId: cloudmonitoring.timeseries.write
      x-api-path-slug: projecttimeserieswrite-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: The project ID
      responses:
        200:
          description: OK
      tags:
      - Monitoring
  /{project}/timeseriesDescriptors/{metric}:
    get:
      summary: Get Project Timeseriesdescriptors Metric
      description: List the descriptors of the time series that match the metric and
        labels values and that have data points in the interval. Large responses are
        paginated; use the nextPageToken returned in the response to request subsequent
        pages of results by setting the pageToken query parameter to the value of
        the nextPageToken.
      operationId: cloudmonitoring.timeseriesDescriptors.list
      x-api-path-slug: projecttimeseriesdescriptorsmetric-get
      parameters:
      - in: query
        name: aggregator
        description: The aggregation function that will reduce the data points in
          each window to a single point
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: count
        description: Maximum number of time series descriptors per page
      - in: query
        name: labels
        description: 'A collection of labels for the matching time series, which are
          represented as:  - key==value: key equals the value - key=~value: key regex
          matches the value - key!=value: key does not equal the value - key!~value:
          key regex does not match the value  For example, to list all of the time
          series descriptors for the region us-central1, you could specify:label=cloud'
      - in: path
        name: metric
        description: Metric names are protocol-free URLs as listed in the Supported
          Metrics page
      - in: query
        name: oldest
        description: Start of the time interval (exclusive), which is expressed as
          an RFC 3339 timestamp
      - in: query
        name: pageToken
        description: The pagination token, which is used to page through large result
          sets
      - in: path
        name: project
        description: The project ID to which this time series belongs
      - in: query
        name: timespan
        description: 'Length of the time interval to query, which is an alternative
          way to declare the interval: (youngest - timespan, youngest]'
      - in: query
        name: window
        description: The sampling window
      - in: query
        name: youngest
        description: End of the time interval (inclusive), which is expressed as an
          RFC 3339 timestamp
      responses:
        200:
          description: OK
      tags:
      - Monitoring
  /v2/controller/debuggees/register:
    post:
      summary: Post Controller Debuggees Register
      description: Registers the debuggee with the controller service. All agents
        attached to the same application should call this method with the same request
        content to get back the same stable `debuggee_id`. Agents should call this
        method again whenever `google.rpc.Code.NOT_FOUND` is returned from any controller
        method. This allows the controller service to disable the agent or recover
        from any data loss. If the debuggee is disabled by the server, the response
        will have `is_disabled` set to `true`.
      operationId: clouddebugger.controller.debuggees.register
      x-api-path-slug: v2controllerdebuggeesregister-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Debugger
  /v2/controller/debuggees/{debuggeeId}/breakpoints:
    get:
      summary: Get Controller Debuggees Debuggeeid Breakpoints
      description: Returns the list of all active breakpoints for the debuggee. The
        breakpoint specification (location, condition, and expression fields) is semantically
        immutable, although the field values may change. For example, an agent may
        update the location line number to reflect the actual line where the breakpoint
        was set, but this doesn't change the breakpoint semantics. This means that
        an agent does not need to check if a breakpoint has changed when it encounters
        the same breakpoint on a successive call. Moreover, an agent should remember
        the breakpoints that are completed until the controller removes them from
        the active list to avoid setting those breakpoints again.
      operationId: clouddebugger.controller.debuggees.breakpoints.list
      x-api-path-slug: v2controllerdebuggeesdebuggeeidbreakpoints-get
      parameters:
      - in: path
        name: debuggeeId
        description: Identifies the debuggee
      - in: query
        name: successOnTimeout
        description: If set to `true`, returns `google
      - in: query
        name: waitToken
        description: A wait token that, if specified, blocks the method call until
          the list of active breakpoints has changed, or a server selected timeout
          has expired
      responses:
        200:
          description: OK
      tags:
      - Debugger
  /v2/controller/debuggees/{debuggeeId}/breakpoints/{id}:
    put:
      summary: Put Controller Debuggees Debuggeeid Breakpoints
      description: Updates the breakpoint state or mutable fields. The entire Breakpoint
        message must be sent back to the controller service. Updates to active breakpoint
        fields are only allowed if the new value does not change the breakpoint specification.
        Updates to the `location`, `condition` and `expression` fields should not
        alter the breakpoint semantics. These may only make changes such as canonicalizing
        a value or snapping the location to the correct line of code.
      operationId: clouddebugger.controller.debuggees.breakpoints.update
      x-api-path-slug: v2controllerdebuggeesdebuggeeidbreakpointsid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: debuggeeId
        description: Identifies the debuggee being debugged
      - in: path
        name: id
        description: Breakpoint identifier, unique in the scope of the debuggee
      responses:
        200:
          description: OK
      tags:
      - Debugger
  /v2/debugger/debuggees:
    get:
      summary: Get Debugger Debuggees
      description: Lists all the debuggees that the user can set breakpoints to.
      operationId: clouddebugger.debugger.debuggees.list
      x-api-path-slug: v2debuggerdebuggees-get
      parameters:
      - in: query
        name: clientVersion
        description: The client version making the call
      - in: query
        name: includeInactive
        description: When set to `true`, the result includes all debuggees
      - in: query
        name: project
        description: Project number of a Google Cloud project whose debuggees to list
      responses:
        200:
          description: OK
      tags:
      - Debugger
  /v2/debugger/debuggees/{debuggeeId}/breakpoints:
    get:
      summary: Get Debugger Debuggees Debuggeeid Breakpoints
      description: Lists all breakpoints for the debuggee.
      operationId: clouddebugger.debugger.debuggees.breakpoints.list
      x-api-path-slug: v2debuggerdebuggeesdebuggeeidbreakpoints-get
      parameters:
      - in: query
        name: action.value
        description: Only breakpoints with the specified action will pass the filter
      - in: query
        name: clientVersion
        description: The client version making the call
      - in: path
        name: debuggeeId
        description: ID of the debuggee whose breakpoints to list
      - in: query
        name: includeAllUsers
        description: When set to `true`, the response includes the list of breakpoints
          set by any user
      - in: query
        name: includeInactive
        description: When set to `true`, the response includes active and inactive
          breakpoints
      - in: query
        name: stripResults
        description: 'When set to `true`, the response breakpoints are stripped of
          the results fields: `stack_frames`, `evaluated_expressions` and `variable_table`'
      - in: query
        name: waitToken
        description: A wait token that, if specified, blocks the call until the breakpoints
          list has changed, or a server selected timeout has expired
      responses:
        200:
          description: OK
      tags:
      - Debugger
  /v2/debugger/debuggees/{debuggeeId}/breakpoints/set:
    post:
      summary: Post Debugger Debuggees Debuggeeid Breakpoints Set
      description: Sets the breakpoint to the debuggee.
      operationId: clouddebugger.debugger.debuggees.breakpoints.set
      x-api-path-slug: v2debuggerdebuggeesdebuggeeidbreakpointsset-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: clientVersion
        description: The client version making the call
      - in: path
        name: debuggeeId
        description: ID of the debuggee where the breakpoint is to be set
      responses:
        200:
          description: OK
      tags:
      - Debugger
  /v2/debugger/debuggees/{debuggeeId}/breakpoints/{breakpointId}:
    delete:
      summary: Delete Debugger Debuggees Debuggeeid Breakpoints Breakpointid
      description: Deletes the breakpoint from the debuggee.
      operationId: clouddebugger.debugger.debuggees.breakpoints.delete
      x-api-path-slug: v2debuggerdebuggeesdebuggeeidbreakpointsbreakpointid-delete
      parameters:
      - in: path
        name: breakpointId
        description: ID of the breakpoint to delete
      - in: query
        name: clientVersion
        description: The client version making the call
      - in: path
        name: debuggeeId
        description: ID of the debuggee whose breakpoint to delete
      responses:
        200:
          description: OK
      tags:
      - Debugger
    get:
      summary: Get Debugger Debuggees Debuggeeid Breakpoints Breakpointid
      description: Gets breakpoint information.
      operationId: clouddebugger.debugger.debuggees.breakpoints.get
      x-api-path-slug: v2debuggerdebuggeesdebuggeeidbreakpointsbreakpointid-get
      parameters:
      - in: path
        name: breakpointId
        description: ID of the breakpoint to get
      - in: query
        name: clientVersion
        description: The client version making the call
      - in: path
        name: debuggeeId
        description: ID of the debuggee whose breakpoint to get
      responses:
        200:
          description: OK
      tags:
      - Debugger
  /v1beta1/{groupName}:
    get:
      summary: Get Groupname
      description: Get the specified group.
      operationId: ""
      x-api-path-slug: v1beta1groupname-get
      parameters:
      - in: path
        name: groupName
        description: '[Required] The group resource name'
      responses:
        200:
          description: OK
      tags:
      - Errors
  /v1beta1/{name}:
    put:
      summary: Put Name
      description: |-
        Replace the data for the specified group.
        Fails if the group does not exist.
      operationId: clouderrorreporting.projects.groups.update
      x-api-path-slug: v1beta1name-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The group resource name
      responses:
        200:
          description: OK
      tags:
      - Errors
  /v1beta1/{projectName}/events:
    delete:
      summary: Delete Project Name Events
      description: Deletes all error events of a given project.
      operationId: clouderrorreporting.projects.deleteEvents
      x-api-path-slug: v1beta1projectnameevents-delete
      parameters:
      - in: path
        name: projectName
        description: '[Required] The resource name of the Google Cloud Platform project'
      responses:
        200:
          description: OK
      tags:
      - Errors
    get:
      summary: Get Project Name Events
      description: Lists the specified events.
      operationId: clouderrorreporting.projects.events.list
      x-api-path-slug: v1beta1projectnameevents-get
      parameters:
      - in: query
        name: groupId
        description: '[Required] The group for which events shall be returned'
      - in: query
        name: pageSize
        description: '[Optional] The maximum number of results to return per response'
      - in: query
        name: pageToken
        description: '[Optional] A `next_page_token` provided by a previous response'
      - in: path
        name: projectName
        description: '[Required] The resource name of the Google Cloud Platform project'
      - in: query
        name: serviceFilter.service
        description: '[Optional] The exact value to match against[`ServiceContext'
      - in: query
        name: serviceFilter.version
        description: '[Optional] The exact value to match against[`ServiceContext'
      - in: query
        name: timeRange.period
        description: Restricts the query to the specified time range
      responses:
        200:
          description: OK
      tags:
      - Errors
  /v1beta1/{projectName}/events:report:
    post:
      summary: Post Project Name Events Report
      description: Report an individual error event. This endpoint accepts <strong>either</strong>
        an OAuth token, or an API key for authentication. To use an API key, append
        it to the URL as the value of a `key` parameter.
      operationId: clouderrorreporting.projects.events.report
      x-api-path-slug: v1beta1projectnameeventsreport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectName
        description: '[Required] The resource name of the Google Cloud Platform project'
      responses:
        200:
          description: OK
      tags:
      - Errors
  /v1beta1/{projectName}/groupStats:
    get:
      summary: Get Project Name Groupstats
      description: Lists the specified groups.
      operationId: clouderrorreporting.projects.groupStats.list
      x-api-path-slug: v1beta1projectnamegroupstats-get
      parameters:
      - in: query
        name: alignment
        description: '[Optional] The alignment of the timed counts to be returned'
      - in: query
        name: alignmentTime
        description: '[Optional] Time where the timed counts shall be aligned if roundedalignment
          is chosen'
      - in: query
        name: groupId
        description: '[Optional] List all ErrorGroupStats with these IDs'
      - in: query
        name: order
        description: '[Optional] The sort order in which the results are returned'
      - in: query
        name: pageSize
        description: '[Optional] The maximum number of results to return per response'
      - in: query
        name: pageToken
        description: '[Optional] A `next_page_token` provided by a previous response'
      - in: path
        name: projectName
        description: '[Required] The resource name of the Google Cloud Platform project'
      - in: query
        name: serviceFilter.service
        description: '[Optional] The exact value to match against[`ServiceContext'
      - in: query
        name: serviceFilter.version
        description: '[Optional] The exact value to match against[`ServiceContext'
      - in: query
        name: timedCountDuration
        description: '[Optional] The preferred duration for a single returned `TimedCount`'
      - in: query
        name: timeRange.period
        description: Restricts the query to the specified time range
      responses:
        200:
          description: OK
      tags:
      - Errors