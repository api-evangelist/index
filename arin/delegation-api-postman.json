{
  "info": {
    "name": "Delegation API Delete Delegation",
    "_postman_id": "8f3e2d27-4c59-454a-983d-ed53e9321f2e",
    "description": "This call will delete the single nameserver specified in your URL from the Delegation specified in your URL, and return a payload containing that Delegation's information after the nameserver has been deleted.  If Reg-RWS returns an error code and/or Error Payload to you when performing this call, refer to the Error Codes section.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Delegation",
      "item": [
        {
          "id": "eef1d042-7fe5-48fa-a6e8-b74a21cc17c3",
          "name": "getDelegation",
          "request": {
            "url": "http://www.arin.net/regrws/core/v1/delegation",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This call will return a payload containing details about the Delegation specified in your URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "502abca0-34c9-4886-8526-1a8143c890aa"
            }
          ]
        },
        {
          "id": "7609ecbb-3189-40b3-8a4f-86e5a0e66437",
          "name": "updateDelegation",
          "request": {
            "url": "http://www.arin.net/regrws/core/v1/delegation",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "This call will modify the details of the Delegation specified in your URL. When making this call, attach a Delegation Payload containing the details of the Delegation you intend to modify. To ensure accuracy, use Get Delegation to get the most current information before making changes. This call returns a payload containing that Delegation's information as it exists after modification."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4edc0f9-5228-49f0-88ad-418184620d53"
            }
          ]
        },
        {
          "id": "b1bcd91f-1536-4575-b6da-5afacfbf03de",
          "name": "addDelegation",
          "request": {
            "url": "http://www.arin.net/regrws/core/v1/delegation",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "This call will add the single nameserver specified in your URL to the Delegation specified in your URL, and return a payload containing that Delegation's information after the nameserver has been added."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "567d5329-f9f9-4a03-8f36-83d6733964fc"
            }
          ]
        },
        {
          "id": "8e31b4e1-2cbd-46b4-9cce-46256a126e38",
          "name": "deleteDelegation",
          "request": {
            "url": "http://www.arin.net/regrws/core/v1/delegation",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "This call will delete the single nameserver specified in your URL from the Delegation specified in your URL, and return a payload containing that Delegation's information after the nameserver has been deleted.  If Reg-RWS returns an error code and/or Error Payload to you when performing this call, refer to the Error Codes section."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8dddc798-2390-48eb-a012-5f2d3973bade"
            }
          ]
        }
      ]
    }
  ]
}