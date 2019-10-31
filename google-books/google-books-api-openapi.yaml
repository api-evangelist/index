swagger: "2.0"
x-collection-name: Google Books
x-complete: 1
info:
  title: Books
  description: searches-for-books-and-manages-your-google-books-library-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /books/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cloudloading/addBook:
    post:
      summary: Add Book
      description: Adds a book and its contents
      operationId: books.cloudloading.addBook
      x-api-path-slug: cloudloadingaddbook-post
      parameters:
      - in: query
        name: drive_document_id
        description: A drive document id
      - in: query
        name: mime_type
        description: The document MIME type
      - in: query
        name: name
        description: The document name
      - in: query
        name: upload_client_token
      responses:
        200:
          description: OK
      tags:
      - Book
  /cloudloading/deleteBook:
    post:
      summary: Remove Book
      description: Remove the book and its contents
      operationId: books.cloudloading.deleteBook
      x-api-path-slug: cloudloadingdeletebook-post
      parameters:
      - in: query
        name: volumeId
        description: The id of the book to be removed
      responses:
        200:
          description: OK
      tags:
      - Book
  /cloudloading/updateBook:
    post:
      summary: Update Book
      description: Updates a book and its contents
      operationId: books.cloudloading.updateBook
      x-api-path-slug: cloudloadingupdatebook-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Book
  /dictionary/listOfflineMetadata:
    get:
      summary: Get Dictionary
      description: Returns a list of offline dictionary metadata available
      operationId: books.dictionary.listOfflineMetadata
      x-api-path-slug: dictionarylistofflinemetadata-get
      parameters:
      - in: query
        name: cpksver
        description: The device/version ID from which to request the data
      responses:
        200:
          description: OK
      tags:
      - Dictionary
  /myconfig/getUserSettings:
    get:
      summary: Get User Settings
      description: Gets the current settings for the user.
      operationId: books.myconfig.getUserSettings
      x-api-path-slug: myconfiggetusersettings-get
      responses:
        200:
          description: OK
      tags:
      - User
  /myconfig/releaseDownloadAccess:
    post:
      summary: Release Access Restrictions
      description: Release downloaded content access restriction.
      operationId: books.myconfig.releaseDownloadAccess
      x-api-path-slug: myconfigreleasedownloadaccess-post
      parameters:
      - in: query
        name: cpksver
        description: The device/version ID from which to release the restriction
      - in: query
        name: locale
        description: ISO-639-1, ISO-3166-1 codes for message localization, i
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: volumeIds
        description: The volume(s) to release restrictions for
      responses:
        200:
          description: OK
      tags:
      - Access
  /myconfig/requestAccess:
    post:
      summary: Request Access
      description: Request concurrent and download access restrictions.
      operationId: books.myconfig.requestAccess
      x-api-path-slug: myconfigrequestaccess-post
      parameters:
      - in: query
        name: cpksver
        description: The device/version ID from which to request the restrictions
      - in: query
        name: licenseTypes
        description: The type of access license to request
      - in: query
        name: locale
        description: ISO-639-1, ISO-3166-1 codes for message localization, i
      - in: query
        name: nonce
        description: The client nonce value
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: volumeId
        description: The volume to request concurrent/download restrictions for
      responses:
        200:
          description: OK
      tags:
      - Access
  /myconfig/syncVolumeLicenses:
    post:
      summary: Sync Volume Licenses
      description: Request downloaded content access for specified volumes on the
        My eBooks shelf.
      operationId: books.myconfig.syncVolumeLicenses
      x-api-path-slug: myconfigsyncvolumelicenses-post
      parameters:
      - in: query
        name: cpksver
        description: The device/version ID from which to release the restriction
      - in: query
        name: features
        description: List of features supported by the client, i
      - in: query
        name: includeNonComicsSeries
        description: Set to true to include non-comics series
      - in: query
        name: locale
        description: ISO-639-1, ISO-3166-1 codes for message localization, i
      - in: query
        name: nonce
        description: The client nonce value
      - in: query
        name: showPreorders
        description: Set to true to show pre-ordered books
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: volumeIds
        description: The volume(s) to request download restrictions for
      responses:
        200:
          description: OK
      tags:
      - Volume License
  /myconfig/updateUserSettings:
    post:
      summary: Update User Settings
      description: Sets the settings for the user. If a sub-object is specified, it
        will overwrite the existing sub-object stored in the server. Unspecified sub-objects
        will retain the existing value.
      operationId: books.myconfig.updateUserSettings
      x-api-path-slug: myconfigupdateusersettings-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - User
  /mylibrary/annotations:
    get:
      summary: Get Annotations
      description: Retrieves a list of annotations, possibly filtered.
      operationId: books.mylibrary.annotations.list
      x-api-path-slug: mylibraryannotations-get
      parameters:
      - in: query
        name: contentVersion
        description: The content version for the requested volume
      - in: query
        name: layerId
        description: The layer ID to limit annotation by
      - in: query
        name: layerIds
        description: The layer ID(s) to limit annotation by
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous page
      - in: query
        name: showDeleted
        description: Set to true to return deleted annotations
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: updatedMax
        description: RFC 3339 timestamp to restrict to items updated prior to this
          timestamp (exclusive)
      - in: query
        name: updatedMin
        description: RFC 3339 timestamp to restrict to items updated since this timestamp
          (inclusive)
      - in: query
        name: volumeId
        description: The volume to restrict annotations to
      responses:
        200:
          description: OK
      tags:
      - Annotation
    post:
      summary: insert Annotation
      description: Inserts a new annotation.
      operationId: books.mylibrary.annotations.insert
      x-api-path-slug: mylibraryannotations-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: country
        description: ISO-3166-1 code to override the IP-based location
      - in: query
        name: showOnlySummaryInResponse
        description: Requests that only the summary of the specified layer be provided
          in the response
      - in: query
        name: source
        description: String to identify the originator of this request
      responses:
        200:
          description: OK
      tags:
      - Annotation
  /mylibrary/annotations/summary:
    post:
      summary: Get Annotation
      description: Gets the summary of specified layers.
      operationId: books.mylibrary.annotations.summary
      x-api-path-slug: mylibraryannotationssummary-post
      parameters:
      - in: query
        name: layerIds
        description: Array of layer IDs to get the summary for
      - in: query
        name: volumeId
        description: Volume id to get the summary for
      responses:
        200:
          description: OK
      tags:
      - Annotation
  /mylibrary/annotations/{annotationId}:
    delete:
      summary: Delete Annotation
      description: Deletes an annotation.
      operationId: books.mylibrary.annotations.delete
      x-api-path-slug: mylibraryannotationsannotationid-delete
      parameters:
      - in: path
        name: annotationId
        description: The ID for the annotation to delete
      - in: query
        name: source
        description: String to identify the originator of this request
      responses:
        200:
          description: OK
      tags:
      - Annotation
    put:
      summary: Update Annotation
      description: Updates an existing annotation.
      operationId: books.mylibrary.annotations.update
      x-api-path-slug: mylibraryannotationsannotationid-put
      parameters:
      - in: path
        name: annotationId
        description: The ID for the annotation to update
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: source
        description: String to identify the originator of this request
      responses:
        200:
          description: OK
      tags:
      - Annotation
  /mylibrary/bookshelves:
    get:
      summary: Get Bookshelves
      description: Retrieves a list of bookshelves belonging to the authenticated
        user.
      operationId: books.mylibrary.bookshelves.list
      x-api-path-slug: mylibrarybookshelves-get
      parameters:
      - in: query
        name: source
        description: String to identify the originator of this request
      responses:
        200:
          description: OK
      tags:
      - Bookshelf
  /mylibrary/bookshelves/{shelf}:
    get:
      summary: Get Bookshelf
      description: Retrieves metadata for a specific bookshelf belonging to the authenticated
        user.
      operationId: books.mylibrary.bookshelves.get
      x-api-path-slug: mylibrarybookshelvesshelf-get
      parameters:
      - in: path
        name: shelf
        description: ID of bookshelf to retrieve
      - in: query
        name: source
        description: String to identify the originator of this request
      responses:
        200:
          description: OK
      tags:
      - Bookshelf
  /mylibrary/bookshelves/{shelf}/addVolume:
    post:
      summary: Add Volume
      description: Adds a volume to a bookshelf.
      operationId: books.mylibrary.bookshelves.addVolume
      x-api-path-slug: mylibrarybookshelvesshelfaddvolume-post
      parameters:
      - in: query
        name: reason
        description: The reason for which the book is added to the library
      - in: path
        name: shelf
        description: ID of bookshelf to which to add a volume
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: volumeId
        description: ID of volume to add
      responses:
        200:
          description: OK
      tags:
      - Volume
  /mylibrary/bookshelves/{shelf}/clearVolumes:
    post:
      summary: Clear Volumes
      description: Clears all volumes from a bookshelf.
      operationId: books.mylibrary.bookshelves.clearVolumes
      x-api-path-slug: mylibrarybookshelvesshelfclearvolumes-post
      parameters:
      - in: path
        name: shelf
        description: ID of bookshelf from which to remove a volume
      - in: query
        name: source
        description: String to identify the originator of this request
      responses:
        200:
          description: OK
      tags:
      - Volume
  /mylibrary/bookshelves/{shelf}/moveVolume:
    post:
      summary: Move Voume
      description: Moves a volume within a bookshelf.
      operationId: books.mylibrary.bookshelves.moveVolume
      x-api-path-slug: mylibrarybookshelvesshelfmovevolume-post
      parameters:
      - in: path
        name: shelf
        description: ID of bookshelf with the volume
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: volumeId
        description: ID of volume to move
      - in: query
        name: volumePosition
        description: Position on shelf to move the item (0 puts the item before the
          current first item, 1 puts it between the first and the second and so on
      responses:
        200:
          description: OK
      tags:
      - Volume
  /mylibrary/bookshelves/{shelf}/removeVolume:
    post:
      summary: Remove Volume
      description: Removes a volume from a bookshelf.
      operationId: books.mylibrary.bookshelves.removeVolume
      x-api-path-slug: mylibrarybookshelvesshelfremovevolume-post
      parameters:
      - in: query
        name: reason
        description: The reason for which the book is removed from the library
      - in: path
        name: shelf
        description: ID of bookshelf from which to remove a volume
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: volumeId
        description: ID of volume to remove
      responses:
        200:
          description: OK
      tags:
      - Volume
  /mylibrary/bookshelves/{shelf}/volumes:
    get:
      summary: Get Volume
      description: Gets volume information for volumes on a bookshelf.
      operationId: books.mylibrary.bookshelves.volumes.list
      x-api-path-slug: mylibrarybookshelvesshelfvolumes-get
      parameters:
      - in: query
        name: country
        description: ISO-3166-1 code to override the IP-based location
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: projection
        description: Restrict information returned to a set of selected fields
      - in: query
        name: q
        description: Full-text search query string in this bookshelf
      - in: path
        name: shelf
        description: The bookshelf ID or name retrieve volumes for
      - in: query
        name: showPreorders
        description: Set to true to show pre-ordered books
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: startIndex
        description: Index of the first element to return (starts at 0)
      responses:
        200:
          description: OK
      tags:
      - Volume
  /mylibrary/readingpositions/{volumeId}:
    get:
      summary: Get Reading Position
      description: Retrieves my reading position information for a volume.
      operationId: books.mylibrary.readingpositions.get
      x-api-path-slug: mylibraryreadingpositionsvolumeid-get
      parameters:
      - in: query
        name: contentVersion
        description: Volume content version for which this reading position is requested
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: path
        name: volumeId
        description: ID of volume for which to retrieve a reading position
      responses:
        200:
          description: OK
      tags:
      - Reading Position
  /mylibrary/readingpositions/{volumeId}/setPosition:
    post:
      summary: Set Reading Position
      description: Sets my reading position information for a volume.
      operationId: books.mylibrary.readingpositions.setPosition
      x-api-path-slug: mylibraryreadingpositionsvolumeidsetposition-post
      parameters:
      - in: query
        name: action
        description: Action that caused this reading position to be set
      - in: query
        name: contentVersion
        description: Volume content version for which this reading position applies
      - in: query
        name: deviceCookie
        description: Random persistent device cookie optional on set position
      - in: query
        name: position
        description: Position string for the new volume reading position
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: timestamp
        description: RFC 3339 UTC format timestamp associated with this reading position
      - in: path
        name: volumeId
        description: ID of volume for which to update the reading position
      responses:
        200:
          description: OK
      tags:
      - Reading Position
  /notification/get:
    get:
      summary: Get Notification
      description: Returns notification details for a given notification id.
      operationId: books.notification.get
      x-api-path-slug: notificationget-get
      parameters:
      - in: query
        name: locale
        description: ISO-639-1 language and ISO-3166-1 country code
      - in: query
        name: notification_id
        description: String to identify the notification
      - in: query
        name: source
        description: String to identify the originator of this request
      responses:
        200:
          description: OK
      tags:
      - Notification
  /onboarding/listCategories:
    get:
      summary: List Categoies
      description: List categories for onboarding experience.
      operationId: books.onboarding.listCategories
      x-api-path-slug: onboardinglistcategories-get
      parameters:
      - in: query
        name: locale
        description: ISO-639-1 language and ISO-3166-1 country code
      responses:
        200:
          description: OK
      tags:
      - Category
  /onboarding/listCategoryVolumes:
    get:
      summary: List Volumes
      description: List available volumes under categories for onboarding experience.
      operationId: books.onboarding.listCategoryVolumes
      x-api-path-slug: onboardinglistcategoryvolumes-get
      parameters:
      - in: query
        name: categoryId
        description: List of category ids requested
      - in: query
        name: locale
        description: ISO-639-1 language and ISO-3166-1 country code
      - in: query
        name: maxAllowedMaturityRating
        description: The maximum allowed maturity rating of returned volumes
      - in: query
        name: pageSize
        description: Number of maximum results per page to be included in the response
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous page
      responses:
        200:
          description: OK
      tags:
      - Volue
  /personalizedstream/get:
    get:
      summary: Get Stream
      description: Returns a stream of personalized book clusters
      operationId: books.personalizedstream.get
      x-api-path-slug: personalizedstreamget-get
      parameters:
      - in: query
        name: locale
        description: ISO-639-1 language and ISO-3166-1 country code
      - in: query
        name: maxAllowedMaturityRating
        description: The maximum allowed maturity rating of returned recommendations
      - in: query
        name: source
        description: String to identify the originator of this request
      responses:
        200:
          description: OK
      tags:
      - Stream
  /promooffer/accept:
    post:
      summary: Accept Promotion Offer
      description: Accept promotion offer
      operationId: books.promooffer.accept
      x-api-path-slug: promoofferaccept-post
      parameters:
      - in: query
        name: androidId
        description: device android_id
      - in: query
        name: device
        description: device device
      - in: query
        name: manufacturer
        description: device manufacturer
      - in: query
        name: model
        description: device model
      - in: query
        name: offerId
      - in: query
        name: product
        description: device product
      - in: query
        name: serial
        description: device serial
      - in: query
        name: volumeId
        description: Volume id to exercise the offer
      responses:
        200:
          description: OK
      tags:
      - Promotion
  /promooffer/dismiss:
    post:
      summary: Dismiss Promotion Offer
      description: Dismiss promotion offer
      operationId: books.promooffer.dismiss
      x-api-path-slug: promoofferdismiss-post
      parameters:
      - in: query
        name: androidId
        description: device android_id
      - in: query
        name: device
        description: device device
      - in: query
        name: manufacturer
        description: device manufacturer
      - in: query
        name: model
        description: device model
      - in: query
        name: offerId
        description: Offer to dimiss
      - in: query
        name: product
        description: device product
      - in: query
        name: serial
        description: device serial
      responses:
        200:
          description: OK
      tags:
      - Promotion
  /promooffer/get:
    get:
      summary: Get Promotion Offer
      description: Returns a list of promo offers available to the user
      operationId: books.promooffer.get
      x-api-path-slug: promoofferget-get
      parameters:
      - in: query
        name: androidId
        description: device android_id
      - in: query
        name: device
        description: device device
      - in: query
        name: manufacturer
        description: device manufacturer
      - in: query
        name: model
        description: device model
      - in: query
        name: product
        description: device product
      - in: query
        name: serial
        description: device serial
      responses:
        200:
          description: OK
      tags:
      - Promotion
  /series/get:
    get:
      summary: Get Series
      description: Returns Series metadata for the given series ids.
      operationId: books.series.get
      x-api-path-slug: seriesget-get
      parameters:
      - in: query
        name: series_id
        description: String that identifies the series
      responses:
        200:
          description: OK
      tags:
      - Series
  /series/membership/get:
    get:
      summary: Get Series Membership
      description: Returns Series membership data given the series id.
      operationId: books.series.membership.get
      x-api-path-slug: seriesmembershipget-get
      parameters:
      - in: query
        name: page_size
        description: Number of maximum results per page to be included in the response
      - in: query
        name: page_token
        description: The value of the nextToken from the previous page
      - in: query
        name: series_id
        description: String that identifies the series
      responses:
        200:
          description: OK
      tags:
      - Series
  /users/{userId}/bookshelves:
    get:
      summary: Get Public Bookkshelves
      description: Retrieves a list of public bookshelves for the specified user.
      operationId: books.bookshelves.list
      x-api-path-slug: usersuseridbookshelves-get
      parameters:
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: path
        name: userId
        description: ID of user for whom to retrieve bookshelves
      responses:
        200:
          description: OK
      tags:
      - Bookshelf
  /users/{userId}/bookshelves/{shelf}:
    get:
      summary: Get Public Bookshelf
      description: Retrieves metadata for a specific bookshelf for the specified user.
      operationId: books.bookshelves.get
      x-api-path-slug: usersuseridbookshelvesshelf-get
      parameters:
      - in: path
        name: shelf
        description: ID of bookshelf to retrieve
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: path
        name: userId
        description: ID of user for whom to retrieve bookshelves
      responses:
        200:
          description: OK
      tags:
      - Bookshelf
  /users/{userId}/bookshelves/{shelf}/volumes:
    get:
      summary: Get Public Volumes
      description: Retrieves volumes in a specific bookshelf for the specified user.
      operationId: books.bookshelves.volumes.list
      x-api-path-slug: usersuseridbookshelvesshelfvolumes-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: path
        name: shelf
        description: ID of bookshelf to retrieve volumes
      - in: query
        name: showPreorders
        description: Set to true to show pre-ordered books
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: startIndex
        description: Index of the first element to return (starts at 0)
      - in: path
        name: userId
        description: ID of user for whom to retrieve bookshelf volumes
      responses:
        200:
          description: OK
      tags:
      - Volume
  /volumes:
    get:
      summary: Book Search
      description: Performs a book search.
      operationId: books.volumes.list
      x-api-path-slug: volumes-get
      parameters:
      - in: query
        name: download
        description: Restrict to volumes by download availability
      - in: query
        name: filter
        description: Filter search results
      - in: query
        name: langRestrict
        description: Restrict results to books with this language code
      - in: query
        name: libraryRestrict
        description: Restrict search to this users library
      - in: query
        name: maxAllowedMaturityRating
        description: The maximum allowed maturity rating of returned recommendations
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: orderBy
        description: Sort search results
      - in: query
        name: partner
        description: Restrict and brand results for partner ID
      - in: query
        name: printType
        description: Restrict to books or magazines
      - in: query
        name: projection
        description: Restrict information returned to a set of selected fields
      - in: query
        name: q
        description: Full-text search query string
      - in: query
        name: showPreorders
        description: Set to true to show books available for preorder
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: startIndex
        description: Index of the first result to return (starts at 0)
      responses:
        200:
          description: OK
      tags:
      - Search
  /volumes/mybooks:
    get:
      summary: Get My Books
      description: Return a list of books in My Library.
      operationId: books.volumes.mybooks.list
      x-api-path-slug: volumesmybooks-get
      parameters:
      - in: query
        name: acquireMethod
        description: How the book was acquired
      - in: query
        name: country
        description: ISO-3166-1 code to override the IP-based location
      - in: query
        name: locale
        description: ISO-639-1 language and ISO-3166-1 country code
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: processingState
        description: The processing state of the user uploaded volumes to be returned
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: startIndex
        description: Index of the first result to return (starts at 0)
      responses:
        200:
          description: OK
      tags:
      - Book
  /volumes/recommended:
    get:
      summary: Get Recommend
      description: Return a list of recommended books for the current user.
      operationId: books.volumes.recommended.list
      x-api-path-slug: volumesrecommended-get
      parameters:
      - in: query
        name: locale
        description: ISO-639-1 language and ISO-3166-1 country code
      - in: query
        name: maxAllowedMaturityRating
        description: The maximum allowed maturity rating of returned recommendations
      - in: query
        name: source
        description: String to identify the originator of this request
      responses:
        200:
          description: OK
      tags:
      - Recommended
  /volumes/recommended/rate:
    post:
      summary: Rate Recommend
      description: Rate a recommended book for the current user.
      operationId: books.volumes.recommended.rate
      x-api-path-slug: volumesrecommendedrate-post
      parameters:
      - in: query
        name: locale
        description: ISO-639-1 language and ISO-3166-1 country code
      - in: query
        name: rating
        description: Rating to be given to the volume
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: volumeId
        description: ID of the source volume
      responses:
        200:
          description: OK
      tags:
      - Recommended
  /volumes/useruploaded:
    get:
      summary: Get Uploaded
      description: Return a list of books uploaded by the current user.
      operationId: books.volumes.useruploaded.list
      x-api-path-slug: volumesuseruploaded-get
      parameters:
      - in: query
        name: locale
        description: ISO-639-1 language and ISO-3166-1 country code
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: processingState
        description: The processing state of the user uploaded volumes to be returned
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: startIndex
        description: Index of the first result to return (starts at 0)
      - in: query
        name: volumeId
        description: The ids of the volumes to be returned
      responses:
        200:
          description: OK
      tags:
      - Upload
  /volumes/{volumeId}:
    get:
      summary: Get Volume
      description: Gets volume information for a single volume.
      operationId: books.volumes.get
      x-api-path-slug: volumesvolumeid-get
      parameters:
      - in: query
        name: country
        description: ISO-3166-1 code to override the IP-based location
      - in: query
        name: includeNonComicsSeries
        description: Set to true to include non-comics series
      - in: query
        name: partner
        description: Brand results for partner ID
      - in: query
        name: projection
        description: Restrict information returned to a set of selected fields
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: user_library_consistent_read
      - in: path
        name: volumeId
        description: ID of volume to retrieve
      responses:
        200:
          description: OK
      tags:
      - Volume
  /volumes/{volumeId}/associated:
    get:
      summary: Get Associated
      description: Return a list of associated books.
      operationId: books.volumes.associated.list
      x-api-path-slug: volumesvolumeidassociated-get
      parameters:
      - in: query
        name: association
        description: Association type
      - in: query
        name: locale
        description: ISO-639-1 language and ISO-3166-1 country code
      - in: query
        name: maxAllowedMaturityRating
        description: The maximum allowed maturity rating of returned recommendations
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: path
        name: volumeId
        description: ID of the source volume
      responses:
        200:
          description: OK
      tags:
      - Associated
  /volumes/{volumeId}/layers/{layerId}:
    get:
      summary: Get Volume Annotations
      description: Gets the volume annotations for a volume and layer.
      operationId: books.layers.volumeAnnotations.list
      x-api-path-slug: volumesvolumeidlayerslayerid-get
      parameters:
      - in: query
        name: contentVersion
        description: The content version for the requested volume
      - in: query
        name: endOffset
        description: The end offset to end retrieving data from
      - in: query
        name: endPosition
        description: The end position to end retrieving data from
      - in: path
        name: layerId
        description: The ID for the layer to get the annotations
      - in: query
        name: locale
        description: The locale information for the data
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous page
      - in: query
        name: showDeleted
        description: Set to true to return deleted annotations
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: startOffset
        description: The start offset to start retrieving data from
      - in: query
        name: startPosition
        description: The start position to start retrieving data from
      - in: query
        name: updatedMax
        description: RFC 3339 timestamp to restrict to items updated prior to this
          timestamp (exclusive)
      - in: query
        name: updatedMin
        description: RFC 3339 timestamp to restrict to items updated since this timestamp
          (inclusive)
      - in: query
        name: volumeAnnotationsVersion
        description: The version of the volume annotations that you are requesting
      - in: path
        name: volumeId
        description: The volume to retrieve annotations for
      responses:
        200:
          description: OK
      tags:
      - Annotation
  /volumes/{volumeId}/layers/{layerId}/annotations/{annotationId}:
    get:
      summary: Get Volume Annotion
      description: Gets the volume annotation.
      operationId: books.layers.volumeAnnotations.get
      x-api-path-slug: volumesvolumeidlayerslayeridannotationsannotationid-get
      parameters:
      - in: path
        name: annotationId
        description: The ID of the volume annotation to retrieve
      - in: path
        name: layerId
        description: The ID for the layer to get the annotations
      - in: query
        name: locale
        description: The locale information for the data
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: path
        name: volumeId
        description: The volume to retrieve annotations for
      responses:
        200:
          description: OK
      tags:
      - Annotation
  /volumes/{volumeId}/layers/{layerId}/data:
    get:
      summary: Get Annotations
      description: Gets the annotation data for a volume and layer.
      operationId: books.layers.annotationData.list
      x-api-path-slug: volumesvolumeidlayerslayeriddata-get
      parameters:
      - in: query
        name: annotationDataId
        description: The list of Annotation Data Ids to retrieve
      - in: query
        name: contentVersion
        description: The content version for the requested volume
      - in: query
        name: h
        description: The requested pixel height for any images
      - in: path
        name: layerId
        description: The ID for the layer to get the annotation data
      - in: query
        name: locale
        description: The locale information for the data
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous page
      - in: query
        name: scale
        description: The requested scale for the image
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: query
        name: updatedMax
        description: RFC 3339 timestamp to restrict to items updated prior to this
          timestamp (exclusive)
      - in: query
        name: updatedMin
        description: RFC 3339 timestamp to restrict to items updated since this timestamp
          (inclusive)
      - in: path
        name: volumeId
        description: The volume to retrieve annotation data for
      - in: query
        name: w
        description: The requested pixel width for any images
      responses:
        200:
          description: OK
      tags:
      - Annotation
  /volumes/{volumeId}/layers/{layerId}/data/{annotationDataId}:
    get:
      summary: Get Annotation
      description: Gets the annotation data.
      operationId: books.layers.annotationData.get
      x-api-path-slug: volumesvolumeidlayerslayeriddataannotationdataid-get
      parameters:
      - in: query
        name: allowWebDefinitions
        description: For the dictionary layer
      - in: path
        name: annotationDataId
        description: The ID of the annotation data to retrieve
      - in: query
        name: contentVersion
        description: The content version for the volume you are trying to retrieve
      - in: query
        name: h
        description: The requested pixel height for any images
      - in: path
        name: layerId
        description: The ID for the layer to get the annotations
      - in: query
        name: locale
        description: The locale information for the data
      - in: query
        name: scale
        description: The requested scale for the image
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: path
        name: volumeId
        description: The volume to retrieve annotations for
      - in: query
        name: w
        description: The requested pixel width for any images
      responses:
        200:
          description: OK
      tags:
      - Annotation
  /volumes/{volumeId}/layersummary:
    get:
      summary: Get Layers
      description: List the layer summaries for a volume.
      operationId: books.layers.list
      x-api-path-slug: volumesvolumeidlayersummary-get
      parameters:
      - in: query
        name: contentVersion
        description: The content version for the requested volume
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous page
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: path
        name: volumeId
        description: The volume to retrieve layers for
      responses:
        200:
          description: OK
      tags:
      - Layer
  /volumes/{volumeId}/layersummary/{summaryId}:
    get:
      summary: Get Layer
      description: Gets the layer summary for a volume.
      operationId: books.layers.get
      x-api-path-slug: volumesvolumeidlayersummarysummaryid-get
      parameters:
      - in: query
        name: contentVersion
        description: The content version for the requested volume
      - in: query
        name: source
        description: String to identify the originator of this request
      - in: path
        name: summaryId
        description: The ID for the layer to get the summary for
      - in: path
        name: volumeId
        description: The volume to retrieve layers for
      responses:
        200:
          description: OK
      tags:
      - Layer