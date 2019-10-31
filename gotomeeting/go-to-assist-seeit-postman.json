{
  "info": {
    "name": "Go To Assist Seeit Get details for a single GoToAssist Seeit session",
    "_postman_id": "d7ae9ff1-7cff-4725-847e-6b60d2ce2f56",
    "description": "<p>This endpoint allows you to get all relevant details for a single GoToAssist Seeit session. Session details are available for 90 days.</p><p>The fields and their values in the response depend on session status and the time elapsed since session end; e.g. session data like snapshots or the session recording are only available for 72 hours.</p>",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sessions",
      "item": [
        {
          "id": "b0c09575-6503-4c2a-8f52-629e4efcec24",
          "name": "sessions.get",
          "request": {
            "url": "http://api.citrixonline.com/seeit/v1/sessions?endTime=%7B%7D&No Name=%7B%7D&page=%7B%7D&size=%7B%7D&sort=%7B%7D&startTime=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "<p>This endpoint allows you to get all relevant details for mulitple GoToAssist Seeit sessions. Session details are available for 90 days.</p></p>The fields and their values in the response depend on session status and the time elapsed since session end; e.g. session data like snapshots or the session recording are only available for 72 hours.</p><p>The results will be paged, with paging customizable to match your requirements.</p>"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f714d6e-3b5d-4ca2-bb2c-c84252d8e809"
            }
          ]
        },
        {
          "id": "7e84acd7-25ff-497f-8688-15fc21f1dbc5",
          "name": "sessions.post",
          "request": {
            "url": "http://api.citrixonline.com/seeit/v1/sessions?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint allows you to create a GoToAssist Seeit session. The session logically exists but is not started until you open the returned startUrl in a suitable browser."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a579d343-2a37-45e7-81f0-b32c0ce54c1b"
            }
          ]
        },
        {
          "id": "94e28613-6930-433e-a7c3-54f6e2c268bf",
          "name": "sessions.uuid.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.citrixonline.com",
              "path": [
                "seeit",
                "v1",
                "sessions/:uuid"
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
                  "id": "uuid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "<p>This endpoint allows you to get all relevant details for a single GoToAssist Seeit session. Session details are available for 90 days.</p><p>The fields and their values in the response depend on session status and the time elapsed since session end; e.g. session data like snapshots or the session recording are only available for 72 hours.</p>"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ce17cdc-0047-4622-8ce4-e38a3272cbd2"
            }
          ]
        }
      ]
    }
  ]
}