swagger: "2.0"
x-collection-name: Polygon
x-complete: 1
info:
  title: Polygon
  description: the-future-of-fintech-
  version: 1.0.0
host: api.polygon.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/companies:
    get:
      summary: Available Companies
      description: Get a list of the traded companies that polygon.io streams. Company
        includes some details about the company which we hope to add more to soon.
      operationId: v1.companies.get
      x-api-path-slug: v1companies-get
      parameters:
      - in: query
        name: page
        description: Which page of results to return
      - in: query
        name: perpage
        description: How many items to be on each page during pagination
      - in: query
        name: sort
        description: Which field to sort by
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/currencies:
    get:
      summary: Available Currencies
      description: Get a list of the currencies that polygon.io streams.
      operationId: v1.currencies.get
      x-api-path-slug: v1currencies-get
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/historic/agg/{size}/{symbol}/{date}:
    get:
      summary: Historic Aggregates
      description: Get historic aggregations for a symbol.
      operationId: v1.historic.agg.size.symbol.date.get
      x-api-path-slug: v1historicaggsizesymboldate-get
      parameters:
      - in: path
        name: date
        description: Date/Day of the historic ticks to retreive
      - in: query
        name: limit
        description: 'Limit the size of response, max: 10000'
      - in: query
        name: offset
        description: Timestamp offset, used for pagination
      - in: path
        name: size
        description: Size of the aggregation
      - in: path
        name: symbol
        description: Symbol of the company to retrieve
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/historic/forex/{from}/{to}/{date}:
    get:
      summary: Historic Forex Ticks
      description: Get historic ticks for a currency pair. Example for **USD/JPY**
        the from would be **USD** and to would be **JPY**. The date formatted like
        **2017-6-22**
      operationId: v1.historic.forex.from.to.date.get
      x-api-path-slug: v1historicforexfromtodate-get
      parameters:
      - in: path
        name: date
        description: Date/Day of the historic ticks to retreive
      - in: path
        name: from
        description: From Symbol of the currency pair
      - in: query
        name: limit
        description: 'Limit the size of response, max: 10000'
      - in: query
        name: offset
        description: Timestamp offset, used for pagination
      - in: path
        name: to
        description: To Symbol of the currency pair
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/historic/quotes/{symbol}/{date}:
    get:
      summary: Historic Quotes
      description: Get historic quotes for a symbol.
      operationId: v1.historic.quotes.symbol.date.get
      x-api-path-slug: v1historicquotessymboldate-get
      parameters:
      - in: path
        name: date
        description: Date/Day of the historic ticks to retreive
      - in: query
        name: limit
        description: 'Limit the size of response, max: 10000'
      - in: query
        name: offset
        description: Timestamp offset, used for pagination
      - in: path
        name: symbol
        description: Symbol of the company to retrieve
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/historic/trades/{symbol}/{date}:
    get:
      summary: Historic Trades
      description: Get historic trades for a symbol.
      operationId: v1.historic.trades.symbol.date.get
      x-api-path-slug: v1historictradessymboldate-get
      parameters:
      - in: path
        name: date
        description: Date/Day of the historic ticks to retreive
      - in: query
        name: limit
        description: 'Limit the size of response, max: 10000'
      - in: query
        name: offset
        description: Timestamp offset, used for pagination
      - in: path
        name: symbol
        description: Symbol of the company to retrieve
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/last/currencies/{from}/{to}:
    get:
      summary: Last Trade for a Currency Pair
      description: Get Last Trade Tick for a Currency Pair.
      operationId: v1.last.currencies.from.to.get
      x-api-path-slug: v1lastcurrenciesfromto-get
      parameters:
      - in: path
        name: from
        description: From Symbol of the pair
      - in: path
        name: to
        description: To Symbol of the pair
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/last/stocks/{symbol}:
    get:
      summary: Last Trade for a Symbol
      description: Get the last trade for a given stock.
      operationId: v1.last.stocks.symbol.get
      x-api-path-slug: v1laststockssymbol-get
      parameters:
      - in: path
        name: symbol
        description: Symbol of the stock to get
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/last_quote/currencies/{from}/{to}:
    get:
      summary: Last Quote for a Currency Pair
      description: Get Last Quote Tick for a Currency Pair.
      operationId: v1.last_quote.currencies.from.to.get
      x-api-path-slug: v1last-quotecurrenciesfromto-get
      parameters:
      - in: path
        name: from
        description: From Symbol of the pair
      - in: path
        name: to
        description: To Symbol of the pair
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/last_quote/stocks/{symbol}:
    get:
      summary: Last Quote for a Symbol
      description: Get the last quote tick for a given stock.
      operationId: v1.last_quote.stocks.symbol.get
      x-api-path-slug: v1last-quotestockssymbol-get
      parameters:
      - in: path
        name: symbol
        description: Symbol of the stock to get
      responses:
        200:
          description: OK
      tags:
      - ""