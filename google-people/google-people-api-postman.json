{
  "info": {
    "name": "Google People API Get Connections",
    "_postman_id": "6339db6c-7e1f-4fdc-b9b7-d1ec156d54e7",
    "description": "Provides a list of the authenticated user's contacts merged with any\nlinked profiles.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "People",
      "item": [
        {
          "id": "829f66fb-abfd-4bcc-b4a1-40a504dbf37a",
          "name": "people.people.getBatchGet",
          "request": {
            "url": "http://people.googleapis.com/v1/people:batchGet?requestMask.includeField=%7B%7D&resourceNames=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides information about a list of specific people by specifying a list\nof requested resource names. Use `people/me` to indicate the authenticated\nuser."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ff3a6cd-6161-4441-8bc9-e88af4dc77c6"
            }
          ]
        },
        {
          "id": "1b9745a1-0c43-4394-b822-a7d6bd4e2c3d",
          "name": "people.people.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "people.googleapis.com",
              "path": [
                "v1/:resourceName"
              ],
              "query": [
                {
                  "key": "requestMask.includeField",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "resourceName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides information about a person resource for a resource name. Use\n`people/me` to indicate the authenticated user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a5ca46f-64c8-4f56-9a47-e9f8285743c3"
            }
          ]
        }
      ]
    },
    {
      "name": "Connection",
      "item": [
        {
          "id": "fd29c34b-342e-4dd3-b2fe-9813aac6ceed",
          "name": "people.people.connections.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "people.googleapis.com",
              "path": [
                "v1/:resourceName/connections"
              ],
              "query": [
                {
                  "key": "pageSize",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "requestMask.includeField",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "requestSyncToken",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sortOrder",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "syncToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "resourceName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides a list of the authenticated user's contacts merged with any\nlinked profiles."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7d7d5e0-eb04-488c-a78c-7b042f09ead9"
            }
          ]
        }
      ]
    }
  ]
}