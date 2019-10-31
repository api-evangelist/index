{
  "info": {
    "name": "NxtPort UN Location Codes API Get Locations Locode",
    "_postman_id": "a41532a6-fdc3-4862-ab9f-1f4883497af1",
    "description": "Get the details of 1 location based on the locode.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Locations",
      "item": [
        {
          "id": "145f7997-ec2f-47be-bb7a-9e990181f157",
          "name": "searchLocations",
          "request": {
            "url": "http://api.nxtport.eu/unlocodes/v1/locations?code=%7B%7D&country=%7B%7D&page=%7B%7D&searchterm=%7B%7D&size=%7B%7D&subdiv=%7B%7D",
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
            "description": "This api will return a (paged) list of locations that match the search parameters (query parameters) ordered by the name without diacritics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be45c8d0-6aef-486b-ac35-9d9b71d5bc5d"
            }
          ]
        },
        {
          "id": "564fb2c8-513c-46b0-bab5-44c260271279",
          "name": "locations_getinNeighbourhood",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nxtport.eu",
              "path": [
                "unlocodes",
                "v1",
                "locations/:latitude/:longitude/:radius"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "size",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "latitude",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "longitude",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "radius",
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
            "description": "This api will return locations in a certain radius of a point, ordered by distance , not necessarily in the same country"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b83e89a-258f-4ecb-a83c-f43537f3ff4f"
            }
          ]
        },
        {
          "id": "3f3bffdb-3045-4acc-aa1a-d275ee4d557c",
          "name": "locations_getByCountryAndLocode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nxtport.eu",
              "path": [
                "unlocodes",
                "v1",
                "locations/:locode"
              ],
              "variable": [
                {
                  "id": "locode",
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
            "description": "Get the details of 1 location based on the locode."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f53fe35-dee5-4949-b1f8-f15faa303e83"
            }
          ]
        }
      ]
    }
  ]
}