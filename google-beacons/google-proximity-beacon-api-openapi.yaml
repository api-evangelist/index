swagger: "2.0"
x-collection-name: Google Beacons
x-complete: 1
info:
  title: Google Proximity Beacon
  description: registers-manages-indexes-and-searches-beacons-
  contact:
    name: Google
    url: https://google.com
  version: v1beta1
host: proximitybeacon.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1beta1/beaconinfo:getforobserved:
    post:
      summary: Get Observed Beacon Info
      description: |-
        Given one or more beacon observations, returns any beacon information
        and attachments accessible to your application. Authorize by using the
        [API key](https://developers.google.com/beacons/proximity/how-tos/authorizing#APIKey)
        for the application.
      operationId: proximitybeacon.beaconinfo.getforobserved
      x-api-path-slug: v1beta1beaconinfogetforobserved-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Beacon
  /v1beta1/beacons:
    get:
      summary: Search Beacons
      description: |-
        Searches the beacon registry for beacons that match the given search
        criteria. Only those beacons that the client has permission to list
        will be returned.

        Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
        from a signed-in user with **viewer**, **Is owner** or **Can edit**
        permissions in the Google Developers Console project.
      operationId: proximitybeacon.beacons.list
      x-api-path-slug: v1beta1beacons-get
      parameters:
      - in: query
        name: pageSize
        description: The maximum number of records to return for this request, up
          to aserver-defined upper limit
      - in: query
        name: pageToken
        description: A pagination token obtained from a previous request to list beacons
      - in: query
        name: projectId
        description: The project id to list beacons under
      - in: query
        name: q
        description: 'Filter query string that supports the following field filters:*
          **description:``**  For example: **description:Room 3**  Returns beacons
          whose description matches tokens in the string Room 3  (not necessarily
          that exact string)'
      responses:
        200:
          description: OK
      tags:
      - Beacon
  /v1beta1/beacons:register:
    post:
      summary: Register Beacon
      description: |-
        Registers a previously unregistered beacon given its `advertisedId`.
        These IDs are unique within the system. An ID can be registered only once.

        Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
        from a signed-in user with **Is owner** or **Can edit** permissions in the
        Google Developers Console project.
      operationId: proximitybeacon.beacons.register
      x-api-path-slug: v1beta1beaconsregister-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: projectId
        description: The project id of the project the beacon will be registered to
      responses:
        200:
          description: OK
      tags:
      - Beacon
  /v1beta1/eidparams:
    get:
      summary: Get Beacon Parameters
      description: |-
        Gets the Proximity Beacon API's current public key and associated
        parameters used to initiate the Diffie-Hellman key exchange required to
        register a beacon that broadcasts the Eddystone-EID format. This key
        changes periodically; clients may cache it and re-use the same public key
        to provision and register multiple beacons. However, clients should be
        prepared to refresh this key when they encounter an error registering an
        Eddystone-EID beacon.
      operationId: proximitybeacon.getEidparams
      x-api-path-slug: v1beta1eidparams-get
      responses:
        200:
          description: OK
      tags:
      - Beacon
  /v1beta1/namespaces:
    get:
      summary: Get Namespace
      description: |-
        Lists all attachment namespaces owned by your Google Developers Console
        project. Attachment data associated with a beacon must include a
        namespaced type, and the namespace must be owned by your project.

        Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
        from a signed-in user with **viewer**, **Is owner** or **Can edit**
        permissions in the Google Developers Console project.
      operationId: proximitybeacon.namespaces.list
      x-api-path-slug: v1beta1namespaces-get
      parameters:
      - in: query
        name: projectId
        description: The project id to list namespaces under
      responses:
        200:
          description: OK
      tags:
      - Namespace
  /v1beta1/{attachmentName}:
    delete:
      summary: Delete Attachment
      description: |-
        Deletes the specified attachment for the given beacon. Each attachment has
        a unique attachment name (`attachmentName`) which is returned when you
        fetch the attachment data via this API. You specify this with the delete
        request to control which attachment is removed. This operation cannot be
        undone.

        Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
        from a signed-in user with **Is owner** or **Can edit** permissions in the
        Google Developers Console project.
      operationId: proximitybeacon.beacons.attachments.delete
      x-api-path-slug: v1beta1attachmentname-delete
      parameters:
      - in: path
        name: attachmentName
        description: The attachment name (`attachmentName`) ofthe attachment to remove
      - in: query
        name: projectId
        description: The project id of the attachment to delete
      responses:
        200:
          description: OK
      tags:
      - Attachment
  /v1beta1/{beaconName}:
    delete:
      summary: Delete Beacon
      description: |-
        Deletes the specified beacon including all diagnostics data for the beacon
        as well as any attachments on the beacon (including those belonging to
        other projects). This operation cannot be undone.

        Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
        from a signed-in user with **Is owner** or **Can edit** permissions in the
        Google Developers Console project.
      operationId: proximitybeacon.beacons.delete
      x-api-path-slug: v1beta1beaconname-delete
      parameters:
      - in: path
        name: beaconName
        description: Beacon that should be deleted
      - in: query
        name: projectId
        description: The project id of the beacon to delete
      responses:
        200:
          description: OK
      tags:
      - Beacon
    get:
      summary: Get Beacon
      description: |-
        Returns detailed information about the specified beacon.

        Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
        from a signed-in user with **viewer**, **Is owner** or **Can edit**
        permissions in the Google Developers Console project.

        Requests may supply an Eddystone-EID beacon name in the form:
        `beacons/4!beaconId` where the `beaconId` is the base16 ephemeral ID
        broadcast by the beacon. The returned `Beacon` object will contain the
        beacon's stable Eddystone-UID. Clients not authorized to resolve the
        beacon's ephemeral Eddystone-EID broadcast will receive an error.
      operationId: proximitybeacon.beacons.get
      x-api-path-slug: v1beta1beaconname-get
      parameters:
      - in: path
        name: beaconName
        description: Resource name of this beacon
      - in: query
        name: projectId
        description: The project id of the beacon to request
      responses:
        200:
          description: OK
      tags:
      - Beacon
    put:
      summary: Update Beacon
      description: |-
        Updates the information about the specified beacon. **Any field that you do
        not populate in the submitted beacon will be permanently erased**, so you
        should follow the "read, modify, write" pattern to avoid inadvertently
        destroying data.

        Changes to the beacon status via this method will be  silently ignored.
        To update beacon status, use the separate methods on this API for
        activation, deactivation, and decommissioning.
        Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
        from a signed-in user with **Is owner** or **Can edit** permissions in the
        Google Developers Console project.
      operationId: proximitybeacon.beacons.update
      x-api-path-slug: v1beta1beaconname-put
      parameters:
      - in: path
        name: beaconName
        description: Resource name of this beacon
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: projectId
        description: The project id of the beacon to update
      responses:
        200:
          description: OK
      tags:
      - Beacon
  /v1beta1/{beaconName}/attachments:
    get:
      summary: Get Attachments
      description: |-
        Returns the attachments for the specified beacon that match the specified
        namespaced-type pattern.

        To control which namespaced types are returned, you add the
        `namespacedType` query parameter to the request. You must either use
        `*/*`, to return all attachments, or the namespace must be one of
        the ones returned from the  `namespaces` endpoint.

        Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
        from a signed-in user with **viewer**, **Is owner** or **Can edit**
        permissions in the Google Developers Console project.
      operationId: proximitybeacon.beacons.attachments.list
      x-api-path-slug: v1beta1beaconnameattachments-get
      parameters:
      - in: path
        name: beaconName
        description: Beacon whose attachments should be fetched
      - in: query
        name: namespacedType
        description: Specifies the namespace and type of attachment to include in
          response innamespace/type format
      - in: query
        name: projectId
        description: The project id to list beacon attachments under
      responses:
        200:
          description: OK
      tags:
      - Attachment
    post:
      summary: Add Attachment
      description: |-
        Associates the given data with the specified beacon. Attachment data must
        contain two parts:
        <ul>
        <li>A namespaced type.</li>
        <li>The actual attachment data itself.</li>
        </ul>
        The namespaced type consists of two parts, the namespace and the type.
        The namespace must be one of the values returned by the `namespaces`
        endpoint, while the type can be a string of any characters except for the
        forward slash (`/`) up to 100 characters in length.

        Attachment data can be up to 1024 bytes long.

        Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
        from a signed-in user with **Is owner** or **Can edit** permissions in the
        Google Developers Console project.
      operationId: proximitybeacon.beacons.attachments.create
      x-api-path-slug: v1beta1beaconnameattachments-post
      parameters:
      - in: path
        name: beaconName
        description: Beacon on which the attachment should be created
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: projectId
        description: The project id of the project the attachment will belong to
      responses:
        200:
          description: OK
      tags:
      - Attachment
  /v1beta1/{beaconName}/attachments:batchDelete:
    post:
      summary: Delete Attachments
      description: |-
        Deletes multiple attachments on a given beacon. This operation is
        permanent and cannot be undone.

        You can optionally specify `namespacedType` to choose which attachments
        should be deleted. If you do not specify `namespacedType`,  all your
        attachments on the given beacon will be deleted. You also may explicitly
        specify `*/*` to delete all.

        Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
        from a signed-in user with **Is owner** or **Can edit** permissions in the
        Google Developers Console project.
      operationId: proximitybeacon.beacons.attachments.batchDelete
      x-api-path-slug: v1beta1beaconnameattachmentsbatchdelete-post
      parameters:
      - in: path
        name: beaconName
        description: The beacon whose attachments should be deleted
      - in: query
        name: namespacedType
        description: Specifies the namespace and type of attachments to delete in`namespace/type`
          format
      - in: query
        name: projectId
        description: The project id to delete beacon attachments under
      responses:
        200:
          description: OK
      tags:
      - Attachment
  /v1beta1/{beaconName}/diagnostics:
    get:
      summary: Get Diagnostics
      description: |-
        List the diagnostics for a single beacon. You can also list diagnostics for
        all the beacons owned by your Google Developers Console project by using
        the beacon name `beacons/-`.

        Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
        from a signed-in user with **viewer**, **Is owner** or **Can edit**
        permissions in the Google Developers Console project.
      operationId: proximitybeacon.beacons.diagnostics.list
      x-api-path-slug: v1beta1beaconnamediagnostics-get
      parameters:
      - in: query
        name: alertFilter
        description: Requests only beacons that have the given alert
      - in: path
        name: beaconName
        description: Beacon that the diagnostics are for
      - in: query
        name: pageSize
        description: Specifies the maximum number of results to return
      - in: query
        name: pageToken
        description: Requests results that occur after the `page_token`, obtained
          from theresponse to a previous request
      - in: query
        name: projectId
        description: Requests only diagnostic records for the given project id
      responses:
        200:
          description: OK
      tags:
      - Diagnostic
  /v1beta1/{beaconName}:activate:
    post:
      summary: Activate Beacon
      description: |-
        Activates a beacon. A beacon that is active will return information
        and attachment data when queried via `beaconinfo.getforobserved`.
        Calling this method on an already active beacon will do nothing (but
        will return a successful response code).

        Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
        from a signed-in user with **Is owner** or **Can edit** permissions in the
        Google Developers Console project.
      operationId: proximitybeacon.beacons.activate
      x-api-path-slug: v1beta1beaconnameactivate-post
      parameters:
      - in: path
        name: beaconName
        description: Beacon that should be activated
      - in: query
        name: projectId
        description: The project id of the beacon to activate
      responses:
        200:
          description: OK
      tags:
      - Beacon
  /v1beta1/{beaconName}:deactivate:
    post:
      summary: Deactivate Beacon
      description: |-
        Deactivates a beacon. Once deactivated, the API will not return
        information nor attachment data for the beacon when queried via
        `beaconinfo.getforobserved`. Calling this method on an already inactive
        beacon will do nothing (but will return a successful response code).

        Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
        from a signed-in user with **Is owner** or **Can edit** permissions in the
        Google Developers Console project.
      operationId: proximitybeacon.beacons.deactivate
      x-api-path-slug: v1beta1beaconnamedeactivate-post
      parameters:
      - in: path
        name: beaconName
        description: Beacon that should be deactivated
      - in: query
        name: projectId
        description: The project id of the beacon to deactivate
      responses:
        200:
          description: OK
      tags:
      - Beacon
  /v1beta1/{beaconName}:decommission:
    post:
      summary: Decomission Beacon
      description: |-
        Decommissions the specified beacon in the service. This beacon will no
        longer be returned from `beaconinfo.getforobserved`. This operation is
        permanent -- you will not be able to re-register a beacon with this ID
        again.

        Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
        from a signed-in user with **Is owner** or **Can edit** permissions in the
        Google Developers Console project.
      operationId: proximitybeacon.beacons.decommission
      x-api-path-slug: v1beta1beaconnamedecommission-post
      parameters:
      - in: path
        name: beaconName
        description: Beacon that should be decommissioned
      - in: query
        name: projectId
        description: The project id of the beacon to decommission
      responses:
        200:
          description: OK
      tags:
      - Beacon
  /v1beta1/{namespaceName}:
    put:
      summary: Update Namespace
      description: |-
        Updates the information about the specified namespace. Only the namespace
        visibility can be updated.
      operationId: proximitybeacon.namespaces.update
      x-api-path-slug: v1beta1namespacename-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaceName
        description: Resource name of this namespace
      - in: query
        name: projectId
        description: The project id of the namespace to update
      responses:
        200:
          description: OK
      tags:
      - Namespace