{
  "info": {
    "name": "HERE Batch Geocoder API Add Jobs",
    "_postman_id": "0f61b4ce-c76a-4b91-b666-f5e0b1d4cb43",
    "description": "* Start asynchronously geocoding a large set of addresses in one batch*\n\nSubmit an HTTP POST request with `action=run` and attach the input data to the body. \n  \n\n\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible behavior in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.\n\n* **action**  `enum`\n \\- Type of request\n\n Valid values are : `cancel`, `run`, `status`\n\n* **mailto**  `text`\n \\- Email address where completion notification is sent.\n\n* **header**  `enum`\n \\- If `true`, a header row is included before the results in the output.  \n\n Valid values are : `false`, `true`\n\n* **indelim**  `text`\n \\- \n\n* **outdelim**  `text`\n \\- \n\n* **outcols**  `text`\n \\- \n\n* **outputCombined**  `enum`\n \\- \n\n Valid values are : `true`, `false`",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Job",
      "item": [
        {
          "id": "6ee94557-6d70-4a70-bd99-7ecc114c2163",
          "name": "getJob",
          "request": {
            "url": "http://batch.geocoder.cit.api.here.com/6.2/jobs/puwWrv32YOU24y8MNoUr793chFAI36aC?action=%7B%7D&app_code=%7B%7D&app_id=%7B%7D",
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
            "description": "*Request the status of a batch geocoder job*\n\nTo check the status, make a request to the `jobs` endpoint  appending the `requestId` and using the parameter `action=status `\n  \n\n\n\n* **action**  `enum`\n \\- Type of request  \n\n Valid values are : `cancel`, `runs`, `status`\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.  \n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75e1bd01-fb46-4318-850e-6d4f514913d7"
            }
          ]
        },
        {
          "id": "fcc008b1-b7f3-4b43-a717-2803c48ba2fd",
          "name": "addJob",
          "request": {
            "url": "http://batch.geocoder.cit.api.here.com/6.2/jobs?action=%7B%7D&app_code=%7B%7D&app_id=%7B%7D&gen=%7B%7D&header=%7B%7D&indelim=%7B%7D&mailto=%7B%7D&outcols=%7B%7D&outdelim=%7B%7D&outputCombined=%7B%7D",
            "method": "POST",
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
            "description": "* Start asynchronously geocoding a large set of addresses in one batch*\n\nSubmit an HTTP POST request with `action=run` and attach the input data to the body. \n  \n\n\n\n* **gen**  `number`\n \\- Enables/disables backward incompatible behavior in the API\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.\n\n* **action**  `enum`\n \\- Type of request\n\n Valid values are : `cancel`, `run`, `status`\n\n* **mailto**  `text`\n \\- Email address where completion notification is sent.\n\n* **header**  `enum`\n \\- If `true`, a header row is included before the results in the output.  \n\n Valid values are : `false`, `true`\n\n* **indelim**  `text`\n \\- \n\n* **outdelim**  `text`\n \\- \n\n* **outcols**  `text`\n \\- \n\n* **outputCombined**  `enum`\n \\- \n\n Valid values are : `true`, `false`"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a25dfda4-b731-44e9-b00c-38f1797b589b"
            }
          ]
        }
      ]
    }
  ]
}