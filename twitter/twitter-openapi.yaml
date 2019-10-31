swagger: "2.0"
x-collection-name: Twitter
x-complete: 1
info:
  title: Twitter
  description: the-twitter-api-gives-you-programmatic-control-over-any-twitter-account-and-most-aspect-of-the-platform--allowing-developers-to-build-social-applications-that-use-the-platform-and-automate-interactions-between-users-
  version: "1.1"
host: api.twitter.com
basePath: /1.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /statuses/mentions_timeline:
    get:
      summary: Mentions Timelines
      description: Returns the 20 most recent mentions for the authenticating user
      operationId: returns-the-20-most-recent-mentions-for-the-authenticating-user
      x-api-path-slug: statusesmentions-timeline-get
      parameters:
      - in: query
        name: contributor_details
        description: This parameter enhances the contributors element of the status
          response
      - in: query
        name: count
        description: Specifies the number of tweets to try and retrieve
      - in: query
        name: include_entities
        description: The entities node will be disincluded when set to false
      - in: query
        name: max_id
        description: Returns results with an ID less than or equal to the specified
          ID
      - in: query
        name: since_id
        description: Returns result with an ID greater than the specified ID
      - in: query
        name: trim_user
        description: When set to either true, t or 1, each tweet returned in a timeline
          will include a user object
      responses:
        200:
          description: OK
      tags:
      - Social
      - Statuses
  /statuses/user_timeline.json:
    get:
      summary: Show Timelines Status
      description: Returns a collection of the most recent Tweets posted by the User
      operationId: returns-a-collection-of-the-most-recent-tweets-posted-by-the-user
      x-api-path-slug: statusesuser-timeline-json-get
      parameters:
      - in: query
        name: contributor_details
        description: This paramters enhances the contributors element of the status
          response to include the screen_name of the contributor
      - in: query
        name: count
        description: Specifies the number of tweets to try and retrieve
      - in: query
        name: exclude_replies
        description: This paramters will prevent from appearing in the returned timeline
      - in: query
        name: include_rts
        description: When set to false, the timeline will strip any native retweet
      - in: query
        name: max_id
        description: Returns results with an ID less than or equal to the specified
          ID
      - in: query
        name: screen_name
        description: The user screen name
        type: string
        format: string
      - in: query
        name: since_id
        description: Returns result with an ID greater than the specified ID
      - in: query
        name: trim_user
        description: When set to either true, t or 1, each tweet returned in a timeline
          will include a user object
      responses:
        200:
          description: OK
      tags:
      - Social
      - Statuses
  /statuses/home_timeline:
    get:
      summary: Status Timeline
      description: Returns a collection of the most recent Tweets
      operationId: returns-a-collection-of-the-most-recent-tweets
      x-api-path-slug: statuseshome-timeline-get
      parameters:
      - in: query
        name: contributor_details
        description: This paramters enhances the contributors element of the status
          response to include the screen_name of the contributor
      - in: query
        name: exclude_replies
        description: This paramters will prevent from appearing in the returned timeline
      - in: query
        name: max_id
        description: Returns results with an ID less than or equal to the specified
          ID
      - in: query
        name: since_id
        description: Returns result with an ID greater than the specified ID
      - in: query
        name: trim_user
        description: When set to either true, t or 1, each tweet returned in a timeline
          will include a user object
      responses:
        200:
          description: OK
      tags:
      - Social
      - Statuses
  /statuses/retweets/{id}:
    post:
      summary: Show Retweets
      description: Retweens a tweet
      operationId: retweens-a-tweet
      x-api-path-slug: statusesretweetsid-post
      parameters:
      - in: path
        name: id
        description: The numerical ID of the desired status
      - in: query
        name: trim_user
        description: When set to either true, t or 1, each tweet returned in a timeline
          will include a user object
      responses:
        200:
          description: OK
      tags:
      - Social
      - Statuses
  /statuses/show/{id}:
    get:
      summary: Show Retweet
      description: Retruns a single Tweet
      operationId: retruns-a-single-tweet
      x-api-path-slug: statusesshowid-get
      parameters:
      - in: path
        name: id
        description: The numerical ID of the desired status
      - in: query
        name: include_entities
        description: The entities node will be disincluded when set to false
      - in: query
        name: include_my_retweet
        description: When set to either true, t or 1, any Tweets returned that have
          been retweeted by the authenticating
      - in: query
        name: trim_user
        description: When set to either true, t or 1, each tweet returned in a timeline
          will include a user object
      responses:
        200:
          description: OK
      tags:
      - Social
      - Tweets
  /statuses/destroy/{id}:
    post:
      summary: Remove Tweet
      description: Destroys the status specified by the required ID parameter
      operationId: destroys-the-status-specified-by-the-required-id-parameter
      x-api-path-slug: statusesdestroyid-post
      parameters:
      - in: path
        name: id
        description: The numerical ID of the desired status
      - in: query
        name: trim_user
        description: When set to either true, t or 1, each tweet returned in a timeline
          will include a user object
      responses:
        200:
          description: OK
      tags:
      - Social
      - Statuses
  /statuses/update:
    post:
      summary: Update Status
      description: Updates the authenticating user's status
      operationId: updates-the-authenticating-users-status
      x-api-path-slug: statusesupdate-post
      parameters:
      - in: query
        name: display_coordinates
        description: Whether or not to put a pin on the exact coordinates a tweet
      - in: query
        name: in_reply_to_status_id
        description: The ID of an existing status
      - in: query
        name: lat
        description: The latitude of the location
      - in: query
        name: long
        description: The longitude of the location
      - in: query
        name: place_id
        description: A place in the world
      - in: query
        name: status
        description: The text of your status update
      - in: query
        name: trim_user
        description: When set to either true, t or 1, each tweet returned in a timeline
          will include a user object
      responses:
        200:
          description: OK
      tags:
      - Social
      - Statuses
  /statuses/oembed:
    get:
      summary: Oembed Statuses
      description: Returns information allowing the creation of an embedded representation
      operationId: returns-information-allowing-the-creation-of-an-embedded-representation
      x-api-path-slug: statusesoembed-get
      parameters:
      - in: query
        name: align
        description: Specifies whether the embedded Tweet should be left aligned
      - in: query
        name: hide_media
        description: Specifies whether the embedded tweet should automatically show
          the original message in the case that the embedded Tweet is a reply
      - in: query
        name: hide_thread
        description: Specifies whether the embedded Tweet html should include a script
          element pointing to widgets
      - in: query
        name: id
        description: The tweet/status id to return embed code for
      - in: query
        name: lang
        description: Languages code for the rendered embed
      - in: query
        name: maxwidth
        description: The maximum width in pixels that the embed should be rendered
          at
      - in: query
        name: related
        description: A value for the TWT related parameters
      - in: query
        name: url
        description: The encoded URL of the Tweet status to be embedded
      responses:
        200:
          description: OK
      tags:
      - Social
      - Statuses
  /lists/list:
    get:
      summary: List LIst
      description: Return all lists the authenticating or specified user subscribes
        to, including their own.
      operationId: return-all-lists-the-authenticating-or-specified-user-subscribes-to-including-their-own
      x-api-path-slug: listslist-get
      parameters:
      - in: query
        name: screen_name
        description: The screen name of the user for whom to return results for
      - in: query
        name: user_id
        description: The ID of the user for whom to return results for
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/statuses.json:
    get:
      summary: List Statuses
      description: Returns a timeline of tweets authored by memebers of the specified
        list
      operationId: returns-a-timeline-of-tweets-authored-by-memebers-of-the-specified-list
      x-api-path-slug: listsstatuses-json-get
      parameters:
      - in: query
        name: count
        description: Specifies the number of results to retrieve per page
      - in: query
        name: include_entities
        description: Entities are ON by default
      - in: query
        name: include_rts
        description: When set to either true, t or 1, the list timeline will contain
          native retweets in addition to the standard stream of tweets
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: max_id
        description: Returns results with an ID less than or equal to the specified
          ID
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: since_id
        description: Returns results with an ID greater than the sepcified ID
      - in: query
        name: slug
        description: You can identify a list by its slug instead of its numerical
          id
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/members/destroy:
    get:
      summary: Remove User From List
      description: Returns the list of memebers destroy
      operationId: returns-the-list-of-memebers-destroy
      x-api-path-slug: listsmembersdestroy-get
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The is of the user who wons the list being requested by a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: slug
        description: You can identify a list by its slug instrad of its numerical
          id
      - in: query
        name: user_id
        description: The id of the user for whom to remove from the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/memberships:
    get:
      summary: Get Memberships
      description: Returns the lists of the specified user has been added to
      operationId: returns-the-lists-of-the-specified-user-has-been-added-to
      x-api-path-slug: listsmemberships-get
      parameters:
      - in: query
        name: cursor
        description: Breaks the results into pages
      - in: query
        name: filter_to_owned_lists
        description: When set to true, t or 1, will return just lists the authenticating
          user owns
      - in: query
        name: screen_name
        description: The screen name of the user for whom to return results for
      - in: query
        name: user_id
        description: The id of the user for whom to return results for
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/subscribers:
    get:
      summary: List Subscribers
      description: Returns the subscribers of the specified list
      operationId: returns-the-subscribers-of-the-specified-list
      x-api-path-slug: listssubscribers-get
      parameters:
      - in: query
        name: cursor
        description: Breaks the results into pages
      - in: query
        name: include_entities
        description: Wehn set to either true, t or 1
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: the screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: skip_status
        description: When set to either true, t or 1
      - in: query
        name: slug
        description: You can identify a list by its slug insted of its numerical id
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/subscribers/create:
    post:
      summary: Add List Subscribers
      description: Subscribes the authenticated user to the specified list
      operationId: subscribes-the-authenticated-user-to-the-specified-list
      x-api-path-slug: listssubscriberscreate-post
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: the screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/subscribers/show:
    get:
      summary: Show List Subscribers
      description: Check if the specified user is a subscriber of the specified list
      operationId: check-if-the-specified-user-is-a-subscriber-of-the-specified-list
      x-api-path-slug: listssubscribersshow-get
      parameters:
      - in: query
        name: include_entities
        description: Wehn set to either true, t or 1
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The is of the user who wons the list being requested by a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: skip_status
        description: When set to either true, t or 1
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      - in: query
        name: user_id
        description: The id of the user for whom to remove from the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/subscribers/destroy:
    get:
      summary: Remove List Subscribers
      description: Returns list of subscribers destroy
      operationId: returns-list-of-subscribers-destroy
      x-api-path-slug: listssubscribersdestroy-get
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: the screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/members/create_all:
    get:
      summary: Add Users to List
      description: Returns lists of members create_all
      operationId: returns-lists-of-members-create-all
      x-api-path-slug: listsmemberscreate-all-get
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: the screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      - in: query
        name: user_id
        description: The id of the user for whom to remove from the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /list/members/show:
    get:
      summary: Show Members
      description: Check if the specified user is a member of the specified list
      operationId: check-if-the-specified-user-is-a-member-of-the-specified-list
      x-api-path-slug: listmembersshow-get
      parameters:
      - in: query
        name: include_entities
        description: Wehn set to either true, t or 1
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: skip_status
        description: When set to either true, t or 1
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      - in: query
        name: user_id
        description: The id of the user for whom to remove from the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /list/members:
    get:
      summary: Get Members
      description: Returns the members of the specified list
      operationId: returns-the-members-of-the-specified-list
      x-api-path-slug: listmembers-get
      parameters:
      - in: query
        name: cursor
        description: Breaks the results into pages
      - in: query
        name: include_entities
        description: Wehn set to either true, t or 1
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: skip_status
        description: When set to either true, t or 1
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /list/members/create:
    post:
      summary: Add Member
      description: Returns list of members create
      operationId: returns-list-of-members-create
      x-api-path-slug: listmemberscreate-post
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/destroy:
    post:
      summary: Destroy List
      description: Returns list of destroy
      operationId: returns-list-of-destroy
      x-api-path-slug: listsdestroy-post
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/update:
    post:
      summary: Update List
      description: Returns lists of updates
      operationId: returns-lists-of-updates
      x-api-path-slug: listsupdate-post
      parameters:
      - in: query
        name: description
        description: The description to give the list
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: mode
        description: Whether your list is public or private
      - in: query
        name: name
        description: The name for the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/create:
    post:
      summary: Create List
      description: Returns list of create
      operationId: returns-list-of-create
      x-api-path-slug: listscreate-post
      parameters:
      - in: query
        name: description
        description: The description to give the list
      - in: query
        name: mode
        description: Whether your list is public or private
      - in: query
        name: name
        description: The name for the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/show:
    get:
      summary: Show LIsts
      description: Returns list of show
      operationId: returns-list-of-show
      x-api-path-slug: listsshow-get
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/subscriptions:
    get:
      summary: Show List Subscriptions
      description: Returns list of subscriptions
      operationId: returns-list-of-subscriptions
      x-api-path-slug: listssubscriptions-get
      parameters:
      - in: query
        name: count
        description: The amount of results to return per page
      - in: query
        name: cursor
        description: Breaks the results into pages
      - in: query
        name: screen_name
        description: The screen name of the user
      - in: query
        name: user_id
        description: The id of the user for whom to return results for
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /list/members/destroy_all:
    get:
      summary: Remove Members
      description: Returns lists of destroy all
      operationId: returns-lists-of-destroy-all
      x-api-path-slug: listmembersdestroy-all-get
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      - in: query
        name: user_id
        description: The id of the user for whom to remove from the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /direct_messages/sent:
    get:
      summary: Get Sent Direct Messages
      description: return 20 most recent direct messages sent
      operationId: return-20-most-recent-direct-messages-sent
      x-api-path-slug: direct-messagessent-get
      parameters:
      - in: query
        name: count
      - in: query
        name: include_entities
      - in: query
        name: max_id
      - in: query
        name: page
      - in: query
        name: since_id
      responses:
        200:
          description: OK
      tags:
      - Social
      - Messages
  /direct_messages/show:
    get:
      summary: Show Direct Message
      description: returns a single direct message specified by an id
      operationId: returns-a-single-direct-message-specified-by-an-id
      x-api-path-slug: direct-messagesshow-get
      parameters:
      - in: query
        name: id
        description: ID of direct message
      responses:
        200:
          description: OK
      tags:
      - Social
      - Messages
  /search/tweets.json:
    get:
      summary: Search Tweets
      description: returns collection of relevant Tweets matching query
      operationId: returns-collection-of-relevant-tweets-matching-query
      x-api-path-slug: searchtweets-json-get
      parameters:
      - in: query
        name: callback
        description: response will use the callback with given name
      - in: query
        name: count
        description: number of tweets to return
      - in: query
        name: geocode
        description: returns tweets by users located within given radius
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: lang
        description: restricts tweets to a given language
      - in: query
        name: locale
        description: language of query you are sending
      - in: query
        name: max_id
        description: returns results with an ID less than/equal to specified ID
      - in: query
        name: q
        description: URL-encoded search query of 500 characters max
      - in: query
        name: result_type
        description: specifies type of search results you prefer
      - in: query
        name: since_id
        description: return results with ID greater than specified
      - in: query
        name: until
        description: returns tweets created before given date
      responses:
        200:
          description: OK
      tags:
      - Social
      - Statuses
  /saved_searches/list:
    get:
      summary: List Saved Searches
      description: Returns the authenticated user's saved search queries
      operationId: returns-the-authenticated-users-saved-search-queries
      x-api-path-slug: saved-searcheslist-get
      responses:
        200:
          description: OK
      tags:
      - Social
      - Search
  /saved_searches/show/{id}:
    get:
      summary: Get Saved Search
      description: Retrieve the information for the saved search represented by the
        given id
      operationId: retrieve-the-information-for-the-saved-search-represented-by-the-given-id
      x-api-path-slug: saved-searchesshowid-get
      parameters:
      - in: path
        name: id
        description: The id of the saved search
      responses:
        200:
          description: OK
      tags:
      - Social
      - Search
  /saved_searches/create:
    post:
      summary: Create Saved Search
      description: Create a new saved search for the authenticated user
      operationId: create-a-new-saved-search-for-the-authenticated-user
      x-api-path-slug: saved-searchescreate-post
      parameters:
      - in: query
        name: query
        description: The query of the search the user would like to save
      responses:
        200:
          description: OK
      tags:
      - Social
      - Search
  /saved_searches/destroy/{id}:
    post:
      summary: Destroy Saved Search
      description: Destroy a saved search for the authenticating user
      operationId: destroy-a-saved-search-for-the-authenticating-user
      x-api-path-slug: saved-searchesdestroyid-post
      parameters:
      - in: path
        name: id
        description: The id of the saved search
      responses:
        200:
          description: OK
      tags:
      - Social
      - Search
  /direct_messages:
    get:
      summary: Get Direct Messages
      description: return 20 most recent direct messages sent to user
      operationId: return-20-most-recent-direct-messages-sent-to-user
      x-api-path-slug: direct-messages-get
      parameters:
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: max_id
        description: returns results with an ID less than/equal to specified ID
      - in: query
        name: since_id
        description: return results with ID greater than specified
      - in: query
        name: skip_status
        description: whether or not to include status
      responses:
        200:
          description: OK
      tags:
      - Social
      - Messages
  /direct_messages/destroy:
    post:
      summary: Remove Direct Message
      description: destroys direct messages specified in required ID
      operationId: destroys-direct-messages-specified-in-required-id
      x-api-path-slug: direct-messagesdestroy-post
      parameters:
      - in: query
        name: id
        description: ID of direct message to delete
      - in: query
        name: include_entities
        description: whether or not to include entities
      responses:
        200:
          description: OK
      tags:
      - Social
      - Messages
  /direct_messages/new:
    post:
      summary: Create Direct Message
      description: sends a new direct message to specified user
      operationId: sends-a-new-direct-message-to-specified-user
      x-api-path-slug: direct-messagesnew-post
      parameters:
      - in: query
        name: screen_name
        description: screen name of user receiving message
      - in: query
        name: text
        description: text of your direct message
      - in: query
        name: user_id
        description: description
      responses:
        200:
          description: OK
      tags:
      - Social
      - Messages
  /friends/ids:
    get:
      summary: Get Friends
      description: returns a cursored collection of user IDs followed by user
      operationId: returns-a-cursored-collection-of-user-ids-followed-by-user
      x-api-path-slug: friendsids-get
      parameters:
      - in: query
        name: count
        description: number of IDs to attempt retrieval of
      - in: query
        name: cursor
        description: causes list of connections to be broken in pages
      - in: query
        name: screen_name
        description: screen name of user for whom to return results for
      - in: query
        name: stringify_ids
        description: IDs converted to strings
      - in: query
        name: user_id
        description: ID of user for whom to return results for
      responses:
        200:
          description: OK
      tags:
      - Social
      - Friends
  /followers/ids:
    get:
      summary: Get Followers
      description: returns a cursored collection of user IDs following the user
      operationId: returns-a-cursored-collection-of-user-ids-following-the-user
      x-api-path-slug: followersids-get
      parameters:
      - in: query
        name: count
        description: number of IDs to attempt retrieval of
      - in: query
        name: cursor
        description: causes list of connections to be broken in pages
      - in: query
        name: screen_name
        description: screen name of user for whom to return results for
      - in: query
        name: stringify_ids
        description: IDs converted to strings
      - in: query
        name: user_id
        description: ID of user for whom to return results for
      responses:
        200:
          description: OK
      tags:
      - Social
      - Friends
  /friendships/incoming:
    get:
      summary: Get Friend Requests
      description: returns collection of IDs of users with pending follow request
      operationId: returns-collection-of-ids-of-users-with-pending-follow-request
      x-api-path-slug: friendshipsincoming-get
      parameters:
      - in: query
        name: cursor
        description: causes list of connections to be broken in pages
      - in: query
        name: stringify_ids
        description: IDs converted to strings
      responses:
        200:
          description: OK
      tags:
      - Social
      - Friends
  /friendships/outgoing:
    get:
      summary: Get Friend Requests
      description: returns collection of IDs of users with pending follow request
        from the user
      operationId: returns-collection-of-ids-of-users-with-pending-follow-request-from-the-user
      x-api-path-slug: friendshipsoutgoing-get
      parameters:
      - in: query
        name: cursor
        description: causes list of connections to be broken in pages
      - in: query
        name: stringify_ids
        description: IDs converted to strings
      responses:
        200:
          description: OK
      tags:
      - Social
      - Friends
  /friendships/create:
    post:
      summary: Follow User
      description: allows users to follow user sepcified by ID
      operationId: allows-users-to-follow-user-sepcified-by-id
      x-api-path-slug: friendshipscreate-post
      parameters:
      - in: query
        name: follow
        description: enable notifications for target user
      - in: query
        name: screen_name
        description: screen name of user for whom to befriend
      - in: query
        name: user_id
        description: ID of user for whom to befriend
      responses:
        200:
          description: OK
      tags:
      - Social
      - Friends
  /friendships/destroy:
    post:
      summary: Unfollow user
      description: allows user to unfollow user psecified by ID
      operationId: allows-user-to-unfollow-user-psecified-by-id
      x-api-path-slug: friendshipsdestroy-post
      parameters:
      - in: query
        name: screen_name
        description: screen name of user for whom to befriend
      - in: query
        name: user_id
        description: ID of user for whom to befriend
      responses:
        200:
          description: OK
      tags:
      - Social
      - Friends
  /friendships/update:
    post:
      summary: Unfollow User
      description: Allows one to enable or disable settings for specified user
      operationId: allows-one-to-enable-or-disable-settings-for-specified-user
      x-api-path-slug: friendshipsupdate-post
      parameters:
      - in: query
        name: device
        description: enable/disable device notifications for user
      - in: query
        name: retweets
        description: enable/disable retweets from target user
      - in: query
        name: screen_name
        description: screen name of user for whom to befriend
      - in: query
        name: user_id
        description: ID of user for whom to befriend
      responses:
        200:
          description: OK
      tags:
      - Social
      - Friends
  /friendships/show:
    get:
      summary: Get Friends
      description: returns detailed info about relationship between two users
      operationId: returns-detailed-info-about-relationship-between-two-users
      x-api-path-slug: friendshipsshow-get
      parameters:
      - in: query
        name: source_id
        description: user id of subject user
      - in: query
        name: source_screen_name
        description: screen_name of subject user
      - in: query
        name: target_id
        description: user id of target user
      - in: query
        name: target_screen_name
        description: screen name of target user
      responses:
        200:
          description: OK
      tags:
      - Social
      - Friends
  /account/settings:
    get:
      summary: Get Account Settings
      description: returns settings for user
      operationId: returns-settings-for-user
      x-api-path-slug: accountsettings-get
      responses:
        200:
          description: OK
      tags:
      - Social
      - Account
    post:
      summary: Update  Account Settings
      description: updates user's settings
      operationId: updates-users-settings
      x-api-path-slug: accountsettings-post
      parameters:
      - in: query
        name: end_sleep_time
        description: the hour that sleep time should end if enabled
      - in: query
        name: lang
        description: language which Twitter should render in for the user
      - in: query
        name: sleep_time_enabled
        description: enables/disables sleep time, silencing notifications
      - in: query
        name: start_sleep_time
        description: the hour that sleep time should begin if enabled
      - in: query
        name: time_zone
        description: timezone dates and times should be displayed in
      - in: query
        name: trend_location_woeid
        description: the Yahoo! Where On Earth ID to user as defaul tend location
      responses:
        200:
          description: OK
      tags:
      - Social
      - Account
  /account/update_delivery_device:
    post:
      summary: Update Account Deliver Service
      description: sets which device Twitter delivers updates to for user
      operationId: sets-which-device-twitter-delivers-updates-to-for-user
      x-api-path-slug: accountupdate-delivery-device-post
      parameters:
      - in: query
        name: device
        description: must be one of sms, none
      - in: query
        name: include_entities
        description: whether or not to include entities
      responses:
        200:
          description: OK
      tags:
      - Social
      - Account
  /account/update_profile:
    post:
      summary: Update Profile
      description: sets values that users ar eable to set under Account tab
      operationId: sets-values-that-users-ar-eable-to-set-under-account-tab
      x-api-path-slug: accountupdate-profile-post
      parameters:
      - in: query
        name: description
        description: a description of user owning account
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: location
        description: city or country describing where user of account is
      - in: query
        name: name
        description: full name of profile
      - in: query
        name: skip_status
        description: whether or not to include statuses in response
      - in: query
        name: url
        description: url associated with profile
      responses:
        200:
          description: OK
      tags:
      - Social
      - Account
  /account/update_profile_background_image:
    post:
      summary: Update Profile Background Image
      description: updates user's profile background image
      operationId: updates-users-profile-background-image
      x-api-path-slug: accountupdate-profile-background-image-post
      parameters:
      - in: formData
        name: file
        description: image to replace background image of profile
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: skip_status
        description: whether or not to include status in returned user objects
      - in: query
        name: tile
        description: whether or not to tile background image
      - in: query
        name: use
        description: display background image or not
      responses:
        200:
          description: OK
      tags:
      - Social
      - Account
  /account/update_profile_colors:
    post:
      summary: Update Profile Colors
      description: sets one or more hex values that controls color scheme
      operationId: sets-one-or-more-hex-values-that-controls-color-scheme
      x-api-path-slug: accountupdate-profile-colors-post
      parameters:
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: profile_background_color
        description: profile background color
      - in: query
        name: profile_link_color
        description: profile link color
      - in: query
        name: profile_sidebar_border_color
        description: profile sidebars border color
      - in: query
        name: profile_sidebar_fill_color
        description: profiles sidebar background color
      - in: query
        name: profile_text_color
        description: profile text color
      - in: query
        name: skip_status
        description: whether or not to include statuses
      responses:
        200:
          description: OK
      tags:
      - Social
      - Account
  /account/update_profile_image:
    post:
      summary: Update Profile Image
      description: updates user's profile image
      operationId: updates-users-profile-image
      x-api-path-slug: accountupdate-profile-image-post
      parameters:
      - in: formData
        name: image
        description: image to be set as profile image
      - in: query
        name: skip_status
        description: whether or not to include statuses
      responses:
        200:
          description: OK
      tags:
      - Social
      - Account
  /blocks/list:
    get:
      summary: Block List
      description: disallows retweets and device notifications from a user
      operationId: disallows-retweets-and-device-notifications-from-a-user
      x-api-path-slug: blockslist-get
      parameters:
      - in: query
        name: cursor
        description: breaks block of user to be broken up into pages
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: skip_status
        description: whether or not to include statuses in response
      responses:
        200:
          description: OK
      tags:
      - Social
      - Block
  /blocks/ids:
    get:
      summary: Block Users
      description: returns array of numeric user ids of blocked users
      operationId: returns-array-of-numeric-user-ids-of-blocked-users
      x-api-path-slug: blocksids-get
      parameters:
      - in: query
        name: cursor
        description: breaks up block of user IDs into pages
      - in: query
        name: stringify_ids
        description: returns array of numeric IDs as string IDs
      responses:
        200:
          description: OK
      tags:
      - Social
      - Block
  /blocks/create:
    post:
      summary: Block User
      description: blocks the specified user
      operationId: blocks-the-specified-user
      x-api-path-slug: blockscreate-post
      parameters:
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: screen_name
        description: screen name of user to be blocked
      - in: query
        name: skip_status
        description: whether or not to skip statuses
      - in: query
        name: user_id
        description: ID of user to be blocked
      responses:
        200:
          description: OK
      tags:
      - Social
      - Block
  /blocks/destroy:
    post:
      summary: Unblock User
      description: un-blocks the specified user
      operationId: unblocks-the-specified-user
      x-api-path-slug: blocksdestroy-post
      parameters:
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: screen_name
        description: screen name of user to be un-blocked
      - in: query
        name: skip_status
        description: whether or not to skip statuses
      - in: query
        name: user_id
        description: ID of user to be un-blocked
      responses:
        200:
          description: OK
      tags:
      - Social
      - Block
  /users/lookup:
    get:
      summary: User Lookup
      description: returns fully-hydrated user objects up to 100
      operationId: returns-fullyhydrated-user-objects-up-to-100
      x-api-path-slug: userslookup-get
      parameters:
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: screen_name
        description: screen name of user to lookup
      - in: query
        name: user_id
        description: ID of user to lookup
      responses:
        200:
          description: OK
      tags:
      - Social
      - Users
  /users/show:
    get:
      summary: Show User
      description: returns a variety of info about specified user
      operationId: returns-a-variety-of-info-about-specified-user
      x-api-path-slug: usersshow-get
      parameters:
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: screen_name
        description: screen name of user to be shown
      - in: query
        name: user_id
        description: ID of user to be shown
      responses:
        200:
          description: OK
      tags:
      - Social
      - Users
  /users/search.json:
    get:
      summary: User Search
      description: simple relevance-based user search
      operationId: simple-relevancebased-user-search
      x-api-path-slug: userssearch-json-get
      parameters:
      - in: query
        name: count
        description: number of people to return per page
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: page
        description: specifies the page of results to receive
      - in: query
        name: q
        description: the search query to run against people search
      responses:
        200:
          description: OK
      tags:
      - Social
      - Users
  /users/contributees:
    get:
      summary: User Contributees
      description: collection of users specified user can contribute to
      operationId: collection-of-users-specified-user-can-contribute-to
      x-api-path-slug: userscontributees-get
      parameters:
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: screen_name
        description: screen name of user that is contributed to
      - in: query
        name: skip_status
        description: whether or not to skip statuses
      - in: query
        name: user_id
        description: ID of user to that is contributed to
      responses:
        200:
          description: OK
      tags:
      - Social
      - Users
  /users/contributors:
    get:
      summary: User Contributors
      description: collection of users that can contribute to specified account
      operationId: collection-of-users-that-can-contribute-to-specified-account
      x-api-path-slug: userscontributors-get
      parameters:
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: screen_name
        description: screen name of user contributing
      - in: query
        name: skip_status
        description: whether or not to skip statuses
      - in: query
        name: user_id
        description: ID of user contributing
      responses:
        200:
          description: OK
      tags:
      - Social
      - Users
  /geo/id/{place_id}:
    get:
      summary: Get Place
      description: Returns all the information about a know place
      operationId: returns-all-the-information-about-a-know-place
      x-api-path-slug: geoidplace-id-get
      parameters:
      - in: path
        name: place_id
        description: A place in the world
      responses:
        200:
          description: OK
      tags:
      - Places
  /geo/reverse_geoncode:
    get:
      summary: Get Lat / Log
      description: Given a latitude and a longitude, searches for up to 20 places
        that can be used as a place_id when updatting a status
      operationId: given-a-latitude-and-a-longitude-searches-for-up-to-20-places-that-can-be-used-as-a-place-id-when-up
      x-api-path-slug: georeverse-geoncode-get
      parameters:
      - in: query
        name: accuracy
        description: A hint on region in which to search
      - in: query
        name: callback
        description: If supplied, the responses will use the JSON format with a callback
          of the given name
      - in: query
        name: granularity
        description: This is the minimal granularity of place types to return
      - in: query
        name: lat
        description: The latitude to search around
      - in: query
        name: long
        description: The longtitude to search around
      - in: query
        name: max_results
        description: A hint as to the number of results to return
      responses:
        200:
          description: OK
      tags:
      - Places
      - Search
  /geo/search:
    get:
      summary: Geo Search
      description: Search for places that can be attached to a statuses/updates
      operationId: search-for-places-that-can-be-attached-to-a-statusesupdates
      x-api-path-slug: geosearch-get
      parameters:
      - in: query
        name: accuracy
        description: A hint on region in which to search
      - in: query
        name: attribute:street_address
        description: This parameter searches for places which have this givven street
          address
      - in: query
        name: callback
        description: If supplied, the responses will use the JSON format with a callback
          of the given name
      - in: query
        name: contained_within
        description: This is the place_id which you would like to restrict the search
          results to
      - in: query
        name: granularity
        description: This is the minimal granularity of place types to return
      - in: query
        name: ip
        description: An Ip address
      - in: query
        name: lat
        description: The latitude to search around
      - in: query
        name: long
        description: The longtitude to search around
      - in: query
        name: query
        description: Free-form text to match against while executing a geo-based query
      responses:
        200:
          description: OK
      tags:
      - Places
      - Similar
  /geo/similar_places:
    get:
      summary: Get Similar Places
      description: Locates places near the given coordinates which are similar in
        name
      operationId: locates-places-near-the-given-coordinates-which-are-similar-in-name
      x-api-path-slug: geosimilar-places-get
      parameters:
      - in: query
        name: attribute:street_address
        description: This parameter searches for places which have this givven street
          address
      - in: query
        name: callback
        description: If supplied, the responses will use the JSON format with a callback
          of the given name
      - in: query
        name: contained_within
        description: This is the place_id which you would like to restrict the search
          results to
      - in: query
        name: lat
        description: The latitude to search around
      - in: query
        name: long
        description: The longtitude to search around
      - in: query
        name: name
        description: The name a place is known as
      responses:
        200:
          description: OK
      tags:
      - Places
      - Similar
  /geo/places:
    get:
      summary: Get Places
      description: Create a new place object at the given latitude and logitude
      operationId: create-a-new-place-object-at-the-given-latitude-and-logitude
      x-api-path-slug: geoplaces-get
      parameters:
      - in: query
        name: attribute:street_address
        description: This parameter searches for places which have this givven street
          address
      - in: query
        name: callback
        description: If supplied, the responses will use the JSON format with a callback
          of the given name
      - in: query
        name: contained_within
        description: This is the place_id which you would like to restrict the search
          results to
      - in: query
        name: lat
        description: The latitude to search around
      - in: query
        name: long
        description: The longtitude to search around
      - in: query
        name: name
        description: The name a place is known as
      - in: query
        name: token
        description: The token found in the response from geo/similar_places
      responses:
        200:
          description: OK
      tags:
      - Places
  /trends/place.json:
    get:
      summary: Show Place Trends
      description: Returns the top 10 trending topics for a specific WOEID
      operationId: returns-the-top-10-trending-topics-for-a-specific-woeid
      x-api-path-slug: trendsplace-json-get
      parameters:
      - in: query
        name: exclude
        description: Setting this equal to hashtages will remove all hashtages from
          the trends list
      - in: query
        name: id
        description: The yahoo where on earch id
      responses:
        200:
          description: OK
      tags:
      - Social
      - Trends
  /trends/available.json:
    get:
      summary: Show Available Trends
      description: Returns the availability
      operationId: returns-the-availability
      x-api-path-slug: trendsavailable-json-get
      responses:
        200:
          description: OK
      tags:
      - Social
      - Trends
  /trends/closest.json:
    get:
      summary: Show Closes Trends
      description: Returns the location that Twitter has trending topic information
        for
      operationId: returns-the-location-that-twitter-has-trending-topic-information-for
      x-api-path-slug: trendsclosest-json-get
      parameters:
      - in: query
        name: lat
        description: If provided with a long parameter the available trend locations
          wil be stored by distance
      - in: query
        name: long
        description: If provided with a lat parameters the available trend locations
          will be sorted by distance
      responses:
        200:
          description: OK
      tags:
      - Social
      - Trends
  /users/report_spam:
    post:
      summary: Report User Spam
      description: Returna users report spam
      operationId: returna-users-report-spam
      x-api-path-slug: usersreport-spam-post
      parameters:
      - in: query
        name: screen_name
        description: The ID or screen_name of the user you want to report as a spammer
      - in: query
        name: user_id
        description: The ID of the user you want to report as a spammer
      responses:
        200:
          description: OK
      tags:
      - Social
      - Users
      - Spam
  /help/configuration:
    get:
      summary: Help Configuration
      description: Returns the current configuration used by Twitter including twitter.com
        slugs which are not usernames
      operationId: returns-the-current-configuration-used-by-twitter-including-twittercom-slugs-which-are-not-usernames
      x-api-path-slug: helpconfiguration-get
      responses:
        200:
          description: OK
      tags:
      - Help
      - Configuration
  /help/languages:
    get:
      summary: Help Langues
      description: Returns the list of languages supported by Twitter along with the
        language code supported by Twitter
      operationId: returns-the-list-of-languages-supported-by-twitter-along-with-the-language-code-supported-by-twitter
      x-api-path-slug: helplanguages-get
      responses:
        200:
          description: OK
      tags:
      - Languages
  /help/privacy:
    get:
      summary: Help Privacy
      description: Returns Twitter's privacy policy
      operationId: returns-twitters-privacy-policy
      x-api-path-slug: helpprivacy-get
      responses:
        200:
          description: OK
      tags:
      - Terms of Service
  /help/tos:
    get:
      summary: Help Terms of Services
      description: Returns the Twitter Terms of Service
      operationId: returns-the-twitter-terms-of-service
      x-api-path-slug: helptos-get
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /application/rate_limit_status:
    get:
      summary: Get Rate Limit Sttaus
      description: Returns the current rate limits for methods belonging to the specified
        resource families
      operationId: returns-the-current-rate-limits-for-methods-belonging-to-the-specified-resource-families
      x-api-path-slug: applicationrate-limit-status-get
      parameters:
      - in: query
        name: resources
        description: A comma-separated list of resource families you want to know
          the current rate limit disposition for
      responses:
        200:
          description: OK
      tags:
      - Rate Limit