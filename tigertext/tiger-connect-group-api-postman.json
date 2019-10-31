{
  "info": {
    "name": "Tiger Connect Group API Remove members from a group.",
    "_postman_id": "8fff48e2-f84b-48fa-a992-2759d83f14d0",
    "description": "Remove members from a group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "cbdd2aff-2648-4acf-ac1e-3306a9e693a5",
      "name": "createNewGroup",
      "request": {
        "url": "http://developer.tigertext.me/v2/group/?avatar=%7B%7D",
        "method": "POST",
        "body": {
          "mode": "urlencoded",
          "urlencoded": [
            {
              "key": "members",
              "value": "{}",
              "disabled": false,
              "description": "The members to add to the group encoded using user address encoding"
            },
            {
              "key": "name",
              "value": "{}",
              "disabled": false,
              "description": "The group name"
            },
            {
              "key": "replay_history",
              "value": "{}",
              "disabled": false,
              "description": "A boolean value indicating if, when a new member is added to the group, it should get the messages sent to the group before that"
            },
            {
              "key": "TT-X-Organization-Key",
              "value": "{}",
              "disabled": false,
              "description": "The organization in which the user wants to create the group"
            }
          ]
        },
        "description": "Create a new group."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "41b00951-df25-47a1-97ac-ebb207b906b0"
        }
      ]
    },
    {
      "id": "5b83c476-bfac-4f52-9cdb-f93f0b6fa5b6",
      "name": "deleteGroup",
      "request": {
        "url": {
          "protocol": "http",
          "host": "developer.tigertext.me",
          "path": [
            "v2",
            "group/:group_token/"
          ],
          "variable": [
            {
              "id": "group_token",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "DELETE",
        "body": {
          "mode": "raw"
        },
        "description": "Delete a group. If the group has already been deleted, no error is reported."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "9f4d2e45-ce14-4d53-8500-f0d007bbf2d2"
        }
      ]
    },
    {
      "id": "f16f7f02-8812-45a3-aaaf-075cfe08767f",
      "name": "addGroupMember",
      "request": {
        "url": {
          "protocol": "http",
          "host": "developer.tigertext.me",
          "path": [
            "v2",
            "group/:group_token/members/"
          ],
          "variable": [
            {
              "id": "group_token",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "POST",
        "body": {
          "mode": "urlencoded",
          "urlencoded": [
            {
              "key": "members",
              "value": "{}",
              "disabled": false,
              "description": "A list of members to add to a group using user address encoding"
            }
          ]
        },
        "description": "Add members to a group."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "1f148c7d-ae77-4aa0-b768-aa4d251bb2f0"
        }
      ]
    },
    {
      "id": "83b7ca74-7e38-4790-a96e-436b5791cb1d",
      "name": "removeMemberFromGroup",
      "request": {
        "url": {
          "protocol": "http",
          "host": "developer.tigertext.me",
          "path": [
            "v2",
            "group/:group_token/members/remove/"
          ],
          "variable": [
            {
              "id": "group_token",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "POST",
        "body": {
          "mode": "urlencoded",
          "urlencoded": [
            {
              "key": "members",
              "value": "{}",
              "disabled": false,
              "description": "A list of members to remove from a group using address encoding"
            }
          ]
        },
        "description": "Remove members from a group."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "d3557903-c825-49cb-a389-d6f3c6eb0c40"
        }
      ]
    }
  ]
}