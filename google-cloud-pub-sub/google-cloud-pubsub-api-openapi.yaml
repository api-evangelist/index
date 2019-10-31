swagger: "2.0"
x-collection-name: Google Cloud Pub Sub
x-complete: 1
info:
  title: Google Cloud Pub/Sub
  description: provides-reliable-manytomany-asynchronous-messaging-between-applications-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: pubsub.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:
    put:
      summary: Create Topic
      description: Creates the given topic with the given name.
      operationId: pubsub.projects.topics.create
      x-api-path-slug: v1name-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The name of the topic
      responses:
        200:
          description: OK
      tags:
      - Topic
  /v1/{project}/subscriptions:
    get:
      summary: List Matching Subscription
      description: Lists matching subscriptions.
      operationId: pubsub.projects.subscriptions.list
      x-api-path-slug: v1projectsubscriptions-get
      parameters:
      - in: query
        name: pageSize
        description: Maximum number of subscriptions to return
      - in: query
        name: pageToken
        description: The value returned by the last `ListSubscriptionsResponse`; indicates
          thatthis is a continuation of a prior `ListSubscriptions` call, and that
          thesystem should return the next page of data
      - in: path
        name: project
        description: The name of the cloud project that subscriptions belong to
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /v1/{project}/topics:
    get:
      summary: List Matching Topics
      description: Lists matching topics.
      operationId: pubsub.projects.topics.list
      x-api-path-slug: v1projecttopics-get
      parameters:
      - in: query
        name: pageSize
        description: Maximum number of topics to return
      - in: query
        name: pageToken
        description: The value returned by the last `ListTopicsResponse`; indicates
          that this isa continuation of a prior `ListTopics` call, and that the system
          shouldreturn the next page of data
      - in: path
        name: project
        description: The name of the cloud project that topics belong to
      responses:
        200:
          description: OK
      tags:
      - Topic
  /v1/{resource}:getIamPolicy:
    get:
      summary: Get IAM Policy
      description: |-
        Gets the access control policy for a resource.
        Returns an empty policy if the resource exists and does not have a policy
        set.
      operationId: pubsub.projects.topics.getIamPolicy
      x-api-path-slug: v1resourcegetiampolicy-get
      parameters:
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy is being requested'
      responses:
        200:
          description: OK
      tags:
      - IAM
  /v1/{resource}:setIamPolicy:
    post:
      summary: Set IAM Policy
      description: |-
        Sets the access control policy on the specified resource. Replaces any
        existing policy.
      operationId: pubsub.projects.topics.setIamPolicy
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
      - IAM
  /v1/{resource}:testIamPermissions:
    post:
      summary: Test IAM Permission
      description: |-
        Returns permissions that a caller has on the specified resource.
        If the resource does not exist, this will return an empty set of
        permissions, not a NOT_FOUND error.

        Note: This operation is designed to be used for building permission-aware
        UIs and command-line tools, not for authorization checking. This operation
        may "fail open" without warning.
      operationId: pubsub.projects.topics.testIamPermissions
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
      - IAM
  /v1/{subscription}:
    delete:
      summary: Delete Subscription
      description: |-
        Deletes an existing subscription. All messages retained in the subscription
        are immediately dropped. Calls to `Pull` after deletion will return
        `NOT_FOUND`. After a subscription is deleted, a new one may be created with
        the same name, but the new one has no association with the old
        subscription or its topic unless the same topic is specified.
      operationId: pubsub.projects.subscriptions.delete
      x-api-path-slug: v1subscription-delete
      parameters:
      - in: path
        name: subscription
        description: The subscription to delete
      responses:
        200:
          description: OK
      tags:
      - Subscription
    get:
      summary: Get Subscription
      description: Gets the configuration details of a subscription.
      operationId: pubsub.projects.subscriptions.get
      x-api-path-slug: v1subscription-get
      parameters:
      - in: path
        name: subscription
        description: The name of the subscription to get
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /v1/{subscription}:acknowledge:
    post:
      summary: Acknowledge Subscription
      description: |-
        Acknowledges the messages associated with the `ack_ids` in the
        `AcknowledgeRequest`. The Pub/Sub system can remove the relevant messages
        from the subscription.

        Acknowledging a message whose ack deadline has expired may succeed,
        but such a message may be redelivered later. Acknowledging a message more
        than once will not result in an error.
      operationId: pubsub.projects.subscriptions.acknowledge
      x-api-path-slug: v1subscriptionacknowledge-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: subscription
        description: The subscription whose message is being acknowledged
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /v1/{subscription}:modifyAckDeadline:
    post:
      summary: Modify ACK Deadline
      description: |-
        Modifies the ack deadline for a specific message. This method is useful
        to indicate that more time is needed to process a message by the
        subscriber, or to make the message available for redelivery if the
        processing was interrupted. Note that this does not modify the
        subscription-level `ackDeadlineSeconds` used for subsequent messages.
      operationId: pubsub.projects.subscriptions.modifyAckDeadline
      x-api-path-slug: v1subscriptionmodifyackdeadline-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: subscription
        description: The name of the subscription
      responses:
        200:
          description: OK
      tags:
      - ACK Deadline
  /v1/{subscription}:modifyPushConfig:
    post:
      summary: Modify Push Configuration
      description: |-
        Modifies the `PushConfig` for a specified subscription.

        This may be used to change a push subscription to a pull one (signified by
        an empty `PushConfig`) or vice versa, or change the endpoint URL and other
        attributes of a push subscription. Messages will accumulate for delivery
        continuously through the call regardless of changes to the `PushConfig`.
      operationId: pubsub.projects.subscriptions.modifyPushConfig
      x-api-path-slug: v1subscriptionmodifypushconfig-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: subscription
        description: The name of the subscription
      responses:
        200:
          description: OK
      tags:
      - Push Configuration
  /v1/{subscription}:pull:
    post:
      summary: Pull Message
      description: |-
        Pulls messages from the server. Returns an empty list if there are no
        messages available in the backlog. The server may return `UNAVAILABLE` if
        there are too many concurrent pull requests pending for the given
        subscription.
      operationId: pubsub.projects.subscriptions.pull
      x-api-path-slug: v1subscriptionpull-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: subscription
        description: The subscription from which messages should be pulled
      responses:
        200:
          description: OK
      tags:
      - Message
  /v1/{topic}:
    delete:
      summary: Delete Topic
      description: |-
        Deletes the topic with the given name. Returns `NOT_FOUND` if the topic
        does not exist. After a topic is deleted, a new topic may be created with
        the same name; this is an entirely new topic with none of the old
        configuration or subscriptions. Existing subscriptions to this topic are
        not deleted, but their `topic` field is set to `_deleted-topic_`.
      operationId: pubsub.projects.topics.delete
      x-api-path-slug: v1topic-delete
      parameters:
      - in: path
        name: topic
        description: Name of the topic to delete
      responses:
        200:
          description: OK
      tags:
      - Topic
    get:
      summary: Get Topic Configuration
      description: Gets the configuration of a topic.
      operationId: pubsub.projects.topics.get
      x-api-path-slug: v1topic-get
      parameters:
      - in: path
        name: topic
        description: The name of the topic to get
      responses:
        200:
          description: OK
      tags:
      - Topic
  /v1/{topic}/subscriptions:
    get:
      summary: Get Topic Subscription
      description: Lists the name of the subscriptions for this topic.
      operationId: pubsub.projects.topics.subscriptions.list
      x-api-path-slug: v1topicsubscriptions-get
      parameters:
      - in: query
        name: pageSize
        description: Maximum number of subscription names to return
      - in: query
        name: pageToken
        description: The value returned by the last `ListTopicSubscriptionsResponse`;
          indicatesthat this is a continuation of a prior `ListTopicSubscriptions`
          call, andthat the system should return the next page of data
      - in: path
        name: topic
        description: The name of the topic that subscriptions are attached to
      responses:
        200:
          description: OK
      tags:
      - Topic
  /v1/{topic}:publish:
    post:
      summary: Publish Topic
      description: |-
        Adds one or more messages to the topic. Returns `NOT_FOUND` if the topic
        does not exist. The message payload must not be empty; it must contain
         either a non-empty data field, or at least one attribute.
      operationId: pubsub.projects.topics.publish
      x-api-path-slug: v1topicpublish-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: topic
        description: The messages in the request will be published on this topic
      responses:
        200:
          description: OK
      tags:
      - Topic