{
  "info": {
    "name": "FlowRoute API List Inbound Routes",
    "_postman_id": "32859e0e-8473-4d35-b25a-1e959a108f49",
    "description": "Returns a list of your inbound routes. From the list, you can then select routes to use as the primary and failover routes for a phone number, which you can do via \"Update Primary Voice Route for a Phone Number\" and \"Update Failover Voice Route for a Phone Number\".",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Messaging",
      "item": [
        {
          "id": "ca4f46c2-987a-41af-8228-2ec7a6d4ce3c",
          "name": "retrieves-a-list-of-message-detail-records-mdrs-within-a-specified-date-range-date-and-time-is-based",
          "request": {
            "url": "{{default}}/v2.1/messages?end_date=%7B%7D&limit=%7B%7D&offset=%7B%7D&start_date=%7B%7D",
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
            "description": "Retrieves a list of Message Detail Records (MDRs) within a specified date range. Date and time is based on Coordinated Universal Time (UTC)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd0245ae-20a4-44f7-8ba9-b45a5ad33ae6"
            }
          ]
        },
        {
          "id": "6a89b870-c2e9-4f26-8dac-815e9c6e0241",
          "name": "sends-an-sms-or-mms-from-a-flowroute-long-code-or-tollfree-phone-number-to-another-valid-phone-numbe",
          "request": {
            "url": "{{default}}/v2.1/messages",
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
            "description": "Sends an SMS or MMS from a Flowroute long code or toll-free phone number to another valid phone number."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95c76d7b-99f4-48d4-aa38-7696bef5d3d9"
            }
          ]
        },
        {
          "id": "2fbc85dd-851f-4426-b39f-40b7e68103a6",
          "name": "searches-for-a-specific-message-record-id-and-returns-a-message-detail-record-in-mdr2-format",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "v2.1/messages/:id"
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
            "description": "Searches for a specific message record ID and returns a Message Detail Record (in MDR2 format)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "134e4951-b4a8-41c6-8f8d-07b50b75be65"
            }
          ]
        },
        {
          "id": "9d1040d3-e229-497e-94e4-1f66c7c94862",
          "name": "returns-a-list-of-all-phone-numbers-currently-on-your-flowroute-account-the-response-includes-detail",
          "request": {
            "url": "{{default}}/v2/numbers?contains=%7B%7D&ends_with=%7B%7D&limit=%7B%7D&offset=%7B%7D&starts_with=%7B%7D",
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
            "description": "Returns a list of all phone numbers currently on your Flowroute account. The response includes details such as the phone number's rate center, state, number type, and whether CNAM Lookup is enabled for that number."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5084b069-e337-4ccf-a8a0-482c491f896c"
            }
          ]
        },
        {
          "id": "5cc66d9b-8d3f-4c72-981c-4da9d4ad9286",
          "name": "lists-all-of-the-information-associated-with-any-of-the-phone-numbers-in-your-account-including-bill",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "v2/numbers/:id"
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
            "description": "Lists all of the information associated with any of the phone numbers in your account, including billing method, primary voice route, and failover voice route."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7af17693-b1ad-4f78-b611-cb5fc4e31671"
            }
          ]
        },
        {
          "id": "2d270a26-656e-458b-8f80-53f7e73d0e48",
          "name": "lets-you-purchase-a-phone-number-from-available-flowroute-inventory",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "v2/numbers/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Lets you purchase a phone number from available Flowroute inventory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7996305c-0e90-4380-8a8d-9c9913b1f890"
            }
          ]
        },
        {
          "id": "acbe4afb-b5c5-47e1-8ad8-86b9cf6b2cfe",
          "name": "this-endpoint-lets-you-search-for-phone-numbers-by-state-or-rate-center-or-by-your-specified-search-",
          "request": {
            "url": "{{default}}/v2/numbers/available?contains=%7B%7D&ends_with=%7B%7D&limit=%7B%7D&offset=%7B%7D&rate_center=%7B%7D&starts_with=%7B%7D&state=%7B%7D",
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
            "description": "This endpoint lets you search for phone numbers by state or rate center, or by your specified search value."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2426869-1581-4ea8-994c-75296aa74062"
            }
          ]
        },
        {
          "id": "dc7f842a-0f0b-4efe-81e6-ac2ce8cde291",
          "name": "returns-a-list-of-all-numbering-plan-area-npa-codes-containing-purchasable-phone-numbers",
          "request": {
            "url": "{{default}}/v2/numbers/available/areacodes?limit=%7B%7D&max_setup_cost=%7B%7D&offset=%7B%7D",
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
            "description": "Returns a list of all Numbering Plan Area (NPA) codes containing purchasable phone numbers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1edd6b9-4b04-4f12-80ad-a89a5488786a"
            }
          ]
        },
        {
          "id": "9509fb88-378c-4ce3-99e1-cdef793e7e77",
          "name": "returns-a-list-of-all-central-office-exchange-codes-containing-purchasable-phone-numbers",
          "request": {
            "url": "{{default}}/v2/numbers/available/exchanges?areacode=%7B%7D&limit=%7B%7D&max_setup_cost=%7B%7D&offset=%7B%7D",
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
            "description": "Returns a list of all Central Office (exchange) codes containing purchasable phone numbers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff2fc4f1-3755-4340-ab80-56727fd8c32f"
            }
          ]
        },
        {
          "id": "bbc92cfe-c38e-4b1b-b0c4-b47b4ab556e6",
          "name": "use-this-endpoint-to-update-the-primary-voice-route-for-a-phone-number-you-must-create-the-route-fir",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "v2/numbers/:number_id/relationships/primary_route"
              ],
              "variable": [
                {
                  "id": "number_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
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
            "description": "Use this endpoint to update the primary voice route for a phone number. You must create the route first by following \"Create an Inbound Route\". You can then assign the created route by specifying its value in a PATCH request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1427220-7d0d-40ac-8a9c-2a4d91dfd06f"
            }
          ]
        },
        {
          "id": "2b93ddf3-3541-46f3-b67f-398f9eb09e67",
          "name": "use-this-endpoint-to-update-the-failover-voice-route-for-a-phone-number-you-must-create-the-route-fi",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "v2/numbers/:number_id/relationships/failover_route"
              ],
              "variable": [
                {
                  "id": "number_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
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
            "description": "Use this endpoint to update the failover voice route for a phone number. You must create the route first by following \"Create an Inbound Route\". You can then assign the created route by specifying its value in a PATCH request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7deb3d29-6d0e-4220-865f-d5d84770f7e3"
            }
          ]
        },
        {
          "id": "46861089-e365-4584-8989-dded9d47c9df",
          "name": "returns-a-list-of-your-inbound-routes-from-the-list-you-can-then-select-routes-to-use-as-the-primary",
          "request": {
            "url": "{{default}}/v2/routes?limit=%7B%7D&offset=%7B%7D&route_type=%7B%7D",
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
            "description": "Returns a list of your inbound routes. From the list, you can then select routes to use as the primary and failover routes for a phone number, which you can do via \"Update Primary Voice Route for a Phone Number\" and \"Update Failover Voice Route for a Phone Number\"."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3ed018a-17c8-442c-abf0-11f7659b9bec"
            }
          ]
        },
        {
          "id": "5c1a1eaa-c8ad-4a1d-accb-8d83ab987a37",
          "name": "creates-a-new-inbound-route-which-can-then-be-associated-with-phone-numbers-please-see-list-inbound-",
          "request": {
            "url": "{{default}}/v2/routes",
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
            "description": "Creates a new inbound route which can then be associated with phone numbers. Please see \"List Inbound Routes\" to review the route values that you can associate with your Flowroute phone numbers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bcca226-82e9-4147-9006-fa446d3e0c44"
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