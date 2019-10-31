{
  "info": {
    "name": "ThingPark DX Admin API Profile Retrieval",
    "_postman_id": "d1243e7b-e364-4271-b112-9a8da7f82a9d",
    "description": "Retrieves the profile corresponding to the provided profile Id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Token",
      "item": [
        {
          "id": "6a37d9a7-93a3-40bc-902f-95025a9ff01d",
          "name": "generates-and-retrieves-a-token-for-a-client",
          "request": {
            "url": "http://dx-api.thingpark.com/admin/v140/api/oauth/token?renewToken=%7B%7D&validityPeriod=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "client_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "Id of the client"
                },
                {
                  "key": "client_secret",
                  "value": "{}",
                  "disabled": false,
                  "description": "Secret of the client"
                },
                {
                  "key": "grant_type",
                  "value": "{}",
                  "disabled": false,
                  "description": "Type of the OAuth2 grant workflow"
                }
              ]
            },
            "description": "Generates and retrieves a token for a client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa1ef4b0-0bb2-4ac3-89ff-919d78c4a4c4"
            }
          ]
        },
        {
          "id": "c0a32996-657e-4967-8749-42a6b9868888",
          "name": "revokes-a-token",
          "request": {
            "url": "http://dx-api.thingpark.com/admin/v140/api/oauth/revoke_token?access_token=%7B%7D",
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
            "description": "Revokes a token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bcf3e4ea-71c0-469e-ac0c-318d0e1eab09"
            }
          ]
        },
        {
          "id": "2f027c75-ccd5-4283-ae23-b2cbf87b983f",
          "name": "retrieves-information-about-a-valid-token",
          "request": {
            "url": "http://dx-api.thingpark.com/admin/v140/api/oauth/tokeninfo?access_token=%7B%7D",
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
            "description": "Retrieves information about a valid token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "712eaf6d-fbeb-4b1d-b039-96ba9030cf59"
            }
          ]
        }
      ]
    },
    {
      "name": "Profiles",
      "item": [
        {
          "id": "30de1a30-73a6-4352-8370-fb919654b37e",
          "name": "retrieves-all-available-profiles-by-default-only-retrieves-actilityowned-profiles",
          "request": {
            "url": "http://dx-api.thingpark.com/admin/v140/api/profiles",
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
            "description": "Retrieves all available profiles. By default only retrieves ACTILITY-owned profiles."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5be92114-49fd-4f65-b2ee-b25431150e36"
            }
          ]
        }
      ]
    },
    {
      "name": "Profile",
      "item": [
        {
          "id": "bb47c797-2f49-40a0-bb12-19bac94f783c",
          "name": "retrieves-the-profile-corresponding-to-the-provided-profile-id",
          "request": {
            "url": {
              "protocol": "http",
              "host": "dx-api.thingpark.com",
              "path": [
                "admin",
                "v140",
                "api",
                "profiles/:profileId"
              ],
              "variable": [
                {
                  "id": "profileId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Retrieves the profile corresponding to the provided profile Id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ae7385c-01ab-4ec5-999f-fde8a7875678"
            }
          ]
        }
      ]
    }
  ]
}