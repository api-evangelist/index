{
  "info": {
    "name": "Bands in Town Get all upcoming artist events or all past and upcoming events within a date range",
    "_postman_id": "d63d8026-7f2f-4cce-84cd-18d330627066",
    "description": "artist events",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bands",
      "item": [
        {
          "id": "e2894675-bee6-481e-ba72-c9901af2ebaa",
          "name": "artist",
          "request": {
            "url": {
              "protocol": "http",
              "host": "rest.bandsintown.com",
              "path": [
                "artists/:artistname"
              ],
              "query": [
                {
                  "key": "app_id",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "artistname",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get artist information"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0ba1dc3-74ed-4e31-9fe8-5bf325eddb25"
            }
          ]
        },
        {
          "id": "652065c3-8b2c-4ead-ac59-193f45ac99ef",
          "name": "artistEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "rest.bandsintown.com",
              "path": [
                "artists/:artistname/events"
              ],
              "query": [
                {
                  "key": "app_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "artistname",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "artist events"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36242fcf-f0b3-417d-80ad-f1c6ca22f46b"
            }
          ]
        }
      ]
    }
  ]
}