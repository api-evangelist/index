{
  "info": {
    "name": "HERE Route Match Extension API Available Attributes within a Map Data Layer",
    "_postman_id": "49ba7c2a-3b3c-43e7-9a58-4abb4c5e1aed",
    "description": "*Request which attributes are available within a specified map data layer*\n\nTo make a request for map data layer information, use the `layer``.json` endpoint, supplying the `release`, `layer` and `region` parameters.\n\n\n\n* **region**  `text`\n \\- Map Coverage Region.    e.g. `APAC`, `NA`, `EU`\n\n* **release**  `text`\n \\- Map release quarter    e.g. `2014Q4` or `LATEST`\n\n* **layer**  `text`\n \\- Thematic layer\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Available",
      "item": [
        {
          "id": "891585db-a1f4-43c8-8061-49d34c568581",
          "name": "DocLayersJsonGet",
          "request": {
            "url": "http://pde.cit.api.here.com/1/doc/layers.json?app_code=%7B%7D&app_id=%7B%7D&region=%7B%7D&release=%7B%7D",
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
            "description": "*Request which data layers can be accessed within a specified map region and release*\n\nTo make a request for data layer availability information, use the `layers.json` endpoint, supplying the `release` and `region` parameters.\n\n\n\n* **region**  `text`\n \\- Map Coverage Region.    e.g. `APAC`, `NA`, `EU`\n\n* **release**  `text`\n \\- Map release quarter    e.g. `2014Q4` or `LATEST`\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6aeefa55-e47e-4bf6-bc60-43495b10e04d"
            }
          ]
        },
        {
          "id": "d2863d04-1ad1-44dc-b33f-3784a92154ce",
          "name": "DocLayerJsonGet",
          "request": {
            "url": "http://pde.cit.api.here.com/1/doc/layer.json?app_code=%7B%7D&app_id=%7B%7D&layer=%7B%7D&region=%7B%7D&release=%7B%7D",
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
            "description": "*Request which attributes are available within a specified map data layer*\n\nTo make a request for map data layer information, use the `layer``.json` endpoint, supplying the `release`, `layer` and `region` parameters.\n\n\n\n* **region**  `text`\n \\- Map Coverage Region.    e.g. `APAC`, `NA`, `EU`\n\n* **release**  `text`\n \\- Map release quarter    e.g. `2014Q4` or `LATEST`\n\n* **layer**  `text`\n \\- Thematic layer\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2842823f-9ead-4966-a088-7faf247861e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Map",
      "item": [
        {
          "id": "b22ad4c1-b36a-45a4-b45a-e15c8251642b",
          "name": "DocMapsJsonGet",
          "request": {
            "url": "http://pde.cit.api.here.com/1/doc/maps.json?app_code=%7B%7D&app_id=%7B%7D",
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
            "description": "*Request the release date and area covered by each available map region*\n\nTo make a request for release date information, use the `maps.json` endpoint.\n\n\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba7802d5-36c8-4f24-b63c-cc19afa9001e"
            }
          ]
        }
      ]
    }
  ]
}