{
  "info": {
    "name": "HERE Routing API Previously calculated route information",
    "_postman_id": "31833c48-4161-434b-aaac-806775b2c471",
    "description": "*Request information about a previously calculated route*\n\nPrevious routes can be retrieved using the `getroute` endpoint and appending a `routeid` to the request. The `routeid` in question has been generated from a previous request. Note that server map updates usually invalidates `routeid` value computed on previous map versions. If it is the case, the `routeid` computation should be requested again on the map in current  use.\n  \n\n\n\n* **mode**  `text`\n \\- Routing mode determines how the route is calculated.    e.g. `fastest;car;traffic:disabled.`  \n\n* **routeid**  `text`\n \\- Route identifier for which the detailed route information is being requested.  \n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.  \n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Link",
      "item": [
        {
          "id": "a4edc10f-7b3a-42be-b811-5d338d67c1cf",
          "name": "GetlinkinfoJsonGet2",
          "request": {
            "url": "http://route.cit.api.here.com/routing/7.2/getlinkinfo.json?app_code=%7B%7D&app_id=%7B%7D&linkids=%7B%7D",
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
            "description": "*Request detailed information about a path segment in the routing network given a linkid*\n\nLink information can be retrieved using the `getlinkinfo` endpoint, by specifying one or more comma separated linkIds using the `linkids` parameter. The `linkids` have been generated from a previous request. Note that positive direction '+' in link Ids has to be URL encoded.\n  \n  \n\n\n\n* **linkids**  `text`\n \\- Link identifiers for which the detailed information is being requested.\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "772f5079-cd06-47d7-8604-8276a65dd182"
            }
          ]
        }
      ]
    },
    {
      "name": "Previously",
      "item": [
        {
          "id": "9b407f69-ade9-48fd-b4e4-b94f2e5069d3",
          "name": "GetrouteJsonGet",
          "request": {
            "url": "http://route.cit.api.here.com/routing/7.2/getroute.json?app_code=%7B%7D&app_id=%7B%7D&mode=%7B%7D&routeid=%7B%7D",
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
            "description": "*Request information about a previously calculated route*\n\nPrevious routes can be retrieved using the `getroute` endpoint and appending a `routeid` to the request. The `routeid` in question has been generated from a previous request. Note that server map updates usually invalidates `routeid` value computed on previous map versions. If it is the case, the `routeid` computation should be requested again on the map in current  use.\n  \n\n\n\n* **mode**  `text`\n \\- Routing mode determines how the route is calculated.    e.g. `fastest;car;traffic:disabled.`  \n\n* **routeid**  `text`\n \\- Route identifier for which the detailed route information is being requested.  \n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.  \n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34a96f6f-96d1-4493-a6ea-55b2a5af686a"
            }
          ]
        }
      ]
    }
  ]
}