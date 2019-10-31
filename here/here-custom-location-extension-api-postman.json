{
  "info": {
    "name": "HERE Custom Location Extension API Find Locations using Corridor",
    "_postman_id": "26ed668b-a156-4a82-8507-52bc3b72e669",
    "description": "*Request a list of user-defined locations near to a given corridor*\n\nThe route corridor consists of a series of latitude, longitude pairs defining the waypoints of a route, along with a defined width. A corridor search is requested using the `corridor` endpoint and by adding a series of comma delimited latitude, longitude waypoints to the `route` parameter of the request URL, along with a `radius` for the search.\n\n\n\n* **layerId**  `text`\n \\- Unique indicator used to retrieve a dataset\n\n* **route**  `text`\n \\- A type of spatial filter. The corridor is defined by its path and width. The path is a line along the center of the corridor represented by a series of latitude/longitude pairs. Corridor width is given in meters.\n\n* **radius**  `number`\n \\- width of the search corridor\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Find",
      "item": [
        {
          "id": "c1c8a5dc-c421-480f-a618-778ab02ee039",
          "name": "BboxGet2",
          "request": {
            "url": "http://customlocation.cit.api.here.com/v1/search/bbox?app_code=%7B%7D&app_id=%7B%7D&bbox=%7B%7D&layerId=%7B%7D",
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
            "description": "*Request a list of user-defined locations within a defined area*\n\nThe request uses the `bbox` endpoint, and the bounding box is specified by adding the `bbox` parameter to the request URL.\n\n\n\n* **layerId**  `text`\n \\- Unique indicator used to retrieve a dataset\n\n* **bbox**  `bbox`\n \\- Restricts results to be found within this bounding box\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b7f8753-ba57-4d94-9822-c42f8a72456f"
            }
          ]
        },
        {
          "id": "dd8dd9b5-2949-4fb7-8ca7-95436e71af3a",
          "name": "ProximityGet2",
          "request": {
            "url": "http://customlocation.cit.api.here.com/v1/search/proximity?app_code=%7B%7D&app_id=%7B%7D&coord=%7B%7D&layerId=%7B%7D&limit=%7B%7D&radius=%7B%7D",
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
            "description": "*Request a list of user-defined locations within a circle around a fixed point*\n\nThe search uses the `proximity` endpoint. The definition of the location and limit of the search is specified using  `coord` and `radius` parameters, and the number of results returned limited by adding the `limit` parameter to the request URL.\n\n\n\n* **layerId**  `text`\n \\- Unique indicator used to retrieve a dataset\n\n* **coord**  `latlng`\n \\- Center of the proximity search\n\n* **radius**  `number`\n \\- width of the search corridor\n\n* **limit**  `number`\n \\- The limit of the number of items contained in the response.\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f46da1e-5739-42ab-bf91-0cc00355c835"
            }
          ]
        },
        {
          "id": "5615942c-f407-4bfc-af4e-b7355ff1c9b0",
          "name": "RouteCorridorGet",
          "request": {
            "url": "http://customlocation.cit.api.here.com/v1/search/route/corridor?app_code=%7B%7D&app_id=%7B%7D&layerId=%7B%7D&limit=%7B%7D&radius=%7B%7D&routeId=%7B%7D",
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
            "description": "*Request a list of user-defined locations along a pre-defined route*\n\nThe route has been pre-calculated and the `routeid` has already been acquired from a previous routing request. A route-based corridor search is requested using the `corridor` endpoint and by adding the `routeid` parameter to the request URL, along with a corridor `width`.\n\n\n\n* **layerId**  `text`\n \\- Unique indicator used to retrieve a dataset\n\n* **routeId**  `text`\n \\- A <b>previously</b> calculated routeId\n\n* **radius**  `number`\n \\- Width of the search corridor\n\n* **limit**  `number`\n \\- The limit of the number of items contained in the response.\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "181506a5-cca3-4bf3-a589-099a5a887b6c"
            }
          ]
        },
        {
          "id": "e57598ca-547f-4df3-9a1e-0e95a74a43a7",
          "name": "CorridorGet",
          "request": {
            "url": "http://customlocation.cit.api.here.com/v1/search/corridor?app_code=%7B%7D&app_id=%7B%7D&layerId=%7B%7D&radius=%7B%7D&route=%7B%7D",
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
            "description": "*Request a list of user-defined locations near to a given corridor*\n\nThe route corridor consists of a series of latitude, longitude pairs defining the waypoints of a route, along with a defined width. A corridor search is requested using the `corridor` endpoint and by adding a series of comma delimited latitude, longitude waypoints to the `route` parameter of the request URL, along with a `radius` for the search.\n\n\n\n* **layerId**  `text`\n \\- Unique indicator used to retrieve a dataset\n\n* **route**  `text`\n \\- A type of spatial filter. The corridor is defined by its path and width. The path is a line along the center of the corridor represented by a series of latitude/longitude pairs. Corridor width is given in meters.\n\n* **radius**  `number`\n \\- width of the search corridor\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6771605-4590-4db7-917f-057b812160f4"
            }
          ]
        }
      ]
    }
  ]
}