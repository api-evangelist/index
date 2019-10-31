{
  "info": {
    "name": "BMC Software API List Actions",
    "_postman_id": "34a385df-4c8e-4765-af41-ac8fd8893a74",
    "description": "List of all Actions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Actions",
      "item": [
        {
          "id": "7843d7c6-4e2d-4b32-b3c8-c77190dba83a",
          "name": "get-all-available-action-types",
          "request": {
            "url": "http://example.com/api/v1/actions",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all known action types"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88cd431d-bf08-4464-bc78-3faa55888835"
            }
          ]
        },
        {
          "id": "7d89a40e-4e2b-4759-9455-a70dfab6259a",
          "name": "get-all-installed-actions",
          "request": {
            "url": "http://example.com/api/v1/actions/installed",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all actions that are installed for the project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f88ca5c5-c798-4d74-8d27-c113cd581320"
            }
          ]
        },
        {
          "id": "3decdd30-05b4-495d-80bf-4effaa76a47b",
          "name": "install-action",
          "request": {
            "url": "http://example.com/api/v1/actions/installed",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Installs an action"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e7bf9e7-68df-49c4-a6eb-9a20a676fe22"
            }
          ]
        },
        {
          "id": "b80f0c44-e36c-4ece-b56c-a8d1028f5b13",
          "name": "get-details-of-an-installed-action",
          "request": {
            "url": "http://example.com/api/v1/actions/installed/:actionId?actionId\nName of plugin=actionId%0AName%20of%20plugin",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a single action definition"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e282d399-3433-42e6-93df-0ce41c35ecdf"
            }
          ]
        },
        {
          "id": "f5e1a9e2-5b43-4fb7-8031-f63f199c8125",
          "name": "uninstall-action",
          "request": {
            "url": "http://example.com/api/v1/actions/installed/:actionId",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Uninstalls an action and remove it from the associated alarms(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c7547f5-0f8e-430d-a64e-d58cbcfed636"
            }
          ]
        },
        {
          "id": "13b09df0-2925-4ac1-9fa4-a3fb9ced3c40",
          "name": "get-all-alarms-using-an-action",
          "request": {
            "url": "http://example.com/api/v1/actions/installed/:actionId/alarms",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get alarms that are using this action installed for the project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2df1b046-902d-4e51-99b4-797996ec2fbc"
            }
          ]
        },
        {
          "id": "29b77e23-1037-42f1-a393-740c0f59730e",
          "name": "get-action",
          "request": {
            "url": "http://example.com/api/v1/actions/:action?action\nName of plugin=action%0AName%20of%20plugin",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a single action type"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8084058c-bc31-4da9-80a7-1998399963f2"
            }
          ]
        },
        {
          "id": "3f9c2372-2afe-4b2e-8c04-4bdf0ead5dbc",
          "name": "list-actions",
          "request": {
            "url": "http://example.com/api/actions?maintenance_id\n        \n        \n            string\n            Unique ID generated by the server. This can be used as an identifier.\n        \n                \n    \n        \n        display_name\n        \n        \n            string\n            Displa=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of all Actions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc69e889-8749-4a5f-bf73-965cc1b7372f"
            }
          ]
        },
        {
          "id": "5911fbc4-999b-4b97-ad91-bd9b5dcdea58",
          "name": "create-action",
          "request": {
            "url": "http://example.com/api/actions?action_name\n        \n        \n            required\n            Display name for the Action.\n        \n    \n    \n        \n        action_url\n        \n        \n            required\n            URL to be invoked for action execution.=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new Action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7c290ef-086e-4918-8f16-aaf35e21b387"
            }
          ]
        },
        {
          "id": "0d833356-fe6d-4127-99d3-d397b2d125b2",
          "name": "update-action",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "actions/:action_id"
              ],
              "query": [
                {
                  "key": "action_name\n        \n        \n            required\n            Display name for the Action.\n        \n    \n    \n        \n        action_url\n        \n        \n            required\n            URL to be invoked for action execution.",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "action_id",
                  "value": "action_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update an existing Action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71560519-cc6c-4948-910d-0e2919d8b043"
            }
          ]
        }
      ]
    }
  ]
}