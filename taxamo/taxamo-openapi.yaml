swagger: "2.0"
x-collection-name: Taxamo
x-complete: 1
info:
  title: Taxamo
  description: taxamos-elegant-suite-of-apis-and-comprehensive-reporting-dashboard-enables-digital-merchants-to-easily-comply-with-eu-regulatory-requirements-on-tax-calculation-evidence-collection-tax-return-creation-and-data-storage-
  version: "1"
host: api.taxamo.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/dictionaries/countries:
    get:
      summary: Countries
      description: Countries.
      operationId: getCountriesDict
      x-api-path-slug: apiv1dictionariescountries-get
      parameters:
      - in: query
        name: tax_supported
        description: Should only countries with tax supported be listed?
      responses:
        200:
          description: OK
      tags:
      - Countries
  /api/v1/dictionaries/currencies:
    get:
      summary: Currencies
      description: Currencies.
      operationId: getCurrenciesDict
      x-api-path-slug: apiv1dictionariescurrencies-get
      responses:
        200:
          description: OK
      tags:
      - Currencies
  /api/v1/dictionaries/product_types:
    get:
      summary: Product Types
      description: Product types.
      operationId: getProductTypesDict
      x-api-path-slug: apiv1dictionariesproduct-types-get
      responses:
        200:
          description: OK
      tags:
      - Product
      - Types
  /api/v1/geoip:
    get:
      summary: Locate IP Address
      description: Locate ip address.
      operationId: locateMyIP
      x-api-path-slug: apiv1geoip-get
      responses:
        200:
          description: OK
      tags:
      - Locate
      - IP
      - Ress
  /api/v1/geoip/{ip}:
    get:
      summary: Locate Provided IP Address
      description: Locate provided ip address.
      operationId: locateGivenIP
      x-api-path-slug: apiv1geoipip-get
      parameters:
      - in: path
        name: ip
        description: IP address
      responses:
        200:
          description: OK
      tags:
      - Locate
      - Provided
      - IP
      - Ress
  /api/v1/reports/domestic/summary:
    get:
      summary: Calculate Domestic Summary
      description: Calculate domestic summary.
      operationId: getDomesticSummaryReport
      x-api-path-slug: apiv1reportsdomesticsummary-get
      parameters:
      - in: query
        name: country_code
        description: ISO 2-letter country code which will be used for determining
          which country is domestic
      - in: query
        name: currency_code
        description: ISO 3-letter currency code, e
      - in: query
        name: end_month
        description: Period end month in yyyy-MM format
      - in: query
        name: format
        description: Output format
      - in: query
        name: fx_date_type
        description: Which date should be used for FX
      - in: query
        name: start_month
        description: Period start month in yyyy-MM format
      responses:
        200:
          description: OK
      tags:
      - Calculate
      - Domestic
      - Summary
  /api/v1/reports/eu/vies:
    get:
      summary: Calculate EU VIES Report
      description: Calculate eu vies report.
      operationId: getEuViesReport
      x-api-path-slug: apiv1reportseuvies-get
      parameters:
      - in: query
        name: currency_code
        description: ISO 3-letter currency code, e
      - in: query
        name: end_month
        description: Period end month in yyyy-MM format
      - in: query
        name: eu_country_code
        description: ISO 2-letter country code which will be used for determining
          which country is domestic
      - in: query
        name: format
        description: Output format
      - in: query
        name: fx_date_type
        description: Which date should be used for FX
      - in: query
        name: lff_sequence_number
        description: Sequence number used to generate report in Large Filer Format
      - in: query
        name: period_length
        description: Length of report period
      - in: query
        name: start_month
        description: Period start month in yyyy-MM format
      - in: query
        name: tax_id
        description: MOSS-assigned tax ID - if not provided, merchants national tax
          number will be used
      - in: query
        name: transformation
        description: Which transformation should be applied
      responses:
        200:
          description: OK
      tags:
      - Calculate
      - EU
      - VIES
      - Report
  /api/v1/settlement/detailed_refunds:
    get:
      summary: Detailed Refunds
      description: Detailed refunds.
      operationId: getDetailedRefunds
      x-api-path-slug: apiv1settlementdetailed-refunds-get
      parameters:
      - in: query
        name: country_codes
        description: Comma separated list of 2-letter country codes
      - in: query
        name: date_from
        description: Take only refunds issued at or after the date
      - in: query
        name: date_to
        description: Take only refunds issued at or before the date
      - in: query
        name: format
        description: Output format
      - in: query
        name: limit
        description: Limit (no more than 1000, defaults to 100)
      - in: query
        name: offset
        description: Offset
      responses:
        200:
          description: OK
      tags:
      - Detailed
      - Refunds
  /api/v1/settlement/refunds:
    get:
      summary: Fetch Refunds
      description: Fetch refunds.
      operationId: getRefunds
      x-api-path-slug: apiv1settlementrefunds-get
      parameters:
      - in: query
        name: date_from
        description: Take only refunds issued at or after the date
      - in: query
        name: format
        description: Output format
      - in: query
        name: moss_country_code
        description: MOSS country code, used to determine currency
      - in: query
        name: tax_region
        description: Tax region key, defaults to EU for backwards compatibility
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Refunds
  /api/v1/settlement/summary/{quarter}:
    get:
      summary: Fetch Summary
      description: Fetch summary.
      operationId: getSettlementSummary
      x-api-path-slug: apiv1settlementsummaryquarter-get
      parameters:
      - in: query
        name: end_month
        description: Period end month in yyyy-MM format
      - in: query
        name: moss_country_code
        description: MOSS country code, used to determine currency
      - in: path
        name: quarter
        description: Quarter in yyyy-MM format
      - in: query
        name: start_month
        description: Period start month in yyyy-MM format
      - in: query
        name: tax_region
        description: Tax region key
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Summary
  /api/v1/settlement/{quarter}:
    get:
      summary: Fetch Settlement
      description: Fetch settlement.
      operationId: getSettlement
      x-api-path-slug: apiv1settlementquarter-get
      parameters:
      - in: query
        name: currency_code
        description: ISO 3-letter currency code, e
      - in: query
        name: end_month
        description: Period end month in yyyy-MM format
      - in: query
        name: format
        description: Output format
      - in: query
        name: moss_country_code
        description: MOSS country code, used to determine currency/region
      - in: query
        name: moss_tax_id
        description: MOSS-assigned tax ID - if not provided, merchants national tax
          number will be used
      - in: path
        name: quarter
        description: Quarter in yyyy-MM format
      - in: query
        name: refund_date_kind_override
        description: Set to order_date to show only refunds for the transactions in
          the selected reporting period
      - in: query
        name: start_month
        description: Period start month in yyyy-MM format
      - in: query
        name: tax_country_code
        description: Tax entity country code, used to determine currency/region
      - in: query
        name: tax_id
        description: MOSS-assigned tax ID - if not provided, merchants national tax
          number will be used
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Settlement
  /api/v1/stats/settlement/by_country:
    get:
      summary: Settlement By Country
      description: Settlement by country.
      operationId: getSettlementStatsByCountry
      x-api-path-slug: apiv1statssettlementby-country-get
      parameters:
      - in: query
        name: date_from
        description: Date from in yyyy-MM format
      - in: query
        name: date_to
        description: Date to in yyyy-MM format
      responses:
        200:
          description: OK
      tags:
      - Settlement
      - Country
  /api/v1/stats/settlement/by_taxation_type:
    get:
      summary: Settlement By Tax Type
      description: Settlement by tax type.
      operationId: getSettlementStatsByTaxationType
      x-api-path-slug: apiv1statssettlementby-taxation-type-get
      parameters:
      - in: query
        name: date_from
        description: Date from in yyyy-MM format
      - in: query
        name: date_to
        description: Date to in yyyy-MM format
      responses:
        200:
          description: OK
      tags:
      - Settlement
      - Tax
      - Type
  /api/v1/stats/settlement/daily:
    get:
      summary: Settlement Stats Over Time
      description: Settlement stats over time.
      operationId: getDailySettlementStats
      x-api-path-slug: apiv1statssettlementdaily-get
      parameters:
      - in: query
        name: date_from
        description: Date from in yyyy-MM format
      - in: query
        name: date_to
        description: Date to in yyyy-MM format
      - in: query
        name: interval
        description: Interval type - day, week, month
      responses:
        200:
          description: OK
      tags:
      - Settlement
      - Stats
      - Over
      - Time
  /api/v1/stats/transactions:
    get:
      summary: Transaction Stats
      description: Transaction stats.
      operationId: getTransactionsStats
      x-api-path-slug: apiv1statstransactions-get
      parameters:
      - in: query
        name: date_from
        description: Date from in yyyy-MM format
      - in: query
        name: date_to
        description: Date to in yyyy-MM format
      - in: query
        name: interval
        description: Interval
      responses:
        200:
          description: OK
      tags:
      - Transaction
      - Stats
  /api/v1/stats/transactions/by_country:
    get:
      summary: Settlement By Country
      description: Settlement by country.
      operationId: getTransactionsStatsByCountry
      x-api-path-slug: apiv1statstransactionsby-country-get
      parameters:
      - in: query
        name: date_from
        description: Date from in yyyy-MM format
      - in: query
        name: date_to
        description: Date to in yyyy-MM format
      - in: query
        name: global_currency_code
        description: Global currency code to use for conversion - in addition to countrys
          currency if rate is available
      responses:
        200:
          description: OK
      tags:
      - Settlement
      - Country
  /api/v1/tax/calculate:
    get:
      summary: Simple Tax
      description: Simple tax.
      operationId: calculateSimpleTax
      x-api-path-slug: apiv1taxcalculate-get
      parameters:
      - in: query
        name: amount
        description: Amount
      - in: query
        name: billing_country_code
        description: Billing two letter ISO country code
      - in: query
        name: buyer_credit_card_prefix
        description: First 6 digits of buyers credit card prefix
      - in: query
        name: buyer_tax_number
        description: Buyers tax number - EU VAT number for example
      - in: query
        name: currency_code
        description: Currency code for transaction - e
      - in: query
        name: force_country_code
        description: Two-letter ISO country code, e
      - in: query
        name: invoice_address_city
        description: Invoice address/postal_code
      - in: query
        name: invoice_address_postal_code
        description: Invoice address/postal_code
      - in: query
        name: invoice_address_region
        description: Invoice address/region
      - in: query
        name: order_date
        description: Order date in yyyy-MM-dd format, in merchants timezone
      - in: query
        name: product_type
        description: Product type, according to dictionary /dictionaries/product_types
      - in: query
        name: quantity
        description: Quantity Defaults to 1
      - in: query
        name: tax_deducted
        description: If the transaction is in a country supported by Taxamo, but the
          tax is not calculated due to merchant settings or EU B2B transaction for
          example
      - in: query
        name: total_amount
        description: Total amount
      - in: query
        name: unit_price
        description: Unit price
      responses:
        200:
          description: OK
      tags:
      - Simple
      - Tax
    post:
      summary: Calculate Tax
      description: Calculate tax.
      operationId: calculateTax
      x-api-path-slug: apiv1taxcalculate-post
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Calculate
      - Tax
  /api/v1/tax/location/calculate:
    get:
      summary: Calculate Location
      description: Calculate location.
      operationId: calculateTaxLocation
      x-api-path-slug: apiv1taxlocationcalculate-get
      parameters:
      - in: query
        name: billing_country_code
        description: Billing two letter ISO country code
      - in: query
        name: buyer_credit_card_prefix
        description: First 6 digits of buyers credit card prefix
      responses:
        200:
          description: OK
      tags:
      - Calculate
      - Location
  /api/v1/tax/vat_numbers/{tax_number}/validate:
    get:
      summary: Validate VAT Number
      description: Validate vat number.
      operationId: validateTaxNumber
      x-api-path-slug: apiv1taxvat-numberstax-numbervalidate-get
      parameters:
      - in: query
        name: country_code
        description: Two-letter ISO country code
      - in: path
        name: tax_number
        description: Tax number
      responses:
        200:
          description: OK
      tags:
      - Validate
      - VAT
      - Number
  /api/v1/transactions:
    get:
      summary: Browse Transactions
      description: Browse transactions.
      operationId: listTransactions
      x-api-path-slug: apiv1transactions-get
      parameters:
      - in: query
        name: currency_code
        description: Three letter ISO currency code
      - in: query
        name: filter_text
        description: Filtering expression
      - in: query
        name: format
        description: Output format - supports csv value for this operation
      - in: query
        name: has_note
        description: Return only transactions with a note field set
      - in: query
        name: invoice_number
        description: Transaction invoice number
      - in: query
        name: key_or_custom_id
        description: Taxamo provided transaction key or custom id
      - in: query
        name: limit
        description: Limit (no more than 1000, defaults to 100)
      - in: query
        name: offset
        description: Offset
      - in: query
        name: order_date_from
        description: Order date from in yyyy-MM-dd format
      - in: query
        name: order_date_to
        description: Order date to in yyyy-MM-dd format
      - in: query
        name: original_transaction_key
        description: Taxamo provided original transaction key
      - in: query
        name: sort_reverse
        description: If true, results are sorted in descending order
      - in: query
        name: statuses
        description: Comma separated list of of transaction statuses
      - in: query
        name: tax_country_code
        description: Two letter ISO tax country code
      - in: query
        name: tax_country_codes
        description: Comma separated list of two letter ISO tax country codes
      - in: query
        name: total_amount_greater_than
        description: Return only transactions with total amount greater than given
          number
      - in: query
        name: total_amount_less_than
        description: Return only transactions with total amount less than a given
          number
      responses:
        200:
          description: OK
      tags:
      - Browse
      - Transactions
    post:
      summary: Store Transaction
      description: Store transaction.
      operationId: createTransaction
      x-api-path-slug: apiv1transactions-post
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Store
      - Transaction
  /api/v1/transactions/{key}:
    delete:
      summary: Delete Transaction
      description: Delete transaction.
      operationId: cancelTransaction
      x-api-path-slug: apiv1transactionskey-delete
      parameters:
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Transaction
    get:
      summary: Retrieve Transaction Data.
      description: Retrieve transaction data..
      operationId: getTransaction
      x-api-path-slug: apiv1transactionskey-get
      parameters:
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Transaction
      - Data
    put:
      summary: Update Transaction
      description: Update transaction.
      operationId: updateTransaction
      x-api-path-slug: apiv1transactionskey-put
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Transaction
  /api/v1/transactions/{key}/confirm:
    post:
      summary: Confirm Transaction
      description: Confirm transaction.
      operationId: confirmTransaction
      x-api-path-slug: apiv1transactionskeyconfirm-post
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Confirm
      - Transaction
  /api/v1/transactions/{key}/invoice/refunds/{refund_note_number}/send_email:
    post:
      summary: Email Credit Note
      description: Email credit note.
      operationId: emailRefund
      x-api-path-slug: apiv1transactionskeyinvoicerefundsrefund-note-numbersend-email-post
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: key
        description: Transaction key
      - in: path
        name: refund_note_number
        description: Refund note id
      responses:
        200:
          description: OK
      tags:
      - Email
      - Credit
      - Note
  /api/v1/transactions/{key}/invoice/send_email:
    post:
      summary: Email Invoice
      description: Email invoice.
      operationId: emailInvoice
      x-api-path-slug: apiv1transactionskeyinvoicesend-email-post
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Email
      - Invoice
  /api/v1/transactions/{key}/payments:
    get:
      summary: List Payments
      description: List payments.
      operationId: listPayments
      x-api-path-slug: apiv1transactionskeypayments-get
      parameters:
      - in: path
        name: key
        description: Transaction key
      - in: query
        name: limit
        description: Max record count (no more than 100, defaults to 10)
      - in: query
        name: offset
        description: How many records need to be skipped, defaults to 0
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
    post:
      summary: Register A Payment
      description: Register a payment.
      operationId: createPayment
      x-api-path-slug: apiv1transactionskeypayments-post
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Register
      - Payment
  /api/v1/transactions/{key}/payments/capture:
    post:
      summary: Capture Payment
      description: Capture payment.
      operationId: capturePayment
      x-api-path-slug: apiv1transactionskeypaymentscapture-post
      parameters:
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Capture
      - Payment
  /api/v1/transactions/{key}/refunds:
    get:
      summary: Get Transaction Refunds
      description: Get transaction refunds.
      operationId: listRefunds
      x-api-path-slug: apiv1transactionskeyrefunds-get
      parameters:
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Transaction
      - Refunds
    post:
      summary: Create A Refund
      description: Create a refund.
      operationId: createRefund
      x-api-path-slug: apiv1transactionskeyrefunds-post
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Refund
  /api/v1/transactions/{key}/unconfirm:
    post:
      summary: Un-confirm The Transaction
      description: Un-confirm the transaction.
      operationId: unconfirmTransaction
      x-api-path-slug: apiv1transactionskeyunconfirm-post
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: key
        description: Transaction key
      responses:
        200:
          description: OK
      tags:
      - Un-confirm
      - Transaction
  /api/v1/verification/sms:
    post:
      summary: Create SMS Token
      description: Create sms token.
      operationId: createSMSToken
      x-api-path-slug: apiv1verificationsms-post
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - SMS
      - Token
  /api/v1/verification/sms/{token}:
    get:
      summary: Verify SMS Token
      description: Verify sms token.
      operationId: verifySMSToken
      x-api-path-slug: apiv1verificationsmstoken-get
      parameters:
      - in: path
        name: token
        description: Provided token
      responses:
        200:
          description: OK
      tags:
      - Verify
      - SMS
      - Token