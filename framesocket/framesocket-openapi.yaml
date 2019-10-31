swagger: "2.0"
x-collection-name: Framesocket
x-complete: 1
info:
  title: Framesocket
  description: framesocket-is-the-best-way-for-developers-and-content-owners-to-tackle-video-projects-of-any-size-
  version: 1.0.0
host: www.framesocket.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /media/activate.php:
    get:
      summary: Activate Media
      description: Activate Media
      operationId: getMediaActivate.php
      x-api-path-slug: mediaactivate-php-get
      parameters:
      - in: query
        name: customid
        description: Custom ID
      - in: query
        name: hash
        description: Video Hash
      - in: query
        name: key
        description: Your account username
      - in: query
        name: secret
        description: Your account API secret
      - in: query
        name: sig
        description: This is an md5 hash of your gatekeeper concatenated with your
          request action
      responses:
        200:
          description: OK
      tags:
      - Media
      - Activate
  /media/deactivate.php:
    get:
      summary: Deactive Media
      description: Deactive Media
      operationId: getMediaDeactivate.php
      x-api-path-slug: mediadeactivate-php-get
      parameters:
      - in: query
        name: customid
        description: Custom ID
      - in: query
        name: hash
        description: Video Hash
      - in: query
        name: key
        description: Your account username
      - in: query
        name: secret
        description: Your account API secret
      - in: query
        name: sig
        description: This is an md5 hash of your gatekeeper concatenated with your
          request action
      responses:
        200:
          description: OK
      tags:
      - Media
      - Deactivate
  /media/images.php:
    get:
      summary: Query Images
      description: Query Images
      operationId: getMediaImages.php
      x-api-path-slug: mediaimages-php-get
      parameters:
      - in: query
        name: customid
        description: Custom ID
      - in: query
        name: hash
        description: Video Hash
      - in: query
        name: key
        description: Your account username
      - in: query
        name: secret
        description: Your account API secret
      - in: query
        name: sig
        description: This is an md5 hash of your gatekeeper concatenated with your
          request action
      responses:
        200:
          description: OK
      tags:
      - Media
      - Images
  /media/query.php:
    get:
      summary: Query Media
      description: Query Media
      operationId: getMediaQuery.php
      x-api-path-slug: mediaquery-php-get
      parameters:
      - in: query
        name: andkeywords
        description: Comma separated list of title words
      - in: query
        name: andtitlewords
        description: Comma separated list of title words
      - in: query
        name: customid
        description: Custom ID
      - in: query
        name: hash
        description: Media Hash Code
      - in: query
        name: key
        description: Your account username
      - in: query
        name: limit
        description: Must be a valid integer
      - in: query
        name: orkeywords
        description: Comma separated list of title words
      - in: query
        name: ortitlewords
        description: Comma separated list of title words
      - in: query
        name: secret
        description: Your account API secret
      - in: query
        name: sig
        description: This is an md5 hash of your gatekeeper concatenated with your
          request action
      - in: query
        name: sort
        description: Must be a valid sorting option, either newest or oldest firs
      - in: query
        name: status
        description: Must be a valid status code
      - in: query
        name: type
        description: Must be a valid type, either image or video
      responses:
        200:
          description: OK
      tags:
      - Media
      - Query
  /media/update.php:
    get:
      summary: Update Media
      description: Update Media
      operationId: getMediaUpdate.php
      x-api-path-slug: mediaupdate-php-get
      parameters:
      - in: query
        name: customid
        description: Custom ID
      - in: query
        name: description
        description: Text String - Limit 1000 characters
      - in: query
        name: hash
        description: Video Hash
      - in: query
        name: imagehash
        description: This needs to refer to an image already assigned to this media
      - in: query
        name: key
        description: Your account username
      - in: query
        name: keywords
        description: Text String - Comma separated by keyword or phrase
      - in: query
        name: secret
        description: Your account API secret
      - in: query
        name: sig
        description: This is an md5 hash of your gatekeeper concatenated with your
          request action
      - in: query
        name: title
        description: Text String - Limit 100 characters
      responses:
        200:
          description: OK
      tags:
      - Media
      - Update
  /media/upload.php:
    post:
      summary: Upload Media
      description: Upload Media
      operationId: postMediaUpload.php
      x-api-path-slug: mediaupload-php-post
      parameters:
      - in: query
        name: callback
      - in: query
        name: customid
        description: Text String - Max Length 32 Characters
      - in: query
        name: description
        description: Text String - Limit 1000 Characters
      - in: query
        name: key
        description: Your account username
      - in: query
        name: keywords
        description: Text String - Comma separated by keyword or phrase
      - in: query
        name: media
        description: Must be properly formatted POST data - either an image or a video
      - in: query
        name: secret
        description: Your account API secret
      - in: query
        name: sig
        description: This is an md5 hash of your gatekeeper concatenated with your
          request action
      - in: query
        name: title
        description: Text String - Limit 100 Characters
      responses:
        200:
          description: OK
      tags:
      - Media
      - Upload