{
  "info": {
    "name": "GoToMeeting Historical meetings by group",
    "_postman_id": "ef3779e0-126c-4395-b877-45299bbd618e",
    "description": "Get historical meetings for the specified group that started within the specified date/time range. This API call is only available to users with the admin role. This API call is restricted to groups with a maximum of 50 organizers. Remark: Meetings which are still ongoing at the time of the request are NOT contained in the result array.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Historical",
      "item": [
        {
          "id": "5392f7cb-c0ae-4bfe-aba5-3b421091c0ee",
          "name": "HistoricalMeetingsGet",
          "request": {
            "url": "http://api.getgo.com/G2M/rest/historicalMeetings?endDate=%7B%7D&startDate=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get historical meetings for the currently authenticated organizer that started within the specified date/time range. Remark: Meetings which are still ongoing at the time of the request are NOT contained in the result array."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "887f6e01-0476-4726-bc9d-8a2f9fbea4f8"
            }
          ]
        },
        {
          "id": "ce0d3ae6-7674-4587-b778-3f970c1ba96a",
          "name": "OrganizersHistoricalMeetingsByOrganizerKeyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2M",
                "rest",
                "organizers/:organizerKey/historicalMeetings"
              ],
              "query": [
                {
                  "key": "endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startDate",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "organizerKey",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get historical meetings for the specified organizer that started within the specified date/time range. Meetings which are still ongoing at the time of the request are not included in the result."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d02c3e25-07e0-4cf3-9762-b560a7efd411"
            }
          ]
        },
        {
          "id": "b2dfb49f-0bc4-45f6-9aa5-09b4ae03eeb8",
          "name": "GroupsHistoricalMeetingsByGroupkeyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2M",
                "rest",
                "groups/:groupkey/historicalMeetings"
              ],
              "query": [
                {
                  "key": "endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startDate",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "groupkey",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get historical meetings for the specified group that started within the specified date/time range. This API call is only available to users with the admin role. This API call is restricted to groups with a maximum of 50 organizers. Remark: Meetings which are still ongoing at the time of the request are NOT contained in the result array."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bbd43a5a-5479-463a-b5c6-ac7353f26328"
            }
          ]
        }
      ]
    }
  ]
}