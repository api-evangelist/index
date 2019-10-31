swagger: "2.0"
x-collection-name: Intuit
x-complete: 1
info:
  title: QuickBooks Online V3 API
  description: the-quickbooks-online-accounting-api-is-a-restful-api-that-is-used-to-access-quickbooks-companies-docs-
  version: 1.0.0
host: DefaultParameterValue
basePath: /v3/company/DefaultParameterValue
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cdc:
    get:
      summary: Get CDC
      description: |-
        Retrive changed Bill and invoice objects since Aug10,2016
        Method - GET
      operationId: getCdc
      x-api-path-slug: cdc-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: changedSince
      - in: header
        name: Content-Type
      - in: query
        name: entities
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - CDC
  /query:
    post:
      summary: Post Query
      description: |-
        Read all transfer objects using the 'Query' endpoint
        Method : POST
      operationId: postQuery
      x-api-path-slug: query-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Query
  /estimate/163:
    get:
      summary: Get Estimate
      description: |-
        Read an Estimate object by Id
        Method : POST
      operationId: getEstimate163
      x-api-path-slug: estimate163-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Estimate
  /invoice:
    post:
      summary: Post Invoice
      description: |-
        Create an invoice object
        Method : POST
      operationId: postInvoice
      x-api-path-slug: invoice-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Invoice
  /term:
    post:
      summary: Post Term
      description: |-
        Update a term object
        Method : POST

        Term object can't be deleted parmanently. It can only be deactived by setting the 'Active' attribute to false.
      operationId: postTerm
      x-api-path-slug: term-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Term
  /preferences:
    get:
      summary: Get Preferences
      description: |-
        Read the preference object
        Method : POST
      operationId: getPreferences
      x-api-path-slug: preferences-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Preferences
    post:
      summary: Post Preferences
      description: |-
        Update the preference object endpoint
        Method : POST
      operationId: postPreferences
      x-api-path-slug: preferences-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Preferences
  /reports/InventoryValuationSummary:
    get:
      summary: Get Reports Inventory Valuation Summary
      description: |-
        Report - Inventory Valuation Summary
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/inventory%20valuation
      operationId: getReportsInventoryvaluationsummary
      x-api-path-slug: reportsinventoryvaluationsummary-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Inventory
      - Valuation
      - Summary
  /purchase:
    post:
      summary: Post Purchase
      description: |-
        Create a puchase object
        Method : POST
      operationId: postPurchase
      x-api-path-slug: purchase-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Purchase
  /salesreceipt/181:
    get:
      summary: Get SaleS Receipt
      description: |-
        Create an salesreceipt object
        Method : POST
      operationId: getSalesreceipt181
      x-api-path-slug: salesreceipt181-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - SaleS
      - Receipt
  /deposit:
    post:
      summary: Post Deposit
      description: |-
        Update a deposit object
        Method : POST
      operationId: postDeposit
      x-api-path-slug: deposit-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Deposit
  /transfer:
    post:
      summary: Post Transfer
      description: |-
        Create a transfer object
        Method : POST
      operationId: postTransfer
      x-api-path-slug: transfer-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Transfer
  /bill:
    post:
      summary: Post Bill
      description: |-
        Create a bill
        Content-Type:application/json
        Method - POST
      operationId: postBill
      x-api-path-slug: bill-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Bill
  /account/1:
    get:
      summary: Get Account
      description: Get the Account which has accountId as 1
      operationId: getAccount1
      x-api-path-slug: account1-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Account
  /invoice/147:
    get:
      summary: Get Invoice
      description: |-
        Read an invoice object by Id
        Method : POST
      operationId: getInvoice147
      x-api-path-slug: invoice147-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Invoice
  /reports/CustomerBalanceDetail:
    get:
      summary: Get Reports Customer Balance Detail
      description: |-
        Report - CustomerBalance Detail
        Method : GET

        The information below provides a reference on how to access the Customer Balance Detail report from the QuickBooks Online Report Service.
      operationId: getReportsCustomerbalancedetail
      x-api-path-slug: reportscustomerbalancedetail-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Customer
      - Balance
      - Detail
  /payment:
    post:
      summary: Post Payment
      description: |-
        Create an payment object
        Method : POST
      operationId: postPayment
      x-api-path-slug: payment-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Payment
  /reports/ProfitAndLossDetail:
    get:
      summary: Get Reports Profit and Loss DETAIL
      description: |-
        Report - Profit and Loss Detail
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/profit%20and%20loss%20detail
      operationId: getReportsProfitandlossdetail
      x-api-path-slug: reportsprofitandlossdetail-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Profit
      - Loss
      - DETAIL
  /salesreceipt:
    post:
      summary: Post Sales Receipt
      description: |-
        Create an salesreceipt object
        Method : POST
      operationId: postSalesreceipt
      x-api-path-slug: salesreceipt-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Sales
      - Receipt
  /upload:
    post:
      summary: Post Upload
      description: "Uploading and linking new attachments\n\nhttps://developer.intuit.com/docs/0100_quickbooks_online/0200_dev_guides/accounting/attachments#Uploading_and_linking_new_attachments\n\nIf
        the attachment is not in the Attachment list already, it's possible to upload
        it and link it to the object in one multipart operation.\n\nOperation:      POST
        https://quickbooks.api.intuit.com/v3/company/companyID/upload\nContent type:
        multipart/form-data\n\nRequest body\n\nThe following sample code shows the
        multipart request body for uploading a file and its supporting Attachable
        metatdata object, with the result of it being both added to the Attachment
        list and added to the object.\n\nThe Attachable object accompanying this request
        supplies metadata and object information to which the attachment is linked.
        \nEach part of the multipart request is separated by a boundary.  In the sample
        below, the string  --YOjcLaTlykb6OxfYJx4O07j1MweeMFem is used.  You can use
        any random and unique string.\nThe file to be uploaded and its Attachable
        object are paired together via the name parameter in the part header for each
        one.\nThe name parameter for the file part is of the form file_content_nn,
        where nn is a unique index number among the set of files being uploaded.\nThe
        name parameter for the Attachable object is of the form file_metadata_nn,
        where nn corresponds to the file index number used with the content .\nThe
        file or files are stored in the Attachment list with the name specified by
        the filename parameter.\nIf the data supplied with the Attachable object cannot
        be validated, an error is returned and the file is not uploaded."
      operationId: postUpload
      x-api-path-slug: upload-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Upload
  /customer:
    post:
      summary: Post Customer
      description: |-
        Create a customer
        Method : POST
      operationId: postCustomer
      x-api-path-slug: customer-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Customer
  /department:
    post:
      summary: Post Department
      description: |-
        Create a department object
        Method : POST
      operationId: postDepartment
      x-api-path-slug: department-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Department
  /reports/GeneralLedger:
    get:
      summary: Get Reports General Ledger
      description: |-
        Report - General Ledger
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/general%20ledger
      operationId: getReportsGeneralledger
      x-api-path-slug: reportsgeneralledger-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - General
      - Ledger
  /reports/VendorBalance:
    get:
      summary: Get Reports Vendor Balance
      description: "Report - Vendor Balance \nMethod : GET\n\nDocs - https://developer.intuit.com/docs/api/accounting/vendor%20balance"
      operationId: getReportsVendorbalance
      x-api-path-slug: reportsvendorbalance-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Vendor
      - Balance
  /purchaseorder/178:
    get:
      summary: Get Purchase Order
      description: |-
        Read a puchase-order object
        Method : POST
      operationId: getPurchaseorder178
      x-api-path-slug: purchaseorder178-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Purchase
      - Order
  /item:
    post:
      summary: Post Item
      description: |-
        Create an item object
        Method : POST
      operationId: postItem
      x-api-path-slug: item-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Item
  /journalentry:
    post:
      summary: Post Journal Entry
      description: |-
        Create an journalentry object
        Method : POST
      operationId: postJournalentry
      x-api-path-slug: journalentry-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Journal
      - Entry
  /taxservice/taxcode:
    post:
      summary: Post Tax Service Tax Code
      description: |-
        Use TaxService to create taxcode and corresponding taxrates
        Method : POST
      operationId: postTaxserviceTaxcode
      x-api-path-slug: taxservicetaxcode-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Tax
      - Service
      - Tax
      - Code
  /creditmemo:
    post:
      summary: Post Credit Memo
      description: |-
        Update a credit memo
        Method : POST
      operationId: postCreditmemo
      x-api-path-slug: creditmemo-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Credit
      - Memo
  /companyinfo/{companyid}:
    get:
      summary: Get Company
      description: 'Method : GET'
      operationId: getCompanyinfoCompany
      x-api-path-slug: companyinfocompanyid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: companyid
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Company
  /journalentry/8:
    get:
      summary: Get Journal Entry
      description: |-
        Read an journalentry object by Id
        Method : POST
      operationId: getJournalentry8
      x-api-path-slug: journalentry8-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Journal
      - Entry
  /paymentmethod:
    post:
      summary: Post Payment Method
      description: |-
        Update a payment method
        Method : POST
      operationId: postPaymentmethod
      x-api-path-slug: paymentmethod-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Payment
      - Method
  /transfer/184:
    get:
      summary: Get TransfeR
      description: |-
        Read a transfer object by Id
        Method : GET
      operationId: getTransfer184
      x-api-path-slug: transfer184-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - TransfeR
  /reports/ItemSales:
    get:
      summary: Get Reports Item Sales
      description: |-
        Report - Item Sales
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/sales%20by%20product
      operationId: getReportsItemsales
      x-api-path-slug: reportsitemsales-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Item
      - Sales
  /account:
    post:
      summary: Post Account
      description: Create a new Account
      operationId: postAccount
      x-api-path-slug: account-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Account
  /employee:
    post:
      summary: Post Employee
      description: |-
        Delete an employee object
        Method : POST

        Delete via deactivation (active=false)
      operationId: postEmployee
      x-api-path-slug: employee-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Employee
  /term/8:
    get:
      summary: Get Term
      description: |-
        Read a term object by Id
        Method : Get
      operationId: getTerm8
      x-api-path-slug: term8-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Term
  /estimate:
    post:
      summary: Post Estimate
      description: |-
        Update an Estimate object
        Method : POST
      operationId: postEstimate
      x-api-path-slug: estimate-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Estimate
  /timeactivity:
    post:
      summary: Post Time Activity
      description: |-
        Create a term object
        Method : POST
      operationId: postTimeactivity
      x-api-path-slug: timeactivity-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Time
      - Activity
  /vendor:
    post:
      summary: Post Vendor
      description: |-
        Update a vendor object
        Method : POST
      operationId: postVendor
      x-api-path-slug: vendor-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Vendor
  /refundreceipt:
    post:
      summary: Post Refund Receipt
      description: |-
        Update a refund-receipt object
        Method : POST
      operationId: postRefundreceipt
      x-api-path-slug: refundreceipt-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Refund
      - Receipt
  /vendorcredit:
    post:
      summary: Post Vendor Credit
      description: "Delete a vendorcredit object by Id\nMethod : POST\n\nSample response
        body \n\n{\n  \"VendorCredit\": {\n    \"domain\": \"QBO\",\n    \"status\":
        \"Deleted\",\n    \"Id\": \"185\"\n  },\n  \"time\": \"2016-09-02T03:14:13.909-07:00\"\n}"
      operationId: postVendorcredit
      x-api-path-slug: vendorcredit-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: operation
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Vendor
      - Credit
  /paymentmethod/8:
    get:
      summary: Get Payment Method
      description: |-
        Read a payment method
        Method : GET
      operationId: getPaymentmethod8
      x-api-path-slug: paymentmethod8-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Payment
      - Method
  /creditmemo/160:
    get:
      summary: Get Credit Memo
      description: |-
        Read a credit memo by Id
        Method : GET
      operationId: getCreditmemo160
      x-api-path-slug: creditmemo160-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Credit
      - Memo
  /reports/VendorExpenses:
    get:
      summary: Get Reports Vendorexpenses
      description: |-
        Report - Vendor Expense
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/expenses%20by%20vendor
      operationId: getReportsVendorexpenses
      x-api-path-slug: reportsvendorexpenses-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Vendorexpenses
  /vendor/70:
    get:
      summary: Get Vendor
      description: |-
        Read a vendor object by Id
        Method : GET
      operationId: getVendor70
      x-api-path-slug: vendor70-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Vendor
  /class:
    post:
      summary: Post Class
      description: |-
        Create a Class object
        Method - POST
      operationId: postClass
      x-api-path-slug: class-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Class
  /purchase/175:
    get:
      summary: Get Purchase
      description: |-
        Read a puchase object by Id
        Method : POST
      operationId: getPurchase175
      x-api-path-slug: purchase175-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Purchase
  /billpayment/118:
    get:
      summary: Get BillpaymenT
      description: |-
        Retrieve BillPayment by Id
        Method - GET
      operationId: getBillpayment
      x-api-path-slug: billpayment118-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - BillpaymenT
  /purchaseorder:
    post:
      summary: Post Purchase Order
      description: |-
        Create a puchase-order object
        Method : POST
      operationId: postPurchaseorder
      x-api-path-slug: purchaseorder-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Purchase
      - Order
  /reports/DepartmentSales:
    get:
      summary: Get Reports Department Sales
      description: |-
        Report - Department Sales
        Method : GET
      operationId: getReportsDepartmentsales
      x-api-path-slug: reportsdepartmentsales-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Department
      - Sales
  /taxagency/3:
    get:
      summary: Get Tax Agency
      description: |-
        Get a tax-agency object by ID
        Method : GET
      operationId: getTaxagency3
      x-api-path-slug: taxagency3-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Tax
      - Agency
  /deposit/162:
    get:
      summary: Get Deposit
      description: |-
        Read a deposit object by Id
        Method : POST
      operationId: getDeposit162
      x-api-path-slug: deposit162-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Deposit
  /reports/AgedPayables:
    get:
      summary: Get Reports Agedpayables
      description: |-
        Report - AgedPayable aging summary
        Method : GET

        The information below provides a reference on how to access the AP Aging summary report from the QuickBooks Online Report Service.
      operationId: getReportsAgedpayables
      x-api-path-slug: reportsagedpayables-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Agedpayables
  /bill/1:
    get:
      summary: Get Bill
      description: |-
        Retrieve a bill by Id
        Accept:application/json
        Method - GET
      operationId: getBill1
      x-api-path-slug: bill1-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Bill
  /attachable:
    post:
      summary: Post Attachable
      description: |-
        Create an attachable object
        Conent-Type:application/json
        Method - POST
      operationId: postAttachable
      x-api-path-slug: attachable-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Attachable
  /taxrate/1:
    get:
      summary: Get Tax Rate
      description: |-
        Read a taxRate by Id
        Method : POST
      operationId: getTaxrate1
      x-api-path-slug: taxrate1-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Tax
      - Rate
  /vendorcredit/185:
    get:
      summary: Get Vendor Credit
      description: |-
        Read a vendorcredit object by Id
        Method : GET

        Please change the VendorCredit it from 165 to a valid VendorCredit objectId which exists in your QBO account
      operationId: getVendorcredit185
      x-api-path-slug: vendorcredit185-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Vendor
      - Credit
  /class/5000000000000018727:
    get:
      summary: Get Class
      description: |-
        Read a Class object by Id
        Method - GET
      operationId: getClass
      x-api-path-slug: class5000000000000018727-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Class
  /taxcode/2:
    get:
      summary: Get Tax Code
      description: |-
        Read a taxcode by Id
        Method : POST
      operationId: getTaxcode2
      x-api-path-slug: taxcode2-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Tax
      - Code
  /customer/63:
    get:
      summary: Get Customer
      description: |-
        Read a customer entry by Id
        Method : GET
      operationId: getCustomer63
      x-api-path-slug: customer63-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Customer
  /batch:
    post:
      summary: Post Batch
      description: |-
        Multiple operations using batch query
        Content-Type:application/json
        Method - POST
      operationId: postBatch
      x-api-path-slug: batch-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Batch
  /reports/AccountList:
    get:
      summary: Get Reports Account List
      description: |-
        Report - Account list detail
        Method : GET

        The information below provides a reference on how to access the account list detail report from the QuickBooks Online Report Service.
      operationId: getReportsAccountlist
      x-api-path-slug: reportsaccountlist-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Account
      - List
  /reports/AgedReceivables:
    get:
      summary: Get Reports Agedreceivables
      description: |-
        Report - AgedReceivable aging summary
        Method : GET

        The information below provides a reference on how to access the AR Aging Summary report from the QuickBooks Online Report Service.
      operationId: getReportsAgedreceivables
      x-api-path-slug: reportsagedreceivables-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Agedreceivables
  /reports/CashFlow:
    get:
      summary: Get Reports Cashflow
      description: |-
        Report - CashFlow
        Method : GET

        The information below provides a reference on how to access the cash flow report from the QuickBooks Online Report Service.
      operationId: getReportsCashflow
      x-api-path-slug: reportscashflow-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Cashflow
  /reports/BalanceSheet:
    get:
      summary: Get Reports Balancesheet
      description: |-
        Report - BalanceSheet
        Method : GET

        The information below provides a reference on how to query the Balance Sheet report from the QuickBooks Online Report Service.
      operationId: getReportsBalancesheet
      x-api-path-slug: reportsbalancesheet-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Balancesheet
  /reports/CustomerIncome:
    get:
      summary: Get Reports Customer Income
      description: |-
        Report - Customer Income
        Method : GET
      operationId: getReportsCustomerincome
      x-api-path-slug: reportscustomerincome-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Customer
      - Income
  /reports/AgedReceivableDetail:
    get:
      summary: Get Reports Agedreceivabledetail
      description: |-
        Report - AgedReceivableDetail aging detail
        Method : GET

        The information below provides a reference on how to access the AR Aging Detail report from the QuickBooks Online Report Service.
      operationId: getReportsAgedreceivabledetail
      x-api-path-slug: reportsagedreceivabledetail-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Agedreceivabledetail
  /refundreceipt/66:
    get:
      summary: Get Refund Receipt
      description: |-
        Read a refund-receipt object
        Method : GET
      operationId: getRefundreceipt66
      x-api-path-slug: refundreceipt66-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Refund
      - Receipt
  /reports/CustomerBalance:
    get:
      summary: Get Reports Customer Balance
      description: |-
        Report - CustomerBalance
        Method : GET
      operationId: getReportsCustomerbalance
      x-api-path-slug: reportscustomerbalance-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Customer
      - Balance
  /billpayment:
    post:
      summary: Post BilL Payment
      description: |-
        Update a BillPayment
        Content-Type:application/json
        Method - POST
      operationId: postBillpayment
      x-api-path-slug: billpayment-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - BilL
      - Payment
  /exchangerate:
    get:
      summary: Get Exchangerate
      description: |-
        Get ExchangeRate
        Method : GET
      operationId: getExchangerate
      x-api-path-slug: exchangerate-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: asofdate
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: query
        name: sourcecurrencycode
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Exchangerate
  /reports/TransactionList:
    get:
      summary: Get Reports Transaction LIST
      description: "Report - Trial List \nMethod : GET\n\nDocs - https://developer.intuit.com/docs/api/accounting/transaction%20list"
      operationId: getReportsTransactionlist
      x-api-path-slug: reportstransactionlist-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Transaction
      - LIST
  /department/1:
    get:
      summary: Get Department
      description: |-
        Read a department object
        Method : GET
      operationId: getDepartment1
      x-api-path-slug: department1-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Department
  /employee/68:
    get:
      summary: Get Employee
      description: |-
        Retrive an employee object by ID
        Method : GET
      operationId: getEmployee68
      x-api-path-slug: employee68-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Employee
  /reports/TrialBalance:
    get:
      summary: Get Reports Trial Balance
      description: "Report - Trial Balance \nMethod : GET\n\nDocs - https://developer.intuit.com/docs/api/accounting/trial%20balance"
      operationId: getReportsTrialbalance
      x-api-path-slug: reportstrialbalance-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Trial
      - Balance
  /item/<ID>:
    get:
      summary: Get Item
      description: |-
        Read an Item by Id
        Method : GET
      operationId: getItem<>
      x-api-path-slug: itemid-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Item
  /reports/CustomerSales:
    get:
      summary: Get Reports Customer Sales
      description: |-
        Report - Customer Sales
        Method : GET
      operationId: getReportsCustomersales
      x-api-path-slug: reportscustomersales-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Customer
      - Sales
  /reports/AgedPayableDetail:
    get:
      summary: Get Reports Agedpayabledetail
      description: |-
        Report - AgedPayable aging detail
        Method : GET

        The information below provides a reference on how to access the AP Aging summary report from the QuickBooks Online Report Service.
      operationId: getReportsAgedpayabledetail
      x-api-path-slug: reportsagedpayabledetail-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Agedpayabledetail
  /attachable/5000000000000029383:
    get:
      summary: Get Attachable
      description: |-
        Retrieve an attachable object by Id
        Accept:application/json
        Method - GET
      operationId: getAttachable
      x-api-path-slug: attachable5000000000000029383-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Attachable
  /reports/ClassSales:
    get:
      summary: Get Reports Classsales
      description: |-
        Report - CashSales
        Method : GET
      operationId: getReportsClasssales
      x-api-path-slug: reportsclasssales-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Classsales
  /payment/174:
    get:
      summary: Get Payment
      description: |-
        Read a payment object by Id
        Method : GET
      operationId: getPayment174
      x-api-path-slug: payment174-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Payment
  /reports/VendorBalanceDetail:
    get:
      summary: Get Reports Vendorbalancedetail
      description: |-
        Report - Vendor Balance Detail
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/vendor%20balance%20detail
      operationId: getReportsVendorbalancedetail
      x-api-path-slug: reportsvendorbalancedetail-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Vendorbalancedetail
  /taxagency:
    post:
      summary: Post Taxagency
      description: |-
        Create a tax-agency object
        Method : POST

        Sample response payload

        {
          "SalesReceipt": {
            "domain": "QBO",
            "status": "Deleted",
            "Id": "181"
          },
          "time": "2016-09-02T02:17:24.353-07:00"
        }
      operationId: postTaxagency
      x-api-path-slug: taxagency-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Taxagency
  /reports/ProfitAndLoss:
    get:
      summary: Get Reports Profit and Loss
      description: |-
        Report - Profit and Loss
        Method : GET

        Docs - https://developer.intuit.com/docs/api/accounting/profit%20and%20loss
      operationId: getReportsProfitandloss
      x-api-path-slug: reportsprofitandloss-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Profit
      - Loss