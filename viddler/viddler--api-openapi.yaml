swagger: "2.0"
x-collection-name: Viddler
x-complete: 1
info:
  title: Viddler  API
  description: the-viddler-api-exposes-viddleru2019s-key-features-to-those-that-would-like-to-build-custom-solutions-on-top-of-viddleru2019s-video-platform-
  termsOfService: http://www.viddler.com/terms-of-use/
  version: v2
host: api.viddler.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  viddler.api.echo:
    get:
      summary: Api Echo
      description: This method is used for testing purposes only. Simply call this
        method to make sure the API is responding fine.
      operationId: api-echo
      x-api-path-slug: viddler-api-echo-get
      parameters:
      - in: query
        name: message
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Api
      - Echo
  viddler.encoding.cancel:
    post:
      summary: Encoding Cancel
      description: Cancel encoding a specific video file.
      operationId: encoding-cancel
      x-api-path-slug: viddler-encoding-cancel-post
      parameters:
      - in: query
        name: file_id
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Encoding
      - Cancel
  viddler.encoding.getSettings:
    get:
      summary: Encoding GetSettings
      description: Returns the current encoding options for an account.
      operationId: encoding-getsettings
      x-api-path-slug: viddler-encoding-getsettings-get
      parameters:
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Encoding
      - GetSettings
  viddler.encoding.getStatus2:
    get:
      summary: Encoding GetStatus2
      description: This method is the same as viddler.encoding.getStatus except that
        it groups files better for users to easily find what they are looking for.
        We could not easily update the previous method without causing complications
        with external applications.
      operationId: encoding-getstatus2
      x-api-path-slug: viddler-encoding-getstatus2-get
      parameters:
      - in: query
        name: sessionid
      - in: query
        name: video_id
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Encoding
      - GetStatus2
  viddler.logins.add:
    post:
      summary: Logins Add
      description: Adds a new login to user account when the main account has multi-user
        sign-on enabled. You must have this feature enabled for your account. Please
        call us at 1-888-444-1119 to enable for you account.
      operationId: logins-add
      x-api-path-slug: viddler-logins-add-post
      parameters:
      - in: query
        name: analytics_permissions
        description: 'options: manage'
      - in: query
        name: api_access_permissions
        description: 'options: manage'
      - in: query
        name: api_settings_permissions
        description: 'options: manage'
      - in: query
        name: billing_settings_permissions
        description: 'options: manage'
      - in: query
        name: branding_settings_permissions
        description: 'options: manage'
      - in: query
        name: email
        description: The email of the user
      - in: query
        name: encoding_settings_permissions
        description: 'options: manage'
      - in: query
        name: interaction_settings_permissions
        description: 'options: manage'
      - in: query
        name: invoices_permissions
        description: 'options: manage'
      - in: query
        name: itunes_settings_permissions
        description: 'options: manage'
      - in: query
        name: login
        description: The login username you would like to create
      - in: query
        name: logins_permissions
        description: 'options: create, read, update and delete'
      - in: query
        name: name
        description: The name of the user
      - in: query
        name: password
        description: The password of the user
      - in: query
        name: player_settings_permissions
        description: 'options: manage'
      - in: query
        name: playlists_permissions
        description: 'options: manage'
      - in: query
        name: playlist_ids
        description: A comma delimited list of playlist IDs this user can view
      - in: query
        name: privacy_settings_permissions
        description: 'options: manage'
      - in: query
        name: profile_permissions
        description: 'options: manage'
      - in: query
        name: recorder_permissions
        description: 'options: manage'
      - in: query
        name: sessionid
      - in: query
        name: subaccounts_permissions
        description: 'options: create, read, update and delete'
      - in: query
        name: support_permissions
        description: 'options: manage'
      - in: query
        name: videos_permissions
        description: 'options: create, read, update and delete'
      - in: query
        name: vidgets_permissions
        description: 'options: manage'
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Logins
      - Add
  viddler.logins.get:
    get:
      summary: Logins Get
      description: Return the current permissions for a specific user.
      operationId: logins-get
      x-api-path-slug: viddler-logins-get-get
      parameters:
      - in: query
        name: login
        description: The login username you would like to return information for
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Logins
      - Get
  viddler.logins.update:
    post:
      summary: Logins Update
      description: Updates a current login.
      operationId: logins-update
      x-api-path-slug: viddler-logins-update-post
      parameters:
      - in: query
        name: analytics_permissions
        description: 'options: manage'
      - in: query
        name: api_access_permissions
        description: 'options: manage'
      - in: query
        name: api_settings_permissions
        description: 'options: manage'
      - in: query
        name: billing_settings_permissions
        description: 'options: manage'
      - in: query
        name: branding_settings_permissions
        description: 'options: manage'
      - in: query
        name: email
        description: The email of the user
      - in: query
        name: encoding_settings_permissions
        description: 'options: manage'
      - in: query
        name: interaction_settings_permissions
        description: 'options: manage'
      - in: query
        name: invoices_permissions
        description: 'options: manage'
      - in: query
        name: itunes_settings_permissions
        description: 'options: manage'
      - in: query
        name: login
        description: The login username you would like to create
      - in: query
        name: logins_permissions
        description: 'options: create, read, update and delete'
      - in: query
        name: name
        description: The name of the user
      - in: query
        name: password
        description: The password of the user
      - in: query
        name: player_settings_permissions
        description: 'options: manage'
      - in: query
        name: playlists_permissions
        description: 'options: manage'
      - in: query
        name: playlist_ids
        description: A comma delimited list of playlist IDs this user can view
      - in: query
        name: privacy_settings_permissions
        description: 'options: manage'
      - in: query
        name: profile_permissions
        description: 'options: manage'
      - in: query
        name: recorder_permissions
        description: 'options: manage'
      - in: query
        name: sessionid
      - in: query
        name: subaccounts_permissions
        description: 'options: create, read, update and delete'
      - in: query
        name: support_permissions
        description: 'options: manage'
      - in: query
        name: videos_permissions
        description: 'options: create, read, update and delete'
      - in: query
        name: vidgets_permissions
        description: 'options: manage'
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Logins
      - Update
  viddler.playlists.create:
    post:
      summary: Playlists Create
      description: Create a playlist. Regular playlist represents user defined videos.
        Smart playlist updates in realtime returning videos matching selected filtering
        rules.
      operationId: playlists-create
      x-api-path-slug: viddler-playlists-create-post
      parameters:
      - in: query
        name: max_age
      - in: query
        name: max_update_date
      - in: query
        name: max_views
      - in: query
        name: min_update_date
      - in: query
        name: min_views
      - in: query
        name: name
      - in: query
        name: playlist_visibility
      - in: query
        name: Regular Playlist Params (all optional)nnvideo_ids
      - in: query
        name: sessionid
      - in: query
        name: Smart Playlist Params (all optional)nnusers
      - in: query
        name: sort
      - in: query
        name: tags
      - in: query
        name: type
      - in: query
        name: visibility
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Playlists
      - Create
  viddler.playlists.delete:
    post:
      summary: Playlists Delete
      description: 'Delete a playlist.u00a0Caution: This operation cannot be undone.'
      operationId: playlists-delete
      x-api-path-slug: viddler-playlists-delete-post
      parameters:
      - in: query
        name: playlist_id
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Playlists
      - Delete
  viddler.playlists.list:
    get:
      summary: Playlists List
      description: List all playlists for an account.
      operationId: playlists-list
      x-api-path-slug: viddler-playlists-list-get
      parameters:
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Playlists
      - List
  viddler.playlists.moveVideo:
    get:
      summary: Playlists MoveVideo
      description: Reorder videos in regular playlist.
      operationId: playlists-movevideo
      x-api-path-slug: viddler-playlists-movevideo-get
      parameters:
      - in: query
        name: from
      - in: query
        name: playlist_id
      - in: query
        name: sessionid
      - in: query
        name: to
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Playlists
      - MoveVideo
  viddler.resellers.getSubaccounts:
    get:
      summary: Resellers GetSubaccounts
      description: List all subaccounts under your account. Only applies to reseller
        accounts. Other accounts do not have access to this method.
      operationId: resellers-getsubaccounts
      x-api-path-slug: viddler-resellers-getsubaccounts-get
      parameters:
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: sessionid
      - in: query
        name: sort
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Resellers
      - GetSubaccounts
  viddler.users.getPlayerBranding:
    get:
      summary: Users GetPlayerBranding
      description: Returns your player branding configuration.
      operationId: users-getplayerbranding
      x-api-path-slug: viddler-users-getplayerbranding-get
      parameters:
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Users
      - GetPlayerBranding
  viddler.users.getProfile:
    get:
      summary: Users GetProfile
      description: Get the public information for a profile. Can only get profile
        information for public profiles.
      operationId: users-getprofile
      x-api-path-slug: viddler-users-getprofile-get
      parameters:
      - in: query
        name: sessionid
      - in: query
        name: user
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Users
      - GetProfile
  viddler.users.getSettings:
    get:
      summary: Users GetSettings
      description: Return account settings.
      operationId: users-getsettings
      x-api-path-slug: viddler-users-getsettings-get
      parameters:
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Users
      - GetSettings
  viddler.users.setPlayerBranding:
    post:
      summary: Users SetPlayerBranding
      description: 'Sets your player branding options. All options are optional other
        than your sessionid. Color formats are inu00a0hexadecimalu00a0format with
        preceding pound sign (IE: #rrggbb)'
      operationId: users-setplayerbranding
      x-api-path-slug: viddler-users-setplayerbranding-post
      parameters:
      - in: query
        name: bclicked
      - in: query
        name: bhover
      - in: query
        name: bidle
      - in: query
        name: control_bar
      - in: query
        name: enable_stripes
      - in: query
        name: logo_align
      - in: query
        name: logo_click_url
      - in: query
        name: logo_offset_x
      - in: query
        name: logo_offset_y
      - in: query
        name: logo_url
      - in: query
        name: logo_visible
      - in: query
        name: pclicked
      - in: query
        name: phover
      - in: query
        name: pidle
      - in: query
        name: sessionid
      - in: query
        name: shade_dark
      - in: query
        name: simple_color
      - in: query
        name: timebackground
      - in: query
        name: timeloaded
      - in: query
        name: timeplayed
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Users
      - SetPlayerBranding
  viddler.users.setProfile:
    get:
      summary: Users SetProfile
      description: Update your profile information.
      operationId: users-setprofile
      x-api-path-slug: viddler-users-setprofile-get
      parameters:
      - in: query
        name: avatar_url
      - in: query
        name: homepage
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Users
      - SetProfile
  viddler.videos.addClosedCaptioning:
    post:
      summary: Videos AddClosedCaptioning
      description: Add new closed captioning file for a specific video. All uploaded
        closed captioning files are enabled by default. The first uploaded file is
        default for a video.
      operationId: videos-addclosedcaptioning
      x-api-path-slug: viddler-videos-addclosedcaptioning-post
      parameters:
      - in: query
        name: closed_captioning_url
      - in: query
        name: default
      - in: query
        name: language
        description: 'The language of the file (Max Characters: 50)'
      - in: query
        name: sessionid
      - in: query
        name: video_id
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Videos
      - AddClosedCaptioning
  viddler.videos.comments.get:
    get:
      summary: Videos Comments Get
      description: Get comments for a video. If logged in and querying comments for
        own video &#8211; all comments with any moderation status will be returned.
        If quering comments as logged out or for not owned video &#8211; only approved
        comments will be returned if the video itself is public.
      operationId: videos-comments-get
      x-api-path-slug: viddler-videos-comments-get-get
      parameters:
      - in: query
        name: page
      - in: query
        name: parent_id
        description: comment parent ID if you want to get the responses to that particular
          comment
      - in: query
        name: per_page
      - in: query
        name: sessionid
      - in: query
        name: video_id
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Videos
      - Comments
      - Get
  viddler.videos.delClosedCaptioning:
    post:
      summary: Videos DelClosedCaptioning
      description: Remove an existing closed captioning file.
      operationId: videos-delclosedcaptioning
      x-api-path-slug: viddler-videos-delclosedcaptioning-post
      parameters:
      - in: query
        name: closed_captioning_id
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Videos
      - DelClosedCaptioning
  viddler.videos.delete:
    post:
      summary: Videos Delete
      description: Delete a video.
      operationId: videos-delete
      x-api-path-slug: viddler-videos-delete-post
      parameters:
      - in: query
        name: sessionid
      - in: query
        name: video_id
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Videos
      - Delete
  viddler.videos.enableAds:
    post:
      summary: Videos EnableAds
      description: Turn ads off for specified videos.
      operationId: videos-enableads
      x-api-path-slug: viddler-videos-enableads-post
      parameters:
      - in: query
        name: sessionid
      - in: query
        name: video_ids
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Videos
      - EnableAds
  viddler.videos.getAdsStatus:
    get:
      summary: Videos GetAdsStatus
      description: viddler.videos.getAdsStatusnGET
      operationId: videos-getadsstatus
      x-api-path-slug: viddler-videos-getadsstatus-get
      parameters:
      - in: query
        name: sessionid
      - in: query
        name: video_id
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Videos
      - GetAdsStatus
  viddler.videos.getEmbedCodeTypes:
    get:
      summary: Videos GetEmbedCodeTypes
      description: Return a list of the embed code types for your account.
      operationId: videos-getembedcodetypes
      x-api-path-slug: viddler-videos-getembedcodetypes-get
      parameters:
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Videos
      - GetEmbedCodeTypes
  viddler.videos.getRecordToken:
    get:
      summary: Videos GetRecordToken
      description: Return a record token to use with Viddler&#8217;s Flash video recorder.
      operationId: videos-getrecordtoken
      x-api-path-slug: viddler-videos-getrecordtoken-get
      parameters:
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Videos
      - GetRecordToken
  viddler.videos.prepareUpload:
    get:
      summary: Videos PrepareUpload
      description: Returns the end-point and token for a new upload session.
      operationId: videos-prepareupload
      x-api-path-slug: viddler-videos-prepareupload-get
      parameters:
      - in: query
        name: allow_replace
        description: Set to true if you are allowing the incoming upload to replace
          an already existing video
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Videos
      - PrepareUpload
  viddler.videos.setClosedCaptioning:
    post:
      summary: Videos SetClosedCaptioning
      description: Update closed captioning details on a previously uploaded file.
      operationId: videos-setclosedcaptioning
      x-api-path-slug: viddler-videos-setclosedcaptioning-post
      parameters:
      - in: query
        name: closed_captioning_id
      - in: query
        name: default
      - in: query
        name: enabled
      - in: query
        name: language
        description: 'The language of the file (Max Characters: 50)'
      - in: query
        name: sessionid
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Videos
      - SetClosedCaptioning
  viddler.videos.uploadProgress:
    get:
      summary: Videos UploadProgress
      description: Return the status of an upload.
      operationId: videos-uploadprogress
      x-api-path-slug: viddler-videos-uploadprogress-get
      parameters:
      - in: query
        name: sessionid
      - in: query
        name: token
      responses:
        200:
          description: OK
      tags:
      - Viddler
      - Videos
      - UploadProgress