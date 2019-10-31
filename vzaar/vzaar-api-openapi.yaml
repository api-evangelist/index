swagger: "2.0"
x-collection-name: Vzaar
x-complete: 1
info:
  title: VZaar API
  description: vzaar-is-an-online-video-hosting-service-with-fantastic-features-that-are-designed-for-business--deliver-to-mobile-or-the-web-straight-from-your-site-
  termsOfService: http://vzaar.com/policies
  version: v1
host: vzaar.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accounts/{account}.{format}:
    get:
      summary: Get Api Accounts Account
      description: 'nnThis API call returns the details and rights for each vzaar
        subscription account type along with its relevant metadata. This will show
        the details of the packages available here: http://vzaar.com/pricingnn'
      operationId: getApiAccountsAccount.Format
      x-api-path-slug: apiaccountsaccount-format-get
      parameters:
      - in: query
        name: account is the vzaar account type. This is an integer.
      responses:
        200:
          description: OK
      tags:
      - Api
      - Accounts
      - Account
      - Format
  /api/upload/link.xmln:
    post:
      summary: Post Api Upload Link.xmln
      description: nnThis API call allows a user to upload &amp; process video file
        from given url.nn
      operationId: postApiUploadLink.xmln
      x-api-path-slug: apiuploadlink-xmln-post
      parameters:
      - in: query
        name: bitrate
        description: Specifies videos bitrate
      - in: query
        name: description
        description: Specifies the description for the video
      - in: query
        name: encoding_params
        description: Includes optional parameters
      - in: query
        name: guid
        description: Specifies the guid to operate on
      - in: query
        name: key
        description: A name for the S3 object that stores the uploaded file
      - in: query
        name: size_id
        description: Specifies the size for the video to be encoded in
      - in: query
        name: title
        description: Specifies the title for the video
      - in: query
        name: transcoding
        description: True forces vzaar to transcode the video, false makes vzaar use
          the original source file
      - in: query
        name: url
        description: Specifies the url to video file
      - in: query
        name: width
        description: Specifies videos width
      - in: query
        name: XML/JSON
      responses:
        200:
          description: OK
      tags:
      - Api
      - Upload
      - Link
      - Xmln
  /api/users/{username}.{format}:
    get:
      summary: Get Api Users Username
      description: nnThis API call returns the users public details along with its
        relevant metadata.nn
      operationId: getApiUsersUsername.Format
      x-api-path-slug: apiusersusername-format-get
      parameters:
      - in: query
        name: 'username is the vzaar login name for the user. Note: This must be the
          actual username and not the email address'
      responses:
        200:
          description: OK
      tags:
      - Api
      - Users
      - Username
      - Format
  /api/videos:
    post:
      summary: Post Api Videos
      description: nnThis API call tells the vzaar system to process a newly uploaded
        video. This will encode it if necessary and then provide a vzaar video idea
        back.nn
      operationId: postApiVeos
      x-api-path-slug: apivideos-post
      parameters:
      - in: query
        name: description
        description: Specifies the description for the video
      - in: query
        name: guid
        description: Specifies the guid to operate on
      - in: query
        name: labels
        description: Comma separated list of labels to be assigned to the video
      - in: query
        name: profile
        description: Specifies the size for the video to be encoded in
      - in: query
        name: replace_id
        description: Specifies the video ID of an existing video that you wish to
          replace with the new video
      - in: query
        name: title
        description: Specifies the title for the video
      - in: query
        name: transcoding
        description: True forces vzaar to transcode the video, false makes vzaar use
          the original source file (available only for mp4 and flv files)
      responses:
        200:
          description: OK
      tags:
      - Api
      - Videos
  /api/videos/signature:
    get:
      summary: Get Api Videos Signature
      description: nnThis API call allows a user to request a GUID and an AWS S3 signature.
        With these credentials the user will then be able upload a file into vzaar
        video storage area.nnThe response for this must be parsed and used in the
        Upload step. The upload will fail if any of these details are incorrect.nn
      operationId: getApiVeosSignature
      x-api-path-slug: apivideossignature-get
      parameters:
      - in: query
        name: flash_request
        description: Allows you to use a flash uploader
      - in: query
        name: max_file_size
        description: Specifies the maximum file size (in bytes) to limit the upload
          too
      - in: query
        name: success_action_redirect
        description: Specifies if to redirect to a URL after a successful post instead
          of issuing a 201
      responses:
        200:
          description: OK
      tags:
      - Api
      - Videos
      - Signature
  /api/videos/{video}.{format}:
    get:
      summary: Get Api Videos
      description: 'nnvzaar uses the oEmbed open standard for allowing 3rd parties
        to integrated with the vzaar. You can use the vzaar video URL to easily obtain
        the appropriate embed code for that video. To find out more about oEmbed view
        the specification here: http://oembed.com/nn'
      operationId: getApiVeosVeo.Format
      x-api-path-slug: apivideosvideo-format-get
      parameters:
      - in: query
        name: borderless,
        description: If set to true and the user has sufficient privileges, the size
          and embeded code returned will be be for a borderless player
      - in: query
        name: embed_only,
        description: When returning data, only include the minimum fields and embed
          code possible
      - in: query
        name: videos is the vzaar video number for that video.
      responses:
        200:
          description: OK
      tags:
      - Api
      - Videos
      - Video
      - Format
  /api/{username}/videos.xml:
    get:
      summary: Get Api Username Videos
      description: nnThis API call returns a list of the users active videos along
        with its relevant metadata. 20 videos are returned by default but this is
        customisable.nn
      operationId: getApiUsernameVeos.xml
      x-api-path-slug: apiusernamevideos-xml-get
      parameters:
      - in: query
        name: count,
        description: Specifies the number of videos to retrieve per page
      - in: query
        name: page,
        description: Specifies the page number to retrieve
      - in: query
        name: sort,
        description: Values can be asc (least_recent) or desc (most_recent)
      - in: query
        name: status,
        description: Values can be processing, active, replaced, deleted and failed
      - in: query
        name: title,
        description: Return only videos with title containing given string
      - in: query
        name: 'username is the vzaar login name for the user. Note: This must be the
          actual username and not the email address'
      responses:
        200:
          description: OK
      tags:
      - Api
      - Username
      - Videos
      - Xml