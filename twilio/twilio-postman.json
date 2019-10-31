{
  "info": {
    "name": "Twilio Add Account Usage Triggers",
    "_postman_id": "c31fc2e6-7fad-481c-85e6-3cc6cd98e852",
    "description": "Creates a new UsageTrigger. Each account can create up to 1,000 UsageTriggers.nCurrently, UsageTriggers that are no longer active are not deleted automatically.nUse DELETE to delete triggers you no longer need.n",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Accounts",
      "item": [
        {
          "id": "636aa9ba-1169-47df-b343-dc5737ee4c82",
          "name": "getAccount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61b23c56-a95e-47d3-bdab-ada7d4fc412a"
            }
          ]
        },
        {
          "id": "adf6727a-7a5c-4b05-a2e1-06febcd182f4",
          "name": "updateAccount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update Account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f2fea00-3d7a-4437-a7dd-a6ea61867421"
            }
          ]
        },
        {
          "id": "7458ed1f-0cc5-4692-88e6-08d268d0b014",
          "name": "addAccount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add Account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "efe90031-e2a7-4606-8252-3dd3a66448c7"
            }
          ]
        },
        {
          "id": "a15aaf20-851c-4626-8709-c8cff5b9b6bc",
          "name": "getAccounts",
          "request": {
            "url": "http://api.twilio.com/2010-04-01/Accounts.json?format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "720389f1-bf41-4195-aa23-664515707544"
            }
          ]
        }
      ]
    },
    {
      "name": "Applications",
      "item": [
        {
          "id": "034b230d-182a-4918-b1e3-3f1d7137e363",
          "name": "get-application-instance-resource",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Applications/:ApplicationSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "ApplicationSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get application instance resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ab7da8d-fef3-4046-b58f-56996fdc5ec3"
            }
          ]
        },
        {
          "id": "dcdc9e79-c722-464d-a389-23e94c022a0e",
          "name": "tries-to-update-the-applications-properties-and-returns-the-updatedresource-representation-if-succes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Applications/:ApplicationSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "ApplicationSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Tries to update the applications properties, and returns the updatednresource representation if successful. The returned response is identicalnto that returned above when making a GET request.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1fc91e5-643a-4676-85d5-ab73c61784df"
            }
          ]
        },
        {
          "id": "4cd1cc7f-f08c-4a77-b2c5-0ac99d4fb176",
          "name": "delete-this-application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Applications/:ApplicationSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "ApplicationSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete Application"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e4b05bd-569b-4fb1-8b48-c74b5f0a84c5"
            }
          ]
        },
        {
          "id": "940cffb1-34bc-4550-a635-6484acae817b",
          "name": "returns-a-list-of-application-resource-representations-each-representingan-application-within-your-a",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Applications.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Applications"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05d64464-68dd-483b-b72d-9d587db361db"
            }
          ]
        },
        {
          "id": "68863cc5-9ed9-44d5-be10-383af85ee639",
          "name": "creates-a-new-application-within-your-account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Applications.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add Applications"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4ae7264-2cd8-486b-9dca-79b0900e3497"
            }
          ]
        },
        {
          "id": "c1c86ed8-194c-45a6-b0eb-536eea7712ad",
          "name": "get-the-properties-of-the-authorized-application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/AuthorizedConnectApps/:ConnectAppSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "ConnectAppSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the properties of the authorized application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37cfc5d9-fee0-40e8-b55f-89a9f33b4251"
            }
          ]
        },
        {
          "id": "3bf3c8d6-6a56-4800-94b2-7d6bb378bab3",
          "name": "returns-a-list-of-connect-app-resource-representations-each-representing-aconnect-app-youve-authoriz",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/AuthorizedConnectApps.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of Connect App resource representations, each representing anConnect App youve authorized to access your account. The list includesnpaging information.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "edff89aa-89a6-49b6-aa83-03f0a3e39a15"
            }
          ]
        },
        {
          "id": "45e80fa1-06a4-4739-8ce5-1cc2b90a6905",
          "name": "get-the-properties-of-a-connect-app",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/ConnectApps/:ConnectAppSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "ConnectAppSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the properties of a Connect App."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0cc69cbf-bfdc-4f7b-94bd-afe969a2eb1d"
            }
          ]
        },
        {
          "id": "ba32925b-0226-4116-9a99-515d9fb1c945",
          "name": "tries-to-update-the-connect-apps-properties-and-returns-the-updatedresource-representation-if-succes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/ConnectApps/:ConnectAppSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "ConnectAppSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Tries to update the Connect Apps properties, and returns the updatednresource representation if successful. The returned response is identicalnto that returned above when making a GET request.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39afa05a-3aa6-46d3-b5a3-a997e71bc15c"
            }
          ]
        },
        {
          "id": "94f6ff65-f978-41a2-8fdd-7bc2859ecd8c",
          "name": "returns-a-list-of-connect-app-resource-representations-each-representinga-connect-app-in-your-accoun",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/ConnectApps.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of Connect App resource representations, each representingna Connect App in your account. The list includes paging information.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a878f8c1-d810-4f20-a508-06784e502abb"
            }
          ]
        }
      ]
    },
    {
      "name": "Phone Numbers",
      "item": [
        {
          "id": "a01b0c4f-8dda-4600-86bb-cba41677a1c7",
          "name": "returns-a-list-of-local-availablephonenumber-resource-representationsthat-match-the-specified-filter",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/AvailablePhoneNumbers/:IsoCountryCode/Local.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "IsoCountryCode",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of local AvailablePhoneNumber resource representationsnthat match the specified filters, each representing a phone number thanis currently available for provisioning within your account.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93f98734-f2c1-4529-95c8-5ed15d91d875"
            }
          ]
        },
        {
          "id": "3baa4658-327a-4b26-969b-61da6bde7253",
          "name": "returns-a-list-of-mobile-availablephonenumber-resource-representations-that-match-the-specified-filt",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/AvailablePhoneNumbers/:IsoCountryCode/Mobile.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "IsoCountryCode",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of mobile AvailablePhoneNumber resource representations that match the specified filters, each representing a phone number that is currently available for provisioning within your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24930b52-d6da-4fea-ab66-01769f4586ab"
            }
          ]
        },
        {
          "id": "5559f8a3-d28d-4d83-aeab-7560b68fafe0",
          "name": "returns-a-list-of-tollfree-availablephonenumber-elements-that-match-thespecified-filters-each-repres",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/AvailablePhoneNumbers/:IsoCountryCode/TollFree.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "IsoCountryCode",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of toll-free AvailablePhoneNumber elements that match thenspecified filters, each representing a phone number that is currentlynavailable for provisioning within your account. To provision an availablenphone number, POST the number to the IncomingPhoneNumbers resource.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b113345-8b2a-4cec-aa65-417f60b597eb"
            }
          ]
        }
      ]
    },
    {
      "name": "Recordings",
      "item": [
        {
          "id": "1ed89a47-635e-45dc-afd7-ffa73bb49a39",
          "name": "returns-a-list-of-recording-resource-representations-each-representing-arecording-generated-during-t",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Calls/:CallSid/Recordings.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "CallSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of Recording resource representations, each representing anrecording generated during the course of a phone call.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6fef6f2c-ef62-4813-bc47-5cca810a342b"
            }
          ]
        },
        {
          "id": "94178082-bd9b-4b67-a1b8-f22ed4dca54e",
          "name": "returns-a-set-of-transcription-resource-representations-that-includes-paginginformation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Recordings/:RecordingSid/Transcriptions"
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "RecordingSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a set of Transcription resource representations that includes pagingninformation.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e508b0b8-7bf9-43ee-bd37-ccc11d1b5953"
            }
          ]
        },
        {
          "id": "32fe1f01-00dc-443c-88af-fb54e60910ae",
          "name": "returns-one-of-several-representationswithout-an-extension-or-with-a-wav-a-binary-wav-audio-file-is-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Recordings/:RecordingSid"
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "RecordingSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns one of several representations:nWithout an extension, or with a .wav, a binary WAV audio file is returnednwith mime-type audio/x-wav.nAppending .mp3 to the URI returns a binary MP3 audio file with mime-typentype audio/mpeg.nAppending .xml to the URI returns a XML representation.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bcfc91d9-2e23-4b00-902b-ad3fffa9bf29"
            }
          ]
        },
        {
          "id": "2c8a3711-386c-409d-9fa1-7c996b5ab96f",
          "name": "deletes-a-recording--from-your-account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Recordings/:RecordingSid"
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "RecordingSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a recording  from your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9b185ed-6f47-4c71-ba6c-b42f45a8573d"
            }
          ]
        },
        {
          "id": "71488905-123d-4a1e-aefc-74e5a337ea79",
          "name": "returns-a-list-of-recording-resource-representations-each-representing-arecording-generated-during-t",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Recordings"
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of Recording resource representations, each representing anrecording generated during the course of a phone call.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f0e60c5-dd71-4d6f-8cad-f3118c67dde2"
            }
          ]
        }
      ]
    },
    {
      "name": "Calls",
      "item": [
        {
          "id": "1087daed-9d20-4cbf-b4bc-aeb02cee5cf7",
          "name": "getCall",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Calls/:CallSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "CallSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Call"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04aa0667-774e-4073-aee3-60562659c0ed"
            }
          ]
        },
        {
          "id": "7d4d5d94-6dec-4cd5-920b-9d4dc3c4fd36",
          "name": "getCalls",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Calls.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Calls"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80e06158-e6fb-4eab-9492-fe0f144139e6"
            }
          ]
        },
        {
          "id": "964480c1-9469-4a3a-8251-2357537d2fd8",
          "name": "to-make-a-call-make-an-http-post-request-initiate-a-new-phone-call",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Calls.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "To make a call, make an HTTP POST request. Initiate a new phone call."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52d46d81-3652-4f6e-87e0-a06357135dd2"
            }
          ]
        }
      ]
    },
    {
      "name": "Conferences",
      "item": [
        {
          "id": "a9c19c8c-d532-4a1c-a2df-cf9c0664edad",
          "name": "getparticipantforconference",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Conferences/:ConferenceSid/Participants/:CallSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "CallSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "ConferenceSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "GetParticipantForConference"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0cda18c-689f-4781-a59b-f34088f78c0c"
            }
          ]
        },
        {
          "id": "f9f10905-9cab-40cf-9b63-2ea673994690",
          "name": "getConference",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Conferences/:ConferenceSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "ConferenceSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Conference"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23fd090e-ded1-493e-ae30-82b7e64daa72"
            }
          ]
        }
      ]
    },
    {
      "name": "Conference Calls",
      "item": [
        {
          "id": "a150f580-9eb7-4253-b967-bede3a19b077",
          "name": "updates-the-status-of-a-participant",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Conferences/:ConferenceSid/Participants/:CallSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "CallSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "ConferenceSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the status of a participant."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb0f4897-bfc6-4557-905c-62019c5d3d64"
            }
          ]
        },
        {
          "id": "92dada86-70ef-448b-81d1-c8a377634220",
          "name": "kick-this-participant-from-the-conference",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Conferences/:ConferenceSid/Participants/:CallSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "CallSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "ConferenceSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Kick this participant from the conference."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d70ede14-925a-4a40-a832-fb9deda113a5"
            }
          ]
        },
        {
          "id": "b2777a31-8387-4e06-b9d8-6988b9eb59ab",
          "name": "returns-the-list-of-participants-in-the-conference-identified-byconferencesid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Conferences/:ConferenceSid/Participants.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "ConferenceSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of participants in the conference identified byn{ConferenceSid}.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40da324e-34c3-4789-ba62-296db8ffbe7b"
            }
          ]
        },
        {
          "id": "f3069299-cf34-432b-bf2f-e1031c60beb3",
          "name": "returns-a-list-of-conferences-within-an-account-the-list-includes-paginginformation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Conferences.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of conferences within an account. The list includes pagingninformation.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "679758c2-f71b-4f76-9519-b6625dd34ba0"
            }
          ]
        }
      ]
    },
    {
      "name": "Incoming Phone Numbers",
      "item": [
        {
          "id": "35b76130-0ba7-44b6-9c6e-a151c4f7b944",
          "name": "returns-a-list-of-local-incomingphonenumber-elements-each-representing-a-local-not-tollfree-phone-nu",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/IncomingPhoneNumbers/Local.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of local <IncomingPhoneNumber> elements, each representing a local (not toll-free) phone number given to your account, under an <IncomingPhoneNumbers> list element that includes paging information. Works exactly the same as the IncomingPhoneNumber resource, but filters out toll-free numbers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9516e98-38cc-41eb-8226-8e37755123c8"
            }
          ]
        },
        {
          "id": "a9ed5bdd-661d-4147-b3b2-b4abd5629237",
          "name": "adds-a-new-phone-number-to-your-account-if-a-phone-number-is-found-for-your-request-twilio-will-add-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/IncomingPhoneNumbers/Local.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new phone number to your account. If a phone number is found for your request, Twilio will add it to your account and bill you for the first months cost of the phone number."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff4c2b91-589e-4cc8-8591-7a81a94a5028"
            }
          ]
        },
        {
          "id": "f0205f2a-75d4-4766-8397-98f9ea92674a",
          "name": "returns-a-list-of-local-incomingphonenumber-elements-each-representing-a-mobile-phone-number-given-t",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/IncomingPhoneNumbers/Mobile.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of local <IncomingPhoneNumber> elements, each representing a mobile phone number given to your account, under an <IncomingPhoneNumbers> list element that includes paging information. Works exactly the same as the IncomingPhoneNumber resource, but filters out local and toll free numbers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a84b4aed-3895-49c4-a1ac-8ed86fc834fd"
            }
          ]
        },
        {
          "id": "a359326e-8e41-44bb-b16e-e647d9bd86d3",
          "name": "get-info-about-incoming-calls-phone-number",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/IncomingPhoneNumbers/:IncomingPhoneNumberSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "IncomingPhoneNumberSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get info about incoming calls phone number."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3d3ccb2-2d76-4d6b-8d4a-f426c46b49cf"
            }
          ]
        },
        {
          "id": "3c2f445f-3dbc-49a4-b9f2-f8ef21a8dc7c",
          "name": "tries-to-update-the-incoming-phone-numbers-properties-and-returns-theupdated-resource-representation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/IncomingPhoneNumbers/:IncomingPhoneNumberSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "IncomingPhoneNumberSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Tries to update the incoming phone numbers properties, and returns thenupdated resource representation if successful. The returned response isnidentical to that returned above when making a GET request.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e35f4f77-295c-42d9-85c1-d2bb93b7589c"
            }
          ]
        },
        {
          "id": "920ea2c4-e5a8-4bea-ae0a-de84380b6f28",
          "name": "tries-to-update-the-incoming-phone-numbers-properties-and-returns-theupdated-resource-representation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/IncomingPhoneNumbers/:IncomingPhoneNumberSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "IncomingPhoneNumberSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Tries to update the incoming phone numbers properties, and returns thenupdated resource representation if successful. The returned response isnidentical to that returned above when making a GET request.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90a756ab-63c4-4ca7-81da-6414ff6b4692"
            }
          ]
        },
        {
          "id": "ee3aba97-485d-4e91-bb90-cc6aa1d06680",
          "name": "release-this-phone-number-from-your-account-twilio-will-no-longer-answercalls-to-this-number-and-you",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/IncomingPhoneNumbers/:IncomingPhoneNumberSid.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "IncomingPhoneNumberSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Release this phone number from your account. Twilio will no longer answerncalls to this number, and you will stop being billed the monthly phonennumber fee. The phone number will eventually be recycled and potentiallyngiven to another customer, so use with care. If you make a mistake, contacnus. We may be able to give you the number back.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c5db091-84cb-42c1-95d5-d20192be28d1"
            }
          ]
        }
      ]
    },
    {
      "name": "Messages",
      "item": [
        {
          "id": "c948d8d8-3fd6-46c6-ae33-bd18a1e1be32",
          "name": "without-an-extension-the-media-is-returned-using-the-mimetype-provided-when-the-media-was-generated",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Messages/:MessageSid/Media/:MediaSid"
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "MediaSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "MessageSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Without an extension, the media is returned using the mime-type provided when the media was generated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11c22b98-9376-4128-88c9-760953b0e980"
            }
          ]
        },
        {
          "id": "873d2f4f-9d62-40db-b455-3d45569c5b1a",
          "name": "returns-a-list-of-media-associated-with-your-message",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Messages/:MessageSid/Media"
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "MessageSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of media associated with your message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74fa4175-81c1-4c6d-ab9f-a94b5a6da0cb"
            }
          ]
        },
        {
          "id": "8ac1476c-f524-430e-8dee-f8f5163bf123",
          "name": "returns-a-single-message-specified-by-the-provided-messagesid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Messages/:MessageSid"
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "MessageSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a single message specified by the provided {MessageSid}.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea7711b5-1048-46bd-8568-b84b32df210b"
            }
          ]
        },
        {
          "id": "1dcf5cdf-cab4-4559-89d7-56985266f723",
          "name": "returns-a-list-of-messages-associated-with-your-account-the-list-includes-paging-information",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Messages.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of messages associated with your account. The list includes paging information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c23d84cc-44d3-4c9f-949e-f126d5aa703f"
            }
          ]
        },
        {
          "id": "96fe5536-fd45-4c54-b5d1-b62c9cd3c5fa",
          "name": "to-send-a-new-outgoing-message-make-an-http-post-to-your-messages-list-resource-uri",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Messages.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "format",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "To send a new outgoing message, make an HTTP POST to your Messages list resource URI"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a94299aa-5f5c-459f-a356-64e476427e3b"
            }
          ]
        }
      ]
    },
    {
      "name": "Outgoing Caller IDs",
      "item": [
        {
          "id": "e89838b4-492e-46e3-b23a-8c2d0f167c93",
          "name": "get-the-set-of-an-accounts-verified-phone-numbers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/OutgoingCallerIds/:OutgoingCallerIdSid"
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "OutgoingCallerIdSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the set of an accounts verified phone numbers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12212d9c-4b83-4c48-a1b7-d6ed1797606c"
            }
          ]
        },
        {
          "id": "2c1004dd-f810-44db-9fb3-83d026417bc7",
          "name": "updates-the-caller-id-and-returns-the-updated-resource-if-successful",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/OutgoingCallerIds/:OutgoingCallerIdSid"
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "OutgoingCallerIdSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the caller id, and returns the updated resource if successful."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34594601-d1f6-4a47-80e9-016a69f1cbb7"
            }
          ]
        },
        {
          "id": "522f671a-10ce-4d13-899c-b30d3d122ccd",
          "name": "updates-the-caller-id-and-returns-the-updated-resource-if-successful",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/OutgoingCallerIds/:OutgoingCallerIdSid"
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "OutgoingCallerIdSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the caller id, and returns the updated resource if successful."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "461b37ae-dedb-4565-99eb-c26afbc7dd8e"
            }
          ]
        },
        {
          "id": "489ef0e5-749e-47b7-aa4d-9f133b4e3818",
          "name": "deleteoutgoingcallerid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/OutgoingCallerIds/:OutgoingCallerIdSid"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "OutgoingCallerIdSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "DeleteOutgoingCallerId"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e2354c8-72fe-41e7-a59e-a23b826bdd6b"
            }
          ]
        },
        {
          "id": "17e5b0cd-e70c-4af0-8649-c109dbf6e1f5",
          "name": "returns-a-list-of-outgoingcallerid-resource-representations-each-represent