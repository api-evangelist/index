swagger: "2.0"
x-collection-name: Google Calendar
x-complete: 1
info:
  title: Google Calendar
  description: manipulates-events-and-other-calendar-data-
  contact:
    name: Google
    url: https://google.com
  version: v3/
host: www.googleapis.com
basePath: /calendar/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calendars:
    post:
      summary: Create Calendar
      description: Creates a secondary calendar.
      operationId: calendar.calendars.insert
      x-api-path-slug: calendars-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Calendar
  /calendars/{calendarId}:
    delete:
      summary: CreaDeletete Calendar
      description: Deletes a secondary calendar. Use calendars.clear for clearing
        all events on primary calendars.
      operationId: calendar.calendars.delete
      x-api-path-slug: calendarscalendarid-delete
      parameters:
      - in: path
        name: calendarId
        description: Calendar identifier
      responses:
        200:
          description: OK
      tags:
      - Calendar
    get:
      summary: Get Calendar
      description: Returns metadata for a calendar.
      operationId: calendar.calendars.get
      x-api-path-slug: calendarscalendarid-get
      parameters:
      - in: path
        name: calendarId
        description: Calendar identifier
      responses:
        200:
          description: OK
      tags:
      - Calendar
    patch:
      summary: Update Calendar
      description: Updates metadata for a calendar. This method supports patch semantics.
      operationId: calendar.calendars.patch
      x-api-path-slug: calendarscalendarid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: calendarId
        description: Calendar identifier
      responses:
        200:
          description: OK
      tags:
      - Calendar
    put:
      summary: Update Calendar
      description: Updates metadata for a calendar.
      operationId: calendar.calendars.update
      x-api-path-slug: calendarscalendarid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: calendarId
        description: Calendar identifier
      responses:
        200:
          description: OK
      tags:
      - Calendar
  /calendars/{calendarId}/acl:
    get:
      summary: Get Calendar ACL
      description: Returns the rules in the access control list for the calendar.
      operationId: calendar.acl.list
      x-api-path-slug: calendarscalendaridacl-get
      parameters:
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: query
        name: maxResults
        description: Maximum number of entries returned on one result page
      - in: query
        name: pageToken
        description: Token specifying which result page to return
      - in: query
        name: showDeleted
        description: Whether to include deleted ACLs in the result
      - in: query
        name: syncToken
        description: Token obtained from the nextSyncToken field returned on the last
          page of results from the previous list request
      responses:
        200:
          description: OK
      tags:
      - Calendar ACL
    post:
      summary: Create Calendar ACL
      description: Creates an access control rule.
      operationId: calendar.acl.insert
      x-api-path-slug: calendarscalendaridacl-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: calendarId
        description: Calendar identifier
      responses:
        200:
          description: OK
      tags:
      - Calendar ACL
  /calendars/{calendarId}/acl/watch:
    post:
      summary: Watch Calendar ACL
      description: Watch for changes to ACL resources.
      operationId: calendar.acl.watch
      x-api-path-slug: calendarscalendaridaclwatch-post
      parameters:
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: query
        name: maxResults
        description: Maximum number of entries returned on one result page
      - in: query
        name: pageToken
        description: Token specifying which result page to return
      - in: body
        name: resource
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: showDeleted
        description: Whether to include deleted ACLs in the result
      - in: query
        name: syncToken
        description: Token obtained from the nextSyncToken field returned on the last
          page of results from the previous list request
      responses:
        200:
          description: OK
      tags:
      - Calendar ACL
  /calendars/{calendarId}/acl/{ruleId}:
    delete:
      summary: Delete Calendar ACL
      description: Deletes an access control rule.
      operationId: calendar.acl.delete
      x-api-path-slug: calendarscalendaridaclruleid-delete
      parameters:
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: path
        name: ruleId
        description: ACL rule identifier
      responses:
        200:
          description: OK
      tags:
      - Calendar ACL
    get:
      summary: Get Calendar ACL
      description: Returns an access control rule.
      operationId: calendar.acl.get
      x-api-path-slug: calendarscalendaridaclruleid-get
      parameters:
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: path
        name: ruleId
        description: ACL rule identifier
      responses:
        200:
          description: OK
      tags:
      - Calendar ACL
    patch:
      summary: Update Calendar ACL
      description: Updates an access control rule. This method supports patch semantics.
      operationId: calendar.acl.patch
      x-api-path-slug: calendarscalendaridaclruleid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: path
        name: ruleId
        description: ACL rule identifier
      responses:
        200:
          description: OK
      tags:
      - Calendar ACL
    put:
      summary: Update Calendar ACL
      description: Updates an access control rule.
      operationId: calendar.acl.update
      x-api-path-slug: calendarscalendaridaclruleid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: path
        name: ruleId
        description: ACL rule identifier
      responses:
        200:
          description: OK
      tags:
      - Calendar ACL
  /calendars/{calendarId}/clear:
    post:
      summary: Clear Primary Calendar
      description: Clears a primary calendar. This operation deletes all events associated
        with the primary calendar of an account.
      operationId: calendar.calendars.clear
      x-api-path-slug: calendarscalendaridclear-post
      parameters:
      - in: path
        name: calendarId
        description: Calendar identifier
      responses:
        200:
          description: OK
      tags:
      - Calendar
  /calendars/{calendarId}/events:
    get:
      summary: Get Events
      description: Returns events on the specified calendar.
      operationId: calendar.events.list
      x-api-path-slug: calendarscalendaridevents-get
      parameters:
      - in: query
        name: alwaysIncludeEmail
        description: Whether to always include a value in the email field for the
          organizer, creator and attendees, even if no real email is available (i
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: query
        name: iCalUID
        description: Specifies event ID in the iCalendar format to be included in
          the response
      - in: query
        name: maxAttendees
        description: The maximum number of attendees to include in the response
      - in: query
        name: maxResults
        description: Maximum number of events returned on one result page
      - in: query
        name: orderBy
        description: The order of the events returned in the result
      - in: query
        name: pageToken
        description: Token specifying which result page to return
      - in: query
        name: privateExtendedProperty
        description: Extended properties constraint specified as propertyName=value
      - in: query
        name: q
        description: Free text search terms to find events that match these terms
          in any field, except for extended properties
      - in: query
        name: sharedExtendedProperty
        description: Extended properties constraint specified as propertyName=value
      - in: query
        name: showDeleted
        description: Whether to include deleted events (with status equals cancelled)
          in the result
      - in: query
        name: showHiddenInvitations
        description: Whether to include hidden invitations in the result
      - in: query
        name: singleEvents
        description: Whether to expand recurring events into instances and only return
          single one-off events and instances of recurring events, but not the underlying
          recurring events themselves
      - in: query
        name: syncToken
        description: Token obtained from the nextSyncToken field returned on the last
          page of results from the previous list request
      - in: query
        name: timeMax
        description: Upper bound (exclusive) for an events start time to filter by
      - in: query
        name: timeMin
        description: Lower bound (inclusive) for an events end time to filter by
      - in: query
        name: timeZone
        description: Time zone used in the response
      - in: query
        name: updatedMin
        description: Lower bound for an events last modification time (as a RFC3339
          timestamp) to filter by
      responses:
        200:
          description: OK
      tags:
      - Event
    post:
      summary: Create Event
      description: Creates an event.
      operationId: calendar.events.insert
      x-api-path-slug: calendarscalendaridevents-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: query
        name: maxAttendees
        description: The maximum number of attendees to include in the response
      - in: query
        name: sendNotifications
        description: Whether to send notifications about the creation of the new event
      - in: query
        name: supportsAttachments
        description: Whether API client performing operation supports event attachments
      responses:
        200:
          description: OK
      tags:
      - Event
  /calendars/{calendarId}/events/import:
    post:
      summary: Import Event
      description: Imports an event. This operation is used to add a private copy
        of an existing event to a calendar.
      operationId: calendar.events.import
      x-api-path-slug: calendarscalendarideventsimport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: query
        name: supportsAttachments
        description: Whether API client performing operation supports event attachments
      responses:
        200:
          description: OK
      tags:
      - Event
  /calendars/{calendarId}/events/quickAdd:
    post:
      summary: Create Event
      description: Creates an event based on a simple text string.
      operationId: calendar.events.quickAdd
      x-api-path-slug: calendarscalendarideventsquickadd-post
      parameters:
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: query
        name: sendNotifications
        description: Whether to send notifications about the creation of the event
      - in: query
        name: text
        description: The text describing the event to be created
      responses:
        200:
          description: OK
      tags:
      - Event
  /calendars/{calendarId}/events/watch:
    post:
      summary: Watch Event
      description: Watch for changes to Events resources.
      operationId: calendar.events.watch
      x-api-path-slug: calendarscalendarideventswatch-post
      parameters:
      - in: query
        name: alwaysIncludeEmail
        description: Whether to always include a value in the email field for the
          organizer, creator and attendees, even if no real email is available (i
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: query
        name: iCalUID
        description: Specifies event ID in the iCalendar format to be included in
          the response
      - in: query
        name: maxAttendees
        description: The maximum number of attendees to include in the response
      - in: query
        name: maxResults
        description: Maximum number of events returned on one result page
      - in: query
        name: orderBy
        description: The order of the events returned in the result
      - in: query
        name: pageToken
        description: Token specifying which result page to return
      - in: query
        name: privateExtendedProperty
        description: Extended properties constraint specified as propertyName=value
      - in: query
        name: q
        description: Free text search terms to find events that match these terms
          in any field, except for extended properties
      - in: body
        name: resource
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: sharedExtendedProperty
        description: Extended properties constraint specified as propertyName=value
      - in: query
        name: showDeleted
        description: Whether to include deleted events (with status equals cancelled)
          in the result
      - in: query
        name: showHiddenInvitations
        description: Whether to include hidden invitations in the result
      - in: query
        name: singleEvents
        description: Whether to expand recurring events into instances and only return
          single one-off events and instances of recurring events, but not the underlying
          recurring events themselves
      - in: query
        name: syncToken
        description: Token obtained from the nextSyncToken field returned on the last
          page of results from the previous list request
      - in: query
        name: timeMax
        description: Upper bound (exclusive) for an events start time to filter by
      - in: query
        name: timeMin
        description: Lower bound (inclusive) for an events end time to filter by
      - in: query
        name: timeZone
        description: Time zone used in the response
      - in: query
        name: updatedMin
        description: Lower bound for an events last modification time (as a RFC3339
          timestamp) to filter by
      responses:
        200:
          description: OK
      tags:
      - Event
  /calendars/{calendarId}/events/{eventId}:
    delete:
      summary: Delete Event
      description: Deletes an event.
      operationId: calendar.events.delete
      x-api-path-slug: calendarscalendarideventseventid-delete
      parameters:
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: path
        name: eventId
        description: Event identifier
      - in: query
        name: sendNotifications
        description: Whether to send notifications about the deletion of the event
      responses:
        200:
          description: OK
      tags:
      - Event
    get:
      summary: Get Event
      description: Returns an event.
      operationId: calendar.events.get
      x-api-path-slug: calendarscalendarideventseventid-get
      parameters:
      - in: query
        name: alwaysIncludeEmail
        description: Whether to always include a value in the email field for the
          organizer, creator and attendees, even if no real email is available (i
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: path
        name: eventId
        description: Event identifier
      - in: query
        name: maxAttendees
        description: The maximum number of attendees to include in the response
      - in: query
        name: timeZone
        description: Time zone used in the response
      responses:
        200:
          description: OK
      tags:
      - Event
    patch:
      summary: Update Event
      description: Updates an event. This method supports patch semantics.
      operationId: calendar.events.patch
      x-api-path-slug: calendarscalendarideventseventid-patch
      parameters:
      - in: query
        name: alwaysIncludeEmail
        description: Whether to always include a value in the email field for the
          organizer, creator and attendees, even if no real email is available (i
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: path
        name: eventId
        description: Event identifier
      - in: query
        name: maxAttendees
        description: The maximum number of attendees to include in the response
      - in: query
        name: sendNotifications
        description: Whether to send notifications about the event update (e
      - in: query
        name: supportsAttachments
        description: Whether API client performing operation supports event attachments
      responses:
        200:
          description: OK
      tags:
      - Event
    put:
      summary: Update Event
      description: Updates an event.
      operationId: calendar.events.update
      x-api-path-slug: calendarscalendarideventseventid-put
      parameters:
      - in: query
        name: alwaysIncludeEmail
        description: Whether to always include a value in the email field for the
          organizer, creator and attendees, even if no real email is available (i
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: path
        name: eventId
        description: Event identifier
      - in: query
        name: maxAttendees
        description: The maximum number of attendees to include in the response
      - in: query
        name: sendNotifications
        description: Whether to send notifications about the event update (e
      - in: query
        name: supportsAttachments
        description: Whether API client performing operation supports event attachments
      responses:
        200:
          description: OK
      tags:
      - Event
  /calendars/{calendarId}/events/{eventId}/instances:
    get:
      summary: Get Event Instance
      description: Returns instances of the specified recurring event.
      operationId: calendar.events.instances
      x-api-path-slug: calendarscalendarideventseventidinstances-get
      parameters:
      - in: query
        name: alwaysIncludeEmail
        description: Whether to always include a value in the email field for the
          organizer, creator and attendees, even if no real email is available (i
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: path
        name: eventId
        description: Recurring event identifier
      - in: query
        name: maxAttendees
        description: The maximum number of attendees to include in the response
      - in: query
        name: maxResults
        description: Maximum number of events returned on one result page
      - in: query
        name: originalStart
        description: The original start time of the instance in the result
      - in: query
        name: pageToken
        description: Token specifying which result page to return
      - in: query
        name: showDeleted
        description: Whether to include deleted events (with status equals cancelled)
          in the result
      - in: query
        name: timeMax
        description: Upper bound (exclusive) for an events start time to filter by
      - in: query
        name: timeMin
        description: Lower bound (inclusive) for an events end time to filter by
      - in: query
        name: timeZone
        description: Time zone used in the response
      responses:
        200:
          description: OK
      tags:
      - Event
  /calendars/{calendarId}/events/{eventId}/move:
    post:
      summary: Move Event
      description: Moves an event to another calendar, i.e. changes an event's organizer.
      operationId: calendar.events.move
      x-api-path-slug: calendarscalendarideventseventidmove-post
      parameters:
      - in: path
        name: calendarId
        description: Calendar identifier of the source calendar where the event currently
          is on
      - in: query
        name: destination
        description: Calendar identifier of the target calendar where the event is
          to be moved to
      - in: path
        name: eventId
        description: Event identifier
      - in: query
        name: sendNotifications
        description: Whether to send notifications about the change of the events
          organizer
      responses:
        200:
          description: OK
      tags:
      - Event
  /channels/stop:
    post:
      summary: Stop Watching Resource
      description: Stop watching resources through this channel
      operationId: calendar.channels.stop
      x-api-path-slug: channelsstop-post
      parameters:
      - in: body
        name: resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Watch
  /colors:
    get:
      summary: Get Colors
      description: Returns the color definitions for calendars and events.
      operationId: calendar.colors.get
      x-api-path-slug: colors-get
      responses:
        200:
          description: OK
      tags:
      - Color
  /freeBusy:
    post:
      summary: Return Free/Busy Information
      description: Returns free/busy information for a set of calendars.
      operationId: calendar.freebusy.query
      x-api-path-slug: freebusy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Free/Busy
  /users/me/calendarList:
    get:
      summary: Return Entries
      description: Returns entries on the user's calendar list.
      operationId: calendar.calendarList.list
      x-api-path-slug: usersmecalendarlist-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of entries returned on one result page
      - in: query
        name: minAccessRole
        description: The minimum access role for the user in the returned entries
      - in: query
        name: pageToken
        description: Token specifying which result page to return
      - in: query
        name: showDeleted
        description: Whether to include deleted calendar list entries in the result
      - in: query
        name: showHidden
        description: Whether to show hidden entries
      - in: query
        name: syncToken
        description: Token obtained from the nextSyncToken field returned on the last
          page of results from the previous list request
      responses:
        200:
          description: OK
      tags:
      - Event
    post:
      summary: Add Entry
      description: Adds an entry to the user's calendar list.
      operationId: calendar.calendarList.insert
      x-api-path-slug: usersmecalendarlist-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: colorRgbFormat
        description: Whether to use the foregroundColor and backgroundColor fields
          to write the calendar colors (RGB)
      responses:
        200:
          description: OK
      tags:
      - Event
  /users/me/calendarList/watch:
    post:
      summary: Watch Entry
      description: Watch for changes to CalendarList resources.
      operationId: calendar.calendarList.watch
      x-api-path-slug: usersmecalendarlistwatch-post
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of entries returned on one result page
      - in: query
        name: minAccessRole
        description: The minimum access role for the user in the returned entries
      - in: query
        name: pageToken
        description: Token specifying which result page to return
      - in: body
        name: resource
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: showDeleted
        description: Whether to include deleted calendar list entries in the result
      - in: query
        name: showHidden
        description: Whether to show hidden entries
      - in: query
        name: syncToken
        description: Token obtained from the nextSyncToken field returned on the last
          page of results from the previous list request
      responses:
        200:
          description: OK
      tags:
      - Event
  /users/me/calendarList/{calendarId}:
    delete:
      summary: Delete Entry
      description: Deletes an entry on the user's calendar list.
      operationId: calendar.calendarList.delete
      x-api-path-slug: usersmecalendarlistcalendarid-delete
      parameters:
      - in: path
        name: calendarId
        description: Calendar identifier
      responses:
        200:
          description: OK
      tags:
      - Event
    get:
      summary: Get Entry
      description: Returns an entry on the user's calendar list.
      operationId: calendar.calendarList.get
      x-api-path-slug: usersmecalendarlistcalendarid-get
      parameters:
      - in: path
        name: calendarId
        description: Calendar identifier
      responses:
        200:
          description: OK
      tags:
      - Event
    patch:
      summary: Update Entry
      description: Updates an entry on the user's calendar list. This method supports
        patch semantics.
      operationId: calendar.calendarList.patch
      x-api-path-slug: usersmecalendarlistcalendarid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: query
        name: colorRgbFormat
        description: Whether to use the foregroundColor and backgroundColor fields
          to write the calendar colors (RGB)
      responses:
        200:
          description: OK
      tags:
      - Event
    put:
      summary: Update Entry
      description: Updates an entry on the user's calendar list.
      operationId: calendar.calendarList.update
      x-api-path-slug: usersmecalendarlistcalendarid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: query
        name: colorRgbFormat
        description: Whether to use the foregroundColor and backgroundColor fields
          to write the calendar colors (RGB)
      responses:
        200:
          description: OK
      tags:
      - Event
  /users/me/settings:
    get:
      summary: Get Settings
      description: Returns all user settings for the authenticated user.
      operationId: calendar.settings.list
      x-api-path-slug: usersmesettings-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of entries returned on one result page
      - in: query
        name: pageToken
        description: Token specifying which result page to return
      - in: query
        name: syncToken
        description: Token obtained from the nextSyncToken field returned on the last
          page of results from the previous list request
      responses:
        200:
          description: OK
      tags:
      - Setting
  /users/me/settings/watch:
    post:
      summary: Watch Settings
      description: Watch for changes to Settings resources.
      operationId: calendar.settings.watch
      x-api-path-slug: usersmesettingswatch-post
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of entries returned on one result page
      - in: query
        name: pageToken
        description: Token specifying which result page to return
      - in: body
        name: resource
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: syncToken
        description: Token obtained from the nextSyncToken field returned on the last
          page of results from the previous list request
      responses:
        200:
          description: OK
      tags:
      - Setting
  /users/me/settings/{setting}:
    get:
      summary: Get Setting
      description: Returns a single user setting.
      operationId: calendar.settings.get
      x-api-path-slug: usersmesettingssetting-get
      parameters:
      - in: path
        name: setting
        description: The id of the user setting
      responses:
        200:
          description: OK
      tags:
      - Setting