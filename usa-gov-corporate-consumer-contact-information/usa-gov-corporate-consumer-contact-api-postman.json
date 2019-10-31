{
  "info": {
    "name": "USA.Gov Corporate Consumer Contact API Get Contact",
    "_postman_id": "a7931a3d-a792-4487-bc39-b03563a56f3f",
    "description": "The Contact call will let you access an individual corporation's information by including its unique identifier in the call.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "contacts",
      "item": [
        {
          "id": "7232aaf1-b3c5-45bf-a339-929da5d5747c",
          "name": "getContact",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.usa.gov",
              "path": [
                "api",
                "USAGovAPI",
                "contacts.:format/contacts/:id"
              ],
              "variable": [
                {
                  "id": "format",
                  "value": "format",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The Contact call will let you access an individual corporation's information by including its unique identifier in the call"
          },
          "response": [
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "[\r\n  {\r\n    \"Id\": \"Id\",\r\n    \"Name\": \"Name\",\r\n    \"Description\": \"Description\",\r\n    \"Subdivision\": \"Subdivision\",\r\n    \"Street1\": \"Street1\",\r\n    \"Street2\": \"Street2\",\r\n    \"City\": \"City\",\r\n    \"StateTer\": \"StateTer\",\r\n    \"Zip\": \"Zip\",\r\n    \"Email\": \"Email\"\r\n  }\r\n]",
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "d9990832-4343-42da-9122-9e644115b82e"
            }
          ]
        }
      ]
    }
  ]
}