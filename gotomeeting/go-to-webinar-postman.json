{
  "info": {
    "name": "Go To Webinar Get session surveys",
    "_postman_id": "957d57fc-5127-4180-9ad1-701cfc932883",
    "description": "Retrieve surveys for a past webinar session. For technical reasons, this call cannot be executed from this documentation. Please use the curl command to execute it.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizers",
      "item": [
        {
          "id": "fdab15ab-7471-4d0d-9e1f-14f97183a170",
          "name": "getOrganizerSessions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.citrixonline.com",
              "path": [
                "G2W",
                "rest",
                "organizers/:organizerKey/sessions"
              ],
              "query": [
                {
                  "key": "fromTime",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "toTime",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "organizerKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve all completed sessions of all the webinars of a given organizer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d00e1a8-4459-44b0-a4b0-cc7b67f088e2"
            }
          ]
        },
        {
          "id": "6e007154-c955-4a03-b104-02ce88657e39",
          "name": "getAllSessions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.citrixonline.com",
              "path": [
                "G2W",
                "rest",
                "organizers/:organizerKey/webinars/:webinarKey/sessions"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "organizerKey",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "webinarKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves details for all past sessions of a specific webinar."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63a96181-78f1-4592-abf4-9a971de45ae0"
            }
          ]
        },
        {
          "id": "df630183-357d-4e18-b55c-dbcd84521a6e",
          "name": "getWebinarSession",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.citrixonline.com",
              "path": [
                "G2W",
                "rest",
                "organizers/:organizerKey/webinars/:webinarKey/sessions/:sessionKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "organizerKey",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "webinarKey",
                  "type": "string"
                },
                {
                  "id": "sessionKey",
                  "value": "sessionKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves attendance details for a specific webinar session that has ended. If attendees attended the session ('registrantsAttended'), specific attendance details, such as attendenceTime for a registrant, will also be retrieved. For technical reasons, this call cannot be executed from this documentation. Please use the curl command to execute it."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "239c6435-a04e-4b0b-b1c4-9a1ff7cb486b"
            }
          ]
        },
        {
          "id": "1bab7666-d689-4b03-9b64-9547700a09f0",
          "name": "getAttendees",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.citrixonline.com",
              "path": [
                "G2W",
                "rest",
                "organizers/:organizerKey/webinars/:webinarKey/sessions/:sessionKey/attendees"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "organizerKey",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "webinarKey",
                  "type": "string"
                },
                {
                  "id": "sessionKey",
                  "value": "sessionKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve details for all attendees of a specific webinar session. For technical reasons, this call cannot be executed from this documentation. Please use the curl command to execute it."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12203a8c-d634-4932-8ccf-4036d77d86b1"
            }
          ]
        },
        {
          "id": "b8f3b00d-d6a6-4926-b813-56f0ea07d755",
          "name": "getAttendee",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.citrixonline.com",
              "path": [
                "G2W",
                "rest",
                "organizers/:organizerKey/webinars/:webinarKey/sessions/:sessionKey/attendees/:registrantKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "organizerKey",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "webinarKey",
                  "type": "string"
                },
                {
                  "id": "sessionKey",
                  "value": "sessionKey",
                  "type": "string"
                },
                {
                  "id": "registrantKey",
                  "value": "registrantKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve registration details for a particular attendee of a specific webinar session. For technical reasons, this call cannot be executed from this documentation. Please use the curl command to execute it."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76c9361f-e38a-4a63-8e97-d38f666c926b"
            }
          ]
        },
        {
          "id": "8c377d67-b8af-4638-80c2-c14ebaad486f",
          "name": "getAttendeePollAnswers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.citrixonline.com",
              "path": [
                "G2W",
                "rest",
                "organizers/:organizerKey/webinars/:webinarKey/sessions/:sessionKey/attendees/:registrantKey/polls"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "organizerKey",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "webinarKey",
                  "type": "string"
                },
                {
                  "id": "sessionKey",
                  "value": "sessionKey",
                  "type": "string"
                },
                {
                  "id": "registrantKey",
                  "value": "registrantKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get poll answers from a particular attendee of a specific webinar session. For technical reasons, this call cannot be executed from this documentation. Please use the curl command to execute it."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb537d5e-2d74-4a6b-8adf-7d4efb6853da"
            }
          ]
        },
        {
          "id": "e8a9375b-235c-4989-99f0-f11ca376358e",
          "name": "getAttendeeQuestions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.citrixonline.com",
              "path": [
                "G2W",
                "rest",
                "organizers/:organizerKey/webinars/:webinarKey/sessions/:sessionKey/attendees/:registrantKey/questions"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "organizerKey",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "webinarKey",
                  "type": "string"
                },
                {
                  "id": "sessionKey",
                  "value": "sessionKey",
                  "type": "string"
                },
                {
                  "id": "registrantKey",
                  "value": "registrantKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get questions asked by an attendee during a webinar session. For technical reasons, this call cannot be executed from this documentation. Please use the curl command to execute it."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e1fee44-dfd4-4158-94f8-87f856f8b9b7"
            }
          ]
        },
        {
          "id": "308263cd-2dab-4b9e-82fc-73ac2e2b2bdc",
          "name": "getAttendeeSurveyAnswers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.citrixonline.com",
              "path": [
                "G2W",
                "rest",
                "organizers/:organizerKey/webinars/:webinarKey/sessions/:sessionKey/attendees/:registrantKey/surveys"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "organizerKey",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "webinarKey",
                  "type": "string"
                },
                {
                  "id": "sessionKey",
                  "value": "sessionKey",
                  "type": "string"
                },
                {
                  "id": "registrantKey",
                  "value": "registrantKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve survey answers from a particular attendee during a webinar session. For technical reasons, this call cannot be executed from this documentation. Please use the curl command to execute it."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5994864-da75-46bf-bd60-c1caa5d359ca"
            }
          ]
        },
        {
          "id": "cfe1a469-74ba-46da-9071-2d82fcc5d9f0",
          "name": "getPerformance",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.citrixonline.com",
              "path": [
                "G2W",
                "rest",
                "organizers/:organizerKey/webinars/:webinarKey/sessions/:sessionKey/performance"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "organizerKey",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "webinarKey",
                  "type": "string"
                },
                {
                  "id": "sessionKey",
                  "value": "sessionKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get performance details for a session. For technical reasons, this call cannot be executed from this documentation. Please use the curl command to execute it."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d500ec4-88fb-4dfd-8eec-eee01f41e872"
            }
          ]
        },
        {
          "id": "02fddebd-0932-41d3-a75c-763414c063ff",
          "name": "getPolls",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.citrixonline.com",
              "path": [
                "G2W",
                "rest",
                "organizers/:organizerKey/webinars/:webinarKey/sessions/:sessionKey/polls"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "organizerKey",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "webinarKey",
                  "type": "string"
                },
                {
                  "id": "sessionKey",
                  "value": "sessionKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve all collated attendee questions and answers for polls from a specific webinar session. For technical reasons, this call cannot be executed from this documentation. Please use the curl command to execute it."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6938719-61dc-4b97-93a2-4da32b83a12d"
            }
          ]
        },
        {
          "id": "6feadeac-dfd5-43e5-b460-d241a6e7ebb2",
          "name": "getQuestions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.citrixonline.com",
              "path": [
                "G2W",
                "rest",
                "organizers/:organizerKey/webinars/:webinarKey/sessions/:sessionKey/questions"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "organizerKey",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "webinarKey",
                  "type": "string"
                },
                {
                  "id": "sessionKey",
                  "value": "sessionKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve questions and answers for a past webinar session. For technical reasons, this call cannot be executed from this documentation. Please use the curl command to execute it."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eafc3390-4e69-4e6b-9212-bf8ba076e049"
            }
          ]
        },
        {
          "id": "5742cfdc-21ef-4cc1-91db-ac9e1cebe342",
          "name": "getSurveys",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.citrixonline.com",
              "path": [
                "G2W",
                "rest",
                "organizers/:organizerKey/webinars/:webinarKey/sessions/:sessionKey/surveys"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "organizerKey",
                  "type": "string"
                },
                {
                  "id": "webinarKey",
                  "value": "webinarKey",
                  "type": "string"
                },
                {
                  "id": "sessionKey",
                  "value": "sessionKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve surveys for a past webinar session. For technical reasons, this call cannot be executed from this documentation. Please use the curl command to execute it."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a8a6910-5783-4b20-ac01-4731aafc1207"
            }
          ]
        }
      ]
    }
  ]
}