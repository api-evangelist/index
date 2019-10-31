swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 1
info:
  title: Urban Airship
  description: the-urban-airships-api-powers-mobile-applications-with-push-rich-push-inapp-purchases-and-subscription-services-
  version: v3
host: go.urbanairship.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /device_tokens/{token}:
    put:
      summary: Put Device Tokens Token
      description: Registers a device token.
      operationId: device_tokens.token.put
      x-api-path-slug: device-tokenstoken-put
      parameters:
      - in: query
        name: token
        description: Device tokens should be represented as an uppercase string, 64
          characters long, without spaces or other separators
      - in: path
        name: token
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Token
    get:
      summary: Get Device Tokens Token
      description: Gets a device token???s alias.
      operationId: device_tokens.token.get
      x-api-path-slug: device-tokenstoken-get
      parameters:
      - in: query
        name: token
        description: Device tokens should be represented as an uppercase string, 64
          characters long, without spaces or other separators
      - in: path
        name: token
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Token
    delete:
      summary: Delete Device Tokens Token
      description: Marks the device token as inactive. No notifications will be delivered
        to it until a PUT is executed again. The DELETE returns HTTP 204 No Content,
        and needs no payload. When a token is deleted in this manner, any alias or
        tags will be cleared.
      operationId: device_tokens.token.delete
      x-api-path-slug: device-tokenstoken-delete
      parameters:
      - in: query
        name: token
        description: Device tokens should be represented as an uppercase string, 64
          characters long, without spaces or other separators
      - in: path
        name: token
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Token
  /push:
    post:
      summary: Post Push
      description: Sends a push message to one or more users. Only one of aliases,
        tags, or device_pins is required, but they can be mixed and matched as much
        as you???d like.
      operationId: push.post
      x-api-path-slug: push-post
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      - in: header
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Push
  /push/scheduled/{notification}:
    delete:
      summary: Delete Push Scheduled Notification
      description: Cancels a scheduled notification.  A successful delete will have
        an HTTP status code of 204. If the scheduled notification does not exist,
        has already been successfully deleted, or was sent, the status code will be
        404.
      operationId: push.scheduled.notification.delete
      x-api-path-slug: pushschedulednotification-delete
      parameters:
      - in: query
        name: notification
        description: Scheduled notification ID
      - in: path
        name: notification
      responses:
        200:
          description: OK
      tags:
      - Push
      - Scheduled
      - Notification
  /push/scheduled:
    post:
      summary: Post Push Scheduled
      description: Bulk deletes scheduled notifications. If you include URLs or aliases
        for scheduled notifications that don???t exist or have already been sent,
        they will be ignored. Any device token in the cancel_device_tokens payload
        will have every notification that is sent to it removed. This will not prevent
        it from receiving scheduled notifications to tags or broadcast messages.
      operationId: push.scheduled.post
      x-api-path-slug: pushscheduled-post
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      - in: header
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Push
      - Scheduled
  /push/scheduled/alias/{alias}:
    put:
      summary: Put Push Scheduled Alias Alias
      description: Changes a scheduled notification alias. Aliases for scheduled notifications
        are unique per Urban Airship application, so you might want to hash the aliases
        with a device ID or use some other mechanism to ensure uniqueness. The only
        other limit is that they must be 255 characters or less.
      operationId: push.scheduled.alias.alias.put
      x-api-path-slug: pushscheduledaliasalias-put
      parameters:
      - in: query
        name: alias
        description: Scheduled notification alias
      - in: path
        name: alias
      - in: query
        name: Content-Type
        description: Content type
      - in: header
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Push
      - Scheduled
      - Alias
      - Alias
    delete:
      summary: Delete Push Scheduled Alias Alias
      description: Deletes a scheduled notification alias.  If you attempt to schedule
        an aliased scheduled notification with an alias that already exists for your
        application, it will overwrite the existing one.
      operationId: push.scheduled.alias.alias.delete
      x-api-path-slug: pushscheduledaliasalias-delete
      parameters:
      - in: query
        name: alias
        description: Scheduled notification alias
      - in: path
        name: alias
      responses:
        200:
          description: OK
      tags:
      - Push
      - Scheduled
      - Alias
      - Alias
  /push/batch:
    post:
      summary: Post Push Batch
      description: Sends a push message to all the listed PINs. Each item in the list
        can contain 0 or many device_pins and 0 or many aliases or tags, and the blackberry
        payload is in the same format as for individual pushes.
      operationId: push.batch.post
      x-api-path-slug: pushbatch-post
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      - in: header
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Push
      - Batch
  /push/broadcast:
    post:
      summary: Post Push Broadcast
      description: 'Sends a push message to all active APIDs (Broadcast). Important:
        The maximum message size is 1024 bytes. This is calculated as the UTF-8 lengths
        of alert and extra fields together.'
      operationId: push.broadcast.post
      x-api-path-slug: pushbroadcast-post
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      - in: header
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Push
      - Broadcast
  /push/stats:
    get:
      summary: Get Push Stats
      description: 'Returns hourly message counts for your application. By default,
        results are returned in JSON. For CSV, either add the header:Accept:text/csv
        or append &format=csv to the query string. Times are in UTC, and data is provided
        for each push platform (currently: iOS, BlackBerry, Android, and C2DM, in
        that order). The statistics system is updated every 15 minutes, so the final
        count for an hour will be done at the latest 15 minutes after the hour is
        done.'
      operationId: push.stats.get
      x-api-path-slug: pushstats-get
      parameters:
      - in: query
        name: end
        description: End date in UTC format
      - in: query
        name: format
        description: Response format
      - in: query
        name: start
        description: Start date in UTC format
      responses:
        200:
          description: OK
      tags:
      - Push
      - Stats
  /device_tokens:
    get:
      summary: Get Device Tokens
      description: Gets information about all of your device tokens. If your application
        has a large number of device tokens, we???ll paginate the request for you.
        By default, we paginate at 5000 device tokens. You can receive the next page
        simply by retrieving the URL from "next_page" - in this way it is easy to
        export all of your device tokens and all their data.
      operationId: device_tokens.get
      x-api-path-slug: device-tokens-get
      parameters:
      - in: query
        name: limit
        description: The total items to return
      - in: query
        name: page
        description: The page number
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
  /device_tokens/count:
    get:
      summary: Get Device Tokens Count
      description: Gets the number of device tokens you have registered.
      operationId: device_tokens.count.get
      x-api-path-slug: device-tokenscount-get
      parameters:
      - in: query
        name: limit
        description: The total items to return
      - in: query
        name: page
        description: The page number
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Count
  /device_tokens/feedback:
    get:
      summary: Get Device Tokens Feedback
      description: Gets what device tokens are now invalid. Apple informs us when
        a push notification is sent to a device that can???t receive it because the
        application has been uninstalled. We mark the device token as inactive and
        immediately stop sending notifications to that device. Once a day is a good
        interval for querying the feedback service, but you can do it more often to
        save on bandwidth from unnecessary notifications. In the response, what does
        marked_inactive_on mean? Apple sends a timestamp for each device token returned
        via the feedback service. Since a device can be off the network for a while,
        this can be a point in the recent past. In order to make this API work smoothly
        for you, we record the timestamp we marked as inactive. This means you only
        need to query for data since the last time you queried. Once a day is a good
        timeframe, or once a week for very small or infrequently used applications.
        A few times a day is good for applications with heavy use.
      operationId: device_tokens.feedback.get
      x-api-path-slug: device-tokensfeedback-get
      parameters:
      - in: query
        name: since
        description: Since timestamp in ISO 8601 format
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Feedback
  /apids/{apid}:
    put:
      summary: Put Aps Ap
      description: Registers an APID. Unlike registration for iOS and BlackBerry applications,
        basic registration tying an APID to your application happens automatically.
        The registration API can be used to set aliases or tags. This returns HTTP
        200 OK for any updates. Registering without any body is a no-op. Not including
        the alias field will clear it. To clear the list of tags, set it to the empty
        list []. If you are registering an APID to be used with C2DM, you will also
        need to include a C2DM registration ID.
      operationId: apids.apid.put
      x-api-path-slug: apidsapid-put
      parameters:
      - in: query
        name: apid
        description: An APID (Android Push ID) is the Urban Airship ID of a device
          to which a message can be pushed
      - in: path
        name: apid
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Apids
      - Apid
    get:
      summary: Get Aps Ap
      description: Gets APID information.
      operationId: apids.apid.get
      x-api-path-slug: apidsapid-get
      parameters:
      - in: query
        name: apid
        description: An APID (Android Push ID) is the Urban Airship ID of a device
          to which a message can be pushed
      - in: path
        name: apid
      responses:
        200:
          description: OK
      tags:
      - Apids
      - Apid
    delete:
      summary: Delete Aps Ap
      description: Marks an APID as invalid. No notifications will be delivered to
        it until it re-registers.
      operationId: apids.apid.delete
      x-api-path-slug: apidsapid-delete
      parameters:
      - in: query
        name: apid
        description: An APID (Android Push ID) is the Urban Airship ID of a device
          to which a message can be pushed
      - in: path
        name: apid
      responses:
        200:
          description: OK
      tags:
      - Apids
      - Apid
  /apids:
    get:
      summary: Get Aps
      description: Gets APIDs. You can control how many APIDs are returned at a time
        by using the limit GET argument. The maximum limit is 5000.
      operationId: apids.get
      x-api-path-slug: apids-get
      parameters:
      - in: query
        name: limit
        description: Control how many APIDs are returned at a time
      - in: query
        name: start
        description: APID from where to start from
      responses:
        200:
          description: OK
      tags:
      - Apids
  /device_pins/{pin}:
    put:
      summary: Put Device Pins Pin
      description: Registers a BlackBerry PIN. This is optional, but recommended,
        for BlackBerry push messages. This returns HTTP 201 Created for the first
        registration and 200 OK for any updates. If you wish to include additional
        information about a device pin, for instance an alias or tags, include a JSON
        payload along with this request. Not including one of these keys removes it
        from the device pin.
      operationId: device_pins.pin.put
      x-api-path-slug: device-pinspin-put
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: pin
        description: A BlackBerry PIN
      - in: path
        name: pin
      responses:
        200:
          description: OK
      tags:
      - Device
      - Pins
      - Pin
    get:
      summary: Get Device Pins Pin
      description: Gets Device PIN information.
      operationId: device_pins.pin.get
      x-api-path-slug: device-pinspin-get
      parameters:
      - in: query
        name: pin
        description: A BlackBerry PIN
      - in: path
        name: pin
      responses:
        200:
          description: OK
      tags:
      - Device
      - Pins
      - Pin
    delete:
      summary: Delete Device Pins Pin
      description: Marks a PIN as inactive. No notifications will be delivered to
        it until a PUT is executed again.
      operationId: device_pins.pin.delete
      x-api-path-slug: device-pinspin-delete
      parameters:
      - in: query
        name: pin
        description: A BlackBerry PIN
      - in: path
        name: pin
      responses:
        200:
          description: OK
      tags:
      - Device
      - Pins
      - Pin
  /user:
    post:
      summary: Post User
      description: Creates a new user and returns the credentials.
      operationId: user.post
      x-api-path-slug: user-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - User
  /user/{user_id}:
    put:
      summary: Put User User
      description: Changes properties of an user - for example, changing or adding
        an email address.
      operationId: user.user_id.put
      x-api-path-slug: useruser-id-put
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: user_id
        description: The user ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
    delete:
      summary: Delete User User
      description: Deletes an user.
      operationId: user.user_id.delete
      x-api-path-slug: useruser-id-delete
      parameters:
      - in: query
        name: user_id
        description: The user ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
    get:
      summary: Get User User
      description: Retrieves an user???s subscription information.
      operationId: user.user_id.get
      x-api-path-slug: useruser-id-get
      parameters:
      - in: query
        name: user_id
        description: User ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
  /user/{user_id}/creds/reset:
    post:
      summary: Post User User Creds Reset
      description: Changes the password of an user.
      operationId: user.user_id.creds.reset.post
      x-api-path-slug: useruser-idcredsreset-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: user_id
        description: The user ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Creds
      - Reset
  /airmail/send:
    post:
      summary: Post Airmail Send
      description: Sends a message. All fields except message are optional, but at
        least one of tags, users or aliases must be specified. Much like the push
        API, we have a batch API call that can make sending multiple messages easier.
        It???s located at /api/airmail/send/batch/ and accepts a list of messages
        in the same format as the standard push call.
      operationId: airmail.send.post
      x-api-path-slug: airmailsend-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Airmail
      - Send
  /airmail/send/broadcast:
    post:
      summary: Post Airmail Send Broadcast
      description: Sends a message to all users (broadcast). Only message is required.
        The message will be sent out to every registered user. Badge numbers will
        be handled automatically as long as the push key is present.
      operationId: airmail.send.broadcast.post
      x-api-path-slug: airmailsendbroadcast-post
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      - in: header
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Airmail
      - Send
      - Broadcast
  /user/{user_id}/messages:
    get:
      summary: Get User User Messages
      description: Returns a list of messages and some metadata about them. It will
        also include some metadata about the user.
      operationId: user.user_id.messages.get
      x-api-path-slug: useruser-idmessages-get
      parameters:
      - in: query
        name: full_list
        description: Get the full message included in this list (which might take
          a while to download)
      - in: query
        name: since
        description: Return only new items
      - in: query
        name: user_id
        description: The user ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Messages
  /user/{user_id}/messages/unread:
    get:
      summary: Get User User Messages Unread
      description: Returns a list of unread message IDs and their URLs.
      operationId: user.user_id.messages.unread.get
      x-api-path-slug: useruser-idmessagesunread-get
      parameters:
      - in: query
        name: user_id
        description: The user ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Messages
      - Unread
    post:
      summary: Post User User Messages Unread
      description: Marks multiple messages as read at once. If a message has already
        been marked as read, it will be silently skipped.
      operationId: user.user_id.messages.unread.post
      x-api-path-slug: useruser-idmessagesunread-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: user_id
        description: The user ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Messages
      - Unread
  /user/{user_id}/messages/message/{message_id}:
    get:
      summary: Get User User Messages Message Message
      description: Gets a message.
      operationId: user.user_id.messages.message.message_id.get
      x-api-path-slug: useruser-idmessagesmessagemessage-id-get
      parameters:
      - in: query
        name: message_id
        description: The message ID
      - in: path
        name: message_id
      - in: query
        name: user_id
        description: The user ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Messages
      - Message
      - Message
      - Id
    delete:
      summary: Delete User User Messages Message Message
      description: Deletes a message.
      operationId: user.user_id.messages.message.message_id.delete
      x-api-path-slug: useruser-idmessagesmessagemessage-id-delete
      parameters:
      - in: query
        name: message_id
        description: The message ID
      - in: path
        name: message_id
      - in: query
        name: user_id
        description: The user ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Messages
      - Message
      - Message
      - Id
  /user/{user_id}/messages/message/{message_id}/body:
    get:
      summary: Get User User Messages Message Message Body
      description: Gets a message's body.
      operationId: user.user_id.messages.message.message_id.body.get
      x-api-path-slug: useruser-idmessagesmessagemessage-idbody-get
      parameters:
      - in: query
        name: message_id
        description: The message ID
      - in: path
        name: message_id
      - in: query
        name: user_id
        description: The user ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Messages
      - Message
      - Message
      - Id
      - Body
  /user/{user_id}/messages/message/{message_id}/read:
    post:
      summary: Post User User Messages Message Message Read
      description: Marks a message as read.
      operationId: user.user_id.messages.message.message_id.read.post
      x-api-path-slug: useruser-idmessagesmessagemessage-idread-post
      parameters:
      - in: query
        name: message_id
        description: The message ID
      - in: path
        name: message_id
      - in: query
        name: user_id
        description: The user ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Messages
      - Message
      - Message
      - Id
      - Read
  /user/{user_id}/messages/delete:
    post:
      summary: Post User User Messages Delete
      description: Deletes multiple messages at once. If a message has already been
        deleted, it will be silently skipped.
      operationId: user.user_id.messages.delete.post
      x-api-path-slug: useruser-idmessagesdelete-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: user_id
        description: The user ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Messages
      - Delete
  /app/content:
    get:
      summary: Get App Content
      description: Gets the store inventory.
      operationId: app.content.get
      x-api-path-slug: appcontent-get
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: user_id
        description: The user ID
      responses:
        200:
          description: OK
      tags:
      - App
      - Content
  /app/content/{product_id}/download:
    post:
      summary: Post App Content Product Download
      description: Returns a temporary URL where the client can download the content.
        In the payload, the receipt string is the receipt data from the purchase.
        It should be unaltered from how Apple delivers it to your application.udid
        is an optional field to help identify a particular user???s purchases, which
        can aid debugging. It should always be a hash of the UDID, not the actual
        UDID, to ensure compliance with Apple???s TOS. The optional version field
        should be the StoreFront library version, or custom if you???re building your
        own.
      operationId: app.content.product_id.download.post
      x-api-path-slug: appcontentproduct-iddownload-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: product_id
        description: The product ID
      - in: path
        name: product_id
      responses:
        200:
          description: OK
      tags:
      - App
      - Content
      - Product
      - Id
      - Download
  /app/updates:
    post:
      summary: Post App Updates
      description: Checks for updates. It can be useful on application launch to compare
        a list of installed updates with our server to see if there are any updates
        to be had for the content.
      operationId: app.updates.post
      x-api-path-slug: appupdates-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: product_id
        description: The product ID
      responses:
        200:
          description: OK
      tags:
      - App
      - Updates
  /user/recover:
    post:
      summary: Post User Recover
      description: Uses the user???s email address as a way to restore subscription
        content across devices.
      operationId: user.recover.post
      x-api-path-slug: userrecover-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - User
      - Recover
  /user/recover/{id}:
    get:
      summary: Get User Recover
      description: Checks the recovery status.
      operationId: user.recover.id.get
      x-api-path-slug: userrecoverid-get
      parameters:
      - in: query
        name: id
        description: ID of the useru2019s account recovery
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - User
      - Recover
      - Id
  /user/{user_id}/available_subscriptions:
    get:
      summary: Get User User Available Subscriptions
      description: Retrieves subscription options.
      operationId: user.user_id.available_subscriptions.get
      x-api-path-slug: useruser-idavailable-subscriptions-get
      parameters:
      - in: query
        name: user_id
        description: User ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Available
      - Subscriptions
  /user/{user_id}/subscriptions/{subscription_key}/purchase:
    post:
      summary: Post User User Subscriptions Subscription Key Purchase
      description: Adds a new subscription.
      operationId: user.user_id.subscriptions.subscription_key.purchase.post
      x-api-path-slug: useruser-idsubscriptionssubscription-keypurchase-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: subscription_key
        description: Subscription Key
      - in: path
        name: subscription_key
      - in: query
        name: user_id
        description: User ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Subscriptions
      - Subscription
      - Key
      - Purchase
  /user/{user_id}/subscription_content:
    get:
      summary: Get User User Subscription Content
      description: Returns a list of available content.
      operationId: user.user_id.subscription_content.get
      x-api-path-slug: useruser-idsubscription-content-get
      parameters:
      - in: query
        name: user_id
        description: User ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Subscription
      - Content
  /user/{user_id}/subscriptions/content/{content_id}/download:
    post:
      summary: Post User User Subscriptions Content Content Download
      description: Downloads the content.
      operationId: user.user_id.subscriptions.content.content_id.download.post
      x-api-path-slug: useruser-idsubscriptionscontentcontent-iddownload-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: content_id
        description: Content ID
      - in: path
        name: content_id
      - in: query
        name: user_id
        description: User ID
      - in: path
        name: user_id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Subscriptions
      - Content
      - Content
      - Id
      - Download
  /feeds:
    post:
      summary: Post Feeds
      description: Creates a new feed item.
      operationId: feeds.post
      x-api-path-slug: feeds-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Feeds
    get:
      summary: Get Feeds
      description: Gets a list of feeds.
      operationId: feeds.get
      x-api-path-slug: feeds-get
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Feeds
  /feeds/{feed_id}:
    get:
      summary: Get Feeds Feed
      description: Returns information about a particular feed.
      operationId: feeds.feed_id.get
      x-api-path-slug: feedsfeed-id-get
      parameters:
      - in: query
        name: feed_id
        description: A particular feed
      - in: path
        name: feed_id
      responses:
        200:
          description: OK
      tags:
      - Feeds
      - Feed
      - Id
    put:
      summary: Put Feeds Feed
      description: Updates a feed.
      operationId: feeds.feed_id.put
      x-api-path-slug: feedsfeed-id-put
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: feed_id
        description: A particular feed
      - in: path
        name: feed_id
      responses:
        200:
          description: OK
      tags:
      - Feeds
      - Feed
      - Id
    delete:
      summary: Delete Feeds Feed
      description: Deletes a feed.
      operationId: feeds.feed_id.delete
      x-api-path-slug: feedsfeed-id-delete
      parameters:
      - in: query
        name: feed_id
        description: A particular feed
      - in: path
        name: feed_id
      responses:
        200:
          description: OK
      tags:
      - Feeds
      - Feed
      - Id
  /tags:
    get:
      summary: Get Tags
      description: Returns all the tags that you have created.
      operationId: tags.get
      x-api-path-slug: tags-get
      parameters:
      - in: query
        name: feed_id
        description: A particular feed
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/{tag}:
    put:
      summary: Put Tags Tag
      description: Deletes a tag.
      operationId: tags.tag.put
      x-api-path-slug: tagstag-put
      parameters:
      - in: query
        name: tag
        description: Tags can be of any format you wish, but we recommend that they
          be URL-safe in order to make less work for you
      - in: path
        name: tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Tag
    post:
      summary: Post Tags Tag
      description: Modifies device tokens on a tag.
      operationId: tags.tag.post
      x-api-path-slug: tagstag-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      - in: query
        name: tag
        description: Tags can be of any format you wish, but we recommend that they
          be URL-safe in order to make less work for you
      - in: path
        name: tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Tag
  /device_tokens/{device_token}/tags:
    get:
      summary: Get Device Tokens Device Token Tags
      description: Gets tags for a specific device token.
      operationId: device_tokens.device_token.tags.get
      x-api-path-slug: device-tokensdevice-tokentags-get
      parameters:
      - in: query
        name: device_token
        description: A specific device token
      - in: path
        name: device_token
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Device
      - Token
      - Tags
  /device_tokens/{device_token}/tags/{tag}:
    put:
      summary: Put Device Tokens Device Token Tags Tag
      description: Creates a tag and associate it with the specific device token.
      operationId: device_tokens.device_token.tags.tag.put
      x-api-path-slug: device-tokensdevice-tokentagstag-put
      parameters:
      - in: query
        name: device_token
        description: A specific device token
      - in: path
        name: device_token
      - in: query
        name: tag
        description: Tags can be of any format you wish, but we recommend that they
          be URL-safe in order to make less work for you
      - in: path
        name: tag
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Device
      - Token
      - Tags
      - Tag
    delete:
      summary: Delete Device Tokens Device Token Tags Tag
      description: Removes a single tag from a device token.
      operationId: device_tokens.device_token.tags.tag.delete
      x-api-path-slug: device-tokensdevice-tokentagstag-delete
      parameters:
      - in: query
        name: device_token
        description: A specific device token
      - in: path
        name: device_token
      - in: query
        name: tag
        description: Tags can be of any format you wish, but we recommend that they
          be URL-safe in order to make less work for you
      - in: path
        name: tag
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Device
      - Token
      - Tags
      - Tag
  /partner/apps:
    get:
      summary: Get Partner Apps
      description: List applications.
      operationId: partner.apps.get
      x-api-path-slug: partnerapps-get
      parameters:
      - in: query
        name: device_token
        description: A specific device token
      - in: query
        name: tag
        description: Tags can be of any format you wish, but we recommend that they
          be URL-safe in order to make less work for you
      responses:
        200:
          description: OK
      tags:
      - Partner
      - Apps
    post:
      summary: Post Partner Apps
      description: Adds a new application.
      operationId: partner.apps.post
      x-api-path-slug: partnerapps-post
      parameters:
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Partner
      - Apps
  /partner/apps/{app_id}:
    put:
      summary: Put Partner Apps App
      description: Updates an application.
      operationId: partner.apps.app_id.put
      x-api-path-slug: partnerappsapp-id-put
      parameters:
      - in: query
        name: app_id
        description: A specific application
      - in: path
        name: app_id
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Partner
      - Apps
      - App
      - Id