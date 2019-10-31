swagger: "2.0"
x-collection-name: Google Cloud Storage
x-complete: 1
info:
  title: Google Cloud Storage
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /b:
    get:
      summary: Get Buckets
      description: Retrieves a list of buckets for a given project.
      operationId: storage.buckets.list
      x-api-path-slug: b-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of buckets to return in a single response
      - in: query
        name: pageToken
        description: A previously-returned page token representing part of the larger
          set of results to view
      - in: query
        name: prefix
        description: Filter results to buckets whose names begin with this prefix
      - in: query
        name: project
        description: A valid API project identifier
      - in: query
        name: projection
        description: Set of properties to return
      responses:
        200:
          description: OK
      tags:
      - Bucket
    post:
      summary: Create Bucket
      description: Creates a new bucket.
      operationId: storage.buckets.insert
      x-api-path-slug: b-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: predefinedAcl
        description: Apply a predefined set of access controls to this bucket
      - in: query
        name: predefinedDefaultObjectAcl
        description: Apply a predefined set of default object access controls to this
          bucket
      - in: query
        name: project
        description: A valid API project identifier
      - in: query
        name: projection
        description: Set of properties to return
      responses:
        200:
          description: OK
      tags:
      - Bucket
  /b/{bucket}:
    delete:
      summary: Delete Bucket
      description: Permanently deletes an empty bucket.
      operationId: storage.buckets.delete
      x-api-path-slug: bbucket-delete
      parameters:
      - in: path
        name: bucket
        description: Name of a bucket
      - in: query
        name: ifMetagenerationMatch
        description: If set, only deletes the bucket if its metageneration matches
          this value
      - in: query
        name: ifMetagenerationNotMatch
        description: If set, only deletes the bucket if its metageneration does not
          match this value
      responses:
        200:
          description: OK
      tags:
      - Bucket
    get:
      summary: Get Bucket
      description: Returns metadata for the specified bucket.
      operationId: storage.buckets.get
      x-api-path-slug: bbucket-get
      parameters:
      - in: path
        name: bucket
        description: Name of a bucket
      - in: query
        name: ifMetagenerationMatch
        description: Makes the return of the bucket metadata conditional on whether
          the buckets current metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the return of the bucket metadata conditional on whether
          the buckets current metageneration does not match the given value
      - in: query
        name: projection
        description: Set of properties to return
      responses:
        200:
          description: OK
      tags:
      - Bucket
    patch:
      summary: Update bucket
      description: Updates a bucket. Changes to the bucket will be readable immediately
        after writing, but configuration changes may take time to propagate. This
        method supports patch semantics.
      operationId: storage.buckets.patch
      x-api-path-slug: bbucket-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of a bucket
      - in: query
        name: ifMetagenerationMatch
        description: Makes the return of the bucket metadata conditional on whether
          the buckets current metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the return of the bucket metadata conditional on whether
          the buckets current metageneration does not match the given value
      - in: query
        name: predefinedAcl
        description: Apply a predefined set of access controls to this bucket
      - in: query
        name: predefinedDefaultObjectAcl
        description: Apply a predefined set of default object access controls to this
          bucket
      - in: query
        name: projection
        description: Set of properties to return
      responses:
        200:
          description: OK
      tags:
      - Bucket
    put:
      summary: Update bucket
      description: Updates a bucket. Changes to the bucket will be readable immediately
        after writing, but configuration changes may take time to propagate.
      operationId: storage.buckets.update
      x-api-path-slug: bbucket-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of a bucket
      - in: query
        name: ifMetagenerationMatch
        description: Makes the return of the bucket metadata conditional on whether
          the buckets current metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the return of the bucket metadata conditional on whether
          the buckets current metageneration does not match the given value
      - in: query
        name: predefinedAcl
        description: Apply a predefined set of access controls to this bucket
      - in: query
        name: predefinedDefaultObjectAcl
        description: Apply a predefined set of default object access controls to this
          bucket
      - in: query
        name: projection
        description: Set of properties to return
      responses:
        200:
          description: OK
      tags:
      - Bucket
  /b/{bucket}/acl:
    get:
      summary: Get Bucket ACLs
      description: Retrieves ACL entries on the specified bucket.
      operationId: storage.bucketAccessControls.list
      x-api-path-slug: bbucketacl-get
      parameters:
      - in: path
        name: bucket
        description: Name of a bucket
      responses:
        200:
          description: OK
      tags:
      - Bucket ACL
    post:
      summary: Create Bucket ACL
      description: Creates a new ACL entry on the specified bucket.
      operationId: storage.bucketAccessControls.insert
      x-api-path-slug: bbucketacl-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of a bucket
      responses:
        200:
          description: OK
      tags:
      - Bucket ACL
  /b/{bucket}/acl/{entity}:
    delete:
      summary: Delete Bucket ACL
      description: Permanently deletes the ACL entry for the specified entity on the
        specified bucket.
      operationId: storage.bucketAccessControls.delete
      x-api-path-slug: bbucketaclentity-delete
      parameters:
      - in: path
        name: bucket
        description: Name of a bucket
      - in: path
        name: entity
        description: The entity holding the permission
      responses:
        200:
          description: OK
      tags:
      - Bucket ACL
    get:
      summary: Get Bucket ACL
      description: Returns the ACL entry for the specified entity on the specified
        bucket.
      operationId: storage.bucketAccessControls.get
      x-api-path-slug: bbucketaclentity-get
      parameters:
      - in: path
        name: bucket
        description: Name of a bucket
      - in: path
        name: entity
        description: The entity holding the permission
      responses:
        200:
          description: OK
      tags:
      - Bucket ACL
    patch:
      summary: Update Bucket ACL
      description: Updates an ACL entry on the specified bucket. This method supports
        patch semantics.
      operationId: storage.bucketAccessControls.patch
      x-api-path-slug: bbucketaclentity-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of a bucket
      - in: path
        name: entity
        description: The entity holding the permission
      responses:
        200:
          description: OK
      tags:
      - Bucket ACL
    put:
      summary: Update Bucket ACL
      description: Updates an ACL entry on the specified bucket.
      operationId: storage.bucketAccessControls.update
      x-api-path-slug: bbucketaclentity-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of a bucket
      - in: path
        name: entity
        description: The entity holding the permission
      responses:
        200:
          description: OK
      tags:
      - Bucket ACL
  /b/{bucket}/defaultObjectAcl:
    get:
      summary: Get Bucket Default ACL
      description: Retrieves default object ACL entries on the specified bucket.
      operationId: storage.defaultObjectAccessControls.list
      x-api-path-slug: bbucketdefaultobjectacl-get
      parameters:
      - in: path
        name: bucket
        description: Name of a bucket
      - in: query
        name: ifMetagenerationMatch
        description: If present, only return default ACL listing if the buckets current
          metageneration matches this value
      - in: query
        name: ifMetagenerationNotMatch
        description: If present, only return default ACL listing if the buckets current
          metageneration does not match the given value
      responses:
        200:
          description: OK
      tags:
      - Bucket ACL
    post:
      summary: Create Bucket Default ACL
      description: Creates a new default object ACL entry on the specified bucket.
      operationId: storage.defaultObjectAccessControls.insert
      x-api-path-slug: bbucketdefaultobjectacl-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of a bucket
      responses:
        200:
          description: OK
      tags:
      - Bucket ACL
  /b/{bucket}/defaultObjectAcl/{entity}:
    delete:
      summary: Default Bucket Default ACL
      description: Permanently deletes the default object ACL entry for the specified
        entity on the specified bucket.
      operationId: storage.defaultObjectAccessControls.delete
      x-api-path-slug: bbucketdefaultobjectaclentity-delete
      parameters:
      - in: path
        name: bucket
        description: Name of a bucket
      - in: path
        name: entity
        description: The entity holding the permission
      responses:
        200:
          description: OK
      tags:
      - Bucket ACL
    get:
      summary: Get Bucket Default ACL
      description: Returns the default object ACL entry for the specified entity on
        the specified bucket.
      operationId: storage.defaultObjectAccessControls.get
      x-api-path-slug: bbucketdefaultobjectaclentity-get
      parameters:
      - in: path
        name: bucket
        description: Name of a bucket
      - in: path
        name: entity
        description: The entity holding the permission
      responses:
        200:
          description: OK
      tags:
      - Bucket ACL
    patch:
      summary: Update Bucket Default ACL
      description: Updates a default object ACL entry on the specified bucket. This
        method supports patch semantics.
      operationId: storage.defaultObjectAccessControls.patch
      x-api-path-slug: bbucketdefaultobjectaclentity-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of a bucket
      - in: path
        name: entity
        description: The entity holding the permission
      responses:
        200:
          description: OK
      tags:
      - Bucket ACL
    put:
      summary: Update Bucket Default ACL
      description: Updates a default object ACL entry on the specified bucket.
      operationId: storage.defaultObjectAccessControls.update
      x-api-path-slug: bbucketdefaultobjectaclentity-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of a bucket
      - in: path
        name: entity
        description: The entity holding the permission
      responses:
        200:
          description: OK
      tags:
      - Bucket ACL
  /b/{bucket}/iam:
    get:
      summary: Get Bucket IAM
      description: Returns an IAM policy for the specified bucket.
      operationId: storage.buckets.getIamPolicy
      x-api-path-slug: bbucketiam-get
      parameters:
      - in: path
        name: bucket
        description: Name of a bucket
      responses:
        200:
          description: OK
      tags:
      - Bucket IAM
    put:
      summary: Update Bucket IAM
      description: Updates an IAM policy for the specified bucket.
      operationId: storage.buckets.setIamPolicy
      x-api-path-slug: bbucketiam-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of a bucket
      responses:
        200:
          description: OK
      tags:
      - Bucket IAM
  /b/{bucket}/iam/testPermissions:
    get:
      summary: Test Bucket IAM Permissions
      description: Tests a set of permissions on the given bucket to see which, if
        any, are held by the caller.
      operationId: storage.buckets.testIamPermissions
      x-api-path-slug: bbucketiamtestpermissions-get
      parameters:
      - in: path
        name: bucket
        description: Name of a bucket
      - in: query
        name: permissions
        description: Permissions to test
      responses:
        200:
          description: OK
      tags:
      - Bucket IAM
  /b/{bucket}/o:
    get:
      summary: Get Objects
      description: Retrieves a list of objects matching the criteria.
      operationId: storage.objects.list
      x-api-path-slug: bbucketo-get
      parameters:
      - in: path
        name: bucket
        description: Name of the bucket in which to look for objects
      - in: query
        name: delimiter
        description: Returns results in a directory-like mode
      - in: query
        name: maxResults
        description: Maximum number of items plus prefixes to return in a single page
          of responses
      - in: query
        name: pageToken
        description: A previously-returned page token representing part of the larger
          set of results to view
      - in: query
        name: prefix
        description: Filter results to objects whose names begin with this prefix
      - in: query
        name: projection
        description: Set of properties to return
      - in: query
        name: versions
        description: If true, lists all versions of an object as distinct results
      responses:
        200:
          description: OK
      tags:
      - Object
    post:
      summary: Add New Object
      description: Stores a new object and metadata.
      operationId: storage.objects.insert
      x-api-path-slug: bbucketo-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of the bucket in which to store the new object
      - in: query
        name: contentEncoding
        description: If set, sets the contentEncoding property of the final object
          to this value
      - in: query
        name: ifGenerationMatch
        description: Makes the operation conditional on whether the objects current
          generation matches the given value
      - in: query
        name: ifGenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          generation does not match the given value
      - in: query
        name: ifMetagenerationMatch
        description: Makes the operation conditional on whether the objects current
          metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          metageneration does not match the given value
      - in: query
        name: name
        description: Name of the object
      - in: query
        name: predefinedAcl
        description: Apply a predefined set of access controls to this object
      - in: query
        name: projection
        description: Set of properties to return
      responses:
        200:
          description: OK
      tags:
      - Object
  /b/{bucket}/o/watch:
    post:
      summary: Update Object
      description: Watch for changes on all objects in a bucket.
      operationId: storage.objects.watchAll
      x-api-path-slug: bbucketowatch-post
      parameters:
      - in: path
        name: bucket
        description: Name of the bucket in which to look for objects
      - in: query
        name: delimiter
        description: Returns results in a directory-like mode
      - in: query
        name: maxResults
        description: Maximum number of items plus prefixes to return in a single page
          of responses
      - in: query
        name: pageToken
        description: A previously-returned page token representing part of the larger
          set of results to view
      - in: query
        name: prefix
        description: Filter results to objects whose names begin with this prefix
      - in: query
        name: projection
        description: Set of properties to return
      - in: body
        name: resource
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: versions
        description: If true, lists all versions of an object as distinct results
      responses:
        200:
          description: OK
      tags:
      - Object
  /b/{bucket}/o/{object}:
    delete:
      summary: Delete Object
      description: Deletes an object and its metadata. Deletions are permanent if
        versioning is not enabled for the bucket, or if the generation parameter is
        used.
      operationId: storage.objects.delete
      x-api-path-slug: bbucketoobject-delete
      parameters:
      - in: path
        name: bucket
        description: Name of the bucket in which the object resides
      - in: query
        name: generation
        description: If present, permanently deletes a specific revision of this object
          (as opposed to the latest version, the default)
      - in: query
        name: ifGenerationMatch
        description: Makes the operation conditional on whether the objects current
          generation matches the given value
      - in: query
        name: ifGenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          generation does not match the given value
      - in: query
        name: ifMetagenerationMatch
        description: Makes the operation conditional on whether the objects current
          metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          metageneration does not match the given value
      - in: path
        name: object
        description: Name of the object
      responses:
        200:
          description: OK
      tags:
      - Object
    get:
      summary: Get Object
      description: Retrieves an object or its metadata.
      operationId: storage.objects.get
      x-api-path-slug: bbucketoobject-get
      parameters:
      - in: path
        name: bucket
        description: Name of the bucket in which the object resides
      - in: query
        name: generation
        description: If present, selects a specific revision of this object (as opposed
          to the latest version, the default)
      - in: query
        name: ifGenerationMatch
        description: Makes the operation conditional on whether the objects generation
          matches the given value
      - in: query
        name: ifGenerationNotMatch
        description: Makes the operation conditional on whether the objects generation
          does not match the given value
      - in: query
        name: ifMetagenerationMatch
        description: Makes the operation conditional on whether the objects current
          metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          metageneration does not match the given value
      - in: path
        name: object
        description: Name of the object
      - in: query
        name: projection
        description: Set of properties to return
      responses:
        200:
          description: OK
      tags:
      - Object
    patch:
      summary: Update Object
      description: Updates an object's metadata. This method supports patch semantics.
      operationId: storage.objects.patch
      x-api-path-slug: bbucketoobject-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of the bucket in which the object resides
      - in: query
        name: generation
        description: If present, selects a specific revision of this object (as opposed
          to the latest version, the default)
      - in: query
        name: ifGenerationMatch
        description: Makes the operation conditional on whether the objects current
          generation matches the given value
      - in: query
        name: ifGenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          generation does not match the given value
      - in: query
        name: ifMetagenerationMatch
        description: Makes the operation conditional on whether the objects current
          metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          metageneration does not match the given value
      - in: path
        name: object
        description: Name of the object
      - in: query
        name: predefinedAcl
        description: Apply a predefined set of access controls to this object
      - in: query
        name: projection
        description: Set of properties to return
      responses:
        200:
          description: OK
      tags:
      - Object
    put:
      summary: Update Object
      description: Updates an object's metadata.
      operationId: storage.objects.update
      x-api-path-slug: bbucketoobject-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of the bucket in which the object resides
      - in: query
        name: generation
        description: If present, selects a specific revision of this object (as opposed
          to the latest version, the default)
      - in: query
        name: ifGenerationMatch
        description: Makes the operation conditional on whether the objects current
          generation matches the given value
      - in: query
        name: ifGenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          generation does not match the given value
      - in: query
        name: ifMetagenerationMatch
        description: Makes the operation conditional on whether the objects current
          metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the operation conditional on whether the objects current
          metageneration does not match the given value
      - in: path
        name: object
        description: Name of the object
      - in: query
        name: predefinedAcl
        description: Apply a predefined set of access controls to this object
      - in: query
        name: projection
        description: Set of properties to return
      responses:
        200:
          description: OK
      tags:
      - Object
  /b/{bucket}/o/{object}/acl:
    get:
      summary: Get Object ACLs
      description: Retrieves ACL entries on the specified object.
      operationId: storage.objectAccessControls.list
      x-api-path-slug: bbucketoobjectacl-get
      parameters:
      - in: path
        name: bucket
        description: Name of a bucket
      - in: query
        name: generation
        description: If present, selects a specific revision of this object (as opposed
          to the latest version, the default)
      - in: path
        name: object
        description: Name of the object
      responses:
        200:
          description: OK
      tags:
      - Object ACL
    post:
      summary: Create Object ACL
      description: Creates a new ACL entry on the specified object.
      operationId: storage.objectAccessControls.insert
      x-api-path-slug: bbucketoobjectacl-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of a bucket
      - in: query
        name: generation
        description: If present, selects a specific revision of this object (as opposed
          to the latest version, the default)
      - in: path
        name: object
        description: Name of the object
      responses:
        200:
          description: OK
      tags:
      - Object ACL
  /b/{bucket}/o/{object}/acl/{entity}:
    delete:
      summary: Delete Object ACL
      description: Permanently deletes the ACL entry for the specified entity on the
        specified object.
      operationId: storage.objectAccessControls.delete
      x-api-path-slug: bbucketoobjectaclentity-delete
      parameters:
      - in: path
        name: bucket
        description: Name of a bucket
      - in: path
        name: entity
        description: The entity holding the permission
      - in: query
        name: generation
        description: If present, selects a specific revision of this object (as opposed
          to the latest version, the default)
      - in: path
        name: object
        description: Name of the object
      responses:
        200:
          description: OK
      tags:
      - Object ACL
    get:
      summary: Get Object ACL
      description: Returns the ACL entry for the specified entity on the specified
        object.
      operationId: storage.objectAccessControls.get
      x-api-path-slug: bbucketoobjectaclentity-get
      parameters:
      - in: path
        name: bucket
        description: Name of a bucket
      - in: path
        name: entity
        description: The entity holding the permission
      - in: query
        name: generation
        description: If present, selects a specific revision of this object (as opposed
          to the latest version, the default)
      - in: path
        name: object
        description: Name of the object
      responses:
        200:
          description: OK
      tags:
      - Object ACL
    patch:
      summary: Update Object ACL
      description: Updates an ACL entry on the specified object. This method supports
        patch semantics.
      operationId: storage.objectAccessControls.patch
      x-api-path-slug: bbucketoobjectaclentity-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of a bucket
      - in: path
        name: entity
        description: The entity holding the permission
      - in: query
        name: generation
        description: If present, selects a specific revision of this object (as opposed
          to the latest version, the default)
      - in: path
        name: object
        description: Name of the object
      responses:
        200:
          description: OK
      tags:
      - Object ACL
    put:
      summary: Update Object ACL
      description: Updates an ACL entry on the specified object.
      operationId: storage.objectAccessControls.update
      x-api-path-slug: bbucketoobjectaclentity-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of a bucket
      - in: path
        name: entity
        description: The entity holding the permission
      - in: query
        name: generation
        description: If present, selects a specific revision of this object (as opposed
          to the latest version, the default)
      - in: path
        name: object
        description: Name of the object
      responses:
        200:
          description: OK
      tags:
      - Object ACL
  /b/{bucket}/o/{object}/iam:
    get:
      summary: Get Object IAM
      description: Returns an IAM policy for the specified object.
      operationId: storage.objects.getIamPolicy
      x-api-path-slug: bbucketoobjectiam-get
      parameters:
      - in: path
        name: bucket
        description: Name of the bucket in which the object resides
      - in: query
        name: generation
        description: If present, selects a specific revision of this object (as opposed
          to the latest version, the default)
      - in: path
        name: object
        description: Name of the object
      responses:
        200:
          description: OK
      tags:
      - Object IAM
    put:
      summary: Update Object IAM
      description: Updates an IAM policy for the specified object.
      operationId: storage.objects.setIamPolicy
      x-api-path-slug: bbucketoobjectiam-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bucket
        description: Name of the bucket in which the object resides
      - in: query
        name: generation
        description: If present, selects a specific revision of this object (as opposed
          to the latest version, the default)
      - in: path
        name: object
        description: Name of the object
      responses:
        200:
          description: OK
      tags:
      - Object IAM
  /b/{bucket}/o/{object}/iam/testPermissions:
    get:
      summary: Test Object IAM Permissions
      description: Tests a set of permissions on the given object to see which, if
        any, are held by the caller.
      operationId: storage.objects.testIamPermissions
      x-api-path-slug: bbucketoobjectiamtestpermissions-get
      parameters:
      - in: path
        name: bucket
        description: Name of the bucket in which the object resides
      - in: query
        name: generation
        description: If present, selects a specific revision of this object (as opposed
          to the latest version, the default)
      - in: path
        name: object
        description: Name of the object
      - in: query
        name: permissions
        description: Permissions to test
      responses:
        200:
          description: OK
      tags:
      - Object IAM
  /b/{destinationBucket}/o/{destinationObject}/compose:
    post:
      summary: Concatenate Objects
      description: Concatenates a list of existing objects into a new object in the
        same bucket.
      operationId: storage.objects.compose
      x-api-path-slug: bdestinationbucketodestinationobjectcompose-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: destinationBucket
        description: Name of the bucket in which to store the new object
      - in: path
        name: destinationObject
        description: Name of the new object
      - in: query
        name: destinationPredefinedAcl
        description: Apply a predefined set of access controls to the destination
          object
      - in: query
        name: ifGenerationMatch
        description: Makes the operation conditional on whether the objects current
          generation matches the given value
      - in: query
        name: ifMetagenerationMatch
        description: Makes the operation conditional on whether the objects current
          metageneration matches the given value
      responses:
        200:
          description: OK
      tags:
      - Object
  /b/{sourceBucket}/o/{sourceObject}/copyTo/b/{destinationBucket}/o/{destinationObject}:
    post:
      summary: Copy Object
      description: Copies a source object to a destination object. Optionally overrides
        metadata.
      operationId: storage.objects.copy
      x-api-path-slug: bsourcebucketosourceobjectcopytobdestinationbucketodestinationobject-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: destinationBucket
        description: Name of the bucket in which to store the new object
      - in: path
        name: destinationObject
        description: Name of the new object
      - in: query
        name: destinationPredefinedAcl
        description: Apply a predefined set of access controls to the destination
          object
      - in: query
        name: ifGenerationMatch
        description: Makes the operation conditional on whether the destination objects
          current generation matches the given value
      - in: query
        name: ifGenerationNotMatch
        description: Makes the operation conditional on whether the destination objects
          current generation does not match the given value
      - in: query
        name: ifMetagenerationMatch
        description: Makes the operation conditional on whether the destination objects
          current metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the operation conditional on whether the destination objects
          current metageneration does not match the given value
      - in: query
        name: ifSourceGenerationMatch
        description: Makes the operation conditional on whether the source objects
          generation matches the given value
      - in: query
        name: ifSourceGenerationNotMatch
        description: Makes the operation conditional on whether the source objects
          generation does not match the given value
      - in: query
        name: ifSourceMetagenerationMatch
        description: Makes the operation conditional on whether the source objects
          current metageneration matches the given value
      - in: query
        name: ifSourceMetagenerationNotMatch
        description: Makes the operation conditional on whether the source objects
          current metageneration does not match the given value
      - in: query
        name: projection
        description: Set of properties to return
      - in: path
        name: sourceBucket
        description: Name of the bucket in which to find the source object
      - in: query
        name: sourceGeneration
        description: If present, selects a specific revision of the source object
          (as opposed to the latest version, the default)
      - in: path
        name: sourceObject
        description: Name of the source object
      responses:
        200:
          description: OK
      tags:
      - Object
  /b/{sourceBucket}/o/{sourceObject}/rewriteTo/b/{destinationBucket}/o/{destinationObject}:
    post:
      summary: Rewrite Object
      description: Rewrites a source object to a destination object. Optionally overrides
        metadata.
      operationId: storage.objects.rewrite
      x-api-path-slug: bsourcebucketosourceobjectrewritetobdestinationbucketodestinationobject-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: destinationBucket
        description: Name of the bucket in which to store the new object
      - in: path
        name: destinationObject
        description: Name of the new object
      - in: query
        name: destinationPredefinedAcl
        description: Apply a predefined set of access controls to the destination
          object
      - in: query
        name: ifGenerationMatch
        description: Makes the operation conditional on whether the destination objects
          current generation matches the given value
      - in: query
        name: ifGenerationNotMatch
        description: Makes the operation conditional on whether the destination objects
          current generation does not match the given value
      - in: query
        name: ifMetagenerationMatch
        description: Makes the operation conditional on whether the destination objects
          current metageneration matches the given value
      - in: query
        name: ifMetagenerationNotMatch
        description: Makes the operation conditional on whether the destination objects
          current metageneration does not match the given value
      - in: query
        name: ifSourceGenerationMatch
        description: Makes the operation conditional on whether the source objects
          generation matches the given value
      - in: query
        name: ifSourceGenerationNotMatch
        description: Makes the operation conditional on whether the source objects
          generation does not match the given value
      - in: query
        name: ifSourceMetagenerationMatch
        description: Makes the operation conditional on whether the source objects
          current metageneration matches the given value
      - in: query
        name: ifSourceMetagenerationNotMatch
        description: Makes the operation conditional on whether the source objects
          current metageneration does not match the given value
      - in: query
        name: maxBytesRewrittenPerCall
        description: The maximum number of bytes that will be rewritten per rewrite
          request
      - in: query
        name: projection
        description: Set of properties to return
      - in: query
        name: rewriteToken
        description: Include this field (from the previous rewrite response) on each
          rewrite request after the first one, until the rewrite response done flag
          is true
      - in: path
        name: sourceBucket
        description: Name of the bucket in which to find the source object
      - in: query
        name: sourceGeneration
        description: If present, selects a specific revision of the source object
          (as opposed to the latest version, the default)
      - in: path
        name: sourceObject
        description: Name of the source object
      responses:
        200:
          description: OK
      tags:
      - Object
  /channels/stop:
    post:
      summary: Stop Watching Channel
      description: Stop watching resources through this channel
      operationId: storage.channels.stop
      x-api-path-slug: channelsstop-post
      parameters:
      - in: body
        name: resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Channel
  /v1/googleServiceAccounts/{projectId}:
    get:
      summary: Get Account
      description: Returns the Google service account that is used by Storage Transfer
        Service to access buckets in the project where transfers run or in other projects.
        Each Google service account is associated with one Google Developers Console
        project. Users should add this service account to the Google Cloud Storage
        bucket ACLs to grant access to Storage Transfer Service. This service account
        is created and owned by Storage Transfer Service and can only be used by Storage
        Transfer Service.
      operationId: storagetransfer.googleServiceAccounts.get
      x-api-path-slug: v1googleserviceaccountsprojectid-get
      parameters:
      - in: path
        name: projectId
        description: The ID of the Google Developers Console project that the Google
          service account is associated with
      responses:
        200:
          description: OK
      tags:
      - Account
  /v1/transferJobs:
    get:
      summary: Get Transfer Jobs
      description: Lists transfer jobs.
      operationId: storagetransfer.transferJobs.list
      x-api-path-slug: v1transferjobs-get
      parameters:
      - in: query
        name: filter
        description: A list of query parameters specified as JSON text in the form
          of {`project_id`:my_project_id, `job_names`:[jobid1,jobid2,
      - in: query
        name: pageSize
        description: The list page size
      - in: query
        name: pageToken
        description: The list page token
      responses:
        200:
          description: OK
      tags:
      - Job
    post:
      summary: Create Transfer Jobs
      description: Creates a transfer job that runs periodically.
      operationId: storagetransfer.transferJobs.create
      x-api-path-slug: v1transferjobs-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1/{jobName}:
    get:
      summary: Get Transfer Jobs
      description: Gets a transfer job.
      operationId: storagetransfer.transferJobs.get
      x-api-path-slug: v1jobname-get
      parameters:
      - in: path
        name: jobName
        description: The job to get
      - in: query
        name: projectId
        description: The ID of the Google Developers Console project that owns the
          job
      responses:
        200:
          description: OK
      tags:
      - Job
    patch:
      summary: Update Transfer Jobs
      description: Updates a transfer job. Updating a job's transfer spec does not
        affect transfer operations that are running already. Updating the scheduling
        of a job is not allowed.
      operationId: storagetransfer.transferJobs.patch
      x-api-path-slug: v1jobname-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: jobName
        description: The name of job to update
      responses:
        200:
          description: OK
      tags:
      - Job
  /v1/{name}:
    delete:
      summary: Delete Transfer Operations
      description: This method is not supported and the server returns `UNIMPLEMENTED`.
      operationId: storagetransfer.transferOperations.delete
      x-api-path-slug: v1name-delete
      parameters:
      - in: path
        name: name
        description: The name of the operation resource to be deleted
      responses:
        200:
          description: OK
      tags:
      - Operation
    get:
      summary: Get Transfer Operations
      description: 'Lists operations that match the specified filter in the request.
        If the server doesn''t support this method, it returns `UNIMPLEMENTED`. NOTE:
        the `name` binding below allows API services to override the binding to use
        different resource name schemes, such as `users/*/operations`.'
      operationId: storagetransfer.transferOperations.list
      x-api-path-slug: v1name-get
      parameters:
      - in: query
        name: filter
        description: The standard list filter
      - in: path
        name: name
        description: The value `transferOperations`
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
      - Operation
  /v1/{name}:cancel:
    post:
      summary: Cancel Transfer Operation
      description: Cancels a transfer. Use the get method to check whether the cancellation
        succeeded or whether the operation completed despite cancellation.
      operationId: storagetransfer.transferOperations.cancel
      x-api-path-slug: v1namecancel-post
      parameters:
      - in: path
        name: name
        description: The name of the operation resource to be cancelled
      responses:
        200:
          description: OK
      tags:
      - Operation
  /v1/{name}:pause:
    post:
      summary: Pause Transfer Operation
      description: Pauses a transfer operation.
      operationId: storagetransfer.transferOperations.pause
      x-api-path-slug: v1namepause-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The name of the transfer operation
      responses:
        200:
          description: OK
      tags:
      - Operation
  /v1/{name}:resume:
    post:
      summary: Resume Transfer Operation
      description: Resumes a transfer operation that is paused.
      operationId: storagetransfer.transferOperations.resume
      x-api-path-slug: v1nameresume-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The name of the transfer operation
      responses:
        200:
          description: OK
      tags:
      - Operation
  /v1:getGoogleServiceAccount:
    get:
      summary: Get Service Account
      description: Returns the Google service account that is used by Storage Transfer
        Service to access buckets in the project where transfers run or in other projects.
        Each Google service account is associated with one Google Developers Console
        project. Users should add this service account to the Google Cloud Storage
        bucket ACLs to grant access to Storage Transfer Service. This service account
        is created and owned by Storage Transfer Service and can only be used by Storage
        Transfer Service.
      operationId: storagetransfer.getGoogleServiceAccount
      x-api-path-slug: v1getgoogleserviceaccount-get
      parameters:
      - in: query
        name: projectId
        description: The ID of the Google Developers Console project that the Google
          service account is associated with
      responses:
        200:
          description: OK
      tags:
      - Account