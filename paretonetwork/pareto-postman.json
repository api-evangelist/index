{
  "info": {
    "name": "Pareto Upload image",
    "_postman_id": "189c9d91-11a0-4dc6-928c-3ea9552ff07d",
    "description": "Upload Image",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sign",
      "item": [
        {
          "id": "a8019561-3115-4644-a2b0-56376eef599b",
          "name": "postSign",
          "request": {
            "url": "{{default}}/sign",
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
            "description": "Test the hash between a message and public key. If the test is passed, a cookie is stored. The parameters of this request are gotten from MetaMask"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9277312e-72ce-426f-a291-4cec41603bf7"
            }
          ]
        }
      ]
    },
    {
      "name": "Rank",
      "item": [
        {
          "id": "7b9e95bb-7203-43ba-bd67-8da62660ab32",
          "name": "getRank",
          "request": {
            "url": "{{default}}/rank",
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
            "description": "Get all the addresses sorted by rank. The ranking is gotten from the Ethereum score"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2888b92-9ef2-4879-a9a5-bb6cdcc86092"
            }
          ]
        }
      ]
    },
    {
      "name": "Auth",
      "item": [
        {
          "id": "00ec07bd-c171-420c-a0a8-e35ba7b36826",
          "name": "getAuth",
          "request": {
            "url": "{{default}}/auth",
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
            "description": "Simple authenticated method to determine if user is properly authenticated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a33d416-341f-479b-9d58-89bb360cc7fd"
            }
          ]
        }
      ]
    },
    {
      "name": "Unsign",
      "item": [
        {
          "id": "936b13ae-0d6c-40d6-a28a-872da51d3553",
          "name": "postUnsign",
          "request": {
            "url": "{{default}}/unsign",
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
            "description": "Manage unsign proccess. Delete cookie with header set-cookie"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "45260a23-eb33-4db2-a196-a717bc8ede99"
            }
          ]
        }
      ]
    },
    {
      "name": "Address",
      "item": [
        {
          "id": "b67a8a04-ae5e-480f-975c-dcfda97f36a8",
          "name": "getAddress",
          "request": {
            "url": "{{default}}/address",
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
            "description": "Get the information of the current user. The current user is fetched using the auth cookie."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba1f096c-b656-4caf-a95e-a40ae24189ba"
            }
          ]
        },
        {
          "id": "3e2690ab-bef8-4d2f-ad91-0036eb24b728",
          "name": "getAddressAddress",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "address/:address"
              ],
              "variable": [
                {
                  "id": "address",
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
            "description": "Get the information of a specific user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "863835c8-3b11-417b-a672-cf3c2aed366b"
            }
          ]
        }
      ]
    },
    {
      "name": "Content",
      "item": [
        {
          "id": "5f2b35a1-3c1e-45a4-9e4a-149125f97135",
          "name": "getContent",
          "request": {
            "url": "{{default}}/content",
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
            "description": "Get all available content about the actionable investing intels."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "abc48079-7124-4d16-b5cb-6e2d212c1d8e"
            }
          ]
        },
        {
          "id": "5e16767a-89dc-4065-8d78-d99e6536ce41",
          "name": "getContentMe",
          "request": {
            "url": "{{default}}/content/me",
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
            "description": "Get the content available for current user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e1fa3a8-e934-483c-ac8c-8214ef52f474"
            }
          ]
        }
      ]
    },
    {
      "name": "Userinfo",
      "item": [
        {
          "id": "43d8cb21-47d1-4bb6-b2ff-c0cedc5c2e64",
          "name": "getUserinfo",
          "request": {
            "url": "{{default}}/userinfo?latest=%7B%7D",
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
            "description": "Get the information of the current user. The current user is fetched using the auth cookie."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a572ce7a-ecee-4013-b3cd-81d6d9ea2d66"
            }
          ]
        },
        {
          "id": "bb5eae97-b956-415f-a8f8-4d353c8575c9",
          "name": "getUserinfoAddress",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "userinfo/:address"
              ],
              "variable": [
                {
                  "id": "address",
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
            "description": "Get the profile of a specific user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3046e3cb-c7f4-4948-9922-383ef51ab890"
            }
          ]
        }
      ]
    },
    {
      "name": "Updateuser",
      "item": [
        {
          "id": "d16e02c6-94a7-49a7-9dec-4c22cc701150",
          "name": "postUpdateuser",
          "request": {
            "url": "{{default}}/updateuser",
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
            "description": "Update the profile of the current user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6186250-0d48-483e-a160-f05818bed462"
            }
          ]
        }
      ]
    },
    {
      "name": "Profile",
      "item": [
        {
          "id": "97377674-b461-4c80-bae8-f3b064ffff36",
          "name": "getProfileImage",
          "request": {
            "url": "{{default}}/profile-image?image=%7B%7D",
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
            "description": "Get the image profile"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8c59fc3-2cc3-418d-8512-07ef50e6f0b6"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "cda261aa-3fe7-454f-b104-1ed1f45c2c89",
          "name": "postUploadProfile",
          "request": {
            "url": "{{default}}/upload-profile",
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
            "description": "Upload Image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3aaf182-1f49-4ea6-ba32-b2f53081ae3f"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/"
    }
  ]
}