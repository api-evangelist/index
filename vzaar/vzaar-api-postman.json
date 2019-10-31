{
  "info": {
    "name": "Vzaar API Get Api Username Videos",
    "_postman_id": "38f5a3f3-ecf9-477c-af41-9685d381ae90",
    "description": "nnThis API call returns a list of the users active videos along with its relevant metadata. 20 videos are returned by default but this is customisable.nn",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Api",
      "item": [
        {
          "id": "499a1810-7861-4dfd-a1ed-a0b47fbb89ef",
          "name": "getApiUsersUsername.Format",
          "request": {
            "url": {
              "protocol": "http",
              "host": "vzaar.com",
              "path": [
                "api/users/:username.json"
              ],
              "query": [
                {
                  "key": "username is the vzaar login name for the user. Note: This must be the actual username and not the email address",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "username",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "nnThis API call returns the users public details along with its relevant metadata.nn"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0bd210c0-1032-4855-b6e0-6cf41426af38"
            }
          ]
        },
        {
          "id": "4b8072c0-3466-44f4-ac03-38151c0866c7",
          "name": "getApiUsernameVeos.xml",
          "request": {
            "url": {
              "protocol": "http",
              "host": "vzaar.com",
              "path": [
                "api/:username/videos.xml"
              ],
              "query": [
                {
                  "key": "count,",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page,",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort,",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "status,",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title,",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "username is the vzaar login name for the user. Note: This must be the actual username and not the email address",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "username",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "nnThis API call returns a list of the users active videos along with its relevant metadata. 20 videos are returned by default but this is customisable.nn"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "268486cb-e95a-444d-a546-4622992ef160"
            }
          ]
        }
      ]
    }
  ]
}