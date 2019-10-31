{
  "info": {
    "name": "Coord Curb Search API Find the rules for curbs near a location at a certain time.",
    "_postman_id": "4be5b9d5-3888-449e-8a10-4147227991fb",
    "description": "Find the rules for a given curb at a given time and on a given day. You can also use this\nto find all of the places that it is possible to perform a given action (for instance, find\nall the loading zones, or everywhere with two-hour parking).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Find",
      "item": [
        {
          "id": "4c06b1da-0b46-48b4-875e-48702da9a734",
          "name": "get_by_bounds",
          "request": {
            "url": "http://api.coord.co/v1/search/curbs/bybounds/all_rules?access_key=%7B%7D&No Name=%7B%7D",
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
            "description": "Find the rules for all curbs within a bounding box.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec697612-a661-4cb1-9ca7-398b62bb1bad"
            }
          ]
        },
        {
          "id": "96a83663-1d39-42ed-a0a3-8b13119b9dff",
          "name": "get_at_time_by_bounds",
          "request": {
            "url": "http://api.coord.co/v1/search/curbs/bybounds/time_rules?access_key=%7B%7D&No Name=%7B%7D",
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
            "description": "Find the rules for all curbs within a bounding box at a particular time.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14a5f92c-e3e8-4ce1-a905-34081bb61f06"
            }
          ]
        },
        {
          "id": "9f8c7cbb-4757-484e-8805-81ca5db058b9",
          "name": "get_by_curb_id",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.coord.co",
              "path": [
                "v1",
                "search",
                "curbs",
                "bycurb/:id/all_rules"
              ],
              "query": [
                {
                  "key": "access_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
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
            "description": "Find the rules on single curb.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9178e551-63f5-43b1-a61c-84402c360381"
            }
          ]
        },
        {
          "id": "a978256d-07cf-4b46-ad8e-13db68bd553b",
          "name": "get_at_time_by_curb_id",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.coord.co",
              "path": [
                "v1",
                "search",
                "curbs",
                "bycurb/:id/time_rules"
              ],
              "query": [
                {
                  "key": "access_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
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
            "description": "Find the rules on a single curb at a certain time.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0490c330-16ba-4f33-bace-ee7d4a7d7b6d"
            }
          ]
        },
        {
          "id": "88ef5b80-055b-4104-90dc-70cf52d9067c",
          "name": "get_by_location",
          "request": {
            "url": "http://api.coord.co/v1/search/curbs/bylocation/all_rules?access_key=%7B%7D&No Name=%7B%7D",
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
            "description": "Find all of the curbs within a given radius of a particular point, and return all of their\nrules across all times of day, days of the week, times of year, etc."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4d4733c-caa8-4ad6-9463-adf27fbe92ec"
            }
          ]
        },
        {
          "id": "b6a745d5-1550-42e1-b760-32e1b4c5d010",
          "name": "get_at_time_by_location",
          "request": {
            "url": "http://api.coord.co/v1/search/curbs/bylocation/time_rules?access_key=%7B%7D&No Name=%7B%7D",
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
            "description": "Find the rules for a given curb at a given time and on a given day. You can also use this\nto find all of the places that it is possible to perform a given action (for instance, find\nall the loading zones, or everywhere with two-hour parking)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73042b18-6db6-4e20-a331-11a9dc046d81"
            }
          ]
        }
      ]
    }
  ]
}