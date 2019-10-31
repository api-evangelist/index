swagger: "2.0"
x-collection-name: Crypto Compare
x-complete: 1
info:
  title: Cryptocompare
  description: todo-add-description
  version: 1.0.0
host: min-api.cryptocompare.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    get:
      summary: API Description
      description: Api description.
      operationId: UnnammedEndpointGet
      x-api-path-slug: get
      responses:
        200:
          description: OK
      tags:
      - Discovery
  /data/price:
    get:
      summary: Get Single Price
      description: Get single price.
      operationId: DataPriceGet
      x-api-path-slug: dataprice-get
      parameters:
      - in: query
        name: fsym
      - in: query
        name: tsyms
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Single
      - Price
  /data/pricemulti:
    get:
      summary: Get Multiple Prices
      description: Get multiple prices.
      operationId: DataPricemultiGet
      x-api-path-slug: datapricemulti-get
      parameters:
      - in: query
        name: fsyms
      - in: query
        name: tsyms
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Multiple
      - Prices
  /data/all/coinlist:
    get:
      summary: Get Coinlist
      description: Get coinlist.
      operationId: DataAllCoinlistGet
      x-api-path-slug: dataallcoinlist-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Coins