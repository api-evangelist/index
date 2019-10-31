swagger: "2.0"
x-collection-name: AWS CloudFront
x-complete: 1
info:
  title: AWS CloudFront API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateCloudFrontOriginAccessIdentity:
    get:
      summary: Create Cloud Front Origin Access Identity
      description: Creates a new origin access identity.
      operationId: createCloudFrontOriginAccessIdentity
      x-api-path-slug: actioncreatecloudfrontoriginaccessidentity-get
      parameters:
      - in: query
        name: CloudFrontOriginAccessIdentityConfig
        description: The current configuration information for the identity
        type: string
      - in: query
        name: CreateCloudFrontOriginAccessIdentityRequest
        description: Root level tag for the CreateCloudFrontOriginAccessIdentityRequest
          parameters
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: VpcId.N
        description: One or more VPCs for which you want to describe the ClassicLink
          status
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cloud
      - Front
      - Origin
      - Access
      - Identity
  /?Action=CreateDistribution:
    get:
      summary: Create Distribution
      description: Creates a new web distribution.
      operationId: createDistribution
      x-api-path-slug: actioncreatedistribution-get
      parameters:
      - in: query
        name: CreateDistributionRequest
        description: Root level tag for the CreateDistributionRequest parameters
        type: string
      - in: query
        name: DistributionConfig
        description: The distributions configuration information
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this request
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: VpcIds.N
        description: One or more VPC IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Distribution
  /?Action=CreateDistributionWithTags:
    get:
      summary: Create Distribution With Tags
      description: Create a new distribution with tags.
      operationId: createDistributionWithTags
      x-api-path-slug: actioncreatedistributionwithtags-get
      parameters:
      - in: query
        name: CreateDistributionWithTagsRequest
        description: Root level tag for the CreateDistributionWithTagsRequest parameters
        type: string
      - in: query
        name: DistributionConfigWithTags
        description: The distributions configuration information
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance to unlink from the VPC
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC to which the instance is linked
        type: string
      responses:
        200:
          description: OK
      tags:
      - Distribution
      - Tags
  /?Action=CreateInvalidation:
    get:
      summary: Create Invalidation
      description: Create a new invalidation.
      operationId: createInvalidation
      x-api-path-slug: actioncreateinvalidation-get
      parameters:
      - in: query
        name: DistributionId
        description: The distributions id
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - Invalidation
  /?Action=CreateStreamingDistribution:
    get:
      summary: Create Streaming Distribution
      description: Creates a new RMTP distribution.
      operationId: createStreamingDistribution
      x-api-path-slug: actioncreatestreamingdistribution-get
      parameters:
      - in: query
        name: CreateStreamingDistributionRequest
        description: Root level tag for the CreateStreamingDistributionRequest parameters
        type: string
      - in: query
        name: StreamingDistributionConfig
        description: The streaming distributions configuration information
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - Streaming
      - Distribution
  /?Action=CreateStreamingDistributionWithTags:
    get:
      summary: Create Streaming Distribution With Tags
      description: Create a new streaming distribution with tags.
      operationId: createStreamingDistributionWithTags
      x-api-path-slug: actioncreatestreamingdistributionwithtags-get
      parameters:
      - in: query
        name: CreateStreamingDistributionWithTagsRequest
        description: Root level tag for the CreateStreamingDistributionWithTagsRequest
          parameters
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: StreamingDistributionConfigWithTags
        description: The streaming distributions configuration information
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - Streaming
      - Distribution
      - Tags
  /?Action=DeleteCloudFrontOriginAccessIdentity:
    get:
      summary: Delete Cloud Front Origin Access Identity
      description: Delete an origin access identity.
      operationId: deleteCloudFrontOriginAccessIdentity
      x-api-path-slug: actiondeletecloudfrontoriginaccessidentity-get
      parameters:
      - in: query
        name: Id
        description: The origin access identitys ID
        type: string
      - in: query
        name: If-Match
        description: The value of the ETag header you received from a previous GET      or
          PUT request
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cloud
      - Front
      - Origin
      - Access
      - Identity
  /?Action=DeleteDistribution:
    get:
      summary: Delete Distribution
      description: Delete a distribution.
      operationId: deleteDistribution
      x-api-path-slug: actiondeletedistribution-get
      parameters:
      - in: query
        name: BgpAsn
        description: For devices that support BGP, the customer gateways BGP ASN
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,             and provides an error response
        type: string
      - in: query
        name: Id
        description: The distribution ID
        type: string
      - in: query
        name: If-Match
        description: The value of the ETag header that you received when you disabled
          the      distribution
        type: string
      - in: query
        name: IpAddress
        description: The Internet-routable IP address for the customer gateways outside
          interface
        type: string
      - in: query
        name: Type
        description: The type of VPN connection that this customer gateway supports
          (ipsec
        type: string
      responses:
        200:
          description: OK
      tags:
      - Distribution
  /?Action=DeleteStreamingDistribution:
    get:
      summary: Delete Streaming Distribution
      description: Delete a streaming distribution.
      operationId: deleteStreamingDistribution
      x-api-path-slug: actiondeletestreamingdistribution-get
      parameters:
      - in: query
        name: CustomerGatewayId
        description: The ID of the customer gateway
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,             and provides an error response
        type: string
      - in: query
        name: Id
        description: The distribution ID
        type: string
      - in: query
        name: If-Match
        description: The value of the ETag header that you received when you disabled
          the      streaming distribution
        type: string
      responses:
        200:
          description: OK
      tags:
      - Streaming
      - Distribution
  /?Action=GetCloudFrontOriginAccessIdentity:
    get:
      summary: Get Cloud Front Origin Access Identity
      description: Get the information about an origin access identity.
      operationId: getCloudFrontOriginAccessIdentity
      x-api-path-slug: actiongetcloudfrontoriginaccessidentity-get
      parameters:
      - in: query
        name: CustomerGatewayId.N
        description: One or more customer gateway IDs
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,             and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: Id
        description: The identitys ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cloud
      - Front
      - Origin
      - Access
      - Identity
  /?Action=GetCloudFrontOriginAccessIdentityConfig:
    get:
      summary: Get Cloud Front Origin Access Identity Config
      description: Get the configuration information about an origin access identity.
      operationId: getCloudFrontOriginAccessIdentityConfig
      x-api-path-slug: actiongetcloudfrontoriginaccessidentityconfig-get
      parameters:
      - in: query
        name: AutoPlacement
        description: This is enabled by default
        type: string
      - in: query
        name: AvailabilityZone
        description: The Availability Zone for the Dedicated Hosts
        type: string
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure idempotency
          of the request
        type: string
      - in: query
        name: Id
        description: The identitys ID
        type: string
      - in: query
        name: InstanceType
        description: Specify the instance type that you want your Dedicated Hosts
          to be configured for
        type: string
      - in: query
        name: Quantity
        description: The number of Dedicated Hosts you want to allocate to your account
          with these            parameters
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cloud
      - Front
      - Origin
      - Access
      - Identity
      - Config
  /?Action=GetDistribution:
    get:
      summary: Get Distribution
      description: Get the information about a distribution.
      operationId: getDistribution
      x-api-path-slug: actiongetdistribution-get
      parameters:
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: HostId.N
        description: The IDs of the Dedicated Hosts
        type: string
      - in: query
        name: Id
        description: The distributions ID
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return for the request in a
          single page
        type: string
      - in: query
        name: NextToken
        description: The token to retrieve the next page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Distribution
  /?Action=GetDistributionConfig:
    get:
      summary: Get Distribution Config
      description: Get the configuration information about a distribution.
      operationId: getDistributionConfig
      x-api-path-slug: actiongetdistributionconfig-get
      parameters:
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: Id
        description: The distributions ID
        type: string
      - in: query
        name: MaxDuration
        description: This is the maximum duration of the reservation youd like to
          purchase, specified            in seconds
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return for the request in a
          single page
        type: string
      - in: query
        name: MinDuration
        description: This is the minimum duration of the reservation youd like to
          purchase, specified            in seconds
        type: string
      - in: query
        name: NextToken
        description: The token to use to retrieve the next page of results
        type: string
      - in: query
        name: OfferingId
        description: The ID of the reservation offering
        type: string
      responses:
        200:
          description: OK
      tags:
      - Distribution
      - Config
  /?Action=GetInvalidation:
    get:
      summary: Get Invalidation
      description: Get the information about an invalidation.
      operationId: getInvalidation
      x-api-path-slug: actiongetinvalidation-get
      parameters:
      - in: query
        name: DistributionId
        description: The distributions ID
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: HostReservationIdSet.N
        description: One or more host reservation IDs
        type: string
      - in: query
        name: Id
        description: The identifier for the invalidation request, for example,      IDFDVBD632BHDS5
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return for the request in a
          single page
        type: string
      - in: query
        name: NextToken
        description: The token to use to retrieve the next page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Invalidation
  /?Action=GetStreamingDistribution:
    get:
      summary: Get Streaming Distribution
      description: |-
        Gets information about a specified RTMP distribution, including the distribution
              configuration.
      operationId: getStreamingDistribution
      x-api-path-slug: actiongetstreamingdistribution-get
      parameters:
      - in: query
        name: HostIdSet.N
        description: The ID/s of the Dedicated Host/s that the reservation will be
          associated            with
        type: string
      - in: query
        name: Id
        description: The streaming distributions ID
        type: string
      - in: query
        name: OfferingId
        description: The offering ID of the reservation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Streaming
      - Distribution
  /?Action=GetStreamingDistributionConfig:
    get:
      summary: Get Streaming Distribution Config
      description: Get the configuration information about a streaming distribution.
      operationId: getStreamingDistributionConfig
      x-api-path-slug: actiongetstreamingdistributionconfig-get
      parameters:
      - in: query
        name: AutoPlacement
        description: Specify whether to enable or disable auto-placement
        type: string
      - in: query
        name: HostId.N
        description: The host IDs of the Dedicated Hosts you want to modify
        type: string
      - in: query
        name: Id
        description: The streaming distributions ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Streaming
      - Distribution
      - Config
  /?Action=ListCloudFrontOriginAccessIdentities:
    get:
      summary: List Cloud Front Origin Access Identities
      description: Lists origin access identities.
      operationId: listCloudFrontOriginAccessIdentities
      x-api-path-slug: actionlistcloudfrontoriginaccessidentities-get
      parameters:
      - in: query
        name: Affinity
        description: The new affinity setting for the instance
        type: string
      - in: query
        name: HostId
        description: The ID of the Dedicated Host that the instance will have affinity
          with
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance that you are modifying
        type: string
      - in: query
        name: Marker
        description: Use this when paginating results to indicate where to begin in
          your list of origin      access identities
        type: string
      - in: query
        name: MaxItems
        description: The maximum number of origin access identities you want in the
          response body
        type: string
      - in: query
        name: Tenancy
        description: The tenancy of the instance that you are modifying
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Cloud
      - Front
      - Origin
      - Access
      - Identities
  /?Action=ListDistributions:
    get:
      summary: List Distributions
      description: List distributions.
      operationId: listDistributions
      x-api-path-slug: actionlistdistributions-get
      parameters:
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure idempotency
          of the request
        type: string
      - in: query
        name: CurrencyCode
        description: The currency in which the totalUpfrontPrice, LimitPrice,            and
          totalHourlyPrice amounts are specified
        type: string
      - in: query
        name: HostIdSet.N
        description: The ID/s of the Dedicated Host/s that the reservation will be
          associated            with
        type: string
      - in: query
        name: LimitPrice
        description: The specified limit is checked against the total upfront cost
          of the reservation            (calculated as the offerings upfront cost
          multiplied by the host count)
        type: string
      - in: query
        name: Marker
        description: Use this when paginating results to indicate where to begin in
          your list of      distributions
        type: string
      - in: query
        name: MaxItems
        description: The maximum number of distributions you want in the response
          body
        type: string
      - in: query
        name: OfferingId
        description: The ID of the offering
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Distributions
  /?Action=ListDistributionsByWebACLId:
    get:
      summary: List Distributions By Web A C L Id
      description: List the distributions that are associated with a specified AWS
        WAF web ACL.
      operationId: listDistributionsByWebACLId
      x-api-path-slug: actionlistdistributionsbywebaclid-get
      parameters:
      - in: query
        name: HostId.N
        description: The IDs of the Dedicated Hosts you want to release
        type: string
      - in: query
        name: Marker
        description: Use Marker and MaxItems to control pagination of results
        type: string
      - in: query
        name: MaxItems
        description: The maximum number of distributions that you want CloudFront
          to return in the response body
        type: string
      - in: query
        name: WebACLId
        description: The ID of the AWS WAF web ACL that you want to list the associated
          distributions
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Distributions
      - Web
      - C
      - L
      - Id
  /?Action=ListInvalidations:
    get:
      summary: List Invalidations
      description: Lists invalidation batches.
      operationId: listInvalidations
      x-api-path-slug: actionlistinvalidations-get
      parameters:
      - in: query
        name: DhcpOptionsId
        description: The ID of the DHCP options set, or default to associate         no
          DHCP options with the VPC
        type: string
      - in: query
        name: DistributionId
        description: The distributions ID
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Marker
        description: Use this parameter when paginating results to indicate where
          to begin in your list of      invalidation batches
        type: string
      - in: query
        name: MaxItems
        description: The maximum number of invalidation batches that you want in the
          response      body
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Invalidations
  /?Action=ListStreamingDistributions:
    get:
      summary: List Streaming Distributions
      description: List streaming distributions.
      operationId: listStreamingDistributions
      x-api-path-slug: actionliststreamingdistributions-get
      parameters:
      - in: query
        name: DhcpConfiguration.N
        description: A DHCP configuration option
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Marker
        description: The value that you provided for the Marker request parameter
        type: string
      - in: query
        name: MaxItems
        description: The value that you provided for the MaxItems request parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Streaming
      - Distributions
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: List tags for a CloudFront resource.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: DhcpOptionsId
        description: The ID of the DHCP options set
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Resource
        description: An ARN of a CloudFront resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Tags
      - Resource
  /?Action=TagResource:
    get:
      summary: Tag Resource
      description: Add tags to a CloudFront resource.
      operationId: tagResource
      x-api-path-slug: actiontagresource-get
      parameters:
      - in: query
        name: DhcpOptionsId.N
        description: The IDs of one or more DHCP options sets
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: Resource
        description: An ARN of a CloudFront resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Resource
  /?Action=UntagResource:
    get:
      summary: Untag Resource
      description: Remove tags from a CloudFront resource.
      operationId: untagResource
      x-api-path-slug: actionuntagresource-get
      parameters:
      - in: query
        name: Device
        description: The device name to expose to the instance (for example, /dev/sdh
          or        xvdh)
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: Resource
        description: An ARN of a CloudFront resource
        type: string
      - in: query
        name: VolumeId
        description: The ID of the EBS volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Untag
      - Resource
  /?Action=UpdateCloudFrontOriginAccessIdentity:
    get:
      summary: Update Cloud Front Origin Access Identity
      description: Update an origin access identity.
      operationId: updateCloudFrontOriginAccessIdentity
      x-api-path-slug: actionupdatecloudfrontoriginaccessidentity-get
      parameters:
      - in: query
        name: Description
        description: A description for the EBS snapshot
        type: string
      - in: query
        name: DestinationRegion
        description: The destination region to use in the PresignedUrl parameter of
          a snapshot copy      operation
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Encrypted
        description: Specifies whether the destination snapshot should be encrypted
        type: string
      - in: query
        name: Id
        description: The identitys id
        type: string
      - in: query
        name: If-Match
        description: The value of the ETag header that you received when retrieving
          the      identitys configuration
        type: string
      - in: query
        name: KmsKeyId
        description: The full ARN of the AWS Key Management Service (AWS KMS) CMK
          to use when creating the snapshot copy
        type: string
      - in: query
        name: PresignedUrl
        description: The pre-signed URL that facilitates copying an encrypted snapshot
        type: string
      - in: query
        name: SourceRegion
        description: The ID of the region that contains the snapshot to be copied
        type: string
      - in: query
        name: SourceSnapshotId
        description: The ID of the EBS snapshot to copy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cloud
      - Front
      - Origin
      - Access
      - Identity
  /?Action=UpdateDistribution:
    get:
      summary: Update Distribution
      description: Update a distribution.
      operationId: updateDistribution
      x-api-path-slug: actionupdatedistribution-get
      parameters:
      - in: query
        name: Description
        description: A description for the snapshot
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Id
        description: The distributions id
        type: string
      - in: query
        name: If-Match
        description: The value of the ETag header that you received when retrieving
          the      distributions configuration
        type: string
      - in: query
        name: VolumeId
        description: The ID of the EBS volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Distribution
  /?Action=UpdateStreamingDistribution:
    get:
      summary: Update Streaming Distribution
      description: Update a streaming distribution.
      operationId: updateStreamingDistribution
      x-api-path-slug: actionupdatestreamingdistribution-get
      parameters:
      - in: query
        name: AvailabilityZone
        description: The Availability Zone in which to create the volume
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Encrypted
        description: Specifies whether the volume should be encrypted
        type: string
      - in: query
        name: Id
        description: The streaming distributions id
        type: string
      - in: query
        name: If-Match
        description: The value of the ETag header that you received when retrieving
          the      streaming distributions configuration
        type: string
      - in: query
        name: Iops
        description: Only valid for Provisioned IOPS SSD volumes
        type: string
      - in: query
        name: KmsKeyId
        description: The full ARN of the AWS Key Management Service (AWS KMS) customer
          master key (CMK) to use when creating the encrypted      volume
        type: string
      - in: query
        name: Size
        description: The size of the volume, in GiBs
        type: string
      - in: query
        name: SnapshotId
        description: The snapshot from which to create the volume
        type: string
      - in: query
        name: VolumeType
        description: The volume type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Streaming
      - Distribution