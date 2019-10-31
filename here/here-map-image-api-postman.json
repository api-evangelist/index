{
  "info": {
    "name": "HERE Map Image API Map Image with Polylines",
    "_postman_id": "8d91d4fd-dc65-4180-889a-d828f970218c",
    "description": "*Request an image of a map including a polyline*\n\nIt supports also different map schemes, image sizes; image formats as \r\nwell as zooming out from automatically calculated zoom level.\n  \n\n\n\n* **r0**  `text`\n \\- List of coordinates describing the first route\n\n* **r1**  `text`\n \\- List of coordinates describing the second route\n\n* **m0**  `text`\n \\- First route marker on the map\n\n* **m1**  `text`\n \\- Second route marker on the map\n\n* **lc0**  `text`\n \\- Color of the first route line displayed on the map\n\n* **sc0**  `text`\n \\- Shadow color of the first route line displayed on the map\n\n* **lw0**  `number`\n \\- Width of the first route line displayed on the map\n\n* **lc1**  `text`\n \\- Color of the second route line displayed on the map\n\n* **sc1**  `text`\n \\- Shadow color of the second route line displayed on the map\n\n* **lw1**  `number`\n \\- Width of the second route line displayed on the map\n\n* **w**  `number`\n \\- Image width in pixels, maximum 2048.\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Map",
      "item": [
        {
          "id": "8b93a2a5-5d61-414d-bc56-cc67ecd6a1f2",
          "name": "MapviewGet15",
          "request": {
            "url": "http://image.maps.cit.api.here.com/mia/1.6/mapview?app_code=%7B%7D&app_id=%7B%7D&bbox=%7B%7D",
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
            "description": "*Request an image of a map based around a given area*\n\nTo specify a bounding box, add the `bbox` parameter to the request URL. On desktop browsers, redirection to `here.com` will occur automatically unless the `nord` parameter is also added to URL.\n\n\n\n* **bbox**  `text`\n \\- Bounding box of the map specifying the top-right and bottom left corners.    e.g. `52.515,13.377,52.134,13.978`\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7f94fd4-05db-47a8-b7ee-45f134ae53de"
            }
          ]
        },
        {
          "id": "0840d19a-5924-48bc-9149-1e8854f38f8f",
          "name": "RouteGet",
          "request": {
            "url": "http://image.maps.cit.api.here.com/mia/1.6/route?app_code=%7B%7D&app_id=%7B%7D&lc0=%7B%7D&lc1=%7B%7D&lw0=%7B%7D&lw1=%7B%7D&m0=%7B%7D&m1=%7B%7D&r0=%7B%7D&r1=%7B%7D&sc0=%7B%7D&sc1=%7B%7D&w=%7B%7D",
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
            "description": "*Request an image of a map including a polyline*\n\nIt supports also different map schemes, image sizes; image formats as \r\nwell as zooming out from automatically calculated zoom level.\n  \n\n\n\n* **r0**  `text`\n \\- List of coordinates describing the first route\n\n* **r1**  `text`\n \\- List of coordinates describing the second route\n\n* **m0**  `text`\n \\- First route marker on the map\n\n* **m1**  `text`\n \\- Second route marker on the map\n\n* **lc0**  `text`\n \\- Color of the first route line displayed on the map\n\n* **sc0**  `text`\n \\- Shadow color of the first route line displayed on the map\n\n* **lw0**  `number`\n \\- Width of the first route line displayed on the map\n\n* **lc1**  `text`\n \\- Color of the second route line displayed on the map\n\n* **sc1**  `text`\n \\- Shadow color of the second route line displayed on the map\n\n* **lw1**  `number`\n \\- Width of the second route line displayed on the map\n\n* **w**  `number`\n \\- Image width in pixels, maximum 2048.\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f122e336-c0dd-4d16-8b51-d6fa860c4bf9"
            }
          ]
        }
      ]
    }
  ]
}