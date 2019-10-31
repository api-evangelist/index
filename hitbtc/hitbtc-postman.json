{
  "info": {
    "name": "HitBTC Transfer Amount To Trading",
    "_postman_id": "15009b53-4c7f-4fe4-b7c4-ba0f6954e2e9",
    "description": "Transfer amount to trading.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Available",
      "item": [
        {
          "id": "bbae3e1d-c234-49db-b249-9d9c3fb7a64e",
          "name": "getPublicSymbol",
          "request": {
            "url": "{{default}}/public/symbol",
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
            "description": "Available currency symbols."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5b306ef-8b26-47d6-a9a9-cd773066fd2d"
            }
          ]
        },
        {
          "id": "0ccda45b-b64f-4f66-bd7c-e7482c192169",
          "name": "getPublicCurrency",
          "request": {
            "url": "{{default}}/public/currency",
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
            "description": "Available currencies."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37a61ab1-8d24-48b5-8bc0-aacdd405b4a0"
            }
          ]
        }
      ]
    },
    {
      "name": "Symbol",
      "item": [
        {
          "id": "9b66d338-e08b-451c-8af4-693c602674fd",
          "name": "getPublicSymbolSymbol",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "public/symbol/:symbol"
              ],
              "variable": [
                {
                  "id": "symbol",
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
            "description": "Get symbol info."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5b2b9db-f9a7-4c8f-a53e-7c19688e609d"
            }
          ]
        }
      ]
    },
    {
      "name": "Currency",
      "item": [
        {
          "id": "1aa70a3c-f83f-457d-a6f9-d517353028ec",
          "name": "getPublicCurrencyCurrency",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "public/currency/:currency"
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
            "description": "Get currency info."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06d599c1-a393-456e-84a3-c883a27c405d"
            }
          ]
        }
      ]
    },
    {
      "name": "Ticker",
      "item": [
        {
          "id": "d44daf01-fff6-4d14-8d24-2c768e7d523b",
          "name": "getPublicTicker",
          "request": {
            "url": "{{default}}/public/ticker",
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
            "description": "Ticker list for all symbols."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46e822b8-2251-4123-8195-258ce7c310b6"
            }
          ]
        }
      ]
    },
    {
      "name": "Tickersymbol",
      "item": [
        {
          "id": "23274135-5867-4706-ad94-178a2575b880",
          "name": "getPublicTickerSymbol",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "public/ticker/:symbol"
              ],
              "variable": [
                {
                  "id": "symbol",
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
            "description": "Ticker for symbol."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3eca2ab-c832-4634-b066-c2be46bcccbe"
            }
          ]
        }
      ]
    },
    {
      "name": "Trades",
      "item": [
        {
          "id": "341d01ee-d9e8-41f8-b65e-672c79619573",
          "name": "getPublicTradesSymbol",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "public/trades/:symbol"
              ],
              "query": [
                {
                  "key": "by",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "from",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "till",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "symbol",
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
            "description": "Trades."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4cd14d5b-197f-4a76-9e09-ffd122b84c4f"
            }
          ]
        }
      ]
    },
    {
      "name": "Orderbook",
      "item": [
        {
          "id": "28e42d46-d6a3-474a-b03a-c3bbad600a74",
          "name": "getPublicOrderbookSymbol",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "public/orderbook/:symbol"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "symbol",
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
            "description": "Orderbook."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7124d7f0-e873-4991-87ec-ffe3c30e093f"
            }
          ]
        }
      ]
    },
    {
      "name": "Candles",
      "item": [
        {
          "id": "880f7b22-2f87-4fb4-9d0f-a5a9ed9bd80a",
          "name": "getPublicCandlesSymbol",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "public/candles/:symbol"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "period",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "symbol",
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
            "description": "Candles."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c62a7b3a-3436-45d7-a67b-0ac2e8bdba5e"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "5617fee9-13da-4b4c-bdeb-f2db620fb709",
          "name": "getOrder",
          "request": {
            "url": "{{default}}/order?symbol=%7B%7D",
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
            "description": "List your current open orders."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2101516-3366-4462-9c10-0a2880535f01"
            }
          ]
        }
      ]
    },
    {
      "name": "New",
      "item": [
        {
          "id": "fed5e81b-6414-4e75-8e04-284fd49fbde0",
          "name": "postOrder",
          "request": {
            "url": "{{default}}/order",
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
                  "key": "clientOrderId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "expireTime",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "price",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "quantity",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "side",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "stopPrice",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "strictValidate",
                  "value": "{}",
                  "disabled": false,
                  "description": "Strict validate amount and price precision without rounding"
                },
                {
                  "key": "symbol",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "timeInForce",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "type",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Create new order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d9df277-33c8-48fe-85f2-cd2cdcddb235"
            }
          ]
        },
        {
          "id": "baeb340d-2723-4a40-9808-c4e91a28bafd",
          "name": "putOrderClientorder",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "order/:clientOrderId"
              ],
              "variable": [
                {
                  "id": "clientOrderId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
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
                  "key": "expireTime",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "price",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "quantity",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "side",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "stopPrice",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "strictValidate",
                  "value": "{}",
                  "disabled": false,
                  "description": "Strict validate amount and price precision without rounding"
                },
                {
                  "key": "symbol",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "timeInForce",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "type",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Create new order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "262979f2-5215-4618-9444-173f64cf8efe"
            }
          ]
        },
        {
          "id": "914579ac-66ec-47f6-a876-813dc94d9566",
          "name": "postAccountCryptoAddressCurrency",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "account/crypto/address/:currency"
              ],
              "variable": [
                {
                  "id": "currency",
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
            "description": "Create new deposit crypro address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a7309db-ec6e-4f4b-b589-442919acfa8a"
            }
          ]
        }
      ]
    },
    {
      "name": "Cancel",
      "item": [
        {
          "id": "fd0353a6-a986-4cfd-9ebf-aa8acea1db24",
          "name": "deleteOrder",
          "request": {
            "url": "{{default}}/order",
            "method": "DELETE",
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
                  "key": "symbol",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Cancel all open orders."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62b898e4-a310-4353-8660-6b8c53c59b29"
            }
          ]
        },
        {
          "id": "ed9b471e-c8cf-4f76-bb34-0144bb51f2d0",
          "name": "deleteOrderClientorder",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "order/:clientOrderId"
              ],
              "variable": [
                {
                  "id": "clientOrderId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Cancel order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a23769b0-a11e-4d4f-b2d3-ee1595d6a626"
            }
          ]
        },
        {
          "id": "07b41404-ece4-4b0a-8258-e0991134ba18",
          "name": "patchOrderClientorder",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "order/:clientOrderId"
              ],
              "variable": [
                {
                  "id": "clientOrderId",
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
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "price",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "quantity",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "requestClientId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Cancel replace order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2098e28-fecc-4358-a3d6-669b2fe067e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Single",
      "item": [
        {
          "id": "6bbafe08-17bd-4ce6-977d-9b4246958d9a",
          "name": "getOrderClientorder",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "order/:clientOrderId"
              ],
              "query": [
                {
                  "key": "wait",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "clientOrderId",
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
            "description": "Get a single order by clientorderid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dbb94b7c-1ebb-4ed3-8587-0461fcefd986"
            }
          ]
        }
      ]
    },
    {
      "name": "Trading",
      "item": [
        {
          "id": "302dd9c8-7dcf-401f-9008-de37424a3779",
          "name": "getTradingBalance",
          "request": {
            "url": "{{default}}/trading/balance",
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
            "description": "Get trading balance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce867e85-3d4f-42aa-b9ad-490fb53e7ffb"
            }
          ]
        },
        {
          "id": "a8e6a227-12c8-4a77-9b60-1a850dc67b17",
          "name": "getTradingFeeSymbol",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "trading/fee/:symbol"
              ],
              "variable": [
                {
                  "id": "symbol",
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
            "description": "Get trading fee rate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "779e0b58-aa4b-478b-83ac-71234468465b"
            }
          ]
        }
      ]
    },
    {
      "name": "Historical",
      "item": [
        {
          "id": "99739f01-5049-42bb-b215-b285cbcd7851",
          "name": "getHistoryTrades",
          "request": {
            "url": "{{default}}/history/trades?by=%7B%7D&from=%7B%7D&limit=%7B%7D&offset=%7B%7D&sort=%7B%7D&symbol=%7B%7D&till=%7B%7D",
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
            "description": "Get historical trades."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "358a5987-d03b-4e25-ba65-92e789165959"
            }
          ]
        },
        {
          "id": "44ce5b93-03fa-4e80-8c23-cd8b67a39859",
          "name": "getHistoryOrder",
          "request": {
            "url": "{{default}}/history/order?clientOrderId=%7B%7D&from=%7B%7D&limit=%7B%7D&offset=%7B%7D&symbol=%7B%7D&till=%7B%7D",
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
            "description": "Get historical orders."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "604813fd-bda8-4b95-9cc5-4003b5364a1c"
            }
          ]
        },
        {
          "id": "73a374ac-5f9c-49db-b08c-3fa58df3e986",
          "name": "getHistoryOrderTrades",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "history/order/:id/trades"
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
            "description": "Get historical trades by specified order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d548e96f-10a3-424e-8449-a7788dcce693"
            }
          ]
        }
      ]
    },
    {
      "name": "Main",
      "item": [
        {
          "id": "36858949-3f9c-4fc1-bccd-4da1c6c454b9",
          "name": "getAccountBalance",
          "request": {
            "url": "{{default}}/account/balance",
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
            "description": "Get main acccount balance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f25a76a-3c7c-47dd-8f39-cfad6e3c6160"
            }
          ]
        }
      ]
    },
    {
      "name": "Account",
      "item": [
        {
          "id": "e52f709f-7aad-45c2-82ba-187f2c105743",
          "name": "getAccountTransactions",
          "request": {
            "url": "{{default}}/account/transactions?by=%7B%7D&currency=%7B%7D&from=%7B%7D&limit=%7B%7D&offset=%7B%7D&sort=%7B%7D&till=%7B%7D",
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
            "description": "Get account transactions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd9764ea-53c4-4dac-8467-b1eefce2ff83"
            }
          ]
        },
        {
          "id": "5e177b5f-f460-4615-b531-0f58d0ecd6f4",
          "name": "getAccountTransactions",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "account/transactions/:id"
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
            "description": "Get account transaction by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b81e8fba-dc1e-4dfd-8adc-625eb37caea9"
            }
          ]
        }
      ]
    },
    {
      "name": "Withdraw",
      "item": [
        {
          "id": "8c98315c-2264-4ee1-913c-5bb3caccf90b",
          "name": "postAccountCryptoWithdraw",
          "request": {
            "url": "{{default}}/account/crypto/withdraw",
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
                  "key": "address",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "amount",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "autoCommit",
                  "value": "{}",
                  "disabled": false,
                  "description": "If Auto commit disabled you should commit it or rollback within 1 hour"
                },
                {
                  "key": "currency",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "includeFee",
                  "value": "{}",
                  "disabled": false,
                  "description": "If enabled, then fee will be subtracted from amount"
                },
                {
                  "key": "networkFee",
                  "value": "{}",
                  "disabled": false,
                  "description": "Suggest preferred network fee"
                },
                {
                  "key": "paymentId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Withdraw crypro."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df4b6ed8-81b7-4ba1-b6ce-4c44e0104fcc"
            }
          ]
        }
      ]
    },
    {
      "name": "Commit",
      "item": [
        {
          "id": "054f743b-5bd2-4e61-a605-54204469e54c",
          "name": "putAccountCryptoWithdraw",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "account/crypto/withdraw/:id"
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
            "description": "Commit withdraw crypro."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb339cc0-e486-4edb-bc54-0a66e12a8623"
            }
          ]
        }
      ]
    },
    {
      "name": "Rollback",
      "item": [
        {
          "id": "49d21a7e-b6c5-49bf-a070-5191e5e2d5a8",
          "name": "deleteAccountCryptoWithdraw",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "account/crypto/withdraw/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Rollback withdraw crypro."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01124a71-a934-4df5-b19b-b910e04af5ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Deposit",
      "item": [
        {
          "id": "aaa1ee7c-3fd7-4902-95bf-60e0be5a233e",
          "name": "getAccountCryptoAddressCurrency",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "account/crypto/address/:currency"
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
            "description": "Get deposit crypro address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29a7ba0e-7e74-4b4a-9a06-e1687a4b1c5c"
            }
          ]
        }
      ]
    },
    {
      "name": "Transfer",
      "item": [
        {
          "id": "e4fe881c-a95b-4227-97f0-985e9daeb8e3",
          "name": "postAccountTransfer",
          "request": {
            "url": "{{default}}/account/transfer",
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
                  "key": "amount",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "currency",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "type",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Transfer amount to trading."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75bd105c-e8ea-4267-9b90-5880313f2656"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/api/2"
    }
  ]
}