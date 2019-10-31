{
  "info": {
    "name": "Plivo SMS Message",
    "_postman_id": "bc2579de-5e1b-4591-b569-dd4fb6ec0983",
    "description": "Get details of a single message.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Message",
      "item": [
        {
          "id": "634cf3b6-25d0-4f00-9714-0c10a2d94f3b",
          "name": "getAuthMessage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.plivo.com",
              "path": [
                "v1",
                ":auth_id/Message/"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "auth_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get details of a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cca1c941-5b1e-4f07-b5ee-f4276e523471"
            }
          ]
        },
        {
          "id": "b75b81b8-cc3f-4a24-b984-2c8832577382",
          "name": "getAuthMessageMessageUu",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.plivo.com",
              "path": [
                "v1",
                ":auth_id/Message/:message_uuid/"
              ],
              "variable": [
                {
                  "id": "auth_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "message_uuid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get details of a single message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70403233-44e2-4a78-8717-4d5b89b2ffe6"
            }
          ]
        }
      ]
    },
    {
      "name": "Send",
      "item": [
        {
          "id": "3e4ec3fc-7734-4eae-a41b-dab6e72deee0",
          "name": "postAuthMessage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.plivo.com",
              "path": [
                "v1",
                ":auth_id/Message/"
              ],
              "query": [
                {
                  "key": "dst",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "log",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "method",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "src",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "text",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "This API enables you to send messages via Plivou2019s SMS service.",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "auth_id",
                  "value": "auth_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "This API enables you to send messages via Plivou2019s SMS service."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa027dcc-91f9-4859-97eb-6c2f3decd329"
            }
          ]
        }
      ]
    }
  ]
}