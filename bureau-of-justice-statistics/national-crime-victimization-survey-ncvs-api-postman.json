{
  "info": {
    "name": "National Crime Victimization Survey (NCVS) API Get Personal Year",
    "_postman_id": "f070bd76-d922-493e-a432-06b3f04b17d3",
    "description": "Returns the personal counts of reported incidents.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Personal",
      "item": [
        {
          "id": "b36ad7d5-b7c5-44b8-8418-07e4c69eb97e",
          "name": "getV2PersonalFields",
          "request": {
            "url": "http://www.bjs.gov/bjs/ncvs/v2/personal/fields/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a description of the fields/columns used returned in the personal data sets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06e9229d-5641-40ba-b61a-2b9bf2362de9"
            }
          ]
        },
        {
          "id": "5a148768-0c74-4a36-862f-f5524dff9956",
          "name": "getV2PersonalPopulationYear",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.bjs.gov",
              "path": [
                "bjs",
                "ncvs",
                "v2/personal/population/:year"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "year",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the personal population of reported incidents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1189084d-dbbc-49fa-8bfb-f6ffc4a0d973"
            }
          ]
        },
        {
          "id": "9b755c26-04b0-4fbc-b8bc-bf195ae72103",
          "name": "getV2PersonalYear",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.bjs.gov",
              "path": [
                "bjs",
                "ncvs",
                "v2/personal/:year"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "year",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the personal counts of reported incidents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b1104ac-4ad0-464e-b206-229eb9f74291"
            }
          ]
        }
      ]
    }
  ]
}