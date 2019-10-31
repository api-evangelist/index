{
  "info": {
    "name": "AWS Security Token Service API Get Session Token",
    "_postman_id": "9433bf1f-cfaf-4f1c-89cd-2f54aa18310c",
    "description": "Returns a set of temporary credentials for an AWS account or IAM user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Roles",
      "item": [
        {
          "id": "e8c5271f-17d1-42e7-922b-4fe0ea865510",
          "name": "assumeRole",
          "request": {
            "url": "http://example.com/api/?Action=AssumeRole?DurationSeconds=DurationSeconds&ExternalId=ExternalId&Policy=Policy&RoleArn=RoleArn&RoleSessionName=RoleSessionName&SerialNumber=SerialNumber&TokenCode=TokenCode",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a set of temporary security credentials (consisting of an access key ID, a\n      secret access key, and a security token) that you can use to access AWS resources that you\n      might not normally have access to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7bf5b8a9-5c71-4ae6-894b-6d46b5097e65"
            }
          ]
        },
        {
          "id": "3cc167db-a4f2-4b52-b042-c83864c3a86e",
          "name": "assumeRoleWithSAML",
          "request": {
            "url": "http://example.com/api/?Action=AssumeRoleWithSAML?DurationSeconds=DurationSeconds&Policy=Policy&PrincipalArn=PrincipalArn&RoleArn=RoleArn&SAMLAssertion=SAMLAssertion",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a set of temporary security credentials for users who have been authenticated\n      via a SAML authentication response."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5fda6d31-e821-4a5d-98bd-0ed2178a1472"
            }
          ]
        },
        {
          "id": "5537e115-1f63-4bbe-847a-7b9af409ff72",
          "name": "assumeRoleWithWebIdentity",
          "request": {
            "url": "http://example.com/api/?Action=AssumeRoleWithWebIdentity?DurationSeconds=DurationSeconds&Policy=Policy&ProviderId=ProviderId&RoleArn=RoleArn&RoleSessionName=RoleSessionName&WebIdentityToken=WebIdentityToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a set of temporary security credentials for users who have been authenticated\n      in a mobile or web application with a web identity provider, such as Amazon Cognito, Login with Amazon,\n      Facebook, Google, or any OpenID Connect-compatible identity provider."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3da9dc5-36ec-4325-9e97-0ee42d1477b9"
            }
          ]
        },
        {
          "id": "17e9e69e-1bf1-4d33-8697-16a2bf653c72",
          "name": "decodeAuthorizationMessage",
          "request": {
            "url": "http://example.com/api/?Action=DecodeAuthorizationMessage?EncodedMessage=EncodedMessage",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Decodes additional information about the authorization status of a request from an\n      encoded message returned in response to an AWS request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe904637-ae3f-44a0-9fc5-4f4655bf1d8a"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity",
      "item": [
        {
          "id": "ef4002d7-92b2-4dea-9f62-54480fb4e29b",
          "name": "getCallerIdentity",
          "request": {
            "url": "http://example.com/api/?Action=GetCallerIdentity?Account=Account&Arn=Arn&UserId=UserId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns details about the IAM identity whose credentials are used to call the\n      API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2620f96-348d-43bb-a367-f76b5e876336"
            }
          ]
        }
      ]
    },
    {
      "name": "Federation Token",
      "item": [
        {
          "id": "2c6dc8f7-b711-4fb4-91d0-5997b7b5e34b",
          "name": "getFederationToken",
          "request": {
            "url": "http://example.com/api/?Action=GetFederationToken?DurationSeconds=DurationSeconds&Name=Name&Policy=Policy",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a set of temporary security credentials (consisting of an access key ID, a\n      secret access key, and a security token) for a federated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6fe12e79-2662-4971-8d60-79997a14f7fb"
            }
          ]
        }
      ]
    },
    {
      "name": "Session Token",
      "item": [
        {
          "id": "72cf164c-d00d-4290-ab92-b1fdfea0b7fd",
          "name": "getSessionToken",
          "request": {
            "url": "http://example.com/api/?Action=GetSessionToken?DurationSeconds=DurationSeconds&SerialNumber=SerialNumber&TokenCode=TokenCode",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a set of temporary credentials for an AWS account or IAM user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d2ecce1-0a06-4cea-910e-a2dcaf63a4a2"
            }
          ]
        }
      ]
    }
  ]
}