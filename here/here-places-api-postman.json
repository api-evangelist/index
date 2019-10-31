{
  "info": {
    "name": "HERE Places API One-Box Search",
    "_postman_id": "7fbd91a5-9c7b-48b4-b0cd-3c771e66b7a2",
    "description": "*Request a list of nearby places based on a query string*\n\nA free-text places search can be made using the `discover/search` endpoint in the request URL and adding the `q` parameter with the query string. The focal point of the search is defined using the `at` parameter.\n\n\n\n* **at**  `latlng`\n \\- Location of the central point for the places search.    e.g. `52.515,13.377`\n\n* **q**  `text`\n \\- Free-form text containing the search term.    e.g. `restaurant` or `Brandenburger Tor`\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.\n\n* **Accept**  `header`\n\n  Format to request from the server",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "a50654ba-bfc2-425e-9b60-18d8649bbf31",
          "name": "SuggestGet",
          "request": {
            "url": "http://places.demo.api.here.com/places/v1/suggest?app_code=%7B%7D&app_id=%7B%7D&at=%7B%7D&q=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "*Request a list of suggestions based on a partial query string*\n\nA suggestions request can be made using the `suggest` endpoint in the request URL and adding the `q` parameter with the partial query string. The focal point for the suggestion service is defined using the `at` parameter.\n\n\n\n* **at**  `latlng`\n \\- Location of the central point for the places search.    e.g. `52.515,13.377`\n\n* **q**  `text`\n \\- Free-form text containing the search term.    e.g. `restaurant` or `Brandenburger Tor`\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.\n\n* **Accept**  `header`\n\n  Format to request from the server"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb3bcfa5-cd0a-4278-96a1-d13151151c57"
            }
          ]
        }
      ]
    },
    {
      "name": "Place",
      "item": [
        {
          "id": "c909e9ed-6736-4602-8f3d-3ac445a2cb79",
          "name": "CategoriesPlacesGet",
          "request": {
            "url": "http://places.demo.api.here.com/places/v1/categories/places?app_code=%7B%7D&app_id=%7B%7D&at=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "*Request a list of place categories available for a given location*\n\nA place category request can be made using the `categories/places` endpoint in the request URL and specifying the  focal point using the `at` parameter.\n\n\n\n* **at**  `latlng`\n \\- Location of the central point for the places search.    e.g. `52.515,13.377`\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.\n\n* **Accept**  `header`\n\n  Format to request from the server"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "491a79b4-ddde-4406-8a63-db7aa940eb0b"
            }
          ]
        }
      ]
    },
    {
      "name": "Explore",
      "item": [
        {
          "id": "c180fee8-b219-4b6c-b1f7-40055d60ecc4",
          "name": "DiscoverExploreGet5",
          "request": {
            "url": "http://places.demo.api.here.com/places/v1/discover/explore?app_code=%7B%7D&app_id=%7B%7D&at=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "*Request a list of popular places around a location*\n\nThe `explore` location context can either be an explicitly given location using the `at` parameter, or implicitly defined by a user's current position or the currently visible map.\n\n\n\n* **at**  `latlng`\n \\- Location of the central point for the places search.    e.g. `52.515,13.377`\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.\n\n* **Accept**  `header`\n\n  Format to request from the server"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6eae2877-5bd6-409b-b2eb-9cbac1233f42"
            }
          ]
        },
        {
          "id": "fca72220-c25b-4fca-b876-b5ceb67088f2",
          "name": "DiscoverHereGet",
          "request": {
            "url": "http://places.demo.api.here.com/places/v1/discover/here?app_code=%7B%7D&app_id=%7B%7D&at=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "*Request a list of places close to a location *\n\nThe `discover/here` endpoint allow users to request a list of places near to a given point, based on a location precision parameter (in this case the `at` parameter) which must be provided. If the precision is high, the places around that point are returned in order of proximity. Otherwise a set of recommended places in the area is returned.\n\n\n\n* **at**  `latlng`\n \\- Location of the central point for the places search.    e.g. `52.515,13.377`\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.\n\n* **Accept**  `header`\n\n  Format to request from the server"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae49d6be-ab48-40ad-a281-7d0f1a3883fc"
            }
          ]
        }
      ]
    },
    {
      "name": "One-Box",
      "item": [
        {
          "id": "670d23ad-ecea-4346-bde7-fafa366c1efb",
          "name": "DiscoverSearchGet",
          "request": {
            "url": "http://places.demo.api.here.com/places/v1/discover/search?app_code=%7B%7D&app_id=%7B%7D&at=%7B%7D&q=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "*Request a list of nearby places based on a query string*\n\nA free-text places search can be made using the `discover/search` endpoint in the request URL and adding the `q` parameter with the query string. The focal point of the search is defined using the `at` parameter.\n\n\n\n* **at**  `latlng`\n \\- Location of the central point for the places search.    e.g. `52.515,13.377`\n\n* **q**  `text`\n \\- Free-form text containing the search term.    e.g. `restaurant` or `Brandenburger Tor`\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.\n\n* **Accept**  `header`\n\n  Format to request from the server"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a63b6835-0b6d-43a7-a58d-1263a0087a3c"
            }
          ]
        }
      ]
    }
  ]
}