swagger: "2.0"
x-collection-name: AWS S3
x-complete: 1
info:
  title: No Title
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    delete:
      summary: DELETE Bucket
      description: This implementation of the DELETE operation deletes the bucket
        named inthe URI
      operationId: delete-bucket
      x-api-path-slug: delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
    head:
      summary: HEAD Bucket
      description: This operation is useful to determine if a bucket exists and you
        have permission to accessit
      operationId: head-bucket
      x-api-path-slug: head
      responses:
        200:
          description: OK
      tags:
      - Bucket
    post:
      summary: POST Object
      description: The POST operation adds an object to a specified bucket using HTML
        forms
      operationId: post-object
      x-api-path-slug: post
      responses:
        200:
          description: OK
      tags:
      - Object
    put:
      summary: PUT Bucket
      description: This implementation of the PUT operation creates a new bucket
      operationId: put-bucket
      x-api-path-slug: put
      parameters:
      - in: header
        name: x-amz-acl
        description: The canned ACL to apply to the bucket you are creating
      - in: header
        name: x-amz-grant-full-control
        description: Allows grantee the READ, WRITE, READ_ACP, and WRITE_ACP permissions
          on thettttttttttttbucket
      - in: header
        name: x-amz-grant-read
        description: Allows grantee to list the objects in the bucket
      - in: header
        name: x-amz-grant-read-acp
        description: Allows grantee to read the bucket ACL
      - in: header
        name: x-amz-grant-write
        description: Allows grantee to create, overwrite, and delete any object in
          the bucket
      - in: header
        name: x-amz-grant-write-acp
        description: Allows grantee to write the ACL for the applicable bucket
      responses:
        200:
          description: OK
      tags:
      - Bucket
  /?accelerate:
    get:
      summary: GET Bucket accelerate
      description: This implementation of the GET operation uses the acceleratesubresource
        to return the Transfer Acceleration state of a bucket, which is eitherEnabled
        or Suspended
      operationId: get-bucket-accelerate
      x-api-path-slug: accelerate-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Accelerate
    put:
      summary: PUT Bucket accelerate
      description: This implementation of the PUT operation uses the acceleratesubresource
        to set the Transfer Acceleration state of an existing bucket
      operationId: put-bucket-accelerate
      x-api-path-slug: accelerate-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Accelerate
  /?acl:
    get:
      summary: GET Bucket ACL
      description: This implementation of the GET operation uses the aclsubresource
        to return the access control list (ACL) of a bucket
      operationId: get-bucket-acl
      x-api-path-slug: acl-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - ACL
    put:
      summary: PUT Bucket ACL
      description: This implementation of the PUT operation uses the aclsubresource
        to set the permissions on an existing bucket using access control lists(ACL)
      operationId: put-bucket-acl
      x-api-path-slug: acl-put
      parameters:
      - in: header
        name: x-amz-acl
        description: Sets the ACL of the bucket using the specified canned ACL
      - in: header
        name: x-amz-grant-full-control
        description: Allows the specified grantee(s) the READ, WRITE, READ_ACP, and
          WRITE_ACPtttttttttpermissions on the bucket
      - in: header
        name: x-amz-grant-read
        description: Allows the specified grantee(s) to list the objects in the bucket
      - in: header
        name: x-amz-grant-read-acp
        description: Allows the specified grantee(s) to read the bucket ACL
      - in: header
        name: x-amz-grant-write
        description: Allows the specified grantee(s) to create, overwrite, and delete
          any object in thetttttttttbucket
      - in: header
        name: x-amz-grant-write-acp
        description: Allows the specified grantee(s) to write the ACL for the applicabletttttttttbucket
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - ACL
  /?analytics:
    get:
      summary: List Bucket Analytics Configurations
      description: This implementation of the GET operation returns a list of analyticsconfigurations
        for the bucket
      operationId: list-bucket-analytics-configurations
      x-api-path-slug: analytics-get
      parameters:
      - in: query
        name: ContinuationToken
        description: The marker that is used to continue an analytics configuration
          listing that has beenttttttttttruncated
      responses:
        200:
          description: OK
      tags:
      - List
      - Bucket
      - Analytics
      - Configurations
  /?analytics&amp;id=analytics-configuration-ID:
    delete:
      summary: DELETE Bucket analyticsnttconfiguration
      description: This implementation of the DELETE operation deletes an analytics
        configuration(identified by the analytics configuration ID) from the bucket
      operationId: delete-bucket-analyticsconfiguration
      x-api-path-slug: analyticsampidanalyticsconfigurationid-delete
      parameters:
      - in: query
        name: id
        description: The ID that identifies the analytics configuration
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Analyticsnttconfiguration
    get:
      summary: GET Bucket analytics configuration
      description: This implementation of the GET operation returns an analytics configuration
        (identified bythe analytics configuration ID) from the bucket
      operationId: get-bucket-analytics-configuration
      x-api-path-slug: analyticsampidanalyticsconfigurationid-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Analytics
      - Configuration
  /?analytics&amp;id=configuration-ID:
    put:
      summary: PUT Bucket analytics configuration
      description: This implementation of the PUT operation adds an analytics configuration(identified
        by the analytics ID) to the bucket
      operationId: put-bucket-analytics-configuration
      x-api-path-slug: analyticsampidconfigurationid-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Analytics
      - Configuration
  /?cors:
    delete:
      summary: DELETE Bucket CORS
      description: Deletes the cors configuration information set for the bucket
      operationId: delete-bucket-cors
      x-api-path-slug: cors-delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - CORS
    get:
      summary: GET Bucket CORS
      description: Returns the cors configuration information set for thebucket
      operationId: get-bucket-cors
      x-api-path-slug: cors-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - CORS
  /?delete:
    post:
      summary: Delete Multiple Objects
      description: The Multi-Object Delete operation enables you to delete multiple
        objects from a bucketusing a single HTTP request
      operationId: delete-multiple-objects
      x-api-path-slug: delete-post
      parameters:
      - in: header
        name: Content-Length
        description: Length of the body according to RFC 2616
      - in: header
        name: Content-MD5
        description: The base64-encoded 128-bit MD5 digest of the data
      - in: header
        name: x-amz-mfa
        description: The value is the concatenation of the authentication devices
          serial number, a space,tttttttttand the value that is displayed on your
          authenticationtttttttttdevice
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Objects
  /?inventory:
    get:
      summary: List Bucket Inventory Configurations
      description: This implementation of the GET operation returns a list of inventoryconfigurations
        for the bucket
      operationId: list-bucket-inventory-configurations
      x-api-path-slug: inventory-get
      parameters:
      - in: query
        name: ContinuationToken
        description: The marker that is used to continue an inventory configuration
          listing that has beenttttttttttruncated
      responses:
        200:
          description: OK
      tags:
      - List
      - Bucket
      - Inventory
      - Configurations
  /?inventory&amp;id=configuration-ID:
    put:
      summary: PUT Bucket inventory configuration
      description: This implementation of the PUT operation adds an inventory configuration(identified
        by the inventory ID) to the bucket
      operationId: put-bucket-inventory-configuration
      x-api-path-slug: inventoryampidconfigurationid-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Inventory
      - Configuration
  /?inventory&amp;id=inventory-configuration-ID:
    delete:
      summary: DELETE Bucket inventory configuration
      description: This implementation of the DELETE operation deletes an inventory
        configuration(identified by the inventory configuration ID) from the bucket
      operationId: delete-bucket-inventoryconfiguration
      x-api-path-slug: inventoryampidinventoryconfigurationid-delete
      parameters:
      - in: query
        name: id
        description: The ID that identifies the inventory configuration
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Inventory
      - Configuration
    get:
      summary: GET Bucket inventory configuration
      description: This implementation of the GET operation returns an inventory configuration
        (identified bythe inventory configuration ID) from the bucket
      operationId: get-bucket-inventory-configuration
      x-api-path-slug: inventoryampidinventoryconfigurationid-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Inventory
      - Configuration
  /?lifecycle:
    delete:
      summary: DELETE Bucket lifecycle
      description: Deletes the lifecycle configuration from the specified bucket
      operationId: delete-bucket-lifecycle
      x-api-path-slug: lifecycle-delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Lifecycle
    get:
      summary: GET Bucket lifecycle
      description: NoteBucket lifecycle configuration now supports specifying lifecycle
        rule usingobject key name prefix, one or more object tags, or combination
        of both
      operationId: get-bucket-lifecycle
      x-api-path-slug: lifecycle-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Lifecycle
    put:
      summary: PUT Bucket lifecycle
      description: Creates a new lifecycle configuration for the bucket or replaces
        an existing lifecycle configuration
      operationId: put-bucket-lifecycle
      x-api-path-slug: lifecycle-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Lifecycle
  /?list-type=2:
    get:
      summary: GET Bucket (List Objects) Version 2
      description: This implementation of the GET operation returns some or all (up
        to 1,000) ofthe objects in a bucket
      operationId: get-bucket-list-objects-version-2
      x-api-path-slug: listtype2-get
      parameters:
      - in: query
        name: continuation-token
        description: When the Amazon S3 response to this API call is truncated (that
          is, IsTruncated responsetttttttttelement value is true), the response also
          includes thettttttttttNextContinuationToken element, the value of whichtttttttttyou
          can use in the next request as thettttttttttcontinuation-token to list the
          next settttttttttof objects
      - in: query
        name: delimiter
        description: A delimiter is a character you use to group keys
      - in: query
        name: encoding-type
        description: Requests Amazon S3 to encode the response and specifies the encoding
          method totttttttttuse
      - in: query
        name: fetch-owner
        description: By default, the API does not return the Owner information in
          the response
      - in: query
        name: list-type
        description: Version 2 of the API requires this parameter and you must set
          its value to 2
      - in: query
        name: max-keys
        description: Sets the maximum number of keys returned in the response body
      - in: query
        name: prefix
        description: Limits the response to keys that begin with the specifiedtttttttttprefix
      - in: query
        name: start-after
        description: If you want the API to return key names after a specifictttttttttobject
          key in your key space, you can add this parameter
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - (List
      - Objects)
      - Version
      - "2"
  /?location:
    get:
      summary: GET Bucket location
      description: This implementation of the GET operation uses thelocation subresource
        to return a bucket's region
      operationId: get-bucket-location
      x-api-path-slug: location-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Location
  /?logging:
    get:
      summary: GET Bucket logging
      description: This implementation of the GET operation uses thelogging subresource
        to return the logging status of a bucketand the permissions users have to
        view and modify that status
      operationId: get-bucket-logging
      x-api-path-slug: logging-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Logging
  /?metrics:
    get:
      summary: List Bucket Metrics
      description: Lists the metrics configurations for the CloudWatch request metrics
        of the bucket
      operationId: list-bucket-metrics
      x-api-path-slug: metrics-get
      parameters:
      - in: query
        name: BucketName
        description: The name of the bucket containing the metrics configurationstttttttttto
          retrieve
      - in: query
        name: ContinuationToken
        description: The marker that is used to continue a metrics configurationtttttttttlisting
          that has been truncated
      responses:
        200:
          description: OK
      tags:
      - List
      - Bucket
      - Metrics
  /?metrics&amp;id=Id:
    delete:
      summary: DELETE Bucket Metrics
      description: Deletes a metrics configuration for the CloudWatch request metrics
        (specified by the metricsconfiguration ID) from the bucket
      operationId: delete-bucket-metrics
      x-api-path-slug: metricsampidid-delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Metrics
    put:
      summary: PUT Bucket Metrics
      description: Sets or updates a metrics configuration for the CloudWatch request
        metrics (specified by themetrics configuration ID) from the bucket
      operationId: put-bucket-metrics
      x-api-path-slug: metricsampidid-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Metrics
  /?metrics&amp;id=id:
    get:
      summary: GET Bucket Metrics
      description: Gets a metrics configuration for the CloudWatch request metrics
        (specified by the metricsconfiguration ID) from the bucket
      operationId: get-bucket-metrics
      x-api-path-slug: metricsampidid-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Metrics
  /?notification:
    get:
      summary: GET Bucket notification
      description: This implementation of the GET operation uses thenotification subresource
        to return the notificationconfiguration of a bucket
      operationId: get-bucket-notification
      x-api-path-slug: notification-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Notification
    put:
      summary: PUT Bucket notification
      description: The Amazon S3 notification feature enables you to receive notifications
        when certain eventshappen in your bucket
      operationId: put-bucket-notification
      x-api-path-slug: notification-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Notification
  /?policy:
    delete:
      summary: DELETE Bucket policy
      description: This implementation of the DELETE operation uses the policy subresource
        to delete the policy on a specified bucket
      operationId: delete-bucket-policy
      x-api-path-slug: policy-delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Policy
    get:
      summary: GET Bucket policy
      description: This implementation of the GET operation uses the policysubresource
        to return the policy of a specified bucket
      operationId: get-bucket-policy
      x-api-path-slug: policy-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Policy
    put:
      summary: PUT Bucket policy
      description: This implementation of the PUT operation uses the policysubresource
        to add to or replace a policy on a bucket
      operationId: put-bucket-policy
      x-api-path-slug: policy-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Policy
  /?replication:
    delete:
      summary: DELETE Bucket replication
      description: Deletes the replication subresource associated with the specified
        bucket
      operationId: delete-bucket-replication
      x-api-path-slug: replication-delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Replication
    get:
      summary: GET Bucket replication
      description: Returns the replication configuration information set on the      bucket
      operationId: get-bucket-replication
      x-api-path-slug: replication-get
      parameters:
      - in: query
        name: AWS Documentation &raquo; Amazon Simple Storage Service (S3) &raquo;
          API Reference &raquo; Operations on Buckets &raquo; GET Bucket replication
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Replication
    put:
      summary: PUT Bucket replication
      description: In a versioning-enabled bucket, this operation creates a new replication
        configuration (or      replaces an existing one, if present)
      operationId: put-bucket-replication
      x-api-path-slug: replication-put
      parameters:
      - in: query
        name: AWS Documentation &raquo; Amazon Simple Storage Service (S3) &raquo;
          API Reference &raquo; Operations on Buckets &raquo; PUT Bucket replication
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Replication
  /?tagging:
    delete:
      summary: DELETE Bucket tagging
      description: This implementation of the DELETE operation uses the taggingsubresource
        to remove a tag set from the specified bucket
      operationId: delete-bucket-tagging
      x-api-path-slug: tagging-delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Tagging
    get:
      summary: GET Bucket tagging
      description: This implementation of the GET operation uses the taggingsubresource
        to return the tag set associated with the bucket
      operationId: get-bucket-tagging
      x-api-path-slug: tagging-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Tagging
    put:
      summary: PUT Bucket tagging
      description: This implementation of the PUT operation uses the taggingsubresource
        to add a set of tags to an existing bucket
      operationId: put-bucket-tagging
      x-api-path-slug: tagging-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Tagging
  /?uploads:
    get:
      summary: List Multipart Uploads
      description: This operation lists in-progress multipart uploads
      operationId: list-multipart-uploads
      x-api-path-slug: uploads-get
      parameters:
      - in: query
        name: delimiter
        description: Character you use to group keys
      - in: query
        name: encoding-type
        description: Requests Amazon S3 to encode the response and specifies the encoding
          method totttttttttuse
      - in: query
        name: key-marker
        description: Together with upload-id-marker, this parameter specifies the
          multiparttttttttttupload after which listing should begin
      - in: query
        name: max-uploads
        description: Sets the maximum number of multipart uploads, from 1 to 1,000,
          to return in thetttttttttresponse body
      - in: query
        name: prefix
        description: Lists in-progress uploads only for those keys that begin with
          the specified prefix
      - in: query
        name: upload-id-&#8203;marker
        description: Together with key-marker, specifies the multipart upload after
          whichtttttttttlisting should begin
      responses:
        200:
          description: OK
      tags:
      - List
      - Multipart
      - Uploads
  /?versioning:
    get:
      summary: GET Bucket versioning
      description: This implementation of the GET operation uses theversioning subresource
        to return the versioning state of abucket
      operationId: get-bucket-versioning
      x-api-path-slug: versioning-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Versioning
    put:
      summary: PUT Bucket versioning
      description: This implementation of the PUT operation uses theversioning subresource
        to set the versioning state of anexisting bucket
      operationId: put-bucket-versioning
      x-api-path-slug: versioning-put
      parameters:
      - in: header
        name: x-amz-mfa
        description: The value is the concatenation of the authenticationtttttttttdevices
          serial number, a space, and the value displayed on yourtttttttttauthentication
          device
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Versioning
  /?versions:
    get:
      summary: GET Bucket Object versions
      description: You can use the versions subresource to list metadata about all
        ofthe versions of objects in a bucket
      operationId: get-bucket-object-versions
      x-api-path-slug: versions-get
      parameters:
      - in: query
        name: delimiter
        description: A delimiter is a character that you specify to group keys
      - in: query
        name: encoding-type
        description: Requests Amazon S3 to encode the response and specifies the encoding
          method totttttttttuse
      - in: query
        name: key-marker
        description: Specifies the key in the bucket that you want to start listingtttttttttfrom
      - in: query
        name: max-keys
        description: Sets the maximum number of keys returned in the response body
      - in: query
        name: prefix
        description: Use this parameter to select only those keys that begin withtttttttttthe
          specified prefix
      - in: query
        name: version-id-marker
        description: Specifies the object version you want to start listing from
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Object
      - Versions
  /?website:
    delete:
      summary: DELETE Bucket website
      description: This operation removes the website configuration for a bucket
      operationId: delete-bucket-website
      x-api-path-slug: website-delete
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Website
    get:
      summary: GET Bucket website
      description: This implementation of the GET operation returns the website configurationassociated
        with a bucket
      operationId: get-bucket-website
      x-api-path-slug: website-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Website
    put:
      summary: PUT Bucket website
      description: Sets the configuration of the website that is specified in thewebsite
        subresource
      operationId: put-bucket-website
      x-api-path-slug: website-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - Website
  /destinationObject:
    put:
      summary: PUT Object - Copy
      description: This implementation of the PUT operation creates a copy of an object
        that is      already stored in Amazon S3
      operationId: put-object--copy
      x-api-path-slug: destinationobject-put
      responses:
        200:
          description: OK
      tags:
      - Object
      - '-'
      - Copy
  /ObjectName:
    delete:
      summary: DELETE Object
      description: The DELETE operation removes the null version (if there is one)
        of anobject and inserts a delete marker, which becomes the current version
        of the object
      operationId: delete-object
      x-api-path-slug: objectname-delete
      parameters:
      - in: header
        name: x-amz-mfa
        description: The value is the concatenation of the authenticationtttttttttdevices
          serial number, a space, and the value displayed on yourtttttttttauthentication
          device
      responses:
        200:
          description: OK
      tags:
      - Object
    get:
      summary: GET Object
      description: This implementation of the GET operation retrieves objects from
        Amazon S3
      operationId: get-object
      x-api-path-slug: objectname-get
      parameters:
      - in: query
        name: response-cache-control
        description: Sets the Cache-Control header of the response
      - in: query
        name: response-content-disposition
        description: Sets the Content-Disposition header of thetttttttttresponse
      - in: query
        name: response-content-encoding
        description: Sets the Content-Encoding header of the response
      - in: query
        name: response-content-language
        description: Sets the Content-Language header of thetttttttttresponse
      - in: query
        name: response-content-type
        description: Sets the Content-Type header of thetttttttttresponse
      - in: query
        name: response-expires
        description: Sets the Expires header of the response
      responses:
        200:
          description: OK
      tags:
      - Object
    head:
      summary: HEAD Object
      description: The HEAD operation retrieves metadata from an object without returning
        theobject itself
      operationId: head-object
      x-api-path-slug: objectname-head
      parameters:
      - in: header
        name: If-Match
        description: Return the object only if its entity tag (ETag) is the same as
          the one specified; otherwise, return a 412 (precondition failed)
      - in: header
        name: If-Modified-Since
        description: Return the object only if it has been modified since the specified
          time, otherwise return a 304 (not modified)
      - in: header
        name: If-None-Match
        description: Return the object only if its entity tag (ETag) is different
          from the one specified; otherwise, return a 304 (not modified)
      - in: header
        name: If-Unmodified-Since
        description: Return the object only if it has not been modified since the
          specified time, otherwise return a 412 (precondition failed)
      - in: header
        name: Range
        description: Downloads the specified range bytes of an object
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-algorithm
        description: Specifies the algorithm to use to when decrypting the requested
          object
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-key
        description: Specifies the customer-provided base64-encoded encryption key
          to use to decrypt the requested object
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-key-MD5
        description: Specifies the base64-encoded 128-bit MD5 digest of the customer-provided
          encryption key according to ttttRFC 1321
      responses:
        200:
          description: OK
      tags:
      - Object
    options:
      summary: OPTIONS object
      description: A browser can send this preflight request to Amazon S3 to determine
        if it can send an actualrequest with the specific origin, HTTP method, and
        headers
      operationId: options-object
      x-api-path-slug: objectname-options
      responses:
        200:
          description: OK
      tags:
      - OPTIONS
      - Object
    put:
      summary: PUT Object
      description: This implementation of the PUT operation adds an object to a bucket
      operationId: put-object
      x-api-path-slug: objectname-put
      responses:
        200:
          description: OK
      tags:
      - Object
  /ObjectName?acl:
    get:
      summary: GET Object ACL
      description: This implementation of the GET operation uses the aclsubresource
        to return the access control list (ACL) of an object
      operationId: get-object-acl
      x-api-path-slug: objectnameacl-get
      responses:
        200:
          description: OK
      tags:
      - Object
      - ACL
    put:
      summary: PUT Object ACL
      description: This implementation of the PUT operation uses the aclsubresource
        to set the access control list (ACL) permissions for an object that alreadyexists
        in a bucket
      operationId: put-object-acl
      x-api-path-slug: objectnameacl-put
      parameters:
      - in: header
        name: x-amz-acl
        description: Sets the ACL of the object using the specified canned ACL
      - in: header
        name: x-amz-grant-full-control
        description: Allows the specified grantee the READ, WRITE, READ_ACP, andtttttttttWRITE_ACP
          permissions on the bucket
      - in: header
        name: x-amz-grant-read
        description: Allows the specified grantee to list the objects in thetttttttttbucket
      - in: header
        name: x-amz-grant-read-acp
        description: Allows the specified grantee to read the buckettttttttttACL
      - in: header
        name: x-amz-grant-write
        description: Not applicable when granting access permissions on objects
      - in: header
        name: x-amz-grant-write-acp
        description: Allows the specified grantee to write the ACL for thetttttttttapplicable
          bucket
      responses:
        200:
          description: OK
      tags:
      - Object
      - ACL
  /ObjectName?partNumber=PartNumber&amp;uploadId=UploadId:
    put:
      summary: Upload Part
      description: This operation uploads a part in a multipart upload
      operationId: upload-part
      x-api-path-slug: objectnamepartnumberpartnumberampuploadiduploadid-put
      parameters:
      - in: query
        name: AWS Documentation &raquo; Amazon Simple Storage Service (S3) &raquo;
          API Reference &raquo; Operations on Objects &raquo; Upload Part - Copy
      - in: header
        name: Content-Length
        description: The size of the part, in bytes
      - in: header
        name: Content-MD5
        description: The base64-encoded 128-bit MD5 digest of the part data
      - in: header
        name: Expect
        description: When your application uses 100-continue, it does not send the
          request body until ittttttttttreceives an acknowledgment
      - in: header
        name: x-amz-copy-source
        description: The name of the source bucket and the source object key name
          separated by a                  slash (/)
      - in: header
        name: x-amz-copy-source&#8203;-server-side&#8203;-encryption&#8203;-customer-algorithm
        description: Specifies algorithm to use when decrypting the source object
      - in: header
        name: x-amz-copy-source&#8203;-server-side&#8203;-encryption&#8203;-customer-key
        description: Specifies the customer provided base-64 encoded encryption key
          for Amazon                      S3 to use to decrypt the source object
      - in: header
        name: x-amz-copy-source-&#8203;server-side&#8203;-encryption&#8203;-customer-key-MD5
        description: Specifies the base64-encoded 128-bit MD5 digest of the encryption
          key                      according to RFC 1321
      - in: header
        name: x-amz-copy-source-if-match
        description: Perform a copy if the source object entity tag (ETag) matches
          the specified                  value
      - in: header
        name: x-amz-copy-source-if-modified-since
        description: Perform a copy if the source object is modified after the time
          specified                  using this header
      - in: header
        name: x-amz-copy-source-if-none-match
        description: Perform a copy if the source object entity tag (ETag) is different
          than the                  value specified using this header
      - in: header
        name: x-amz-copy-source-if-unmodified-since
        description: Perform a copy if the source object is not modified after the
          time                  specified using this header
      - in: header
        name: x-amz-copy-source-range
        description: The range of bytes to copy from the source object
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-algorithm
        description: Specifies the algorithm to use to when encrypting the object
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-key
        description: Specifies the customer-provided base64-encoded encryption key
          for Amazon S3 to use intttttttttttttencrypting data
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-key-MD5
        description: Specifies the base64-encoded 128-bit MD5 digest of the encryption
          key according to RFC 1321
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Part
  /ObjectName?restore&amp;versionId=VersionID:
    post:
      summary: POST Object restore
      description: Restores a temporary copy of an archived object
      operationId: post-object-restore
      x-api-path-slug: objectnamerestoreampversionidversionid-post
      parameters:
      - in: header
        name: Content-MD5
        description: The base64-encoded 128-bit MD5 digest of the data
      responses:
        200:
          description: OK
      tags:
      - Object
      - Restore
  /ObjectName?tagging:
    get:
      summary: GET Object tagging
      description: This implementation of the GET operation returns the tags associated
        with anobject
      operationId: get-object-tagging
      x-api-path-slug: objectnametagging-get
      responses:
        200:
          description: OK
      tags:
      - Object
      - Tagging
    put:
      summary: PUT Object tagging
      description: This implementation of the PUT operation uses the taggingsubresource
        to add a set of tags to an existing object
      operationId: put-object-tagging
      x-api-path-slug: objectnametagging-put
      responses:
        200:
          description: OK
      tags:
      - Object
      - Tagging
  /ObjectName?torrent:
    get:
      summary: GET Object torrent
      description: This implementation of the GET operation uses thetorrent subresource
        to return torrent files from a bucket
      operationId: get-object-torrent
      x-api-path-slug: objectnametorrent-get
      responses:
        200:
          description: OK
      tags:
      - Object
      - Torrent
  /ObjectName?uploadId=UploadId:
    delete:
      summary: Abort Multipart Upload
      description: This operation aborts a multipart upload
      operationId: abort-multipart-upload
      x-api-path-slug: objectnameuploadiduploadid-delete
      responses:
        200:
          description: OK
      tags:
      - Abort
      - Multipart
      - Upload
    get:
      summary: List Parts
      description: This operation lists the parts that have been uploaded for a specific
        multipart upload
      operationId: list-parts
      x-api-path-slug: objectnameuploadiduploadid-get
      parameters:
      - in: query
        name: encoding-type
        description: Requests Amazon S3 to encode the response and specifies the encoding
          method totttttttttuse
      - in: query
        name: max-parts
        description: Sets the maximum number of parts to return in the response body
      - in: query
        name: part-number&#8203;-marker
        description: Specifies the part after which listing should begin
      - in: query
        name: uploadId
        description: Upload ID identifying the multipart upload whose parts are being
          listed
      responses:
        200:
          description: OK
      tags:
      - List
      - Parts
    post:
      summary: Complete Multipart Upload
      description: This operation completes a multipart upload by assembling previously
        uploaded parts
      operationId: complete-multipart-upload
      x-api-path-slug: objectnameuploadiduploadid-post
      responses:
        200:
          description: OK
      tags:
      - Complete
      - Multipart
      - Upload
  /ObjectName?uploads:
    post:
      summary: Initiate Multipart Upload
      description: This operation initiates a multipart upload and returns an upload
        ID
      operationId: initiate-multipart-upload
      x-api-path-slug: objectnameuploads-post
      parameters:
      - in: header
        name: Cache-Control
        description: Can be used to specify caching behavior along the request/reply
          chain
      - in: header
        name: Content-&#8203;Disposition
        description: Specifies presentational information for the object
      - in: header
        name: Content-Encoding
        description: Specifies what content encodings have been applied to the object
          and thus                  what decoding mechanisms must be applied to obtain
          the media-type referenced by                  the Content-Type header field
      - in: header
        name: Content-Type
        description: A standard MIME type describing the format of the object data
      - in: header
        name: Expires
        description: The date and time at which the object is no longer cacheable
      - in: header
        name: x-amz-acl
        description: The canned ACL to apply to the object
      - in: header
        name: x-amz-grant-full-control
        description: Allows grantee the READ, READ_ACP, and WRITE_ACP permissions
          on the                        object
      - in: header
        name: x-amz-grant-read
        description: Allows grantee to read the object data and its metadata
      - in: header
        name: x-amz-grant-read-acp
        description: Allows grantee to read the object ACL
      - in: header
        name: x-amz-grant-write
        description: Not applicable
      - in: header
        name: x-amz-grant-write-acp
        description: Allows grantee to write the ACL for the applicable object
      - in: header
        name: x-amz-meta-
        description: Headers starting with this prefix are user-defined metadata
      - in: header
        name: x-amz-server-side&#8203;-encryption
        description: Specifies a server-side encryption algorithm to use when Amazon
          S3 creates                        an object
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-algorithm
        description: Specifies the algorithm to use to when encrypting the                          object
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-key
        description: Specifies the customer-provided base64-encoded encryption key
          for                          Amazon S3 to use in encrypting data
      - in: header
        name: x-amz-server-side&#8203;-encryption&#8203;-customer-key-MD5
        description: Specifies the base64-encoded 128-bit MD5 digest of the encryption                          key
          according to RFC                            1321
      - in: header
        name: x-amz-server-side-encryption-aws-kms-key-id
        description: If the x-amz-server-side-encryption is present and has                        the
          value of aws:kms, this header specifies the ID of the AWS                        Key
          Management Service (KMS) master encryption key that was used for the                        object
      - in: header
        name: x-amz-server-side-encryption-context
        description: If x-amz-server-side-encryption is present, and if its                        value
          is aws:kms, this header specifies the encryption context                        for
          the object
      - in: header
        name: x-amz-storage-&#8203;class
        description: The type of storage to use for the object that is created after
          successful                  multipart upload
      - in: header
        name: x-amz-website&#8203;-redirect-location
        description: If the bucket is configured as a website, redirect requests for
          this object                  to another object in the same bucket or to
          an external URL
      responses:
        200:
          description: OK
      tags:
      - Initiate
      - Multipart
      - Upload
  ?requestPayment:
    get:
      summary: GET Bucket requestPayment
      description: This implementation of the GET operation uses therequestPayment
        subresource to return the request paymentconfiguration of a bucket
      operationId: get-bucket-requestpayment
      x-api-path-slug: requestpayment-get
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - RequestPayment
    put:
      summary: PUT Bucket requestPayment
      description: This implementation of the PUT operation uses therequestPayment
        subresource to set the request paymentconfiguration of a bucket
      operationId: put-bucket-requestpayment
      x-api-path-slug: requestpayment-put
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - RequestPayment
  ObjectKey/?tagging:
    delete:
      summary: DELETE Object tagging
      description: This implementation of the DELETE operation uses thetagging subresource
        to remove the entire tag set from thespecified object
      operationId: delete-object-tagging
      x-api-path-slug: objectkeytagging-delete
      responses:
        200:
          description: OK
      tags:
      - Object
      - Tagging