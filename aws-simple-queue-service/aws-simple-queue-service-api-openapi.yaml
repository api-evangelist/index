swagger: "2.0"
x-collection-name: AWS Simple Queue Service
x-complete: 1
info:
  title: AWS Simple Queue Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddPermission:
    get:
      summary: Add Permission
      description: Adds a permission to a queue for a specific.
      operationId: addPermission
      x-api-path-slug: actionaddpermission-get
      parameters:
      - in: query
        name: ActionName.N
        description: The action the client wants to allow for the specified principal
        type: string
      - in: query
        name: AWSAccountId.N
        description: The AWS account number of the principal who is given permission
        type: string
      - in: query
        name: Label
        description: The unique identification of the permission youre setting (for
          example, AliceSendMessage)
        type: string
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue to which permissions are added
        type: string
      responses:
        200:
          description: OK
      tags:
      - Permissions
  /?Action=ChangeMessageVisibility:
    get:
      summary: Change Message Visibility
      description: Changes the visibility timeout of a specified message in a queue
        to a new value.
      operationId: changeMessageVisibility
      x-api-path-slug: actionchangemessagevisibility-get
      parameters:
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue whose messages visibility is
          changed
        type: string
      - in: query
        name: ReceiptHandle
        description: The receipt handle associated with the message whose visibility
          timeout is changed
        type: string
      - in: query
        name: VisibilityTimeout
        description: The new value for the messages visibility timeout (in seconds)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Message Visibility
  /?Action=ChangeMessageVisibilityBatch:
    get:
      summary: Change Message Visibility Batch
      description: Changes the visibility timeout of multiple messages.
      operationId: changeMessageVisibilityBatch
      x-api-path-slug: actionchangemessagevisibilitybatch-get
      parameters:
      - in: query
        name: ChangeMessageVisibilityBatchRequestEntry.N
        description: A list of receipt handles of the messages for which the visibility
          timeout must be changed
        type: string
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue whose messages visibility is
          changed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Message Visibility
  /?Action=CreateQueue:
    get:
      summary: Create Queue
      description: Creates a new standard or FIFO queue or returns the URL of an existing
        queue.
      operationId: createQueue
      x-api-path-slug: actioncreatequeue-get
      parameters:
      - in: query
        name: |-
          Attribute
                      , Attribute.N.Name (key), Attribute.N.Value (value)
        description: A map of attributes with their corresponding values
        type: string
      - in: query
        name: QueueName
        description: The name of the new queue
        type: string
      responses:
        200:
          description: OK
      tags:
      - Queues
  /?Action=DeleteMessage:
    get:
      summary: Delete Message
      description: Deletes the specified message from the specified queue.
      operationId: deleteMessage
      x-api-path-slug: actiondeletemessage-get
      parameters:
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue from which messages are deleted
        type: string
      - in: query
        name: ReceiptHandle
        description: The receipt handle associated with the message to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Messages
  /?Action=DeleteMessageBatch:
    get:
      summary: Delete Message Batch
      description: Deletes up to ten messages from the specified queue.
      operationId: deleteMessageBatch
      x-api-path-slug: actiondeletemessagebatch-get
      parameters:
      - in: query
        name: DeleteMessageBatchRequestEntry.N
        description: A list of receipt handles for the messages to be deleted
        type: string
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue from which messages are deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Messages
  /?Action=DeleteQueue:
    get:
      summary: Delete Queue
      description: Deletes the queue specified by the QueueUrl, even if the queue
        is empty.
      operationId: deleteQueue
      x-api-path-slug: actiondeletequeue-get
      parameters:
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Queues
  /?Action=GetQueueAttributes:
    get:
      summary: Get Queue Attributes
      description: Gets attributes for the specified queue.
      operationId: getQueueAttributes
      x-api-path-slug: actiongetqueueattributes-get
      parameters:
      - in: query
        name: AttributeName.N
        description: A list of attributes for which to retrieve information
        type: string
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue whose attribute information is
          retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Queues
  /?Action=GetQueueUrl:
    get:
      summary: Get Queue Url
      description: Returns the URL of an existing queue.
      operationId: getQueueUrl
      x-api-path-slug: actiongetqueueurl-get
      parameters:
      - in: query
        name: QueueName
        description: The name of the queue whose URL must be fetched
        type: string
      - in: query
        name: QueueOwnerAWSAccountId
        description: The AWS account ID of the account that created the queue
        type: string
      responses:
        200:
          description: OK
      tags:
      - Queues
  /?Action=ListDeadLetterSourceQueues:
    get:
      summary: List Dead Letter Source Queues
      description: Returns a list of your queues that have the RedrivePolicy queue
        attribute configured with a dead letter queue.
      operationId: listDeadLetterSourceQueues
      x-api-path-slug: actionlistdeadlettersourcequeues-get
      parameters:
      - in: query
        name: QueueUrl
        description: The URL of a dead letter queue
        type: string
      responses:
        200:
          description: OK
      tags:
      - Queues
  /?Action=ListQueues:
    get:
      summary: List Queues
      description: Returns a list of your queues.
      operationId: listQueues
      x-api-path-slug: actionlistqueues-get
      parameters:
      - in: query
        name: QueueNamePrefix
        description: A string to use for filtering the list results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Queues
  /?Action=PurgeQueue:
    get:
      summary: Purge Queue
      description: Deletes the messages in a queue specified by the QueueURL parameter.
      operationId: purgeQueue
      x-api-path-slug: actionpurgequeue-get
      parameters:
      - in: query
        name: QueueUrl
        description: The URL of the queue from which the PurgeQueue action deletes
          messages
        type: string
      responses:
        200:
          description: OK
      tags:
      - Queues
  /?Action=ReceiveMessage:
    get:
      summary: Receive Message
      description: Retrieves one or more messages (up to 10), from the specified queue.
      operationId: receiveMessage
      x-api-path-slug: actionreceivemessage-get
      parameters:
      - in: query
        name: AttributeName.N
        description: A list of attributes that need to be returned along with each
          message
        type: string
      - in: query
        name: MaxNumberOfMessages
        description: The maximum number of messages to return
        type: string
      - in: query
        name: MessageAttributeName.N
        description: The name of the message attribute, where N is the index
        type: string
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue from which messages are received
        type: string
      - in: query
        name: ReceiveRequestAttemptId
        description: This parameter applies only to FIFO (first-in-first-out) queues
        type: string
      - in: query
        name: VisibilityTimeout
        description: The duration (in seconds) that the received messages are hidden
          from subsequent retrieve requests after being retrieved by a ReceiveMessage
          request
        type: string
      - in: query
        name: WaitTimeSeconds
        description: The duration (in seconds) for which the call waits for a message
          to arrive in the queue before returning
        type: string
      responses:
        200:
          description: OK
      tags:
      - Messages
  /?Action=RemovePermission:
    get:
      summary: Remove Permission
      description: Revokes any permissions in the queue policy that matches the specified
        Label parameter.
      operationId: removePermission
      x-api-path-slug: actionremovepermission-get
      parameters:
      - in: query
        name: Label
        description: The identification of the permission to remove
        type: string
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue from which permissions are removed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Permissions
  /?Action=SendMessage:
    get:
      summary: Send Message
      description: Delivers a message to the specified queue.
      operationId: sendMessage
      x-api-path-slug: actionsendmessage-get
      parameters:
      - in: query
        name: DelaySeconds
        description: The number of seconds to delay a specific message
        type: string
      - in: query
        name: |-
          MessageAttribute
                      , MessageAttribute.N.Name (key), MessageAttribute.N.Value (value)
        description: Each message attribute consists of a Name, Type, and Value
        type: string
      - in: query
        name: MessageBody
        description: The message to send
        type: string
      - in: query
        name: MessageDeduplicationId
        description: This parameter applies only to FIFO (first-in-first-out) queues
        type: string
      - in: query
        name: MessageGroupId
        description: This parameter applies only to FIFO (first-in-first-out) queues
        type: string
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue to which a message is sent
        type: string
      responses:
        200:
          description: OK
      tags:
      - Messages
  /?Action=SendMessageBatch:
    get:
      summary: Send Message Batch
      description: Delivers up to ten messages to the specified queue.
      operationId: sendMessageBatch
      x-api-path-slug: actionsendmessagebatch-get
      parameters:
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue to which batched messages are
          sent
        type: string
      - in: query
        name: SendMessageBatchRequestEntry.N
        description: A list of                      SendMessageBatchRequestEntry                   items
        type: string
      responses:
        200:
          description: OK
      tags:
      - Messages
  /?Action=SetQueueAttributes:
    get:
      summary: Set Queue Attributes
      description: Sets the value of one or more queue attributes.
      operationId: setQueueAttributes
      x-api-path-slug: actionsetqueueattributes-get
      parameters:
      - in: query
        name: |-
          Attribute
                      , Attribute.N.Name (key), Attribute.N.Value (value)
        description: A map of attributes to set
        type: string
      - in: query
        name: QueueUrl
        description: The URL of the Amazon SQS queue whose attributes are set
        type: string
      responses:
        200:
          description: OK
      tags:
      - Queues