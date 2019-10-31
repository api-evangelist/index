swagger: "2.0"
x-collection-name: PayJunction
x-complete: 1
info:
  title: PayJunction API Basic
  description: todo-add-description
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /customers:
    get:
      summary: Get Customers
      description: Gets a list of 15 customers
      operationId: CustomersGet
      x-api-path-slug: customers-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: offset
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
  /customers/{customerId}:
    get:
      summary: Get Customers
      description: /customers/{customerid}.
      operationId: CustomersByCustomerIdGet
      x-api-path-slug: customerscustomerid-get
      parameters:
      - in: path
        name: customerId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
    put:
      summary: Put Customers
      description: /customers/{customerid}.
      operationId: CustomersByCustomerIdPut
      x-api-path-slug: customerscustomerid-put
      parameters:
      - in: formData
        name: companyName
      - in: formData
        name: custom1
      - in: path
        name: customerId
      - in: formData
        name: defaultAddressId
      - in: formData
        name: email
      - in: formData
        name: firstName
      - in: formData
        name: identifier
      - in: formData
        name: jobTitle
      - in: formData
        name: lastName
      - in: formData
        name: middleName
      - in: formData
        name: phone
      - in: formData
        name: phone2
      - in: formData
        name: website
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
    delete:
      summary: Delete Customers
      description: /customers/{customerid}.
      operationId: CustomersByCustomerIdDelete
      x-api-path-slug: customerscustomerid-delete
      parameters:
      - in: path
        name: customerId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
  /customers/:
    post:
      summary: Post Customers
      description: Add a new customer
      operationId: CustomersPost
      x-api-path-slug: customers-post
      parameters:
      - in: formData
        name: companyName
        description: Text, Max Length 64
      - in: formData
        name: custom1
        description: Text, Max Length 32
      - in: formData
        name: email
        description: Email (1), Max Length 128
      - in: formData
        name: firstName
        description: Text, Max Length 16
      - in: formData
        name: identifier
        description: Text, Max Length 64
      - in: formData
        name: jobTitle
        description: Text, Max Length 32
      - in: formData
        name: lastName
        description: Text, Max Length 32
      - in: formData
        name: middleName
        description: Text, Max Length 32
      - in: formData
        name: phone
        description: Phone Number, Max Length 24, Must contain at least 10 digits
      - in: formData
        name: phone2
        description: Phone Number, Max Length 24, Must contain at least 10 digits
      - in: formData
        name: website
        description: Text, Max Length 128
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
  /customers/{customerId}/notes:
    get:
      summary: Get Customers Notes
      description: /customers/{customerid}/notes.
      operationId: CustomersNotesByCustomerIdGet
      x-api-path-slug: customerscustomeridnotes-get
      parameters:
      - in: path
        name: customerId
      - in: query
        name: limit
      - in: query
        name: offset
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Notes
    post:
      summary: Post Customers Notes
      description: /customers/{customerid}/notes.
      operationId: CustomersNotesByCustomerIdPost
      x-api-path-slug: customerscustomeridnotes-post
      parameters:
      - in: path
        name: customerId
      - in: formData
        name: note
        description: Max Length 2048
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Notes
  /customers/{customerId}/notes/{noteId}:
    get:
      summary: Get Customers Notes
      description: /customers/{customerid}/notes/{noteid}.
      operationId: CustomersNotesByCustomerIdAndNoteIdGet
      x-api-path-slug: customerscustomeridnotesnoteid-get
      parameters:
      - in: path
        name: customerId
      - in: path
        name: noteId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Notes
    put:
      summary: Put Customers Notes
      description: /customers/{customerid}/notes/{noteid}.
      operationId: CustomersNotesByCustomerIdAndNoteIdPut
      x-api-path-slug: customerscustomeridnotesnoteid-put
      parameters:
      - in: header
        name: Content-Type
      - in: path
        name: customerId
      - in: formData
        name: note
        description: Max Length 2048
      - in: path
        name: noteId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Notes
    delete:
      summary: Delete Customers Notes
      description: /customers/{customerid}/notes/{noteid}.
      operationId: CustomersNotesByCustomerIdAndNoteIdDelete
      x-api-path-slug: customerscustomeridnotesnoteid-delete
      parameters:
      - in: path
        name: customerId
      - in: path
        name: noteId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Notes
  /customers/{customerId}/vaults/:
    get:
      summary: Get Customers Vaults
      description: Retrieve customer's payment vaults
      operationId: CustomersVaultsByCustomerIdGet
      x-api-path-slug: customerscustomeridvaults-get
      parameters:
      - in: path
        name: customerId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Vaults
  /customers/{customerId}/vaults/{vaultId}:
    get:
      summary: Get Customers Vaults
      description: /customers/{customerid}/vaults/{vaultid}.
      operationId: CustomersVaultsByCustomerIdAndVaultIdGet
      x-api-path-slug: customerscustomeridvaultsvaultid-get
      parameters:
      - in: path
        name: customerId
      - in: path
        name: vaultId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Vaults
    delete:
      summary: Delete Customers Vaults
      description: /customers/{customerid}/vaults/{vaultid}.
      operationId: CustomersVaultsByCustomerIdAndVaultIdDelete
      x-api-path-slug: customerscustomeridvaultsvaultid-delete
      parameters:
      - in: path
        name: customerId
      - in: path
        name: vaultId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Vaults
  /customers/{customerId}/vaults:
    post:
      summary: Post Customers Vaults
      description: /customers/{customerid}/vaults (card).
      operationId: CustomersVaultsByCustomerIdPost2
      x-api-path-slug: customerscustomeridvaults-post
      parameters:
      - in: formData
        name: address
      - in: formData
        name: addressId
      - in: formData
        name: cardExpMonth
        description: 1-12
      - in: formData
        name: cardExpYear
        description: YYYY, YY
      - in: formData
        name: cardNumber
        description: 5105105105105100,5105-1051-0510-5100,5105 1051 0510 5100
      - in: formData
        name: city
      - in: path
        name: customerId
      - in: formData
        name: state
      - in: header
        name: X-PJ-Application-Key
      - in: formData
        name: zip
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Vaults
  /customers/{customerId}/vaults/{achVault}:
    put:
      summary: Put Customers Vaults ACH Vault
      description: /customers/{customerid}/vaults/{vaultid} (ach).
      operationId: CustomersVaultsByCustomerIdAndAchVaultPut
      x-api-path-slug: customerscustomeridvaultsachvault-put
      parameters:
      - in: formData
        name: achAccountType
        description: CHECKING, SAVINGS
      - in: formData
        name: achType
        description: CCD, PPD, TEL, WEB
      - in: path
        name: achVault
      - in: formData
        name: address
      - in: formData
        name: addressId
      - in: formData
        name: city
      - in: path
        name: customerId
      - in: formData
        name: state
      - in: header
        name: X-PJ-Application-Key
      - in: formData
        name: zip
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Vaults
      - ACH
      - Vault
  /customers/{customerId}/vaults/{cardVault}:
    put:
      summary: Put Customers Vaults Card Vault
      description: /customers/{customerid}/vaults/{vaultid} (card).
      operationId: CustomersVaultsByCustomerIdAndCardVaultPut
      x-api-path-slug: customerscustomeridvaultscardvault-put
      parameters:
      - in: formData
        name: address
      - in: formData
        name: addressId
      - in: formData
        name: cardExpMonth
        description: 1-12
      - in: formData
        name: cardExpYear
        description: YYYY, YY
      - in: path
        name: cardVault
      - in: formData
        name: city
      - in: path
        name: customerId
      - in: formData
        name: state
      - in: header
        name: X-PJ-Application-Key
      - in: formData
        name: zip
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Vaults
      - Card
      - Vault
  /customers/{customerId}/addresses:
    get:
      summary: Get Customers Addresses
      description: Gets a list of a customer's addresses.
      operationId: CustomersAddressesByCustomerIdGet
      x-api-path-slug: customerscustomeridaddresses-get
      parameters:
      - in: path
        name: customerId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Resses
    post:
      summary: Post Customers Addresses
      description: /customers/{customerid}/addresses/.
      operationId: CustomersAddressesByCustomerIdPost
      x-api-path-slug: customerscustomeridaddresses-post
      parameters:
      - in: formData
        name: address
        description: Text, Max Length 128
      - in: formData
        name: city
        description: Text, Max Length 32
      - in: formData
        name: country
        description: Text, Max Length 32
      - in: path
        name: customerId
      - in: formData
        name: state
        description: Text, Max Length 32
      - in: header
        name: X-PJ-Application-Key
      - in: formData
        name: zip
        description: Text, Max Length 16
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Resses
  /customers/{customerId}/addresses/{addressId}:
    get:
      summary: Get Customers Addresses
      description: /customers/{customerid}/addresses/{addressid}.
      operationId: CustomersAddressesByCustomerIdAndAddressIdGet
      x-api-path-slug: customerscustomeridaddressesaddressid-get
      parameters:
      - in: path
        name: addressId
      - in: path
        name: customerId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Resses
    put:
      summary: Put Customers Addresses
      description: /customers/{customerid}/addresses/{addressid}.
      operationId: CustomersAddressesByCustomerIdAndAddressIdPut
      x-api-path-slug: customerscustomeridaddressesaddressid-put
      parameters:
      - in: formData
        name: address
      - in: path
        name: addressId
      - in: formData
        name: city
      - in: formData
        name: country
      - in: path
        name: customerId
      - in: formData
        name: state
      - in: header
        name: X-PJ-Application-Key
      - in: formData
        name: zip
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Resses
    delete:
      summary: Delete Customers Addresses
      description: /customers/{customerid}/addresses/{addressid}.
      operationId: CustomersAddressesByCustomerIdAndAddressIdDelete
      x-api-path-slug: customerscustomeridaddressesaddressid-delete
      parameters:
      - in: path
        name: addressId
      - in: header
        name: Content-Type
      - in: path
        name: customerId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Resses
  /transactions:
    post:
      summary: Post Transactions
      description: /transactions/ (swiped cc).
      operationId: TransactionsPost6
      x-api-path-slug: transactions-post
      parameters:
      - in: formData
        name: action
      - in: formData
        name: amountBase
      - in: formData
        name: billingCompanyName
      - in: formData
        name: billingFirstName
      - in: formData
        name: billingLastName
      - in: formData
        name: cardTrack
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
  /transactions/:
    get:
      summary: Get Transactions
      description: 'Not Available At Time at Time of Publishing this collection: Get
        a list of transactions'
      operationId: TransactionsGet
      x-api-path-slug: transactions-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: offset
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
  /transactions/{transactionId}:
    get:
      summary: Get Transactions
      description: /transactions/{transactionid}.
      operationId: TransactionsByTransactionIdGet
      x-api-path-slug: transactionstransactionid-get
      parameters:
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
    put:
      summary: Put Transactions
      description: Update an unsettled transaction
      operationId: TransactionsByTransactionIdPut
      x-api-path-slug: transactionstransactionid-put
      parameters:
      - in: formData
        name: amountBase
      - in: formData
        name: amountReject
      - in: formData
        name: amountShipping
      - in: formData
        name: amountTax
      - in: formData
        name: amountTip
      - in: header
        name: Content-Type
      - in: formData
        name: status
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
  /transactions/{transactionId}/notes:
    get:
      summary: Get Transactions Notes
      description: Get a list of notes for a transaction
      operationId: TransactionsNotesByTransactionIdGet
      x-api-path-slug: transactionstransactionidnotes-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: offset
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Notes
    post:
      summary: Post Transactions Notes
      description: /transactions/{transactionid}/notes/.
      operationId: TransactionsNotesByTransactionIdPost
      x-api-path-slug: transactionstransactionidnotes-post
      parameters:
      - in: formData
        name: note
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Notes
  /transactions/{transactionId}/notes/{noteId}:
    get:
      summary: Get Transactions Notes
      description: /transactions/{transactionid}/notes/{noteid}.
      operationId: TransactionsNotesByTransactionIdAndNoteIdGet
      x-api-path-slug: transactionstransactionidnotesnoteid-get
      parameters:
      - in: path
        name: noteId
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Notes
    put:
      summary: Put Transactions Notes
      description: /transactions/{transactionid}/notes/{noteid}.
      operationId: TransactionsNotesByTransactionIdAndNoteIdPut
      x-api-path-slug: transactionstransactionidnotesnoteid-put
      parameters:
      - in: formData
        name: note
      - in: path
        name: noteId
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Notes
    delete:
      summary: Delete Transactions Notes
      description: /transactions/{transactionid}/notes/{noteid}.
      operationId: TransactionsNotesByTransactionIdAndNoteIdDelete
      x-api-path-slug: transactionstransactionidnotesnoteid-delete
      parameters:
      - in: path
        name: noteId
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Notes
  /transactions/{transactionId}/signature/capture:
    post:
      summary: Post Transactions Signature Capture
      description: Capture a signature using the scriptel signature capture
      operationId: TransactionsSignatureCaptureByTransactionIdPost
      x-api-path-slug: transactionstransactionidsignaturecapture-post
      parameters:
      - in: formData
        name: signature
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Signature
      - Capture
  /transactions/{transactionId}/receipts/latest/email:
    post:
      summary: Post Transactions Receipts Latest Email
      description: /transactions/{transactionid}/receipts/latest/email.
      operationId: TransactionsReceiptsLatestEmailByTransactionIdPost
      x-api-path-slug: transactionstransactionidreceiptslatestemail-post
      parameters:
      - in: formData
        name: replyTo
      - in: formData
        name: requestSignature
      - in: formData
        name: to
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Receipts
      - Latest
      - Email
  /transactions/{transactionId}/receipts:
    get:
      summary: Get Transactions Receipts
      description: Get all of the signed receipts for a transaction.
      operationId: TransactionsReceiptsByTransactionIdGet
      x-api-path-slug: transactionstransactionidreceipts-get
      parameters:
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Receipts
  /transactions/{transactionId}/receipts/latest:
    get:
      summary: Get Transactions Receipts Latest
      description: Retrieve the most recent version of the receipt.
      operationId: TransactionsReceiptsLatestByTransactionIdGet
      x-api-path-slug: transactionstransactionidreceiptslatest-get
      parameters:
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Receipts
      - Latest
  /transactions/{transactionId}/receipts/latest/thermal:
    get:
      summary: Get Transactions Receipts Latest Thermal
      description: Get the most recent version of the thermal receipt HTML Document
      operationId: TransactionsReceiptsLatestThermalByTransactionIdGet
      x-api-path-slug: transactionstransactionidreceiptslatestthermal-get
      parameters:
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Receipts
      - Latest
      - Thermal
  /transactions/{transactionId}/receipts/latest/fullpage:
    get:
      summary: Get Transactions Receipts Latest Fullpage
      description: Get the most recent version of the full page (8.5x11) receipt HTML
        document
      operationId: TransactionsReceiptsLatestFullpageByTransactionIdGet
      x-api-path-slug: transactionstransactionidreceiptslatestfullpage-get
      parameters:
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Receipts
      - Latest
      - Fullpage
  /transactions/{transactionId}/receipts/unsigned:
    get:
      summary: Get Transactions Receipts Unsigned
      description: /transactions/{transactionid}/receipts/unsigned.
      operationId: TransactionsReceiptsUnsignedByTransactionIdGet
      x-api-path-slug: transactionstransactionidreceiptsunsigned-get
      parameters:
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Receipts
      - Unsigned
  /transactions/{transactionId}/receipts/unsigned/thermal:
    get:
      summary: Get Transactions Receipts Unsigned Thermal
      description: /transactions/{transactionid}/receipts/unsigned/thermal.
      operationId: TransactionsReceiptsUnsignedThermalByTransactionIdGet
      x-api-path-slug: transactionstransactionidreceiptsunsignedthermal-get
      parameters:
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Receipts
      - Unsigned
      - Thermal
  /transactions/{transactionId}/receipts/unsigned/fullpage:
    get:
      summary: Get Transactions Receipts Unsigned Fullpage
      description: /transactions/{transactionid}/receipts/unsigned/fullpage.
      operationId: TransactionsReceiptsUnsignedFullpageByTransactionIdGet
      x-api-path-slug: transactionstransactionidreceiptsunsignedfullpage-get
      parameters:
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Receipts
      - Unsigned
      - Fullpage
  /transactions/{transactionId}/receipt/{receiptId}:
    get:
      summary: Get Transactions Receipt Receiptid
      description: /transactions/{transactionid}/receipts/{receiptid}.
      operationId: TransactionsReceiptByTransactionIdAndReceiptIdGet
      x-api-path-slug: transactionstransactionidreceiptreceiptid-get
      parameters:
      - in: path
        name: receiptId
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Receipt
      - Receiptid
  /webhooks:
    get:
      summary: Get Webhooks
      description: Gets a list of webhooks
      operationId: WebhooksGet
      x-api-path-slug: webhooks-get
      parameters:
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Webhooks
    post:
      summary: Post Webhooks
      description: /webhooks/{webhooks}.
      operationId: WebhooksPost
      x-api-path-slug: webhooks-post
      parameters:
      - in: query
        name: event
      - in: formData
        name: secret
        description: Text, max length 255
      - in: formData
        name: url
        description: Text, URL with max length 255
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Webhooks
  /webhooks/{webhookId}:
    put:
      summary: Put Webhooks
      description: /webhooks/{webhookid}.
      operationId: WebhooksByWebhookIdPut
      x-api-path-slug: webhookswebhookid-put
      parameters:
      - in: formData
        name: secret
        description: Text, max length 255
      - in: formData
        name: url
        description: Text, URL with max length 255
      - in: path
        name: webhookId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Webhooks
    delete:
      summary: Delete Webhooks
      description: /webhooks/{webhookid}.
      operationId: WebhooksByWebhookIdDelete
      x-api-path-slug: webhookswebhookid-delete
      parameters:
      - in: path
        name: webhookId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Webhooks
  /terminals:
    get:
      summary: Get Terminals
      description: Get a list of Terminal Id's for an account.
      operationId: TerminalsGet
      x-api-path-slug: terminals-get
      parameters:
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Terminals
  /smartterminals/{smartTerminaIId}/request-payment:
    post:
      summary: Post Smart Trminals Request Payment
      description: /smartterminals/{smartterminald}/request-payment.
      operationId: SmartterminalsRequestPaymentBySmartTerminaIIdPost
      x-api-path-slug: smartterminalssmartterminaiidrequestpayment-post
      parameters:
      - in: query
        name: amountBase
      - in: formData
        name: invoiceNumber
        description: NumericAn invoice number to include in the transaction details
      - in: formData
        name: showReceiptPrompt
        description: true | falsetrue - Displays the receipt prompt
      - in: path
        name: smartTerminaIId
      - in: query
        name: terminalId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Smart
      - Trminals
      - Request
      - Payment
  /smartterminals/{smartTerminaIId}/main:
    post:
      summary: Post Smart Terminals Main
      description: "Returns the Smart Terminal to the main \"Smart Terminal by PayJunction\"
        screen to await a new transaction request. \n\nFor instance, this request
        can be used when a user decides to cancel a Smart Terminal payment request.
        When this request is sent, the Smart Terminal will return to the main screen
        that reads \"Smart Terminal by PayJunction\", preventing the customer from
        making a payment.\n\nNote: If the customer has already inserted the chip card,
        or swiped the card, then the transaction is already processed and it is too
        late to cancel the payment request. In this case, the transaction should be
        voided instead."
      operationId: SmartterminalsMainBySmartTerminaIIdPost
      x-api-path-slug: smartterminalssmartterminaiidmain-post
      parameters:
      - in: path
        name: smartTerminaIId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Smart
      - Terminals
      - Main
  /smartterminals:
    get:
      summary: Get Smart Terminals
      description: Get a list of Smart Terminals for an account
      operationId: SmartterminalsGet
      x-api-path-slug: smartterminals-get
      parameters:
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Smart
      - Terminals
  /smartterminals/requests/{requestPaymentId}:
    get:
      summary: Get Smart Terminals Requests
      description: "Gets the status of a Smart Terminal payment request by querying
        the requestPaymentId returned by POST /smartterminals/{smartterminalId}/request-payment\n\nThe
        status of a payment request can be queried up to 1 day after the Smart Terminal
        payment request has been completed. After this cut off the requestPaymentId
        is purged and will return a 404 Not Found when queried. \n\nIn order to discourage
        busy polling, requests to this endpoint are rate limited to 1 request every
        2 seconds per request."
      operationId: SmartterminalsRequestsByRequestPaymentIdGet
      x-api-path-slug: smartterminalsrequestsrequestpaymentid-get
      parameters:
      - in: path
        name: requestPaymentId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Smart
      - Terminals
      - Requests