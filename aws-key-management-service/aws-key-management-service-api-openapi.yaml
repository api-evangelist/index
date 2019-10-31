swagger: "2.0"
x-collection-name: AWS Key Management Service
x-complete: 1
info:
  title: AWS Key Management Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CancelKeyDeletion:
    get:
      summary: Cancel Key Deletion
      description: Cancels the deletion of a customer master key (CMK).
      operationId: cancelKeyDeletion
      x-api-path-slug: actioncancelkeydeletion-get
      parameters:
      - in: query
        name: KeyId
        description: The unique identifier for the customer master key (CMK) for which
          to cancel      deletion
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=CreateAlias:
    get:
      summary: Create Alias
      description: Creates a display name for a customer master key.
      operationId: createAlias
      x-api-path-slug: actioncreatealias-get
      parameters:
      - in: query
        name: AliasName
        description: String that contains the display name
        type: string
      - in: query
        name: TargetKeyId
        description: An identifier of the key for which you are creating the alias
        type: string
      responses:
        200:
          description: OK
      tags:
      - Aliases
  /?Action=CreateGrant:
    get:
      summary: Create Grant
      description: Adds a grant to a key to specify who can use the key and under
        what conditions.
      operationId: createGrant
      x-api-path-slug: actioncreategrant-get
      parameters:
      - in: query
        name: Constraints
        description: The conditions under which the operations permitted by the grant
          are allowed
        type: string
      - in: query
        name: GranteePrincipal
        description: The principal that is given permission to perform the operations
          that the grant      permits
        type: string
      - in: query
        name: GrantTokens
        description: A list of grant tokens
        type: string
      - in: query
        name: KeyId
        description: The unique identifier for the customer master key (CMK) that
          the grant applies      to
        type: string
      - in: query
        name: Name
        description: A friendly name for identifying the grant
        type: string
      - in: query
        name: Operations
        description: A list of operations that the grant permits
        type: string
      - in: query
        name: RetiringPrincipal
        description: The principal that is given permission to retire the grant by
          using RetireGrant operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Grants
  /?Action=CreateKey:
    get:
      summary: Create Key
      description: Creates a customer master key (CMK).
      operationId: createKey
      x-api-path-slug: actioncreatekey-get
      parameters:
      - in: query
        name: BypassPolicyLockoutSafetyCheck
        description: A flag to indicate whether to bypass the key policy lockout safety
          check
        type: string
      - in: query
        name: Description
        description: A description of the CMK
        type: string
      - in: query
        name: KeyUsage
        description: The intended use of the CMK
        type: string
      - in: query
        name: Origin
        description: The source of the CMKs key material
        type: string
      - in: query
        name: Policy
        description: The key policy to attach to the CMK
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=Decrypt:
    get:
      summary: Decrypt
      description: Decrypts ciphertext.
      operationId: decrypt
      x-api-path-slug: actiondecrypt-get
      parameters:
      - in: query
        name: CiphertextBlob
        description: Ciphertext to be decrypted
        type: string
      - in: query
        name: EncryptionContext
        description: The encryption context
        type: string
      - in: query
        name: GrantTokens
        description: A list of grant tokens
        type: string
      responses:
        200:
          description: OK
      tags:
      - Decrypt
  /?Action=DeleteAlias:
    get:
      summary: Delete Alias
      description: Deletes the specified alias.
      operationId: deleteAlias
      x-api-path-slug: actiondeletealias-get
      parameters:
      - in: query
        name: AliasName
        description: The alias to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Aliases
  /?Action=DeleteImportedKeyMaterial:
    get:
      summary: Delete Imported Key Material
      description: |-
        Deletes key material that you previously imported and makes the specified customer
              master key (CMK) unusable.
      operationId: deleteImportedKeyMaterial
      x-api-path-slug: actiondeleteimportedkeymaterial-get
      parameters:
      - in: query
        name: KeyId
        description: The identifier of the CMK whose key material to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=DescribeKey:
    get:
      summary: Describe Key
      description: Provides detailed information about the specified customer master
        key.
      operationId: describeKey
      x-api-path-slug: actiondescribekey-get
      parameters:
      - in: query
        name: GrantTokens
        description: A list of grant tokens
        type: string
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=DisableKey:
    get:
      summary: Disable Key
      description: |-
        Sets the state of a customer master key (CMK) to disabled, thereby preventing its use
              for cryptographic operations.
      operationId: disableKey
      x-api-path-slug: actiondisablekey-get
      parameters:
      - in: query
        name: KeyId
        description: A unique identifier for the CMK
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=DisableKeyRotation:
    get:
      summary: Disable Key Rotation
      description: Disables rotation of the specified key.
      operationId: disableKeyRotation
      x-api-path-slug: actiondisablekeyrotation-get
      parameters:
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=EnableKey:
    get:
      summary: Enable Key
      description: Marks a key as enabled, thereby permitting its use.
      operationId: enableKey
      x-api-path-slug: actionenablekey-get
      parameters:
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=EnableKeyRotation:
    get:
      summary: Enable Key Rotation
      description: Enables rotation of the specified customer master key.
      operationId: enableKeyRotation
      x-api-path-slug: actionenablekeyrotation-get
      parameters:
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=Encrypt:
    get:
      summary: Encrypt
      description: Encrypts plaintext into ciphertext by using a customer master key.
      operationId: encrypt
      x-api-path-slug: actionencrypt-get
      parameters:
      - in: query
        name: EncryptionContext
        description: Name-value pair that specifies the encryption context to be used
          for authenticated      encryption
        type: string
      - in: query
        name: GrantTokens
        description: A list of grant tokens
        type: string
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key
        type: string
      - in: query
        name: Plaintext
        description: Data to be encrypted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Encrypt
  /?Action=GenerateDataKey:
    get:
      summary: Generate Data Key
      description: |-
        Returns a data encryption key that you can use in your application to encrypt
              data locally.
      operationId: generateDataKey
      x-api-path-slug: actiongeneratedatakey-get
      parameters:
      - in: query
        name: EncryptionContext
        description: A set of key-value pairs that represents additional authenticated
          data
        type: string
      - in: query
        name: GrantTokens
        description: A list of grant tokens
        type: string
      - in: query
        name: KeyId
        description: The identifier of the CMK under which to generate and encrypt
          the data encryption      key
        type: string
      - in: query
        name: KeySpec
        description: The length of the data encryption key
        type: string
      - in: query
        name: NumberOfBytes
        description: The length of the data encryption key in bytes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=GenerateDataKeyWithoutPlaintext:
    get:
      summary: Generate Data Key Without Plaintext
      description: Returns a data encryption key encrypted under a customer master
        key (CMK).
      operationId: generateDataKeyWithoutPlaintext
      x-api-path-slug: actiongeneratedatakeywithoutplaintext-get
      parameters:
      - in: query
        name: EncryptionContext
        description: A set of key-value pairs that represents additional authenticated
          data
        type: string
      - in: query
        name: GrantTokens
        description: A list of grant tokens
        type: string
      - in: query
        name: KeyId
        description: The identifier of the CMK under which to generate and encrypt
          the data encryption      key
        type: string
      - in: query
        name: KeySpec
        description: The length of the data encryption key
        type: string
      - in: query
        name: NumberOfBytes
        description: The length of the data encryption key in bytes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=GenerateRandom:
    get:
      summary: Generate Random
      description: Generates an unpredictable byte string.
      operationId: generateRandom
      x-api-path-slug: actiongeneraterandom-get
      parameters:
      - in: query
        name: NumberOfBytes
        description: The length of the byte string
        type: string
      responses:
        200:
          description: OK
      tags:
      - Randoms
  /?Action=GetKeyPolicy:
    get:
      summary: Get Key Policy
      description: Retrieves a policy attached to the specified key.
      operationId: getKeyPolicy
      x-api-path-slug: actiongetkeypolicy-get
      parameters:
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key
        type: string
      - in: query
        name: PolicyName
        description: String that contains the name of the policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Policies
  /?Action=GetKeyRotationStatus:
    get:
      summary: Get Key Rotation Status
      description: |-
        Retrieves a Boolean value that indicates whether key rotation is enabled for the
              specified key.
      operationId: getKeyRotationStatus
      x-api-path-slug: actiongetkeyrotationstatus-get
      parameters:
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=GetParametersForImport:
    get:
      summary: Get Parameters For Import
      description: |-
        Returns the items you need in order to import key material into AWS KMS from your
              existing key management infrastructure.
      operationId: getParametersForImport
      x-api-path-slug: actiongetparametersforimport-get
      parameters:
      - in: query
        name: KeyId
        description: The identifier of the CMK into which you will import key material
        type: string
      - in: query
        name: WrappingAlgorithm
        description: The algorithm you will use to encrypt the key material before
          importing it with ImportKeyMaterial
        type: string
      - in: query
        name: WrappingKeySpec
        description: The type of wrapping key (public key) to return in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameters
  /?Action=ImportKeyMaterial:
    get:
      summary: Import Key Material
      description: |-
        Imports key material into an AWS KMS customer master key (CMK) from your existing key
              management infrastructure.
      operationId: importKeyMaterial
      x-api-path-slug: actionimportkeymaterial-get
      parameters:
      - in: query
        name: EncryptedKeyMaterial
        description: The encrypted key material to import
        type: string
      - in: query
        name: ExpirationModel
        description: Specifies whether the key material expires
        type: string
      - in: query
        name: ImportToken
        description: The import token that you received in the response to a previous
          GetParametersForImport request
        type: string
      - in: query
        name: KeyId
        description: The identifier of the CMK to import the key material into
        type: string
      - in: query
        name: ValidTo
        description: The time at which the imported key material expires
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=ListAliases:
    get:
      summary: List Aliases
      description: Lists all of the key aliases in the account.
      operationId: listAliases
      x-api-path-slug: actionlistaliases-get
      parameters:
      - in: query
        name: Limit
        description: When paginating results, specify the maximum number of items
          to return in the response
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only in a
          subsequent request after      you receive a response with truncated results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Aliases
  /?Action=ListGrants:
    get:
      summary: List Grants
      description: List the grants for a specified key.
      operationId: listGrants
      x-api-path-slug: actionlistgrants-get
      parameters:
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key
        type: string
      - in: query
        name: Limit
        description: When paginating results, specify the maximum number of items
          to return in the response
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only in a
          subsequent request after      you receive a response with truncated results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Grants
  /?Action=ListKeyPolicies:
    get:
      summary: List Key Policies
      description: Retrieves a list of policies attached to a key.
      operationId: listKeyPolicies
      x-api-path-slug: actionlistkeypolicies-get
      parameters:
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key (CMK)
        type: string
      - in: query
        name: Limit
        description: When paginating results, specify the maximum number of items
          to return in the response
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only in a
          subsequent request after      you receive a response with truncated results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=ListKeys:
    get:
      summary: List Keys
      description: Lists the customer master keys.
      operationId: listKeys
      x-api-path-slug: actionlistkeys-get
      parameters:
      - in: query
        name: Limit
        description: When paginating results, specify the maximum number of items
          to return in the response
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only in a
          subsequent request after      you receive a response with truncated results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=ListRetirableGrants:
    get:
      summary: List Retirable Grants
      description: |-
        Returns a list of all grants for which the grant's RetiringPrincipal
              matches the one specified.
      operationId: listRetirableGrants
      x-api-path-slug: actionlistretirablegrants-get
      parameters:
      - in: query
        name: Limit
        description: When paginating results, specify the maximum number of items
          to return in the response
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only in a
          subsequent request after      you receive a response with truncated results
        type: string
      - in: query
        name: RetiringPrincipal
        description: The retiring principal for which to list grants
        type: string
      responses:
        200:
          description: OK
      tags:
      - Grants
  /?Action=PutKeyPolicy:
    get:
      summary: Put Key Policy
      description: Attaches a key policy to the specified customer master key (CMK).
      operationId: putKeyPolicy
      x-api-path-slug: actionputkeypolicy-get
      parameters:
      - in: query
        name: BypassPolicyLockoutSafetyCheck
        description: A flag to indicate whether to bypass the key policy lockout safety
          check
        type: string
      - in: query
        name: KeyId
        description: A unique identifier for the CMK
        type: string
      - in: query
        name: Policy
        description: The key policy to attach to the CMK
        type: string
      - in: query
        name: PolicyName
        description: The name of the key policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=ReEncrypt:
    get:
      summary: Re Encrypt
      description: |-
        Encrypts data on the server side with a new customer master key (CMK) without exposing
              the plaintext of the data on the client side.
      operationId: reEncrypt
      x-api-path-slug: actionreencrypt-get
      parameters:
      - in: query
        name: CiphertextBlob
        description: Ciphertext of the data to reencrypt
        type: string
      - in: query
        name: DestinationEncryptionContext
        description: Encryption context to use when the data is reencrypted
        type: string
      - in: query
        name: DestinationKeyId
        description: A unique identifier for the CMK to use to reencrypt the data
        type: string
      - in: query
        name: GrantTokens
        description: A list of grant tokens
        type: string
      - in: query
        name: SourceEncryptionContext
        description: Encryption context used to encrypt and decrypt the data specified
          in the        CiphertextBlob parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Encrypt
  /?Action=RetireGrant:
    get:
      summary: Retire Grant
      description: Retires a grant.
      operationId: retireGrant
      x-api-path-slug: actionretiregrant-get
      parameters:
      - in: query
        name: GrantId
        description: Unique identifier of the grant to retire
        type: string
      - in: query
        name: GrantToken
        description: Token that identifies the grant to be retired
        type: string
      - in: query
        name: KeyId
        description: The Amazon Resource Name of the CMK associated with the grant
        type: string
      responses:
        200:
          description: OK
      tags:
      - Grants
  /?Action=RevokeGrant:
    get:
      summary: Revoke Grant
      description: Revokes a grant.
      operationId: revokeGrant
      x-api-path-slug: actionrevokegrant-get
      parameters:
      - in: query
        name: GrantId
        description: Identifier of the grant to be revoked
        type: string
      - in: query
        name: KeyId
        description: A unique identifier for the customer master key associated with
          the grant
        type: string
      responses:
        200:
          description: OK
      tags:
      - Grants
  /?Action=ScheduleKeyDeletion:
    get:
      summary: Schedule Key Deletion
      description: Schedules the deletion of a customer master key (CMK).
      operationId: scheduleKeyDeletion
      x-api-path-slug: actionschedulekeydeletion-get
      parameters:
      - in: query
        name: KeyId
        description: The unique identifier for the customer master key (CMK) to delete
        type: string
      - in: query
        name: PendingWindowInDays
        description: The waiting period, specified in number of days
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys
  /?Action=UpdateAlias:
    get:
      summary: Update Alias
      description: Updates an alias to map it to a different key.
      operationId: updateAlias
      x-api-path-slug: actionupdatealias-get
      parameters:
      - in: query
        name: AliasName
        description: String that contains the name of the alias to be modified
        type: string
      - in: query
        name: TargetKeyId
        description: Unique identifier of the customer master key to be mapped to
          the alias
        type: string
      responses:
        200:
          description: OK
      tags:
      - Aliases
  /?Action=UpdateKeyDescription:
    get:
      summary: Update Key Description
      description: Updates the description of a customer master key (CMK).
      operationId: updateKeyDescription
      x-api-path-slug: actionupdatekeydescription-get
      parameters:
      - in: query
        name: Description
        description: New description for the CMK
        type: string
      - in: query
        name: KeyId
        description: A unique identifier for the CMK
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys