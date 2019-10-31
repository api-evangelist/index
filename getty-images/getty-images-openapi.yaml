swagger: "2.0"
x-collection-name: Getty Images
x-complete: 1
info:
  title: Getty Images
  description: build-applications-using-the-worlds-most-powerful-imagery
  version: 1.0.0
host: api.gettyimages.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/artists/images:
    get:
      summary: Search Artist Images
      description: Search for images by a photographer
      operationId: Artists_GetImagesByArtist
      x-api-path-slug: v3artistsimages-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: query
        name: artist_name
        description: Name of artist for desired images
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Comma separated list of fields
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      responses:
        200:
          description: OK
      tags:
      - Images
      - Artists
  /v3/artists/videos:
    get:
      summary: Search Artist ImaVideosges
      description: Search for videos by a photographer
      operationId: Artists_GetVideosByArtist
      x-api-path-slug: v3artistsvideos-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: query
        name: artist_name
        description: Name of artist for desired images
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Comma separated list of fields
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      responses:
        200:
          description: OK
      tags:
      - Images
      - Artists
      - Videos
  /v3/asset-changes/change-sets:
    put:
      summary: Get Asset Change Notifications
      description: "# Asset Changes\r\n\r\nGet notifications about new, updated or
        deleted assets.\r\n\r\n##  Quickstart\r\n\r\nYou'll need an API key and a
        [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key. \r\n\r\n    \r\nPartner
        channels that have not been checked within the last 120 days will be removed
        and that partner will no longer be able \r\nto get change notifications from
        that channel.\r\nPartners who would like to start using the Asset Changes
        API again after a period of dormancy should contact their sales\r\nrepresentative
        to be set up again."
      operationId: AssetChanges_PutAssetChanges
      x-api-path-slug: v3assetchangeschangesets-put
      parameters:
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: batch_size
        description: Specifies the number of assets to return
      - in: query
        name: channel_id
        description: Specifies the id of the channel for the asset data
      responses:
        200:
          description: OK
      tags:
      - Images
      - Changes
  /v3/asset-changes/change-sets/{change-set-id}:
    delete:
      summary: Get Asset Change Notification
      description: "# Delete Asset Changes\r\n\r\nConfirm asset changes acknowledges
        receipt of asset changes (from the PUT asset changes endpoint).\r\n\r\n##
        \ Quickstart\r\n\r\nYou'll need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: AssetChanges_DeleteAssetChanges
      x-api-path-slug: v3assetchangeschangesetschangesetid-delete
      parameters:
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: change-set-id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Changes
  /v3/asset-changes/channels:
    get:
      summary: Get Asset Change Channels
      description: "# Get Partner Channels\r\n\r\nRetrieves the channel data for the
        partner. This data can be used to populate the channel_id parameter in the
        Put Asset Changes query.\r\n\r\n##  Quickstart\r\n\r\nYou'll need an API key
        and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key. \r\n\r\nOnly channels
        that have been queried in the last 120 days will be included in the list of
        channels.\r\nPartners who have a channel that has been removed should contact
        their sales representative to be set up again."
      operationId: AssetChanges_GetPartnerChannel
      x-api-path-slug: v3assetchangeschannels-get
      parameters:
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      responses:
        200:
          description: OK
      tags:
      - Images
      - Changes
  /v3/asset-registrations:
    post:
      summary: Register Assets
      description: "# Register Assets\r\n\r\nRegisters a list of assets that a customer
        has stored in their system.\r\n\r\n##  Quickstart\r\n\r\nYou'll need an API
        key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key. \r\n\r\n_Note_:
        In the event of a successful query (response code 200) there will be nothing
        in the response body."
      operationId: AssetRegistration_Register
      x-api-path-slug: v3assetregistrations-post
      parameters:
      - in: body
        name: request
        description: Specify JSON containing an array of asset ids to register
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Images
      - Registrations
  /v3/boards:
    get:
      summary: Get All Boards
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to retrieve all Boards available for a user.\r\n\r\nYou'll
        need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_GetAllBoards
      x-api-path-slug: v3boards-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: board_relationship
        description: Search for boards the user owns or has been invited to as an
          editor
      - in: query
        name: page
        description: Request results starting at a page number (default is 1)
      - in: query
        name: pageSize
        description: Request number of boards to return in each page
      - in: query
        name: sort_order
        description: Sort the list of boards by last update date or name
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
    post:
      summary: Create Board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to create a Board by a specific id.\r\n\r\nYou'll need an
        API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key.\r\n\r\n**NOTE:**
        *The input to this endpoint is not sanitized in any way, so it is the responsibility
        of the client to ensure that it is properly formatted and guards against malicious
        data (for example cross-site scripting attacks or HTML injection) when accessing
        the data.*"
      operationId: Boards_CreateBoard
      x-api-path-slug: v3boards-post
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: body
        name: new_board
        description: Specify a name and description of the board to create (name is
          required)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
  /v3/boards/{board_id}:
    delete:
      summary: Delete Board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to delete a Board by a specific id.\r\n\r\nYou'll need an
        API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_DeleteBoard
      x-api-path-slug: v3boardsboard-id-delete
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
    get:
      summary: Get Board Assets
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to retrieve a Board by a specific id.\r\n\r\nYou'll need
        an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_GetBoard
      x-api-path-slug: v3boardsboard-id-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
    put:
      summary: Update Board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to update a Board by a specific id.\r\n\r\nYou'll need an
        API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key.\r\n\r\n**NOTE:**
        *The input to this endpoint is not sanitized in any way, so it is the responsibility
        of the client to ensure that it is properly formatted and guards against malicious
        data (for example cross-site scripting attacks or HTML injection) when accessing
        the data.*"
      operationId: Boards_UpdateBoard
      x-api-path-slug: v3boardsboard-id-put
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
      - in: body
        name: board_info
        description: Specify a new name and description for the board (name is required)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
  /v3/boards/{board_id}/assets:
    delete:
      summary: Remove Assets From Board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
        this endpoint to remove a set of assets from a board.\r\n\r\nYou'll need an
        API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_RemoveAssets
      x-api-path-slug: v3boardsboard-idassets-delete
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: query
        name: asset_ids
        description: List the assets to be removed from the board
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
    put:
      summary: Add Assets to a Board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
        this endpoint to add a set of assets to a board.\r\n\r\nYou'll need an API
        key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_AddAssets
      x-api-path-slug: v3boardsboard-idassets-put
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: body
        name: board_assets
        description: List assets to add to the board
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: board_id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
  /v3/boards/{board_id}/assets/{asset_id}:
    delete:
      summary: Remove an asset from a board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to remove an asset from a board.\r\n\r\nYou'll need an API
        key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_RemoveAsset
      x-api-path-slug: v3boardsboard-idassetsasset-id-delete
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: path
        name: asset_id
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
    put:
      summary: Add an asset to a board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place.\r\nMore information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to add an asset to a board.\r\n\r\nYou'll need an API key
        and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_AddAsset
      x-api-path-slug: v3boardsboard-idassetsasset-id-put
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: path
        name: asset_id
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
  /v3/boards/{board_id}/comments:
    get:
      summary: Get comments from a board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).
        Use this endpoint to retrieve all comments for a specific board.\r\n\r\nYou'll
        need an API key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_GetComments
      x-api-path-slug: v3boardsboard-idcomments-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
      - Comments
    post:
      summary: Add a comment to a board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
        this endpoint to add a comment to a board.\r\n\r\nYou'll need an API key and
        a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_AddComment
      x-api-path-slug: v3boardsboard-idcomments-post
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
      - in: body
        name: comment
        description: Comment to be added to the board
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
      - Comments
  /v3/boards/{board_id}/comments/{comment_id}:
    delete:
      summary: Delete a comment from a board
      description: "Boards are where you collect, curate, collaborate on and manage
        photo and video assets in one place. More information on the [Boards FAQ](http://www.gettyimages.com/boards/faq).\r\nUse
        this endpoint to delete a comment from a board.\r\n\r\nYou'll need an API
        key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Boards_DeleteComment
      x-api-path-slug: v3boardsboard-idcommentscomment-id-delete
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
      - in: path
        name: comment_id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Boards
      - Comments
  /v3/collections:
    get:
      summary: Get Collections
      description: "Use this endpoint to retrieve collections associated with your
        Getty Images account. To browse available collections see our [Image collections
        page]( http://www.gettyimages.com/creative-images/collections).\r\n\r\nYou'll
        need an API key and access token to use this resource. Please see our [Getting
        Started](http://developers.gettyimages.com/en/getting-started.html) page for
        more information on how to sign up for an API key."
      operationId: Collections_GetCollections
      x-api-path-slug: v3collections-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      responses:
        200:
          description: OK
      tags:
      - Images
      - Collections
  /v3/countries:
    get:
      summary: Get Countries
      description: "Returns a list of country objects that contains country name,
        two letter ISO abbreviation and three letter ISO abbreviation.\r\n\r\nYou'll
        need an API key and access token to use this resource. Please see our [Getting
        Started](http://developers.gettyimages.com/en/getting-started.html) page for
        more information on how to sign up for an API key."
      operationId: Countries_GetCountries
      x-api-path-slug: v3countries-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      responses:
        200:
          description: OK
      tags:
      - Images
      - Countries
  /v3/downloads:
    get:
      summary: Get Downloads
      description: "Returns information about a customer's previously downloaded assets.\r\n\r\nYou'll
        need an API key and access token to use this resource. Please see our [Getting
        Started](http://developers.gettyimages.com/en/getting-started.html) page for
        more information on how to sign up for an API key. \r\n \r\n\t\r\nThis endpoint
        requires being a Getty Images customer to limit your results to only assets
        that you have a license to use, \r\nyou need to also include an authorization
        token in the header of your request. \r\nPlease consult our [Authorization
        FAQ](http://developers.gettyimages.com/en/authorization-faq.html) for more
        information on authorization tokens."
      operationId: Downloads_GetDownloads
      x-api-path-slug: v3downloads-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: company_downloads
        description: If specified, returns the list of previously downloaded images
          for all users in your company
      - in: query
        name: end_date
        description: If specified, select assets downloaded on or before this date
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      - in: query
        name: product_type
        description: Specifies product type to be included in the previous download
          results
      - in: query
        name: start_date
        description: If specified, select assets downloaded on or after this date
      responses:
        200:
          description: OK
      tags:
      - Images
      - Downloads
  /v3/downloads/images/{id}:
    post:
      summary: Download an image
      description: "Use this endpoint to generate download URLs and related data for
        images you are authorized to download.\r\n\r\nMost product offerings have
        enforced periodic download limits such as monthly, weekly, and daily. When
        this operation executes, the count of allowed downloads is decremented by
        one for the product offering. Once the download limit is reached for a given
        product offering, no further downloads may be requested for that product offering
        until the next download period.\r\n\r\nThe download limit for a given download
        period is covered in your product agreement established with Getty Images.\r\n\r\nYou'll
        need an API key and a [Resource Owner Grant or Implicit Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key. \r\n\r\n## Auto
        Downloads\r\nThe `auto_download` request query parameter specifies whether
        to automatically download the image.\r\n\r\nIf the `auto_download` request
        query parameter is set to _true_, the API will return an HTTP status code
        303 *See Other*.???Your client code will need to process this response and
        redirect to the URI specified in the *Location* header to enable you to automatically
        download the file. The redirection workflow follows the [HTTP 1.1 protocol](https://tools.ietf.org/html/rfc7231#section-6.4.4).\r\n\r\nClient
        Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/images/[asset_id]?auto_download=true\r\n```\r\n\r\nServer
        Response:\r\n\r\n```\r\nHTTP/1.1 303 See Other\r\nLocation: https://delivery.gettyimages.com/...\r\n```\r\n\r\nIf
        the `auto_download` request query parameter is set to false, the API will
        return a HTTP status code 200, along with the URI in the response body which
        can be used to download the image. \r\n\r\nClient Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/images/[asset_id]?auto_download=false\r\n```\r\n\r\nServer
        Response:\r\n\r\n```\r\nHTTP/1.1 200 OK\r\n{\r\n\t\"uri\": \"https://delivery.gettyimages.com/...\"\r\n}\r\n```"
      operationId: Downloads_PostDownloads
      x-api-path-slug: v3downloadsimagesid-post
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: auto_download
        description: Specifies whether to auto-download the image
      - in: body
        name: download_details
        description: Additional information required from specific customers when
          downloading
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: file_type
        description: File Type expressed with three character file extension
      - in: query
        name: height
        description: Specifies the pixel height of the particular image to download
      - in: path
        name: id
        description: Id of image to download
      - in: query
        name: product_id
        description: Identifier of the instance for the selected product offering
          type
      - in: query
        name: product_type
        description: Product type
      responses:
        200:
          description: OK
      tags:
      - Images
      - Downloads
  /v3/downloads/videos/{id}:
    post:
      summary: Download a video
      description: "Use this endpoint to generate download URLs and related data for
        videos you are authorized to download.\r\n\r\nMost product offerings have
        enforced periodic download limits such as monthly, weekly, and daily. When
        this operation executes, the count of allowed downloads is decremented by
        one for the product offering. Once the download limit is reached for a given
        product offering, no further downloads may be requested for that product offering
        until the next download period.\r\n\r\nThe download limit for a given download
        period is covered in your product agreement established with Getty Images.\r\n\r\nYou'll
        need an API key and a [Resource Owner Grant or Implicit Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key. \r\n\r\n## Auto
        Downloads\r\nThe `auto_download` request query parameter specifies whether
        to automatically download the video.\r\n\r\nIf the `auto_download` request
        query parameter is set to _true_, the API will return an HTTP status code
        303 *See Other*.???Your client code will need to process this response and
        redirect to the URI specified in the *Location* header to enable you to automatically
        download the file. The redirection workflow follows the [HTTP 1.1 protocol](https://tools.ietf.org/html/rfc7231#section-6.4.4).\r\n\r\nClient
        Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/videos/[asset_id]?auto_download=true\r\n```\r\n\r\nServer
        Response:\r\n\r\n```\r\nHTTP/1.1 303 See Other\r\nLocation: https://delivery.gettyimages.com/...\r\n```\r\n\r\nIf
        the `auto_download` request query parameter is set to false, the API will
        return a HTTP status code 200, along with the URI in the response body which
        can be used to download the video. \r\n\r\nClient Request:\r\n\r\n```\r\nhttps://api.gettyimages.com/v3/downloads/videos/[asset_id]?auto_download=false\r\n```\r\n\r\nServer
        Response:\r\n\r\n```\r\nHTTP/1.1 200 OK\r\n{\r\n\t\"uri\": \"https://delivery.gettyimages.com/...\"\r\n}\r\n```"
      operationId: Downloads_PostVideoDownloads
      x-api-path-slug: v3downloadsvideosid-post
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: auto_download
        description: Specifies whether to auto-download the video
      - in: body
        name: download_details
        description: Additional information required from specific customers when
          downloading
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Id of video to download
      - in: query
        name: product_id
        description: Identifier of the instance for the selected product offering
          type
      - in: query
        name: size
        description: Specifies the size to be downloaded
      responses:
        200:
          description: OK
      tags:
      - Images
      - Downloads
      - Videos
  /v3/events:
    get:
      summary: Get metadata for multiple events
      description: "This endpoint returns the detailed event metadata for all specified
        events. Getty Images news, sports and entertainment photographers and\r\nvideographers
        cover editorially relevant events occurring around the world.  All images
        or video clips produced in association with \r\nan event, are assigned the
        same EventID. EventIDs are part of the meta-data returned in SearchForImages
        Results. Only content \r\nproduced under a Getty Images brand name (Getty
        Images News, Getty Images Sports, Getty Images Entertainment, Film Magic,
        Wire Image) \r\nwill be consistently assigned an EventID. The Event framework
        may also be used to group similar content, such as \r\n\"Hats from the Royal
        Wedding\" or \"Odd-ballOffbeat images of the week\". \r\n\r\nYou'll need an
        API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Events_GetBatch
      x-api-path-slug: v3events-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: A comma separated list of fields to return in the response
      - in: query
        name: ids
        description: A comma separated list of event ids
      responses:
        200:
          description: OK
      tags:
      - Images
      - Events
  /v3/events/{id}:
    get:
      summary: Get metadata for a single event
      description: "This endpoint returns the detailed event metadata for a specified
        event. Getty Images news, sports and entertainment \r\nphotographers and videographers
        cover editorially relevant events occurring around the world.  \r\nAll images
        or video clips produced in association with an event, are assigned the same
        EventID. \r\nEventIDs are part of the meta-data returned in SearchForImages
        Results. Only content produced under a Getty Images \r\nbrand name (Getty
        Images News, Getty Images Sports, Getty Images Entertainment, Film Magic,
        Wire Image) will be \r\nconsistently assigned an EventID. The Event framework
        may also be used to group similar content, such as \r\n\"Hats from the Royal
        Wedding\" or \"Odd-ballOffbeat images of the week\". \r\n\r\nYou'll need an
        API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage
        for more information on how to sign up for an API key."
      operationId: Events_Get
      x-api-path-slug: v3eventsid-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: A comma separated list of fields to return in the response
      - in: path
        name: id
        description: An event id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Events
  /v3/images:
    get:
      summary: Get Images
      description: "This endpoint returns the detailed image metadata for all specified
        images. Due to a wide variety of available image resolutions,\r\nthe images
        are grouped into a handful of size categories for simplicity. \r\n\r\nYou'll
        need an API key and access token to use this resource. Please see our [Getting
        Started](http://developers.gettyimages.com/en/getting-started.html) \r\npage
        for more information on how to sign up for an API key. \r\n\r\n## Working
        with Fields Sets\r\n\r\nFields sets are used in the **fields** request parameter
        to receive a suite of metadata fields. The following fields sets are available:\r\n\r\n####
        Summary Fields Set\r\n\r\nThe **summary_set** query string parameter fields
        value represents a small batch of metadata fields that are often used to build
        \r\nsearch response results. The following fields are provided for every image
        in your result set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"images\":\r\n    [\r\n        \"artist\",\r\n        \"asset_family\",\r\n
        \       \"caption\",\r\n        \"collection_code\",\r\n        \"collection_id\",\r\n
        \       \"collection_name\",\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n
        \       \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Detail Fields Set\r\n\r\nThe
        **detail_set** query string parameter fields value represents a large batch
        of metadata fields that are often used to build a \r\ndetailed view of images.
        The following fields are provided for every image in your result set when
        you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n
        \   [\r\n        \"allowed_use\",\r\n        \"artist\", \r\n        \"artist_title\",
        \r\n        \"asset_family\",\r\n        \"call_for_image\",\r\n        \"caption\",
        \r\n        \"city\",\r\n        \"collection_code\",\r\n        \"collection_id\",
        \r\n        \"collection_name\",\r\n        \"color_type\", \r\n        \"copyright\",
        \r\n        \"country\", \r\n        \"credit_line\", \r\n        \"date_created\",
        \r\n        \"date_submitted\",\r\n        \"download_sizes\", \r\n        \"editorial_segments\",\r\n
        \       \"event_ids\",\r\n        \"graphical_style\",\r\n        \"license_model\",\r\n
        \       \"max_dimensions\",\r\n        \"orientation\",\r\n        \"prestige\",\r\n
        \       \"product_types\",\r\n        \"quality_rank\",\r\n        \"referral_destinations\",\r\n
        \       \"state_province\", \r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Display Fields Set\r\n\r\nThe **display_set** query string parameter fields
        value represents the fields that provide you with URLs for the low resolution\r\nfiles
        that are most frequently used to build a UI displaying search results. The
        following fields are provided for every image \r\nin your result set when
        you include **display_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n
        \   [\r\n        \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\":
        \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
        \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n
        \           }\r\n        ]\r\n    ]\r\n}\r\n```\r\n\r\n## Request Usage Considerations\r\n\r\n-
        Specifying the \"entity_details\" response field can have significant performance
        implications. The field should be used only when necessary."
      operationId: Images_GetBatch
      x-api-path-slug: v3images-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: ids
        description: Specifies one or more image ids to return
      responses:
        200:
          description: OK
      tags:
      - Images
  /v3/images/{id}:
    get:
      summary: Get Image
      description: "This endpoint returns the detailed image metadata for a specified
        image. Due to a wide variety of available image resolutions, \r\nthe images
        are grouped into a handful of size categories for simplicity. \r\n\r\nYou'll
        need an API key and access token to use this resource. Please see our [Getting
        Started](http://developers.gettyimages.com/en/getting-started.html) \r\npage
        for more information on how to sign up for an API key. \r\n \r\n## Working
        with Fields Sets\r\n\r\nFields sets are used in the **fields** request parameter
        to receive a suite of metadata fields. The following fields sets are available:\r\n\r\n####
        Summary Fields Set\r\n\r\nThe **summary_set** query string parameter fields
        value represents a small batch of metadata fields that\r\nare often used to
        build search response results. The following fields are provided for every
        image in your\r\nresult set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"images\":\r\n    [\r\n        \"artist\",\r\n        \"asset_family\",\r\n
        \       \"caption\",\r\n        \"collection_code\",\r\n        \"collection_id\",\r\n
        \       \"collection_name\",\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n
        \       \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Detail Fields Set\r\n\r\nThe
        **detail_set** query string parameter fields value represents a large batch
        of metadata fields that are \r\noften used to build a detailed view of images.
        The following fields are provided for every image in your \r\nresult set when
        you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n
        \   [\r\n        \"allowed_use\",\r\n        \"artist\", \r\n        \"artist_title\",
        \r\n        \"asset_family\",\r\n        \"call_for_image\",\r\n        \"caption\",
        \r\n        \"city\",\r\n        \"collection_code\",\r\n        \"collection_id\",
        \r\n        \"collection_name\",\r\n        \"color_type\", \r\n        \"copyright\",
        \r\n        \"country\", \r\n        \"credit_line\", \r\n        \"date_created\",
        \r\n        \"date_submitted\",\r\n        \"download_sizes\", \r\n        \"editorial_segments\",\r\n
        \       \"event_ids\",\r\n        \"graphical_style\",\r\n        \"license_model\",\r\n
        \       \"max_dimensions\",\r\n        \"orientation\",\r\n        \"prestige\",\r\n
        \       \"product_types\",\r\n        \"quality_rank\",\r\n        \"referral_destinations\",\r\n
        \       \"state_province\", \r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Display Fields Set\r\n\r\nThe **display_set** query string parameter fields
        value represents the fields that provide you with URLs for the low\r\nresolution
        files that are most frequently used to build a UI displaying search results.
        The following fields are provided \r\nfor every image in your result set when
        you include **display_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n
        \   [\r\n        \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\":
        \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
        \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n
        \           }\r\n        ]\r\n    ]\r\n}\r\n```\r\n\r\n## Request Usage Considerations\r\n\r\n-
        Specifying the \"entity_details\" response field can have significant performance
        implications. The field should be used only when necessary."
      operationId: Images_Get
      x-api-path-slug: v3imagesid-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Specifies fields to return
      - in: path
        name: id
        description: An image id
      responses:
        200:
          description: OK
      tags:
      - Images
  /v3/images/{id}/similar:
    get:
      summary: Search Similar Images
      description: "This endpoint will search our asset database for images similar
        to the specified asset id. Due to a wide variety of available \r\nimage resolutions,
        the images are grouped into a handful of size categories for simplicity. \r\n\r\nYou'll
        need an API key and access token to use this resource. Please see our [Getting
        Started](http://developers.gettyimages.com/en/getting-started.html) \r\npage
        for more information on how to sign up for an API key. \r\n\r\n## Working
        with Fields Sets\r\n\r\nFields sets are used in the **fields** request parameter
        to receive a suite of metadata fields. The following fields sets are available:\r\n\r\n####
        Summary Fields Set\r\n\r\nThe **summary_set** query string parameter fields
        value represents a small batch of metadata fields that are often used to build\r\nsearch
        response results. The following fields are provided for every image in your
        result set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"images\":\r\n    [\r\n        \"asset_family\",\r\n        \"caption\",\r\n
        \       \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n
        \       \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\":
        \"thumb\"\r\n            }\r\n        ]\r\n        \"license_model\",\r\n
        \       \"max_dimensions\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields
        value represents a large batch of metadata fields that are often used to build
        a \r\ndetailed view of images. The following fields are provided for every
        image in your result set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"images\":\r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n
        \       \"asset_family\",\r\n        \"call_for_image\",\r\n        \"caption\",\r\n
        \       \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n
        \       \"copyright\",\r\n        \"date_created\",\r\n        \"display_sizes\":
        \r\n        [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
        \           {\r\n                \"name\": \"preview\"\r\n            },\r\n
        \           {\r\n                \"name\": \"thumb\"\r\n            }\r\n
        \       ],\r\n        \"editorial_segments\",\r\n        \"event_ids\",\r\n
        \       \"graphical_style\",\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n
        \       \"orientation\",\r\n        \"product_types\",\r\n        \"quality_rank\",\r\n
        \       \"referral_destinations\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Display Fields Set\r\n\r\nThe **display_set** query string parameter fields
        value represents the fields that provide you with URLs for the low resolution
        files \r\nthat are most frequently used to build a UI displaying search results.
        The following fields are provided for every image in your result\r\nset when
        you include **display_set** in your request.\r\n\r\n```\r\n{\r\n    \"images\":\r\n
        \   [\r\n        \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\":
        \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
        \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n
        \           }\r\n        ]\r\n    ]\r\n}\r\n```"
      operationId: Images_GetSimilarImages
      x-api-path-slug: v3imagesidsimilar-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Specifies fields to return
      - in: path
        name: id
        description: Identifies an existing image
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      responses:
        200:
          description: OK
      tags:
      - Images
      - Similar
  /v3/products:
    get:
      summary: Get Products
      description: "This endpoint returns all products available to the username used
        during authentication. As such, this endpoint requires the use of\r\na fully
        authorized access_token. The product data can then be used as search filters,
        restricting results to images from a specific product.\r\n\r\nYou'll need
        an API key and access token to use this resource. Please see our [Getting
        Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage
        for more information on how to sign up for an API key."
      operationId: Products_GetProducts
      x-api-path-slug: v3products-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Comma separated list of fields
      responses:
        200:
          description: OK
      tags:
      - Images
      - Products
  /v3/purchased-assets:
    get:
      summary: Get Purchased Images
      description: "This endpoint returns a list of all assets purchased on gettyimages.com
        by the username used for authentication. \r\nUse of this endpoint requires
        configuration changes to your API key. \r\nPlease contact [developersupport@gettyimages.com](mailto:developersupport@gettyimages.com)
        to learn more.\r\n\r\nYou'll need an API key and access token to use this
        resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage
        for more information on how to sign up for an API key."
      operationId: Purchases_GetPreviousAssetPurchases
      x-api-path-slug: v3purchasedassets-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: end_date
        description: If specified, retrieves previous purchases on or before this
          date
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      - in: query
        name: start_date
        description: If specified, retrieves previous purchases on or after this date
      responses:
        200:
          description: OK
      tags:
      - Images
      - Purchases
  /v3/purchased-images:
    get:
      summary: Get Previously Purchased Images
      description: "This endpoint returns a list of all images purchased on gettyimages.com
        by the username used for authentication.\r\nUse of this endpoint requires
        configuration changes to your API key. Please contact [developersupport@gettyimages.com](mailto:developersupport@gettyimages.com)\r\nto
        learn more.\r\n\r\nYou'll need an API key and access token to use this resource.
        Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage
        for more information on how to sign up for an API key."
      operationId: Purchases_GetPreviousPurchases
      x-api-path-slug: v3purchasedimages-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: end_date
        description: If specified, retrieves previous purchases on or before this
          date
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      - in: query
        name: start_date
        description: If specified, retrieves previous purchases on or after this date
      responses:
        200:
          description: OK
      tags:
      - Images
      - Purchases
  /v3/search/events:
    get:
      summary: Search for events
      description: "Use this endpoint to search Getty Images news, sports and entertainment
        events. Getty Images photographers and videographers cover editorially relevant
        events occurring around the world.  All images or video clips produced in
        association with an event, are assigned the same EventID. EventIDs are part
        of the meta-data returned in Search Results. Only content produced under a
        Getty Images brand name (Getty Images News, Getty Images Sports, Getty Images
        Entertainment, Film Magic, Wire Image) will be consistently assigned an EventID.
        The Event framework may also be used to group similar content, such as \"Hats
        from the Royal Wedding\" or \"Odd-ballOffbeat images of the week\".   \r\n\r\nYou'll
        need an API key and access token to use this resource. Please see our [Getting
        Started](http://developers.gettyimages.com/en/getting-started.html) page for
        more information on how to sign up for an API key.\r\n\r\n\r\nYou can show
        different information in the response by specifying values on the \"fields\"
        parameter (see details below).\r\nYou can search with only an API key, and
        that will give you search results that are equivalent to doing a search on
        the GettyImages.com site without being logged in (anonymous search).  If you
        are a Getty Images API customer and would like to ensure that your API searches
        return only assets that you have a license to use, you need to also include
        an authorization token in the header of your request.  Please consult our
        [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
        for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
        for code examples of getting a token."
      operationId: Search_GetEvents
      x-api-path-slug: v3searchevents-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: date_from
        description: Filters to events that start on or after this date
      - in: query
        name: date_to
        description: Filters to events that start on or before this date
      - in: query
        name: editorial_segment
        description: Filters to events with a matching editorial segment
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: page
        description: Request results starting at a page number (default is 1, maximum
          is 50)
      - in: query
        name: page_size
        description: Request number of images to return in each page
      - in: query
        name: phrase
        description: Filters to events related to this phrase
      responses:
        200:
          description: OK
      tags:
      - Images
      - Search
  /v3/search/images:
    get:
      summary: Search Images
      description: Use this endpoint to search over a blend of our contemporary stock
        photos, illustrations, archival images, editorial photos, illustrations and
        archival images.
      operationId: Search_GetImagesByPhrase
      x-api-path-slug: v3searchimages-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: query
        name: age_of_people
        description: Filter based on the age of individuals in an image
      - in: query
        name: artists
        description: Search for images by specific artists (free-text, comma-separated
          list of artists)
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: collections_filter_type
        description: Provides searching based on specified collection(s)
      - in: query
        name: collection_codes
        description: Filter by collection codes (comma-separated list)
      - in: query
        name: color
        description: Filter based on predominant color in an image
      - in: query
        name: compositions
        description: Filter based on image composition
      - in: query
        name: embed_content_only
        description: Restrict search results to embeddable images
      - in: query
        name: ethnicity
        description: Filter search results based on the ethnicity of individuals in
          an image
      - in: query
        name: event_ids
        description: Filter based on specific events
      - in: query
        name: exclude_nudity
        description: Excludes images containing nudity
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: file_types
        description: Return only images having a specific file type
      - in: query
        name: graphical_styles
        description: Filter based on graphical style of the image
      - in: query
        name: keyword_ids
        description: Return only images tagged with specific keyword(s)
      - in: query
        name: license_models
        description: Specifies the image licensing model(s)
      - in: query
        name: minimum_size
        description: Filter based on minimum size requested
      - in: query
        name: number_of_people
        description: Filter based on the number of people in the image
      - in: query
        name: orientations
        description: Return only images with selected aspect ratios
      - in: query
        name: page
        description: Request results starting at a page number (default is 1)
      - in: query
        name: page_size
        description: Request number of images to return in each page
      - in: query
        name: phrase
        description: Search images using a search phrase
      - in: query
        name: prestige_content_only
        description: Restrict search results to prestige images
      - in: query
        name: product_types
        description: Filter images to those from one of your product types
      - in: query
        name: sort_order
        description: Select sort order of results
      - in: query
        name: specific_people
        description: Return only images associated with specific people (using a comma-delimited
          list)
      responses:
        200:
          description: OK
      tags:
      - Images
      - Search
  /v3/search/images/creative:
    get:
      summary: Search for creative images only
      description: "Use this endpoint to search our contemporary stock photos, illustrations
        and archival images.\r\n\r\nYou'll need an API key and access token to use
        this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        \r\npage for more information on how to sign up for an API key. \r\n \r\nYou
        can show different information in the response by specifying values on the
        \"fields\" parameter (see details below).\r\nYou can search with only an API
        key, and that will give you search results that are equivalent to doing a
        search on the GettyImages.com site without being logged in (anonymous search).
        \ If you are a Getty Images API customer and would like to ensure that your
        API searches return only assets that you have a license to use, you need to
        also include an authorization token in the header of your request.  Please
        consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
        for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
        for code examples of getting a token.\r\n\r\n## Working with Fields Sets\r\n\r\nFields
        sets are used in the **fields** request parameter to receive a suite of metadata
        fields. The following fields sets are available:\r\n\r\n#### Summary Fields
        Set\r\n\r\nThe **summary_set** query string parameter fields value represents
        a small batch of metadata fields that are often used to \r\nbuild search response
        results. The following fields are provided for every image in your result
        set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"images\": \r\n    [\r\n        \"asset_family\",\r\n        \"caption\",\r\n
        \       \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n
        \       \"display_sizes\": \r\n        [\r\n            {\r\n                \"name\":
        \"thumb\"\r\n            }\r\n        ],\r\n        \"license_model\",\r\n
        \       \"max_dimensions\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields
        value represents a large batch of metadata fields that are often used to \r\nbuild
        a detailed view of images. The following fields are provided for every image
        in your result set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"images\": \r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n
        \       \"asset_family\",\r\n        \"call_for_image\",\r\n        \"caption\",\r\n
        \       \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n
        \       \"copyright\",\r\n        \"date_created\",\r\n        \"display_sizes\":
        \r\n        [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
        \           {\r\n                \"name\": \"preview\"\r\n            },\r\n
        \           {\r\n                \"name\": \"thumb\"\r\n            }\r\n
        \       ],\r\n        \"editorial_segments\",\r\n        \"event_ids\",\r\n
        \       \"graphical_style\",\r\n        \"license_model\",\r\n        \"max_dimensions\",\r\n
        \       \"orientation\",\r\n        \"product_types\",\r\n        \"quality_rank\",\r\n
        \       \"referral_destinations\",\r\n        \"title\"\r\n    ]\r\n]\r\n```\r\n\r\n####
        Display Fields Set\r\n\r\nThe **display_set** query string parameter fields
        value represents the fields that provide you with URLs for the low resolution\r\nfiles
        that are most frequently used to build a UI displaying search results. The
        following fields are provided for every image \r\nin your result set when
        you include **display_set** in your request.\r\n\r\n```Go\r\n{\r\n    \"images\":
        \r\n    [\r\n        \"display_sizes\": \r\n        [\r\n            {\r\n
        \               \"name\": \"comp\"\r\n            },\r\n            {\r\n
        \               \"name\": \"preview\"\r\n            },\r\n            {\r\n
        \               \"name\": \"thumb\"\r\n            }\r\n        ]\r\n    ]\r\n}\r\n```"
      operationId: Search_GetCreativeImagesByPhrase
      x-api-path-slug: v3searchimagescreative-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: query
        name: age_of_people
        description: Filter based on the age of individuals in an image
      - in: query
        name: artists
        description: Search for images by specific artists (free-text, comma-separated
          list of artists)
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: collections_filter_type
        description: Use to include or exclude collections from search
      - in: query
        name: collection_codes
        description: Filter by collection codes (comma-separated list)
      - in: query
        name: color
        description: Filter based on predominant color in an image
      - in: query
        name: compositions
        description: Filter based on image composition
      - in: query
        name: embed_content_only
        description: Restrict search results to embeddable images
      - in: query
        name: ethnicity
        description: Filter search results based on the ethnicity of individuals in
          an image
      - in: query
        name: exclude_nudity
        description: Excludes images containing nudity
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: file_types
        description: Return only images having a specific file type
      - in: query
        name: graphical_styles
        description: Filter based on graphical style of the image
      - in: query
        name: keyword_ids
        description: Return only images tagged with specific keyword(s)
      - in: query
        name: license_models
        description: Specifies the image licensing model(s)
      - in: query
        name: minimum_size
        description: Filter based on minimum size requested
      - in: query
        name: number_of_people
        description: Filter based on the number of people in the image
      - in: query
        name: orientations
        description: Return only images with selected aspect ratios
      - in: query
        name: page
        description: Request results starting at a page number (default is 1)
      - in: query
        name: page_size
        description: Request number of images to return in each page
      - in: query
        name: phrase
        description: Search images using a search phrase
      - in: query
        name: prestige_content_only
        description: Restrict search results to prestige images
      - in: query
        name: product_types
        description: Filter images to those from one of your product types
      - in: query
        name: sort_order
        description: Select sort order of results
      responses:
        200:
          description: OK
      tags:
      - Images
      - Search
  /v3/search/images/creative/by-image:
    get:
      summary: Search Images by Image
      description: "Allows searching for similar creative images by passing the URL
        to an existing image.\r\n\r\nBefore calling the search by image endpoint,
        an image must be uploaded to a specific AWS S3 bucket. The bucket name is
        `search-by-image.s3.amazonaws.com`.\r\nFor example, using cURL:\r\n```sh\r\ncurl
        -i -X PUT https://search-by-image.s3.amazonaws.com/my-test-image.jpg -H \"Content-Type:
        image/jpeg\" --data-binary \"@testimage.jpg\"\r\n```\r\n\r\nUploads can be
        overwritten if the names are the same, so using a prefix like the API Key,
        application name or company name would help keep that\r\nfrom happening.\r\n\r\nOnce
        the image has been uploaded, use the full URL in the `image_url` parameter,
        e.g. `image_url=https://search-by-image.s3.amazonaws.com/my-test-image.jpg`.\r\n\r\nSubsequent
        searches for the same image can be executed using the `image_fingerprint`
        that is returned by the inital search."
      operationId: Search_GetCreativeImagesByUrl
      x-api-path-slug: v3searchimagescreativebyimage-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: image_fingerprint
        description: Specifies the fingerprint of the image to use in the search
      - in: query
        name: image_url
        description: Specifies the location of the image to use in the search
      - in: query
        name: page
        description: Request results starting at a page number (default is 1)
      - in: query
        name: page_size
        description: Request number of images to return in each page
      - in: query
        name: product_types
        description: Filter images to those from one of your product types
      responses:
        200:
          description: OK
      tags:
      - Images
      - Search
  /v3/search/images/editorial:
    get:
      summary: Search Editorial Images
      description: Use this endpoint to search our editorial stock photos, illustrations
        and archival images.  Editorial images represent newsworthy events or illustrate
        matters of general interest, such as news, sport and entertainment and are
        generally intended for editorial use.
      operationId: Search_GetEditorialImagesByPhrase
      x-api-path-slug: v3searchimageseditorial-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: query
        name: age_of_people
        description: Filter based on the age of individuals in an image
      - in: query
        name: artists
        description: Search for images by specific artists (free-text, comma-separated
          list of artists)
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: collections_filter_type
        description: Use to include or exclude collections from search
      - in: query
        name: collection_codes
        description: Filter by collections (comma-separated list of collection codes)
      - in: query
        name: compositions
        description: Filter based on image composition
      - in: query
        name: editorial_segments
        description: Return only events with a matching editorial segment
      - in: query
        name: embed_content_only
        description: Restrict search results to embeddable images
      - in: query
        name: end_date
        description: Return only images that are created on or before this date
      - in: query
        name: entity_uris
        description: specify linked data entity uri
      - in: query
        name: ethnicity
        description: Filter search results based on the ethnicity of individuals in
          an image
      - in: query
        name: event_ids
        description: Filter based on specific events
      - in: query
        name: exclude_nudity
        description: Excludes images containing nudity
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: file_types
        description: Return only images having a specific file type
      - in: query
        name: graphical_styles
        description: Filter based on graphical style of the image
      - in: query
        name: keyword_ids
        description: Return only images tagged with specific keyword(s)
      - in: query
        name: minimum_quality_rank
        description: Filter search results based on minimum quality ranking
      - in: query
        name: minimum_size
        description: Filter based on minimum size requested
      - in: query
        name: number_of_people
        description: Filter based on the number of people in the image
      - in: query
        name: orientations
        description: Return only images with selected aspect ratios
      - in: query
        name: page
        description: Request results starting at a page number (default is 1)
      - in: query
        name: page_size
        description: Request number of images to return in each page
      - in: query
        name: phrase
        description: Search images using a search phrase
      - in: query
        name: product_types
        description: Filter images to those from one of your product types
      - in: query
        name: sort_order
        description: Select sort order of results
      - in: query
        name: specific_people
        description: Return only images associated with specific people (using a comma-delimited
          list)
      - in: query
        name: start_date
        description: Return only images that are created on or after this date
      responses:
        200:
          description: OK
      tags:
      - Images
      - Search
      - Editorial
  /v3/search/videos:
    get:
      summary: Search Editorial Videos
      description: "Use this endpoint to search over a blend of our premium stock,
        contemporary 4K and HD footage, celebrities, news, newsmakers, entertainment,
        events and archival videos.\r\n\r\nYou'll need an API key and access token
        to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key.\r\n\r\n\r\nYou
        can show different information in the response by specifying values on the
        \"fields\" parameter (see details below).\r\nYou can search with only an API
        key, and that will give you search results that are equivalent to doing a
        search on the GettyImages.com site without being logged in (anonymous search).
        \ If you are a Getty Images API customer and would like to ensure that your
        API searches return only assets that you have a license to use, you need to
        also include an authorization token in the header of your request.  Please
        consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
        for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
        for code examples of getting a token.\r\n\r\n## Working with Fields Sets\r\n\r\nFields
        sets are used in the **fields** request parameter to receive a suite of metadata
        fields. The following fields sets are available:\r\n\r\n#### Summary Fields
        Set\r\n\r\nThe **summary_set** query string parameter fields value represents
        a small batch of metadata fields that are often used to build search response
        results. The following fields are provided for every video in your result
        set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"videos\":\r\n    [\r\n        \"asset_family\",\r\n        \"caption\",\r\n
        \       \"collection_code\",\r\n        \"collection_name\",\r\n        \"display_sizes\":\r\n
        \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
        \           {\r\n                \"name\": \"preview\"\r\n            },\r\n
        \           {\r\n                \"name\": \"thumb\"\r\n            }\r\n
        \       ],\r\n        \"license_model\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields
        value represents a large batch of metadata fields that are often used to build
        a detailed view of videos. The following fields are provided for every video
        in your result set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"videos\":\r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n
        \       \"asset_family\",\r\n        \"caption\",\r\n        \"clip_length\",\r\n
        \       \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n
        \       \"color_type\",\r\n        \"copyright\",\r\n        \"date_created\",\r\n
        \       \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
        \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
        \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n
        \           }\r\n        ],\r\n        \"era\",\r\n        \"license_model\",\r\n
        \       \"mastered_to\",\r\n        \"originally_shot_on\",\r\n        \"product_types\",\r\n
        \       \"shot_speed\",\r\n        \"source\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Display Fields Set\r\n\r\nThe **display_set** query string parameter fields
        value represents the fields that provide you with URLs for the low resolution
        files that are most frequently used to build a UI displaying search results.
        The following fields are provided for every video in your result set when
        you include **display_set** in your request.\r\n\r\n```\r\n{\r\n    \"videos\":\r\n
        \   [\r\n        \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
        \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
        \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n
        \           }\r\n        ]\r\n    ]\r\n}\r\n```\r\n\r\n## Request Usage Considerations\r\n\r\n-
        Specifying the \"entity_details\" response field can have significant performance
        implications. The field should be used only when necessary."
      operationId: Search_GetVideosByPhrase
      x-api-path-slug: v3searchvideos-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: query
        name: age_of_people
        description: Provides filtering according to the age of individuals in a video
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: collections_filter_type
        description: Provides searching based on specified collection(s)
      - in: query
        name: collection_codes
        description: Provides filtering by collection code
      - in: query
        name: editorial_video_types
        description: Allows filtering by types of video
      - in: query
        name: exclude_nudity
        description: Excludes images containing nudity
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: format_available
        description: Filters according to the digital video format available on a
          film asset
      - in: query
        name: frame_rates
        description: Provides filtering by video frame rate (frames/second)
      - in: query
        name: keyword_ids
        description: Return only images tagged with specific keyword(s)
      - in: query
        name: license_models
        description: Specifies the video licensing model(s)
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      - in: query
        name: phrase
        description: Free-text search query
      - in: query
        name: product_types
        description: Filter images to those from one of your product types
      - in: query
        name: sort_order
        description: Allows sorting of results
      - in: query
        name: specific_people
        description: Provides filtering by specific peoples names
      responses:
        200:
          description: OK
      tags:
      - Images
      - Search
      - Videos
  /v3/search/videos/creative:
    get:
      summary: Search for creative videos
      description: "Use this endpoint to search premium stock video, from archival
        film to contemporary 4K and HD footage.\r\n\r\nYou'll need an API key and
        access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage
        for more information on how to sign up for an API key.\r\n\r\nYou can show
        different information in the response by specifying values on the \"fields\"
        parameter (see details below).\r\nYou can search with only an API key, and
        that will give you search results that are equivalent to doing a search on
        the GettyImages.com site without\r\nbeing logged in (anonymous search).  If
        you are a Getty Images API customer and would like to ensure that your API
        searches return only \r\nassets that you have a license to use, you need to
        also include an authorization token in the header of your request.\r\nPlease
        consult our [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
        for more information on authorization tokens.\r\n\r\n## Working with Fields
        Sets\r\n\r\nFields sets are used in the **fields** request parameter to receive
        a suite of metadata fields. The following fields sets are available:\r\n\r\n####
        Summary Fields Set\r\n\r\nThe **summary_set** query string parameter fields
        value represents a small batch of metadata fields that are often used to build
        search\r\nresponse results. The following fields are provided for every video
        in your result set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"videos\": \r\n    [\r\n        \"asset_family\", \r\n        \"caption\",\r\n
        \       \"collection_code\",\r\n        \"collection_name\",\r\n        \"display_sizes\":\r\n
        \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
        \           {\r\n                \"name\": \"preview\"\r\n            },\r\n
        \           {\r\n                \"name\": \"thumb\"\r\n            }\r\n
        \       ],\r\n        \"license_model\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields
        value represents a large batch of metadata fields that are often used to build
        a \r\ndetailed view of videos. The following fields are provided for every
        video in your result set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"videos\": \r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n
        \       \"asset_family\", \r\n        \"caption\", \r\n        \"clip_length\",\r\n
        \       \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",
        \r\n        \"color_type\",\r\n        \"copyright\",\r\n        \"date_created\",\r\n
        \       \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
        \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
        \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n
        \           }\r\n        ],\r\n        \"era\",\r\n        \"license_model\",\r\n
        \       \"mastered_to\",\r\n        \"originally_shot_on\",\r\n        \"product_types\",\r\n
        \       \"shot_speed\",\r\n        \"source\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Display Fields Set\r\n\r\nThe **display_set** query string parameter fields
        value represents the fields that provide you with URLs for the low resolution
        files \r\nthat are most frequently used to build a UI displaying search results.
        The following fields are provided for every video in your result \r\nset when
        you include **display_set** in your request.\r\n\r\n```\r\n{\r\n    \"videos\":\r\n
        \   [\r\n        \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
        \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
        \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n
        \           }\r\n        ]\r\n    ]\r\n}\r\n```"
      operationId: Search_GetCreativeVideosByPhrase
      x-api-path-slug: v3searchvideoscreative-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: query
        name: age_of_people
        description: Provides filtering according to the age of individuals in a video
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: collections_filter_type
        description: Provides searching based on specified collection(s)
      - in: query
        name: collection_codes
        description: Provides filtering by collection code
      - in: query
        name: exclude_nudity
        description: Excludes images containing nudity
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: format_available
        description: Filters according to the digital video format available on a
          film asset
      - in: query
        name: frame_rates
        description: Provides filtering by video frame rate (frames/second)
      - in: query
        name: keyword_ids
        description: Return only images tagged with specific keyword(s)
      - in: query
        name: license_models
        description: Specifies the video licensing model(s)
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      - in: query
        name: phrase
        description: Free-text search query
      - in: query
        name: product_types
        description: Filter images to those from one of your product types
      - in: query
        name: sort_order
        description: Allows sorting of results
      responses:
        200:
          description: OK
      tags:
      - Images
      - Search
      - Videos
  /v3/search/videos/editorial:
    get:
      summary: Search for editorial videos
      description: "Use this endpoint to search current and archival video clips of
        celebrities, newsmakers, and events.\r\n\r\nYou'll need an API key and access
        token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key.\r\n\r\nYou can
        show different information in the response by specifying values on the \"fields\"
        parameter (see details below).\r\nYou can search with only an API key, and
        that will give you search results that are equivalent to doing a search on
        the GettyImages.com site without being logged in (anonymous search).  If you
        are a Getty Images API customer and would like to ensure that your API searches
        return only assets that you have a license to use, you need to also include
        an authorization token in the header of your request.  Please consult our
        [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
        for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
        for code examples of getting a token.\r\n\r\n## Working with Fields Sets\r\n\r\nFields
        sets are used in the **fields** request parameter to receive a suite of metadata
        fields. The following fields sets are available:\r\n\r\n#### Summary Fields
        Set\r\n\r\nThe **summary_set** query string parameter fields value represents
        a small batch of metadata fields that are often used to build search response
        results. The following fields are provided for every video in your result
        set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"videos\": \r\n    [\r\n        \"asset_family\", \r\n        \"caption\",\r\n
        \       \"collection_code\",\r\n        \"collection_name\",\r\n        \"display_sizes\":\r\n
        \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
        \           {\r\n                \"name\": \"preview\"\r\n            },\r\n
        \           {\r\n                \"name\": \"thumb\"\r\n            }\r\n
        \       ],\r\n        \"license_model\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields
        value represents a large batch of metadata fields that are often used to build
        a detailed view of videos. The following fields are provided for every video
        in your result set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"videos\": \r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n
        \       \"asset_family\", \r\n        \"caption\", \r\n        \"clip_length\",\r\n
        \       \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",
        \r\n        \"color_type\",\r\n        \"copyright\",\r\n        \"date_created\",\r\n
        \       \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
        \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
        \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n
        \           }\r\n        ],\r\n        \"era\",\r\n        \"license_model\",\r\n
        \       \"mastered_to\",\r\n        \"originally_shot_on\",\r\n        \"product_types\",\r\n
        \       \"shot_speed\",\r\n        \"source\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Display Fields Set\r\n\r\nThe **display_set** query string parameter fields
        value represents the fields that provide you with URLs for the low resolution
        files that are most frequently used to build a UI displaying search results.
        The following fields are provided for every video in your result set when
        you include **display_set** in your request.\r\n\r\n```\r\n{\r\n    \"videos\":\r\n
        \   [\r\n        \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
        \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
        \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n
        \           }\r\n        ]\r\n    ]\r\n}\r\n```\r\n\r\n## Request Usage Considerations\r\n\r\n-
        Specifying the \"entity_details\" response field can have significant performance
        implications. The field should be used only when necessary."
      operationId: Search_GetEditorialVideosByPhrase
      x-api-path-slug: v3searchvideoseditorial-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: query
        name: age_of_people
        description: Provides filtering according to the age of individuals in a video
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: collections_filter_type
        description: Provides searching based on specified collection(s)
      - in: query
        name: collection_codes
        description: Provides filtering by collection code
      - in: query
        name: editorial_video_types
        description: Allows filtering by types of video
      - in: query
        name: entity_uris
        description: specify link data entity uri
      - in: query
        name: exclude_nudity
        description: Excludes images containing nudity
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: format_available
        description: Filters according to the digital video format available on a
          film asset
      - in: query
        name: frame_rates
        description: Provides filtering by video frame rate (frames/second)
      - in: query
        name: keyword_ids
        description: Return only images tagged with specific keyword(s)
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      - in: query
        name: phrase
        description: Free-text search query
      - in: query
        name: product_types
        description: Filter images to those from one of your product types
      - in: query
        name: sort_order
        description: Allows sorting of results
      - in: query
        name: specific_people
        description: Allows filtering by specific peoples names
      responses:
        200:
          description: OK
      tags:
      - Images
      - Search
      - Videos
      - Editoria
  /v3/usage-batches/{id}:
    put:
      summary: Reports Usage Batches
      description: "# Report Usage\r\n\r\nUse this endpoint to report the usages of
        a set of assets. The count of assets submitted in a single batch to this endpoint
        is limited to 1000. Note that all asset Ids specified must be valid or the
        operation will fail causing no usages to be recorded. In this case, you will
        need to remove the invalid asset Ids from the query request and re-submit
        the query.\r\n\r\n##  Quickstart\r\n\r\nYou'll need an API key and a [Resource
        Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key. \r\n\r\n\r\n_Note_:
        Date of use can be in any unambiguous date format."
      operationId: Usage_Put
      x-api-path-slug: v3usagebatchesid-put
      parameters:
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: id
        description: Specifies a unique batch transaction id to identify the report
      - in: body
        name: request
        description: Specifies up to 1000 sets of asset Id, usage count, and date
          of use to submit usages for
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Images
      - Batches
  /v3/videos:
    get:
      summary: Get Videos Metadatata
      description: "Use this endpoint to return detailed video metadata for all the
        specified video ids.\r\n\r\nYou'll need an API key and access token to use
        this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key.\r\n\r\nYou can
        show different information in the response by specifying values on the \"fields\"
        parameter (see details below).\r\nYou can search with only an API key, and
        that will give you search results that are equivalent to doing a search on
        the GettyImages.com site without being logged in (anonymous search).  If you
        are a Getty Images API customer and would like to ensure that your API searches
        return only assets that you have a license to use, you need to also include
        an authorization token in the header of your request.  Please consult our
        [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
        for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
        for code examples of getting a token.\r\n\r\n## Working with Fields Sets\r\n\r\nFields
        sets are used in the **fields** request parameter to receive a suite of metadata
        fields. The following fields sets are available:\r\n\r\n#### Summary Fields
        Set\r\n\r\nThe **summary_set** query string parameter fields value represents
        a small batch of metadata fields that are often used to build search response
        results. The following fields are provided for every video in your result
        set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"videos\": \r\n    [\r\n        \"asset_family\",\r\n        \"caption\",\r\n
        \       \"collection_code\",\r\n        \"collection_name\",\r\n        \"display_sizes\":\r\n
        \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
        \           {\r\n                \"name\": \"preview\"\r\n            },\r\n
        \           {\r\n                \"name\": \"thumb\"\r\n            }\r\n
        \       ],\r\n        \"license_model\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields
        value represents a large batch of metadata fields that are often used to build
        a detailed view of videos. The following fields are provided for every video
        in your result set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"videos\": \r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n
        \       \"asset_family\",\r\n        \"caption\",\r\n        \"clip_length\",\r\n
        \       \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n
        \       \"color_type\",\r\n        \"copyright\",\r\n        \"date_created\",\r\n
        \       \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
        \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
        \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n
        \           }\r\n        ],\r\n        \"download_sizes\",\r\n        \"era\",\r\n
        \       \"license_model\",\r\n        \"mastered_to\",\r\n        \"originally_shot_on\",\r\n
        \       \"product_types\",\r\n        \"shot_speed\",\r\n        \"source\",\r\n
        \       \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Display Fields Set\r\n\r\nThe
        **display_set** query string parameter fields value represents the fields
        that provide you with URLs for the low resolution files that are most frequently
        used to build a UI displaying search results. The following fields are provided
        for every video in your result set when you include **display_set** in your
        request.\r\n\r\n```\r\n{\r\n    \"videos\":\r\n    [\r\n        \"display_sizes\":
        \r\n        [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
        \           {\r\n                \"name\": \"preview\"\r\n            },\r\n
        \           {\r\n                \"name\": \"thumb\"\r\n            }\r\n
        \       ]\r\n    ]\r\n}\r\n```\r\n\r\n## Request Usage Considerations\r\n\r\n-
        Specifying the \"entity_details\" response field can have significant performance
        implications. The field should be used only when necessary."
      operationId: Videos_GetBatch
      x-api-path-slug: v3videos-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: Specifies fields to return
      - in: query
        name: ids
        description: Specifies one or more video ids to return
      responses:
        200:
          description: OK
      tags:
      - Images
      - Videos
  /v3/videos/{id}:
    get:
      summary: Get Video Metadatata
      description: "Use this endpoint to return detailed video metadata for the specified
        video id.\r\n\r\nYou'll need an API key and access token to use this resource.
        Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key.\r\n\r\nYou can
        show different information in the response by specifying values on the \"fields\"
        parameter (see details below).\r\nYou can search with only an API key, and
        that will give you search results that are equivalent to doing a search on
        the GettyImages.com site without being logged in (anonymous search).  If you
        are a Getty Images API customer and would like to ensure that your API searches
        return only assets that you have a license to use, you need to also include
        an authorization token in the header of your request.  Please consult our
        [Authorization FAQ](http://developers.gettyimages.com/en/authorization-faq.html)
        for more information on authorization tokens, and our [Authorization Workflows](https://github.com/gettyimages/gettyimages-api/blob/master/OAuth2Workflow.md)
        for code examples of getting a token.\r\n\r\n## Working with Fields Sets\r\n\r\nFields
        sets are used in the **fields** request parameter to receive a suite of metadata
        fields. The following fields sets are available:\r\n\r\n#### Summary Fields
        Set\r\n\r\nThe **summary_set** query string parameter fields value represents
        a small batch of metadata fields that are often used to build search response
        results. The following fields are provided for every video in your result
        set when you include **summary_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"videos\":\r\n    [\r\n        \"asset_family\",\r\n        \"caption\",\r\n
        \       \"collection_code\",\r\n        \"collection_name\",\r\n        \"display_sizes\":\r\n
        \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
        \           {\r\n                \"name\": \"preview\"\r\n            },\r\n
        \           {\r\n                \"name\": \"thumb\"\r\n            }\r\n
        \       ],\r\n        \"license_model\",\r\n        \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n####
        Detail Fields Set\r\n\r\nThe **detail_set** query string parameter fields
        value represents a large batch of metadata fields that are often used to build
        a detailed view of videos. The following fields are provided for every video
        in your result set when you include **detail_set** in your request.\r\n\r\n```\r\n{\r\n
        \   \"videos\":\r\n    [\r\n        \"allowed_use\",\r\n        \"artist\",\r\n
        \       \"asset_family\",\r\n        \"caption\",\r\n        \"clip_length\",\r\n
        \       \"collection_code\",\r\n        \"collection_id\",\r\n        \"collection_name\",\r\n
        \       \"color_type\",\r\n        \"copyright\",\r\n        \"date_created\",\r\n
        \       \"display_sizes\":\r\n        [\r\n            {\r\n                \"name\":
        \"comp\"\r\n            },\r\n            {\r\n                \"name\": \"preview\"\r\n
        \           },\r\n            {\r\n                \"name\": \"thumb\"\r\n
        \           }\r\n        ],\r\n        \"download_sizes\",\r\n        \"era\",\r\n
        \       \"license_model\",\r\n        \"mastered_to\",\r\n        \"originally_shot_on\",\r\n
        \       \"product_types\",\r\n        \"shot_speed\",\r\n        \"source\",\r\n
        \       \"title\"\r\n    ]\r\n}\r\n```\r\n\r\n#### Display Fields Set\r\n\r\nThe
        **display_set** query string parameter fields value represents the fields
        that provide you with URLs for the low resolution files that are most frequently
        used to build a UI displaying search results. The following fields are provided
        for every video in your result set when you include **display_set** in your
        request.\r\n\r\n```\r\n{\r\n    \"videos\":\r\n    [\r\n        \"display_sizes\":\r\n
        \       [\r\n            {\r\n                \"name\": \"comp\"\r\n            },\r\n
        \           {\r\n                \"name\": \"preview\"\r\n            },\r\n
        \           {\r\n                \"name\": \"thumb\"\r\n            }\r\n
        \       ]\r\n    ]\r\n}\r\n```\r\n\r\n## Request Usage Considerations\r\n\r\n-
        Specifying the \"entity_details\" response field can have significant performance
        implications. The field should be used only when necessary."
      operationId: Videos_Get
      x-api-path-slug: v3videosid-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: comma delimited list of fields to retrive for the video
      - in: path
        name: id
        description: A video id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Videos
  /v3/videos/{id}/similar:
    get:
      summary: Get Similar Videos
      description: Get videos similar to a video by supplying one video id
      operationId: Videos_GetSimilarVideos
      x-api-path-slug: v3videosidsimilar-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: comma delimited list of fields to retrive for the videos
      - in: path
        name: id
        description: A video id
      - in: query
        name: page
        description: Identifies page to return
      - in: query
        name: page_size
        description: Specifies page size
      responses:
        200:
          description: OK
      tags:
      - Images
      - Videos
      - Similiar