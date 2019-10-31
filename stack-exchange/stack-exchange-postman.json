{
  "info": {
    "name": "Stack Exchange Get User Write Permissions",
    "_postman_id": "e65a13fa-4b06-4615-940b-58967cbbfe58",
    "description": "Returns the write permissions a user has via the api.\n \nThe Stack Exchange API gives users the ability to create, edit, and delete certain types. This method returns whether the passed user is capable of performing those actions at all, as well as how many times a day they can.\n \nThis method does not consider the user's current quota (ie. if they've already exhausted it for today) nor any additional restrictions on write access, such as editing deleted comments.\n \nThis method returns a list of write_permissions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "write permissions",
      "item": [
        {
          "id": "e8b0f021-ab82-47c8-ab51-836ab4b439e6",
          "name": "returns-the-write-permissions-a-user-has-via-the-api-the-stack-exchange-api-gives-users-the-ability-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stackexchange.com",
              "path": [
                "2.2",
                "users/:id/write-permissions"
              ],
              "query": [
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pagesize",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "site",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the write permissions a user has via the api"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2f83200-c539-4570-a9df-7ad10626c2d8"
            }
          ]
        }
      ]
    }
  ]
}