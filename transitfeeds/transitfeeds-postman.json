{
  "info": {
    "name": "TransitFeeds Retrieve a list of versions of specified (or all) feeds.",
    "_postman_id": "859c8b73-4819-4a7c-a299-b5404aa700ff",
    "description": "This API call allows you to easily see every single feed update in the TranstiFeeds.com system. Since this can be quite\nlong, it's also possible to filter this list by a single feed ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "29d2ea65-9ee7-40a1-b4e4-88fd5b6391c3",
          "name": "getLocations",
          "request": {
            "url": "http://api.transitfeeds.com/v1/getLocations?key=%7B%7D",
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
            "description": "Retrieve a list of locations. Each location (except for the root) has a parent location, and each\nlocation has zero or more child locations. This hierarchy is generally structured so countries contain\nstates, states contain cities (although this typically depends on the country)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e0e3372-353d-416a-b4a7-de7f18860dca"
            }
          ]
        },
        {
          "id": "173f17b5-cb31-4bbf-a61d-8645b39e3fe2",
          "name": "getFeeds",
          "request": {
            "url": "http://api.transitfeeds.com/v1/getFeeds?descendants=%7B%7D&key=%7B%7D&limit=%7B%7D&location=%7B%7D&page=%7B%7D&type=%7B%7D",
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
            "description": "Used this API to retrieve a list of feeds in the system. Doing so can be usedful to discover feed IDs that\ncan be used in other API calls."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50a0b00f-b30b-42a6-a261-a4f43dc86839"
            }
          ]
        },
        {
          "id": "b9d8c471-1915-4310-8ffe-f463cdb419ff",
          "name": "getLatestFeedVersion",
          "request": {
            "url": "http://api.transitfeeds.com/v1/getLatestFeedVersion?feed=%7B%7D&key=%7B%7D",
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
            "description": "Once you have used `/getFeeds` to discover a feed's URL, you can use this endpoint to download its latest version from TranstiFeeds.\nIt will be unmodified in the original format from the provider."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0706708c-f484-4a0e-893b-acddd22aa840"
            }
          ]
        },
        {
          "id": "a0e59ff0-cd1a-4434-9086-b71392cf9244",
          "name": "getFeedVersions",
          "request": {
            "url": "http://api.transitfeeds.com/v1/getFeedVersions?err=%7B%7D&feed=%7B%7D&key=%7B%7D&limit=%7B%7D&page=%7B%7D&warn=%7B%7D",
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
            "description": "This API call allows you to easily see every single feed update in the TranstiFeeds.com system. Since this can be quite\nlong, it's also possible to filter this list by a single feed ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77b48f6b-be5c-4a94-a9d2-246ba9fabd43"
            }
          ]
        }
      ]
    }
  ]
}