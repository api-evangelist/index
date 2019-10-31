{
  "info": {
    "name": "Ehr Scape Clinical Decision Support APIs Toggles default behaviour of persisting guide execution result.",
    "_postman_id": "791615a0-e3c1-4556-a055-1da329d4ca17",
    "description": "Toggles default behaviour of persisting guide execution result..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Guide",
      "item": [
        {
          "id": "f4b95acc-44fb-4e36-a9b3-4bb368eaf96f",
          "name": "getGuides",
          "request": {
            "url": "http://rest.ehrscape.com/ThinkCDS/services/CDSResources/guide",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List available guides.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49f2f722-499e-4193-8f4c-6577e178c033"
            }
          ]
        },
        {
          "id": "f1033767-12e3-4122-8eac-5675788fd884",
          "name": "executeGuide",
          "request": {
            "url": {
              "protocol": "http",
              "host": "rest.ehrscape.com",
              "path": [
                "ThinkCDS",
                "services",
                "CDSResources",
                "guide/execute/:guideId/:ehrIds"
              ],
              "query": [
                {
                  "key": "persist",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ehrIds",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "guideId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "ThinkEhr credentials as HTTP Basic Authorization",
                "disabled": false
              },
              {
                "key": "Ehr-Session",
                "value": "{}",
                "description": "Active Ehr Session token",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Execute guide on given ehr ids."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69bba0b3-a7ed-4ca2-9cc7-c8592a7ef4d8"
            }
          ]
        },
        {
          "id": "82fc05ad-2aa7-4a27-b056-309f2c4cdb05",
          "name": "uploadGuide",
          "request": {
            "url": "http://rest.ehrscape.com/ThinkCDS/services/CDSResources/guide/upload",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "guide",
                  "value": "{}",
                  "disabled": false,
                  "description": "Base64 encoded guide definition"
                }
              ]
            },
            "description": "Uploads new guide definition.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f38c241-84bd-4dd8-8fdd-8e6a5b83aeb6"
            }
          ]
        },
        {
          "id": "6dae1a0a-555e-4db4-a894-5a8b3bfab400",
          "name": "deleteGuide",
          "request": {
            "url": {
              "protocol": "http",
              "host": "rest.ehrscape.com",
              "path": [
                "ThinkCDS",
                "services",
                "CDSResources",
                "guide/:guideId"
              ],
              "variable": [
                {
                  "id": "guideId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes guide.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2811a101-eee0-40bc-bcb2-8dc86d5360b8"
            }
          ]
        },
        {
          "id": "4492d971-d66a-4c7b-bb0f-22697803627b",
          "name": "getGuideGDL",
          "request": {
            "url": {
              "protocol": "http",
              "host": "rest.ehrscape.com",
              "path": [
                "ThinkCDS",
                "services",
                "CDSResources",
                "guide/:guideId/gdl"
              ],
              "variable": [
                {
                  "id": "guideId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns guide definition.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0850797-91a7-4af3-8ab6-5e1764783acd"
            }
          ]
        },
        {
          "id": "bf78b0c8-62c1-47a1-9118-dc3add8fe337",
          "name": "toggleGuidePersistence",
          "request": {
            "url": {
              "protocol": "http",
              "host": "rest.ehrscape.com",
              "path": [
                "ThinkCDS",
                "services",
                "CDSResources",
                "guide/:guideId/toggleGuidePersistence"
              ],
              "variable": [
                {
                  "id": "guideId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Toggles default behaviour of persisting guide execution result.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3aa65ed3-57fe-4ccb-9800-1877676aa271"
            }
          ]
        }
      ]
    }
  ]
}