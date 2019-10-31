{
  "info": {
    "name": "Point-In-Polygon Census Intersection Last Quote for a Symbol",
    "_postman_id": "692b9391-a23a-4fbf-be82-b9280e4ae81d",
    "description": "Get the last quote tick for a given stock.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "ac3b6865-9912-42cd-b67a-2db97974b2e7",
      "name": "v1.companies.get",
      "request": {
        "url": "http://api.polygon.io/v1/companies?page=%7B%7D&perpage=%7B%7D&sort=%7B%7D",
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
        "description": "Get a list of the traded companies that polygon.io streams. Company includes some details about the company which we hope to add more to soon."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "0215d28b-f84c-4cea-a1a9-5d7eb37769c4"
        }
      ]
    },
    {
      "id": "acb8c31a-3a89-4342-9254-350346087ba2",
      "name": "v1.currencies.get",
      "request": {
        "url": "http://api.polygon.io/v1/currencies",
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
        "description": "Get a list of the currencies that polygon.io streams."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "1fa8ed1e-8c67-4764-b0bb-ac9ec389cb9c"
        }
      ]
    },
    {
      "id": "b31e1353-bf48-4a94-a69a-7b3ff0f8f619",
      "name": "v1.historic.agg.size.symbol.date.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.polygon.io",
          "path": [
            "v1/historic/agg/:size/:symbol/:date"
          ],
          "query": [
            {
              "key": "limit",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "offset",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "date",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "size",
              "value": "{}",
              "type": "string"
            },
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
        "description": "Get historic aggregations for a symbol."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "5837e67e-abfe-4fb9-a7ba-da84964662cd"
        }
      ]
    },
    {
      "id": "1106e557-dd98-447f-9382-367479a5db72",
      "name": "v1.historic.forex.from.to.date.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.polygon.io",
          "path": [
            "v1/historic/forex/:from/:to/:date"
          ],
          "query": [
            {
              "key": "limit",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "offset",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "date",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "from",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "to",
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
        "description": "Get historic ticks for a currency pair. Example for **USD/JPY** the from would be **USD** and to would be **JPY**. The date formatted like **2017-6-22**"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "e6426b99-7184-4281-b6fd-2073163106a8"
        }
      ]
    },
    {
      "id": "ae5dceea-e26a-4fad-a4b2-9d9550d9499a",
      "name": "v1.historic.quotes.symbol.date.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.polygon.io",
          "path": [
            "v1/historic/quotes/:symbol/:date"
          ],
          "query": [
            {
              "key": "limit",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "offset",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "date",
              "value": "{}",
              "type": "string"
            },
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
        "description": "Get historic quotes for a symbol."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "41740f6f-8f80-4cdd-beb3-8e913f3c9cfb"
        }
      ]
    },
    {
      "id": "1b0f8650-f7c3-45ce-a51c-c5d913dd30e8",
      "name": "v1.historic.trades.symbol.date.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.polygon.io",
          "path": [
            "v1/historic/trades/:symbol/:date"
          ],
          "query": [
            {
              "key": "limit",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "offset",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "date",
              "value": "{}",
              "type": "string"
            },
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
        "description": "Get historic trades for a symbol."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "f90490b2-56fe-440e-a84b-503a8d516ab1"
        }
      ]
    },
    {
      "id": "d612b54f-599a-4276-a15c-76513ebc1886",
      "name": "v1.last.currencies.from.to.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.polygon.io",
          "path": [
            "v1/last/currencies/:from/:to"
          ],
          "variable": [
            {
              "id": "from",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "to",
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
        "description": "Get Last Trade Tick for a Currency Pair."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "5bb644db-2663-4501-b85c-48e179ed693a"
        }
      ]
    },
    {
      "id": "7e24c72a-6209-43ba-b2d7-7e26267f90e8",
      "name": "v1.last.stocks.symbol.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.polygon.io",
          "path": [
            "v1/last/stocks/:symbol"
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
        "description": "Get the last trade for a given stock."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "ebb8b7f2-dcd0-4173-b576-3d92e81df7cd"
        }
      ]
    },
    {
      "id": "14fbddf4-4a0a-4648-9dc7-9bd7283f2dd7",
      "name": "v1.last_quote.currencies.from.to.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.polygon.io",
          "path": [
            "v1/last_quote/currencies/:from/:to"
          ],
          "variable": [
            {
              "id": "from",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "to",
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
        "description": "Get Last Quote Tick for a Currency Pair."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "24f1e427-b166-4f86-bd24-9d75a2d534b5"
        }
      ]
    },
    {
      "id": "42440488-2413-4378-bacf-0536669d4c2b",
      "name": "v1.last_quote.stocks.symbol.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.polygon.io",
          "path": [
            "v1/last_quote/stocks/:symbol"
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
        "description": "Get the last quote tick for a given stock."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "45c37ca3-e661-4213-9e4d-4f71d66769d6"
        }
      ]
    }
  ]
}