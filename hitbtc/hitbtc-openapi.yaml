swagger: "2.0"
x-collection-name: HitBTC
x-complete: 1
info:
  title: HitBTC API
  description: create-api-keys-in-your-profile-httpshitbtc-comsettingsapikeys-and-use-public-api-key-as-username-and-secret-as-password-to-authorize-
  version: 1.0.0
basePath: /api/2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /public/symbol:
    get:
      summary: Available Currency Symbols
      description: Available currency symbols.
      operationId: getPublicSymbol
      x-api-path-slug: publicsymbol-get
      responses:
        200:
          description: OK
      tags:
      - Available
      - Currency
      - Symbols
  /public/symbol/{symbol}:
    get:
      summary: Get Symbol Info
      description: Get symbol info.
      operationId: getPublicSymbolSymbol
      x-api-path-slug: publicsymbolsymbol-get
      parameters:
      - in: path
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - Symbol
      - Info
  /public/currency:
    get:
      summary: Available Currencies
      description: Available currencies.
      operationId: getPublicCurrency
      x-api-path-slug: publiccurrency-get
      responses:
        200:
          description: OK
      tags:
      - Available
      - Currencies
  /public/currency/{currency}:
    get:
      summary: Get Currency Info
      description: Get currency info.
      operationId: getPublicCurrencyCurrency
      x-api-path-slug: publiccurrencycurrency-get
      parameters:
      - in: path
        name: currency
      responses:
        200:
          description: OK
      tags:
      - Currency
      - Info
  /public/ticker:
    get:
      summary: Ticker List For All Symbols
      description: Ticker list for all symbols.
      operationId: getPublicTicker
      x-api-path-slug: publicticker-get
      responses:
        200:
          description: OK
      tags:
      - Ticker
      - List
      - Symbols
  /public/ticker/{symbol}:
    get:
      summary: Ticker For Symbol
      description: Ticker for symbol.
      operationId: getPublicTickerSymbol
      x-api-path-slug: publictickersymbol-get
      parameters:
      - in: path
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - Tickersymbol
  /public/trades/{symbol}:
    get:
      summary: Trades
      description: Trades.
      operationId: getPublicTradesSymbol
      x-api-path-slug: publictradessymbol-get
      parameters:
      - in: query
        name: by
        description: Filter field
      - in: query
        name: from
        description: If filter by timestamp, then datetime in iso format or timestamp
          in millisecond otherwise trade id
      - in: query
        name: limit
      - in: query
        name: offset
      - in: query
        name: sort
        description: Sort direction
      - in: path
        name: symbol
      - in: query
        name: till
        description: If filter by timestamp, then datetime in iso format or timestamp
          in millisecond otherwise trade id
      responses:
        200:
          description: OK
      tags:
      - Trades
  /public/orderbook/{symbol}:
    get:
      summary: Orderbook
      description: Orderbook.
      operationId: getPublicOrderbookSymbol
      x-api-path-slug: publicorderbooksymbol-get
      parameters:
      - in: query
        name: limit
        description: 0 - full orderbook otherwise number of levels
      - in: path
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - Orderbook
  /public/candles/{symbol}:
    get:
      summary: Candles
      description: Candles.
      operationId: getPublicCandlesSymbol
      x-api-path-slug: publiccandlessymbol-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: period
      - in: path
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - Candles
  /order:
    get:
      summary: List Your Current Open Orders
      description: List your current open orders.
      operationId: getOrder
      x-api-path-slug: order-get
      parameters:
      - in: query
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - List
      - Your
      - Current
      - Open
      - Orders
    post:
      summary: Create New Order
      description: Create new order.
      operationId: postOrder
      x-api-path-slug: order-post
      parameters:
      - in: formData
        name: clientOrderId
      - in: formData
        name: expireTime
      - in: formData
        name: price
      - in: formData
        name: quantity
      - in: formData
        name: side
      - in: formData
        name: stopPrice
      - in: formData
        name: strictValidate
        description: Strict validate amount and price precision without rounding
      - in: formData
        name: symbol
      - in: formData
        name: timeInForce
      - in: formData
        name: type
      responses:
        200:
          description: OK
      tags:
      - New
      - Order
    delete:
      summary: Cancel All Open Orders
      description: Cancel all open orders.
      operationId: deleteOrder
      x-api-path-slug: order-delete
      parameters:
      - in: formData
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - ""
      - Open
      - Orders
  /order/{clientOrderId}:
    get:
      summary: Get A Single Order By ClientOrderId
      description: Get a single order by clientorderid.
      operationId: getOrderClientorder
      x-api-path-slug: orderclientorderid-get
      parameters:
      - in: path
        name: clientOrderId
      - in: query
        name: wait
        description: Long polling wait timeout in milliseconds
      responses:
        200:
          description: OK
      tags:
      - Single
      - Order
      - By
      - ClientOrderId
    put:
      summary: Create New Order
      description: Create new order.
      operationId: putOrderClientorder
      x-api-path-slug: orderclientorderid-put
      parameters:
      - in: path
        name: clientOrderId
      - in: formData
        name: expireTime
      - in: formData
        name: price
      - in: formData
        name: quantity
      - in: formData
        name: side
      - in: formData
        name: stopPrice
      - in: formData
        name: strictValidate
        description: Strict validate amount and price precision without rounding
      - in: formData
        name: symbol
      - in: formData
        name: timeInForce
      - in: formData
        name: type
      responses:
        200:
          description: OK
      tags:
      - New
      - Order
    delete:
      summary: Cancel Order
      description: Cancel order.
      operationId: deleteOrderClientorder
      x-api-path-slug: orderclientorderid-delete
      parameters:
      - in: path
        name: clientOrderId
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Order
    patch:
      summary: Cancel Replace Order
      description: Cancel replace order.
      operationId: patchOrderClientorder
      x-api-path-slug: orderclientorderid-patch
      parameters:
      - in: path
        name: clientOrderId
      - in: formData
        name: price
      - in: formData
        name: quantity
      - in: formData
        name: requestClientId
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Replace
      - Order
  /trading/balance:
    get:
      summary: Get Trading Balance
      description: Get trading balance.
      operationId: getTradingBalance
      x-api-path-slug: tradingbalance-get
      responses:
        200:
          description: OK
      tags:
      - Trading
      - Balance
  /trading/fee/{symbol}:
    get:
      summary: Get Trading Fee Rate
      description: Get trading fee rate.
      operationId: getTradingFeeSymbol
      x-api-path-slug: tradingfeesymbol-get
      parameters:
      - in: path
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - Trading
      - Fee
      - Rate
  /history/trades:
    get:
      summary: Get Historical Trades
      description: Get historical trades.
      operationId: getHistoryTrades
      x-api-path-slug: historytrades-get
      parameters:
      - in: query
        name: by
        description: Filter field
      - in: query
        name: from
        description: If filter by timestamp, then datetime in iso format or timestamp
          in millisecond otherwise trade id
      - in: query
        name: limit
      - in: query
        name: offset
      - in: query
        name: sort
        description: Sort direction
      - in: query
        name: symbol
      - in: query
        name: till
        description: If filter by timestamp, then datetime in iso format or timestamp
          in millisecond otherwise trade id
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Trades
  /history/order:
    get:
      summary: Get Historical Orders
      description: Get historical orders.
      operationId: getHistoryOrder
      x-api-path-slug: historyorder-get
      parameters:
      - in: query
        name: clientOrderId
      - in: query
        name: from
        description: Datetime in iso format or timestamp in millisecond
      - in: query
        name: limit
      - in: query
        name: offset
      - in: query
        name: symbol
      - in: query
        name: till
        description: Datetime in iso format or timestamp in millisecond
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Orders
  /history/order/{id}/trades:
    get:
      summary: Get Historical Trades By Specified Order
      description: Get historical trades by specified order.
      operationId: getHistoryOrderTrades
      x-api-path-slug: historyorderidtrades-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Trades
      - By
      - Specified
      - Order
  /account/balance:
    get:
      summary: Get Main Acccount Balance
      description: Get main acccount balance.
      operationId: getAccountBalance
      x-api-path-slug: accountbalance-get
      responses:
        200:
          description: OK
      tags:
      - Main
      - Acccount
      - Balance
  /account/transactions:
    get:
      summary: Get Account Transactions
      description: Get account transactions.
      operationId: getAccountTransactions
      x-api-path-slug: accounttransactions-get
      parameters:
      - in: query
        name: by
        description: Filter field
      - in: query
        name: currency
      - in: query
        name: from
        description: Datetime in iso format or timestamp in millisecond, or index
      - in: query
        name: limit
      - in: query
        name: offset
      - in: query
        name: sort
        description: Sort direction
      - in: query
        name: till
        description: Datetime in iso format or timestamp in millisecond, or index
      responses:
        200:
          description: OK
      tags:
      - Account
      - Transactions
  /account/transactions/{id}:
    get:
      summary: Get Account Transaction By Id
      description: Get account transaction by id.
      operationId: getAccountTransactions
      x-api-path-slug: accounttransactionsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Account
      - Transaction
      - By
      - Id
  /account/crypto/withdraw:
    post:
      summary: Withdraw Crypro
      description: Withdraw crypro.
      operationId: postAccountCryptoWithdraw
      x-api-path-slug: accountcryptowithdraw-post
      parameters:
      - in: formData
        name: address
      - in: formData
        name: amount
      - in: formData
        name: autoCommit
        description: If Auto commit disabled you should commit it or rollback within
          1 hour
      - in: formData
        name: currency
      - in: formData
        name: includeFee
        description: If enabled, then fee will be subtracted from amount
      - in: formData
        name: networkFee
        description: Suggest preferred network fee
      - in: formData
        name: paymentId
      responses:
        200:
          description: OK
      tags:
      - Withdraw
      - Crypro
  /account/crypto/withdraw/{id}:
    put:
      summary: Commit Withdraw Crypro
      description: Commit withdraw crypro.
      operationId: putAccountCryptoWithdraw
      x-api-path-slug: accountcryptowithdrawid-put
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Commit
      - Withdraw
      - Crypro
    delete:
      summary: Rollback Withdraw Crypro
      description: Rollback withdraw crypro.
      operationId: deleteAccountCryptoWithdraw
      x-api-path-slug: accountcryptowithdrawid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Rollback
      - Withdraw
      - Crypro
  /account/crypto/address/{currency}:
    get:
      summary: Get Deposit Crypro Address
      description: Get deposit crypro address.
      operationId: getAccountCryptoAddressCurrency
      x-api-path-slug: accountcryptoaddresscurrency-get
      parameters:
      - in: path
        name: currency
      responses:
        200:
          description: OK
      tags:
      - Deposit
      - Crypro
      - Address
    post:
      summary: Create New Deposit Crypro Address
      description: Create new deposit crypro address.
      operationId: postAccountCryptoAddressCurrency
      x-api-path-slug: accountcryptoaddresscurrency-post
      parameters:
      - in: path
        name: currency
      responses:
        200:
          description: OK
      tags:
      - New
      - Deposit
      - Crypro
      - Address
  /account/transfer:
    post:
      summary: Transfer Amount To Trading
      description: Transfer amount to trading.
      operationId: postAccountTransfer
      x-api-path-slug: accounttransfer-post
      parameters:
      - in: formData
        name: amount
      - in: formData
        name: currency
      - in: formData
        name: type
      responses:
        200:
          description: OK
      tags:
      - Transfer
      - Amount
      - To
      - Trading