{
  "info": {
    "name": "U.S. Digital Registry Mobile App API Mobile App",
    "_postman_id": "e6e1d58d-afdb-403f-8f06-39f0c287e997",
    "description": "This returns an mobile app based on an ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Mobile Apps",
      "item": [
        {
          "id": "a1b8d874-5ba6-4029-9668-8afd9b4c9249",
          "name": "Api::V1::MobileApps#tokeninput",
          "request": {
            "url": "http://usdigitalregistry.digitalgov.gov/api/v1/mobile_apps/tokeninput.json?q=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This returns tokens representing agencies, tags, and a basic text search token for the purpose of building search dialogs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09fd7aac-facf-455f-a726-925b3e21704b"
            }
          ]
        },
        {
          "id": "e4a0b373-2ae3-46d4-8475-f797e750e304",
          "name": "Api::V1::MobileApps#index",
          "request": {
            "url": "http://usdigitalregistry.digitalgov.gov/api/v1/mobile_apps.json?agencies=%7B%7D&language=%7B%7D&page=%7B%7D&page_size=%7B%7D&q=%7B%7D&tags=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This lists all active mobile apps.  It accepts parameters to perform basic search as well as searching by tag and agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99e5012a-a5dd-418e-b3bb-44ce6146852d"
            }
          ]
        },
        {
          "id": "c2164c50-c6a1-484c-88ed-947acaeed4fe",
          "name": "Api::V1::MobileApps#show",
          "request": {
            "url": {
              "protocol": "http",
              "host": "usdigitalregistry.digitalgov.gov",
              "path": [
                "api",
                "v1",
                "mobile_apps/:id.json"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This returns an mobile app based on an ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96f0c6dd-9f67-4dc7-af0b-dd2b7e20db85"
            }
          ]
        }
      ]
    }
  ]
}