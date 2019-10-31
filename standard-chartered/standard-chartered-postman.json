{
  "info": {
    "name": "Standard Chartered Retrieve trade finance transaction status for specific transaction reference Id",
    "_postman_id": "334d4280-f649-4ea7-bb8f-534f76ea5b03",
    "description": "Retrieve trade finance transaction status for specific transaction reference Id",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cib",
      "item": [
        {
          "id": "95a16076-1644-4073-a0b3-4356e0f1fb94",
          "name": "getCibServiceS2bApiV1BanksScbAccountsAccountViewAccount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/banks/scb/accounts/:accountId/:viewId/account"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "viewId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "GroupId",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "UserId",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The ???GetAccountBalance??? API upon successful user authentication and entitlement checks will return the various types of ???Account Balances??? applicable for the specified Account Number."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be34f94d-cde1-4fce-a800-96d814b1f775"
            }
          ]
        },
        {
          "id": "e774c2f6-880d-4290-bdae-085ad64fb5c0",
          "name": "getCibServiceS2bApiV1BanksScbAccountsAccountViewTransactionRequestTypes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/banks/scb/accounts/:accountId/:viewId/transaction-request-types"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "viewId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "GroupId",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "UserId",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The ???GetTransactionTypes??? API upon successful user authentication and entitlement checks will return the supported transaction types for the specified account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4b6accc-46c9-4f1e-b9d0-f3a41b80e71a"
            }
          ]
        },
        {
          "id": "68a225e4-66fc-49fa-8eaf-5a9ac45a2726",
          "name": "getCibServiceS2bApiV1BanksScbAccountsViewAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/banks/scb/accounts/:viewId/accounts"
              ],
              "variable": [
                {
                  "id": "viewId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "GroupId",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "UserId",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List available bank accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a553e2fc-4325-419e-8027-f3a520c73a48"
            }
          ]
        },
        {
          "id": "ab6aa93f-2aa2-45f6-90ec-81ef614dbc4b",
          "name": "postCibServiceS2bApiV1BanksScbReferenceDefaultBranches",
          "request": {
            "url": "http://developer.sc.com/cib/service/s2b/api/v1/banks/scb/reference/default/branches",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "The ???GetBankCode??? API returns list of Bank Codes for the specified combination of ???Country???, ???City??? and ???Bank??? combination. The data will contain the ???Bank Code(s)??? as well as the address for the Bank & Branch."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae70e55e-e2ef-4c94-b5f5-b13429bab19f"
            }
          ]
        },
        {
          "id": "7f0e179a-5aa8-4dfe-9123-81900d960ac4",
          "name": "getCibServiceS2bApiV1BanksScbReferenceDefaultHolayCalendarCountryCountry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/banks/scb/reference/default/holiday-calendar/country/:country"
              ],
              "query": [
                {
                  "key": "endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startDate",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "country",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The ???GetHolidayCalendar??? API returns list of holidays applicable for the specified combination of:\n<ul><li>Country</li><li>Date Range</li></lu>"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4138c532-5358-4890-b4c2-22697c7a8ef9"
            }
          ]
        },
        {
          "id": "b25e50f3-74d2-4575-97c8-34f47fc5bd90",
          "name": "getCibServiceS2bApiV1BanksScbReferenceDefaultHolayCalendarCurrencyCurrency",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/banks/scb/reference/default/holiday-calendar/currency/:currency"
              ],
              "query": [
                {
                  "key": "endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startDate",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "currency",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The ???GetHolidayCalendar??? API returns list of holidays applicable for the specified combination of:\n<ul><li>Currency</li><li>Date Range</li></lu>"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c95abc7-4bb3-479c-b79b-f7c3845050f4"
            }
          ]
        },
        {
          "id": "34a80aac-9be0-479a-a630-4e1d4e44e503",
          "name": "getCibServiceS2bApiV1TradeCountrycodeCustomerProfile",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/trade/:countryCode/:customerId/profile"
              ],
              "variable": [
                {
                  "id": "countryCode",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve trade finance customer profile"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37017a6e-6cfb-4359-a723-649f35e607cf"
            }
          ]
        },
        {
          "id": "e24ddbe9-da67-4a62-8e69-e77144834c68",
          "name": "getCibServiceS2bApiV1TradeCountrycodeCustomerLimits",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/trade/:countryCode/:customerId/limits"
              ],
              "variable": [
                {
                  "id": "countryCode",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve trade finance limit details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0d5ebbf-7aca-4cb2-aa5c-ca6a235e2346"
            }
          ]
        },
        {
          "id": "2f389aab-6dc9-4381-b3f9-a856ca8cb510",
          "name": "getCibServiceS2bApiV1TradeCountrycodeCustomerTransactions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/trade/:countryCode/:customerId/transactions"
              ],
              "query": [
                {
                  "key": "tz",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "countryCode",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve all trade finance transaction status for the current date (localised to tz)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3fc7ef0-865a-4b24-8540-09c201b6a854"
            }
          ]
        },
        {
          "id": "c5c61d95-08c3-4206-ad41-3ee300d7ec4d",
          "name": "getCibServiceS2bApiV1TradeCountrycodeCustomerTransactionTransaction",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.sc.com",
              "path": [
                "cib/service/s2b/api/v1/trade/:countryCode/:customerId/transaction/:transactionId"
              ],
              "variable": [
                {
                  "id": "countryCode",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "customerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "transactionId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve trade finance transaction status for specific transaction reference Id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37a66779-880b-403b-8142-b3bc05ce70e4"
            }
          ]
        }
      ]
    }
  ]
}