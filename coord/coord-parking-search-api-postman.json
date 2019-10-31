{
  "info": {
    "name": "Coord Parking Search API Get a list of off-street parking locations.",
    "_postman_id": "db189910-7588-426b-abbc-c30ae989f043",
    "description": "Find a single locations within a given are and return their pricing information and\n(when present) availability. If the `duration_m` parameter is set, total cost for a stay\nof that duration will also be returned.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "47b0f2b0-ed30-45b3-8d2b-0da00362ca55",
          "name": "get_locations",
          "request": {
            "url": "http://api.coord.co/v1/search/parking/location?access_key=%7B%7D&duration_m=%7B%7D&latitude=%7B%7D&location_ids=%7B%7D&longitude=%7B%7D&parking_start_time=%7B%7D&radius_km=%7B%7D",
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
            "description": "Find all of the locations within a given are and return their pricing information and\n(when present) availability. If the `duration_m` parameter is set, total cost for a stay\nof that duration will also be returned."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d375ad3a-bc98-4bfc-9403-f6fbc4209197"
            }
          ]
        },
        {
          "id": "4fb8a343-09f8-454c-8cbc-a24714246011",
          "name": "get_location",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.coord.co",
              "path": [
                "v1",
                "search",
                "parking",
                "location/:id"
              ],
              "query": [
                {
                  "key": "access_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "duration_m",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "parking_start_time",
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
            "description": "Find a single locations within a given are and return their pricing information and\n(when present) availability. If the `duration_m` parameter is set, total cost for a stay\nof that duration will also be returned."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ed619c5-a579-4f36-8f50-4aa5bbfbba72"
            }
          ]
        }
      ]
    }
  ]
}