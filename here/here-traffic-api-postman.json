{
  "info": {
    "name": "HERE Traffic API Traffic Incidents via Proximity",
    "_postman_id": "bc7a47b1-3fb6-4981-aa36-c247352135ae",
    "description": "*Request traffic incident information within specified area*\n\nTraffic incidents can be retrieved through several different request types, based on the addressing schemes that they use to specify their geography. Traffic requests can be output to either XML or JSON format. API also supports filters to limit the amount of information provided in the response. Filters are based on on status, criticality, TMC table IDs, profiles, or start and end times, etc.\n\n\n\n* **prox**  `prox`\n \\- A type of spatial filter. Proximity specifies a circle to search using a latitude, a longitude, and a radius in meters.    e.g. `52.515,13.377,100`\n\n* **criticality**  `multi-enum`\n \\- A filter that selects incident reports according to criticality,  `0`=critical, `1`=major, `2`=minor,  `3`=lowImpact\n\n Valid values are : `0` - critical, `1` - major, `2` - minor, `3` - lowImpact\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Traffic",
      "item": [
        {
          "id": "70b01678-0ad2-49ca-8871-1432883475e8",
          "name": "60FlowavailabilityJsonGet",
          "request": {
            "url": "http://tiles.traffic.cit.api.here.com/traffic/6.0/tiles/8/133/86/256/6.0/flowavailability.json?app_code=%7B%7D&app_id=%7B%7D",
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
            "description": "*Flow availability requests allow you to see what traffic flow coverage exists in the current Traffic API.*\n\nT<i></i>he Server also supports an XML response.\n\n\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e919aac-f69f-406a-a739-ff71669109dd"
            }
          ]
        },
        {
          "id": "77078c04-f641-4b1d-a23c-31b8a3a0aea6",
          "name": "60IncidentsJsonGet3",
          "request": {
            "url": "http://tiles.traffic.cit.api.here.com/traffic/6.0/tiles/8/133/86/256/6.0/incidents.json?app_code=%7B%7D&app_id=%7B%7D&criticality=%7B%7D&prox=%7B%7D",
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
            "description": "*Request traffic incident information within specified area*\n\nTraffic incidents can be retrieved through several different request types, based on the addressing schemes that they use to specify their geography. Traffic requests can be output to either XML or JSON format. API also supports filters to limit the amount of information provided in the response. Filters are based on on status, criticality, TMC table IDs, profiles, or start and end times, etc.\n\n\n\n* **prox**  `prox`\n \\- A type of spatial filter. Proximity specifies a circle to search using a latitude, a longitude, and a radius in meters.    e.g. `52.515,13.377,100`\n\n* **criticality**  `multi-enum`\n \\- A filter that selects incident reports according to criticality,  `0`=critical, `1`=major, `2`=minor,  `3`=lowImpact\n\n Valid values are : `0` - critical, `1` - major, `2` - minor, `3` - lowImpact\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc4b4559-7432-41af-b548-8ebea116652d"
            }
          ]
        }
      ]
    }
  ]
}