{
  "info": {
    "name": "Instructure Canvas Calendar Events API Reserve a time slot",
    "_postman_id": "0da860ba-c64e-494e-b200-fa066c0d8df6",
    "description": "Reserve a time slot.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calendar",
      "item": [
        {
          "id": "ed606ac5-9c10-4bc0-a354-d46645d2d6d5",
          "name": "list-calendar-events",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/calendar_events?all_events=%7B%7D&context_codes=%5B%7B%7D%5D&end_date=%7B%7D&excludes=%5B%7B%7D%5D&start_date=%7B%7D&type=%7B%7D&undated=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List calendar events."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90ae4873-132b-437a-992b-6adf74d0cbaa"
            }
          ]
        },
        {
          "id": "2cdb802d-fe58-4428-ab2e-82f7a88a2298",
          "name": "create-a-calendar-event",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/calendar_events?calendar_event[child_event_data][X][context_code]=%7B%7D&calendar_event[child_event_data][X][end_at]=%7B%7D&calendar_event[child_event_data][X][start_at]=%7B%7D&calendar_event[context_code]=%7B%7D&calendar_event[description]=%7B%7D&calendar_event[duplicate][append_iterator]=%7B%7D&calendar_event[duplicate][count]=%7B%7D&calendar_event[duplicate][frequency]=%7B%7D&calendar_event[duplicate][interval]=%7B%7D&calendar_event[end_at]=%7B%7D&calendar_event[location_address]=%7B%7D&calendar_event[location_name]=%7B%7D&calendar_event[start_at]=%7B%7D&calendar_event[time_zone_edited]=%7B%7D&calendar_event[title]=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a calendar event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4750fd90-e7f1-42c2-8c15-8c110ef7be3d"
            }
          ]
        },
        {
          "id": "b99489b0-781c-4473-90f2-ce6e75727b53",
          "name": "get-a-single-calendar-event-or-assignment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "calendar_events/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single calendar event or assignment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "440321c5-3693-4185-9544-87cc2f5e58e5"
            }
          ]
        },
        {
          "id": "9cc4bf57-e4a0-4737-8d5c-44672262902e",
          "name": "update-a-calendar-event",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "calendar_events/:id"
              ],
              "query": [
                {
                  "key": "calendar_event[child_event_data][X][context_code]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[child_event_data][X][end_at]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[child_event_data][X][start_at]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[context_code]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[description]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[end_at]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[location_address]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[location_name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[start_at]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[time_zone_edited]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[title]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a calendar event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec01fd8a-12f7-4048-a983-2102ba55f965"
            }
          ]
        },
        {
          "id": "4407cc8c-79ef-406f-acf3-9926ed1fef39",
          "name": "delete-a-calendar-event",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "calendar_events/:id"
              ],
              "query": [
                {
                  "key": "cancel_reason",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a calendar event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70b4b35a-4eae-4454-83d7-ec3f0e71dd90"
            }
          ]
        },
        {
          "id": "1d73e590-dfa1-41ff-9f1b-3a61450d9a44",
          "name": "reserve-a-time-slot",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "calendar_events/:id/reservations"
              ],
              "query": [
                {
                  "key": "cancel_existing",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "comments",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "participant_id",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Reserve a time slot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aae9d041-0a7f-48f2-9dad-3c2693e51468"
            }
          ]
        },
        {
          "id": "54eb5590-91a2-4852-927e-e0a80775b235",
          "name": "reserve-a-time-slot1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "calendar_events/:id/reservations/participant_id"
              ],
              "query": [
                {
                  "key": "cancel_existing",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "comments",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "participant_id",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Reserve a time slot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8174501-d4ba-4b01-a90d-8920ebc093b5"
            }
          ]
        }
      ]
    }
  ]
}