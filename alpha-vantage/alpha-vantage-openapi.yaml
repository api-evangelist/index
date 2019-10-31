swagger: "2.0"
x-collection-name: Alpha Vantage
x-complete: 1
info:
  title: Alpha Vantage
  description: alpha-vantage-apis-are-grouped-into-four-categories-1-stock-time-series-data-2-physical-and-digitalcrypto-currencies-e-g--bitcoin-3-stock-technical-indicators-and-4-sector-performances--all-apis-are-realtime-the-latest-data-points-are-derived-from-the-current-trading-day--
  version: 1.0.0
host: www.alphavantage.co
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /query?function=TIME_SERIES_INTRADAY:
    get:
      summary: Intraday Time Series
      description: This API returns intraday time series (timestamp, open, high, low,
        close, volume) of the equity specified, updated realtime.
      operationId: getIntradayTimeSeries
      x-api-path-slug: queryfunctiontime-series-intraday-get
      parameters:
      - in: query
        name: datatype
        description: By default, datatype=json
        type: string
        format: string
      - in: query
        name: interval
        description: The interval for series (1min, 5min, 15min, 30min, 60min)
        type: string
        format: string
      - in: query
        name: outputsize
        description: By default, outputsize=compact
        type: string
        format: string
      - in: query
        name: symbol
        description: The stocker ticker symbol
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Time Series
  /query?function=TIME_SERIES_DAILY_ADJUSTED:
    get:
      summary: Daily Time Series Adjusted
      description: This API returns daily time series (date, daily open, daily high,
        daily low, daily close, daily volume, daily adjusted close, and split/dividend
        events) of the equity specified, covering up to 20 years of historical data.
      operationId: getDailyTimeSeriesAdjusted
      x-api-path-slug: queryfunctiontime-series-daily-adjusted-get
      parameters:
      - in: query
        name: symbol
        description: The stocker ticker symbol
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Time Series
  /query?function=TIME_SERIES_WEEKLY:
    get:
      summary: Weekly Time Series
      description: This API returns weekly time series (last trading day of each week,
        weekly open, weekly high, weekly low, weekly close, weekly volume) of the
        equity specified, covering up to 20 years of historical data.
      operationId: getWeeklyTimeSeries
      x-api-path-slug: queryfunctiontime-series-weekly-get
      parameters:
      - in: query
        name: symbol
        description: The stocker ticker symbol
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Time Series
  /query?function=TIME_SERIES_DAILY:
    get:
      summary: Daily Time Series
      description: This API returns daily time series (date, daily open, daily high,
        daily low, daily close, daily volume) of the equity specified, covering up
        to 20 years of historical data.
      operationId: getDailyTimeSeries
      x-api-path-slug: queryfunctiontime-series-daily-get
      parameters:
      - in: query
        name: symbol
        description: The stocker ticker symbol
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Time Series
  /query?function=TIME_SERIES_MONTHLY:
    get:
      summary: Monthly Time Series
      description: This API returns monthly time series (last trading day of each
        month, monthly open, monthly high, monthly low, monthly close, monthly volume)
        of the equity specified, covering up to 20 years of historical data.
      operationId: getMonthlyTimeSeries
      x-api-path-slug: queryfunctiontime-series-monthly-get
      parameters:
      - in: query
        name: symbol
        description: The stocker ticker symbol
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Time Series
  /query?function=TIME_SERIES_MONTHLY_ADJUSTED:
    get:
      summary: Monthly Time Series Adjusted
      description: This API returns monthly adjusted time series (last trading day
        of each month, monthly open, monthly high, monthly low, monthly close, monthly
        adjusted close, monthly volume, monthly dividend) of the equity specified,
        covering up to 20 years of historical data.
      operationId: getMonthlyTimeSeriesAdjusted
      x-api-path-slug: queryfunctiontime-series-monthly-adjusted-get
      parameters:
      - in: query
        name: symbol
        description: The stocker ticker symbol
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Time Series
  /query?function=BATCH_STOCK_QUOTES:
    get:
      summary: Batch Stock Quotes
      description: The batch stock quotes API enables the querying of multiple stock
        quotes with a single API request, updated realtime. It may serve as a lightweight
        alternative to our core stock time series APIs above (which have richer content
        but are symbol-specific).
      operationId: getBatchStockQuotes
      x-api-path-slug: queryfunctionbatch-stock-quotes-get
      parameters:
      - in: query
        name: symbols
        description: Up to 100 stock symbols seperated by comma
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Time Series
      - Stock Quotes
  /query?function=CURRENCY_EXCHANGE_RATE:
    get:
      summary: Currency Exchange Rates
      description: Realtime currency exchange rates for physical and digital currencies.
      operationId: getCurrencyExchangeRates
      x-api-path-slug: queryfunctioncurrency-exchange-rate-get
      parameters:
      - in: query
        name: from_currency
        description: The currency you would like to get the exchange rate for
        type: string
        format: string
      - in: query
        name: to_currency
        description: The destination currency for the exchange rate
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Currency
      - Exchange Rates
  /query?function=DIGITAL_CURRENCY_INTRADAY:
    get:
      summary: Digital Currencies Intraday
      description: This API returns the realtime intraday time series (in 5-minute
        intervals) for any digital currency (e.g., BTC) traded on a specific market
        (e.g., CNY/Chinese Yuan). Prices and volumes are quoted in both the market-specific
        currency and USD.
      operationId: getDigitalCurrenciesIntraday
      x-api-path-slug: queryfunctiondigital-currency-intraday-get
      parameters:
      - in: query
        name: market
        description: The exchange market of your choice
        type: string
        format: string
      - in: query
        name: symbol
        description: The digital/crypto currency of your choice
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Digital Currencies
      - Intraday
      - Time Series
  /query?function=DIGITAL_CURRENCY_DAILY:
    get:
      summary: Digital Currencies Daily
      description: This API returns the daily historical time series for a digital
        currency (e.g., BTC) traded on a specific market (e.g., CNY/Chinese Yuan),
        refreshed daily at midnight (UTC). Prices and volumes are quoted in both the
        market-specific currency and USD.
      operationId: getDigitalCurrenciesDaily
      x-api-path-slug: queryfunctiondigital-currency-daily-get
      parameters:
      - in: query
        name: market
        description: The exchange market of your choice
        type: string
        format: string
      - in: query
        name: symbol
        description: The digital/crypto currency of your choice
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Digital Currencies
      - Daily
      - Time Series
  /query?function=DIGITAL_CURRENCY_WEEKLY:
    get:
      summary: Digital Currencies Weekly
      description: This API returns the weekly historical time series for a digital
        currency (e.g., BTC) traded on a specific market (e.g., CNY/Chinese Yuan),
        refreshed daily at midnight (UTC). Prices and volumes are quoted in both the
        market-specific currency and USD.
      operationId: getDigitalCurrenciesWeekly
      x-api-path-slug: queryfunctiondigital-currency-weekly-get
      parameters:
      - in: query
        name: market
        description: The exchange market of your choice
        type: string
        format: string
      - in: query
        name: symbol
        description: The digital/crypto currency of your choice
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Digital Currencies
      - Weekly
      - Time Series
  /query?function=DIGITAL_CURRENCY_MONTHLY:
    get:
      summary: Digital Currencies Monthly
      description: This API returns the monthly historical time series for a digital
        currency (e.g., BTC) traded on a specific market (e.g., CNY/Chinese Yuan),
        refreshed daily at midnight (UTC). Prices and volumes are quoted in both the
        market-specific currency and USD.
      operationId: getDigitalCurrenciesMonthly
      x-api-path-slug: queryfunctiondigital-currency-monthly-get
      parameters:
      - in: query
        name: market
        description: The exchange market of your choice
        type: string
        format: string
      - in: query
        name: symbol
        description: The digital/crypto currency of your choice
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Digital Currencies
      - Monthly
      - Time Series
  /query?function=SMA:
    get:
      summary: Simple Moving Average (SMA)
      description: This API returns the simple moving average (SMA) values.
      operationId: getSimpleMovingAverage
      x-api-path-slug: queryfunctionsma-get
      parameters:
      - in: query
        name: interval
        description: Time interval between two consecutive data points in the time
          series
        type: string
        format: string
      - in: query
        name: series_type
        description: The desired price type in the time series
        type: string
        format: string
      - in: query
        name: symbol
        description: The name of the equity of your choice
        type: string
        format: string
      - in: query
        name: time_period
        description: Number of data points used to calculate each moving average value
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Simple Moving Average
      - SMA
  /query?function=EMA:
    get:
      summary: Exponential Moving Average (EMA)
      description: This API returns the exponential moving average (EMA)
      operationId: getExponentialMovingAverage
      x-api-path-slug: queryfunctionema-get
      parameters:
      - in: query
        name: interval
        description: Time interval between two consecutive data points in the time
          series
        type: string
        format: string
      - in: query
        name: series_type
        description: The desired price type in the time series
        type: string
        format: string
      - in: query
        name: symbol
        description: The name of the equity of your choice
        type: string
        format: string
      - in: query
        name: time_period
        description: Number of data points used to calculate each moving average value
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Exponential Moving Average
      - EMA
  /query?function=MACD:
    get:
      summary: Moving Average Convergence / Divergence (MACD)
      description: This API returns the moving average convergence / divergence (MACD)
        values.
      operationId: getMovingAverageConvergenceDivergence
      x-api-path-slug: queryfunctionmacd-get
      parameters:
      - in: query
        name: interval
        description: Time interval between two consecutive data points in the time
          series
        type: string
        format: string
      - in: query
        name: series_type
        description: The desired price type in the time series
        type: string
        format: string
      - in: query
        name: symbol
        description: The name of the equity of your choice
        type: string
        format: string
      - in: query
        name: time_period
        description: Number of data points used to calculate each moving average value
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Moving Average Convergence
      - MACD
  /query?function=STOCH:
    get:
      summary: Stochastic Oscillator (STOCH)
      description: This API returns the stochastic oscillator (STOCH) values.
      operationId: getStochasticOscillator
      x-api-path-slug: queryfunctionstoch-get
      parameters:
      - in: query
        name: interval
        description: Time interval between two consecutive data points in the time
          series
        type: string
        format: string
      - in: query
        name: symbol
        description: The name of the equity of your choice
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Stochastic Oscillator
      - STOCH
  /query?function=RSI:
    get:
      summary: Relative Strength Index (RSI)
      description: This API returns the relative strength index (RSI) values.
      operationId: getRelativeStrengthIndex
      x-api-path-slug: queryfunctionrsi-get
      parameters:
      - in: query
        name: interval
        description: Time interval between two consecutive data points in the time
          series
        type: string
        format: string
      - in: query
        name: series_type
        description: The desired price type in the time series
        type: string
        format: string
      - in: query
        name: symbol
        description: The name of the equity of your choice
        type: string
        format: string
      - in: query
        name: time_period
        description: Number of data points used to calculate each moving average value
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Relative Strength Index
      - RSI
  /query?function=ADX:
    get:
      summary: Average Directional Movement Index (ADX)
      description: This API returns the average directional movement index (ADX) values.
      operationId: getAverageDirectionalMovementIndex
      x-api-path-slug: queryfunctionadx-get
      parameters:
      - in: query
        name: interval
        description: Time interval between two consecutive data points in the time
          series
        type: string
        format: string
      - in: query
        name: symbol
        description: The name of the equity of your choice
        type: string
        format: string
      - in: query
        name: time_period
        description: Number of data points used to calculate each moving average value
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Average Directional Movement Index
      - ADX
  /query?function=CCI:
    get:
      summary: Commodity Channel Index (CCI)
      description: This API returns the commodity channel index (CCI) values.
      operationId: getCommodityChannelIndex
      x-api-path-slug: queryfunctioncci-get
      parameters:
      - in: query
        name: interval
        description: Time interval between two consecutive data points in the time
          series
        type: string
        format: string
      - in: query
        name: symbol
        description: The name of the equity of your choice
        type: string
        format: string
      - in: query
        name: time_period
        description: Number of data points used to calculate each moving average value
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Commodity Channel Index
      - CCI
  /query?function=AROON:
    get:
      summary: Aroon (AROON)
      description: This API returns the Aroon (AROON) values.
      operationId: getArroon
      x-api-path-slug: queryfunctionaroon-get
      parameters:
      - in: query
        name: interval
        description: Time interval between two consecutive data points in the time
          series
        type: string
        format: string
      - in: query
        name: symbol
        description: The name of the equity of your choice
        type: string
        format: string
      - in: query
        name: time_period
        description: Number of data points used to calculate each moving average value
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Aroon
      - AROON
  /query?function=BBANDS:
    get:
      summary: Bollinger bands (BBANDS)
      description: This API returns the Bollinger bands (BBANDS) values.
      operationId: getbollingerBands
      x-api-path-slug: queryfunctionbbands-get
      parameters:
      - in: query
        name: interval
        description: Time interval between two consecutive data points in the time
          series
        type: string
        format: string
      - in: query
        name: series_type
        description: The desired price type in the time series
        type: string
        format: string
      - in: query
        name: symbol
        description: The name of the equity of your choice
        type: string
        format: string
      - in: query
        name: time_period
        description: Number of data points used to calculate each moving average value
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Bollinger bands
      - BBANDS
  /query?function=AD:
    get:
      summary: Chaikin A/D line (AD)
      description: This API returns the Chaikin A/D line (AD) values.
      operationId: getChalkinADLine
      x-api-path-slug: queryfunctionad-get
      parameters:
      - in: query
        name: interval
        description: Time interval between two consecutive data points in the time
          series
        type: string
        format: string
      - in: query
        name: symbol
        description: The name of the equity of your choice
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Chaikin A/D Line
      - AD)
  /query?function=OBV:
    get:
      summary: Balance Volume (OBV)
      description: This API returns the on balance volume (OBV) values.
      operationId: getBalanceVolume
      x-api-path-slug: queryfunctionobv-get
      parameters:
      - in: query
        name: interval
        description: Time interval between two consecutive data points in the time
          series
        type: string
        format: string
      - in: query
        name: symbol
        description: The name of the equity of your choice
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Balance Volume
      - OBV
  /query?function=SECTOR:
    get:
      summary: Sector Performance
      description: This API returns the realtime and historical sector performances
        calculated from S&P500 incumbents.
      operationId: getSectorPerformance
      x-api-path-slug: queryfunctionsector-get
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Sector
      - Performance