swagger: "2.0"
x-collection-name: BMC Software
x-complete: 1
info:
  title: BMC Software Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account:
    get:
      summary: Account Resource
      description: Information about the authorized account.
      operationId: information-about-the-authorized-account
      x-api-path-slug: account-get
      responses:
        200:
          description: OK
      tags:
      - Account
  ? '/events?message={message}&amp;severity={severity}&amp;timestamp_utc_from={timestamp_utc_from}&amp;timestamp_utc_to={timestamp_utc_to} '
  : ' get ':
      summary: Events?message={message}&amp;severity={severity}&amp;timestamp_utc_from={timestamp_utc_from}&amp;timestamp_utc_to={timestamp_utc_to}
      description: Gets a list of events for the current user.
      operationId: -eventsmessagemessageampseverityseverityamptimestamp-utc-fromtimestamp-utc-fromamptimestamp-utc-toti
      x-api-path-slug: eventsmessagemessageampseverityseverityamptimestamp-utc-fromtimestamp-utc-fromamptimestamp-utc-totimestamp-utc-to-get
      responses:
        200:
          description: OK
      tags:
      - Custom Events
  '/custom_events ':
    ' post ':
      summary: Custom Events
      description: Creates new custom event.
      operationId: -custom-events-
      x-api-path-slug: custom-events-post
      responses:
        200:
          description: OK
      tags:
      - Custom Events
  '/custom_events/all?fromUtc={fromUtc}&amp;toUtc={toUtc} ':
    ' get ':
      summary: Custom Events
      description: Gets all custom events using optional filter.
      operationId: -custom-events-allfromutcfromutcamptoutctoutc-
      x-api-path-slug: custom-eventsallfromutcfromutcamptoutctoutc-get
      responses:
        200:
          description: OK
      tags:
      - Custom Events
  '/custom_events/{id} ':
    ' get ':
      summary: Custom_events {id}
      description: Gets custom event by Id.
      operationId: -custom-events-id-
      x-api-path-slug: custom-eventsid-get
      responses:
        200:
          description: OK
      tags:
      - Custom Events
    ' put ':
      summary: Custom_events {id}
      description: Updates custom event.
      operationId: -custom-events-id-
      x-api-path-slug: custom-eventsid-put
      responses:
        200:
          description: OK
      tags:
      - Custom Events
    ' delete ':
      summary: Custom_events {id}
      description: Deletes custom event.
      operationId: -custom-events-id-
      x-api-path-slug: custom-eventsid-delete
      responses:
        200:
          description: OK
      tags:
      - Custom Events
  /v1/account/aws/status:
    get:
      summary: Get AWS Integration Status
      description: Gets AWS status
      operationId: get-aws-integration-status
      x-api-path-slug: v1accountawsstatus-get
      responses:
        200:
          description: OK
      tags:
      - Account
  /v1/actions:
    get:
      summary: Get all available action types
      description: Gets all known action types
      operationId: get-all-available-action-types
      x-api-path-slug: v1actions-get
      responses:
        200:
          description: OK
      tags:
      - Actions
  /v1/actions/installed:
    get:
      summary: Get all installed actions
      description: Gets all actions that are installed for the project
      operationId: get-all-installed-actions
      x-api-path-slug: v1actionsinstalled-get
      responses:
        200:
          description: OK
      tags:
      - Actions
    put:
      summary: Install action
      description: Installs an action
      operationId: install-action
      x-api-path-slug: v1actionsinstalled-put
      responses:
        200:
          description: OK
      tags:
      - Actions
  /v1/actions/installed/:actionId:
    get:
      summary: Get details of an installed action
      description: Gets a single action definition
      operationId: get-details-of-an-installed-action
      x-api-path-slug: v1actionsinstalledactionid-get
      parameters:
      - in: query
        name: |-
          actionId
          Name of plugin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Actions
    delete:
      summary: Uninstall action
      description: Uninstalls an action and remove it from the associated alarms(s).
      operationId: uninstall-action
      x-api-path-slug: v1actionsinstalledactionid-delete
      responses:
        200:
          description: OK
      tags:
      - Actions
  /v1/actions/installed/:actionId/alarms:
    get:
      summary: Get all alarms using an action
      description: Get alarms that are using this action installed for the project
      operationId: get-all-alarms-using-an-action
      x-api-path-slug: v1actionsinstalledactionidalarms-get
      responses:
        200:
          description: OK
      tags:
      - Actions
  /v1/actions/:action:
    get:
      summary: Get action
      description: Gets a single action type
      operationId: get-action
      x-api-path-slug: v1actionsaction-get
      parameters:
      - in: query
        name: |-
          action
          Name of plugin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Actions
  /v1/alarms:
    get:
      summary: Get All Alarms
      description: Get all of the Alarms
      operationId: get-all-alarms
      x-api-path-slug: v1alarms-get
      responses:
        200:
          description: OK
      tags:
      - Alarms
    post:
      summary: Create Alarm
      description: Create an Alarm
      operationId: create-alarm
      x-api-path-slug: v1alarms-post
      parameters:
      - in: formData
        name: name
        description: The name of the alarm
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
  /v1/alarm/:alarmId:
    get:
      summary: Get Alarm by Id
      description: Retrieves a single alarm
      operationId: get-alarm-by-id
      x-api-path-slug: v1alarmalarmid-get
      parameters:
      - in: query
        name: alarmId
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
    put:
      summary: Update Alarm
      description: Update an Alarm
      operationId: update-alarm
      x-api-path-slug: v1alarmalarmid-put
      parameters:
      - in: formData
        name: name
        description: The name of the alarm
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
    delete:
      summary: Delete Alarm
      description: Deletes an alarm
      operationId: delete-alarm
      x-api-path-slug: v1alarmalarmid-delete
      parameters:
      - in: query
        name: |-
          alarmId
          The alarm to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
  /v1/alarms/search:
    get:
      summary: Get Alarms by Name
      description: Retrieves alarms by name
      operationId: get-alarms-by-name
      x-api-path-slug: v1alarmssearch-get
      parameters:
      - in: query
        name: alarmName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
  /v2/alarms:
    post:
      summary: Create Alarm
      description: Create an Alarm
      operationId: create-alarm
      x-api-path-slug: v2alarms-post
      responses:
        200:
          description: OK
      tags:
      - Alarms
    get:
      summary: Get All Alarms
      description: Get all of the Alarms
      operationId: get-all-alarms
      x-api-path-slug: v2alarms-get
      responses:
        200:
          description: OK
      tags:
      - Alarms
  /v2/alarms/:alarmId:
    put:
      summary: Update Alarm
      description: Updates an alarm
      operationId: update-alarm
      x-api-path-slug: v2alarmsalarmid-put
      parameters:
      - in: query
        name: |-
          alarmId integer
          The alarm to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
    get:
      summary: Get Alarm by Id
      description: Retrieves a single alarm
      operationId: get-alarm-by-id
      x-api-path-slug: v2alarmsalarmid-get
      parameters:
      - in: query
        name: alarmId
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
    delete:
      summary: Delete Alarm
      description: Deletes an alarm
      operationId: delete-alarm
      x-api-path-slug: v2alarmsalarmid-delete
      parameters:
      - in: query
        name: |-
          alarmId
          The alarm to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alarms
  /v1/batch:
    post:
      summary: Perform batch
      description: |-
        Allows making an arbitrary set of API calls.    All calls are made in parallel.
        The query string parameter <em>?series</em> can be used to override this behavior and call the API in series stopping at the first error.
      operationId: perform-batch
      x-api-path-slug: v1batch-post
      responses:
        200:
          description: OK
      tags:
      - Batch
  /v1/mobile-devices/:userDeviceId:
    delete:
      summary: Delete Mobile Device
      description: Deletes a device from a user
      operationId: delete-mobile-device
      x-api-path-slug: v1mobiledevicesuserdeviceid-delete
      parameters:
      - in: query
        name: |-
          userDeviceId
          The user device ID to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /v1/account/mobile-devices/:accountDeviceId:
    delete:
      summary: Delete Account Mobile Device
      description: Deletes a device from an account
      operationId: delete-account-mobile-device
      x-api-path-slug: v1accountmobiledevicesaccountdeviceid-delete
      parameters:
      - in: query
        name: |-
          accountDeviceId
          The account device ID to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account
  /v1/account/mobile-devices:
    get:
      summary: Get All Account Mobile Devices
      description: Gets all of the devices for an account
      operationId: get-all-account-mobile-devices
      x-api-path-slug: v1accountmobiledevices-get
      responses:
        200:
          description: OK
      tags:
      - Account
  /v1/datasets/*:
    get:
      summary: List dataset
      description: '*'
      operationId: list-dataset
      x-api-path-slug: v1datasets-get
      responses:
        200:
          description: OK
      tags:
      - Datasets
  /v1/events:
    post:
      summary: Create event
      description: Creates an event. Every event occurrence is persisted to the database
        as a RawEvent. Based on the EventFingerprint, a new Event will be created
        or an existing one will be de-duplicated.
      operationId: create-event
      x-api-path-slug: v1events-post
      responses:
        200:
          description: OK
      tags:
      - Events
    get:
      summary: List events
      description: Searches for events in the specified organization.
      operationId: list-events
      x-api-path-slug: v1events-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /v1/events/raw:
    get:
      summary: List raw events
      description: Queries all event occurrences (raw events) for the specified organization.
      operationId: list-raw-events
      x-api-path-slug: v1eventsraw-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /v1/events/:event_id:
    get:
      summary: Get event
      description: Returns the event with the specified event id from the database.
      operationId: get-event
      x-api-path-slug: v1eventsevent-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /v1/events/:event_id/raw:
    get:
      summary: Get raw events
      description: Returns all of the event occurrences (raw events) for the specified
        event.
      operationId: get-raw-events
      x-api-path-slug: v1eventsevent-idraw-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /v1/hostgroups:
    get:
      summary: Get All Hostgroups
      description: Get all of the Hostgroups in your account
      operationId: get-all-hostgroups
      x-api-path-slug: v1hostgroups-get
      responses:
        200:
          description: OK
      tags:
      - Hostgroups
    post:
      summary: Create Hostgroup
      description: Create a Hostgroup
      operationId: create-hostgroup
      x-api-path-slug: v1hostgroups-post
      responses:
        200:
          description: OK
      tags:
      - Hostgroups
  /v1/hostgroups/search:
    get:
      summary: Search Hostgroups
      description: Searches the hostgroups in your account
      operationId: search-hostgroups
      x-api-path-slug: v1hostgroupssearch-get
      parameters:
      - in: query
        name: |-
          name
          The hostgroup name to search for.  Currently supported search parameters:

          name - search by the name of the hostgroup
        type: string
      responses:
        200:
          description: OK
      tags:
      - Hostgroups
  /v1/hostgroups/:hostgroupId:
    get:
      summary: Get Hostgroup by Id
      description: Retrieves a single hostgroup by its id
      operationId: get-hostgroup-by-id
      x-api-path-slug: v1hostgroupshostgroupid-get
      parameters:
      - in: query
        name: |-
          hostgroupId
          The Id of the hostgroup you are requesting
        type: string
      responses:
        200:
          description: OK
      tags:
      - Hostgroups
    put:
      summary: Update Hostgroup
      description: Update a Hostgroup
      operationId: update-hostgroup
      x-api-path-slug: v1hostgroupshostgroupid-put
      responses:
        200:
          description: OK
      tags:
      - Hostgroups
    delete:
      summary: Delete Hostgroup
      description: Delete an hostgroup
      operationId: delete-hostgroup
      x-api-path-slug: v1hostgroupshostgroupid-delete
      parameters:
      - in: query
        name: |-
          hostgroupId
          The hostgroup to delete
          forceRemove
          Remove the hostgroup, even if it&#39;s being used by a dashboard or alarm
        type: string
      responses:
        200:
          description: OK
      tags:
      - Hostgroups
  /v1/meter/:meterName/registration:
    post:
      summary: Registration
      description: Register a Meter with TrueSight Pulse
      operationId: registration
      x-api-path-slug: v1metermeternameregistration-post
      parameters:
      - in: formData
        name: meterVersion
        description: What version of the Meter is running, ex
        type: string
      responses:
        200:
          description: OK
      tags:
      - Meters
  /v1/measurements:
    post:
      summary: Add measures
      description: Adds measurement readings to the data store.
      operationId: add-measures
      x-api-path-slug: v1measurements-post
      parameters:
      - in: formData
        name: source
        description: The source of the metric
        type: string
      responses:
        200:
          description: OK
      tags:
      - Measurements
  /v1/metrics:
    post:
      summary: Create metric
      description: Creates a new metric
      operationId: create-metric
      x-api-path-slug: v1metrics-post
      parameters:
      - in: formData
        name: |-
          name
          Name of the metric, must be globally unique, recommended that you add your own namespace
        description: typeType of metric, could be a device metric, a plugin metric
          or any arbitrary type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metrics
    get:
      summary: Get Metrics
      description: Retrieves the list of metrics in a project.
      operationId: get-metrics
      x-api-path-slug: v1metrics-get
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /v1/batch/metrics:
    post:
      summary: Create metrics batch
      description: Creates metrics, but in a batch
      operationId: create-metrics-batch
      x-api-path-slug: v1batchmetrics-post
      responses:
        200:
          description: OK
      tags:
      - Batch
    put:
      summary: Update metrics batch
      description: Updates a batch of metrics
      operationId: update-metrics-batch
      x-api-path-slug: v1batchmetrics-put
      parameters:
      - in: formData
        name: |-
          type
          Type of metric, could be a device metric, a plugin metric or any arbitrary type
        description: descriptionDescription of the metric
        type: string
      responses:
        200:
          description: OK
      tags:
      - Batch
  /v1/measurements/:metric:
    get:
      summary: Get measures
      description: Retrieves measurement readings.
      operationId: get-measures
      x-api-path-slug: v1measurementsmetric-get
      responses:
        200:
          description: OK
      tags:
      - Measurements
  /v1/measurementsBatch:
    post:
      summary: Get measures batch
      description: Same as /v1/measurements/:metric except that an array of query
        objects are passed in the body.
      operationId: get-measures-batch
      x-api-path-slug: v1measurementsbatch-post
      responses:
        200:
          description: OK
      tags:
      - Measurements
  /v1/metrics/:metric:
    delete:
      summary: Remove metric
      description: |-
        Removes a metric from the account.
         Note that a metric will not deleted if it has been alarmed unless that <em>removeAlarms</em>
         flag is added.
      operationId: remove-metric
      x-api-path-slug: v1metricsmetric-delete
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /v1/metrics/dashactions/:dashboardSetId:
    get:
      summary: Get actions for a dashboard
      description: |-
        Retrieves the needed configuration changes for a dashboard
         Returns an an array of objects, each has the following properties:
      operationId: get-actions-for-a-dashboard
      x-api-path-slug: v1metricsdashactionsdashboardsetid-get
      responses:
        200:
          description: OK
      tags:
      - Metrics
    post:
      summary: Perform dashboard actions
      description: |-
        Performs necessary actions for a dashboard.
         Only enables or adds metrics at this time.
      operationId: perform-dashboard-actions
      x-api-path-slug: v1metricsdashactionsdashboardsetid-post
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /v1/metrics/:metricName:
    put:
      summary: Update metric
      description: Updates a metric
      operationId: update-metric
      x-api-path-slug: v1metricsmetricname-put
      parameters:
      - in: formData
        name: |-
          type
          Type of metric, could be a device metric, a plugin metric or any arbitrary type
        description: descriptionDescription of the metric
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /v1/plugins:
    get:
      summary: Get all plugins
      description: Gets all known plugin definitions
      operationId: get-all-plugins
      x-api-path-slug: v1plugins-get
      responses:
        200:
          description: OK
      tags:
      - Plugins
  /v1/plugins/:plugin/components:
    get:
      summary: Get plugin components
      description: Finds the components associated with an installed plugin including
        metrics and dashboards
      operationId: get-plugin-components
      x-api-path-slug: v1pluginsplugincomponents-get
      responses:
        200:
          description: OK
      tags:
      - Plugins
  /v1/plugins/installed:
    get:
      summary: Get installed plugins
      description: Gets plugins that are installed for the project
      operationId: get-installed-plugins
      x-api-path-slug: v1pluginsinstalled-get
      responses:
        200:
          description: OK
      tags:
      - Plugins
  /v1/plugins/installed/:plugin:
    put:
      summary: Install or update plugin
      description: Installs a plugin
      operationId: install-or-update-plugin
      x-api-path-slug: v1pluginsinstalledplugin-put
      responses:
        200:
          description: OK
      tags:
      - Plugins
    delete:
      summary: Uninstall plugin
      description: Uninstalls a plugin and optionally removes related dashboard(s)
        and metric(s).
      operationId: uninstall-plugin
      x-api-path-slug: v1pluginsinstalledplugin-delete
      responses:
        200:
          description: OK
      tags:
      - Plugins
  /v1/plugins/private/:plugin/:org/:repo:
    put:
      summary: Add private plugin
      description: |-
        Adds or updates a private plugin.
        A plugin exists as a repository in Github.
        By adding a private plugin the plugin will appear on your settings -&gt; plugins tab just like any other plugin which
        can then be installed and/or added to a relay.
        If a private plugin has the same name as an existing plugin it will override the existing plugin within your account.
      operationId: add-private-plugin
      x-api-path-slug: v1pluginsprivatepluginorgrepo-put
      parameters:
      - in: query
        name: |-
          plugin
          Name of the plugin
          org
          Github organization or user owning the plugin
          repo
          Github repository name for plugin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Plugins
  /v1/plugins/private/:plugin:
    delete:
      summary: Remove private plugin
      description: |-
        Removes a private plugin from your account. Use this function after adding a private plugin to make your private
        plugin disappear from available plugins in your settings.
      operationId: remove-private-plugin
      x-api-path-slug: v1pluginsprivateplugin-delete
      parameters:
      - in: query
        name: |-
          plugin
          Name of plugin to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - Plugins
  /v1/plugins/:plugin:
    get:
      summary: Get plugin
      description: Gets a single plugin definition
      operationId: get-plugin
      x-api-path-slug: v1pluginsplugin-get
      parameters:
      - in: query
        name: |-
          plugin
          Name of plugin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Plugins
  /v1/relays/heartbeat:
    post:
      summary: Set Relay Heartbeat
      description: |-
        Updates the &#39;lastHeardFrom&#39; field of the relay configuration
        Returns the current system time in UNIX epoch of server.
      operationId: set-relay-heartbeat
      x-api-path-slug: v1relaysheartbeat-post
      responses:
        200:
          description: OK
      tags:
      - Relays
  /v1/relays:
    get:
      summary: Get All Relay Configurations
      description: Gets the configurations for all visible relays
      operationId: get-all-relay-configurations
      x-api-path-slug: v1relays-get
      responses:
        200:
          description: OK
      tags:
      - Relays
  /v1/relays/:relay/config:
    get:
      summary: Get Relay Configuration
      description: |-
        Retrieves config for a relay host if changed
        If no timestamp specified, configuration data is always returned
        If config has not changed the string &#39;not-modified&#39; is returned
      operationId: get-relay-configuration
      x-api-path-slug: v1relaysrelayconfig-get
      responses:
        200:
          description: OK
      tags:
      - Relays
    put:
      summary: Set Relay Configuration
      description: |-
        Stores configuration for a relay.
         The relay will gather the configuration on the next poll and reconfigure itself as needed.
      operationId: set-relay-configuration
      x-api-path-slug: v1relaysrelayconfig-put
      responses:
        200:
          description: OK
      tags:
      - Relays
  /v1/relays/:relay/toggle:
    post:
      summary: Toggle relay
      description: Set a relay to be disabled or enabled
      operationId: toggle-relay
      x-api-path-slug: v1relaysrelaytoggle-post
      parameters:
      - in: formData
        name: disabled
        description: true or false
        type: string
      - in: query
        name: |-
          relay
          Name of relay to toggle
        type: string
      responses:
        200:
          description: OK
      tags:
      - Relays
  /v1/relays/:relay/togglePlugin:
    post:
      summary: Toggle relay plugin
      description: Sets a relay plugin to be disabled or enabled
      operationId: toggle-relay-plugin
      x-api-path-slug: v1relaysrelaytoggleplugin-post
      parameters:
      - in: formData
        name: plugin
        description: Name of plugin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Relays
  /v1/relays/:relay/output:
    post:
      summary: Add relay output
      description: |-
        Adds output messages to the relay.
        Used by the relay to communicate output from execution and commands
      operationId: add-relay-output
      x-api-path-slug: v1relaysrelayoutput-post
      responses:
        200:
          description: OK
      tags:
      - Relays
    delete:
      summary: Clear relay output
      description: Wipes the logged output from the relay up to present.
      operationId: clear-relay-output
      x-api-path-slug: v1relaysrelayoutput-delete
      responses:
        200:
          description: OK
      tags:
      - Relays
  /v1/relays/:relay/output/:since:
    get:
      summary: Get relay output
      description: Queries for relay output messages.
      operationId: get-relay-output
      x-api-path-slug: v1relaysrelayoutputsince-get
      responses:
        200:
          description: OK
      tags:
      - Relays
  /v1/sources/byName:
    delete:
      summary: Remove Old Sources By Name
      description: Remove Old Sources from your account by using a list of names
      operationId: remove-old-sources-by-name
      x-api-path-slug: v1sourcesbyname-delete
      parameters:
      - in: formData
        name: names
        description: An array of source names to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Sources
  /v1/account/sources/:lastModified?:
    get:
      summary: Get all source information
      description: Gets all source (host + data stream) information
      operationId: get-all-source-information
      x-api-path-slug: v1accountsourceslastmodified-get
      responses:
        200:
          description: OK
      tags:
      - Account
  /v1/account/sources:
    put:
      summary: Set source metadata
      description: Sets one or more source metadata
      operationId: set-source-metadata
      x-api-path-slug: v1accountsources-put
      responses:
        200:
          description: OK
      tags:
      - Account
  /metrics:
    get:
      summary: Get list of active metrics
      description: Get the list of actively reporting metrics from a given time until
        now. This endpoint is not available in the Python and Ruby libraries.
      operationId: get-list-of-active-metrics
      x-api-path-slug: metrics-get
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
      - ""
  /api/v1/events:
    post:
      summary: Post an Event
      description: This end point allows you to post events to the stream. You can
        tag them, set priority and event aggregate them with other events.
      operationId: post-an-event
      x-api-path-slug: apiv1events-post
      responses:
        200:
          description: OK
      tags:
      - ""
  ? |2-

        /api/{version}/actions
  : ? |2-

          get
    : summary: Get Actions (Alerts) List
      description: Returns a list of actions (alerts) that have been generated for
        your account.
      operationId: get-actions-alerts-list
      x-api-path-slug: apiversionactions-get
      parameters:
      - in: query
        name: checkids
        description: Comma-separated list of check identifiers
        type: <td>string</td>
      - in: query
        name: contactids
        description: Comma-separated list of contact identifiers
        type: <td>string</td>
      - in: query
        name: from
        description: Only include actions generated later than this timestamp
        type: <td>integer</td>
      - in: query
        name: limit
        description: Limits the number of returned results to the specified quantity
        type: <td>integer (max 300)</td>
      - in: query
        name: offset
        description: Offset for listing
        type: <td>integer</td>
      - in: query
        name: status
        description: Comma-separated list of statuses
        type: <td>string (sent, delivered, error, not_deliv
      - in: query
        name: to
        description: Only include actions generated prior to this timestamp
        type: <td>integer</td>
      - in: query
        name: via
        description: Comma-separated list of via mediums
        type: <td>string (email, sms, twitter, iphone, andr
      responses:
        200:
          description: OK
      tags:
      - Actions
  /metrics/definitions:
    "":
      summary: Available metrics
      description: Determine which metrics are available to return historical data
        for, for a specific subject (device or service) over a specific time range.
      operationId: available-metrics
      x-api-path-slug: metricsdefinitions-
      parameters:
      - in: query
        name: end
        description: The UTC date string for the end time range in format YYYY-MM-DDTHH:mm:SSZ
          e
        type: string
      - in: query
        name: start
        description: The UTC date string for the start time range in format YYYY-MM-DDTHH:mm:SSZ
          e
        type: string
      - in: query
        name: subjectId
        description: The ID of the subject to get the definitions for, e
        type: string
      - in: query
        name: token
        description: Your API token
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /metrics/dynamicgraphs/:
    "":
      summary: Dynamic metrics
      description: Return historical metrics data, for a devices and/or services that
        match a search or regex style inventory filter search over a specific time
        range.
      operationId: dynamic-metrics
      x-api-path-slug: metricsdynamicgraphs-
      parameters:
      - in: query
        name: end
        description: The UTC date string for the end time range in format YYYY-MM-DDTHH:mm:SSZ
          e
        type: string
      - in: query
        name: ids
        description: List of inventory IDs
        type: string
      - in: query
        name: inventoryFilter
        description: A regular expression that will return all devices or services
          that match the pattern
        type: string
      - in: query
        name: names
        description: Human-readable names of a device or service
        type: string
      - in: query
        name: start
        description: The UTC date string for the start time range in format YYYY-MM-DDTHH:mm:SSZ
          e
        type: string
      - in: query
        name: token
        description: Your API token
        type: string
      - in: query
        name: type
        description: Specify whether to return only devices, services or all
        type: string
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /actions:
    post:
      summary: Create Action
      description: Create a new Action.
      operationId: create-action
      x-api-path-slug: actions-post
      parameters:
      - in: path
        name: "action_name\n        \n        \n            required\n            Display
          name for the Action.\n        \n    \n    \n        \n        action_url\n
          \       \n        \n            required\n            URL to be invoked
          for action execution."
      responses:
        200:
          description: OK
      tags:
      - Actions
    get:
      summary: List Actions
      description: List of all Actions.
      operationId: list-actions
      x-api-path-slug: actions-get
      parameters:
      - in: path
        name: "maintenance_id\n        \n        \n            string\n            Unique
          ID generated by the server. This can be used as an identifier.\n        \n
          \               \n    \n        \n        display_name\n        \n        \n
          \           string\n            Displa"
      responses:
        200:
          description: OK
      tags:
      - Actions
  /actions/{action_id}:
    put:
      summary: Update Action
      description: Update an existing Action.
      operationId: update-action
      x-api-path-slug: actionsaction-id-put
      parameters:
      - in: path
        name: "action_name\n        \n        \n            required\n            Display
          name for the Action.\n        \n    \n    \n        \n        action_url\n
          \       \n        \n            required\n            URL to be invoked
          for action execution."
      responses:
        200:
          description: OK
      tags:
      - Actions