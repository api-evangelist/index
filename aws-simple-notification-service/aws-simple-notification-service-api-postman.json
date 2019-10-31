{
  "info": {
    "name": "AWS Simple Notification Service API Unsubscribe",
    "_postman_id": "125877be-917d-4161-adc8-1f06cf759592",
    "description": "Deletes a subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Permissions",
      "item": [
        {
          "id": "9260ac01-fcb0-4f66-94b3-7ecc95125700",
          "name": "addPermission",
          "request": {
            "url": "http://example.com/api/?Action=AddPermission?ActionName.member.N=ActionName.member.N&AWSAccountId.member.N=AWSAccountId.member.N&Label=Label&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a statement to a topic's access control policy, granting access for the specified AWS accounts to the specified actions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b9b23dd-a865-43e1-a156-0dacc0c702eb"
            }
          ]
        },
        {
          "id": "9d0d2370-cf50-49cc-bdcc-b2bd9c2841c1",
          "name": "removePermission",
          "request": {
            "url": "http://example.com/api/?Action=RemovePermission?Label=Label&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a statement from a topic's access control policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f849654-2596-4bc2-ad25-c88ecd1264b5"
            }
          ]
        }
      ]
    },
    {
      "name": "Opt Out",
      "item": [
        {
          "id": "0472c246-d320-4f42-991c-8752aa3b29ff",
          "name": "checkIfPhoneNumberIsOptedOut",
          "request": {
            "url": "http://example.com/api/?Action=CheckIfPhoneNumberIsOptedOut?phoneNumber=phoneNumber",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Accepts a phone number and indicates whether the phone holder has opted out of receiving SMS messages from your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c83e00b-8a4b-4b8c-96d7-2e44839e9234"
            }
          ]
        },
        {
          "id": "d5488a70-93d6-4321-a601-53c457ed1308",
          "name": "listPhoneNumbersOptedOut",
          "request": {
            "url": "http://example.com/api/?Action=ListPhoneNumbersOptedOut?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of phone numbers that are opted out, meaning you cannot send SMS messages to them."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e3798f9-9259-489a-9bd6-733bff4911d8"
            }
          ]
        },
        {
          "id": "a71d8440-d472-4885-8b38-9fb12036aca5",
          "name": "optInPhoneNumber",
          "request": {
            "url": "http://example.com/api/?Action=OptInPhoneNumber?phoneNumber=phoneNumber",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Use this request to opt in a phone number that is opted out, which enables you to resume sending SMS messages to the number."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5d7681f-756b-4054-9912-70a1d4740b0a"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "52533ea7-4347-49f8-aadc-7e5cd650d276",
          "name": "confirmSubscription",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmSubscription?AuthenticateOnUnsubscribe=AuthenticateOnUnsubscribe&Token=Token&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Verifies an endpoint owner's intent to receive messages by validating the token sent to the\n      endpoint by an earlier Subscribe action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e28506d7-5216-4034-ae5b-c33e3bff9661"
            }
          ]
        },
        {
          "id": "b0525aed-e535-4a67-8f76-3cd4ffb0d499",
          "name": "getSubscriptionAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetSubscriptionAttributes?SubscriptionArn=SubscriptionArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all of the properties of a subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66d2d86b-2749-4a41-916d-3eb9f7f23a60"
            }
          ]
        },
        {
          "id": "04c9117e-8cbf-47f0-9989-f92e777430d1",
          "name": "listSubscriptions",
          "request": {
            "url": "http://example.com/api/?Action=ListSubscriptions?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the requester's subscriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9047e7bc-665a-4431-bdd9-3536b4c7b8fb"
            }
          ]
        },
        {
          "id": "9e3e5804-e25d-4415-9426-163bc64aa7bb",
          "name": "listSubscriptionsByTopic",
          "request": {
            "url": "http://example.com/api/?Action=ListSubscriptionsByTopic?NextToken=NextToken&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the subscriptions to a specific topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c6e13a1-c5c5-44b4-a869-6bbe9f3d43d2"
            }
          ]
        },
        {
          "id": "c412eef8-fbb9-4639-b8de-e9d9e8bc1354",
          "name": "setSubscriptionAttributes",
          "request": {
            "url": "http://example.com/api/?Action=SetSubscriptionAttributes?AttributeName=AttributeName&AttributeValue=AttributeValue&SubscriptionArn=SubscriptionArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows a subscription owner to set an attribute of the topic to a new value."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c23387e0-1a56-42bc-9850-38aacee5e94b"
            }
          ]
        }
      ]
    },
    {
      "name": "Platform Applications",
      "item": [
        {
          "id": "42be0dbe-b87f-4f20-89c4-eb10ddd96928",
          "name": "createPlatformApplication",
          "request": {
            "url": "http://example.com/api/?Action=CreatePlatformApplication?Attributes\n            , Attributes.entry.N.key (key), Attributesentry.N.value (value)=Attributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20Attributes.entry.N.key%20%28key%29%2C%20Attributesentry.N.value%20%28value%29&Name=Name&Platform=Platform",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a platform application object for one of the supported push notification services,\n      such as APNS and GCM, to which devices and mobile apps may register."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f863d920-2c88-4e12-8d63-b7f063b4ad45"
            }
          ]
        },
        {
          "id": "f083d4d9-b95e-4211-bf14-59fb118911d3",
          "name": "deletePlatformApplication",
          "request": {
            "url": "http://example.com/api/?Action=DeletePlatformApplication?PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a platform application object for one of the supported push notification services,\n      such as APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da0e0595-ce99-46a7-bb51-e6556f64b4a3"
            }
          ]
        },
        {
          "id": "0b0ef36a-45d5-4858-99c1-dd2588bd22b5",
          "name": "getPlatformApplicationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetPlatformApplicationAttributes?PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the attributes of the platform application object for the supported push\n      notification services, such as APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ab08e77-8ea1-49fd-b559-2d34d6bd1e62"
            }
          ]
        },
        {
          "id": "c655c959-568b-4779-9e96-3ca10d0fccfa",
          "name": "listPlatformApplications",
          "request": {
            "url": "http://example.com/api/?Action=ListPlatformApplications?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the platform application objects for the supported push notification services, such as\n      APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1231c2bf-1823-4349-bc10-4ebd7d8222f7"
            }
          ]
        },
        {
          "id": "ab40760a-009a-46ed-9817-8f04af8bb26c",
          "name": "setPlatformApplicationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=SetPlatformApplicationAttributes?Attributes\n            , Attributes.entry.N.key (key), Attributesentry.N.value (value)=Attributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20Attributes.entry.N.key%20%28key%29%2C%20Attributesentry.N.value%20%28value%29&PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the attributes of the platform application object for the supported push notification\n      services, such as APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf659f02-d1ce-4d08-9cef-a54ee32f4a25"
            }
          ]
        }
      ]
    },
    {
      "name": "Platform Endpoints",
      "item": [
        {
          "id": "42e739ae-f3a2-4b50-99a6-e122dbc8a65e",
          "name": "createPlatformEndpoint",
          "request": {
            "url": "http://example.com/api/?Action=CreatePlatformEndpoint?Attributes\n            , Attributes.entry.N.key (key), Attributesentry.N.value (value)=Attributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20Attributes.entry.N.key%20%28key%29%2C%20Attributesentry.N.value%20%28value%29&CustomUserData=CustomUserData&PlatformApplicationArn=PlatformApplicationArn&Token=Token",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an endpoint for a device and mobile app on one of the supported push notification\n      services, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1debf2b2-f8fd-426f-80c6-1cae02ffb732"
            }
          ]
        }
      ]
    },
    {
      "name": "Topics",
      "item": [
        {
          "id": "23225e71-7f3c-4512-891b-c2990a72e100",
          "name": "createTopic",
          "request": {
            "url": "http://example.com/api/?Action=CreateTopic?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a topic to which notifications can be published."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8961e2c-617c-47b1-a5fd-bd8595cab7d2"
            }
          ]
        },
        {
          "id": "c10e9dc8-7d02-4ef3-8a49-a646cedeb97e",
          "name": "deleteTopic",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTopic?TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a topic and all its subscriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a957921-1d4c-4db4-b172-82570bb49987"
            }
          ]
        },
        {
          "id": "13bf4d39-3486-4b45-ac17-63c24d24fbf6",
          "name": "getTopicAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetTopicAttributes?TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all of the properties of a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b4ba758-afb8-46fa-9094-4ecb38a6f723"
            }
          ]
        },
        {
          "id": "9f738a40-9a2b-4301-b0bb-eb0f417b0956",
          "name": "listTopics",
          "request": {
            "url": "http://example.com/api/?Action=ListTopics?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the requester's topics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ee09805-1042-4c0d-8592-8eaf9b29f861"
            }
          ]
        },
        {
          "id": "471640fe-b8aa-49f1-8aef-f6b27ae692aa",
          "name": "setTopicAttributes",
          "request": {
            "url": "http://example.com/api/?Action=SetTopicAttributes?AttributeName=AttributeName&AttributeValue=AttributeValue&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows a topic owner to set an attribute of the topic to a new value."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "afa2813a-f491-4c86-818a-438a46f4f9f8"
            }
          ]
        }
      ]
    },
    {
      "name": "Endpoints",
      "item": [
        {
          "id": "31aca0c0-2b6f-4df7-9813-ac579250036f",
          "name": "deleteEndpoint",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEndpoint?EndpointArn=EndpointArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the endpoint for a device and mobile app from Amazon SNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7925e197-6f04-4775-86dc-2f2fc3a980aa"
            }
          ]
        },
        {
          "id": "4c90c25f-2cf8-4797-abb6-bccd0760607c",
          "name": "getEndpointAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetEndpointAttributes?EndpointArn=EndpointArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the endpoint attributes for a device on one of the supported push notification\n      services, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b95f6001-d29b-462d-8c66-c6333a0371c0"
            }
          ]
        },
        {
          "id": "f0c2c5d2-7eee-4546-a65f-e582e579a060",
          "name": "listEndpointsByPlatformApplication",
          "request": {
            "url": "http://example.com/api/?Action=ListEndpointsByPlatformApplication?NextToken=NextToken&PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the endpoints and endpoint attributes for devices in a supported push notification\n      service, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f70bff05-a478-4a22-bf42-a7de5dbf34ef"
            }
          ]
        },
        {
          "id": "9b0873b4-f29b-413e-a918-33f50e6de6fe",
          "name": "setEndpointAttributes",
          "request": {
            "url": "http://example.com/api/?Action=SetEndpointAttributes?Attributes\n            , Attributes.entry.N.key (key), Attributesentry.N.value (value)=Attributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20Attributes.entry.N.key%20%28key%29%2C%20Attributesentry.N.value%20%28value%29&EndpointArn=EndpointArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the attributes for an endpoint for a device on one of the supported push notification\n      services, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3f18740-0ad5-427d-bb96-c38e20ea3235"
            }
          ]
        },
        {
          "id": "dadca940-5bfd-437a-8a7b-e7b75eb8dfc7",
          "name": "subscribe",
          "request": {
            "url": "http://example.com/api/?Action=Subscribe?Endpoint=Endpoint&Protocol=Protocol&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Prepares to subscribe an endpoint by sending the endpoint a confirmation message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6bc07f7c-fb0e-4bb4-ae39-2ff236dd0eaf"
            }
          ]
        }
      ]
    },
    {
      "name": "SMS",
      "item": [
        {
          "id": "b01bfaf5-4576-4da3-a175-63a9cc377677",
          "name": "getSMSAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetSMSAttributes?attributes.member.N=attributes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the settings for sending SMS messages from your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9eb29ce9-9ccb-4a95-b182-0691c10e5650"
            }
          ]
        },
        {
          "id": "3b363ebc-c944-4964-af50-950b51e58997",
          "name": "setSMSAttributes",
          "request": {
            "url": "http://example.com/api/?Action=SetSMSAttributes?attributes\n            , attributes.entry.N.key (key), attributesentry.N.value (value)=attributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20attributes.entry.N.key%20%28key%29%2C%20attributesentry.N.value%20%28value%29",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Use this request to set the default settings for sending SMS messages and receiving daily SMS usage reports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7bd8847a-b519-4a06-a62f-91422c2d4faf"
            }
          ]
        }
      ]
    },
    {
      "name": "Publish",
      "item": [
        {
          "id": "cd24b160-5451-4880-9474-bd51640a4e21",
          "name": "publish",
          "request": {
            "url": "http://example.com/api/?Action=Publish?Message=Message&MessageAttributes\n            , MessageAttributes.entry.N.Name (key), MessageAttributesentry.N.Value (value)=MessageAttributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20MessageAttributes.entry.N.Name%20%28key%29%2C%20MessageAttributesentry.N.Value%20%28value%29&MessageStructure=MessageStructure&PhoneNumber=PhoneNumber&Subject=Subject&TargetArn=TargetArn&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sends a message to all of a topic's subscribed endpoints."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c8fccdb-7086-4c3d-a3bd-65de50094c05"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "0b7dd449-519a-4cbc-9a22-788a93d0dfe9",
          "name": "unsubscribe",
          "request": {
            "url": "http://example.com/api/?Action=Unsubscribe?SubscriptionArn=SubscriptionArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a5af288-5ca6-4625-b8e6-3a8902c224bf"
            }
          ]
        }
      ]
    }
  ]
}