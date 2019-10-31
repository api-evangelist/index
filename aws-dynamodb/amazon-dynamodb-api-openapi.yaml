swagger: "2.0"
x-collection-name: AWS DynamoDB
x-complete: 1
info:
  title: AWS DynamoDB API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=BatchGetItem:
    get:
      summary: Batch Get Item
      description: |-
        The BatchGetItem operation returns the attributes of one or more items from one or
              more tables.
      operationId: batchGetItem
      x-api-path-slug: actionbatchgetitem-get
      parameters:
      - in: query
        name: RequestItems
        description: A map of one or more table names and, for each table, a map that
          describes one or more items to retrieve from that table
        type: string
      - in: query
        name: ReturnConsumedCapacity
        description: 'Determines the level of detail about provisioned throughput
          consumption that is returned in the response:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Batch Items
  /?Action=BatchWriteItem:
    get:
      summary: Batch Write Item
      description: The BatchWriteItem operation puts or deletes multiple items in
        one or more tables.
      operationId: batchWriteItem
      x-api-path-slug: actionbatchwriteitem-get
      parameters:
      - in: query
        name: RequestItems
        description: A map of one or more table names and, for each table, a list
          of operations to be performed        (DeleteRequest or PutRequest)
        type: string
      - in: query
        name: ReturnConsumedCapacity
        description: 'Determines the level of detail about provisioned throughput
          consumption that is returned in the response:'
        type: string
      - in: query
        name: ReturnItemCollectionMetrics
        description: Determines whether item collection metrics are returned
        type: string
      responses:
        200:
          description: OK
      tags:
      - Batch Items
  /?Action=CreateTable:
    get:
      summary: Create Table
      description: The CreateTable operation adds a new table to your account.
      operationId: createTable
      x-api-path-slug: actioncreatetable-get
      parameters:
      - in: query
        name: AttributeDefinitions
        description: An array of attributes that describe the key schema for the table
          and indexes
        type: string
      - in: query
        name: GlobalSecondaryIndexes
        description: One or more global secondary indexes (the maximum is five) to
          be created on the table
        type: string
      - in: query
        name: KeySchema
        description: Specifies the attributes that make up the primary key for a table
          or an index
        type: string
      - in: query
        name: LocalSecondaryIndexes
        description: One or more local secondary indexes (the maximum is five) to
          be created on the table
        type: string
      - in: query
        name: ProvisionedThroughput
        description: Represents the provisioned throughput settings for a specified
          table or index
        type: string
      - in: query
        name: StreamSpecification
        description: The settings for DynamoDB Streams on the table
        type: string
      - in: query
        name: TableName
        description: The name of the table to create
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tables
  /?Action=DeleteItem:
    get:
      summary: Delete Item
      description: Deletes a single item in a table by primary key.
      operationId: deleteItem
      x-api-path-slug: actiondeleteitem-get
      parameters:
      - in: query
        name: ConditionalOperator
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConditionExpression
        description: A condition that must be satisfied in order for a conditional
          DeleteItem to      succeed
        type: string
      - in: query
        name: Expected
        description: This is a legacy parameter
        type: string
      - in: query
        name: ExpressionAttributeNames
        description: One or more substitution tokens for attribute names in an expression
        type: string
      - in: query
        name: ExpressionAttributeValues
        description: One or more values that can be substituted in an expression
        type: string
      - in: query
        name: Key
        description: A map of attribute names to AttributeValue objects, representing
          the primary key of      the item to delete
        type: string
      - in: query
        name: ReturnConsumedCapacity
        description: 'Determines the level of detail about provisioned throughput
          consumption that is returned in the response:'
        type: string
      - in: query
        name: ReturnItemCollectionMetrics
        description: Determines whether item collection metrics are returned
        type: string
      - in: query
        name: ReturnValues
        description: Use ReturnValues if you want to get the item attributes as they
          appeared before they      were deleted
        type: string
      - in: query
        name: TableName
        description: The name of the table from which to delete the item
        type: string
      responses:
        200:
          description: OK
      tags:
      - Items
  /?Action=DeleteTable:
    get:
      summary: Delete Table
      description: The DeleteTable operation deletes a table and all of its items.
      operationId: deleteTable
      x-api-path-slug: actiondeletetable-get
      parameters:
      - in: query
        name: TableName
        description: The name of the table to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tables
  /?Action=DescribeLimits:
    get:
      summary: Describe Limits
      description: Returns the current provisioned-capacity limits for your AWS account
        in a region, both for the region as a whole and for any one DynamoDB table
        that you create there.
      operationId: describeLimits
      x-api-path-slug: actiondescribelimits-get
      parameters:
      - in: query
        name: AccountMaxReadCapacityUnits
        description: The maximum total read capacity units that your account allows
          you to provision across all of your tables in this region
        type: string
      - in: query
        name: AccountMaxWriteCapacityUnits
        description: The maximum total write capacity units that your account allows
          you to provision across all of your tables in this region
        type: string
      - in: query
        name: TableMaxReadCapacityUnits
        description: The maximum read capacity units that your account allows you
          to provision for a new table that you are creating in this region, including
          the read capacity units provisioned for its global secondary indexes (GSIs)
        type: string
      - in: query
        name: TableMaxWriteCapacityUnits
        description: The maximum write capacity units that your account allows you
          to provision for a new table that you are creating in this region, including
          the write capacity units provisioned for its global secondary indexes (GSIs)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Limits
  /?Action=DescribeTable:
    get:
      summary: Describe Table
      description: Returns information about the table, including the current status
        of the table, when it was created, the primary key schema, and any indexes
        on the table.
      operationId: describeTable
      x-api-path-slug: actiondescribetable-get
      parameters:
      - in: query
        name: TableName
        description: The name of the table to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tables
  /?Action=GetItem:
    get:
      summary: Get Item
      description: |-
        The GetItem operation returns a set of attributes for the item with the given primary
                  key.
      operationId: getItem
      x-api-path-slug: actiongetitem-get
      parameters:
      - in: query
        name: AttributesToGet
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConsistentRead
        description: 'Determines the read consistency model:  If set to true, then
          the operation uses strongly consistent reads; otherwise, the operation uses
          eventually consistent reads'
        type: string
      - in: query
        name: ExpressionAttributeNames
        description: One or more substitution tokens for attribute names in an expression
        type: string
      - in: query
        name: Key
        description: A map of attribute names to AttributeValue objects, representing
          the primary key of      the item to retrieve
        type: string
      - in: query
        name: ProjectionExpression
        description: A string that identifies one or more attributes to retrieve from
          the table
        type: string
      - in: query
        name: ReturnConsumedCapacity
        description: 'Determines the level of detail about provisioned throughput
          consumption that is returned in the response:'
        type: string
      - in: query
        name: TableName
        description: The name of the table containing the requested item
        type: string
      responses:
        200:
          description: OK
      tags:
      - Items
  /?Action=ListTables:
    get:
      summary: List Tables
      description: Returns an array of table names associated with the current account
        and endpoint.
      operationId: listTables
      x-api-path-slug: actionlisttables-get
      parameters:
      - in: query
        name: ExclusiveStartTableName
        description: The first table name that this operation will evaluate
        type: string
      - in: query
        name: Limit
        description: A maximum number of table names to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tables
  /?Action=PutItem:
    get:
      summary: Put Item
      description: Creates a new item, or replaces an old item with a new item.
      operationId: putItem
      x-api-path-slug: actionputitem-get
      parameters:
      - in: query
        name: ConditionalOperator
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConditionExpression
        description: A condition that must be satisfied in order for a conditional
          PutItem operation to      succeed
        type: string
      - in: query
        name: Expected
        description: This is a legacy parameter
        type: string
      - in: query
        name: ExpressionAttributeNames
        description: One or more substitution tokens for attribute names in an expression
        type: string
      - in: query
        name: ExpressionAttributeValues
        description: One or more values that can be substituted in an expression
        type: string
      - in: query
        name: Item
        description: A map of attribute name/value pairs, one for each attribute
        type: string
      - in: query
        name: ReturnConsumedCapacity
        description: 'Determines the level of detail about provisioned throughput
          consumption that is returned in the response:'
        type: string
      - in: query
        name: ReturnItemCollectionMetrics
        description: Determines whether item collection metrics are returned
        type: string
      - in: query
        name: ReturnValues
        description: Use ReturnValues if you want to get the item attributes as they
          appeared before they      were updated with the PutItem request
        type: string
      - in: query
        name: TableName
        description: The name of the table to contain the item
        type: string
      responses:
        200:
          description: OK
      tags:
      - Items
  /?Action=Query:
    get:
      summary: Query
      description: |-
        A Query operation uses the primary key of a table or a secondary index
                    to directly access items from that table or index.
      operationId: query
      x-api-path-slug: actionquery-get
      parameters:
      - in: query
        name: AttributesToGet
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConditionalOperator
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConsistentRead
        description: 'Determines the read consistency model:  If set to true, then
          the operation uses strongly consistent reads; otherwise, the operation uses
          eventually consistent reads'
        type: string
      - in: query
        name: ExclusiveStartKey
        description: The primary key of the first item that this operation will evaluate
        type: string
      - in: query
        name: ExpressionAttributeNames
        description: One or more substitution tokens for attribute names in an expression
        type: string
      - in: query
        name: ExpressionAttributeValues
        description: One or more values that can be substituted in an expression
        type: string
      - in: query
        name: FilterExpression
        description: A string that contains conditions that DynamoDB applies after
          the Query operation, but       before the data is returned to you
        type: string
      - in: query
        name: IndexName
        description: The name of an index to query
        type: string
      - in: query
        name: KeyConditionExpression
        description: The condition that specifies the key value(s) for items to be
          retrieved by the Query      action
        type: string
      - in: query
        name: KeyConditions
        description: This is a legacy parameter
        type: string
      - in: query
        name: Limit
        description: The maximum number of items to evaluate (not necessarily the
          number of matching items)
        type: string
      - in: query
        name: ProjectionExpression
        description: A string that identifies one or more attributes to retrieve from
          the table
        type: string
      - in: query
        name: QueryFilter
        description: This is a legacy parameter
        type: string
      - in: query
        name: ReturnConsumedCapacity
        description: 'Determines the level of detail about provisioned throughput
          consumption that is returned in the response:'
        type: string
      - in: query
        name: ScanIndexForward
        description: 'Specifies the order for index traversal: If true (default),
          the traversal is performed in ascending order; if false, the traversal is
          performed in descending order'
        type: string
      - in: query
        name: Select
        description: The attributes to be returned in the          result
        type: string
      - in: query
        name: TableName
        description: The name of the table containing the requested items
        type: string
      responses:
        200:
          description: OK
      tags:
      - Query
  /?Action=Scan:
    get:
      summary: Scan
      description: |-
        The Scan operation returns one or more items and item attributes by accessing every
              item in a table or a secondary index.
      operationId: scan
      x-api-path-slug: actionscan-get
      parameters:
      - in: query
        name: AttributesToGet
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConditionalOperator
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConsistentRead
        description: 'A Boolean value that determines the read consistency model during
          the scan:'
        type: string
      - in: query
        name: ExclusiveStartKey
        description: The primary key of the first item that this operation will evaluate
        type: string
      - in: query
        name: ExpressionAttributeNames
        description: One or more substitution tokens for attribute names in an expression
        type: string
      - in: query
        name: ExpressionAttributeValues
        description: One or more values that can be substituted in an expression
        type: string
      - in: query
        name: FilterExpression
        description: A string that contains conditions that DynamoDB applies after
          the Scan operation, but       before the data is returned to you
        type: string
      - in: query
        name: IndexName
        description: The name of a secondary index to scan
        type: string
      - in: query
        name: Limit
        description: The maximum number of items to evaluate (not necessarily the
          number of matching items)
        type: string
      - in: query
        name: ProjectionExpression
        description: A string that identifies one or more attributes to retrieve from
          the specified table or index
        type: string
      - in: query
        name: ReturnConsumedCapacity
        description: 'Determines the level of detail about provisioned throughput
          consumption that is returned in the response:'
        type: string
      - in: query
        name: ScanFilter
        description: This is a legacy parameter
        type: string
      - in: query
        name: Segment
        description: For a parallel Scan request, Segment identifies an individual
          segment to be      scanned by an application worker
        type: string
      - in: query
        name: Select
        description: The attributes to be returned in the            result
        type: string
      - in: query
        name: TableName
        description: The name of the table containing the requested items; or, if
          you provide             IndexName, the name of the table to which that index
          belongs
        type: string
      - in: query
        name: TotalSegments
        description: For a parallel Scan request, TotalSegments represents the total
          number of      segments into which the Scan operation will be divided
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scan
  /?Action=UpdateItem:
    get:
      summary: Update Item
      description: Edits an existing item's attributes, or adds a new item to the
        table if it does not already exist.
      operationId: updateItem
      x-api-path-slug: actionupdateitem-get
      parameters:
      - in: query
        name: AttributeUpdates
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConditionalOperator
        description: This is a legacy parameter
        type: string
      - in: query
        name: ConditionExpression
        description: A condition that must be satisfied in order for a conditional
          update to succeed
        type: string
      - in: query
        name: Expected
        description: This is a legacy parameter
        type: string
      - in: query
        name: ExpressionAttributeNames
        description: One or more substitution tokens for attribute names in an expression
        type: string
      - in: query
        name: ExpressionAttributeValues
        description: One or more values that can be substituted in an expression
        type: string
      - in: query
        name: Key
        description: The primary key of the item to be updated
        type: string
      - in: query
        name: ReturnConsumedCapacity
        description: 'Determines the level of detail about provisioned throughput
          consumption that is returned in the response:'
        type: string
      - in: query
        name: ReturnItemCollectionMetrics
        description: Determines whether item collection metrics are returned
        type: string
      - in: query
        name: ReturnValues
        description: Use ReturnValues if you want to get the item attributes as they
          appeared either before      or after they were updated
        type: string
      - in: query
        name: TableName
        description: The name of the table containing the item to update
        type: string
      - in: query
        name: UpdateExpression
        description: An expression that defines one or more attributes to be updated,
          the action to be performed on them, and new value(s) for them
        type: string
      responses:
        200:
          description: OK
      tags:
      - Items
  /?Action=UpdateTable:
    get:
      summary: Update Table
      description: Modifies the provisioned throughput settings, global secondary
        indexes, or DynamoDB Streams settings for a given table.
      operationId: updateTable
      x-api-path-slug: actionupdatetable-get
      parameters:
      - in: query
        name: AttributeDefinitions
        description: An array of attributes that describe the key schema for the table
          and indexes
        type: string
      - in: query
        name: GlobalSecondaryIndexUpdates
        description: An array of one or more global secondary indexes for the table
        type: string
      - in: query
        name: ProvisionedThroughput
        description: The new provisioned throughput settings for the specified table
          or index
        type: string
      - in: query
        name: StreamSpecification
        description: Represents the DynamoDB Streams configuration for the table
        type: string
      - in: query
        name: TableName
        description: The name of the table to be updated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tables