{
  "info": {
    "name": "NPR Retrieve metadata for the station with the given numeric ID",
    "_postman_id": "276f6dba-7e09-4f44-a10a-ebfe5987ea94",
    "description": "This endpoint retrieves information about a given station, based on its numeric ID, which is consistent across all of NPR's APIs.\n\nA typical use case for this data is for clients who want to create a dropdown menu, modal/pop-up or dedicated page displaying more information about the station the client is localized to, including, for example, links to the station's homepage and donation (pledge) page.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "stationfinder",
      "item": [
        {
          "id": "2b2832ad-726a-4982-8efb-13781422437e",
          "name": "getStationById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.npr.org",
              "path": [
                "stationfinder/v3/stations/:stationId"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "stationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint retrieves information about a given station, based on its numeric ID, which is consistent across all of NPR's APIs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42dbdb10-4207-4ea5-8cf1-1359d8445156"
            }
          ]
        }
      ]
    }
  ]
}