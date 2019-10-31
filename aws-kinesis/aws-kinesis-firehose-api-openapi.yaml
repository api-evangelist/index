swagger: "2.0"
x-collection-name: AWS Kinesis
x-complete: 1
info:
  title: AWS Kinesis Firehose API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateDeliveryStream:
    get:
      summary: Create Delivery Stream
      description: creates a delivery stream.
      operationId: CreateDeliveryStream
      x-api-path-slug: actioncreatedeliverystream-get
      parameters:
      - in: query
        name: DeliveryStreamName
        description: The name of the delivery stream
        type: string
      - in: query
        name: ElasticsearchDestinationConfiguration
        description: The destination in Amazon ES
        type: string
      - in: query
        name: ExtendedS3DestinationConfiguration
        description: The destination in Amazon S3
        type: string
      - in: query
        name: RedshiftDestinationConfiguration
        description: The destination in Amazon Redshift
        type: string
      - in: query
        name: S3DestinationConfiguration
        description: '[Deprecated] The destination in Amazon S3'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Streams
  /?Action=DeleteDeliveryStream:
    get:
      summary: Delete Delivery Stream
      description: deletes a delivery stream and its data.
      operationId: DeleteDeliveryStream
      x-api-path-slug: actiondeletedeliverystream-get
      parameters:
      - in: query
        name: DeliveryStreamName
        description: The name of the delivery stream
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Streams
  /?Action=DescribeDeliveryStream:
    get:
      summary: Describe Delivery Stream
      description: describes the specified delivery stream and gets the status.
      operationId: DescribeDeliveryStream
      x-api-path-slug: actiondescribedeliverystream-get
      parameters:
      - in: query
        name: DeliveryStreamName
        description: The name of the delivery stream
        type: string
      - in: query
        name: ExclusiveStartDestinationId
        description: The ID of the destination to start returning the destination
          information
        type: string
      - in: query
        name: Limit
        description: The limit on the number of destinations to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Streams
  /?Action=ListDeliveryStreams:
    get:
      summary: List Delivery Streams
      description: lists your delivery streams.
      operationId: ListDeliveryStreams
      x-api-path-slug: actionlistdeliverystreams-get
      parameters:
      - in: query
        name: ExclusiveStartDeliveryStreamName
        description: The name of the delivery stream to start the list with
        type: string
      - in: query
        name: Limit
        description: The maximum number of delivery streams to list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Streams
  /?Action=PutRecord:
    get:
      summary: Put Record
      description: writes a single data record into an Amazon Kinesis Firehose delivery
        stream.
      operationId: PutRecord
      x-api-path-slug: actionputrecord-get
      parameters:
      - in: query
        name: DeliveryStreamName
        description: The name of the delivery stream
        type: string
      - in: query
        name: Record
        description: The record
        type: string
      responses:
        200:
          description: OK
      tags:
      - Records
  /?Action=PutRecordBatch:
    get:
      summary: Put Record Batch
      description: |-
        writes multiple data records into a delivery stream in a single call, which can
                 achieve higher throughput per producer than when writing single records.
      operationId: PutRecordBatch
      x-api-path-slug: actionputrecordbatch-get
      parameters:
      - in: query
        name: DeliveryStreamName
        description: The name of the delivery stream
        type: string
      - in: query
        name: Records
        description: One or more records
        type: string
      responses:
        200:
          description: OK
      tags:
      - Records
  /?Action=UpdateDestination:
    get:
      summary: Update Destination
      description: updates the specified destination of the specified delivery stream.
      operationId: UpdateDestination
      x-api-path-slug: actionupdatedestination-get
      parameters:
      - in: query
        name: CurrentDeliveryStreamVersionId
        description: Obtain this value from the VersionId result of             DeliveryStreamDescription
        type: string
      - in: query
        name: DeliveryStreamName
        description: The name of the delivery stream
        type: string
      - in: query
        name: DestinationId
        description: The ID of the destination
        type: string
      - in: query
        name: ElasticsearchDestinationUpdate
        description: Describes an update for a destination in Amazon ES
        type: string
      - in: query
        name: ExtendedS3DestinationUpdate
        description: Describes an update for a destination in Amazon S3
        type: string
      - in: query
        name: RedshiftDestinationUpdate
        description: Describes an update for a destination in Amazon Redshift
        type: string
      - in: query
        name: S3DestinationUpdate
        description: '[Deprecated] Describes an update for a destination in Amazon
          S3'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Destinations