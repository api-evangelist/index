{
  "info": {
    "name": "HERE Geocoder API Multi-reverse Geocode Addresses",
    "_postman_id": "38ae1da9-7e27-444e-b95a-c1448d32eee4",
    "description": "*Request the addresses of up to one hundred locations with one multi-reverse geocoding request*\n\nThe body of the HTTP POST request contains the coordinates and optional radius in the `prox` parameter and an optional numeric identifier in the `id` parameter as plain text, one line per pair of coordinates. The identifier associates each result with the corresponding input. If no id is provided the system creates one starting with 0.\n  \n\n\n\n* **mode**  `enum`\n \\- Search for prominent landmarks nearby  \n\n Valid values are : `retrieveAddresses`, `retrieveAreas`, `retrieveLandmarks`, `retrieveAll`, `trackPosition`\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible behavior in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.\n\n* **Content-Type**  `header`\n\n  Accept any content in return\n\n* **Cache-Control**  `header`\n\n  Ensure that the request is always passed to server so that latest response is retrieved",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Geocode",
      "item": [
        {
          "id": "82fcb43c-63ce-4292-aa86-d965eb1d32bb",
          "name": "GeocodeJsonGet5",
          "request": {
            "url": "http://geocoder.cit.api.here.com/6.2/geocode.json?app_code=%7B%7D&app_id=%7B%7D&city=%7B%7D&country=%7B%7D&gen=%7B%7D&housenumber=%7B%7D&street=%7B%7D",
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
            "description": "*Request the latitude, longitude and details of an address based on partial address information*\n\nThis example shows a structured (qualified) geocoding request using the `geocode` endpoint. In this structured request the data is provided in `country`, `city`, `street` and `housenumber` parameters in the request URL. Note that the street name misses the directional (\"W\") and also the street type. The omitted directional makes the query ambiguous and the response contains therefore two results: One address on West Randolph St and one on East Randolph St.\n  \n\n\n\n* **housenumber**  `text`\n \\- The house number or house name\n\n* **street**  `text`\n \\- The street name can include suite, apt and floor information.\n\n* **city**  `text`\n \\- City name\n\n* **country**  `text`\n \\- Specify the country or list of countries using the country code (3 bytes, ISO 3166-1-alpha-3) or the country name\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible behavior in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ffab65a4-03b0-41a5-90bf-69dc7db007d1"
            }
          ]
        }
      ]
    },
    {
      "name": "Reverse",
      "item": [
        {
          "id": "3fe04dc4-5fb3-4b1f-86f2-807edaf7b25e",
          "name": "ReversegeocodeJsonGet4",
          "request": {
            "url": "http://geocoder.cit.api.here.com/6.2/reversegeocode.json?app_code=%7B%7D&app_id=%7B%7D&gen=%7B%7D&mode=%7B%7D&prox=%7B%7D",
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
            "description": "*Request details of landmarks near to a given latitude and longitude*\n\nLandmark reverse geocoding requests can be made using the `reversegeocode` endpoint, specifying the parameter `mode=retrieveLandmarks`, and adding the `prox` parameter to the request URL.  Consult the  Geocoder API Reference for a full list of available landmark types.\n\n\n\n* **prox**  `prox`\n \\- A type of spatial filter. Proximity specifies a circle to search using a latitude, a longitude, and a radius in meters.    e.g. `52.515,13.377,100`\n\n* **mode**  `enum`\n \\- Type of search invoked. Search for streets, administrative areas or landmarks, or a combination of all three\n\n Valid values are : `retrieveAddresses`, `retrieveAreas`, `retrieveLandmarks`, `retrieveAll`, `trackPosition`\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible behavior in the API"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9875b0b-5cdf-4528-82d2-60007d7ce746"
            }
          ]
        }
      ]
    },
    {
      "name": "Multi-reverse",
      "item": [
        {
          "id": "e8c6a5a7-2640-4f7e-b2a0-5a077b03e1c7",
          "name": "MultiReversegeocodeJsonPost2",
          "request": {
            "url": "http://geocoder.cit.api.here.com/6.2/multi-reversegeocode.json?app_code=%7B%7D&app_id=%7B%7D&gen=%7B%7D&mode=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Cache-Control",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "*Request the addresses of up to one hundred locations with one multi-reverse geocoding request*\n\nThe body of the HTTP POST request contains the coordinates and optional radius in the `prox` parameter and an optional numeric identifier in the `id` parameter as plain text, one line per pair of coordinates. The identifier associates each result with the corresponding input. If no id is provided the system creates one starting with 0.\n  \n\n\n\n* **mode**  `enum`\n \\- Search for prominent landmarks nearby  \n\n Valid values are : `retrieveAddresses`, `retrieveAreas`, `retrieveLandmarks`, `retrieveAll`, `trackPosition`\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible behavior in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.\n\n* **Content-Type**  `header`\n\n  Accept any content in return\n\n* **Cache-Control**  `header`\n\n  Ensure that the request is always passed to server so that latest response is retrieved"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0bd1b1b2-09e8-4876-8fcc-38173d626e31"
            }
          ]
        }
      ]
    }
  ]
}