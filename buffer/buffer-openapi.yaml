swagger: "2.0"
x-collection-name: Buffer
x-complete: 1
info:
  title: Bufferapp
  description: social-media-management-for-marketers-and-agencies
  version: "1"
host: api.bufferapp.com
basePath: /1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /info/configuration{mediaTypeExtension}:
    get:
      summary: Get Info Configuration Mediatypeextension
      description: Returns an object with the current configuration that Buffer is
        using, including supported services, their icons and the varying limits of
        character and schedules.
      operationId: returns-an-object-with-the-current-configuration-that-buffer-is-using-including-supported-services-t
      x-api-path-slug: infoconfigurationmediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
      responses:
        200:
          description: OK
      tags:
      - Info
      - ConfigurationmediaTypeExtension
  /links/shares{mediaTypeExtension}:
    get:
      summary: Get Links Shares Mediatypeextension
      description: Returns an object with a the numbers of shares a link has had using
        Buffer.
      operationId: returns-an-object-with-a-the-numbers-of-shares-a-link-has-had-using-buffer-
      x-api-path-slug: linkssharesmediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
      - in: query
        name: url
        description: URL-encoded URL of the page for which the number of shares is
          requested
      responses:
        200:
          description: OK
      tags:
      - Links
      - SharesmediaTypeExtension
  /profiles/{id}/schedules/update{mediaTypeExtension}:
    post:
      summary: Post Profiles Schedules Update Mediatypeextension
      description: Post Profiles Schedules Update Mediatypeextension
      operationId: set-the-posting-schedules-for-the-specified-social-media-profile-
      x-api-path-slug: profilesidschedulesupdatemediatypeextension-post
      parameters:
      - in: path
        name: id
      - in: path
        name: mediaTypeExtension
      responses:
        200:
          description: OK
      tags:
      - Profiles
      - Id
      - Schedules
      - UpdatemediaTypeExtension
  /profiles/{id}/schedules{mediaTypeExtension}:
    get:
      summary: Get Profiles Schedules Mediatypeextension
      description: Returns details of the posting schedules associated with a social
        media profile.
      operationId: returns-details-of-the-posting-schedules-associated-with-a-social-media-profile-
      x-api-path-slug: profilesidschedulesmediatypeextension-get
      parameters:
      - in: path
        name: id
      - in: path
        name: mediaTypeExtension
      responses:
        200:
          description: OK
      tags:
      - Profiles
      - Id
      - SchedulesmediaTypeExtension
  /profiles/{id}/updates/pending{mediaTypeExtension}:
    get:
      summary: Get Profiles Updates Pending Mediatypeextension
      description: Get Profiles Updates Pending Mediatypeextension
      operationId: returns-an-array-of-updates-that-are-currently-in-the-buffer-for-an-individual-social-media-profile-
      x-api-path-slug: profilesidupdatespendingmediatypeextension-get
      parameters:
      - in: query
        name: count
        description: Specifies the number of status updates to receive
      - in: path
        name: id
      - in: path
        name: mediaTypeExtension
      - in: query
        name: page
        description: Specifies the page of status updates to receive
      - in: query
        name: since
        description: Specifies a unix timestamp which only status updates created
          after this time will be retrieved
      - in: query
        name: utc
        description: If utc is set times will be returned relative to UTC rather than
          the users associated timezone
      responses:
        200:
          description: OK
      tags:
      - Profiles
      - Id
      - Updates
      - PendingmediaTypeExtension
  /profiles/{id}/updates/reorder{mediaTypeExtension}:
    post:
      summary: Post Profiles Updates Reorder Mediatypeextension
      description: Edit the order at which statuses for the specified social media
        profile will be sent out of the buffer.
      operationId: edit-the-order-at-which-statuses-for-the-specified-social-media-profile-will-be-sent-out-of-the-buff
      x-api-path-slug: profilesidupdatesreordermediatypeextension-post
      parameters:
      - in: path
        name: id
      - in: path
        name: mediaTypeExtension
      responses:
        200:
          description: OK
      tags:
      - Profiles
      - Id
      - Updates
      - ReordermediaTypeExtension
  /profiles/{id}/updates/sent{mediaTypeExtension}:
    get:
      summary: Get Profiles Updates Sent Mediatypeextension
      description: Returns an array of updates that have been sent from the buffer
        for an individual social media profile.
      operationId: returns-an-array-of-updates-that-have-been-sent-from-the-buffer-for-an-individual-social-media-profi
      x-api-path-slug: profilesidupdatessentmediatypeextension-get
      parameters:
      - in: query
        name: count
        description: Specifies the number of status updates to receive
      - in: path
        name: id
      - in: path
        name: mediaTypeExtension
      - in: query
        name: page
        description: Specifies the page of status updates to receive
      - in: query
        name: since
        description: Specifies a unix timestamp which only status updates created
          after this time will be retrieved
      - in: query
        name: utc
        description: If utc is set times will be returned relative to UTC rather than
          the users associated timezone
      responses:
        200:
          description: OK
      tags:
      - Profiles
      - Id
      - Updates
      - SentmediaTypeExtension
  /profiles/{id}/updates/shuffle{mediaTypeExtension}:
    post:
      summary: Post Profiles Updates Shuffle Mediatypeextension
      description: Randomize the order at which statuses for the specified social
        media profile will be sent out of the buffer.
      operationId: randomize-the-order-at-which-statuses-for-the-specified-social-media-profile-will-be-sent-out-of-the
      x-api-path-slug: profilesidupdatesshufflemediatypeextension-post
      parameters:
      - in: path
        name: id
      - in: path
        name: mediaTypeExtension
      responses:
        200:
          description: OK
      tags:
      - Profiles
      - Id
      - Updates
      - ShufflemediaTypeExtension
  /profiles/{id}{mediaTypeExtension}:
    get:
      summary: Get Profiles Mediatypeextension
      description: Returns details of the single specified social media profile.
      operationId: returns-details-of-the-single-specified-social-media-profile-
      x-api-path-slug: profilesidmediatypeextension-get
      parameters:
      - in: path
        name: id
      - in: path
        name: mediaTypeExtension
      responses:
        200:
          description: OK
      tags:
      - Profiles
      - IdmediaTypeExtension
  /profiles{mediaTypeExtension}:
    get:
      summary: Get Profiles Mediatypeextension
      description: Returns an array of social media profiles connected to a users
        account.
      operationId: returns-an-array-of-social-media-profiles-connected-to-a-users-account-
      x-api-path-slug: profilesmediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
      responses:
        200:
          description: OK
      tags:
      - ProfilesmediaTypeExtension
  /updates/create{mediaTypeExtension}:
    post:
      summary: Post Updates Create Mediatypeextension
      description: Create one or more new status updates.
      operationId: create-one-or-more-new-status-updates-
      x-api-path-slug: updatescreatemediatypeextension-post
      parameters:
      - in: path
        name: mediaTypeExtension
      responses:
        200:
          description: OK
      tags:
      - Updates
      - CreatemediaTypeExtension
  /updates/{id}/destroy{mediaTypeExtension}:
    post:
      summary: Post Updates Destroy Mediatypeextension
      description: Permanently delete an existing status update.
      operationId: permanently-delete-an-existing-status-update-
      x-api-path-slug: updatesiddestroymediatypeextension-post
      parameters:
      - in: path
        name: id
      - in: path
        name: mediaTypeExtension
      responses:
        200:
          description: OK
      tags:
      - Updates
      - Id
      - DestroymediaTypeExtension
  /updates/{id}/interactions{mediaTypeExtension}:
    get:
      summary: Get Updates Interactions Mediatypeextension
      description: Returns the detailed information on individual interactions with
        the social media update such as favorites, retweets and likes.
      operationId: returns-the-detailed-information-on-individual-interactions-with-the-social-media-update-such-as-fav
      x-api-path-slug: updatesidinteractionsmediatypeextension-get
      parameters:
      - in: query
        name: count
        description: Specifies the number of status updates to receive
      - in: query
        name: event
        description: Specifies a type of event to be retrieved, for example retweet,
          like, comment, mention or reshare
      - in: path
        name: id
      - in: path
        name: mediaTypeExtension
      - in: query
        name: page
        description: Specifies the page of status updates to receive
      responses:
        200:
          description: OK
      tags:
      - Updates
      - Id
      - InteractionsmediaTypeExtension
  /updates/{id}/move_to_top{mediaTypeExtension}:
    post:
      summary: Post Updates Move To Top Mediatypeextension
      description: Move an existing status update to the top of the queue and recalculate
        times for all updates in the queue. Returns the update with its new posting
        time.
      operationId: move-an-existing-status-update-to-the-top-of-the-queue-and-recalculate-times-for-all-updates-in-the-
      x-api-path-slug: updatesidmove-to-topmediatypeextension-post
      parameters:
      - in: path
        name: id
      - in: path
        name: mediaTypeExtension
      responses:
        200:
          description: OK
      tags:
      - Updates
      - Id
      - Move
      - To
      - TopmediaTypeExtension
  /updates/{id}/share{mediaTypeExtension}:
    post:
      summary: Post Updates Share Mediatypeextension
      description: Immediately shares a single pending update and recalculates times
        for updates remaining in the queue.
      operationId: immediately-shares-a-single-pending-update-and-recalculates-times-for-updates-remaining-in-the-queue
      x-api-path-slug: updatesidsharemediatypeextension-post
      parameters:
      - in: path
        name: id
      - in: path
        name: mediaTypeExtension
      responses:
        200:
          description: OK
      tags:
      - Updates
      - Id
      - SharemediaTypeExtension
  /updates/{id}/update{mediaTypeExtension}:
    post:
      summary: Post Updates Update Mediatypeextension
      description: Edit an existing, individual status update.
      operationId: edit-an-existing-individual-status-update-
      x-api-path-slug: updatesidupdatemediatypeextension-post
      parameters:
      - in: path
        name: id
      - in: path
        name: mediaTypeExtension
      responses:
        200:
          description: OK
      tags:
      - Updates
      - Id
      - UpdatemediaTypeExtension
  /updates/{id}{mediaTypeExtension}:
    get:
      summary: Get Updates Mediatypeextension
      description: Returns a single social media update.
      operationId: returns-a-single-social-media-update-
      x-api-path-slug: updatesidmediatypeextension-get
      parameters:
      - in: path
        name: id
      - in: path
        name: mediaTypeExtension
      responses:
        200:
          description: OK
      tags:
      - Updates
      - IdmediaTypeExtension
  /user{mediaTypeExtension}:
    get:
      summary: Get User Mediatypeextension
      description: Get user mediatypeextension.
      operationId: returns-a-single-user-
      x-api-path-slug: usermediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
      responses:
        200:
          description: OK
      tags:
      - UsermediaTypeExtension