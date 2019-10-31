swagger: "2.0"
x-collection-name: Google Cloud Key Management Service
x-complete: 1
info:
  title: Google Cloud Key Management Service (KMS)
  description: manages-encryption-for-your-cloud-services-the-same-way-you-do-onpremise--you-can-generate-use-rotate-and-destroy-aes256-encryption-keys-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: cloudkms.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:
    get:
      summary: Get Key
      description: Returns metadata for a given CryptoKeyVersion.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.cryptoKeyVersions.get
      x-api-path-slug: v1name-get
      parameters:
      - in: path
        name: name
        description: The name of the CryptoKeyVersion to get
      responses:
        200:
          description: OK
      tags:
      - Key
    patch:
      summary: Update Key
      description: |-
        Update a CryptoKeyVersion's metadata.

        state may be changed between
        ENABLED and
        DISABLED using this
        method. See DestroyCryptoKeyVersion and RestoreCryptoKeyVersion to
        move between other states.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.cryptoKeyVersions.patch
      x-api-path-slug: v1name-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: Output only
      - in: query
        name: updateMask
        description: Required list of fields to be updated in this request
      responses:
        200:
          description: OK
      tags:
      - Key
  /v1/{name}/locations:
    get:
      summary: Get Locations
      description: Lists information about the supported locations for this service.
      operationId: cloudkms.projects.locations.list
      x-api-path-slug: v1namelocations-get
      parameters:
      - in: query
        name: filter
        description: The standard list filter
      - in: path
        name: name
        description: The resource that owns the locations collection, if applicable
      - in: query
        name: pageSize
        description: The standard list page size
      - in: query
        name: pageToken
        description: The standard list page token
      responses:
        200:
          description: OK
      tags:
      - Location
  /v1/{name}:decrypt:
    post:
      summary: Decrypt Data
      description: Decrypt data that was protected by Encrypt.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.decrypt
      x-api-path-slug: v1namedecrypt-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Location
  /v1/{name}:destroy:
    post:
      summary: Destroy Key
      description: |-
        Schedule a CryptoKeyVersion for destruction.

        Upon calling this method, CryptoKeyVersion.state will be set to
        DESTROY_SCHEDULED
        and destroy_time will be set to a time 24
        hours in the future, at which point the state
        will be changed to
        DESTROYED, and the key
        material will be irrevocably destroyed.

        Before the destroy_time is reached,
        RestoreCryptoKeyVersion may be called to reverse the process.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.cryptoKeyVersions.destroy
      x-api-path-slug: v1namedestroy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The resource name of the CryptoKeyVersion to destroy
      responses:
        200:
          description: OK
      tags:
      - Key
  /v1/{name}:encrypt:
    post:
      summary: Encrypt Data
      description: Encrypt data, so that it can only be recovered by a call to Decrypt.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.encrypt
      x-api-path-slug: v1nameencrypt-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Encryption
  /v1/{name}:restore:
    post:
      summary: Restore Key
      description: |-
        Restore a CryptoKeyVersion in the
        DESTROY_SCHEDULED,
        state.

        Upon restoration of the CryptoKeyVersion, state
        will be set to DISABLED,
        and destroy_time will be cleared.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.cryptoKeyVersions.restore
      x-api-path-slug: v1namerestore-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The resource name of the CryptoKeyVersion to restore
      responses:
        200:
          description: OK
      tags:
      - Key
  /v1/{name}:updatePrimaryVersion:
    post:
      summary: Update Version
      description: Update the version of a CryptoKey that will be used in Encrypt
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.updatePrimaryVersion
      x-api-path-slug: v1nameupdateprimaryversion-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The resource name of the CryptoKey to update
      responses:
        200:
          description: OK
      tags:
      - Version
  /v1/{parent}/cryptoKeyVersions:
    get:
      summary: List Key Versions
      description: Lists CryptoKeyVersions.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.cryptoKeyVersions.list
      x-api-path-slug: v1parentcryptokeyversions-get
      parameters:
      - in: query
        name: pageSize
        description: Optional limit on the number of CryptoKeyVersions toinclude in
          the response
      - in: query
        name: pageToken
        description: Optional pagination token, returned earlier viaListCryptoKeyVersionsResponse
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Key Version
    post:
      summary: Create Key Version
      description: |-
        Create a new CryptoKeyVersion in a CryptoKey.

        The server will assign the next sequential id. If unset,
        state will be set to
        ENABLED.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.cryptoKeyVersions.create
      x-api-path-slug: v1parentcryptokeyversions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Key Version
  /v1/{parent}/cryptoKeys:
    get:
      summary: List Keys
      description: Lists CryptoKeys.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.list
      x-api-path-slug: v1parentcryptokeys-get
      parameters:
      - in: query
        name: pageSize
        description: Optional limit on the number of CryptoKeys to include in theresponse
      - in: query
        name: pageToken
        description: Optional pagination token, returned earlier viaListCryptoKeysResponse
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Key
    post:
      summary: Create Key
      description: |-
        Create a new CryptoKey within a KeyRing.

        CryptoKey.purpose is required.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.create
      x-api-path-slug: v1parentcryptokeys-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: cryptoKeyId
        description: Required
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Key
  /v1/{parent}/keyRings:
    get:
      summary: List Key Rings
      description: Lists KeyRings.
      operationId: cloudkms.projects.locations.keyRings.list
      x-api-path-slug: v1parentkeyrings-get
      parameters:
      - in: query
        name: pageSize
        description: Optional limit on the number of KeyRings to include in theresponse
      - in: query
        name: pageToken
        description: Optional pagination token, returned earlier viaListKeyRingsResponse
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Key Ring
    post:
      summary: Create Key Ring
      description: Create a new KeyRing in a given Project and Location.
      operationId: cloudkms.projects.locations.keyRings.create
      x-api-path-slug: v1parentkeyrings-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: keyRingId
        description: Required
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Key Ring
  /v1/{resource}:getIamPolicy:
    get:
      summary: Get IAM Policy
      description: |-
        Gets the access control policy for a resource.
        Returns an empty policy if the resource exists and does not have a policy
        set.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.getIamPolicy
      x-api-path-slug: v1resourcegetiampolicy-get
      parameters:
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy is being requested'
      responses:
        200:
          description: OK
      tags:
      - IAM Policy
  /v1/{resource}:setIamPolicy:
    post:
      summary: Set IAM Policy
      description: |-
        Sets the access control policy on the specified resource. Replaces any
        existing policy.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.setIamPolicy
      x-api-path-slug: v1resourcesetiampolicy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy is being specified'
      responses:
        200:
          description: OK
      tags:
      - IAM Policy
  /v1/{resource}:testIamPermissions:
    post:
      summary: Test IAM Permissions
      description: |-
        Returns permissions that a caller has on the specified resource.
        If the resource does not exist, this will return an empty set of
        permissions, not a NOT_FOUND error.

        Note: This operation is designed to be used for building permission-aware
        UIs and command-line tools, not for authorization checking. This operation
        may "fail open" without warning.
      operationId: cloudkms.projects.locations.keyRings.cryptoKeys.testIamPermissions
      x-api-path-slug: v1resourcetestiampermissions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy detail is being
          requested'
      responses:
        200:
          description: OK
      tags:
      - IAM Permission