swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{packageName}/edits:
    post:
      summary: Create App Edit
      description: Creates a new edit for an app, populated with the app's current
        state.
      operationId: androidpublisher.edits.insert
      x-api-path-slug: packagenameedits-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Application
  /{packageName}/edits/{editId}:
    delete:
      summary: Delete App Edit
      description: Deletes an edit for an app. Creating a new edit will automatically
        delete any of your previous edits so this method need only be called if you
        want to preemptively abandon an edit.
      operationId: androidpublisher.edits.delete
      x-api-path-slug: packagenameeditseditid-delete
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Application
    get:
      summary: DGetelete App Edit
      description: Returns information about the edit specified. Calls will fail if
        the edit is no long active (e.g. has been deleted, superseded or expired).
      operationId: androidpublisher.edits.get
      x-api-path-slug: packagenameeditseditid-get
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Application
  /{packageName}/edits/{editId}/apks/externallyHosted:
    post:
      summary: Create APK
      description: Creates a new APK without uploading the APK itself to Google Play,
        instead hosting the APK at a specified URL. This function is only available
        to enterprises using Google Play for Work whose application is configured
        to restrict distribution to the enterprise domain.
      operationId: androidpublisher.edits.apks.addexternallyhosted
      x-api-path-slug: packagenameeditseditidapksexternallyhosted-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Application
  /{packageName}/edits/{editId}/apks/{apkVersionCode}/deobfuscationFiles/{deobfuscationFileType}:
    post:
      summary: Update Deobfuscation FIle
      description: Uploads the deobfuscation file of the specified APK. If a deobfuscation
        file already exists, it will be replaced.
      operationId: androidpublisher.edits.deobfuscationfiles.upload
      x-api-path-slug: packagenameeditseditidapksapkversioncodedeobfuscationfilesdeobfuscationfiletype-post
      parameters:
      - in: path
        name: apkVersionCode
        description: The version code of the APK whose deobfuscation file is being
          uploaded
      - in: path
        name: deobfuscationFileType
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier of the Android app for which the deobfuscatiuon
          files are being uploaded; for example, com
      responses:
        200:
          description: OK
      tags:
      - Deobfuscation FIle
  /{packageName}/edits/{editId}/apks/{apkVersionCode}/expansionFiles/{expansionFileType}:
    get:
      summary: Get Expansion File
      description: Fetches the Expansion File configuration for the APK specified.
      operationId: androidpublisher.edits.expansionfiles.get
      x-api-path-slug: packagenameeditseditidapksapkversioncodeexpansionfilesexpansionfiletype-get
      parameters:
      - in: path
        name: apkVersionCode
        description: The version code of the APK whose Expansion File configuration
          is being read or modified
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: expansionFileType
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Expansion File
    patch:
      summary: Update APK Expansion File
      description: Updates the APK's Expansion File configuration to reference another
        APK's Expansion Files. To add a new Expansion File use the Upload method.
        This method supports patch semantics.
      operationId: androidpublisher.edits.expansionfiles.patch
      x-api-path-slug: packagenameeditseditidapksapkversioncodeexpansionfilesexpansionfiletype-patch
      parameters:
      - in: path
        name: apkVersionCode
        description: The version code of the APK whose Expansion File configuration
          is being read or modified
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: expansionFileType
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - APK Expansion File
    post:
      summary: Upload APK Expansion File
      description: Uploads and attaches a new Expansion File to the APK specified.
      operationId: androidpublisher.edits.expansionfiles.upload
      x-api-path-slug: packagenameeditseditidapksapkversioncodeexpansionfilesexpansionfiletype-post
      parameters:
      - in: path
        name: apkVersionCode
        description: The version code of the APK whose Expansion File configuration
          is being read or modified
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: expansionFileType
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - APK Expansion File
    put:
      summary: Update APK Expansion File
      description: Updates the APK's Expansion File configuration to reference another
        APK's Expansion Files. To add a new Expansion File use the Upload method.
      operationId: androidpublisher.edits.expansionfiles.update
      x-api-path-slug: packagenameeditseditidapksapkversioncodeexpansionfilesexpansionfiletype-put
      parameters:
      - in: path
        name: apkVersionCode
        description: The version code of the APK whose Expansion File configuration
          is being read or modified
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: expansionFileType
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - APK Expansion File
  /{packageName}/edits/{editId}/apks/{apkVersionCode}/listings:
    delete:
      summary: Delete All APK Localized Listing
      description: Deletes all the APK-specific localized listings for a specified
        APK.
      operationId: androidpublisher.edits.apklistings.deleteall
      x-api-path-slug: packagenameeditseditidapksapkversioncodelistings-delete
      parameters:
      - in: path
        name: apkVersionCode
        description: The APK version code whose APK-specific listings should be read
          or modified
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - APK Localized Listing
    get:
      summary: Get APK Localized Listings
      description: Lists all the APK-specific localized listings for a specified APK.
      operationId: androidpublisher.edits.apklistings.list
      x-api-path-slug: packagenameeditseditidapksapkversioncodelistings-get
      parameters:
      - in: path
        name: apkVersionCode
        description: The APK version code whose APK-specific listings should be read
          or modified
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - APK Localized Listing
  /{packageName}/edits/{editId}/apks/{apkVersionCode}/listings/{language}:
    delete:
      summary: Delete APK Localized Listing
      description: Deletes the APK-specific localized listing for a specified APK
        and language code.
      operationId: androidpublisher.edits.apklistings.delete
      x-api-path-slug: packagenameeditseditidapksapkversioncodelistingslanguage-delete
      parameters:
      - in: path
        name: apkVersionCode
        description: The APK version code whose APK-specific listings should be read
          or modified
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: language
        description: The language code (a BCP-47 language tag) of the APK-specific
          localized listing to read or modify
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - APK Localized Listing
    get:
      summary: Get APK Localized Listing
      description: Fetches the APK-specific localized listing for a specified APK
        and language code.
      operationId: androidpublisher.edits.apklistings.get
      x-api-path-slug: packagenameeditseditidapksapkversioncodelistingslanguage-get
      parameters:
      - in: path
        name: apkVersionCode
        description: The APK version code whose APK-specific listings should be read
          or modified
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: language
        description: The language code (a BCP-47 language tag) of the APK-specific
          localized listing to read or modify
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - APK Localized Listing
    patch:
      summary: Update APK Localized Listing
      description: Updates or creates the APK-specific localized listing for a specified
        APK and language code. This method supports patch semantics.
      operationId: androidpublisher.edits.apklistings.patch
      x-api-path-slug: packagenameeditseditidapksapkversioncodelistingslanguage-patch
      parameters:
      - in: path
        name: apkVersionCode
        description: The APK version code whose APK-specific listings should be read
          or modified
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: language
        description: The language code (a BCP-47 language tag) of the APK-specific
          localized listing to read or modify
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - APK Localized Listing
    put:
      summary: Update APK Localized Listing
      description: Updates or creates the APK-specific localized listing for a specified
        APK and language code.
      operationId: androidpublisher.edits.apklistings.update
      x-api-path-slug: packagenameeditseditidapksapkversioncodelistingslanguage-put
      parameters:
      - in: path
        name: apkVersionCode
        description: The APK version code whose APK-specific listings should be read
          or modified
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: language
        description: The language code (a BCP-47 language tag) of the APK-specific
          localized listing to read or modify
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - APK Localized Listing
  /{packageName}/edits/{editId}/details:
    get:
      summary: Get App Detail
      description: Fetches app details for this edit. This includes the default language
        and developer support contact information.
      operationId: androidpublisher.edits.details.get
      x-api-path-slug: packagenameeditseditiddetails-get
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Application
    patch:
      summary: Update App Detail
      description: Updates app details for this edit. This method supports patch semantics.
      operationId: androidpublisher.edits.details.patch
      x-api-path-slug: packagenameeditseditiddetails-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Application
    put:
      summary: Update App Detail
      description: Updates app details for this edit.
      operationId: androidpublisher.edits.details.update
      x-api-path-slug: packagenameeditseditiddetails-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Application
  /{packageName}/edits/{editId}/listings:
    delete:
      summary: Delete App Detail
      description: Deletes all localized listings from an edit.
      operationId: androidpublisher.edits.listings.deleteall
      x-api-path-slug: packagenameeditseditidlistings-delete
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Application
    get:
      summary: Get App Details
      description: Returns all of the localized store listings attached to this edit.
      operationId: androidpublisher.edits.listings.list
      x-api-path-slug: packagenameeditseditidlistings-get
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Application
  /{packageName}/edits/{editId}/listings/{language}:
    delete:
      summary: Delete Localized Store Listing
      description: Deletes the specified localized store listing from an edit.
      operationId: androidpublisher.edits.listings.delete
      x-api-path-slug: packagenameeditseditidlistingslanguage-delete
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: language
        description: The language code (a BCP-47 language tag) of the localized listing
          to read or modify
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Localized Store Listing
    get:
      summary: Get Localized Store Listing
      description: Fetches information about a localized store listing.
      operationId: androidpublisher.edits.listings.get
      x-api-path-slug: packagenameeditseditidlistingslanguage-get
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: language
        description: The language code (a BCP-47 language tag) of the localized listing
          to read or modify
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Localized Store Listing
    patch:
      summary: Update Localized Store Listing
      description: Creates or updates a localized store listing. This method supports
        patch semantics.
      operationId: androidpublisher.edits.listings.patch
      x-api-path-slug: packagenameeditseditidlistingslanguage-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: language
        description: The language code (a BCP-47 language tag) of the localized listing
          to read or modify
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Localized Store Listing
    put:
      summary: Update Localized Store Listing
      description: Creates or updates a localized store listing.
      operationId: androidpublisher.edits.listings.update
      x-api-path-slug: packagenameeditseditidlistingslanguage-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: language
        description: The language code (a BCP-47 language tag) of the localized listing
          to read or modify
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Localized Store Listing
  /{packageName}/edits/{editId}/listings/{language}/{imageType}:
    delete:
      summary: Delete All Images
      description: Deletes all images for the specified language and image type.
      operationId: androidpublisher.edits.images.deleteall
      x-api-path-slug: packagenameeditseditidlistingslanguageimagetype-delete
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: imageType
      - in: path
        name: language
        description: The language code (a BCP-47 language tag) of the localized listing
          whose images are to read or modified
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Image
    get:
      summary: Get All Images
      description: Lists all images for the specified language and image type.
      operationId: androidpublisher.edits.images.list
      x-api-path-slug: packagenameeditseditidlistingslanguageimagetype-get
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: imageType
      - in: path
        name: language
        description: The language code (a BCP-47 language tag) of the localized listing
          whose images are to read or modified
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Image
    post:
      summary: Upoads Image
      description: Uploads a new image and adds it to the list of images for the specified
        language and image type.
      operationId: androidpublisher.edits.images.upload
      x-api-path-slug: packagenameeditseditidlistingslanguageimagetype-post
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: imageType
      - in: path
        name: language
        description: The language code (a BCP-47 language tag) of the localized listing
          whose images are to read or modified
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Image
  /enterprises:
    get:
      summary: Get Enterprises
      description: Looks up an enterprise by domain name. This is only supported for
        enterprises created via the Google-initiated creation flow. Lookup of the
        id is not needed for enterprises created via the EMM-initiated flow since
        the EMM learns the enterprise ID in the callback specified in the Enterprises.generateSignupUrl
        call.
      operationId: androidenterprise.enterprises.list
      x-api-path-slug: enterprises-get
      parameters:
      - in: query
        name: domain
        description: The exact primary domain name of the enterprise to look up
      responses:
        200:
          description: OK
      tags:
      - Enterprise
    post:
      summary: Create Enterprise
      description: Establishes the binding between the EMM and an enterprise. This
        is now deprecated; use enroll instead.
      operationId: androidenterprise.enterprises.insert
      x-api-path-slug: enterprises-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: token
        description: The token provided by the enterprise to register the EMM
      responses:
        200:
          description: OK
      tags:
      - Enterprise
  /enterprises/acknowledgeNotificationSet:
    post:
      summary: Create Acknowledges Notification Set
      description: Acknowledges notifications that were received from Enterprises.PullNotificationSet
        to prevent subsequent calls from returning the same notifications.
      operationId: androidenterprise.enterprises.acknowledgeNotificationSet
      x-api-path-slug: enterprisesacknowledgenotificationset-post
      parameters:
      - in: query
        name: notificationSetId
        description: The notification set ID as returned by Enterprises
      responses:
        200:
          description: OK
      tags:
      - Notification
  /enterprises/completeSignup:
    post:
      summary: Complete Signup Flow
      description: Completes the signup flow, by specifying the Completion token and
        Enterprise token. This request must not be called multiple times for a given
        Enterprise Token.
      operationId: androidenterprise.enterprises.completeSignup
      x-api-path-slug: enterprisescompletesignup-post
      parameters:
      - in: query
        name: completionToken
        description: The Completion token initially returned by GenerateSignupUrl
      - in: query
        name: enterpriseToken
        description: The Enterprise token appended to the Callback URL
      responses:
        200:
          description: OK
      tags:
      - Signup
  /{packageName}/edits/{editId}/listings/{language}/{imageType}/{imageId}:
    delete:
      summary: Delete Image
      description: Deletes the image (specified by id) from the edit.
      operationId: androidpublisher.edits.images.delete
      x-api-path-slug: packagenameeditseditidlistingslanguageimagetypeimageid-delete
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: imageId
        description: Unique identifier an image within the set of images attached
          to this edit
      - in: path
        name: imageType
      - in: path
        name: language
        description: The language code (a BCP-47 language tag) of the localized listing
          whose images are to read or modified
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Image
  /enterprises/enroll:
    post:
      summary: Entroll Enterprise
      description: Enrolls an enterprise with the calling EMM.
      operationId: androidenterprise.enterprises.enroll
      x-api-path-slug: enterprisesenroll-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: token
        description: The token provided by the enterprise to register the EMM
      responses:
        200:
          description: OK
      tags:
      - Enroll
  /enterprises/pullNotificationSet:
    post:
      summary: Get Notification Set
      description: |-
        Pulls and returns a notification set for the enterprises associated with the service account authenticated for the request. The notification set may be empty if no notification are pending.
        A notification set returned needs to be acknowledged within 20 seconds by calling Enterprises.AcknowledgeNotificationSet, unless the notification set is empty.
        Notifications that are not acknowledged within the 20 seconds will eventually be included again in the response to another PullNotificationSet request, and those that are never acknowledged will ultimately be deleted according to the Google Cloud Platform Pub/Sub system policy.
        Multiple requests might be performed concurrently to retrieve notifications, in which case the pending notifications (if any) will be split among each caller, if any are pending.
        If no notifications are present, an empty notification list is returned. Subsequent requests may return more notifications once they become available.
      operationId: androidenterprise.enterprises.pullNotificationSet
      x-api-path-slug: enterprisespullnotificationset-post
      parameters:
      - in: query
        name: requestMode
        description: The request mode for pulling notifications
      responses:
        200:
          description: OK
      tags:
      - Notification
  /enterprises/signupUrl:
    post:
      summary: ""
      description: Generates a sign-up URL.
      operationId: androidenterprise.enterprises.generateSignupUrl
      x-api-path-slug: enterprisessignupurl-post
      parameters:
      - in: query
        name: callbackUrl
        description: The callback URL to which the Admin will be redirected after
          successfully creating an enterprise
      responses:
        200:
          description: OK
      tags:
      - Signup
  /enterprises/{enterpriseId}:
    delete:
      summary: Delete Enterprise
      description: Deletes the binding between the EMM and enterprise. This is now
        deprecated. Use this method only to unenroll customers that were previously
        enrolled with the insert call, then enroll them again with the enroll call.
      operationId: androidenterprise.enterprises.delete
      x-api-path-slug: enterprisesenterpriseid-delete
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Enterprise
    get:
      summary: Get Enterprise
      description: Retrieves the name and domain of an enterprise.
      operationId: androidenterprise.enterprises.get
      x-api-path-slug: enterprisesenterpriseid-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Enterprise
  /enterprises/{enterpriseId}/account:
    put:
      summary: Update Enterprise Account
      description: Sets the account that will be used to authenticate to the API as
        the enterprise.
      operationId: androidenterprise.enterprises.setAccount
      x-api-path-slug: enterprisesenterpriseidaccount-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Enterprise
  /enterprises/{enterpriseId}/createWebToken:
    post:
      summary: Create Web Token
      description: Returns a unique token to access an embeddable UI. To generate
        a web UI, pass the generated token into the managed Google Play javascript
        API. Each token may only be used to start one UI session. See the javascript
        API documentation for further information.
      operationId: androidenterprise.enterprises.createWebToken
      x-api-path-slug: enterprisesenterpriseidcreatewebtoken-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Token
  /enterprises/{enterpriseId}/groupLicenses:
    get:
      summary: Get Group Licenses
      description: Retrieves IDs of all products for which the enterprise has a group
        license.
      operationId: androidenterprise.grouplicenses.list
      x-api-path-slug: enterprisesenterpriseidgrouplicenses-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - License
  /enterprises/{enterpriseId}/groupLicenses/{groupLicenseId}:
    get:
      summary: Get Group License
      description: Retrieves details of an enterprise's group license for a product.
      operationId: androidenterprise.grouplicenses.get
      x-api-path-slug: enterprisesenterpriseidgrouplicensesgrouplicenseid-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: groupLicenseId
        description: The ID of the product the group license is for, e
      responses:
        200:
          description: OK
      tags:
      - License
  /{packageName}/edits/{editId}/tracks:
    get:
      summary: Get Track Configurations
      description: Lists all the track configurations for this edit.
      operationId: androidpublisher.edits.tracks.list
      x-api-path-slug: packagenameeditseditidtracks-get
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Track Configuration
  /enterprises/{enterpriseId}/groupLicenses/{groupLicenseId}/users:
    get:
      summary: Get Group License User
      description: Retrieves the IDs of the users who have been granted entitlements
        under the license.
      operationId: androidenterprise.grouplicenseusers.list
      x-api-path-slug: enterprisesenterpriseidgrouplicensesgrouplicenseidusers-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: groupLicenseId
        description: The ID of the product the group license is for, e
      responses:
        200:
          description: OK
      tags:
      - License
  /{packageName}/edits/{editId}/tracks/{track}:
    get:
      summary: Get Track Configuration
      description: Fetches the track configuration for the specified track type. Includes
        the APK version codes that are in this track.
      operationId: androidpublisher.edits.tracks.get
      x-api-path-slug: packagenameeditseditidtrackstrack-get
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      - in: path
        name: track
        description: The track type to read or modify
      responses:
        200:
          description: OK
      tags:
      - Track Configuration
    patch:
      summary: Update Track Configuration
      description: Updates the track configuration for the specified track type. When
        halted, the rollout track cannot be updated without adding new APKs, and adding
        new APKs will cause it to resume. This method supports patch semantics.
      operationId: androidpublisher.edits.tracks.patch
      x-api-path-slug: packagenameeditseditidtrackstrack-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      - in: path
        name: track
        description: The track type to read or modify
      responses:
        200:
          description: OK
      tags:
      - Track Configuration
    put:
      summary: Update Track Configuration
      description: Updates the track configuration for the specified track type. When
        halted, the rollout track cannot be updated without adding new APKs, and adding
        new APKs will cause it to resume.
      operationId: androidpublisher.edits.tracks.update
      x-api-path-slug: packagenameeditseditidtrackstrack-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      - in: path
        name: track
        description: The track type to read or modify
      responses:
        200:
          description: OK
      tags:
      - Track Configuration
  /enterprises/{enterpriseId}/products:
    get:
      summary: Get Products
      description: Finds approved products that match a query, or all approved products
        if there is no query.
      operationId: androidenterprise.products.list
      x-api-path-slug: enterprisesenterpriseidproducts-get
      parameters:
      - in: query
        name: approved
        description: Specifies whether to search among all products (false) or among
          only products that have been approved (true)
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: query
        name: language
        description: The BCP47 tag for the users preferred language (e
      - in: query
        name: maxResults
        description: Specifies the maximum number of products that can be returned
          per request
      - in: query
        name: query
        description: The search query as typed in the Google Play store search box
      - in: query
        name: token
        description: A pagination token is contained in a requests response when there
          are more products
      responses:
        200:
          description: OK
      tags:
      - Product
  /enterprises/{enterpriseId}/products/{productId}:
    get:
      summary: Get Product
      description: Retrieves details of a product for display to an enterprise admin.
      operationId: androidenterprise.products.get
      x-api-path-slug: enterprisesenterpriseidproductsproductid-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: query
        name: language
        description: The BCP47 tag for the users preferred language (e
      - in: path
        name: productId
        description: The ID of the product, e
      responses:
        200:
          description: OK
      tags:
      - Product
  /enterprises/{enterpriseId}/products/{productId}/appRestrictionsSchema:
    get:
      summary: Get Restriction Schema
      description: Retrieves the schema that defines the configurable properties for
        this product. All products have a schema, but this schema may be empty if
        no managed configurations have been defined. This schema can be used to populate
        a UI that allows an admin to configure the product. To apply a managed configuration
        based on the schema obtained using this API, see Managed Configurations through
        Play.
      operationId: androidenterprise.products.getAppRestrictionsSchema
      x-api-path-slug: enterprisesenterpriseidproductsproductidapprestrictionsschema-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: query
        name: language
        description: The BCP47 tag for the users preferred language (e
      - in: path
        name: productId
        description: The ID of the product
      responses:
        200:
          description: OK
      tags:
      - Schema
  /{packageName}/edits/{editId}:commit:
    post:
      summary: Commit Changes
      description: Commits/applies the changes made in this edit back to the app.
      operationId: androidpublisher.edits.commit
      x-api-path-slug: packagenameeditseditidcommit-post
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Change
  /{packageName}/edits/{editId}:validate:
    post:
      summary: Validate Changes
      description: Checks that the edit can be successfully committed. The edit's
        changes are not applied to the live app.
      operationId: androidpublisher.edits.validate
      x-api-path-slug: packagenameeditseditidvalidate-post
      parameters:
      - in: path
        name: editId
        description: Unique identifier for this edit
      - in: path
        name: packageName
        description: Unique identifier for the Android app that is being updated;
          for example, com
      responses:
        200:
          description: OK
      tags:
      - Change
  /enterprises/{enterpriseId}/products/{productId}/approve:
    post:
      summary: Approve Product
      description: |-
        Approves the specified product and the relevant app permissions, if any. The maximum number of products that you can approve per enterprise customer is 1,000.

        To learn how to use managed Google Play to design and create a store layout to display approved products to your users, see Store Layout Design.
      operationId: androidenterprise.products.approve
      x-api-path-slug: enterprisesenterpriseidproductsproductidapprove-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: productId
        description: The ID of the product
      responses:
        200:
          description: OK
      tags:
      - Product
  /{packageName}/entitlements:
    get:
      summary: Get Entitlements
      description: Lists the user's current inapp item or subscription entitlements
      operationId: androidpublisher.entitlements.list
      x-api-path-slug: packagenameentitlements-get
      parameters:
      - in: query
        name: maxResults
      - in: path
        name: packageName
        description: The package name of the application the inapp product was sold
          in (for example, com
      - in: query
        name: productId
        description: The product id of the inapp product (for example, sku1)
      - in: query
        name: startIndex
      - in: query
        name: token
      responses:
        200:
          description: OK
      tags:
      - Entitlement
  /enterprises/{enterpriseId}/products/{productId}/generateApprovalUrl:
    post:
      summary: Generates a URL
      description: |-
        Generates a URL that can be rendered in an iframe to display the permissions (if any) of a product. An enterprise admin must view these permissions and accept them on behalf of their organization in order to approve that product.

        Admins should accept the displayed permissions by interacting with a separate UI element in the EMM console, which in turn should trigger the use of this URL as the approvalUrlInfo.approvalUrl property in a Products.approve call to approve the product. This URL can only be used to display permissions for up to 1 day.
      operationId: androidenterprise.products.generateApprovalUrl
      x-api-path-slug: enterprisesenterpriseidproductsproductidgenerateapprovalurl-post
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: query
        name: languageCode
        description: The BCP 47 language code used for permission names and descriptions
          in the returned iframe, for instance en-US
      - in: path
        name: productId
        description: The ID of the product
      responses:
        200:
          description: OK
      tags:
      - URL
  /enterprises/{enterpriseId}/products/{productId}/permissions:
    get:
      summary: Retrieves the Android App Permission
      description: Retrieves the Android app permissions required by this app.
      operationId: androidenterprise.products.getPermissions
      x-api-path-slug: enterprisesenterpriseidproductsproductidpermissions-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: productId
        description: The ID of the product
      responses:
        200:
          description: OK
      tags:
      - Permission
  /{packageName}/inappproducts:
    get:
      summary: Get In App Products
      description: List all the in-app products for an Android app, both subscriptions
        and managed in-app products..
      operationId: androidpublisher.inappproducts.list
      x-api-path-slug: packagenameinappproducts-get
      parameters:
      - in: query
        name: maxResults
      - in: path
        name: packageName
        description: Unique identifier for the Android app with in-app products; for
          example, com
      - in: query
        name: startIndex
      - in: query
        name: token
      responses:
        200:
          description: OK
      tags:
      - In App Product
    post:
      summary: Create In App Products
      description: Creates a new in-app product for an app.
      operationId: androidpublisher.inappproducts.insert
      x-api-path-slug: packagenameinappproducts-post
      parameters:
      - in: query
        name: autoConvertMissingPrices
        description: If true the prices for all regions targeted by the parent app
          that dont have a price specified for this in-app product will be auto converted
          to the target currency based on the default price
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: packageName
        description: Unique identifier for the Android app; for example, com
      responses:
        200:
          description: OK
      tags:
      - In App Product
  /enterprises/{enterpriseId}/products/{productId}/unapprove:
    post:
      summary: Unnarove Product
      description: Unapproves the specified product (and the relevant app permissions,
        if any)
      operationId: androidenterprise.products.unapprove
      x-api-path-slug: enterprisesenterpriseidproductsproductidunapprove-post
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: productId
        description: The ID of the product
      responses:
        200:
          description: OK
      tags:
      - Product
  /enterprises/{enterpriseId}/sendTestPushNotification:
    post:
      summary: Send Test Push
      description: Sends a test push notification to validate the EMM integration
        with the Google Cloud Pub/Sub service for this enterprise.
      operationId: androidenterprise.enterprises.sendTestPushNotification
      x-api-path-slug: enterprisesenterpriseidsendtestpushnotification-post
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Testing
  /enterprises/{enterpriseId}/serviceAccount:
    get:
      summary: Return Service Account
      description: |-
        Returns a service account and credentials. The service account can be bound to the enterprise by calling setAccount. The service account is unique to this enterprise and EMM, and will be deleted if the enterprise is unbound. The credentials contain private key data and are not stored server-side.

        This method can only be called after calling Enterprises.Enroll or Enterprises.CompleteSignup, and before Enterprises.SetAccount; at other times it will return an error.

        Subsequent calls after the first will generate a new, unique set of credentials, and invalidate the previously generated credentials.

        Once the service account is bound to the enterprise, it can be managed using the serviceAccountKeys resource.
      operationId: androidenterprise.enterprises.getServiceAccount
      x-api-path-slug: enterprisesenterpriseidserviceaccount-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: query
        name: keyType
        description: The type of credential to return with the service account
      responses:
        200:
          description: OK
      tags:
      - Account
  /{packageName}/inappproducts/{sku}:
    delete:
      summary: Delete In App Products
      description: Delete an in-app product for an app.
      operationId: androidpublisher.inappproducts.delete
      x-api-path-slug: packagenameinappproductssku-delete
      parameters:
      - in: path
        name: packageName
        description: Unique identifier for the Android app with the in-app product;
          for example, com
      - in: path
        name: sku
        description: Unique identifier for the in-app product
      responses:
        200:
          description: OK
      tags:
      - In App Product
    get:
      summary: Get In App Product
      description: Returns information about the in-app product specified.
      operationId: androidpublisher.inappproducts.get
      x-api-path-slug: packagenameinappproductssku-get
      parameters:
      - in: path
        name: packageName
      - in: path
        name: sku
        description: Unique identifier for the in-app product
      responses:
        200:
          description: OK
      tags:
      - In App Product
    patch:
      summary: Update In App Product
      description: Updates the details of an in-app product. This method supports
        patch semantics.
      operationId: androidpublisher.inappproducts.patch
      x-api-path-slug: packagenameinappproductssku-patch
      parameters:
      - in: query
        name: autoConvertMissingPrices
        description: If true the prices for all regions targeted by the parent app
          that dont have a price specified for this in-app product will be auto converted
          to the target currency based on the default price
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: packageName
        description: Unique identifier for the Android app with the in-app product;
          for example, com
      - in: path
        name: sku
        description: Unique identifier for the in-app product
      responses:
        200:
          description: OK
      tags:
      - In App Product
    put:
      summary: Update In App Product
      description: Updates the details of an in-app product.
      operationId: androidpublisher.inappproducts.update
      x-api-path-slug: packagenameinappproductssku-put
      parameters:
      - in: query
        name: autoConvertMissingPrices
        description: If true the prices for all regions targeted by the parent app
          that dont have a price specified for this in-app product will be auto converted
          to the target currency based on the default price
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: packageName
        description: Unique identifier for the Android app with the in-app product;
          for example, com
      - in: path
        name: sku
        description: Unique identifier for the in-app product
      responses:
        200:
          description: OK
      tags:
      - In App Product
  /enterprises/{enterpriseId}/serviceAccountKeys:
    get:
      summary: Return Active Credentials
      description: Lists all active credentials for the service account associated
        with this enterprise. Only the ID and key type are returned. The calling service
        account must have been retrieved by calling Enterprises.GetServiceAccount
        and must have been set as the enterprise service account by calling Enterprises.SetAccount.
      operationId: androidenterprise.serviceaccountkeys.list
      x-api-path-slug: enterprisesenterpriseidserviceaccountkeys-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Credential
    post:
      summary: Generate New Credentials
      description: |-
        Generates new credentials for the service account associated with this enterprise. The calling service account must have been retrieved by calling Enterprises.GetServiceAccount and must have been set as the enterprise service account by calling Enterprises.SetAccount.

        Only the type of the key should be populated in the resource to be inserted.
      operationId: androidenterprise.serviceaccountkeys.insert
      x-api-path-slug: enterprisesenterpriseidserviceaccountkeys-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Credential
  /enterprises/{enterpriseId}/serviceAccountKeys/{keyId}:
    delete:
      summary: Remove and Invalidates Credentials
      description: Removes and invalidates the specified credentials for the service
        account associated with this enterprise. The calling service account must
        have been retrieved by calling Enterprises.GetServiceAccount and must have
        been set as the enterprise service account by calling Enterprises.SetAccount.
      operationId: androidenterprise.serviceaccountkeys.delete
      x-api-path-slug: enterprisesenterpriseidserviceaccountkeyskeyid-delete
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: keyId
        description: The ID of the key
      responses:
        200:
          description: OK
      tags:
      - Credential
  /enterprises/{enterpriseId}/storeLayout:
    get:
      summary: Get Store Layout
      description: Returns the store layout for the enterprise. If the store layout
        has not been set, or if the store layout has no homepageId set, returns a
        NOT_FOUND error.
      operationId: androidenterprise.enterprises.getStoreLayout
      x-api-path-slug: enterprisesenterpriseidstorelayout-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Store Layout
    put:
      summary: Update Store Layout
      description: Sets the store layout for the enterprise. By default, storeLayoutType
        is set to "basic" and the basic store layout is enabled. The basic layout
        only contains apps approved by the admin, and that have been added to the
        available product set for a user (using the  setAvailableProductSet call).
        Apps on the page are sorted in order of their product ID value. If you create
        a custom store layout (by setting storeLayoutType = "custom"), the basic store
        layout is disabled.
      operationId: androidenterprise.enterprises.setStoreLayout
      x-api-path-slug: enterprisesenterpriseidstorelayout-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Store Layout
  /enterprises/{enterpriseId}/storeLayout/pages:
    get:
      summary: Get Store Layout Pages
      description: Retrieves the details of all pages in the store.
      operationId: androidenterprise.storelayoutpages.list
      x-api-path-slug: enterprisesenterpriseidstorelayoutpages-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page
    post:
      summary: Create Store Layout Page
      description: Inserts a new store page.
      operationId: androidenterprise.storelayoutpages.insert
      x-api-path-slug: enterprisesenterpriseidstorelayoutpages-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page
  /{packageName}/purchases/products/{productId}/tokens/{token}:
    get:
      summary: Get In App Purchases
      description: Checks the purchase and consumption status of an inapp item.
      operationId: androidpublisher.purchases.products.get
      x-api-path-slug: packagenamepurchasesproductsproductidtokenstoken-get
      parameters:
      - in: path
        name: packageName
        description: The package name of the application the inapp product was sold
          in (for example, com
      - in: path
        name: productId
        description: The inapp product SKU (for example, com
      - in: path
        name: token
        description: The token provided to the users device when the inapp product
          was purchased
      responses:
        200:
          description: OK
      tags:
      - In App Purchase
  /enterprises/{enterpriseId}/storeLayout/pages/{pageId}:
    delete:
      summary: Delete Store Layout Page
      description: Deletes a store page.
      operationId: androidenterprise.storelayoutpages.delete
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageid-delete
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page
    get:
      summary: Get Store Layout Page
      description: Retrieves details of a store page.
      operationId: androidenterprise.storelayoutpages.get
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageid-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page
    patch:
      summary: Update Store Layout Page
      description: Updates the content of a store page. This method supports patch
        semantics.
      operationId: androidenterprise.storelayoutpages.patch
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page
    put:
      summary: Create Store Layout Page
      description: Updates the content of a store page.
      operationId: androidenterprise.storelayoutpages.update
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page Cluster
  /{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:
    get:
      summary: Check User Subscriptions
      description: Checks whether a user's subscription purchase is valid and returns
        its expiry time.
      operationId: androidpublisher.purchases.subscriptions.get
      x-api-path-slug: packagenamepurchasessubscriptionssubscriptionidtokenstoken-get
      parameters:
      - in: path
        name: packageName
        description: The package name of the application for which this subscription
          was purchased (for example, com
      - in: path
        name: subscriptionId
        description: The purchased subscription ID (for example, monthly001)
      - in: path
        name: token
        description: The token provided to the users device when the subscription
          was purchased
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:cancel:
    post:
      summary: Cancel User Subscription
      description: Cancels a user's subscription purchase. The subscription remains
        valid until its expiration time.
      operationId: androidpublisher.purchases.subscriptions.cancel
      x-api-path-slug: packagenamepurchasessubscriptionssubscriptionidtokenstokencancel-post
      parameters:
      - in: path
        name: packageName
        description: The package name of the application for which this subscription
          was purchased (for example, com
      - in: path
        name: subscriptionId
        description: The purchased subscription ID (for example, monthly001)
      - in: path
        name: token
        description: The token provided to the users device when the subscription
          was purchased
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:defer:
    post:
      summary: Defer User Subscription
      description: Defers a user's subscription purchase until a specified future
        expiration time.
      operationId: androidpublisher.purchases.subscriptions.defer
      x-api-path-slug: packagenamepurchasessubscriptionssubscriptionidtokenstokendefer-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: packageName
        description: The package name of the application for which this subscription
          was purchased (for example, com
      - in: path
        name: subscriptionId
        description: The purchased subscription ID (for example, monthly001)
      - in: path
        name: token
        description: The token provided to the users device when the subscription
          was purchased
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /enterprises/{enterpriseId}/storeLayout/pages/{pageId}/clusters:
    get:
      summary: Get Store Layout Page Clusters
      description: Retrieves the details of all clusters on the specified page.
      operationId: androidenterprise.storelayoutclusters.list
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageidclusters-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page Cluster
    post:
      summary: Insert Store Layout Page Cluster
      description: Inserts a new cluster in a page.
      operationId: androidenterprise.storelayoutclusters.insert
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageidclusters-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page Cluster
  /{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:refund:
    post:
      summary: Refund User Subscription
      description: Refunds a user's subscription purchase, but the subscription remains
        valid until its expiration time and it will continue to recur.
      operationId: androidpublisher.purchases.subscriptions.refund
      x-api-path-slug: packagenamepurchasessubscriptionssubscriptionidtokenstokenrefund-post
      parameters:
      - in: path
        name: packageName
        description: The package name of the application for which this subscription
          was purchased (for example, com
      - in: path
        name: subscriptionId
        description: The purchased subscription ID (for example, monthly001)
      - in: path
        name: token
        description: The token provided to the users device when the subscription
          was purchased
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /enterprises/{enterpriseId}/storeLayout/pages/{pageId}/clusters/{clusterId}:
    delete:
      summary: Delete Store Layout Page Cluster
      description: Deletes a cluster.
      operationId: androidenterprise.storelayoutclusters.delete
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageidclustersclusterid-delete
      parameters:
      - in: path
        name: clusterId
        description: The ID of the cluster
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page Cluster
    get:
      summary: Get Store Layout Page Cluster
      description: Retrieves details of a cluster.
      operationId: androidenterprise.storelayoutclusters.get
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageidclustersclusterid-get
      parameters:
      - in: path
        name: clusterId
        description: The ID of the cluster
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page Cluster
    patch:
      summary: Update Store Layout Page Cluster
      description: Updates a cluster. This method supports patch semantics.
      operationId: androidenterprise.storelayoutclusters.patch
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageidclustersclusterid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: clusterId
        description: The ID of the cluster
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page Cluster
    put:
      summary: Update Store Layout Page Cluster
      description: Updates a cluster.
      operationId: androidenterprise.storelayoutclusters.update
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageidclustersclusterid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: clusterId
        description: The ID of the cluster
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page Cluster
  /{packageName}/purchases/subscriptions/{subscriptionId}/tokens/{token}:revoke:
    post:
      summary: Refunds and Revoke
      description: Refunds and immediately revokes a user's subscription purchase.
        Access to the subscription will be terminated immediately and it will stop
        recurring.
      operationId: androidpublisher.purchases.subscriptions.revoke
      x-api-path-slug: packagenamepurchasessubscriptionssubscriptionidtokenstokenrevoke-post
      parameters:
      - in: path
        name: packageName
        description: The package name of the application for which this subscription
          was purchased (for example, com
      - in: path
        name: subscriptionId
        description: The purchased subscription ID (for example, monthly001)
      - in: path
        name: token
        description: The token provided to the users device when the subscription
          was purchased
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /{packageName}/purchases/voidedpurchases:
    get:
      summary: List Cancelled Purches
      description: Lists the purchases that were cancelled, refunded or charged-back.
      operationId: androidpublisher.purchases.voidedpurchases.list
      x-api-path-slug: packagenamepurchasesvoidedpurchases-get
      parameters:
      - in: query
        name: endTime
        description: The time, in milliseconds since the Epoch, of the newest voided
          in-app product purchase that you want to see in the response
      - in: query
        name: maxResults
      - in: path
        name: packageName
        description: The package name of the application for which voided purchases
          need to be returned (for example, com
      - in: query
        name: startIndex
      - in: query
        name: startTime
        description: The time, in milliseconds since the Epoch, of the oldest voided
          in-app product purchase that you want to see in the response
      - in: query
        name: token
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /{packageName}/reviews:
    get:
      summary: Get Reviews
      description: Returns a list of reviews. Only reviews from last week will be
        returned.
      operationId: androidpublisher.reviews.list
      x-api-path-slug: packagenamereviews-get
      parameters:
      - in: query
        name: maxResults
      - in: path
        name: packageName
        description: Unique identifier for the Android app for which we want reviews;
          for example, com
      - in: query
        name: startIndex
      - in: query
        name: token
      - in: query
        name: translationLanguage
      responses:
        200:
          description: OK
      tags:
      - Reviews
  /enterprises/{enterpriseId}/unenroll:
    post:
      summary: Unenroll Enterprise
      description: Unenrolls an enterprise from the calling EMM.
      operationId: androidenterprise.enterprises.unenroll
      x-api-path-slug: enterprisesenterpriseidunenroll-post
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Enterprise
  /{packageName}/reviews/{reviewId}:
    get:
      summary: Get Review
      description: Returns a single review.
      operationId: androidpublisher.reviews.get
      x-api-path-slug: packagenamereviewsreviewid-get
      parameters:
      - in: path
        name: packageName
        description: Unique identifier for the Android app for which we want reviews;
          for example, com
      - in: path
        name: reviewId
      - in: query
        name: translationLanguage
      responses:
        200:
          description: OK
      tags:
      - Reviews
  /enterprises/{enterpriseId}/users:
    get:
      summary: Lookup User
      description: Looks up a user by primary email address. This is only supported
        for Google-managed users. Lookup of the id is not needed for EMM-managed users
        because the id is already returned in the result of the Users.insert call.
      operationId: androidenterprise.users.list
      x-api-path-slug: enterprisesenterpriseidusers-get
      parameters:
      - in: query
        name: email
        description: The exact primary email address of the user to look up
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - User
    post:
      summary: Create New User
      description: |-
        Creates a new EMM-managed user.

        The Users resource passed in the body of the request should include an accountIdentifier and an accountType.
        If a corresponding user already exists with the same account identifier, the user will be updated with the resource. In this case only the displayName field can be changed.
      operationId: androidenterprise.users.insert
      x-api-path-slug: enterprisesenterpriseidusers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - User
  /{packageName}/reviews/{reviewId}:reply:
    post:
      summary: Reply To Review
      description: Reply to a single review, or update an existing reply.
      operationId: androidpublisher.reviews.reply
      x-api-path-slug: packagenamereviewsreviewidreply-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: packageName
        description: Unique identifier for the Android app for which we want reviews;
          for example, com
      - in: path
        name: reviewId
      responses:
        200:
          description: OK
      tags:
      - Reviews
  /enterprises/{enterpriseId}/users/{userId}:
    delete:
      summary: Delete User
      description: Deleted an EMM-managed user.
      operationId: androidenterprise.users.delete
      x-api-path-slug: enterprisesenterpriseidusersuserid-delete
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - User
    get:
      summary: Get User
      description: Retrieves a user's details.
      operationId: androidenterprise.users.get
      x-api-path-slug: enterprisesenterpriseidusersuserid-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - User
    patch:
      summary: Update User
      description: |-
        Updates the details of an EMM-managed user.

        Can be used with EMM-managed users only (not Google managed users). Pass the new details in the Users resource in the request body. Only the displayName field can be changed. Other fields must either be unset or have the currently active value. This method supports patch semantics.
      operationId: androidenterprise.users.patch
      x-api-path-slug: enterprisesenterpriseidusersuserid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - User
    put:
      summary: Update User
      description: |-
        Updates the details of an EMM-managed user.

        Can be used with EMM-managed users only (not Google managed users). Pass the new details in the Users resource in the request body. Only the displayName field can be changed. Other fields must either be unset or have the currently active value.
      operationId: androidenterprise.users.update
      x-api-path-slug: enterprisesenterpriseidusersuserid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - User
  /enterprises/{enterpriseId}/users/{userId}/authenticationToken:
    post:
      summary: Generate Authentication Token
      description: |-
        Generates an authentication token which the device policy client can use to provision the given EMM-managed user account on a device. The generated token is single-use and expires after a few minutes.

        This call only works with EMM-managed accounts.
      operationId: androidenterprise.users.generateAuthenticationToken
      x-api-path-slug: enterprisesenterpriseidusersuseridauthenticationtoken-post
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Token
  /enterprises/{enterpriseId}/users/{userId}/availableProductSet:
    get:
      summary: Get Products
      description: Retrieves the set of products a user is entitled to access.
      operationId: androidenterprise.users.getAvailableProductSet
      x-api-path-slug: enterprisesenterpriseidusersuseridavailableproductset-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Product
    put:
      summary: Update Products
      description: Modifies the set of products that a user is entitled to access
        (referred to as whitelisted products). Only products that are approved or
        products that were previously approved (products with revoked approval) can
        be whitelisted.
      operationId: androidenterprise.users.setAvailableProductSet
      x-api-path-slug: enterprisesenterpriseidusersuseridavailableproductset-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Product
  /enterprises/{enterpriseId}/users/{userId}/devices:
    get:
      summary: Get User Devices
      description: Retrieves the IDs of all of a user's devices.
      operationId: androidenterprise.devices.list
      x-api-path-slug: enterprisesenterpriseidusersuseriddevices-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Device
  /enterprises/{enterpriseId}/users/{userId}/devices/{deviceId}:
    get:
      summary: Get User Device
      description: Retrieves the details of a device.
      operationId: androidenterprise.devices.get
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceid-get
      parameters:
      - in: path
        name: deviceId
        description: The ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Device
  /enterprises/{enterpriseId}/users/{userId}/devices/{deviceId}/installs:
    get:
      summary: Get App Installs
      description: Retrieves the details of all apps installed on the specified device.
      operationId: androidenterprise.installs.list
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidinstalls-get
      parameters:
      - in: path
        name: deviceId
        description: The Android ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
  /enterprises/{enterpriseId}/users/{userId}/devices/{deviceId}/installs/{installId}:
    delete:
      summary: Remove App Install
      description: Requests to remove an app from a device. A call to get or list
        will still show the app as installed on the device until it is actually removed.
      operationId: androidenterprise.installs.delete
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidinstallsinstallid-delete
      parameters:
      - in: path
        name: deviceId
        description: The Android ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: installId
        description: The ID of the product represented by the install, e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
    get:
      summary: Get App Install
      description: Retrieves details of an installation of an app on a device.
      operationId: androidenterprise.installs.get
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidinstallsinstallid-get
      parameters:
      - in: path
        name: deviceId
        description: The Android ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: installId
        description: The ID of the product represented by the install, e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
    patch:
      summary: Update App Install
      description: Requests to install the latest version of an app to a device. If
        the app is already installed, then it is updated to the latest version if
        necessary. This method supports patch semantics.
      operationId: androidenterprise.installs.patch
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidinstallsinstallid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: deviceId
        description: The Android ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: installId
        description: The ID of the product represented by the install, e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
    put:
      summary: Update App Install
      description: Requests to install the latest version of an app to a device. If
        the app is already installed, then it is updated to the latest version if
        necessary.
      operationId: androidenterprise.installs.update
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidinstallsinstallid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: deviceId
        description: The Android ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: installId
        description: The ID of the product represented by the install, e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
  /enterprises/{enterpriseId}/users/{userId}/devices/{deviceId}/managedConfigurationsForDevice:
    get:
      summary: Get Per Device App Installs
      description: Lists all the per-device managed configurations for the specified
        device. Only the ID is set.
      operationId: androidenterprise.managedconfigurationsfordevice.list
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevice-get
      parameters:
      - in: path
        name: deviceId
        description: The Android ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
  /enterprises/{enterpriseId}/users/{userId}/devices/{deviceId}/managedConfigurationsForDevice/{managedConfigurationForDeviceId}:
    delete:
      summary: Remove Per Device App Install
      description: Removes a per-device managed configuration for an app for the specified
        device.
      operationId: androidenterprise.managedconfigurationsfordevice.delete
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevicemanagedconfigurationfordeviceid-delete
      parameters:
      - in: path
        name: deviceId
        description: The Android ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: managedConfigurationForDeviceId
        description: The ID of the managed configuration (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
    get:
      summary: Get Per Device App Install
      description: Retrieves details of a per-device managed configuration.
      operationId: androidenterprise.managedconfigurationsfordevice.get
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevicemanagedconfigurationfordeviceid-get
      parameters:
      - in: path
        name: deviceId
        description: The Android ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: managedConfigurationForDeviceId
        description: The ID of the managed configuration (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
    patch:
      summary: Update Per Device App Install
      description: Adds or updates a per-device managed configuration for an app for
        the specified device. This method supports patch semantics.
      operationId: androidenterprise.managedconfigurationsfordevice.patch
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevicemanagedconfigurationfordeviceid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: deviceId
        description: The Android ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: managedConfigurationForDeviceId
        description: The ID of the managed configuration (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
    put:
      summary: Update Per Device App Install
      description: Adds or updates a per-device managed configuration for an app for
        the specified device.
      operationId: androidenterprise.managedconfigurationsfordevice.update
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidmanagedconfigurationsfordevicemanagedconfigurationfordeviceid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: deviceId
        description: The Android ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: managedConfigurationForDeviceId
        description: The ID of the managed configuration (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
  /enterprises/{enterpriseId}/users/{userId}/devices/{deviceId}/state:
    get:
      summary: Get Per Device App Install State
      description: Retrieves whether a device's access to Google services is enabled
        or disabled. The device state takes effect only if enforcing EMM policies
        on Android devices is enabled in the Google Admin Console. Otherwise, the
        device state is ignored and all devices are allowed access to Google services.
        This is only supported for Google-managed users.
      operationId: androidenterprise.devices.getState
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidstate-get
      parameters:
      - in: path
        name: deviceId
        description: The ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
    put:
      summary: Update Per Device App Install State
      description: Sets whether a device's access to Google services is enabled or
        disabled. The device state takes effect only if enforcing EMM policies on
        Android devices is enabled in the Google Admin Console. Otherwise, the device
        state is ignored and all devices are allowed access to Google services. This
        is only supported for Google-managed users.
      operationId: androidenterprise.devices.setState
      x-api-path-slug: enterprisesenterpriseidusersuseriddevicesdeviceidstate-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: deviceId
        description: The ID of the device
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - App Install
  /enterprises/{enterpriseId}/users/{userId}/entitlements:
    get:
      summary: Get Entitlements
      description: Lists all entitlements for the specified user. Only the ID is set.
      operationId: androidenterprise.entitlements.list
      x-api-path-slug: enterprisesenterpriseidusersuseridentitlements-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Entitlement
  /enterprises/{enterpriseId}/users/{userId}/entitlements/{entitlementId}:
    delete:
      summary: Remove Entitlement
      description: Removes an entitlement to an app for a user.
      operationId: androidenterprise.entitlements.delete
      x-api-path-slug: enterprisesenterpriseidusersuseridentitlementsentitlementid-delete
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: entitlementId
        description: The ID of the entitlement (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Entitlement
    get:
      summary: Get Entitlement
      description: Retrieves details of an entitlement.
      operationId: androidenterprise.entitlements.get
      x-api-path-slug: enterprisesenterpriseidusersuseridentitlementsentitlementid-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: entitlementId
        description: The ID of the entitlement (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Entitlement
    patch:
      summary: Update Entitlement
      description: Adds or updates an entitlement to an app for a user. This method
        supports patch semantics.
      operationId: androidenterprise.entitlements.patch
      x-api-path-slug: enterprisesenterpriseidusersuseridentitlementsentitlementid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: entitlementId
        description: The ID of the entitlement (a product ID), e
      - in: query
        name: install
        description: Set to true to also install the product on all the users devices
          where possible
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Entitlement
    put:
      summary: Update Entitlement
      description: Adds or updates an entitlement to an app for a user.
      operationId: androidenterprise.entitlements.update
      x-api-path-slug: enterprisesenterpriseidusersuseridentitlementsentitlementid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: entitlementId
        description: The ID of the entitlement (a product ID), e
      - in: query
        name: install
        description: Set to true to also install the product on all the users devices
          where possible
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Entitlement
  /enterprises/{enterpriseId}/users/{userId}/managedConfigurationsForUser:
    get:
      summary: Get Per User Configurations
      description: Lists all the per-user managed configurations for the specified
        user. Only the ID is set.
      operationId: androidenterprise.managedconfigurationsforuser.list
      x-api-path-slug: enterprisesenterpriseidusersuseridmanagedconfigurationsforuser-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Configuration
  /enterprises/{enterpriseId}/users/{userId}/managedConfigurationsForUser/{managedConfigurationForUserId}:
    delete:
      summary: Delete Per User Configurations
      description: Removes a per-user managed configuration for an app for the specified
        user.
      operationId: androidenterprise.managedconfigurationsforuser.delete
      x-api-path-slug: enterprisesenterpriseidusersuseridmanagedconfigurationsforusermanagedconfigurationforuserid-delete
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: managedConfigurationForUserId
        description: The ID of the managed configuration (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Configuration
    get:
      summary: Get Per User Configuration
      description: Retrieves details of a per-user managed configuration for an app
        for the specified user.
      operationId: androidenterprise.managedconfigurationsforuser.get
      x-api-path-slug: enterprisesenterpriseidusersuseridmanagedconfigurationsforusermanagedconfigurationforuserid-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: managedConfigurationForUserId
        description: The ID of the managed configuration (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Configuration
    patch:
      summary: Update Per User Configuration
      description: Adds or updates a per-user managed configuration for an app for
        the specified user. This method supports patch semantics.
      operationId: androidenterprise.managedconfigurationsforuser.patch
      x-api-path-slug: enterprisesenterpriseidusersuseridmanagedconfigurationsforusermanagedconfigurationforuserid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: managedConfigurationForUserId
        description: The ID of the managed configuration (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Configuration
    put:
      summary: Update Per User Configuration
      description: Adds or updates a per-user managed configuration for an app for
        the specified user.
      operationId: androidenterprise.managedconfigurationsforuser.update
      x-api-path-slug: enterprisesenterpriseidusersuseridmanagedconfigurationsforusermanagedconfigurationforuserid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: managedConfigurationForUserId
        description: The ID of the managed configuration (a product ID), e
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Configuration
  /enterprises/{enterpriseId}/users/{userId}/token:
    delete:
      summary: Delete User Token
      description: Revokes a previously generated token (activation code) for the
        user.
      operationId: androidenterprise.users.revokeToken
      x-api-path-slug: enterprisesenterpriseidusersuseridtoken-delete
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Token
    post:
      summary: Generate User Token
      description: |-
        Generates a token (activation code) to allow this user to configure their managed account in the Android Setup Wizard. Revokes any previously generated token.

        This call only works with Google managed accounts.
      operationId: androidenterprise.users.generateToken
      x-api-path-slug: enterprisesenterpriseidusersuseridtoken-post
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Token
  /permissions/{permissionId}:
    get:
      summary: Get Permissions
      description: Retrieves details of an Android app permission for display to an
        enterprise admin.
      operationId: androidenterprise.permissions.get
      x-api-path-slug: permissionspermissionid-get
      parameters:
      - in: query
        name: language
        description: The BCP47 tag for the users preferred language (e
      - in: path
        name: permissionId
        description: The ID of the permission
      responses:
        200:
          description: OK
      tags:
      - Permission
  /states:
    get:
      summary: Get State Keys
      description: Lists all the states keys, and optionally the state data.
      operationId: appstate.states.list
      x-api-path-slug: states-get
      parameters:
      - in: query
        name: includeData
        description: Whether to include the full data in addition to the version number
      responses:
        200:
          description: OK
      tags:
      - Application State
  /states/{stateKey}:
    delete:
      summary: Delete State Key
      description: Deletes a key and the data associated with it. The key is removed
        and no longer counts against the key quota. Note that since this method is
        not safe in the face of concurrent modifications, it should only be used for
        development and testing purposes. Invoking this method in shipping code can
        result in data loss and data corruption.
      operationId: appstate.states.delete
      x-api-path-slug: statesstatekey-delete
      parameters:
      - in: path
        name: stateKey
        description: The key for the data to be retrieved
      responses:
        200:
          description: OK
      tags:
      - Application State
    get:
      summary: Get State Key
      description: Retrieves the data corresponding to the passed key. If the key
        does not exist on the server, an HTTP 404 will be returned.
      operationId: appstate.states.get
      x-api-path-slug: statesstatekey-get
      parameters:
      - in: path
        name: stateKey
        description: The key for the data to be retrieved
      responses:
        200:
          description: OK
      tags:
      - Application State
    put:
      summary: Update State Key
      description: Update the data associated with the input key if and only if the
        passed version matches the currently stored version. This method is safe in
        the face of concurrent writes. Maximum per-key size is 128KB.
      operationId: appstate.states.update
      x-api-path-slug: statesstatekey-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: currentStateVersion
        description: The version of the app state your application is attempting to
          update
      - in: path
        name: stateKey
        description: The key for the data to be retrieved
      responses:
        200:
          description: OK
      tags:
      - Application State
  /states/{stateKey}/clear:
    post:
      summary: Clear State Key
      description: Clears (sets to empty) the data for the passed key if and only
        if the passed version matches the currently stored version. This method results
        in a conflict error on version mismatch.
      operationId: appstate.states.clear
      x-api-path-slug: statesstatekeyclear-post
      parameters:
      - in: query
        name: currentDataVersion
        description: The version of the data to be cleared
      - in: path
        name: stateKey
        description: The key for the data to be retrieved
      responses:
        200:
          description: OK
      tags:
      - Application State
  /achievements:
    get:
      summary: Get Achievements
      description: Lists all the achievement definitions for your application.
      operationId: games.achievementDefinitions.list
      x-api-path-slug: achievements-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: query
        name: maxResults
        description: The maximum number of achievement resources to return in the
          response, used for paging
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Achievement
  /achievements/updateMultiple:
    post:
      summary: Update Multiple Achievements
      description: Updates multiple achievements for the currently authenticated player.
      operationId: games.achievements.updateMultiple
      x-api-path-slug: achievementsupdatemultiple-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      responses:
        200:
          description: OK
      tags:
      - Achievement
  /achievements/{achievementId}/increment:
    post:
      summary: Increment Step Of Achievement
      description: Increments the steps of the achievement with the given ID for the
        currently authenticated player.
      operationId: games.achievements.increment
      x-api-path-slug: achievementsachievementidincrement-post
      parameters:
      - in: path
        name: achievementId
        description: The ID of the achievement used by this method
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: requestId
        description: A randomly generated numeric ID for each request specified by
          the caller
      - in: query
        name: stepsToIncrement
        description: The number of steps to increment
      responses:
        200:
          description: OK
      tags:
      - Achievement
  /achievements/{achievementId}/reveal:
    post:
      summary: Set State of Achievement
      description: Sets the state of the achievement with the given ID to REVEALED
        for the currently authenticated player.
      operationId: games.achievements.reveal
      x-api-path-slug: achievementsachievementidreveal-post
      parameters:
      - in: path
        name: achievementId
        description: The ID of the achievement used by this method
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      responses:
        200:
          description: OK
      tags:
      - Achievement
  /achievements/{achievementId}/setStepsAtLeast:
    post:
      summary: Set Steps for Achievements
      description: Sets the steps for the currently authenticated player towards unlocking
        an achievement. If the steps parameter is less than the current number of
        steps that the player already gained for the achievement, the achievement
        is not modified.
      operationId: games.achievements.setStepsAtLeast
      x-api-path-slug: achievementsachievementidsetstepsatleast-post
      parameters:
      - in: path
        name: achievementId
        description: The ID of the achievement used by this method
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: steps
        description: The minimum value to set the steps to
      responses:
        200:
          description: OK
      tags:
      - Achievement
  /achievements/{achievementId}/unlock:
    post:
      summary: Unlock Achievement
      description: Unlocks this achievement for the currently authenticated player.
      operationId: games.achievements.unlock
      x-api-path-slug: achievementsachievementidunlock-post
      parameters:
      - in: path
        name: achievementId
        description: The ID of the achievement used by this method
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      responses:
        200:
          description: OK
      tags:
      - Achievement
  /applications/played:
    post:
      summary: Set Played
      description: Indicate that the the currently authenticated user is playing your
        application.
      operationId: games.applications.played
      x-api-path-slug: applicationsplayed-post
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      responses:
        200:
          description: OK
      tags:
      - Application
  /applications/{applicationId}:
    get:
      summary: Get Application
      description: Retrieves the metadata of the application with the given ID. If
        the requested application is not available for the specified platformType,
        the returned response will not include any instance data.
      operationId: games.applications.get
      x-api-path-slug: applicationsapplicationid-get
      parameters:
      - in: path
        name: applicationId
        description: The application ID from the Google Play developer console
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: query
        name: platformType
        description: Restrict application details returned to the specific platform
      responses:
        200:
          description: OK
      tags:
      - Application
  /applications/{applicationId}/verify:
    get:
      summary: Verify Token
      description: Verifies the auth token provided with this request is for the application
        with the specified ID, and returns the ID of the player it was granted for.
      operationId: games.applications.verify
      x-api-path-slug: applicationsapplicationidverify-get
      parameters:
      - in: path
        name: applicationId
        description: The application ID from the Google Play developer console
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      responses:
        200:
          description: OK
      tags:
      - Token
  /eventDefinitions:
    get:
      summary: Get Event Definitions
      description: Returns a list of the event definitions in this application.
      operationId: games.events.listDefinitions
      x-api-path-slug: eventdefinitions-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: query
        name: maxResults
        description: The maximum number of event definitions to return in the response,
          used for paging
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Event
  /events:
    get:
      summary: Get Events
      description: Returns a list showing the current progress on events in this application
        for the currently authenticated user.
      operationId: games.events.listByPlayer
      x-api-path-slug: events-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: query
        name: maxResults
        description: The maximum number of events to return in the response, used
          for paging
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Event
    post:
      summary: Create Event
      description: Records a batch of changes to the number of times events have occurred
        for the currently authenticated user of this application.
      operationId: games.events.record
      x-api-path-slug: events-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      responses:
        200:
          description: OK
      tags:
      - Event
  /leaderboards:
    get:
      summary: Get Leader Boards
      description: Lists all the leaderboard metadata for your application.
      operationId: games.leaderboards.list
      x-api-path-slug: leaderboards-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: query
        name: maxResults
        description: The maximum number of leaderboards to return in the response
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Leader Board
  /leaderboards/scores:
    post:
      summary: Create Leader Board
      description: Submits multiple scores to leaderboards.
      operationId: games.scores.submitMultiple
      x-api-path-slug: leaderboardsscores-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      responses:
        200:
          description: OK
      tags:
      - Leader Board
  /leaderboards/{leaderboardId}:
    get:
      summary: Get Leader Board
      description: Retrieves the metadata of the leaderboard with the given ID.
      operationId: games.leaderboards.get
      x-api-path-slug: leaderboardsleaderboardid-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: leaderboardId
        description: The ID of the leaderboard
      responses:
        200:
          description: OK
      tags:
      - Leader Board
  /leaderboards/{leaderboardId}/scores:
    post:
      summary: Update Leader Board Score
      description: Submits a score to the specified leaderboard.
      operationId: games.scores.submit
      x-api-path-slug: leaderboardsleaderboardidscores-post
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: leaderboardId
        description: The ID of the leaderboard
      - in: query
        name: score
        description: The score youre submitting
      - in: query
        name: scoreTag
        description: Additional information about the score youre submitting
      responses:
        200:
          description: OK
      tags:
      - Leader Board
  /leaderboards/{leaderboardId}/scores/{collection}:
    get:
      summary: Get Leader Board Scores
      description: Lists the scores in a leaderboard, starting from the top.
      operationId: games.scores.list
      x-api-path-slug: leaderboardsleaderboardidscorescollection-get
      parameters:
      - in: path
        name: collection
        description: The collection of scores youre requesting
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: leaderboardId
        description: The ID of the leaderboard
      - in: query
        name: maxResults
        description: The maximum number of leaderboard scores to return in the response
      - in: query
        name: pageToken
        description: The token returned by the previous request
      - in: query
        name: timeSpan
        description: The time span for the scores and ranks youre requesting
      responses:
        200:
          description: OK
      tags:
      - Leader Board
  /leaderboards/{leaderboardId}/window/{collection}:
    get:
      summary: Get Leader Board Window
      description: Lists the scores in a leaderboard around (and including) a player's
        score.
      operationId: games.scores.listWindow
      x-api-path-slug: leaderboardsleaderboardidwindowcollection-get
      parameters:
      - in: path
        name: collection
        description: The collection of scores youre requesting
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: leaderboardId
        description: The ID of the leaderboard
      - in: query
        name: maxResults
        description: The maximum number of leaderboard scores to return in the response
      - in: query
        name: pageToken
        description: The token returned by the previous request
      - in: query
        name: resultsAbove
        description: The preferred number of scores to return above the players score
      - in: query
        name: returnTopIfAbsent
        description: True if the top scores should be returned when the player is
          not in the leaderboard
      - in: query
        name: timeSpan
        description: The time span for the scores and ranks youre requesting
      responses:
        200:
          description: OK
      tags:
      - Leader Board
  /metagameConfig:
    get:
      summary: Get Metagame Confirmation
      description: Return the metagame configuration data for the calling application.
      operationId: games.metagame.getMetagameConfig
      x-api-path-slug: metagameconfig-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      responses:
        200:
          description: OK
      tags:
      - Game
  /players/me/players/{collection}:
    get:
      summary: Get PLayers
      description: Get the collection of players for the currently authenticated user.
      operationId: games.players.list
      x-api-path-slug: playersmeplayerscollection-get
      parameters:
      - in: path
        name: collection
        description: Collection of players being retrieved
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: query
        name: maxResults
        description: The maximum number of player resources to return in the response,
          used for paging
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Player
  /players/{playerId}:
    get:
      summary: Get Player
      description: Retrieves the Player resource with the given ID. To retrieve the
        player for the currently authenticated user, set playerId to me.
      operationId: games.players.get
      x-api-path-slug: playersplayerid-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: playerId
        description: A player ID
      responses:
        200:
          description: OK
      tags:
      - Player
  /players/{playerId}/achievements:
    get:
      summary: Get Player Achievements
      description: Lists the progress for all your application's achievements for
        the currently authenticated player.
      operationId: games.achievements.list
      x-api-path-slug: playersplayeridachievements-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: query
        name: maxResults
        description: The maximum number of achievement resources to return in the
          response, used for paging
      - in: query
        name: pageToken
        description: The token returned by the previous request
      - in: path
        name: playerId
        description: A player ID
      - in: query
        name: state
        description: Tells the server to return only achievements with the specified
          state
      responses:
        200:
          description: OK
      tags:
      - Player
  /players/{playerId}/categories/{collection}:
    get:
      summary: Get Player Categories
      description: List play data aggregated per category for the player corresponding
        to playerId.
      operationId: games.metagame.listCategoriesByPlayer
      x-api-path-slug: playersplayeridcategoriescollection-get
      parameters:
      - in: path
        name: collection
        description: The collection of categories for which data will be returned
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: query
        name: maxResults
        description: The maximum number of category resources to return in the response,
          used for paging
      - in: query
        name: pageToken
        description: The token returned by the previous request
      - in: path
        name: playerId
        description: A player ID
      responses:
        200:
          description: OK
      tags:
      - Player
  /players/{playerId}/leaderboards/{leaderboardId}/scores/{timeSpan}:
    get:
      summary: Get Player Leaderboard Scores
      description: |-
        Get high scores, and optionally ranks, in leaderboards for the currently authenticated player. For a specific time span, leaderboardId can be set to ALL to retrieve data for all leaderboards in a given time span.
        NOTE: You cannot ask for 'ALL' leaderboards and 'ALL' timeSpans in the same request; only one parameter may be set to 'ALL'.
      operationId: games.scores.get
      x-api-path-slug: playersplayeridleaderboardsleaderboardidscorestimespan-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: includeRankType
        description: The types of ranks to return
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: leaderboardId
        description: The ID of the leaderboard
      - in: query
        name: maxResults
        description: The maximum number of leaderboard scores to return in the response
      - in: query
        name: pageToken
        description: The token returned by the previous request
      - in: path
        name: playerId
        description: A player ID
      - in: path
        name: timeSpan
        description: The time span for the scores and ranks youre requesting
      responses:
        200:
          description: OK
      tags:
      - Player
  /players/{playerId}/quests:
    get:
      summary: Get Guests
      description: Get a list of quests for your application and the currently authenticated
        player.
      operationId: games.quests.list
      x-api-path-slug: playersplayeridquests-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: query
        name: maxResults
        description: The maximum number of quest resources to return in the response,
          used for paging
      - in: query
        name: pageToken
        description: The token returned by the previous request
      - in: path
        name: playerId
        description: A player ID
      responses:
        200:
          description: OK
      tags:
      - Guest
  /players/{playerId}/snapshots:
    get:
      summary: Get Player Snapshots
      description: Retrieves a list of snapshots created by your application for the
        player corresponding to the player ID.
      operationId: games.snapshots.list
      x-api-path-slug: playersplayeridsnapshots-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: query
        name: maxResults
        description: The maximum number of snapshot resources to return in the response,
          used for paging
      - in: query
        name: pageToken
        description: The token returned by the previous request
      - in: path
        name: playerId
        description: A player ID
      responses:
        200:
          description: OK
      tags:
      - Player
  /pushtokens:
    put:
      summary: Register Push Token
      description: Registers a push token for the current user and application.
      operationId: games.pushtokens.update
      x-api-path-slug: pushtokens-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      responses:
        200:
          description: OK
      tags:
      - Token
  /pushtokens/remove:
    post:
      summary: Remove Push Token
      description: Removes a push token for the current user and application. Removing
        a non-existent push token will report success.
      operationId: games.pushtokens.remove
      x-api-path-slug: pushtokensremove-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      responses:
        200:
          description: OK
      tags:
      - Token
  /quests/{questId}/accept:
    post:
      summary: Accept Quest
      description: Indicates that the currently authorized user will participate in
        the quest.
      operationId: games.quests.accept
      x-api-path-slug: questsquestidaccept-post
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: questId
        description: The ID of the quest
      responses:
        200:
          description: OK
      tags:
      - Quest
  /quests/{questId}/milestones/{milestoneId}/claim:
    put:
      summary: Claim Quest Milestone
      description: Report that a reward for the milestone corresponding to milestoneId
        for the quest corresponding to questId has been claimed by the currently authorized
        user.
      operationId: games.questMilestones.claim
      x-api-path-slug: questsquestidmilestonesmilestoneidclaim-put
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: path
        name: milestoneId
        description: The ID of the milestone
      - in: path
        name: questId
        description: The ID of the quest
      - in: query
        name: requestId
        description: A numeric ID to ensure that the request is handled correctly
          across retries
      responses:
        200:
          description: OK
      tags:
      - Milestone
  /revisions/check:
    get:
      summary: Check Revision
      description: Checks whether the games client is out of date.
      operationId: games.revisions.check
      x-api-path-slug: revisionscheck-get
      parameters:
      - in: query
        name: clientRevision
        description: The revision of the client SDK used by your application
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      responses:
        200:
          description: OK
      tags:
      - Revision
  /rooms:
    get:
      summary: Get Rooms
      description: Returns invitations to join rooms.
      operationId: games.rooms.list
      x-api-path-slug: rooms-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: query
        name: maxResults
        description: The maximum number of rooms to return in the response, used for
          paging
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Room
  /rooms/create:
    post:
      summary: Create Room
      description: Create a room. For internal use by the Games SDK only. Calling
        this method directly is unsupported.
      operationId: games.rooms.create
      x-api-path-slug: roomscreate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      responses:
        200:
          description: OK
      tags:
      - Room
  /rooms/{roomId}:
    get:
      summary: Get Room
      description: Get the data for a room.
      operationId: games.rooms.get
      x-api-path-slug: roomsroomid-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: roomId
        description: The ID of the room
      responses:
        200:
          description: OK
      tags:
      - Room
  /rooms/{roomId}/decline:
    post:
      summary: Decline Room
      description: Decline an invitation to join a room. For internal use by the Games
        SDK only. Calling this method directly is unsupported.
      operationId: games.rooms.decline
      x-api-path-slug: roomsroomiddecline-post
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: roomId
        description: The ID of the room
      responses:
        200:
          description: OK
      tags:
      - Room
  /rooms/{roomId}/dismiss:
    post:
      summary: Dismiss Room
      description: Dismiss an invitation to join a room. For internal use by the Games
        SDK only. Calling this method directly is unsupported.
      operationId: games.rooms.dismiss
      x-api-path-slug: roomsroomiddismiss-post
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: path
        name: roomId
        description: The ID of the room
      responses:
        200:
          description: OK
      tags:
      - Room
  /rooms/{roomId}/join:
    post:
      summary: Join Room
      description: Join a room. For internal use by the Games SDK only. Calling this
        method directly is unsupported.
      operationId: games.rooms.join
      x-api-path-slug: roomsroomidjoin-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: roomId
        description: The ID of the room
      responses:
        200:
          description: OK
      tags:
      - Room
  /rooms/{roomId}/leave:
    post:
      summary: Leave Room
      description: Leave a room. For internal use by the Games SDK only. Calling this
        method directly is unsupported.
      operationId: games.rooms.leave
      x-api-path-slug: roomsroomidleave-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: roomId
        description: The ID of the room
      responses:
        200:
          description: OK
      tags:
      - Room
  /rooms/{roomId}/reportstatus:
    post:
      summary: Report Room Status
      description: Updates sent by a client reporting the status of peers in a room.
        For internal use by the Games SDK only. Calling this method directly is unsupported.
      operationId: games.rooms.reportStatus
      x-api-path-slug: roomsroomidreportstatus-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: roomId
        description: The ID of the room
      responses:
        200:
          description: OK
      tags:
      - Room
  /snapshots/{snapshotId}:
    get:
      summary: Get Snapshot
      description: Retrieves the metadata for a given snapshot ID.
      operationId: games.snapshots.get
      x-api-path-slug: snapshotssnapshotid-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: snapshotId
        description: The ID of the snapshot
      responses:
        200:
          description: OK
      tags:
      - Snapshot
  /turnbasedmatches:
    get:
      summary: Return Turn-Based Match
      description: Returns turn-based matches the player is or was involved in.
      operationId: games.turnBasedMatches.list
      x-api-path-slug: turnbasedmatches-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: includeMatchData
        description: True if match data should be returned in the response
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: query
        name: maxCompletedMatches
        description: The maximum number of completed or canceled matches to return
          in the response
      - in: query
        name: maxResults
        description: The maximum number of matches to return in the response, used
          for paging
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Match
  /turnbasedmatches/create:
    post:
      summary: Create Turn-Based Match
      description: Create a turn-based match.
      operationId: games.turnBasedMatches.create
      x-api-path-slug: turnbasedmatchescreate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      responses:
        200:
          description: OK
      tags:
      - Match
  /turnbasedmatches/sync:
    get:
      summary: Sync Turn-Based Match
      description: Returns turn-based matches the player is or was involved in that
        changed since the last sync call, with the least recent changes coming first.
        Matches that should be removed from the local cache will have a status of
        MATCH_DELETED.
      operationId: games.turnBasedMatches.sync
      x-api-path-slug: turnbasedmatchessync-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: includeMatchData
        description: True if match data should be returned in the response
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: query
        name: maxCompletedMatches
        description: The maximum number of completed or canceled matches to return
          in the response
      - in: query
        name: maxResults
        description: The maximum number of matches to return in the response, used
          for paging
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Match
  /turnbasedmatches/{matchId}:
    get:
      summary: Get Turn-Based Match
      description: Get the data for a turn-based match.
      operationId: games.turnBasedMatches.get
      x-api-path-slug: turnbasedmatchesmatchid-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: includeMatchData
        description: Get match data along with metadata
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: matchId
        description: The ID of the match
      responses:
        200:
          description: OK
      tags:
      - Match
  /turnbasedmatches/{matchId}/cancel:
    put:
      summary: Update Turn-Based Match
      description: Cancel a turn-based match.
      operationId: games.turnBasedMatches.cancel
      x-api-path-slug: turnbasedmatchesmatchidcancel-put
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: path
        name: matchId
        description: The ID of the match
      responses:
        200:
          description: OK
      tags:
      - Match
  /turnbasedmatches/{matchId}/decline:
    put:
      summary: Decline Turn-Based Match
      description: Decline an invitation to play a turn-based match.
      operationId: games.turnBasedMatches.decline
      x-api-path-slug: turnbasedmatchesmatchiddecline-put
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: matchId
        description: The ID of the match
      responses:
        200:
          description: OK
      tags:
      - Match
  /turnbasedmatches/{matchId}/dismiss:
    put:
      summary: Dismiss Turn-Based Match
      description: Dismiss a turn-based match from the match list. The match will
        no longer show up in the list and will not generate notifications.
      operationId: games.turnBasedMatches.dismiss
      x-api-path-slug: turnbasedmatchesmatchiddismiss-put
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: path
        name: matchId
        description: The ID of the match
      responses:
        200:
          description: OK
      tags:
      - Match
  /turnbasedmatches/{matchId}/finish:
    put:
      summary: Finish Turn-Based Match
      description: Finish a turn-based match. Each player should make this call once,
        after all results are in. Only the player whose turn it is may make the first
        call to Finish, and can pass in the final match state.
      operationId: games.turnBasedMatches.finish
      x-api-path-slug: turnbasedmatchesmatchidfinish-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: matchId
        description: The ID of the match
      responses:
        200:
          description: OK
      tags:
      - Match
  /turnbasedmatches/{matchId}/join:
    put:
      summary: Join Turn-Based Match
      description: Join a turn-based match.
      operationId: games.turnBasedMatches.join
      x-api-path-slug: turnbasedmatchesmatchidjoin-put
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: matchId
        description: The ID of the match
      responses:
        200:
          description: OK
      tags:
      - Match
  /turnbasedmatches/{matchId}/leave:
    put:
      summary: Leave Turn-Based Match
      description: Leave a turn-based match when it is not the current player's turn,
        without canceling the match.
      operationId: games.turnBasedMatches.leave
      x-api-path-slug: turnbasedmatchesmatchidleave-put
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: matchId
        description: The ID of the match
      responses:
        200:
          description: OK
      tags:
      - Match
  /turnbasedmatches/{matchId}/leaveTurn:
    put:
      summary: ReLeave Turnturn Turn-Based Match
      description: Leave a turn-based match during the current player's turn, without
        canceling the match.
      operationId: games.turnBasedMatches.leaveTurn
      x-api-path-slug: turnbasedmatchesmatchidleaveturn-put
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: matchId
        description: The ID of the match
      - in: query
        name: matchVersion
        description: The version of the match being updated
      - in: query
        name: pendingParticipantId
        description: The ID of another participant who should take their turn next
      responses:
        200:
          description: OK
      tags:
      - Match
  /turnbasedmatches/{matchId}/rematch:
    post:
      summary: Rematch Turn-Based Match
      description: Create a rematch of a match that was previously completed, with
        the same participants. This can be called by only one player on a match still
        in their list; the player must have called Finish first. Returns the newly
        created match; it will be the caller's turn.
      operationId: games.turnBasedMatches.rematch
      x-api-path-slug: turnbasedmatchesmatchidrematch-post
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: matchId
        description: The ID of the match
      - in: query
        name: requestId
        description: A randomly generated numeric ID for each request specified by
          the caller
      responses:
        200:
          description: OK
      tags:
      - Match
  /turnbasedmatches/{matchId}/turn:
    put:
      summary: Turn Turn-Based Match
      description: Commit the results of a player turn.
      operationId: games.turnBasedMatches.takeTurn
      x-api-path-slug: turnbasedmatchesmatchidturn-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: matchId
        description: The ID of the match
      responses:
        200:
          description: OK
      tags:
      - Match
  /v1/accounts/{accountId}/avails:
    get:
      summary: Get Available Movies
      description: |-
        List Avails owned or managed by the partner.

        See _Authentication and Authorization rules_ and
        _List methods rules_ for more information about this method.
      operationId: playmoviespartner.accounts.avails.list
      x-api-path-slug: v1accountsaccountidavails-get
      parameters:
      - in: path
        name: accountId
        description: REQUIRED
      - in: query
        name: altId
        description: Filter Avails that match a case-insensitive, partner-specific
          custom id
      - in: query
        name: altIds
        description: Filter Avails that match (case-insensitive) any of the given
          partner-specific custom ids
      - in: query
        name: pageSize
        description: See _List methods rules_ for info about this field
      - in: query
        name: pageToken
        description: See _List methods rules_ for info about this field
      - in: query
        name: pphNames
        description: See _List methods rules_ for info about this field
      - in: query
        name: studioNames
        description: See _List methods rules_ for info about this field
      - in: query
        name: territories
        description: 'Filter Avails that match (case-insensitive) any of the given
          country codes,using the ISO 3166-1 alpha-2 format (examples: US, us, Us)'
      - in: query
        name: title
        description: Filter that matches Avails with a `title_internal_alias`,`series_title_internal_alias`,
          `season_title_internal_alias`,or `episode_title_internal_alias` that contains
          the givencase-insensitive title
      - in: query
        name: videoIds
        description: Filter Avails that match any of the given `video_id`s
      responses:
        200:
          description: OK
      tags:
      - Movie
  /v1/accounts/{accountId}/avails/{availId}:
    get:
      summary: Get Available Movie
      description: Get an Avail given its avail group id and avail id.
      operationId: playmoviespartner.accounts.avails.get
      x-api-path-slug: v1accountsaccountidavailsavailid-get
      parameters:
      - in: path
        name: accountId
        description: REQUIRED
      - in: path
        name: availId
        description: REQUIRED
      responses:
        200:
          description: OK
      tags:
      - Movie
  /v1/accounts/{accountId}/orders:
    get:
      summary: Get Orders
      description: |-
        List Orders owned or managed by the partner.

        See _Authentication and Authorization rules_ and
        _List methods rules_ for more information about this method.
      operationId: playmoviespartner.accounts.orders.list
      x-api-path-slug: v1accountsaccountidorders-get
      parameters:
      - in: path
        name: accountId
        description: REQUIRED
      - in: query
        name: customId
        description: Filter Orders that match a case-insensitive, partner-specific
          custom id
      - in: query
        name: name
        description: Filter that matches Orders with a `name`, `show`, `season` or
          `episode`that contains the given case-insensitive name
      - in: query
        name: pageSize
        description: See _List methods rules_ for info about this field
      - in: query
        name: pageToken
        description: See _List methods rules_ for info about this field
      - in: query
        name: pphNames
        description: See _List methods rules_ for info about this field
      - in: query
        name: status
        description: Filter Orders that match one of the given status
      - in: query
        name: studioNames
        description: See _List methods rules_ for info about this field
      - in: query
        name: videoIds
        description: Filter Orders that match any of the given `video_id`s
      responses:
        200:
          description: OK
      tags:
      - Order
  /v1/accounts/{accountId}/orders/{orderId}:
    get:
      summary: Get Order
      description: |-
        Get an Order given its id.

        See _Authentication and Authorization rules_ and
        _Get methods rules_ for more information about this method.
      operationId: playmoviespartner.accounts.orders.get
      x-api-path-slug: v1accountsaccountidordersorderid-get
      parameters:
      - in: path
        name: accountId
        description: REQUIRED
      - in: path
        name: orderId
        description: REQUIRED
      responses:
        200:
          description: OK
      tags:
      - Order
  /v1/accounts/{accountId}/storeInfos:
    get:
      summary: Get Store Information
      description: |-
        List StoreInfos owned or managed by the partner.

        See _Authentication and Authorization rules_ and
        _List methods rules_ for more information about this method.
      operationId: playmoviespartner.accounts.storeInfos.list
      x-api-path-slug: v1accountsaccountidstoreinfos-get
      parameters:
      - in: path
        name: accountId
        description: REQUIRED
      - in: query
        name: countries
        description: 'Filter StoreInfos that match (case-insensitive) any of the given
          countrycodes, using the ISO 3166-1 alpha-2 format (examples: US, us, Us)'
      - in: query
        name: mids
        description: Filter StoreInfos that match any of the given `mid`s
      - in: query
        name: name
        description: Filter that matches StoreInfos with a `name` or `show_name`that
          contains the given case-insensitive name
      - in: query
        name: pageSize
        description: See _List methods rules_ for info about this field
      - in: query
        name: pageToken
        description: See _List methods rules_ for info about this field
      - in: query
        name: pphNames
        description: See _List methods rules_ for info about this field
      - in: query
        name: seasonIds
        description: Filter StoreInfos that match any of the given `season_id`s
      - in: query
        name: studioNames
        description: See _List methods rules_ for info about this field
      - in: query
        name: videoId
        description: Filter StoreInfos that match a given `video_id`
      - in: query
        name: videoIds
        description: Filter StoreInfos that match any of the given `video_id`s
      responses:
        200:
          description: OK
      tags:
      - Store
  /v1/accounts/{accountId}/storeInfos/{videoId}/country/{country}:
    get:
      summary: Get Video Country
      description: |-
        Get a StoreInfo given its video id and country.

        See _Authentication and Authorization rules_ and
        _Get methods rules_ for more information about this method.
      operationId: playmoviespartner.accounts.storeInfos.country.get
      x-api-path-slug: v1accountsaccountidstoreinfosvideoidcountrycountry-get
      parameters:
      - in: path
        name: accountId
        description: REQUIRED
      - in: path
        name: country
        description: REQUIRED
      - in: path
        name: videoId
        description: REQUIRED
      responses:
        200:
          description: OK
      tags:
      - Country