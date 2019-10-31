swagger: "2.0"
x-collection-name: Barchart
x-complete: 1
info:
  title: Barchart API
  description: stock-futures-and-forex-quotes-and-historical-data-
  version: 1.0.0
host: marketdata.websol.barchart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /getQuote.json:
    get:
      summary: Get Quote
      description: The getQuote API is used to request price data, either real-time,
        delayed or end-of-day, by symbol. In addition to Last Price or Settlement,
        other fields such as Open, High, Low, Close, Bid, Ask, 52-week high and low,
        and more are available.
      operationId: getQuote
      x-api-path-slug: getquote-json-get
      parameters:
      - in: query
        name: symbols
        description: A symbol or code that identifies a financial instrument
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Quotes
  /getEquitiesByExchange.json:
    get:
      summary: Get Equities by Exchange
      description: Receive all real-time or delayed stock and/or index price data
        by exchange through a single onDemand query.
      operationId: getEquitiesByExchange
      x-api-path-slug: getequitiesbyexchange-json-get
      parameters:
      - in: query
        name: symbols
        description: A symbol or code that identifies a financial instrument
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Equities
  /getFuturesByExchange.json:
    get:
      summary: Get Futures by Exchange
      description: Receive all real-time or delayed, or end-of-day Futures data by
        exchange through a single onDemand query.
      operationId: getFuturesByExchange
      x-api-path-slug: getfuturesbyexchange-json-get
      responses:
        200:
          description: OK
      tags:
      - Futures
  /getClosePrice.json:
    get:
      summary: Get Close Price
      description: Get the close price for given instruments for the given date.
      operationId: getClosePrice
      x-api-path-slug: getcloseprice-json-get
      parameters:
      - in: query
        name: symbols
        description: A symbol or code that identifies a financial instrument
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Stocks
      - Price