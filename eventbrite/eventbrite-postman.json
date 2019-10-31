{
  "info": {
    "name": "Eventbrite Get Payment Update",
    "_postman_id": "8cca8f89-441d-44f0-8a6a-ad46bbb9a5ef",
    "description": "This method creates or updates the payment options for this event. Only the fields passed as arguments will be modified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Checkout",
      "item": [
        {
          "id": "abde1161-9393-42e9-bdd9-7700bf6e1aa0",
          "name": "getCheckoutSettingsMethods",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/checkout_settings/methods/?country=%7B%7D&currency=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the available checkout methods to do payments given a country and a currency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ecfa5d3-97a2-4686-ae85-7ffe31631413"
            }
          ]
        }
      ]
    },
    {
      "name": "Media",
      "item": [
        {
          "id": "c6e7b05a-d1be-4319-a85f-6185e7e9c84c",
          "name": "getMedia",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "media/:id/"
              ],
              "query": [
                {
                  "key": "height",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "width",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
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
            "description": "Return an image for a given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a7ebe62-21f6-43fb-8c8b-4b7e12d8c5bd"
            }
          ]
        },
        {
          "id": "f02aef53-9d9b-4cb6-ac59-e36acbe81763",
          "name": "getMediaUpload",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/media/upload/?type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "See Media Uploads."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "701d64c4-5842-4073-8155-567e591efac6"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "5717de9c-8b70-4620-9c07-25fddbfc6dfb",
          "name": "getUsersMeNotifications",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/users/me/notifications/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a paginated response of notification objects for a determined user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47e479dc-105e-41dc-af8a-6a50aad0fbfa"
            }
          ]
        },
        {
          "id": "34d1e833-0435-42a7-9723-c21b47268c5f",
          "name": "getUsersAssortment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "users/:id/assortment/"
              ],
              "variable": [
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
            "description": "Retrieve the assortment for the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1eff00ff-59c3-4edb-ba3e-cc99273fd1d7"
            }
          ]
        },
        {
          "id": "2783c2df-3da7-4e90-8add-b6afea1f7086",
          "name": "postUsersAssortment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "users/:id/assortment/"
              ],
              "query": [
                {
                  "key": "plan",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Set a user&#8217;s assortment and returns the assortment for the specified\nuser."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "997febbe-a6b4-4c58-bdb9-f172a5fd040b"
            }
          ]
        }
      ]
    },
    {
      "name": "System",
      "item": [
        {
          "id": "ebc9d69f-a9c4-4352-ac1f-79dc0278be2e",
          "name": "getSystemTimezones",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/system/timezones/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a paginated response with a key of timezones,\ncontaining a list of timezones."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5cceec8-6e9a-4aaa-96db-9d07d68dfb67"
            }
          ]
        }
      ]
    },
    {
      "name": "Payment",
      "item": [
        {
          "id": "7bcd174c-f162-427c-a3e9-d061ef335930",
          "name": "Get_payment_update_",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/payment_update?accept_cash=%7B%7D&accept_check=%7B%7D&accept_google=%7B%7D&accept_invoice=%7B%7D&accept_paypal=%7B%7D&data-type=%7B%7D&event_id=%7B%7D&google_merchant_id=%7B%7D&google_merchant_key=%7B%7D&instructions_cash=%7B%7D&instructions_check=%7B%7D&instructions_invoice=%7B%7D&paypal_email=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method creates or updates the payment options for this event. Only the fields passed as arguments will be modified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e40f1fd-6e70-4a59-9456-a3c16aa08abd"
            }
          ]
        }
      ]
    }
  ]
}