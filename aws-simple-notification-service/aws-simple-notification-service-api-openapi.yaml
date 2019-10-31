swagger: "2.0"
x-collection-name: AWS Simple Notification Service
x-complete: 1
info:
  title: AWS Simple Notification Service API
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
      description: Adds a statement to a topic's access control policy, granting access
        for the specified AWS accounts to the specified actions.
      operationId: addPermission
      x-api-path-slug: actionaddpermission-get
      parameters:
      - in: query
        name: ActionName.member.N
        description: The action you want to allow for the specified principal(s)
        type: string
      - in: query
        name: AWSAccountId.member.N
        description: The AWS account IDs of the users (principals) who will be given
          access to the specified actions
        type: string
      - in: query
        name: Label
        description: A unique identifier for the new policy statement
        type: string
      - in: query
        name: TopicArn
        description: The ARN of the topic whose access control policy you wish to
          modify
        type: string
      responses:
        200:
          description: OK
      tags:
      - Permissions
  /?Action=CheckIfPhoneNumberIsOptedOut:
    get:
      summary: Check If Phone Number Is Opted Out
      description: Accepts a phone number and indicates whether the phone holder has
        opted out of receiving SMS messages from your account.
      operationId: checkIfPhoneNumberIsOptedOut
      x-api-path-slug: actioncheckifphonenumberisoptedout-get
      parameters:
      - in: query
        name: phoneNumber
        description: The phone number for which you want to check the opt out status
        type: string
      responses:
        200:
          description: OK
      tags:
      - Opt Out
  /?Action=ConfirmSubscription:
    get:
      summary: Confirm Subscription
      description: |-
        Verifies an endpoint owner's intent to receive messages by validating the token sent to the
              endpoint by an earlier Subscribe action.
      operationId: confirmSubscription
      x-api-path-slug: actionconfirmsubscription-get
      parameters:
      - in: query
        name: AuthenticateOnUnsubscribe
        description: Disallows unauthenticated unsubscribes of the subscription
        type: string
      - in: query
        name: Token
        description: Short-lived token sent to an endpoint during the Subscribe action
        type: string
      - in: query
        name: TopicArn
        description: The ARN of the topic for which you wish to confirm a subscription
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=CreatePlatformApplication:
    get:
      summary: Create Platform Application
      description: |-
        Creates a platform application object for one of the supported push notification services,
              such as APNS and GCM, to which devices and mobile apps may register.
      operationId: createPlatformApplication
      x-api-path-slug: actioncreateplatformapplication-get
      parameters:
      - in: query
        name: |-
          Attributes
                      , Attributes.entry.N.key (key), Attributesentry.N.value (value)
        description: For a list of attributes, see SetPlatformApplicationAttributes
        type: string
      - in: query
        name: Name
        description: Application names must be made up of only uppercase and lowercase
          ASCII letters, numbers, underscores, hyphens, and periods, and must be between
          1 and 256 characters long
        type: string
      - in: query
        name: Platform
        description: 'The following platforms are supported: ADM (Amazon Device Messaging),
          APNS (Apple Push Notification Service), APNS_SANDBOX, and GCM (Google Cloud
          Messaging)'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Platform Applications
  /?Action=CreatePlatformEndpoint:
    get:
      summary: Create Platform Endpoint
      description: |-
        Creates an endpoint for a device and mobile app on one of the supported push notification
              services, such as GCM and APNS.
      operationId: createPlatformEndpoint
      x-api-path-slug: actioncreateplatformendpoint-get
      parameters:
      - in: query
        name: |-
          Attributes
                      , Attributes.entry.N.key (key), Attributesentry.N.value (value)
        description: For a list of attributes, see SetEndpointAttributes
        type: string
      - in: query
        name: CustomUserData
        description: Arbitrary user data to associate with the endpoint
        type: string
      - in: query
        name: PlatformApplicationArn
        description: PlatformApplicationArn returned from CreatePlatformApplication
          is used to create a an endpoint
        type: string
      - in: query
        name: Token
        description: Unique identifier created by the notification service for an
          app on a device
        type: string
      responses:
        200:
          description: OK
      tags:
      - Platform Endpoints
  /?Action=CreateTopic:
    get:
      summary: Create Topic
      description: Creates a topic to which notifications can be published.
      operationId: createTopic
      x-api-path-slug: actioncreatetopic-get
      parameters:
      - in: query
        name: Name
        description: The name of the topic you want to create
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topics
  /?Action=DeleteEndpoint:
    get:
      summary: Delete Endpoint
      description: Deletes the endpoint for a device and mobile app from Amazon SNS.
      operationId: deleteEndpoint
      x-api-path-slug: actiondeleteendpoint-get
      parameters:
      - in: query
        name: EndpointArn
        description: EndpointArn of endpoint to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /?Action=DeletePlatformApplication:
    get:
      summary: Delete Platform Application
      description: |-
        Deletes a platform application object for one of the supported push notification services,
              such as APNS and GCM.
      operationId: deletePlatformApplication
      x-api-path-slug: actiondeleteplatformapplication-get
      parameters:
      - in: query
        name: PlatformApplicationArn
        description: PlatformApplicationArn of platform application object to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Platform Applications
  /?Action=DeleteTopic:
    get:
      summary: Delete Topic
      description: Deletes a topic and all its subscriptions.
      operationId: deleteTopic
      x-api-path-slug: actiondeletetopic-get
      parameters:
      - in: query
        name: TopicArn
        description: The ARN of the topic you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topics
  /?Action=GetEndpointAttributes:
    get:
      summary: Get Endpoint Attributes
      description: |-
        Retrieves the endpoint attributes for a device on one of the supported push notification
              services, such as GCM and APNS.
      operationId: getEndpointAttributes
      x-api-path-slug: actiongetendpointattributes-get
      parameters:
      - in: query
        name: EndpointArn
        description: EndpointArn for GetEndpointAttributes input
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /?Action=GetPlatformApplicationAttributes:
    get:
      summary: Get Platform Application Attributes
      description: |-
        Retrieves the attributes of the platform application object for the supported push
              notification services, such as APNS and GCM.
      operationId: getPlatformApplicationAttributes
      x-api-path-slug: actiongetplatformapplicationattributes-get
      parameters:
      - in: query
        name: PlatformApplicationArn
        description: PlatformApplicationArn for GetPlatformApplicationAttributesInput
        type: string
      responses:
        200:
          description: OK
      tags:
      - Platform Applications
  /?Action=GetSMSAttributes:
    get:
      summary: Get S M S Attributes
      description: Returns the settings for sending SMS messages from your account.
      operationId: getSMSAttributes
      x-api-path-slug: actiongetsmsattributes-get
      parameters:
      - in: query
        name: attributes.member.N
        description: A list of the individual attribute names, such as MonthlySpendLimit,
          for which      you want values
        type: string
      responses:
        200:
          description: OK
      tags:
      - SMS
  /?Action=GetSubscriptionAttributes:
    get:
      summary: Get Subscription Attributes
      description: Returns all of the properties of a subscription.
      operationId: getSubscriptionAttributes
      x-api-path-slug: actiongetsubscriptionattributes-get
      parameters:
      - in: query
        name: SubscriptionArn
        description: The ARN of the subscription whose properties you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=GetTopicAttributes:
    get:
      summary: Get Topic Attributes
      description: Returns all of the properties of a topic.
      operationId: getTopicAttributes
      x-api-path-slug: actiongettopicattributes-get
      parameters:
      - in: query
        name: TopicArn
        description: The ARN of the topic whose properties you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topics
  /?Action=ListEndpointsByPlatformApplication:
    get:
      summary: List Endpoints By Platform Application
      description: |-
        Lists the endpoints and endpoint attributes for devices in a supported push notification
              service, such as GCM and APNS.
      operationId: listEndpointsByPlatformApplication
      x-api-path-slug: actionlistendpointsbyplatformapplication-get
      parameters:
      - in: query
        name: NextToken
        description: NextToken string is used when calling ListEndpointsByPlatformApplication
          action to retrieve additional records that are available after the first
          page results
        type: string
      - in: query
        name: PlatformApplicationArn
        description: PlatformApplicationArn for ListEndpointsByPlatformApplicationInput
          action
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /?Action=ListPhoneNumbersOptedOut:
    get:
      summary: List Phone Numbers Opted Out
      description: Returns a list of phone numbers that are opted out, meaning you
        cannot send SMS messages to them.
      operationId: listPhoneNumbersOptedOut
      x-api-path-slug: actionlistphonenumbersoptedout-get
      parameters:
      - in: query
        name: nextToken
        description: A NextToken string is used when you call the      ListPhoneNumbersOptedOut
          action to retrieve additional records that are      available after the
          first page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Opt Out
  /?Action=ListPlatformApplications:
    get:
      summary: List Platform Applications
      description: |-
        Lists the platform application objects for the supported push notification services, such as
              APNS and GCM.
      operationId: listPlatformApplications
      x-api-path-slug: actionlistplatformapplications-get
      parameters:
      - in: query
        name: NextToken
        description: NextToken string is used when calling ListPlatformApplications
          action to retrieve additional records that are available after the first
          page results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Platform Applications
  /?Action=ListSubscriptions:
    get:
      summary: List Subscriptions
      description: Returns a list of the requester's subscriptions.
      operationId: listSubscriptions
      x-api-path-slug: actionlistsubscriptions-get
      parameters:
      - in: query
        name: NextToken
        description: Token returned by the previous ListSubscriptions request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=ListSubscriptionsByTopic:
    get:
      summary: List Subscriptions By Topic
      description: Returns a list of the subscriptions to a specific topic.
      operationId: listSubscriptionsByTopic
      x-api-path-slug: actionlistsubscriptionsbytopic-get
      parameters:
      - in: query
        name: NextToken
        description: Token returned by the previous ListSubscriptionsByTopic request
        type: string
      - in: query
        name: TopicArn
        description: The ARN of the topic for which you wish to find subscriptions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=ListTopics:
    get:
      summary: List Topics
      description: Returns a list of the requester's topics.
      operationId: listTopics
      x-api-path-slug: actionlisttopics-get
      parameters:
      - in: query
        name: NextToken
        description: Token returned by the previous ListTopics request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topics
  /?Action=OptInPhoneNumber:
    get:
      summary: Opt In Phone Number
      description: Use this request to opt in a phone number that is opted out, which
        enables you to resume sending SMS messages to the number.
      operationId: optInPhoneNumber
      x-api-path-slug: actionoptinphonenumber-get
      parameters:
      - in: query
        name: phoneNumber
        description: The phone number to opt in
        type: string
      responses:
        200:
          description: OK
      tags:
      - Opt Out
  /?Action=Publish:
    get:
      summary: Publish
      description: Sends a message to all of a topic's subscribed endpoints.
      operationId: publish
      x-api-path-slug: actionpublish-get
      parameters:
      - in: query
        name: Message
        description: The message you want to send to the topic
        type: string
      - in: query
        name: |-
          MessageAttributes
                      , MessageAttributes.entry.N.Name (key), MessageAttributesentry.N.Value (value)
        description: Message attributes for Publish action
        type: string
      - in: query
        name: MessageStructure
        description: Set MessageStructure to json if you want to send a different      message
          for each protocol
        type: string
      - in: query
        name: PhoneNumber
        description: The phone number to which you want to deliver an SMS message
        type: string
      - in: query
        name: Subject
        description: Optional parameter to be used as the Subject line when the message
          is delivered to email endpoints
        type: string
      - in: query
        name: TargetArn
        description: Either TopicArn or EndpointArn, but not both
        type: string
      - in: query
        name: TopicArn
        description: The topic you want to publish to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Publish
  /?Action=RemovePermission:
    get:
      summary: Remove Permission
      description: Removes a statement from a topic's access control policy.
      operationId: removePermission
      x-api-path-slug: actionremovepermission-get
      parameters:
      - in: query
        name: Label
        description: The unique label of the statement you want to remove
        type: string
      - in: query
        name: TopicArn
        description: The ARN of the topic whose access control policy you wish to
          modify
        type: string
      responses:
        200:
          description: OK
      tags:
      - Permissions
  /?Action=SetEndpointAttributes:
    get:
      summary: Set Endpoint Attributes
      description: |-
        Sets the attributes for an endpoint for a device on one of the supported push notification
              services, such as GCM and APNS.
      operationId: setEndpointAttributes
      x-api-path-slug: actionsetendpointattributes-get
      parameters:
      - in: query
        name: |-
          Attributes
                      , Attributes.entry.N.key (key), Attributesentry.N.value (value)
        description: A map of the endpoint attributes
        type: string
      - in: query
        name: EndpointArn
        description: EndpointArn used for SetEndpointAttributes action
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /?Action=SetPlatformApplicationAttributes:
    get:
      summary: Set Platform Application Attributes
      description: |-
        Sets the attributes of the platform application object for the supported push notification
              services, such as APNS and GCM.
      operationId: setPlatformApplicationAttributes
      x-api-path-slug: actionsetplatformapplicationattributes-get
      parameters:
      - in: query
        name: |-
          Attributes
                      , Attributes.entry.N.key (key), Attributesentry.N.value (value)
        description: A map of the platform application attributes
        type: string
      - in: query
        name: PlatformApplicationArn
        description: PlatformApplicationArn for SetPlatformApplicationAttributes action
        type: string
      responses:
        200:
          description: OK
      tags:
      - Platform Applications
  /?Action=SetSMSAttributes:
    get:
      summary: Set SMS Attributes
      description: Use this request to set the default settings for sending SMS messages
        and receiving daily SMS usage reports.
      operationId: setSMSAttributes
      x-api-path-slug: actionsetsmsattributes-get
      parameters:
      - in: query
        name: |-
          attributes
                      , attributes.entry.N.key (key), attributesentry.N.value (value)
        description: The default settings for sending SMS messages from your account
        type: string
      responses:
        200:
          description: OK
      tags:
      - SMS
  /?Action=SetSubscriptionAttributes:
    get:
      summary: Set Subscription Attributes
      description: Allows a subscription owner to set an attribute of the topic to
        a new value.
      operationId: setSubscriptionAttributes
      x-api-path-slug: actionsetsubscriptionattributes-get
      parameters:
      - in: query
        name: AttributeName
        description: The name of the attribute you want to set
        type: string
      - in: query
        name: AttributeValue
        description: The new value for the attribute in JSON format
        type: string
      - in: query
        name: SubscriptionArn
        description: The ARN of the subscription to modify
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=SetTopicAttributes:
    get:
      summary: Set Topic Attributes
      description: Allows a topic owner to set an attribute of the topic to a new
        value.
      operationId: setTopicAttributes
      x-api-path-slug: actionsettopicattributes-get
      parameters:
      - in: query
        name: AttributeName
        description: The name of the attribute you want to set
        type: string
      - in: query
        name: AttributeValue
        description: The new value for the attribute
        type: string
      - in: query
        name: TopicArn
        description: The ARN of the topic to modify
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topics
  /?Action=Subscribe:
    get:
      summary: Subscribe
      description: Prepares to subscribe an endpoint by sending the endpoint a confirmation
        message.
      operationId: subscribe
      x-api-path-slug: actionsubscribe-get
      parameters:
      - in: query
        name: Endpoint
        description: The endpoint that you want to receive notifications
        type: string
      - in: query
        name: Protocol
        description: The protocol you want to use
        type: string
      - in: query
        name: TopicArn
        description: The ARN of the topic you want to subscribe to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /?Action=Unsubscribe:
    get:
      summary: Unsubscribe
      description: Deletes a subscription.
      operationId: unsubscribe
      x-api-path-slug: actionunsubscribe-get
      parameters:
      - in: query
        name: SubscriptionArn
        description: The ARN of the subscription to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""