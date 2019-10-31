swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 1
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ActivateGateway:
    get:
      summary: Activate Gateway
      description: Activates the gateway you previously deployed on your host.
      operationId: activateGateway
      x-api-path-slug: actionactivategateway-get
      parameters:
      - in: query
        name: ActivationKey
        description: Your gateway activation key
        type: string
      - in: query
        name: GatewayName
        description: The name you configured for your gateway
        type: string
      - in: query
        name: GatewayRegion
        description: A value that indicates the region where you want to store the
          snapshot backups
        type: string
      - in: query
        name: GatewayTimezone
        description: A value that indicates the time zone you want to set for the
          gateway
        type: string
      - in: query
        name: GatewayType
        description: A value that defines the type of gateway to activate
        type: string
      - in: query
        name: MediumChangerType
        description: The value that indicates the type of medium changer to use for
          gateway-VTL
        type: string
      - in: query
        name: TapeDriveType
        description: The value that indicates the type of tape drive to use for gateway-VTL
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
  /?Action=AddCache:
    get:
      summary: Add Cache
      description: Configures one or more gateway local disks as cache for a cached-volume
        gateway.
      operationId: addCache
      x-api-path-slug: actionaddcache-get
      parameters:
      - in: query
        name: DiskIds
        description: 'Type: array of Strings'
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache
  /?Action=AddTagsToResource:
    get:
      summary: Add Tags To Resource
      description: Adds one or more tags to the specified resource.
      operationId: addTagsToResource
      x-api-path-slug: actionaddtagstoresource-get
      parameters:
      - in: query
        name: ResourceARN
        description: The Amazon Resource Name (ARN) of the resource you want to add
          tags to
        type: string
      - in: query
        name: Tags
        description: The key-value pair that represents the tag you want to add to
          the resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=AddUploadBuffer:
    get:
      summary: Add Upload Buffer
      description: Configures one or more gateway local disks as upload buffer for
        a specified gateway.
      operationId: addUploadBuffer
      x-api-path-slug: actionadduploadbuffer-get
      parameters:
      - in: query
        name: DiskIds
        description: 'Type: array of Strings'
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload Buffer
  /?Action=AddWorkingStorage:
    get:
      summary: Add Working Storage
      description: Configures one or more gateway local disks as working storage for
        a gateway.
      operationId: addWorkingStorage
      x-api-path-slug: actionaddworkingstorage-get
      parameters:
      - in: query
        name: DiskIds
        description: An array of strings that identify disks that are to be configured
          as working storage
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Working Storage
  /?Action=CancelArchival:
    get:
      summary: Cancel Archival
      description: |-
        Cancels archiving of a virtual tape to the virtual tape shelf (VTS) after the
                 archiving process is initiated.
      operationId: cancelArchival
      x-api-path-slug: actioncancelarchival-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: TapeARN
        description: The Amazon Resource Name (ARN) of the virtual tape you want to
          cancel archiving         for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Archival
  /?Action=CancelRetrieval:
    get:
      summary: Cancel Retrieval
      description: |-
        Cancels retrieval of a virtual tape from the virtual tape shelf (VTS) to a gateway
                 after the retrieval process is initiated.
      operationId: cancelRetrieval
      x-api-path-slug: actioncancelretrieval-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: TapeARN
        description: The Amazon Resource Name (ARN) of the virtual tape you want to
          cancel retrieval         for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Retrieval
  /?Action=CreateCachediSCSIVolume:
    get:
      summary: Create Cached SCSI Volume
      description: Creates a cached volume on a specified cached gateway.
      operationId: createCachediSCSIVolume
      x-api-path-slug: actioncreatecachediscsivolume-get
      parameters:
      - in: query
        name: ClientToken
        description: 'Type: String'
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: NetworkInterfaceId
        description: 'Type: String'
        type: string
      - in: query
        name: SnapshotId
        description: 'Type: String'
        type: string
      - in: query
        name: SourceVolumeARN
        description: The ARN for an existing volume
        type: string
      - in: query
        name: TargetName
        description: 'Type: String'
        type: string
      - in: query
        name: VolumeSizeInBytes
        description: 'Type: Long'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cached SCSI Volume
  /?Action=CreateNFSFileShare:
    get:
      summary: Create NFS File Share
      description: Creates a file share on an existing file gateway.
      operationId: createNFSFileShare
      x-api-path-slug: actioncreatenfsfileshare-get
      parameters:
      - in: query
        name: ClientToken
        description: A unique string value that you supply that is used by file gateway
          to ensure         idempotent file share creation
        type: string
      - in: query
        name: DefaultStorageClass
        description: The default storage class for objects put into an Amazon S3 bucket
          by file gateway
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the file gateway on which you
          want to create a file share
        type: string
      - in: query
        name: KMSEncrypted
        description: True to use Amazon S3 server side encryption with your own AWS
          KMS key, or false to         use a key managed by Amazon S3
        type: string
      - in: query
        name: KMSKey
        description: The KMS key used for Amazon S3 server side encryption
        type: string
      - in: query
        name: LocationARN
        description: The ARN of the backend storage used for storing file data
        type: string
      - in: query
        name: NFSFileShareDefaults
        description: File share default values
        type: string
      - in: query
        name: Role
        description: The ARN of the AWS Identity and Access Management (IAM) role
          that a file gateway         assumes when it accesses the underlying storage
        type: string
      responses:
        200:
          description: OK
      tags:
      - NFS File Share
  /?Action=CreateSnapshot:
    get:
      summary: Create Snapshot
      description: Initiates a snapshot of a volume.
      operationId: createSnapshot
      x-api-path-slug: actioncreatesnapshot-get
      parameters:
      - in: query
        name: SnapshotDescription
        description: Textual description of the snapshot that appears in the Amazon
          EC2 console, Elastic         Block Store snapshots panel in the Description
          field, and         in the AWS Storage Gateway snapshot Details pane,            Description
          field
        type: string
      - in: query
        name: VolumeARN
        description: The Amazon Resource Name (ARN) of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=CreateSnapshotFromVolumeRecoveryPoint:
    get:
      summary: Create Snapshot From Volume Recovery Point
      description: Initiates a snapshot of a gateway from a volume recovery point.
      operationId: createSnapshotFromVolumeRecoveryPoint
      x-api-path-slug: actioncreatesnapshotfromvolumerecoverypoint-get
      parameters:
      - in: query
        name: SnapshotDescription
        description: 'Type: String'
        type: string
      - in: query
        name: VolumeARN
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=CreateStorediSCSIVolume:
    get:
      summary: Create Stored SCSI Volume
      description: Creates a volume on a specified gateway.
      operationId: createStorediSCSIVolume
      x-api-path-slug: actioncreatestorediscsivolume-get
      parameters:
      - in: query
        name: DiskId
        description: The unique identifier for the gateway local disk that is configured
          as a stored         volume
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The network interface of the gateway on which to expose the iSCSI
          target
        type: string
      - in: query
        name: PreserveExistingData
        description: Specify this field as true if you want to preserve the data on
          the local disk
        type: string
      - in: query
        name: SnapshotId
        description: The snapshot ID (e
        type: string
      - in: query
        name: TargetName
        description: The name of the iSCSI target used by initiators to connect to
          the target and as a         suffix for the target ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stored SCSI Volume
  /?Action=CreateTapes:
    get:
      summary: Create Tapes
      description: Creates one or more virtual tapes.
      operationId: createTapes
      x-api-path-slug: actioncreatetapes-get
      parameters:
      - in: query
        name: ClientToken
        description: A unique identifier that you use to retry a request
        type: string
      - in: query
        name: GatewayARN
        description: The unique Amazon Resource Name (ARN) that represents the gateway
          to associate the         virtual tapes with
        type: string
      - in: query
        name: NumTapesToCreate
        description: The number of virtual tapes that you want to create
        type: string
      - in: query
        name: TapeBarcodePrefix
        description: A prefix that you append to the barcode of the virtual tape you
          are creating
        type: string
      - in: query
        name: TapeSizeInBytes
        description: The size, in bytes, of the virtual tapes that you want to create
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tapes
  /?Action=CreateTapeWithBarcode:
    get:
      summary: Create Tape With Barcode
      description: Creates a virtual tape by using your own barcode.
      operationId: createTapeWithBarcode
      x-api-path-slug: actioncreatetapewithbarcode-get
      parameters:
      - in: query
        name: GatewayARN
        description: The unique Amazon Resource Name (ARN) that represents the gateway
          to associate the         virtual tape with
        type: string
      - in: query
        name: TapeBarcode
        description: The barcode that you want to assign to the tape
        type: string
      - in: query
        name: TapeSizeInBytes
        description: The size, in bytes, of the virtual tape that you want to create
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tape With Barcode
  /?Action=DeleteBandwidthRateLimit:
    get:
      summary: Delete Bandwidth Rate Limit
      description: Deletes the bandwidth rate limits of a gateway.
      operationId: deleteBandwidthRateLimit
      x-api-path-slug: actiondeletebandwidthratelimit-get
      parameters:
      - in: query
        name: BandwidthType
        description: One of the BandwidthType values that indicates the gateway         bandwidth
          rate limit to delete
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bandwidth Rate Limit
  /?Action=DeleteChapCredentials:
    get:
      summary: Delete Chap Credentials
      description: |-
        Deletes Challenge-Handshake Authentication Protocol (CHAP) credentials for a
                 specified iSCSI target and initiator pair.
      operationId: deleteChapCredentials
      x-api-path-slug: actiondeletechapcredentials-get
      parameters:
      - in: query
        name: InitiatorName
        description: The iSCSI initiator that connects to the target
        type: string
      - in: query
        name: TargetARN
        description: The Amazon Resource Name (ARN) of the iSCSI volume target
        type: string
      responses:
        200:
          description: OK
      tags:
      - Chap Credentials
  /?Action=DeleteFileShare:
    get:
      summary: Delete File Share
      description: Deletes a file share from a file gateway.
      operationId: deleteFileShare
      x-api-path-slug: actiondeletefileshare-get
      parameters:
      - in: query
        name: FileShareARN
        description: The Amazon Resource Name (ARN) of the file share to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - File Share
  /?Action=DeleteGateway:
    get:
      summary: Delete Gateway
      description: Deletes a gateway.
      operationId: deleteGateway
      x-api-path-slug: actiondeletegateway-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
  /?Action=DeleteSnapshotSchedule:
    get:
      summary: Delete Snapshot Schedule
      description: Deletes a snapshot of a volume.
      operationId: deleteSnapshotSchedule
      x-api-path-slug: actiondeletesnapshotschedule-get
      parameters:
      - in: query
        name: VolumeARN
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DeleteTape:
    get:
      summary: Delete Tape
      description: Deletes the specified virtual tape.
      operationId: deleteTape
      x-api-path-slug: actiondeletetape-get
      parameters:
      - in: query
        name: GatewayARN
        description: The unique Amazon Resource Name (ARN) of the gateway that the
          virtual tape to delete         is associated with
        type: string
      - in: query
        name: TapeARN
        description: The Amazon Resource Name (ARN) of the virtual tape to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tapes
  /?Action=DeleteTapeArchive:
    get:
      summary: Delete Tape Archive
      description: Deletes the specified virtual tape from the virtual tape shelf
        (VTS).
      operationId: deleteTapeArchive
      x-api-path-slug: actiondeletetapearchive-get
      parameters:
      - in: query
        name: TapeARN
        description: The Amazon Resource Name (ARN) of the virtual tape to delete
          from the virtual tape         shelf (VTS)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tapes
      - Archives
  /?Action=DeleteVolume:
    get:
      summary: Delete Volume
      description: Deletes the specified gateway volume that you previously created
        using the.
      operationId: deleteVolume
      x-api-path-slug: actiondeletevolume-get
      parameters:
      - in: query
        name: VolumeARN
        description: The Amazon Resource Name (ARN) of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Volumes
  /?Action=DescribeBandwidthRateLimit:
    get:
      summary: Describe Bandwidth Rate Limit
      description: Returns the bandwidth rate limits of a gateway.
      operationId: describeBandwidthRateLimit
      x-api-path-slug: actiondescribebandwidthratelimit-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bandwidth Rate Limit
  /?Action=DescribeCache:
    get:
      summary: Describe Cache
      description: Returns information about the cache of a gateway.
      operationId: describeCache
      x-api-path-slug: actiondescribecache-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache
  /?Action=DescribeCachediSCSIVolumes:
    get:
      summary: Describe Cached SCSI Volumes
      description: Returns a description of the gateway volumes specified in the request.
      operationId: describeCachediSCSIVolumes
      x-api-path-slug: actiondescribecachediscsivolumes-get
      parameters:
      - in: query
        name: VolumeARNs
        description: 'Type: array of Strings'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cached SCSI Volumes
  /?Action=DescribeChapCredentials:
    get:
      summary: Describe Chap Credentials
      description: |-
        Returns an array of Challenge-Handshake Authentication Protocol (CHAP) credentials
                 information for a specified iSCSI target, one for each target-initiator pair.
      operationId: describeChapCredentials
      x-api-path-slug: actiondescribechapcredentials-get
      parameters:
      - in: query
        name: TargetARN
        description: The Amazon Resource Name (ARN) of the iSCSI volume target
        type: string
      responses:
        200:
          description: OK
      tags:
      - Chap Credentials
  /?Action=DescribeGatewayInformation:
    get:
      summary: Describe Gateway Information
      description: |-
        Returns metadata about a gateway such as its name, network interfaces, configured
                 time zone, and the state (whether the gateway is running or not).
      operationId: describeGatewayInformation
      x-api-path-slug: actiondescribegatewayinformation-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
  /?Action=DescribeMaintenanceStartTime:
    get:
      summary: Describe Maintenance Start Time
      description: |-
        Returns your gateway's weekly maintenance start time including the day and time of
                 the week.
      operationId: describeMaintenanceStartTime
      x-api-path-slug: actiondescribemaintenancestarttime-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
  /?Action=DescribeNFSFileShares:
    get:
      summary: Describe NFS File Shares
      description: Gets a description for one or more file shares from a file gateway.
      operationId: describeNFSFileShares
      x-api-path-slug: actiondescribenfsfileshares-get
      parameters:
      - in: query
        name: FileShareARNList
        description: An array containing the Amazon Resource Name (ARN) of each file
          share to be described
        type: string
      responses:
        200:
          description: OK
      tags:
      - NFS File Shares
  /?Action=DescribeSnapshotSchedule:
    get:
      summary: Describe Snapshot Schedule
      description: Describes the snapshot schedule for the specified gateway volume.
      operationId: describeSnapshotSchedule
      x-api-path-slug: actiondescribesnapshotschedule-get
      parameters:
      - in: query
        name: VolumeARN
        description: The Amazon Resource Name (ARN) of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DescribeStorediSCSIVolumes:
    get:
      summary: Describe Stored SCSI Volumes
      description: Returns the description of the gateway volumes specified in the
        request.
      operationId: describeStorediSCSIVolumes
      x-api-path-slug: actiondescribestorediscsivolumes-get
      parameters:
      - in: query
        name: VolumeARNs
        description: An array of strings where each string represents the Amazon Resource
          Name (ARN) of a         stored volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stored SCSI Volumes
  /?Action=DescribeTapeArchives:
    get:
      summary: Describe Tape Archives
      description: |-
        Returns a description of specified virtual tapes in the virtual tape shelf
                 (VTS).
      operationId: describeTapeArchives
      x-api-path-slug: actiondescribetapearchives-get
      parameters:
      - in: query
        name: Limit
        description: Specifies that the number of virtual tapes descried be limited
          to the specified         number
        type: string
      - in: query
        name: Marker
        description: An opaque string that indicates the position at which to begin
          describing virtual         tapes
        type: string
      - in: query
        name: TapeARNs
        description: Specifies one or more unique Amazon Resource Names (ARNs) that
          represent the virtual         tapes you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tape Archives
  /?Action=DescribeTapeRecoveryPoints:
    get:
      summary: Describe Tape Recovery Points
      description: |-
        Returns a list of virtual tape recovery points that are available for the specified
                 gateway-VTL.
      operationId: describeTapeRecoveryPoints
      x-api-path-slug: actiondescribetaperecoverypoints-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: Limit
        description: Specifies that the number of virtual tape recovery points that
          are described be         limited to the specified number
        type: string
      - in: query
        name: Marker
        description: An opaque string that indicates the position at which to begin
          describing the virtual         tape recovery points
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tape Recovery Points
  /?Action=DescribeTapes:
    get:
      summary: Describe Tapes
      description: Returns a description of the specified Amazon Resource Name (ARN)
        of virtual tapes.
      operationId: describeTapes
      x-api-path-slug: actiondescribetapes-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: Limit
        description: Specifies that the number of virtual tapes described be limited
          to the specified         number
        type: string
      - in: query
        name: Marker
        description: A marker value, obtained in a previous call to DescribeTapes
        type: string
      - in: query
        name: TapeARNs
        description: Specifies one or more unique Amazon Resource Names (ARNs) that
          represent the virtual         tapes you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tapes
  /?Action=DescribeUploadBuffer:
    get:
      summary: Describe Upload Buffer
      description: Returns information about the upload buffer of a gateway.
      operationId: describeUploadBuffer
      x-api-path-slug: actiondescribeuploadbuffer-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload Buffer
  /?Action=DescribeVTLDevices:
    get:
      summary: Describe VTL Devices
      description: |-
        Returns a description of virtual tape library (VTL) devices for the specified
                 gateway.
      operationId: describeVTLDevices
      x-api-path-slug: actiondescribevtldevices-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: Limit
        description: Specifies that the number of VTL devices described be limited
          to the specified         number
        type: string
      - in: query
        name: Marker
        description: An opaque string that indicates the position at which to begin
          describing the VTL         devices
        type: string
      - in: query
        name: VTLDeviceARNs
        description: An array of strings, where each string represents the Amazon
          Resource Name (ARN) of a         VTL device
        type: string
      responses:
        200:
          description: OK
      tags:
      - VTL Devices
  /?Action=DescribeWorkingStorage:
    get:
      summary: Describe Working Storage
      description: Returns information about the working storage of a gateway.
      operationId: describeWorkingStorage
      x-api-path-slug: actiondescribeworkingstorage-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Working Storage
  /?Action=DisableGateway:
    get:
      summary: Disable Gateway
      description: Disables a gateway when the gateway is no longer functioning.
      operationId: disableGateway
      x-api-path-slug: actiondisablegateway-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
  /?Action=ListFileShares:
    get:
      summary: List File Shares
      description: Gets a list of the file shares for a specific file gateway, or
        the list of file shares that belong to the calling user account.
      operationId: listFileShares
      x-api-path-slug: actionlistfileshares-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon resource Name (ARN) of the gateway whose file shares
          you want to list
        type: string
      - in: query
        name: Limit
        description: The maximum number of file shares to return in the response
        type: string
      - in: query
        name: Marker
        description: Opaque pagination token returned from a previous ListFileShares
          operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - File Shares
  /?Action=ListGateways:
    get:
      summary: List Gateways
      description: Lists gateways owned by an AWS account in a region specified in
        the request.
      operationId: listGateways
      x-api-path-slug: actionlistgateways-get
      parameters:
      - in: query
        name: Limit
        description: Specifies that the list of gateways returned be limited to the
          specified number of         items
        type: string
      - in: query
        name: Marker
        description: An opaque string that indicates the position at which to begin
          the returned list of         gateways
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateways
  /?Action=ListLocalDisks:
    get:
      summary: List Local Disks
      description: Returns a list of the gateway's local disks.
      operationId: listLocalDisks
      x-api-path-slug: actionlistlocaldisks-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Local Disks
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: Lists the tags that have been added to the specified resource.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: Limit
        description: Specifies that the list of tags returned be limited to the specified
          number of         items
        type: string
      - in: query
        name: Marker
        description: An opaque string that indicates the position at which to begin
          returning the list of         tags
        type: string
      - in: query
        name: ResourceARN
        description: The Amazon Resource Name (ARN) of the resource for which you
          want to list         tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=ListTapes:
    get:
      summary: List Tapes
      description: |-
        Lists virtual tapes in your virtual tape library (VTL) and your virtual tape shelf
                 (VTS).
      operationId: listTapes
      x-api-path-slug: actionlisttapes-get
      parameters:
      - in: query
        name: Limit
        description: An optional number limit for the tapes in the list returned by
          this call
        type: string
      - in: query
        name: Marker
        description: A string that indicates the position at which to begin the returned
          list of         tapes
        type: string
      - in: query
        name: TapeARNs
        description: The Amazon Resource Name (ARN) of each of the tapes you want
          to list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tapes
  /?Action=ListVolumeInitiators:
    get:
      summary: List Volume Initiators
      description: Lists iSCSI initiators that are connected to a volume.
      operationId: listVolumeInitiators
      x-api-path-slug: actionlistvolumeinitiators-get
      parameters:
      - in: query
        name: VolumeARN
        description: The Amazon Resource Name (ARN) of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Volume Initiators
  /?Action=ListVolumeRecoveryPoints:
    get:
      summary: List Volume Recovery Points
      description: Lists the recovery points for a specified gateway.
      operationId: listVolumeRecoveryPoints
      x-api-path-slug: actionlistvolumerecoverypoints-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Volume Recovery
  /?Action=ListVolumes:
    get:
      summary: List Volumes
      description: Lists the iSCSI stored volumes of a gateway.
      operationId: listVolumes
      x-api-path-slug: actionlistvolumes-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: Limit
        description: Specifies that the list of volumes returned be limited to the
          specified number of         items
        type: string
      - in: query
        name: Marker
        description: A string that indicates the position at which to begin the returned
          list of volumes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Volumes
  /?Action=RemoveTagsFromResource:
    get:
      summary: Remove Tags From Resource
      description: Removes one or more tags from the specified resource.
      operationId: removeTagsFromResource
      x-api-path-slug: actionremovetagsfromresource-get
      parameters:
      - in: query
        name: ResourceARN
        description: The Amazon Resource Name (ARN) of the resource you want to remove
          the tags         from
        type: string
      - in: query
        name: TagKeys
        description: The keys of the tags you want to remove from the specified resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=ResetCache:
    get:
      summary: Reset Cache
      description: |-
        Resets all cache disks that have encountered a error and makes the disks available
                 for reconfiguration as cache storage.
      operationId: resetCache
      x-api-path-slug: actionresetcache-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache
  /?Action=RetrieveTapeArchive:
    get:
      summary: Retrieve Tape Archive
      description: |-
        Retrieves an archived virtual tape from the virtual tape shelf (VTS) to a
                 gateway-VTL.
      operationId: retrieveTapeArchive
      x-api-path-slug: actionretrievetapearchive-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway you want to retrieve
          the virtual tape         to
        type: string
      - in: query
        name: TapeARN
        description: The Amazon Resource Name (ARN) of the virtual tape you want to
          retrieve from the         virtual tape shelf (VTS)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tapes
      - Archives
  /?Action=RetrieveTapeRecoveryPoint:
    get:
      summary: Retrieve Tape Recovery Point
      description: Retrieves the recovery point for the specified virtual tape.
      operationId: retrieveTapeRecoveryPoint
      x-api-path-slug: actionretrievetaperecoverypoint-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: TapeARN
        description: The Amazon Resource Name (ARN) of the virtual tape for which
          you want to retrieve the         recovery point
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tape Recovery
  /?Action=SetLocalConsolePassword:
    get:
      summary: Set Local Console Password
      description: Sets the password for your VM local console.
      operationId: setLocalConsolePassword
      x-api-path-slug: actionsetlocalconsolepassword-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: LocalConsolePassword
        description: The password you want to set for your VM local console
        type: string
      responses:
        200:
          description: OK
      tags:
      - Local Console Password
  /?Action=ShutdownGateway:
    get:
      summary: Shutdown Gateway
      description: Shuts down a gateway.
      operationId: shutdownGateway
      x-api-path-slug: actionshutdowngateway-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
  /?Action=StartGateway:
    get:
      summary: Start Gateway
      description: Starts a gateway that you previously shut down (see.
      operationId: startGateway
      x-api-path-slug: actionstartgateway-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
  /?Action=UpdateBandwidthRateLimit:
    get:
      summary: Update Bandwidth Rate Limit
      description: Updates the bandwidth rate limits of a gateway.
      operationId: updateBandwidthRateLimit
      x-api-path-slug: actionupdatebandwidthratelimit-get
      parameters:
      - in: query
        name: AverageDownloadRateLimitInBitsPerSec
        description: The average download bandwidth rate limit in bits per second
        type: string
      - in: query
        name: AverageUploadRateLimitInBitsPerSec
        description: The average upload bandwidth rate limit in bits per second
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bandwidth Rate Limit
  /?Action=UpdateChapCredentials:
    get:
      summary: Update Chap Credentials
      description: |-
        Updates the Challenge-Handshake Authentication Protocol (CHAP) credentials for a
                 specified iSCSI target.
      operationId: updateChapCredentials
      x-api-path-slug: actionupdatechapcredentials-get
      parameters:
      - in: query
        name: InitiatorName
        description: The iSCSI initiator that connects to the target
        type: string
      - in: query
        name: SecretToAuthenticateInitiator
        description: The secret key that the initiator (for example, the Windows client)
          must provide to         participate in mutual CHAP with the target
        type: string
      - in: query
        name: SecretToAuthenticateTarget
        description: The secret key that the target must provide to participate in
          mutual CHAP with the         initiator (e
        type: string
      - in: query
        name: TargetARN
        description: The Amazon Resource Name (ARN) of the iSCSI volume target
        type: string
      responses:
        200:
          description: OK
      tags:
      - Chap Credentials
  /?Action=UpdateGatewayInformation:
    get:
      summary: Update Gateway Information
      description: Updates a gateway's metadata, which includes the gateway's name
        and time zone.
      operationId: updateGatewayInformation
      x-api-path-slug: actionupdategatewayinformation-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: GatewayName
        description: The name you configured for your gateway
        type: string
      - in: query
        name: GatewayTimezone
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
  /?Action=UpdateGatewaySoftwareNow:
    get:
      summary: Update Gateway Software Now
      description: Updates the gateway virtual machine (VM) software.
      operationId: updateGatewaySoftwareNow
      x-api-path-slug: actionupdategatewaysoftwarenow-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Gateway
  /?Action=UpdateMaintenanceStartTime:
    get:
      summary: Update Maintenance Start Time
      description: |-
        Updates a gateway's weekly maintenance start time information, including day and time
                 of the week.
      operationId: updateMaintenanceStartTime
      x-api-path-slug: actionupdatemaintenancestarttime-get
      parameters:
      - in: query
        name: DayOfWeek
        description: The maintenance start time day of the week represented as an
          ordinal number from 0 to 6,          where 0 represents Sunday and 6 Saturday
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: HourOfDay
        description: The hour component of the maintenance start time represented
          as            hh, where hh is the hour (00 to 23)
        type: string
      - in: query
        name: MinuteOfHour
        description: The minute component of the maintenance start time represented
          as            mm, where mm is the minute (00 to 59)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
  /?Action=UpdateNFSFileShare:
    get:
      summary: Update NFS File Share
      description: Updates a file share.
      operationId: updateNFSFileShare
      x-api-path-slug: actionupdatenfsfileshare-get
      parameters:
      - in: query
        name: DefaultStorageClass
        description: The default storage class for objects put into an Amazon S3 bucket
          by a file gateway
        type: string
      - in: query
        name: FileShareARN
        description: The Amazon Resource Name (ARN) of the file share to be updated
        type: string
      - in: query
        name: KMSEncrypted
        description: True to use Amazon S3 server side encryption with your own AWS
          KMS key, or false to         use a key managed by Amazon S3
        type: string
      - in: query
        name: KMSKey
        description: The KMS key used for Amazon S3 server side encryption
        type: string
      - in: query
        name: NFSFileShareDefaults
        description: The default values for the file share
        type: string
      responses:
        200:
          description: OK
      tags:
      - NFS File Share
  /?Action=UpdateSnapshotSchedule:
    get:
      summary: Update Snapshot Schedule
      description: Updates a snapshot schedule configured for a gateway volume.
      operationId: updateSnapshotSchedule
      x-api-path-slug: actionupdatesnapshotschedule-get
      parameters:
      - in: query
        name: Description
        description: Optional description of the snapshot that overwrites the existing         description
        type: string
      - in: query
        name: RecurrenceInHours
        description: Frequency of snapshots
        type: string
      - in: query
        name: StartAt
        description: The hour of the day at which the snapshot schedule begins represented
          as            hh, where hh is the hour (0 to 23)
        type: string
      - in: query
        name: VolumeARN
        description: The Amazon Resource Name (ARN) of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=UpdateVTLDeviceType:
    get:
      summary: Update VTL Device Type
      description: Updates the type of medium changer in a gateway-VTL.
      operationId: updateVTLDeviceType
      x-api-path-slug: actionupdatevtldevicetype-get
      parameters:
      - in: query
        name: DeviceType
        description: The type of medium changer you want to select
        type: string
      - in: query
        name: VTLDeviceARN
        description: The Amazon Resource Name (ARN) of the medium changer you want
          to select
        type: string
      responses:
        200:
          description: OK
      tags:
      - VTL Device Type