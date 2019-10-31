{
  "info": {
    "name": "Transavia Airports API Get Aiport",
    "_postman_id": "18000470-40e5-470f-b8ae-61d8ed25b124",
    "description": "Retrieve airport by id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Airports",
      "item": [
        {
          "id": "0a4a60d7-901a-4809-b37c-fa3bac5dc155",
          "name": ".get",
          "request": {
            "url": "http://api.transavia.com/v2/airports/",
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
            "description": "Retrieve all airports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4cc19038-fafd-4554-afed-a990ae91ffdc"
            }
          ]
        },
        {
          "id": "48c0b731-dcb4-427b-b540-79555bbaf328",
          "name": "countrycode.countryCode.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.transavia.com",
              "path": [
                "v2",
                "airports",
                "countrycode/:countryCode"
              ],
              "variable": [
                {
                  "id": "countryCode",
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
            "description": "Retrieve airports by country code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "525eb19c-ad5a-46da-9384-c9431590bc01"
            }
          ]
        },
        {
          "id": "77b0e3c9-44ef-42df-96f0-2da8621fadc3",
          "name": "nearest.get",
          "request": {
            "url": "http://api.transavia.com/v2/airports/nearest?latitude=%7B%7D&limit=%7B%7D&longitude=%7B%7D&maxDistanceInKm=%7B%7D",
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
            "description": "Retrieve nearest airports by geo coordinates (latitude/longitude)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "971dc73f-11fe-4be6-8000-45e72749bdd2"
            }
          ]
        },
        {
          "id": "3b1978a4-d63a-44b6-87ff-76973d12e96c",
          "name": "nearest.id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.transavia.com",
              "path": [
                "v2",
                "airports",
                "nearest/:id"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxDistanceInKm",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Retrieve nearest airports by station id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90b65b98-d6ff-4865-b5c7-3d637dd699f8"
            }
          ]
        },
        {
          "id": "ce620cae-7b5b-492f-924d-cae10c9642e8",
          "name": "id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.transavia.com",
              "path": [
                "v2",
                "airports",
                ":id"
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
            "description": "Retrieve airport by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d91a966-ce52-4060-b470-9ae311f125ab"
            }
          ]
        }
      ]
    }
  ]
}