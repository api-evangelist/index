{
  "info": {
    "name": "3Scale Billing API Invoice Payment Transactions List",
    "_postman_id": "aa5b59dc-7465-4399-aa53-31b3e92f42e0",
    "description": "Invoice payment transactions list.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Invoice",
      "item": [
        {
          "id": "bfffcbf0-d5c2-4b0f-99e7-1b2bb0c79471",
          "name": "finance",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "api/accounts/:account_id/invoices.xml"
              ],
              "query": [
                {
                  "key": "month",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "per_page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Invoice list by account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "836c596c-b8dc-4294-b3a9-04e69cd66794"
            }
          ]
        },
        {
          "id": "6998e23d-a459-46b1-b516-b096c1e0856e",
          "name": "finance",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "api/accounts/:account_id/invoices/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Invoice by account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "398fc71c-c53c-44cb-8ad1-275d2e405e0a"
            }
          ]
        },
        {
          "id": "6f47de5a-5215-4198-9be7-d83366fa64d3",
          "name": "finance",
          "request": {
            "url": "http://su1.3scale.net/api/invoices.xml?month=%7B%7D&page=%7B%7D&per_page=%7B%7D&provider_key=%7B%7D&state=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Invoice list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79bad48d-9d38-45e0-b1c7-a65e9cc89cf5"
            }
          ]
        },
        {
          "id": "926e4dcd-c725-44e7-98be-39ab9e5b959c",
          "name": "finance",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "api/invoices/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
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
            "description": "Invoice."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4359c47f-cb61-4d15-954d-cc3bcf24957f"
            }
          ]
        },
        {
          "id": "b0eae2ab-4b1d-4123-bc9d-46ed126adf71",
          "name": "finance",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "api/invoices/:id/state.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "state",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Invoice."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3bb6303d-5580-467f-ab42-a40a052ce347"
            }
          ]
        },
        {
          "id": "08130e28-36a8-4d7d-af77-7a0ae06a5da2",
          "name": "finance",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "api/invoices/:invoice_id/line_items.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "invoice_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Invoice line items list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6656806f-b9da-41be-8de8-8f535d5d0d6c"
            }
          ]
        },
        {
          "id": "599390b0-8ad3-41b9-9e69-54c2a18a1aaf",
          "name": "finance1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "api/invoices/:invoice_id/payment_transactions.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "invoice_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Invoice payment transactions list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ab22439-d0bf-4db2-9c22-adbcdd83c674"
            }
          ]
        }
      ]
    }
  ]
}