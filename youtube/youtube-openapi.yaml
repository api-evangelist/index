swagger: "2.0"
x-collection-name: YouTube
x-complete: 1
info:
  title: YouTube
  description: youtube-allows-users-to-upload-view-rate-share-add-to-favorites-report-comment-on-videos-and-subscribe-to-other-users--it-offers-a-wide-variety-of-usergenerated-and-corporate-media-videos--available-content-includes-video-clips-tv-show-clips-music-videos-short-and-documentary-films-audio-recordings-movie-trailers-live-streams-and-other-content-such-as-video-blogging-short-original-videos-and-educational-videos--most-of-the-content-on-youtube-is-uploaded-by-individuals-but-media-corporations-including-cbs-the-bbc-vevo-and-hulu-offer-some-of-their-material-via-youtube-as-part-of-the-youtube-partnership-program--unregistered-users-can-only-watch-videos-on-the-site-while-registered-users-are-permitted-to-upload-an-unlimited-number-of-videos-and-add-comments-to-videos-
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: www.googleapis.com
basePath: /youtube/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/jobs:
    get:
      summary: Get Jobs
      description: Lists jobs.
      operationId: getV1Jobs
      x-api-path-slug: v1jobs-get
      parameters:
      - in: query
        name: includeSystemManaged
        description: If set to true, also system-managed jobs will be returned; otherwise
          onlyuser-created jobs will be returned
      - in: query
        name: onBehalfOfContentOwner
        description: The content owners external ID on which behalf the user is acting
          on
      - in: query
        name: pageSize
        description: Requested page size
      - in: query
        name: pageToken
        description: A token identifying a page of results the server should return
      responses:
        200:
          description: OK
      tags:
      - V1
      - Jobs
    post:
      summary: Add Jobs
      description: Creates a job and returns it.
      operationId: postV1Jobs
      x-api-path-slug: v1jobs-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: The content owners external ID on which behalf the user is acting
          on
      responses:
        200:
          description: OK
      tags:
      - V1
      - Jobs
  /v1/jobs/{jobId}:
    delete:
      summary: Delete Jobs Job
      description: Delete v1 jobs job
      operationId: deleteV1JobsJob
      x-api-path-slug: v1jobsjobid-delete
      parameters:
      - in: path
        name: jobId
        description: The ID of the job to delete
      - in: query
        name: onBehalfOfContentOwner
        description: The content owners external ID on which behalf the user is acting
          on
      responses:
        200:
          description: OK
      tags:
      - V1
      - Jobs
      - Job
    get:
      summary: Get Jobs Job
      description: Get v1 jobs job
      operationId: getV1JobsJob
      x-api-path-slug: v1jobsjobid-get
      parameters:
      - in: path
        name: jobId
        description: The ID of the job to retrieve
      - in: query
        name: onBehalfOfContentOwner
        description: The content owners external ID on which behalf the user is acting
          on
      responses:
        200:
          description: OK
      tags:
      - V1
      - Jobs
      - Job
  /v1/jobs/{jobId}/reports:
    get:
      summary: Get Jobs Job Reports
      description: |-
        Lists reports created by a specific job.
        Returns NOT_FOUND if the job does not exist.
      operationId: getV1JobsJobReports
      x-api-path-slug: v1jobsjobidreports-get
      parameters:
      - in: query
        name: createdAfter
        description: If set, only reports created after the specified date/time are
          returned
      - in: path
        name: jobId
        description: The ID of the job
      - in: query
        name: onBehalfOfContentOwner
        description: The content owners external ID on which behalf the user is acting
          on
      - in: query
        name: pageSize
        description: Requested page size
      - in: query
        name: pageToken
        description: A token identifying a page of results the server should return
      - in: query
        name: startTimeAtOrAfter
        description: If set, only reports whose start time is greater than or equal
          thespecified date/time are returned
      - in: query
        name: startTimeBefore
        description: If set, only reports whose start time is smaller than the specifieddate/time
          are returned
      responses:
        200:
          description: OK
      tags:
      - V1
      - Jobs
      - Job
      - Reports
  /v1/jobs/{jobId}/reports/{reportId}:
    get:
      summary: Get Jobs Job Reports Report
      description: Gets the metadata of a specific report.
      operationId: getV1JobsJobReportsReport
      x-api-path-slug: v1jobsjobidreportsreportid-get
      parameters:
      - in: path
        name: jobId
        description: The ID of the job
      - in: query
        name: onBehalfOfContentOwner
        description: The content owners external ID on which behalf the user is acting
          on
      - in: path
        name: reportId
        description: The ID of the report to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Jobs
      - Job
      - Reports
      - Report
  /v1/media/{resourceName}:
    get:
      summary: Get Media Resource Name
      description: |-
        Method for media download. Download is supported
        on the URI `/v1/media/{+name}?alt=media`.
      operationId: getV1MediaResourcename
      x-api-path-slug: v1mediaresourcename-get
      parameters:
      - in: path
        name: resourceName
        description: Name of the media that is being downloaded
      responses:
        200:
          description: OK
      tags:
      - V1
      - Media
      - Resourcename
  /v1/reportTypes:
    get:
      summary: Get Reporttypes
      description: Lists report types.
      operationId: getV1Reporttypes
      x-api-path-slug: v1reporttypes-get
      parameters:
      - in: query
        name: includeSystemManaged
        description: If set to true, also system-managed report types will be returned;otherwise
          only the report types that can be used to create new reportingjobs will
          be returned
      - in: query
        name: onBehalfOfContentOwner
        description: The content owners external ID on which behalf the user is acting
          on
      - in: query
        name: pageSize
        description: Requested page size
      - in: query
        name: pageToken
        description: A token identifying a page of results the server should return
      responses:
        200:
          description: OK
      tags:
      - V1
      - Reporttypes
  /activities:
    get:
      summary: Get Activities
      description: Returns a list of channel activity events that match the request
        criteria. For example, you can retrieve events associated with a particular
        channel, events associated with the user's subscriptions and Google+ friends,
        or the YouTube home page feed, which is customized for each user.
      operationId: getActivities
      x-api-path-slug: activities-get
      parameters:
      - in: query
        name: channelId
        description: The channelId parameter specifies a unique YouTube channel ID
      - in: query
        name: home
        description: Set this parameters value to true to retrieve the activity feed
          that displays on the YouTube home page for the currently authenticated user
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: mine
        description: Set this parameters value to true to retrieve a feed of the authenticated
          users activities
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more activity resource properties that the API response will include
      - in: query
        name: publishedAfter
        description: The publishedAfter parameter specifies the earliest date and
          time that an activity could have occurred for that activity to be included
          in the API response
      - in: query
        name: publishedBefore
        description: The publishedBefore parameter specifies the date and time before
          which an activity must have occurred for that activity to be included in
          the API response
      - in: query
        name: regionCode
        description: The regionCode parameter instructs the API to return results
          for the specified country
      responses:
        200:
          description: OK
      tags:
      - Activities
    post:
      summary: Add Activities
      description: |-
        Posts a bulletin for a specific channel. (The user submitting the request must be authorized to act on the channel's behalf.)

        Note: Even though an activity resource can contain information about actions like a user rating a video or marking a video as a favorite, you need to use other API methods to generate those activity resources. For example, you would use the API's videos.rate() method to rate a video and the playlistItems.insert() method to mark a video as a favorite.
      operationId: postActivities
      x-api-path-slug: activities-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Activities
  /captions:
    delete:
      summary: Delete Captions
      description: Deletes a specified caption track.
      operationId: deleteCaptions
      x-api-path-slug: captions-delete
      parameters:
      - in: query
        name: id
        description: The id parameter identifies the caption track that is being deleted
      - in: query
        name: onBehalfOf
        description: ID of the Google+ Page for the channel that the request is be
          on behalf of
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Captions
    get:
      summary: Get Captions
      description: Returns a list of caption tracks that are associated with a specified
        video. Note that the API response does not contain the actual captions and
        that the captions.download method provides the ability to retrieve a caption
        track.
      operationId: getCaptions
      x-api-path-slug: captions-get
      parameters:
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of IDs that
          identify the caption resources that should be retrieved
      - in: query
        name: onBehalfOf
        description: ID of the Google+ Page for the channel that the request is on
          behalf of
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more caption resource parts that the API response will include
      - in: query
        name: videoId
        description: The videoId parameter specifies the YouTube video ID of the video
          for which the API should return caption tracks
      responses:
        200:
          description: OK
      tags:
      - Captions
    post:
      summary: Add Captions
      description: Uploads a caption track.
      operationId: postCaptions
      x-api-path-slug: captions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOf
        description: ID of the Google+ Page for the channel that the request is be
          on behalf of
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: part
        description: The part parameter specifies the caption resource parts that
          the API response will include
      - in: query
        name: sync
        description: The sync parameter indicates whether YouTube should automatically
          synchronize the caption file with the audio track of the video
      responses:
        200:
          description: OK
      tags:
      - Captions
    put:
      summary: Put Captions
      description: Updates a caption track. When updating a caption track, you can
        change the track's draft status, upload a new caption file for the track,
        or both.
      operationId: putCaptions
      x-api-path-slug: captions-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOf
        description: ID of the Google+ Page for the channel that the request is be
          on behalf of
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      - in: query
        name: sync
        description: 'Note: The API server only processes the parameter value if the
          request contains an updated caption file'
      responses:
        200:
          description: OK
      tags:
      - Captions
  /captions/{id}:
    get:
      summary: Get Captions
      description: Downloads a caption track. The caption track is returned in its
        original format unless the request specifies a value for the tfmt parameter
        and in its original language unless the request specifies a value for the
        tlang parameter.
      operationId: getCaptions
      x-api-path-slug: captionsid-get
      parameters:
      - in: path
        name: id
        description: The id parameter identifies the caption track that is being retrieved
      - in: query
        name: onBehalfOf
        description: ID of the Google+ Page for the channel that the request is be
          on behalf of
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: tfmt
        description: The tfmt parameter specifies that the caption track should be
          returned in a specific format
      - in: query
        name: tlang
        description: The tlang parameter specifies that the API response should return
          a translation of the specified caption track
      responses:
        200:
          description: OK
      tags:
      - Captions
  /channelBanners/insert:
    post:
      summary: Add Channel Banners Insert
      description: |-
        Uploads a channel banner image to YouTube. This method represents the first two steps in a three-step process to update the banner image for a channel:

        - Call the channelBanners.insert method to upload the binary image data to YouTube. The image must have a 16:9 aspect ratio and be at least 2120x1192 pixels.
        - Extract the url property's value from the response that the API returns for step 1.
        - Call the channels.update method to update the channel's branding settings. Set the brandingSettings.image.bannerExternalUrl property's value to the URL obtained in step 2.
      operationId: postChannelbannersInsert
      x-api-path-slug: channelbannersinsert-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: channelId
        description: The channelId parameter identifies the YouTube channel to which
          the banner is uploaded
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Channelbanners
      - Insert
  /channelSections:
    delete:
      summary: Delete Channel Sections
      description: Deletes a channelSection.
      operationId: deleteChannelsections
      x-api-path-slug: channelsections-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube channelSection ID for
          the resource that is being deleted
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Channelsections
    get:
      summary: Get Channel Sections
      description: Returns channelSection resources that match the API request criteria.
      operationId: getChannelsections
      x-api-path-slug: channelsections-get
      parameters:
      - in: query
        name: channelId
        description: The channelId parameter specifies a YouTube channel ID
      - in: query
        name: hl
        description: The hl parameter indicates that the snippet
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of the YouTube
          channelSection ID(s) for the resource(s) that are being retrieved
      - in: query
        name: mine
        description: Set this parameters value to true to retrieve a feed of the authenticated
          users channelSections
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more channelSection resource properties that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Channelsections
    post:
      summary: Add Channel Sections
      description: Adds a channelSection for the authenticated user's channel.
      operationId: postChannelsections
      x-api-path-slug: channelsections-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Channelsections
    put:
      summary: Put Channel Sections
      description: Update a channelSection.
      operationId: putChannelsections
      x-api-path-slug: channelsections-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Channelsections
  /channels:
    get:
      summary: Get Channels
      description: Returns a collection of zero or more channel resources that match
        the request criteria.
      operationId: getChannels
      x-api-path-slug: channels-get
      parameters:
      - in: query
        name: categoryId
        description: The categoryId parameter specifies a YouTube guide category,
          thereby requesting YouTube channels associated with that category
      - in: query
        name: forUsername
        description: The forUsername parameter specifies a YouTube username, thereby
          requesting the channel associated with that username
      - in: query
        name: hl
        description: The hl parameter should be used for filter out the properties
          that are not in the given language
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of the YouTube
          channel ID(s) for the resource(s) that are being retrieved
      - in: query
        name: managedByMe
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: mine
        description: Set this parameters value to true to instruct the API to only
          return channels owned by the authenticated user
      - in: query
        name: mySubscribers
        description: Use the subscriptions
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more channel resource properties that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Channels
    put:
      summary: Put Channels
      description: Updates a channel's metadata. Note that this method currently only
        supports updates to the channel resource's brandingSettings and invideoPromotion
        objects and their child properties.
      operationId: putChannels
      x-api-path-slug: channels-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: The onBehalfOfContentOwner parameter indicates that the authenticated
          user is acting on behalf of the content owner specified in the parameter
          value
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Channels
  /commentThreads:
    get:
      summary: Get Comment Threads
      description: Returns a list of comment threads that match the API request parameters.
      operationId: getCommentthreads
      x-api-path-slug: commentthreads-get
      parameters:
      - in: query
        name: allThreadsRelatedToChannelId
        description: The allThreadsRelatedToChannelId parameter instructs the API
          to return all comment threads associated with the specified channel
      - in: query
        name: channelId
        description: The channelId parameter instructs the API to return comment threads
          containing comments about the specified channel
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of comment
          thread IDs for the resources that should be retrieved
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: moderationStatus
        description: Set this parameter to limit the returned comment threads to a
          particular moderation state
      - in: query
        name: order
        description: The order parameter specifies the order in which the API response
          should list comment threads
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more commentThread resource properties that the API response will include
      - in: query
        name: searchTerms
        description: The searchTerms parameter instructs the API to limit the API
          response to only contain comments that contain the specified search terms
      - in: query
        name: textFormat
        description: Set this parameters value to html or plainText to instruct the
          API to return the comments left by users in html formatted or in plain text
      - in: query
        name: videoId
        description: The videoId parameter instructs the API to return comment threads
          associated with the specified video ID
      responses:
        200:
          description: OK
      tags:
      - Commentthreads
    post:
      summary: Add Comment Threads
      description: Creates a new top-level comment. To add a reply to an existing
        comment, use the comments.insert method instead.
      operationId: postCommentthreads
      x-api-path-slug: commentthreads-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: part
        description: The part parameter identifies the properties that the API response
          will include
      responses:
        200:
          description: OK
      tags:
      - Commentthreads
    put:
      summary: Put Comment Threads
      description: Modifies the top-level comment in a comment thread.
      operationId: putCommentthreads
      x-api-path-slug: commentthreads-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of commentThread
          resource properties that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Commentthreads
  /comments:
    delete:
      summary: Delete Comments
      description: Deletes a comment.
      operationId: deleteComments
      x-api-path-slug: comments-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the comment ID for the resource that
          is being deleted
      responses:
        200:
          description: OK
      tags:
      - Comments
    get:
      summary: Get Comments
      description: Returns a list of comments that match the API request parameters.
      operationId: getComments
      x-api-path-slug: comments-get
      parameters:
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of comment
          IDs for the resources that are being retrieved
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: parentId
        description: The parentId parameter specifies the ID of the comment for which
          replies should be retrieved
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more comment resource properties that the API response will include
      - in: query
        name: textFormat
        description: This parameter indicates whether the API should return comments
          formatted as HTML or as plain text
      responses:
        200:
          description: OK
      tags:
      - Comments
    post:
      summary: Add Comments
      description: 'Creates a reply to an existing comment. Note: To create a top-level
        comment, use the commentThreads.insert method.'
      operationId: postComments
      x-api-path-slug: comments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: part
        description: The part parameter identifies the properties that the API response
          will include
      responses:
        200:
          description: OK
      tags:
      - Comments
    put:
      summary: Put Comments
      description: Modifies a comment.
      operationId: putComments
      x-api-path-slug: comments-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: part
        description: The part parameter identifies the properties that the API response
          will include
      responses:
        200:
          description: OK
      tags:
      - Comments
  /comments/markAsSpam:
    post:
      summary: Add Comments Mark as SPAM
      description: Expresses the caller's opinion that one or more comments should
        be flagged as spam.
      operationId: postCommentsMarkasspam
      x-api-path-slug: commentsmarkasspam-post
      parameters:
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of IDs of comments
          that the caller believes should be classified as spam
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Markasspam
  /comments/setModerationStatus:
    post:
      summary: Add Comments Set Moderation Status
      description: Sets the moderation status of one or more comments. The API request
        must be authorized by the owner of the channel or video associated with the
        comments.
      operationId: postCommentsSetmoderationstatus
      x-api-path-slug: commentssetmoderationstatus-post
      parameters:
      - in: query
        name: banAuthor
        description: The banAuthor parameter lets you indicate that you want to automatically
          reject any additional comments written by the comments author
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of IDs that
          identify the comments for which you are updating the moderation status
      - in: query
        name: moderationStatus
        description: Identifies the new moderation status of the specified comments
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Setmoderationstatus
  /fanFundingEvents:
    get:
      summary: Get Fanfundingevents
      description: Lists fan funding events for a channel.
      operationId: getFanfundingevents
      x-api-path-slug: fanfundingevents-get
      parameters:
      - in: query
        name: hl
        description: The hl parameter instructs the API to retrieve localized resource
          metadata for a specific application language that the YouTube website supports
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies the fanFundingEvent resource parts
          that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Fanfundingevents
  /guideCategories:
    get:
      summary: Get Guecategories
      description: Returns a list of categories that can be associated with YouTube
        channels.
      operationId: getGuecategories
      x-api-path-slug: guidecategories-get
      parameters:
      - in: query
        name: hl
        description: The hl parameter specifies the language that will be used for
          text values in the API response
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of the YouTube
          channel category ID(s) for the resource(s) that are being retrieved
      - in: query
        name: part
        description: The part parameter specifies the guideCategory resource properties
          that the API response will include
      - in: query
        name: regionCode
        description: The regionCode parameter instructs the API to return the list
          of guide categories available in the specified country
      responses:
        200:
          description: OK
      tags:
      - Guecategories
  /i18nLanguages:
    get:
      summary: Get Languages
      description: Returns a list of application languages that the YouTube website
        supports.
      operationId: getI18nlanguages
      x-api-path-slug: i18nlanguages-get
      parameters:
      - in: query
        name: hl
        description: The hl parameter specifies the language that should be used for
          text values in the API response
      - in: query
        name: part
        description: The part parameter specifies the i18nLanguage resource properties
          that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Languages
  /i18nRegions:
    get:
      summary: Get Regions
      description: Returns a list of content regions that the YouTube website supports.
      operationId: getI18nregions
      x-api-path-slug: i18nregions-get
      parameters:
      - in: query
        name: hl
        description: The hl parameter specifies the language that should be used for
          text values in the API response
      - in: query
        name: part
        description: The part parameter specifies the i18nRegion resource properties
          that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Regions
  /liveBroadcasts:
    delete:
      summary: Delete Live Broadcasts
      description: Delete livebroadcasts
      operationId: deleteLivebroadcasts
      x-api-path-slug: livebroadcasts-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube live broadcast ID for
          the resource that is being deleted
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      responses:
        200:
          description: OK
      tags:
      - Livebroadcasts
    get:
      summary: Get Live Broadcasts
      description: Returns a list of YouTube broadcasts that match the API request
        parameters.
      operationId: getLivebroadcasts
      x-api-path-slug: livebroadcasts-get
      parameters:
      - in: query
        name: broadcastStatus
        description: The broadcastStatus parameter filters the API response to only
          include broadcasts with the specified status
      - in: query
        name: broadcastType
        description: The broadcastType parameter filters the API response to only
          include broadcasts with the specified type
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of YouTube
          broadcast IDs that identify the broadcasts being retrieved
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: mine
        description: The mine parameter can be used to instruct the API to only return
          broadcasts owned by the authenticated user
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more liveBroadcast resource properties that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Livebroadcasts
    post:
      summary: Add Live Broadcasts
      description: Creates a broadcast.
      operationId: postLivebroadcasts
      x-api-path-slug: livebroadcasts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Livebroadcasts
    put:
      summary: Put Live Broadcasts
      description: Updates a broadcast. For example, you could modify the broadcast
        settings defined in the liveBroadcast resource's contentDetails object.
      operationId: putLivebroadcasts
      x-api-path-slug: livebroadcasts-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Livebroadcasts
  /liveBroadcasts/bind:
    post:
      summary: Add Live Broadcasts Bind
      description: Binds a YouTube broadcast to a stream or removes an existing binding
        between a broadcast and a stream. A broadcast can only be bound to one video
        stream, though a video stream may be bound to more than one broadcast.
      operationId: postLivebroadcastsBind
      x-api-path-slug: livebroadcastsbind-post
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the unique ID of the broadcast that
          is being bound to a video stream
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more liveBroadcast resource properties that the API response will include
      - in: query
        name: streamId
        description: The streamId parameter specifies the unique ID of the video stream
          that is being bound to a broadcast
      responses:
        200:
          description: OK
      tags:
      - Livebroadcasts
      - Bind
  /liveBroadcasts/control:
    post:
      summary: Add Live Broadcasts Control
      description: Controls the settings for a slate that can be displayed in the
        broadcast stream.
      operationId: postLivebroadcastsControl
      x-api-path-slug: livebroadcastscontrol-post
      parameters:
      - in: query
        name: displaySlate
        description: The displaySlate parameter specifies whether the slate is being
          enabled or disabled
      - in: query
        name: id
        description: The id parameter specifies the YouTube live broadcast ID that
          uniquely identifies the broadcast in which the slate is being updated
      - in: query
        name: offsetTimeMs
        description: The offsetTimeMs parameter specifies a positive time offset when
          the specified slate change will occur
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more liveBroadcast resource properties that the API response will include
      - in: query
        name: walltime
        description: The walltime parameter specifies the wall clock time at which
          the specified slate change will occur
      responses:
        200:
          description: OK
      tags:
      - Livebroadcasts
      - Control
  /liveBroadcasts/transition:
    post:
      summary: Add Live Broadcasts Transition
      description: Changes the status of a YouTube live broadcast and initiates any
        processes associated with the new status. For example, when you transition
        a broadcast's status to testing, YouTube starts to transmit video to that
        broadcast's monitor stream. Before calling this method, you should confirm
        that the value of the status.streamStatus property for the stream bound to
        your broadcast is active.
      operationId: postLivebroadcastsTransition
      x-api-path-slug: livebroadcaststransition-post
      parameters:
      - in: query
        name: broadcastStatus
        description: The broadcastStatus parameter identifies the state to which the
          broadcast is changing
      - in: query
        name: id
        description: The id parameter specifies the unique ID of the broadcast that
          is transitioning to another status
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more liveBroadcast resource properties that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Livebroadcasts
      - Transition
  /liveChat/bans:
    delete:
      summary: Delete Live Chat Bans
      description: Delete livechat bans
      operationId: deleteLivechatBans
      x-api-path-slug: livechatbans-delete
      parameters:
      - in: query
        name: id
        description: The id parameter identifies the chat ban to remove
      responses:
        200:
          description: OK
      tags:
      - Chat
      - Bans
    post:
      summary: Add Live Chat Bans
      description: Adds a new ban to the chat.
      operationId: postLivechatBans
      x-api-path-slug: livechatbans-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Chat
      - Bans
  /liveChat/messages:
    delete:
      summary: Delete Live Chat Messages
      description: Delete livechat messages
      operationId: deleteLivechatMessages
      x-api-path-slug: livechatmessages-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube chat message ID of the
          resource that is being deleted
      responses:
        200:
          description: OK
      tags:
      - Chat
      - Messages
    get:
      summary: Get Live Chat Messages
      description: Lists live chat messages for a specific chat.
      operationId: getLivechatMessages
      x-api-path-slug: livechatmessages-get
      parameters:
      - in: query
        name: hl
        description: The hl parameter instructs the API to retrieve localized resource
          metadata for a specific application language that the YouTube website supports
      - in: query
        name: liveChatId
        description: The liveChatId parameter specifies the ID of the chat whose messages
          will be returned
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of messages
          that should be returned in the result set
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies the liveChatComment resource parts
          that the API response will include
      - in: query
        name: profileImageSize
        description: The profileImageSize parameter specifies the size of the user
          profile pictures that should be returned in the result set
      responses:
        200:
          description: OK
      tags:
      - Chat
      - Messages
    post:
      summary: Add Live Chat Messages
      description: Adds a message to a live chat.
      operationId: postLivechatMessages
      x-api-path-slug: livechatmessages-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: part
        description: The part parameter serves two purposes
      responses:
        200:
          description: OK
      tags:
      - Chat
      - Messages
  /liveChat/moderators:
    delete:
      summary: Delete Live Chat Moderators
      description: Delete livechat moderators
      operationId: deleteLivechatModerators
      x-api-path-slug: livechatmoderators-delete
      parameters:
      - in: query
        name: id
        description: The id parameter identifies the chat moderator to remove
      responses:
        200:
          description: OK
      tags:
      - Chat
      - Moderators
    get:
      summary: Get Live Chat Moderators
      description: Lists moderators for a live chat.
      operationId: getLivechatModerators
      x-api-path-slug: livechatmoderators-get
      parameters:
      - in: query
        name: liveChatId
        description: The liveChatId parameter specifies the YouTube live chat for
          which the API should return moderators
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies the liveChatModerator resource parts
          that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Chat
      - Moderators
    post:
      summary: Add Live Chat Moderators
      description: Adds a new moderator for the chat.
      operationId: postLivechatModerators
      x-api-path-slug: livechatmoderators-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Chat
      - Moderators
  /liveStreams:
    delete:
      summary: Delete Livestreams
      description: Deletes a video stream.
      operationId: deleteLivestreams
      x-api-path-slug: livestreams-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube live stream ID for the
          resource that is being deleted
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      responses:
        200:
          description: OK
      tags:
      - Livestreams
    get:
      summary: Get Livestreams
      description: Returns a list of video streams that match the API request parameters.
      operationId: getLivestreams
      x-api-path-slug: livestreams-get
      parameters:
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of YouTube
          stream IDs that identify the streams being retrieved
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: mine
        description: The mine parameter can be used to instruct the API to only return
          streams owned by the authenticated user
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more liveStream resource properties that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Livestreams
    post:
      summary: Add Livestreams
      description: Creates a video stream. The stream enables you to send your video
        to YouTube, which can then broadcast the video to your audience.
      operationId: postLivestreams
      x-api-path-slug: livestreams-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Livestreams
    put:
      summary: Put Livestreams
      description: Updates a video stream. If the properties that you want to change
        cannot be updated, then you need to create a new stream with the proper settings.
      operationId: putLivestreams
      x-api-path-slug: livestreams-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Livestreams
  /playlistItems:
    delete:
      summary: Delete Play List Items
      description: Deletes a playlist item.
      operationId: deletePlaylistitems
      x-api-path-slug: playlistitems-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube playlist item ID for the
          playlist item that is being deleted
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Playlistitems
    get:
      summary: Get Play List Items
      description: Returns a collection of playlist items that match the API request
        parameters. You can retrieve all of the playlist items in a specified playlist
        or retrieve one or more playlist items by their unique IDs.
      operationId: getPlaylistitems
      x-api-path-slug: playlistitems-get
      parameters:
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of one or more
          unique playlist item IDs
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more playlistItem resource properties that the API response will include
      - in: query
        name: playlistId
        description: The playlistId parameter specifies the unique ID of the playlist
          for which you want to retrieve playlist items
      - in: query
        name: videoId
        description: The videoId parameter specifies that the request should return
          only the playlist items that contain the specified video
      responses:
        200:
          description: OK
      tags:
      - Playlistitems
    post:
      summary: Add Play List Items
      description: Adds a resource to a playlist.
      operationId: postPlaylistitems
      x-api-path-slug: playlistitems-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Playlistitems
    put:
      summary: Put Play List Items
      description: Modifies a playlist item. For example, you could update the item's
        position in the playlist.
      operationId: putPlaylistitems
      x-api-path-slug: playlistitems-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Playlistitems
  /playlists:
    delete:
      summary: Delete Playlists
      description: Deletes a playlist.
      operationId: deletePlaylists
      x-api-path-slug: playlists-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube playlist ID for the playlist
          that is being deleted
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Playlists
    get:
      summary: Get Playlists
      description: Returns a collection of playlists that match the API request parameters.
        For example, you can retrieve all playlists that the authenticated user owns,
        or you can retrieve one or more playlists by their unique IDs.
      operationId: getPlaylists
      x-api-path-slug: playlists-get
      parameters:
      - in: query
        name: channelId
        description: This value indicates that the API should only return the specified
          channels playlists
      - in: query
        name: hl
        description: The hl parameter should be used for filter out the properties
          that are not in the given language
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of the YouTube
          playlist ID(s) for the resource(s) that are being retrieved
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: mine
        description: Set this parameters value to true to instruct the API to only
          return playlists owned by the authenticated user
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more playlist resource properties that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Playlists
    post:
      summary: Add Playlists
      description: Creates a playlist.
      operationId: postPlaylists
      x-api-path-slug: playlists-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Playlists
    put:
      summary: Put Playlists
      description: Modifies a playlist. For example, you could change a playlist's
        title, description, or privacy status.
      operationId: putPlaylists
      x-api-path-slug: playlists-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Playlists
  /search:
    get:
      summary: Get Search
      description: Returns a collection of search results that match the query parameters
        specified in the API request. By default, a search result set identifies matching
        video, channel, and playlist resources, but you can also configure queries
        to only retrieve a specific type of resource.
      operationId: getSearch
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: channelId
        description: The channelId parameter indicates that the API response should
          only contain resources created by the channel
      - in: query
        name: channelType
        description: The channelType parameter lets you restrict a search to a particular
          type of channel
      - in: query
        name: eventType
        description: The eventType parameter restricts a search to broadcast events
      - in: query
        name: forContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: forDeveloper
        description: The forDeveloper parameter restricts the search to only retrieve
          videos uploaded via the developers application or website
      - in: query
        name: forMine
        description: The forMine parameter restricts the search to only retrieve videos
          owned by the authenticated user
      - in: query
        name: location
        description: The location parameter, in conjunction with the locationRadius
          parameter, defines a circular geographic area and also restricts a search
          to videos that specify, in their metadata, a geographic location that falls
          within that area
      - in: query
        name: locationRadius
        description: The locationRadius parameter, in conjunction with the location
          parameter, defines a circular geographic area
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: order
        description: The order parameter specifies the method that will be used to
          order resources in the API response
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more search resource properties that the API response will include
      - in: query
        name: publishedAfter
        description: The publishedAfter parameter indicates that the API response
          should only contain resources created after the specified time
      - in: query
        name: publishedBefore
        description: The publishedBefore parameter indicates that the API response
          should only contain resources created before the specified time
      - in: query
        name: q
        description: The q parameter specifies the query term to search for
      - in: query
        name: regionCode
        description: The regionCode parameter instructs the API to return search results
          for the specified country
      - in: query
        name: relatedToVideoId
        description: The relatedToVideoId parameter retrieves a list of videos that
          are related to the video that the parameter value identifies
      - in: query
        name: relevanceLanguage
        description: The relevanceLanguage parameter instructs the API to return search
          results that are most relevant to the specified language
      - in: query
        name: safeSearch
        description: The safeSearch parameter indicates whether the search results
          should include restricted content as well as standard content
      - in: query
        name: topicId
        description: The topicId parameter indicates that the API response should
          only contain resources associated with the specified topic
      - in: query
        name: type
        description: The type parameter restricts a search query to only retrieve
          a particular type of resource
      - in: query
        name: videoCaption
        description: The videoCaption parameter indicates whether the API should filter
          video search results based on whether they have captions
      - in: query
        name: videoCategoryId
        description: The videoCategoryId parameter filters video search results based
          on their category
      - in: query
        name: videoDefinition
        description: The videoDefinition parameter lets you restrict a search to only
          include either high definition (HD) or standard definition (SD) videos
      - in: query
        name: videoDimension
        description: The videoDimension parameter lets you restrict a search to only
          retrieve 2D or 3D videos
      - in: query
        name: videoDuration
        description: The videoDuration parameter filters video search results based
          on their duration
      - in: query
        name: videoEmbeddable
        description: The videoEmbeddable parameter lets you to restrict a search to
          only videos that can be embedded into a webpage
      - in: query
        name: videoLicense
        description: The videoLicense parameter filters search results to only include
          videos with a particular license
      - in: query
        name: videoSyndicated
        description: The videoSyndicated parameter lets you to restrict a search to
          only videos that can be played outside youtube
      - in: query
        name: videoType
        description: The videoType parameter lets you restrict a search to a particular
          type of videos
      responses:
        200:
          description: OK
      tags:
      - Search
  /sponsors:
    get:
      summary: Get Sponsors
      description: Lists sponsors for a channel.
      operationId: getSponsors
      x-api-path-slug: sponsors-get
      parameters:
      - in: query
        name: filter
        description: The filter parameter specifies which channel sponsors to return
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies the sponsor resource parts that
          the API response will include
      responses:
        200:
          description: OK
      tags:
      - Sponsors
  /subscriptions:
    delete:
      summary: Delete Subscriptions
      description: Deletes a subscription.
      operationId: deleteSubscriptions
      x-api-path-slug: subscriptions-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube subscription ID for the
          resource that is being deleted
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
    get:
      summary: Get Subscriptions
      description: Returns subscription resources that match the API request criteria.
      operationId: getSubscriptions
      x-api-path-slug: subscriptions-get
      parameters:
      - in: query
        name: channelId
        description: The channelId parameter specifies a YouTube channel ID
      - in: query
        name: forChannelId
        description: The forChannelId parameter specifies a comma-separated list of
          channel IDs
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of the YouTube
          subscription ID(s) for the resource(s) that are being retrieved
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: mine
        description: Set this parameters value to true to retrieve a feed of the authenticated
          users subscriptions
      - in: query
        name: myRecentSubscribers
        description: Set this parameters value to true to retrieve a feed of the subscribers
          of the authenticated user in reverse chronological order (newest first)
      - in: query
        name: mySubscribers
        description: Set this parameters value to true to retrieve a feed of the subscribers
          of the authenticated user in no particular order
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: order
        description: The order parameter specifies the method that will be used to
          sort resources in the API response
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more subscription resource properties that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
    post:
      summary: Add Subscriptions
      description: Adds a subscription for the authenticated user's channel.
      operationId: postSubscriptions
      x-api-path-slug: subscriptions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /superChatEvents:
    get:
      summary: Get Superchatevents
      description: Lists Super Chat events for a channel.
      operationId: getSuperchatevents
      x-api-path-slug: superchatevents-get
      parameters:
      - in: query
        name: hl
        description: The hl parameter instructs the API to retrieve localized resource
          metadata for a specific application language that the YouTube website supports
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies the superChatEvent resource parts
          that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Chat
  /thumbnails/set:
    post:
      summary: Add Thumbnails Set
      description: Uploads a custom video thumbnail to YouTube and sets it for a video.
      operationId: postThumbnailsSet
      x-api-path-slug: thumbnailsset-post
      parameters:
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: videoId
        description: The videoId parameter specifies a YouTube video ID for which
          the custom video thumbnail is being provided
      responses:
        200:
          description: OK
      tags:
      - Thumbnails
      - Set
  /videoAbuseReportReasons:
    get:
      summary: Get Video Abuse Report Reasons
      description: Returns a list of abuse reasons that can be used for reporting
        abusive videos.
      operationId: getVeoabusereportreasons
      x-api-path-slug: videoabusereportreasons-get
      parameters:
      - in: query
        name: hl
        description: The hl parameter specifies the language that should be used for
          text values in the API response
      - in: query
        name: part
        description: The part parameter specifies the videoCategory resource parts
          that the API response will include
      responses:
        200:
          description: OK
      tags:
      - Veoabusereportreasons
  /videoCategories:
    get:
      summary: Get Veocategories
      description: Returns a list of categories that can be associated with YouTube
        videos.
      operationId: getVeocategories
      x-api-path-slug: videocategories-get
      parameters:
      - in: query
        name: hl
        description: The hl parameter specifies the language that should be used for
          text values in the API response
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of video category
          IDs for the resources that you are retrieving
      - in: query
        name: part
        description: The part parameter specifies the videoCategory resource properties
          that the API response will include
      - in: query
        name: regionCode
        description: The regionCode parameter instructs the API to return the list
          of video categories available in the specified country
      responses:
        200:
          description: OK
      tags:
      - Veocategories
  /videos:
    delete:
      summary: Delete Videos
      description: Deletes a YouTube video.
      operationId: deleteVeos
      x-api-path-slug: videos-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube video ID for the resource
          that is being deleted
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Veos
    get:
      summary: Get Videos
      description: Returns a list of videos that match the API request parameters.
      operationId: getVeos
      x-api-path-slug: videos-get
      parameters:
      - in: query
        name: chart
        description: The chart parameter identifies the chart that you want to retrieve
      - in: query
        name: hl
        description: The hl parameter instructs the API to retrieve localized resource
          metadata for a specific application language that the YouTube website supports
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of the YouTube
          video ID(s) for the resource(s) that are being retrieved
      - in: query
        name: locale
        description: DEPRECATED
      - in: query
        name: maxHeight
        description: The maxHeight parameter specifies a maximum height of the embedded
          player
      - in: query
        name: maxResults
        description: The maxResults parameter specifies the maximum number of items
          that should be returned in the result set
      - in: query
        name: maxWidth
        description: The maxWidth parameter specifies a maximum width of the embedded
          player
      - in: query
        name: myRating
        description: Set this parameters value to like or dislike to instruct the
          API to only return videos liked or disliked by the authenticated user
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      - in: query
        name: part
        description: The part parameter specifies a comma-separated list of one or
          more video resource properties that the API response will include
      - in: query
        name: regionCode
        description: The regionCode parameter instructs the API to select a video
          chart available in the specified region
      - in: query
        name: videoCategoryId
        description: The videoCategoryId parameter identifies the video category for
          which the chart should be retrieved
      responses:
        200:
          description: OK
      tags:
      - Veos
    post:
      summary: Add Videos
      description: Uploads a video to YouTube and optionally sets the video's metadata.
      operationId: postVeos
      x-api-path-slug: videos-post
      parameters:
      - in: query
        name: autoLevels
        description: The autoLevels parameter indicates whether YouTube should automatically
          enhance the videos lighting and color
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: notifySubscribers
        description: The notifySubscribers parameter indicates whether YouTube should
          send a notification about the new video to users who subscribe to the videos
          channel
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: onBehalfOfContentOwnerChannel
        description: This parameter can only be used in a properly authorized request
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      - in: query
        name: stabilize
        description: The stabilize parameter indicates whether YouTube should adjust
          the video to remove shaky camera motions
      responses:
        200:
          description: OK
      tags:
      - Veos
    put:
      summary: Put Videos
      description: Updates a video's metadata.
      operationId: putVeos
      x-api-path-slug: videos-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: part
        description: The part parameter serves two purposes in this operation
      responses:
        200:
          description: OK
      tags:
      - Veos
  /videos/getRating:
    get:
      summary: Get Videos Get Rating
      description: Retrieves the ratings that the authorized user gave to a list of
        specified videos.
      operationId: getVeosGetrating
      x-api-path-slug: videosgetrating-get
      parameters:
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of the YouTube
          video ID(s) for the resource(s) for which you are retrieving rating data
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Veos
      - Getrating
  /videos/rate:
    post:
      summary: Add Videos Rate
      description: Add a like or dislike rating to a video or remove a rating from
        a video.
      operationId: postVeosRate
      x-api-path-slug: videosrate-post
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube video ID of the video
          that is being rated or having its rating removed
      - in: query
        name: rating
        description: Specifies the rating to record
      responses:
        200:
          description: OK
      tags:
      - Veos
      - Rate
  /videos/reportAbuse:
    post:
      summary: Add Videos Report Abuse
      description: Report abuse for a video.
      operationId: postVeosReportabuse
      x-api-path-slug: videosreportabuse-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Veos
      - Reportabuse
  /watermarks/set:
    post:
      summary: Add Watermarks Set
      description: Uploads a watermark image to YouTube and sets it for a channel.
      operationId: postWatermarksSet
      x-api-path-slug: watermarksset-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: channelId
        description: The channelId parameter specifies the YouTube channel ID for
          which the watermark is being provided
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Watermarks
      - Set
  /watermarks/unset:
    post:
      summary: Add Watermarks Unset
      description: Deletes a channel's watermark image.
      operationId: postWatermarksUnset
      x-api-path-slug: watermarksunset-post
      parameters:
      - in: query
        name: channelId
        description: The channelId parameter specifies the YouTube channel ID for
          which the watermark is being unset
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Watermarks
      - Unset
  /groupItems:
    delete:
      summary: Delete Groupitems
      description: Removes an item from a group.
      operationId: deleteGroupitems
      x-api-path-slug: groupitems-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube group item ID for the
          group that is being deleted
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Groupitems
    get:
      summary: Get Groupitems
      description: Returns a collection of group items that match the API request
        parameters.
      operationId: getGroupitems
      x-api-path-slug: groupitems-get
      parameters:
      - in: query
        name: groupId
        description: The id parameter specifies the unique ID of the group for which
          you want to retrieve group items
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Groupitems
    post:
      summary: Add Groupitems
      description: Creates a group item.
      operationId: postGroupitems
      x-api-path-slug: groupitems-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Groupitems
  /groups:
    delete:
      summary: Delete Groups
      description: Deletes a group.
      operationId: deleteGroups
      x-api-path-slug: groups-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube group ID for the group
          that is being deleted
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Groups
    get:
      summary: Get Groups
      description: Returns a collection of groups that match the API request parameters.
        For example, you can retrieve all groups that the authenticated user owns,
        or you can retrieve one or more groups by their unique IDs.
      operationId: getGroups
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of the YouTube
          group ID(s) for the resource(s) that are being retrieved
      - in: query
        name: mine
        description: Set this parameters value to true to instruct the API to only
          return groups owned by the authenticated user
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      responses:
        200:
          description: OK
      tags:
      - Groups
    post:
      summary: Add Groups
      description: Creates a group.
      operationId: postGroups
      x-api-path-slug: groups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Groups
    put:
      summary: Put Groups
      description: Modifies a group. For example, you could change a group's title.
      operationId: putGroups
      x-api-path-slug: groups-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Groups
  /reports:
    get:
      summary: Get Reports
      description: Retrieve your YouTube Analytics reports.
      operationId: getReports
      x-api-path-slug: reports-get
      parameters:
      - in: query
        name: currency
        description: The currency to which financial metrics should be converted
      - in: query
        name: dimensions
        description: A comma-separated list of YouTube Analytics dimensions, such
          as views or ageGroup,gender
      - in: query
        name: end-date
        description: The end date for fetching YouTube Analytics data
      - in: query
        name: filters
        description: A list of filters that should be applied when retrieving YouTube
          Analytics data
      - in: query
        name: ids
        description: Identifies the YouTube channel or content owner for which you
          are retrieving YouTube Analytics data
      - in: query
        name: include-historical-channel-data
        description: If set to true historical data (i
      - in: query
        name: max-results
        description: The maximum number of rows to include in the response
      - in: query
        name: metrics
        description: A comma-separated list of YouTube Analytics metrics, such as
          views or likes,dislikes
      - in: query
        name: sort
        description: A comma-separated list of dimensions or metrics that determine
          the sort order for YouTube Analytics data
      - in: query
        name: start-date
        description: The start date for fetching YouTube Analytics data
      - in: query
        name: start-index
        description: An index of the first entity to retrieve
      responses:
        200:
          description: OK
      tags:
      - Reports