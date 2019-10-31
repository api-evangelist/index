{
  "info": {
    "name": "HERE Waypoint Sequence Extension API Waypoint Sequence for Hazardous Materials",
    "_postman_id": "fc71381c-1751-476e-9c5e-4ba1b482cde2",
    "description": "*Request an ordered list of destinations for a truck carrying hazardous materials*\n\nWaypoint sequence calcuations are made using the `findsequence` endpoint and appending  `start` and `end` parameters and consecutively numbered `destination` parameters are used to add intermediate points  to the request. Hazardous material types are added as a comma-delimited list to the  `shippedHazardousGoods` parameter. The list of values is defined in the Enterprise Routing API\n\n\n\n* **start**  `latlng`\n \\- Start point for the route calculations.    e.g. `52.515,13.377`\n\n* **destination1**  `latlng`\n \\- A point through which the route must pass.    e.g. `52.6172,13.3833`\n\n* **destination2**  `latlng`\n \\- A point through which the route must pass.    e.g. `52.6172,13.3833`\n\n* **destination3**  `latlng`\n \\- A point through which the route must pass.    e.g. `52.6172,13.3833`\n\n* **destination4**  `latlng`\n \\- A point through which the route must pass.    e.g. `52.6172,13.3833`\n\n* **end**  `latlng`\n \\- End point for the route calculations.    e.g. `50.121,8.925`\n\n* **improveFor**  `enum`\n \\- Whether to improve for time or distance\n\n Valid values are : `time`, `distance`\n\n* **mode**  `text`\n \\- Routing mode determines how the route is calculated.    e.g. `fastest;car;traffic:disabled`\n\n* **shippedHazardousGoods**  `multi-enum`\n \\- Truck routing only, list of hazardous materials in the vehicle.\n\n Valid values are : `combustible`, `corrosive`, `explosive`, `flammable`, `gas`, `harmfulToWater`, `organic`, `other`, `poison`, `poisonousInhalation`, `radioActive`\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Waypoint",
      "item": [
        {
          "id": "0cad7e96-533c-4423-9529-83975ea63a81",
          "name": "FindsequenceJsonGet4",
          "request": {
            "url": "http://wse.cit.api.here.com/2/findsequence.json?app_code=%7B%7D&app_id=%7B%7D&destination1=%7B%7D&destination2=%7B%7D&destination3=%7B%7D&destination4=%7B%7D&end=%7B%7D&improveFor=%7B%7D&mode=%7B%7D&shippedHazardousGoods=%7B%7D&start=%7B%7D",
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
            "description": "*Request an ordered list of destinations for a truck carrying hazardous materials*\n\nWaypoint sequence calcuations are made using the `findsequence` endpoint and appending  `start` and `end` parameters and consecutively numbered `destination` parameters are used to add intermediate points  to the request. Hazardous material types are added as a comma-delimited list to the  `shippedHazardousGoods` parameter. The list of values is defined in the Enterprise Routing API\n\n\n\n* **start**  `latlng`\n \\- Start point for the route calculations.    e.g. `52.515,13.377`\n\n* **destination1**  `latlng`\n \\- A point through which the route must pass.    e.g. `52.6172,13.3833`\n\n* **destination2**  `latlng`\n \\- A point through which the route must pass.    e.g. `52.6172,13.3833`\n\n* **destination3**  `latlng`\n \\- A point through which the route must pass.    e.g. `52.6172,13.3833`\n\n* **destination4**  `latlng`\n \\- A point through which the route must pass.    e.g. `52.6172,13.3833`\n\n* **end**  `latlng`\n \\- End point for the route calculations.    e.g. `50.121,8.925`\n\n* **improveFor**  `enum`\n \\- Whether to improve for time or distance\n\n Valid values are : `time`, `distance`\n\n* **mode**  `text`\n \\- Routing mode determines how the route is calculated.    e.g. `fastest;car;traffic:disabled`\n\n* **shippedHazardousGoods**  `multi-enum`\n \\- Truck routing only, list of hazardous materials in the vehicle.\n\n Valid values are : `combustible`, `corrosive`, `explosive`, `flammable`, `gas`, `harmfulToWater`, `organic`, `other`, `poison`, `poisonousInhalation`, `radioActive`\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40463824-7938-460e-be2e-3414ea42a50f"
            }
          ]
        }
      ]
    }
  ]
}