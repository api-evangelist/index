swagger: "2.0"
x-collection-name: Spreaker
x-complete: 1
info:
  title: Spreaker API
  version: v1
host: api.spreaker.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /categories/flat:
    get:
      summary: Get Categories
      description: Retrieves all categories in Spreaker
      operationId: getCategoriesFlat
      x-api-path-slug: categoriesflat-get
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Categories
  /episode/<episode_id>/image:
    put:
      summary: Change Episode Image
      description: Change Episode Image
      operationId: putEpisode<episode>Image
      x-api-path-slug: episodeepisode-idimage-put
      parameters:
      - in: path
        name: episode_id
        description: The unique episode id
      - in: query
        name: image_id
        description: The id of the image to set to the episode
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Change
      - Episode
      - Image
  /episode/{episode_id}:
    delete:
      summary: Delete Episode
      description: Deletes an episode. Theres no way to recover a deleted episode.
      operationId: deleteEpisodeEpisode
      x-api-path-slug: episodeepisode-id-delete
      parameters:
      - in: path
        name: episode_id
        description: The unique episode id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Episode
    get:
      summary: Get Episode
      description: Retrieves an episode by unique identifier.
      operationId: getEpisodeEpisode
      x-api-path-slug: episodeepisode-id-get
      parameters:
      - in: path
        name: episode_id
        description: The episode unique id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Episode
    put:
      summary: Edit Episode
      description: Edit episode info (eg. title, description, category, tags, ...)
      operationId: putEpisodeEpisode
      x-api-path-slug: episodeepisode-id-put
      parameters:
      - in: query
        name: category_id
        description: Episode category
      - in: query
        name: description
        description: Episode description, max length 10k chars
      - in: path
        name: episode_id
        description: the episode id
      - in: query
        name: tags
        description: Episode tags (comma separated)
      - in: query
        name: title
        description: Episode title, max length 40 chars
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Edit
      - Episode
  /episode/{episode_id}/media:
    get:
      summary: Get Episode Media List
      description: Get Episode Media List
      operationId: getEpisodeEpisodeMedia
      x-api-path-slug: episodeepisode-idmedia-get
      parameters:
      - in: path
        name: episode_id
        description: Unique id of episode
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Episode
      - Media
      - List
  /episode/{episode_id}/streams/icy:
    get:
      summary: Get Episode Streams
      description: The response contains a collection of ICY streams.
      operationId: getEpisodeEpisodeStreamsIcy
      x-api-path-slug: episodeepisode-idstreamsicy-get
      parameters:
      - in: query
        name: episode_id
        description: The episode id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Episode
      - Streams
  /episode/{episode_id}/streams/rtmp:
    get:
      summary: Get Episode Streams
      description: The response contains a collection of RTMP / RTMPT streams.
      operationId: getEpisodeEpisodeStreamsRtmp
      x-api-path-slug: episodeepisode-idstreamsrtmp-get
      parameters:
      - in: path
        name: episode_id
        description: The episode id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Episode
      - Streams
  /episodes/live:
    get:
      summary: Get Live Episodes
      description: Retrieves all live episodes at the moment of the request
      operationId: getEpisodesLive
      x-api-path-slug: episodeslive-get
      parameters:
      - in: query
        name: show_id
        description: An list of show_id applied as a filter
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Live
      - Episodes
  /explore/{category_id}:
    get:
      summary: Explore Category Items
      description: 'This API returns information and items of a specific category.
        The response contains two properties at root level:'
      operationId: getExploreCategory
      x-api-path-slug: explorecategory-id-get
      parameters:
      - in: query
        name: explore_category
        description: contains category information, the exact same information exported
          by /explore/categories API
      - in: query
        name: items
        description: contains a sorted list of shows or episodes, depending on the
          category type (type 1 and 3 contain episodes, type 2 contains shows)
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Explore
      - Category
      - Items
  /library/{user_id}:
    post:
      summary: Create Media
      description: Upload a new Media in the specified user library
      operationId: postLibraryUser
      x-api-path-slug: libraryuser-id-post
      parameters:
      - in: path
        name: Filedata
        description: The file to upload, encoded multipart/form-data
      - in: query
        name: length
        description: The media length in milliseconds
      - in: query
        name: style_id
        description: The music style associated to this media
      - in: query
        name: type
        description: 'The media type: can be one of SONG, JINGLE, LOOP, UNKNOWN, EFFECT,
          EPISODE'
      - in: path
        name: user_id
        description: The unique user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Media
  /library/{user_id}/effects/owned:
    get:
      summary: Get Owned Media
      description: Get a paginated list of media owned by <user_id> filtered by type:.
      operationId: getLibraryUserEffectsOwned
      x-api-path-slug: libraryuser-ideffectsowned-get
      parameters:
      - in: query
        name: sort_col
        description: The column upon which the results are sorted
      - in: query
        name: sort_dir
        description: The direction of sorting
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Owned
      - Media
  /library/{user_id}/jingles/owned:
    get:
      summary: Get Owned Media
      description: Get a paginated list of media owned by <user_id> filtered by type:.
      operationId: getLibraryUserJinglesOwned
      x-api-path-slug: libraryuser-idjinglesowned-get
      parameters:
      - in: query
        name: sort_col
        description: The column upon which the results are sorted
      - in: query
        name: sort_dir
        description: The direction of sorting
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Owned
      - Media
  /library/{user_id}/loops/owned:
    get:
      summary: Get Owned Media
      description: Get a paginated list of media owned by <user_id> filtered by type:.
      operationId: getLibraryUserLoopsOwned
      x-api-path-slug: libraryuser-idloopsowned-get
      parameters:
      - in: query
        name: sort_col
        description: The column upon which the results are sorted
      - in: query
        name: sort_dir
        description: The direction of sorting
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Owned
      - Media
  /library/{user_id}/songs/owned:
    get:
      summary: Get Owned Media
      description: Get a paginated list of media owned by <user_id> filtered by type:.
      operationId: getLibraryUserSongsOwned
      x-api-path-slug: libraryuser-idsongsowned-get
      parameters:
      - in: query
        name: sort_col
        description: The column upon which the results are sorted
      - in: query
        name: sort_dir
        description: The direction of sorting
      - in: query
        name: user_id
        description: Users id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Owned
      - Media
  /library/{user_id}/soundtracks/owned:
    get:
      summary: Get Owned Media
      description: Get a paginated list of media owned by <user_id> filtered by type:.
      operationId: getLibraryUserSoundtracksOwned
      x-api-path-slug: libraryuser-idsoundtracksowned-get
      parameters:
      - in: query
        name: sort_col
        description: The column upon which the results are sorted
      - in: query
        name: sort_dir
        description: The direction of sorting
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Owned
      - Media
  /lives/top:
    get:
      summary: Get Top Live Episodes
      description: Retrieves live episodes sorted by rank
      operationId: getLivesTop
      x-api-path-slug: livestop-get
      parameters:
      - in: query
        name: I
        description: The rank is language - based
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Top
      - Live
      - Episodes
  /media/{media_id}:
    get:
      summary: Get Media
      description: Retrieves a Media by unique identifier.
      operationId: getMediaMedia
      x-api-path-slug: mediamedia-id-get
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Media
  /search/{query}:
    get:
      summary: Search users, shows and episodes
      description: Search users, shows and episodes
      operationId: getSearchQuery
      x-api-path-slug: searchquery-get
      parameters:
      - in: path
        name: query
        description: Search query
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Search
      - Users
      - ""
      - Shows
      - Episodes
  /show/search/{query}:
    get:
      summary: Search Shows
      description: This API allows to find shows.
      operationId: getShowSearchQuery
      x-api-path-slug: showsearchquery-get
      parameters:
      - in: path
        name: query
        description: Search query
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Search
      - Shows
  /show/{show_id}:
    delete:
      summary: Dele Show
      description: Deletes a show. Theres no way to recover a deleted show. Only show
        without episodes in it can be deleted.
      operationId: deleteShowShow
      x-api-path-slug: showshow-id-delete
      parameters:
      - in: query
        name: description
        description: Show description
      - in: query
        name: email
        description: Shows email contact
      - in: query
        name: facebook_url
        description: Shows facebook page url
      - in: path
        name: show_id
        description: The show id
      - in: query
        name: skype_name
        description: Shows skypy account name
      - in: query
        name: sms_number
        description: Shows sms number (eg
      - in: query
        name: tel_number
        description: Shows telephone number (eg
      - in: query
        name: title
        description: Show title
      - in: query
        name: twitter_name
        description: Shows twitter account name
      - in: query
        name: website_url
        description: Shows website url
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Dele
      - Show
    get:
      summary: Get Show
      description: Retrieves show information.
      operationId: getShowShow
      x-api-path-slug: showshow-id-get
      parameters:
      - in: path
        name: show_id
        description: The show id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Show
    put:
      summary: Edit Show
      description: Edit show info (name, description and contacts).
      operationId: putShowShow
      x-api-path-slug: showshow-id-put
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Edit
      - Show
  /show/{show_id}/episodes:
    get:
      summary: Get Show Episodes
      description: Retrieves all listenable episodes by show (both live and podcast,
        ordered by published_at DESC).
      operationId: getShowShowEpisodes
      x-api-path-slug: showshow-idepisodes-get
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Show
      - Episodes
    post:
      summary: Create podcast
      description: Creates new podcast episode.
      operationId: postShowShowEpisodes
      x-api-path-slug: showshow-idepisodes-post
      parameters:
      - in: query
        name: category_id
        description: Episode category
      - in: query
        name: description
        description: Episode description
      - in: query
        name: download_enabled
        description: Enable / disable download (defaults to true)
      - in: query
        name: explicit
        description: True if the episode contains explicit content (defaults to false)
      - in: query
        name: hidden
        description: True if the episode should be private (defaults to false)
      - in: query
        name: media_id
        description: The single media_id or ordered list of media_id that compose
          the episode
      - in: query
        name: shares
        description: The channels on which this episode has to be shared
      - in: path
        name: show_id
        description: Unique show id
      - in: query
        name: tags
        description: Episode tags (comma separated)
      - in: query
        name: title
        description: Episode title
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Podcast
  /show/{show_id}/episodes/all:
    get:
      summary: Get All Show Episodes
      description: Retrieves all episodes by show (both live and podcast, ordered
        by published_at DESC).
      operationId: getShowShowEpisodesAll
      x-api-path-slug: showshow-idepisodesall-get
      parameters:
      - in: path
        name: show_id
        description: The unique show id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Show
      - Episodes
  /shows:
    post:
      summary: Create Show
      description: Create a new Show.
      operationId: postShows
      x-api-path-slug: shows-post
      parameters:
      - in: query
        name: title
        description: Show title
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Show
  /user/{followed_id}/fans:
    get:
      summary: Get List of Followers
      description: Get List of Followers
      operationId: getUserFollowedFans
      x-api-path-slug: userfollowed-idfans-get
      parameters:
      - in: path
        name: followed_id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - List
      - Of
      - Followers
    post:
      summary: Follow User
      description: Follow User
      operationId: postUserFollowedFans
      x-api-path-slug: userfollowed-idfans-post
      parameters:
      - in: path
        name: followed_id
        description: Allows the authenticating user to follow the user specified in
          the  parameter
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Follow
      - User
  /user/{followed_id}/fans/{follower_id}:
    delete:
      summary: Unfollow User
      description: Unfollow User
      operationId: deleteUserFollowedFansFollower
      x-api-path-slug: userfollowed-idfansfollower-id-delete
      parameters:
      - in: path
        name: followed_id
      - in: path
        name: follower_id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Unfollow
      - User
  /user/{follower_id}/users/fan:
    get:
      summary: Get List of Following
      description: Get List of Following
      operationId: getUserFollowerUsersFan
      x-api-path-slug: userfollower-idusersfan-get
      parameters:
      - in: path
        name: follower_id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - List
      - Of
      - Following
  /user/{user_id}:
    get:
      summary: Get User
      description: Retrieves an user by unique identifier.
      operationId: getUserUser
      x-api-path-slug: useruser-id-get
      parameters:
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - User
    put:
      summary: Edit User
      description: Edit user info (eg. fullname, description aka biography, gender,
        birthday, ...).
      operationId: putUserUser
      x-api-path-slug: useruser-id-put
      parameters:
      - in: query
        name: description
        description: User biography, max length 180 chars
      - in: query
        name: fullname
        description: User fullname, max length 30 chars
      - in: query
        name: gender
        description: 'User gender: can be MALE or FEMALE'
      - in: query
        name: show_age
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Edit
      - User
  /user/{user_id}/actions:
    get:
      summary: Get User Actions
      description: Retrieves the user actions settings
      operationId: getUserUserActions
      x-api-path-slug: useruser-idactions-get
      parameters:
      - in: query
        name: EPISODE_BROADCAST
        description: The user has published a new episode ( either live or podcast
          )
      - in: query
        name: FACEBOOK
        description: The user wants to share on facebook the specified action
      - in: query
        name: RADIO_FOLLOW
        description: The user starts following a radio
      - in: query
        name: RADIO_MESSAGE
        description: The user has sent a message to a radio
      - in: query
        name: SHOW_FOLLOW
        description: The user starts following a show
      - in: query
        name: SHOW_MESSAGE
        description: The user has sent a message to a show
      - in: query
        name: TWITTER
        description: The user wants to share on twitter the specified action
      - in: query
        name: USER_FOLLOW
        description: The user starts following another user
      - in: query
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - User
      - Actions
  /user/{user_id}/actions/facebook:
    get:
      summary: Facebook Settings
      description: Edit facebook share settings.
      operationId: getUserUserActionsFacebook
      x-api-path-slug: useruser-idactionsfacebook-get
      parameters:
      - in: query
        name: EPISODE_BROADCAST
        description: on to enable sharing when the user has published a new episode,
          off otherwise
      - in: query
        name: RADIO_FOLLOW
        description: on to enable sharing when the user starts following a radio,
          off otherwise
      - in: query
        name: RADIO_MESSAGE
        description: on to enable sharing when the user has sent a message to a radio,
          off otherwise
      - in: query
        name: SHOW_FOLLOW
        description: on to enable sharing when the user starts following a show, off
          otherwise
      - in: query
        name: SHOW_MESSAGE
        description: on to enable sharing when the user has sent a message to a show,
          off otherwise
      - in: query
        name: USER_FOLLOW
        description: on to enable sharing when the user starts following another user,
          off otherwise
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Facebook
      - Settings
  /user/{user_id}/actions/twitter:
    put:
      summary: Twitter Settings
      description: Edit twitter share settings.
      operationId: putUserUserActionsTwitter
      x-api-path-slug: useruser-idactionstwitter-put
      parameters:
      - in: query
        name: EPISODE_BROADCAST
        description: on to enable sharing when the user has published a new episode,
          off otherwise
      - in: query
        name: RADIO_FOLLOW
        description: on to enable sharing when the user starts following a radio,
          off otherwise
      - in: query
        name: SHOW_FOLLOW
        description: on to enable sharing when the user starts following a show, off
          otherwise
      - in: query
        name: USER_FOLLOW
        description: on to enable sharing when the user starts following another user,
          off otherwise
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Twitter
      - Settings
  /user/{user_id}/device/{token}:
    delete:
      summary: Delete Device
      description: Delete the association from a mobile device and a registered user
      operationId: deleteUserUserDeviceToken
      x-api-path-slug: useruser-iddevicetoken-delete
      parameters:
      - in: path
        name: token
        description: The device token
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Device
  /user/{user_id}/devices:
    get:
      summary: Create Device
      description: Creates a new device.
      operationId: getUserUserDevices
      x-api-path-slug: useruser-iddevices-get
      parameters:
      - in: query
        name: application_id
        description: The application related to the request
      - in: path
        name: Delete Device
        description: The user id
      - in: query
        name: device_name
        description: The device name, max length 255
      - in: query
        name: device_token
        description: The device token, max length 255
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Device
  /user/{user_id}/episodes:
    get:
      summary: Get User Episodes
      description: Retrieves all listenable episodes by user (both live and podcast,
        ordered by published_at DESC).
      operationId: getUserUserEpisodes
      x-api-path-slug: useruser-idepisodes-get
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - User
      - Episodes
  /user/{user_id}/image:
    put:
      summary: Change User Profile Image
      description: Change User Profile Image
      operationId: putUserUserImage
      x-api-path-slug: useruser-idimage-put
      parameters:
      - in: query
        name: image_id
        description: The id of the image to set to the user profile
      - in: path
        name: user_id
        description: The unique user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Change
      - User
      - Profile
      - Image
  /user/{user_id}/images:
    post:
      summary: Upload An Image
      description: Upload An Image
      operationId: postUserUserImages
      x-api-path-slug: useruser-idimages-post
      parameters:
      - in: body
        name: Filedata
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Upload
      - Image
  /user/{user_id}/lives/fan:
    get:
      summary: Get Favorite Live Episodes
      description: ""
      operationId: getUserUserLivesFan
      x-api-path-slug: useruser-idlivesfan-get
      parameters:
      - in: path
        name: /user/{user_id}/lives/fan
        description: Users id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Favorite
      - Live
      - Episodes
  /user/{user_id}/newsfeed:
    get:
      summary: Newsfeed
      description: This API returns a list of newsfeed items. The request MUST be
        authenticated (an user can only fetch its own newsfeed).
      operationId: getUserUserNewsfeed
      x-api-path-slug: useruser-idnewsfeed-get
      parameters:
      - in: query
        name: last_id
        description: The last newsfeed item received in the previous request, so that
          this request will contains immediately subsequent items
      - in: query
        name: max_per_page
        description: Max number of items in the response
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Newsfeed
  /user/{user_id}/shows/author:
    get:
      summary: GEt Shows By Author
      description: ""
      operationId: getUserUserShowsAuthor
      x-api-path-slug: useruser-idshowsauthor-get
      parameters:
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - GEt
      - Shows
      - Author
  /user/{user_id}/shows/fan:
    get:
      summary: Get Favorite Shows
      description: Retrieves the list of shows whose authors are followed by <user_id>.
      operationId: getUserUserShowsFan
      x-api-path-slug: useruser-idshowsfan-get
      parameters:
      - in: query
        name: latest_episode
        description: True (1) to enable the export of the latest episode
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Favorite
      - Shows
  /users/search/{query}:
    get:
      summary: Search Users
      description: This API allows to find users.
      operationId: getUsersSearchQuery
      x-api-path-slug: userssearchquery-get
      parameters:
      - in: path
        name: query
        description: Search query
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Search
      - Users
  /whoami:
    get:
      summary: Get Authenticated User
      description: Retrieves information about the authenticated user.
      operationId: getWhoami
      x-api-path-slug: whoami-get
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Authenticated
      - User
  show/{show_id}/image:
    put:
      summary: Change Show Image
      description: Change Show Image
      operationId: putShowShowImage
      x-api-path-slug: showshow-idimage-put
      parameters:
      - in: query
        name: image_id
        description: The id of the image to set to the show
      - in: path
        name: show_id
        description: Unique show id
      responses:
        200:
          description: OK
      tags:
      - Podcasts
      - Change
      - Show
      - Image