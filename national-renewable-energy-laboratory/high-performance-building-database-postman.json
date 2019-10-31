{
  "info": {
    "name": "High Performance Building Database Get Project Details",
    "_postman_id": "0db1234f-3ad0-499b-a459-ff7d3657bd9e",
    "description": "This API allows users to request metadata associated with the specific Document.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "3d42e2fc-7c6b-454f-b986-52b79b1a33bf",
          "name": "getProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.nrel.gov",
              "path": [
                "api",
                "building-case-studies",
                "project.:output_format"
              ],
              "query": [
                {
                  "key": "city",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "portal",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "province",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "region",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "search",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "output_format",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Projects"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e94d54ab-526f-4ad3-9468-82e932585dbb"
            }
          ]
        },
        {
          "id": "803af70f-36aa-4759-9349-34bd699e78da",
          "name": "document",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.nrel.gov",
              "path": [
                "api",
                "building-case-studies",
                "project/:project_id.:output_format"
              ],
              "variable": [
                {
                  "id": "output_format",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "project_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API allows users to request metadata associated with the specific Document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18969f3e-2e46-4820-a5e8-3cb9dfb69807"
            }
          ]
        }
      ]
    }
  ]
}