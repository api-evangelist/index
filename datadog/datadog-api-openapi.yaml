swagger: "2.0"
x-collection-name: Datadog
x-complete: 1
info:
  title: DataDog Merged API
  version: 1.0.0
basePath: api/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /metrics:
    get:
      summary: Get Metrics
      description: Get the list of actively reporting metrics from a given time until
        now. This endpoint is not available in the Python and Ruby libraries.
      operationId: getMetrics
      x-api-path-slug: metrics-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Metrics
  /series:
    post:
      summary: Add Series
      description: |-
        The metrics end-point allows you to post time-series data that can be
                  graphed on Datadog's dashboards.
      operationId: postSeries
      x-api-path-slug: series-post
      parameters:
      - in: query
        name: '[[POSIX_timestamp, numeric_value], ...]'
        description: Note that the timestamp should be in seconds, must be current,
          and the numeric value is a 32bit float gauge-type value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Series
  /query:
    get:
      summary: Get Query
      description: This end point allows you to query for metrics from any time period.
      operationId: getQuery
      x-api-path-slug: query-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Query
  /check_run:
    post:
      summary: Add Check Run
      description: Post a Check Run
      operationId: postCheckRun
      x-api-path-slug: check-run-post
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Checks
      - Run
  /downtime:
    post:
      summary: Add Downtime
      description: Schedule monitor downtime
      operationId: postDowntime
      x-api-path-slug: downtime-post
      parameters:
      - in: query
        name: period
        description: how often to repeat as an integer
        type: string
      - in: query
        name: type
        description: the type of recurrence
        type: string
      - in: query
        name: until_date
        description: (optional) the date at which the recurrence should end as a POSIX
          timestmap
        type: string
      - in: query
        name: until_occurrences
        description: (optional) how many times the downtime will be rescheduled
        type: string
      - in: query
        name: week_days
        description: (optional) a list of week days to repeat on
        type: string
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Downtime
    get:
      summary: Get Downtime
      description: Get all monitor downtimes
      operationId: getDowntime
      x-api-path-slug: downtime-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Downtime
  /downtime/:downtime_id:
    put:
      summary: Put Downtime Downtime
      description: Update monitor downtime
      operationId: putDowntimeDowntime
      x-api-path-slug: downtimedowntime-id-put
      parameters:
      - in: query
        name: period
        description: how often to repeat as an integer
        type: string
      - in: query
        name: type
        description: the type of recurrence
        type: string
      - in: query
        name: until_date
        description: (optional) the date at which the recurrence should end as a POSIX
          timestmap
        type: string
      - in: query
        name: until_occurrences
        description: (optional) how many times the downtime will be rescheduled
        type: string
      - in: query
        name: week_days
        description: (optional) a list of week days to repeat on
        type: string
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Downtime
      - Downtime
    delete:
      summary: Delete Downtime Downtime
      description: DELETE downtime downtime
      operationId: deleteDowntimeDowntime
      x-api-path-slug: downtimedowntime-id-delete
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Downtime
      - Downtime
    get:
      summary: Get Downtime Downtime
      description: Get a monitor downtime
      operationId: getDowntimeDowntime
      x-api-path-slug: downtimedowntime-id-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Downtime
      - Downtime
  /screen:
    post:
      summary: Add Screen
      description: POST screen
      operationId: postScreen
      x-api-path-slug: screen-post
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Screen
    get:
      summary: Get Screen
      description: Fetch all of your screenboards' definitions.
      operationId: getScreen
      x-api-path-slug: screen-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Screen
  /screen/:board_id:
    put:
      summary: Put Screen Board
      description: PUT screen board
      operationId: putScreenBoard
      x-api-path-slug: screenboard-id-put
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Screen
      - Board
    delete:
      summary: Delete Screen Board
      description: Delete an existing screenboard.
      operationId: deleteScreenBoard
      x-api-path-slug: screenboard-id-delete
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Screen
      - Board
    get:
      summary: Get Screen Board
      description: Fetch an existing screenboard's definition.
      operationId: getScreenBoard
      x-api-path-slug: screenboard-id-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Screen
      - Board
  /screen/share/:board_id:
    get:
      summary: Get Screen Share Board
      description: Share an existing screenboard's with a public URL.
      operationId: getScreenShareBoard
      x-api-path-slug: screenshareboard-id-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Screen
      - Share
      - Board
    delete:
      summary: Delete Screen Share Board
      description: Revoke a currently shared screenboard's.
      operationId: deleteScreenShareBoard
      x-api-path-slug: screenshareboard-id-delete
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Screen
      - Share
      - Board
  /tags/hosts:
    get:
      summary: Get Tags Hosts
      description: Return a mapping of tags to hosts for your whole infrastructure.
      operationId: getTagsHosts
      x-api-path-slug: tagshosts-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tags
      - Hosts
  /tags/hosts/:host_name:
    get:
      summary: Get Tags Hosts Host Name
      description: Return the list of tags that apply to a given host.
      operationId: getTagsHostsHostName
      x-api-path-slug: tagshostshost-name-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tags
      - Hosts
      - Host
      - Name
    post:
      summary: Add Tags Hosts Host Name
      description: This end point allows you to add tags to a host.
      operationId: postTagsHostsHostName
      x-api-path-slug: tagshostshost-name-post
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tags
      - Hosts
      - Host
      - Name
    put:
      summary: Put Tags Hosts Host Name
      description: This end point allows you to update all tags for a given host.
      operationId: putTagsHostsHostName
      x-api-path-slug: tagshostshost-name-put
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tags
      - Hosts
      - Host
      - Name
    delete:
      summary: Delete Tags Hosts Host Name
      description: This end point allows you to remove all tags for a given host.
      operationId: deleteTagsHostsHostName
      x-api-path-slug: tagshostshost-name-delete
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tags
      - Hosts
      - Host
      - Name
  comments:
    post:
      summary: Add Comments
      description: |-
        Comments are essentially special forms of events that
                  appear in the stream. They can start a new discussion thread or
                  optionally, reply in another thread.
      operationId: postComments
      x-api-path-slug: comments-post
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Comments
  comments/:comment_id:
    put:
      summary: Put Comments Comment
      description: PUT comments comment
      operationId: putCommentsComment
      x-api-path-slug: commentscomment-id-put
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Comments
      - Comment
    delete:
      summary: Delete Comments Comment
      description: DELETE comments comment
      operationId: deleteCommentsComment
      x-api-path-slug: commentscomment-id-delete
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Comments
      - Comment
  graph/snapshot:
    get:
      summary: Get Graph Snapshot
      description: GET graph snapshot
      operationId: getGraphSnapshot
      x-api-path-slug: graphsnapshot-get
      parameters:
      - in: query
        name: graph_def
        description: can be used instead of metric_query
        type: string
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Graph
      - Snapshot
  /events:
    post:
      summary: Add Events
      description: Post an Event
      operationId: postEvents
      x-api-path-slug: events-post
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Events
  /events/:event_id:
    get:
      summary: Get Events Event
      description: GET events event
      operationId: getEventsEvent
      x-api-path-slug: eventsevent-id-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Events
      - Event
    delete:
      summary: Delete Events Event
      description: DELETE events event
      operationId: deleteEventsEvent
      x-api-path-slug: eventsevent-id-delete
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Events
      - Event
  /monitor:
    post:
      summary: Add Monitor
      description: Create a monitor
      operationId: postMonitor
      x-api-path-slug: monitor-post
      parameters:
      - in: query
        name: '#'
        description: an integer or decimal number used to set the              threshold
        type: string
      - in: query
        name: change_aggr
        description: change, pct_change
        type: string
      - in: query
        name: check
        description: name of the check, e
        type: string
      - in: query
        name: count
        description: must be at &gt;= your max threshold (defined              in
          the options)
        type: string
      - in: query
        name: escalation_message
        description: a message to include with a              re-notification
        type: string
      - in: query
        name: event
        description: ', the event query string:                                  string_query
          free text query to match against event title and text'
        type: string
      - in: query
        name: event alert
        type: string
      - in: query
        name: excluded_tags
        description: exluded event tags (comma-separated)
        type: string
      - in: query
        name: host
        description: event reporting host (comma-separated)
        type: string
      - in: query
        name: include_tags
        description: a boolean indicating whether              notifications from
          this monitor will automatically insert its              triggering tags
          into the title
        type: string
      - in: query
        name: key
        description: a key in key:value tag syntax; defines a              separate
          alert for each tag in the group (multi-alert)
        type: string
      - in: query
        name: last
        description: the timeframe to roll up the counts
        type: string
      - in: query
        name: locked
        description: a boolean indicating whether changes to              to this
          monitor should be restricted to the creator or admins
        type: string
      - in: query
        name: metric alert
        type: string
      - in: query
        name: notify_audit
        description: a boolean indicating whether tagged              users will be
          notified on changes to this monitor
        type: string
      - in: query
        name: notify_no_data
        description: a boolean indicating whether this              monitor will notify
          when data stops reporting
        type: string
      - in: query
        name: no_data_timeframe
        description: the number of minutes before a              monitor will notify
          when data stops reporting
        type: string
      - in: query
        name: operator
        description: '&lt;, &lt;=, &gt;, &gt;=, ==, or !='
        type: string
      - in: query
        name: priority
        description: event priorities (comma-separated)
        type: string
      - in: query
        name: renotify_interval
        description: the number of minutes after              the last notification
          before a monitor will re-notify on the              current status
        type: string
      - in: query
        name: require_full_window
        description: a boolean indicating whether              this monitor needs
          a full window of data before its evaluated
        type: string
      - in: query
        name: role:db
        description: 'for a short time:                      {role:db: 1412798116}'
        type: string
      - in: query
        name: rollup
        description: the stats rollup method
        type: string
      - in: query
        name: service check
        type: string
      - in: query
        name: silenced
        description: dictionary of scopes to timestamps or              None
        type: string
      - in: query
        name: sources
        description: event sources (comma-separated)
        type: string
      - in: query
        name: space_aggr
        description: avg, sum, min, or max
        type: string
      - in: query
        name: status
        description: event statuses (comma-separated)
        type: string
      - in: query
        name: tags
        description: one or more tags (comma-separated), or *
        type: string
      - in: query
        name: thresholds
        description: a dictionary of thresholds by threshold              type
        type: string
      - in: query
        name: timeout_h
        description: the number of hours of the monitor not              reporting
          data before it will automatically resolve from a              triggered
          state
        type: string
      - in: query
        name: timeshift
        description: '#m_ago (5, 10, 15, or 30),              #h_ago (1, 2, or 4),
          or 1d_ago'
        type: string
      - in: query
        name: time_aggr
        description: avg, sum, max, min
        type: string
      - in: query
        name: 'time_aggr(time_window):space_aggr:metric{tags} [by {key}] operator
          #'
        description: time_aggr avg, sum, max, min, change, or pct_change
        type: string
      - in: query
        name: time_window
        description: last_#m (5, 10, 15, or 30),              last_#h (1, 2, or 4),
          or last_1d
        type: string
      - in: query
        name: '[Triggered] Monitor Title'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Monitor
    get:
      summary: Get Monitor
      description: Get all monitor details
      operationId: getMonitor
      x-api-path-slug: monitor-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Monitor
  /monitor/:monitor_id:
    get:
      summary: Get Monitor Monitor
      description: GET monitor monitor
      operationId: getMonitorMonitor
      x-api-path-slug: monitormonitor-id-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Monitor
      - Monitor
    put:
      summary: Put Monitor Monitor
      description: PUT monitor monitor
      operationId: putMonitorMonitor
      x-api-path-slug: monitormonitor-id-put
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Monitor
      - Monitor
    delete:
      summary: Delete Monitor Monitor
      description: DELETE monitor monitor
      operationId: deleteMonitorMonitor
      x-api-path-slug: monitormonitor-id-delete
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Monitor
      - Monitor
  /monitor/mute_all:
    post:
      summary: Add Monitor Mute All
      description: |-
        Muting will prevent all monitors from notifying through email and posts
                to the event stream. State changes will only be visible by checking
                the alert page.
      operationId: postMonitorMuteAll
      x-api-path-slug: monitormute-all-post
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Monitor
      - Mute
      - All
  /monitor/unmute_all:
    post:
      summary: Add Monitor Unmute All
      description: |-
        Disables muting all monitors. Throws an error if mute all was
                not enabled previously.
      operationId: postMonitorUnmuteAll
      x-api-path-slug: monitorunmute-all-post
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Monitor
      - Unmute
      - All
  /monitor/:monitor_id/mute:
    post:
      summary: Add Monitor Monitor  Mute
      description: POST monitor monitor  mute
      operationId: postMonitorMonitorMute
      x-api-path-slug: monitormonitor-idmute-post
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Monitor
      - Monitor
      - ""
      - Mute
  /dash:
    post:
      summary: Add Dash
      description: Create a Timeboard
      operationId: postDash
      x-api-path-slug: dash-post
      parameters:
      - in: query
        name: '{requests: [{q: system.cpu.idle{} by {host}}'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Dash
    get:
      summary: Get Dash
      description: Get all Timeboards
      operationId: getDash
      x-api-path-slug: dash-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Dash
  /dash/:dash_id:
    put:
      summary: Put Dash Dash
      description: Update a Timeboard
      operationId: putDashDash
      x-api-path-slug: dashdash-id-put
      parameters:
      - in: query
        name: '{requests: [{q: system.cpu.idle{} by {host}}'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Dash
      - Dash
    delete:
      summary: Delete Dash Dash
      description: Delete a Timeboard
      operationId: deleteDashDash
      x-api-path-slug: dashdash-id-delete
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Dash
      - Dash
  user:
    post:
      summary: Add User
      description: POST user
      operationId: postUser
      x-api-path-slug: user-post
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
    get:
      summary: Get User
      description: GET user
      operationId: getUser
      x-api-path-slug: user-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
  user/:handle:
    get:
      summary: Get User Handle
      description: GET user handle
      operationId: getUserHandle
      x-api-path-slug: userhandle-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Handle
    put:
      summary: Put User Handle
      description: Can only be used with application keys belonging to administrators.
      operationId: putUserHandle
      x-api-path-slug: userhandle-put
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Handle
  graph/embed:
    get:
      summary: Get Graph Embed
      description: Gets a list of previously created embeddable graphs.
      operationId: getGraphEmbed
      x-api-path-slug: graphembed-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Graph
      - Embed
    post:
      summary: Add Graph Embed
      description: Creates a new embeddable graph.
      operationId: postGraphEmbed
      x-api-path-slug: graphembed-post
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Graph
      - Embed
  graph/embed/:embed_id:
    get:
      summary: Get Graph Embed Embed
      description: Get the HTML fragment for a previously generated embed with embed_id.
      operationId: getGraphEmbedEmbed
      x-api-path-slug: graphembedembed-id-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Graph
      - Embed
      - Embed
  graph/embed/:embed_id/enable:
    get:
      summary: Get Graph Embed Embed  Enable
      description: Enable a specified embed.
      operationId: getGraphEmbedEmbedEnable
      x-api-path-slug: graphembedembed-idenable-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Graph
      - Embed
      - Embed
      - ""
      - Enable