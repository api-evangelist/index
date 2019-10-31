{
  "info": {
    "name": "Azure Billing API Operations List",
    "_postman_id": "f6233e17-39bb-4a59-afa3-33e04a8cfd7f",
    "description": "Lists all of the available consumption REST API operations.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Billing Period",
      "item": [
        {
          "id": "b68ce9fe-1cb6-421a-aefc-67dc1eb6f737",
          "name": "BillingPeriods_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Billing/billingPeriods"
              ],
              "query": [
                {
                  "key": "$filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$skiptoken",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$top",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the available billing periods for a subscription in reverse chronological order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f66fa235-eb00-4e66-8818-0754cc099c09"
            }
          ]
        },
        {
          "id": "9e838e00-1373-4e51-8746-012bf9c68cb8",
          "name": "BillingPeriods_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Billing/billingPeriods/:billingPeriodName"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "billingPeriodName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a named billing period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "486b984a-9db0-4bff-892b-2cf90c07b0d3"
            }
          ]
        }
      ]
    },
    {
      "name": "Invoice",
      "item": [
        {
          "id": "72c8dd26-5b64-43dd-8cf3-dd19a9ca4008",
          "name": "Invoices_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Billing/invoices"
              ],
              "query": [
                {
                  "key": "$expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$skiptoken",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$top",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the available invoices for a subscription in reverse chronological order beginning with the most recent invoice. In preview, invoices are available via this API only for invoice periods which end December 1, 2016 or later."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc26f7e2-8ebd-4d3f-9204-8873106a0e03"
            }
          ]
        },
        {
          "id": "4d71f9a5-e639-4781-930c-fd88160d7d0b",
          "name": "Invoices_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Billing/invoices/:invoiceName"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "invoiceName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a named invoice resource. When getting a single invoice, the downloadUrl property is expanded automatically."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25e97cd0-6416-4188-b82d-f1486fd88b81"
            }
          ]
        },
        {
          "id": "1b9a72a0-95f5-40d2-8914-85851b7012c7",
          "name": "Invoices_GetLatest",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Billing/invoices/latest"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the most recent invoice. When getting a single invoice, the downloadUrl property is expanded automatically."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5beb0036-1289-4cec-9d67-7ec5bc3e004a"
            }
          ]
        }
      ]
    },
    {
      "name": "Operation",
      "item": [
        {
          "id": "2e446254-f646-4ca6-8aa8-fddb65e86268",
          "name": "Operations_List",
          "request": {
            "url": "http://management.azure.com/providers/Microsoft.Billing/operations?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all of the available billing REST API operations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf5c00cd-7edb-4961-b871-974463937435"
            }
          ]
        },
        {
          "id": "cdc601e4-af9c-4cad-8f73-19ea1f1ce2b7",
          "name": "Operations_List1",
          "request": {
            "url": "http://management.azure.com/providers/Microsoft.Consumption/operations?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all of the available consumption REST API operations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a815c05-6d0d-4bbb-b85a-fc93e5e128b0"
            }
          ]
        }
      ]
    },
    {
      "name": "Usage",
      "item": [
        {
          "id": "06134068-1126-481f-a74b-f93b162f5d4b",
          "name": "UsageDetails_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                ":scope/providers/Microsoft.Consumption/usageDetails"
              ],
              "query": [
                {
                  "key": "$expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$skiptoken",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$top",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "scope",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the usage details for a scope in reverse chronological order by billing period. Usage details are available via this API only for January 1, 2017 or later."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c4c5c54-6127-4af9-8b17-8d14c14773c8"
            }
          ]
        }
      ]
    }
  ]
}