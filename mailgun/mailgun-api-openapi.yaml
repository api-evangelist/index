swagger: "2.0"
x-collection-name: Mailgun
x-complete: 1
info:
  title: Mailgun API
  description: powerful-apis-that-allow-you-to-send-receive-and-track-email-effortlessly-
  version: v2
host: api.mailgun.net
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  bounces/:
    get:
      summary: Bounces
      description: Fetches the list of bounces.
      operationId: getBounces
      x-api-path-slug: bounces-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of records to return
      - in: query
        name: skip
        description: Number of records to skip
      responses:
        200:
          description: OK
      tags:
      - Bounces
    post:
      summary: Add Bounce
      description: Adds a permanent bounce to the bounces table. Updates the existing
        record if already here.
      operationId: postBounces
      x-api-path-slug: bounces-post
      parameters:
      - in: query
        name: address
        description: Email address to add to bounce list
      - in: query
        name: code
        description: Error code (default 550)
      - in: query
        name: error
        description: Error description, (default is empty)
      responses:
        200:
          description: OK
      tags:
      - Bounce
  bounces/{address}:
    delete:
      summary: Delete Bounce
      description: Clears a bounce event.
      operationId: deleteBouncesAddress
      x-api-path-slug: bouncesaddress-delete
      responses:
        200:
          description: OK
      tags:
      - Bounce
    get:
      summary: Bounce
      description: Fetches a single bounce event by a given email address. This is
        useful to check if a given email address has bounced before.
      operationId: getBouncesAddress
      x-api-path-slug: bouncesaddress-get
      parameters:
      - in: path
        name: address
        description: The email address to get bounce request for
      responses:
        200:
          description: OK
      tags:
      - Bounce
  complaints/:
    get:
      summary: Complaints
      description: Fetches the list of complaints.
      operationId: getComplaints
      x-api-path-slug: complaints-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of records to return
      - in: query
        name: skip
        description: Number of records to skip
      responses:
        200:
          description: OK
      tags:
      - Complaints
    post:
      summary: Add Complaint
      description: Adds an address to the complaints table.
      operationId: postComplaints
      x-api-path-slug: complaints-post
      parameters:
      - in: query
        name: address
        description: Email address to add to the complaint list
      responses:
        200:
          description: OK
      tags:
      - Complaint
  complaints/{address}:
    delete:
      summary: Delete Complaint
      description: Removes a given spam complaint.
      operationId: deleteComplaintsAddress
      x-api-path-slug: complaintsaddress-delete
      parameters:
      - in: query
        name: address
        description: Email address of complaint to remove
      responses:
        200:
          description: OK
      tags:
      - Complaint
    get:
      summary: Complaint
      description: Fetches a single spam complaint by a given email address. This
        is useful to check if a particular user has complained.
      operationId: getComplaintsAddress
      x-api-path-slug: complaintsaddress-get
      parameters:
      - in: query
        name: address
        description: Email address of the complaint to get
      responses:
        200:
          description: OK
      tags:
      - Complaint
  lists:
    post:
      summary: Create List
      description: Creates a new mailing list.
      operationId: postLists
      x-api-path-slug: lists-post
      parameters:
      - in: query
        name: access_level
        description: 'List access level, one of: readonly (default), members, everyone'
      - in: query
        name: address
        description: A valid email address for the mailing list, e
      - in: query
        name: description
        description: A description
      - in: query
        name: name
        description: Mailing list name, e
      responses:
        200:
          description: OK
      tags:
      - List
  lists/:
    get:
      summary: Lists
      description: Returns a list of mailing lists under your account.
      operationId: getLists
      x-api-path-slug: lists-get
      parameters:
      - in: query
        name: access_level
        description: 'List access level, one of: readonly (default), members, everyone'
      - in: query
        name: address
        description: Find a mailing list by itu2019s address (optional)
      - in: query
        name: description
        description: Description string
      - in: query
        name: limit
        description: Maximum number of records to return (100 by default)
      - in: query
        name: namespace_id
        description: New name, e
      - in: query
        name: skip
        description: Records to skip (0 by default)
      responses:
        200:
          description: OK
      tags:
      - Lists
  lists/{address}:
    delete:
      summary: Delete List
      description: Deletes a mailing list.
      operationId: deleteListsAddress
      x-api-path-slug: listsaddress-delete
      parameters:
      - in: query
        name: address
        description: Address to remove
      responses:
        200:
          description: OK
      tags:
      - List
    get:
      summary: List
      description: Returns a single mailing list by a given address.
      operationId: getListsAddress
      x-api-path-slug: listsaddress-get
      parameters:
      - in: query
        name: address
        description: Address to return for a single list
      responses:
        200:
          description: OK
      tags:
      - List
    put:
      summary: Update List
      description: Update mailing list properties, such as address, description or
        name
      operationId: putListsAddress
      x-api-path-slug: listsaddress-put
      responses:
        200:
          description: OK
      tags:
      - List
  lists/{address}/members:
    get:
      summary: Add To List
      description: Adds a member to the mailing list.
      operationId: getListsAddressMembers
      x-api-path-slug: listsaddressmembers-get
      parameters:
      - in: query
        name: address
        description: Valid email address specification, e
      - in: query
        name: Name
        description: Optional member name
      - in: query
        name: subscribed
        description: yes to add as subscribed (default), no as unsubscribed
      - in: query
        name: upsert
        description: yes to update member if present, no to raise error in case of
          a duplicate member (default)
      - in: query
        name: vars
        description: JSON-encoded dictionary string with arbitrary parameters, e
      responses:
        200:
          description: OK
      tags:
      - List
  lists/{address}/members/:
    get:
      summary: List Members
      description: Fetches the list of mailing list members.
      operationId: getListsAddressMembers
      x-api-path-slug: listsaddressmembers-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of records to return (100 by default)
      - in: query
        name: skip
        description: Records to skip (0 by default)
      - in: query
        name: subscribed
        description: yes to list subscribed, no for unsubscribed, list all if not
          set
      responses:
        200:
          description: OK
      tags:
      - List
      - Members
  lists/{address}/members/{member_address}:
    get:
      summary: List Member
      description: Retrieves a mailing list member.
      operationId: getListsAddressMembersMemberAddress
      x-api-path-slug: listsaddressmembersmember-address-get
      parameters:
      - in: query
        name: address
        description: Email address of commenter
      - in: query
        name: member_address
        description: Email address on the list
      responses:
        200:
          description: OK
      tags:
      - List
      - Member
  messages.mime:
    post:
      summary: Posts Mime Message
      description: 'Posts a message in MIME format. Note: you will need to build a
        MIME string yourself. Use a MIME library for your programming language to
        do this. Pass the resulting MIME string as message parameter.'
      operationId: postMessages.mime
      x-api-path-slug: messages-mime-post
      parameters:
      - in: query
        name: h:X-My-Header
        description: 'h: prefix followed by an arbitrary value allows to appendna
          custom MIME header to the message (X-My-Headernin this case)'
      - in: query
        name: message
        description: MIME string of the message
      - in: query
        name: o:campaign
        description: Id of the campaign the message belongs to
      - in: query
        name: o:deliverytime
        description: Desired time of delivery
      - in: query
        name: o:dkim
        description: Enables/disabled DKIM signatures on per-message basis
      - in: query
        name: o:tag
        description: Tag string
      - in: query
        name: o:testmode
        description: Enables sending in test mode
      - in: query
        name: o:tracking
        description: Toggles tracking on a per-message basis, seenTracking Messages
          for details
      - in: query
        name: o:tracking-clicks
        description: Toggles clicks tracking on a per-message basis
      - in: query
        name: o:tracking-opens
        description: Toggles opens tracking on a per-message basis
      - in: query
        name: to
        description: Email address of the recipient(s)
      - in: query
        name: v:my-var
        description: 'v: prefix followed by an arbitrary name allows tonattach a custom
          JSON data to the message'
      responses:
        200:
          description: OK
      tags:
      - S
      - Mime
      - Message
  messages/:
    post:
      summary: Send Message
      description: Sends a message by assembling it from the components. Note that
        you can specify most parameters multiple times, HTTP supports this out of
        the box. This makes sense for parameters like cc, to or attachment.
      operationId: postMessages
      x-api-path-slug: messages-post
      parameters:
      - in: query
        name: attachment
        description: File attachment
      - in: query
        name: bcc
        description: Same as To but for Bcc
      - in: query
        name: cc
        description: Same as To but for Cc
      - in: query
        name: from
        description: Email address for From header
      - in: query
        name: h:X-My-Header
        description: 'h: prefix followed by an arbitrary value allows to appendna
          custom MIME header to the message (X-My-Headernin this case)'
      - in: query
        name: html
        description: Body of the message
      - in: query
        name: inline
        description: Attachment with inline disposition
      - in: query
        name: o:campaign
        description: Id of the campaign the message belongs to
      - in: query
        name: o:deliverytime
        description: Desired time of delivery
      - in: query
        name: o:dkim
        description: Enables/disables DKIM signatures on per-message basis
      - in: query
        name: o:tag
        description: Tag string
      - in: query
        name: o:testmode
        description: Enables sending in test mode
      - in: query
        name: o:tracking
        description: Toggles tracking on a per-message basis, seenTracking Messages
          for details
      - in: query
        name: o:tracking-clicks
        description: Toggles clicks tracking on a per-message basis
      - in: query
        name: o:tracking-opens
        description: Toggles opens tracking on a per-message basis
      - in: query
        name: subject
        description: Message subject
      - in: query
        name: text
        description: Body of the message
      - in: query
        name: to
        description: Email address of the recipient(s)
      - in: query
        name: v:my-var
        description: 'v: prefix followed by an arbitrary name allows tonattach a custom
          JSON data to the message'
      responses:
        200:
          description: OK
      tags:
      - Send
      - Message
  messages/{id}:
    get:
      summary: Message
      description: Gets a message.
      operationId: getMessages
      x-api-path-slug: messagesid-get
      parameters:
      - in: query
        name: id
        description: ID of the message
      responses:
        200:
          description: OK
      tags:
      - Message
  routes/:
    get:
      summary: Routes
      description: Fetches the list of routes. Note that routes are defined globally,
        per account, not per domain as most of other API calls.
      operationId: getRoutes
      x-api-path-slug: routes-get
      responses:
        200:
          description: OK
      tags:
      - Routes
    post:
      summary: Add Route
      description: Creates a new route.
      operationId: postRoutes
      x-api-path-slug: routes-post
      parameters:
      - in: query
        name: action
        description: Route action
      - in: query
        name: description
        description: An arbitrary string
      - in: query
        name: expression
        description: A filter expression like match_recipient(
      - in: query
        name: priority
        description: 'Integer: smaller number indicates higher priority'
      responses:
        200:
          description: OK
      tags:
      - Route
  routes/{id}:
    delete:
      summary: Delete Route
      description: Deletes a route based on the id.
      operationId: deleteRoutes
      x-api-path-slug: routesid-delete
      parameters:
      - in: path
        name: id
        description: ID of the route
      responses:
        200:
          description: OK
      tags:
      - Route
    get:
      summary: Route
      description: Returns a single route object based on its ID.
      operationId: getRoutes
      x-api-path-slug: routesid-get
      responses:
        200:
          description: OK
      tags:
      - Route
    put:
      summary: Updates Route
      description: Updates a given route by ID.
      operationId: putRoutes
      x-api-path-slug: routesid-put
      parameters:
      - in: query
        name: action
        description: Route action
      - in: query
        name: description
        description: An arbitrary string
      - in: query
        name: expression
        description: A filter expression like match_recipient(
      - in: path
        name: id
        description: ID of the route
      - in: query
        name: priority
        description: 'Integer: smaller number indicates higher priority'
      responses:
        200:
          description: OK
      tags:
      - S
      - Route
  stats/:
    get:
      summary: Stats
      description: Returns a list of event stat items. Each record represents counts
        for one event per one day.
      operationId: getStats
      x-api-path-slug: stats-get
      parameters:
      - in: query
        name: event
        description: Name of the event to receive the stats for
      - in: query
        name: limit
        description: Maximum number of records to return
      - in: query
        name: skip
        description: Number of records to skip
      - in: query
        name: start-date
        description: The date to receive the stats starting from
      responses:
        200:
          description: OK
      tags:
      - Stats
  tags/{tag}:
    delete:
      summary: Delete Tag
      description: Deletes all counters for particular tag and the tag itself.
      operationId: deleteTagsTag
      x-api-path-slug: tagstag-delete
      responses:
        200:
          description: OK
      tags:
      - Tag
  unsubscribes/:
    get:
      summary: Unsubscribes
      description: This API allows you to programmatically download the list of recipients
        who have unsubscribed from your emails.
      operationId: getUnsubscribes
      x-api-path-slug: unsubscribes-get
      parameters:
      - in: query
        name: limit
        description: Number of records to return
      - in: query
        name: skip
        description: Number of records to skip
      responses:
        200:
          description: OK
      tags:
      - Unsubscribes
    post:
      summary: Add to unsubscribe list.
      description: Adds address to unsubscribed table.
      operationId: postUnsubscribes
      x-api-path-slug: unsubscribes-post
      parameters:
      - in: query
        name: address
        description: The address to add to unsubscribe list
      - in: query
        name: tag
        description: Tag to unsubscribe from, use * to unsubscribe address from domain
      responses:
        200:
          description: OK
      tags:
      - To
      - Unsubscribe
      - List
  unsubscribes/{address}:
    delete:
      summary: Delete Unsubscribe
      description: Removes an address from the unsubscribes table. Address defines
        which events to delete.
      operationId: deleteUnsubscribesAddress
      x-api-path-slug: unsubscribesaddress-delete
      parameters:
      - in: query
        name: address
        description: The email address of the person on the unsubscribe list
      responses:
        200:
          description: OK
      tags:
      - Unsubscribe
    get:
      summary: Unsubscribe
      description: Retreives a single unsubscribe record. Can be used to check if
        a given address is present in the list of unsubscribed users.
      operationId: getUnsubscribesAddress
      x-api-path-slug: unsubscribesaddress-get
      parameters:
      - in: query
        name: address
        description: The email address of the person on the unsubscribe list
      responses:
        200:
          description: OK
      tags:
      - Unsubscribe