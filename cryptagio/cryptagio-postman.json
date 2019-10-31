{
  "info": {
    "name": "Cryptagio Delete Orders",
    "_postman_id": "6dc24219-4dc2-46b3-a598-d4210f3ca184",
    "description": "Cancel order by uuid..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "d6ff23fc-2c05-420c-9e8d-c155018449df",
          "name": "getInfo",
          "request": {
            "url": "{{default}}/info",
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
            "description": "Get information.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38a05f73-1552-4d2c-8c09-e003571aed79"
            }
          ]
        },
        {
          "id": "e7f21276-77ca-4501-90d0-e6ac2d9b400f",
          "name": "getTicker",
          "request": {
            "url": "{{default}}/ticker",
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
            "description": "Get ticker of all markets.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1c919b1-8610-4e47-9db1-8062efd710ac"
            }
          ]
        },
        {
          "id": "9bcf2d93-67e9-44ec-b15b-5173805c400e",
          "name": "getTrades",
          "request": {
            "url": "{{default}}/trades?from_time=%7B%7D&from_uuid=%7B%7D&limit=%7B%7D&market=%7B%7D&order=%7B%7D&side=%7B%7D&to_time=%7B%7D",
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
            "description": "Get recent trades on market, each trade is included only once. Trades are sorted in reverse creation order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9412ab32-b343-405e-93df-c199ae7ded8a"
            }
          ]
        },
        {
          "id": "27834ee8-0075-4932-ad3a-83a34ae28530",
          "name": "getTradesMy",
          "request": {
            "url": "{{default}}/trades/my?from_time=%7B%7D&from_uuid=%7B%7D&limit=%7B%7D&market=%7B%7D&order=%7B%7D&side=%7B%7D&to_time=%7B%7D",
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
            "description": "Trades are sorted in reverse creation order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5b47111-8a5f-4c5c-bbfd-230dc155cbe3"
            }
          ]
        },
        {
          "id": "8823b812-3ef9-4dfa-902a-ae80ced48bc9",
          "name": "getBalances",
          "request": {
            "url": "{{default}}/balances",
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
            "description": "Get user balances.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce3e8cc1-b46d-4076-a578-30d569a4a5f7"
            }
          ]
        },
        {
          "id": "e66c8aa4-c9e4-4dbb-89c5-b2cf7596df40",
          "name": "getOrdersMy",
          "request": {
            "url": "{{default}}/orders/my?from_time=%7B%7D&from_uuid=%7B%7D&limit=%7B%7D&market=%7B%7D&order=%7B%7D&side=%7B%7D&status=%7B%7D&to_time=%7B%7D&type=%7B%7D",
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
            "description": "Trades are sorted in reverse creation order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2127b19-1281-4388-a865-1bfbc30d3596"
            }
          ]
        },
        {
          "id": "b0273b99-d295-4923-8c1b-dd18d422addf",
          "name": "postOrders",
          "request": {
            "url": "{{default}}/orders",
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
            "description": "Accepts an array of JSON objects."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12c2bdc0-4cd8-400a-b295-dd93a7a27b1d"
            }
          ]
        },
        {
          "id": "2a8b2ce6-6461-49a7-9c1f-a0480a479ce8",
          "name": "postOrdersCancel",
          "request": {
            "url": "{{default}}/orders/cancel",
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
            "description": "Accepts JSON object. Cancels all orders if no parameters are passed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e25d46fa-a807-441b-b9d9-68bcf16eab20"
            }
          ]
        },
        {
          "id": "9171e8ee-ae38-44cf-bf5b-19cf94f38e7d",
          "name": "deleteOrdersUu",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "orders/:uuid"
              ],
              "variable": [
                {
                  "id": "uuid",
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
            "description": "Cancel order by uuid.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5083f34e-bb5a-4814-b96e-6c56fd1889ea"
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