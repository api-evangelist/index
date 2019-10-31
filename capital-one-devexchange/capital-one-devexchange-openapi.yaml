swagger: "2.0"
x-collection-name: Capital One DevExchange
x-complete: 1
info:
  title: Capital One DevExchange
  description: nessie-is-capital-ones-hackathon-api-that-gives-you-access-to-a-multitude-of-real-publicfacing-data--such-as-atm-and-bank-branch-locations--along-with-mock-customer-account-data--use-http-requests-to-set-up-peertopeer-transactions-simulate-a-weekly-paycheck-or-even-schedule-bills-for-customers-this-is-all-structured-in-a-way-that-resembles-how-we-actually-run-things-here-at-capital-one-
  version: 1.0.0
host: api.reimaginebanking.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts:
    get:
      summary: Get all accounts
      description: Returns the accounts that have been assigned to you.
      operationId: returns-the-accounts-that-have-been-assigned-to-you
      x-api-path-slug: accounts-get
      parameters:
      - in: query
        name: type
        description: Empty Param will return all types of accounts
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
  /accounts/{id}:
    get:
      summary: Get account by id
      description: Returns the account with the specific id
      operationId: returns-the-account-with-the-specific-id
      x-api-path-slug: accountsid-get
      parameters:
      - in: path
        name: id
        description: ID of account that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
    put:
      summary: Update a specific existing account
      description: Updates the specific account
      operationId: updates-the-specific-account
      x-api-path-slug: accountsid-put
      parameters:
      - in: body
        name: body
        description: Updated account object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of account that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
    delete:
      summary: Delete a specific existing account
      description: Deletes the specific account
      operationId: deletes-the-specific-account
      x-api-path-slug: accountsid-delete
      parameters:
      - in: path
        name: id
        description: ID of account that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
  /customers/{id}/accounts:
    post:
      summary: Create an account
      description: Creates an account for the customer with the id provided
      operationId: creates-an-account-for-the-customer-with-the-id-provided
      x-api-path-slug: customersidaccounts-post
      parameters:
      - in: body
        name: body
        description: Account to be created
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of customer that account will belong to
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Customers
      - ""
      - Accounts
    get:
      summary: Get accounts by customer id
      description: Returns the accounts associated with the specific customer
      operationId: returns-the-accounts-associated-with-the-specific-customer
      x-api-path-slug: customersidaccounts-get
      parameters:
      - in: path
        name: id
        description: ID of customer to fetch accounts for
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Customers
      - ""
      - Accounts
  /accounts/{id}/customer:
    get:
      summary: Get customer that owns the specified account
      description: Returns the customer that the account belongs to.
      operationId: returns-the-customer-that-the-account-belongs-to
      x-api-path-slug: accountsidcustomer-get
      parameters:
      - in: path
        name: id
        description: ID of customer that account will belong to
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Customer
  /atms:
    get:
      summary: Get all ATMs
      description: Returns all of the Capital One ATMs in the speified search area.
      operationId: returns-all-of-the-capital-one-atms-in-the-speified-search-area
      x-api-path-slug: atms-get
      parameters:
      - in: query
        name: lat
        description: Latitude of where youre looking for an ATM
      - in: query
        name: lng
        description: Longitude of where youre looking for an ATM
      - in: query
        name: rad
        description: Search radius in miles
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Atms
  /atms/{id}:
    get:
      summary: Get ATM by id
      description: Returns the ATM with the specific id
      operationId: returns-the-atm-with-the-specific-id
      x-api-path-slug: atmsid-get
      parameters:
      - in: path
        name: id
        description: ID of ATM that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Atms
  /accounts/{id}/bills:
    get:
      summary: Get all bills for a specific account
      description: Returns the bills that are tied to the specific account.
      operationId: returns-the-bills-that-are-tied-to-the-specific-account
      x-api-path-slug: accountsidbills-get
      parameters:
      - in: path
        name: id
        description: ID of account to fetch bills for
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Bills
    post:
      summary: Create a bill
      description: Creates a bill for the specific account
      operationId: creates-a-bill-for-the-specific-account
      x-api-path-slug: accountsidbills-post
      parameters:
      - in: body
        name: body
        description: Bill to be created
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of account that the bill will belong to
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Bills
  /bills/{billId}:
    get:
      summary: Get bill by id
      description: Returns the bill with the specific id
      operationId: returns-the-bill-with-the-specific-id
      x-api-path-slug: billsbillid-get
      parameters:
      - in: path
        name: billId
        description: ID of the bill to fetch
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Bills
      - Bill
    put:
      summary: Update a specific existing bill
      description: Updates the specific bill
      operationId: updates-the-specific-bill
      x-api-path-slug: billsbillid-put
      parameters:
      - in: path
        name: billId
        description: ID of the bill to update
      - in: body
        name: body
        description: Bill to be updated
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Bills
      - Bill
    delete:
      summary: Delete a specific existing bill
      description: Deletes the specific bill
      operationId: deletes-the-specific-bill
      x-api-path-slug: billsbillid-delete
      parameters:
      - in: path
        name: billId
        description: ID of the bill to delete
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Bills
      - Bill
  /branches:
    get:
      summary: Get all branches
      description: Returns all of the Capital One branches.
      operationId: returns-all-of-the-capital-one-branches
      x-api-path-slug: branches-get
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Branches
  /branches/{id}:
    get:
      summary: Get branch by id
      description: Returns the branch with the specific id
      operationId: returns-the-branch-with-the-specific-id
      x-api-path-slug: branchesid-get
      parameters:
      - in: path
        name: id
        description: ID of branch that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Branches
  /customers:
    get:
      summary: Get all customers
      description: Returns the customers that have been assigned to you.
      operationId: returns-the-customers-that-have-been-assigned-to-you
      x-api-path-slug: customers-get
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Customers
    post:
      summary: Create a customer
      description: Creates a customer
      operationId: creates-a-customer
      x-api-path-slug: customers-post
      parameters:
      - in: body
        name: body
        description: Customer to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Customers
  /customers/{id}:
    get:
      summary: Get customer by id
      description: Returns the customer with the specific id
      operationId: returns-the-customer-with-the-specific-id
      x-api-path-slug: customersid-get
      parameters:
      - in: path
        name: id
        description: ID of customer that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Customers
    put:
      summary: Update a specific existing customer
      description: Updates the specific customer
      operationId: updates-the-specific-customer
      x-api-path-slug: customersid-put
      parameters:
      - in: body
        name: body
        description: Updated customer object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of customer that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Customers
  /customers/{id}/bills:
    get:
      summary: Get bills by customer id
      description: Returns the bills associated with the specific customer
      operationId: returns-the-bills-associated-with-the-specific-customer
      x-api-path-slug: customersidbills-get
      parameters:
      - in: path
        name: id
        description: ID of customer to fetch bills for
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Customers
      - ""
      - Bills
  /data:
    delete:
      summary: Delete data associated with your API key.
      description: This endpoint deletes any data associated with your API key and
        of the type passed in as query parameters.  If you do not specify any type
        to delete, no data will be deleted.
      operationId: this-endpoint-deletes-any-data-associated-with-your-api-key-and-of-the-type-passed-in-as-query-param
      x-api-path-slug: data-delete
      parameters:
      - in: query
        name: type
        description: Collection to delete data from
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Data
  /accounts/{id}/deposits:
    get:
      summary: Get all deposits
      description: Returns the deposits that you are involved in.
      operationId: returns-the-deposits-that-you-are-involved-in
      x-api-path-slug: accountsiddeposits-get
      parameters:
      - in: path
        name: id
        description: ID of account associated with the deposit
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Deposits
    post:
      summary: Create a deposit
      description: Creates a deposit where the account with the ID specified receives
        the amount.
      operationId: creates-a-deposit-where-the-account-with-the-id-specified-receives-the-amount
      x-api-path-slug: accountsiddeposits-post
      parameters:
      - in: body
        name: body
        description: Deposit to be created
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of account receiver of deposit
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Deposits
  /deposits/{id}:
    get:
      summary: Get deposit by id
      description: Returns the deposit with the specific id
      operationId: returns-the-deposit-with-the-specific-id
      x-api-path-slug: depositsid-get
      parameters:
      - in: path
        name: id
        description: ID of the deposit that is being fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Deposits
    put:
      summary: Update a specific existing deposit
      description: Updates the specific deposit
      operationId: updates-the-specific-deposit
      x-api-path-slug: depositsid-put
      parameters:
      - in: body
        name: body
        description: deposit to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of the deposit that is being updated
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Deposits
    delete:
      summary: Delete a specific existing deposit
      description: Deletes the specific deposit
      operationId: deletes-the-specific-deposit
      x-api-path-slug: depositsid-delete
      parameters:
      - in: path
        name: id
        description: ID of the deposit that is being deleted
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Deposits
  /accounts/{id}/loans:
    get:
      summary: Get all loans
      description: Returns the loans that you are involved in.
      operationId: returns-the-loans-that-you-are-involved-in
      x-api-path-slug: accountsidloans-get
      parameters:
      - in: path
        name: id
        description: ID of account associated with the loan
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Loans
    post:
      summary: Create a loan
      description: Creates a loan where the account with the ID specified is debitted.
      operationId: creates-a-loan-where-the-account-with-the-id-specified-is-debitted
      x-api-path-slug: accountsidloans-post
      parameters:
      - in: body
        name: body
        description: loan to be created
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of account receiver of loan
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Loans
  /loans/{id}:
    get:
      summary: Get loan by id
      description: Returns the loan with the specific id
      operationId: returns-the-loan-with-the-specific-id
      x-api-path-slug: loansid-get
      parameters:
      - in: path
        name: id
        description: ID of the loan that is being fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Loans
    put:
      summary: Update a specific existing loan
      description: Updates the specific loan
      operationId: updates-the-specific-loan
      x-api-path-slug: loansid-put
      parameters:
      - in: body
        name: body
        description: loan to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of the loan that is being updated
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Loans
    delete:
      summary: Delete a specific existing loan
      description: Deletes the specific loan
      operationId: deletes-the-specific-loan
      x-api-path-slug: loansid-delete
      parameters:
      - in: path
        name: id
        description: ID of the loan that is being deleted
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Loans
  /merchants:
    get:
      summary: Get all merchants
      description: Returns the merchants that have been assigned to you.
      operationId: returns-the-merchants-that-have-been-assigned-to-you
      x-api-path-slug: merchants-get
      parameters:
      - in: query
        name: lat
        description: Latitude of where youre looking for a merchant
      - in: query
        name: lng
        description: Longitude of where youre looking for a merchant
      - in: query
        name: rad
        description: Search radius in miles
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Merchants
    post:
      summary: Create a merchant
      description: Creates a merchant
      operationId: creates-a-merchant
      x-api-path-slug: merchants-post
      parameters:
      - in: body
        name: body
        description: Merchant to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Merchants
  /merchants/{id}:
    get:
      summary: Get merchant by id
      description: Returns the merchant with the specific id
      operationId: returns-the-merchant-with-the-specific-id
      x-api-path-slug: merchantsid-get
      parameters:
      - in: path
        name: id
        description: ID of merchant that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Merchants
    put:
      summary: Update a specific existing merchant
      description: Updates the specific merchant
      operationId: updates-the-specific-merchant
      x-api-path-slug: merchantsid-put
      parameters:
      - in: body
        name: body
        description: Updated merchant object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of merchant that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Merchants
  /accounts/{id}/purchases:
    get:
      summary: Get all purchases
      description: Returns the purchases that you are involved in.
      operationId: returns-the-purchases-that-you-are-involved-in
      x-api-path-slug: accountsidpurchases-get
      parameters:
      - in: path
        name: id
        description: ID of account associated with the purchase
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Purchases
    post:
      summary: Create a purchase
      description: Creates a purchase where the account with the ID specified is the
        payer.
      operationId: creates-a-purchase-where-the-account-with-the-id-specified-is-the-payer
      x-api-path-slug: accountsidpurchases-post
      parameters:
      - in: body
        name: body
        description: Purchase to be created
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of account payer in purchase
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Purchases
  /purchases/{id}:
    get:
      summary: Get purchase by id
      description: Returns the purchase with the specific id
      operationId: returns-the-purchase-with-the-specific-id
      x-api-path-slug: purchasesid-get
      parameters:
      - in: path
        name: id
        description: ID of the purchase that is being fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Purchases
    delete:
      summary: Delete a specific existing purchase
      description: Deletes the specific purchase
      operationId: deletes-the-specific-purchase
      x-api-path-slug: purchasesid-delete
      parameters:
      - in: path
        name: id
        description: ID of the purchase that is being deleted
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Purchases
    put:
      summary: Update a specific existing purchase
      description: Updates the specific purchase
      operationId: updates-the-specific-purchase
      x-api-path-slug: purchasesid-put
      parameters:
      - in: body
        name: body
        description: Purchase to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of the purchase that is being updated
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Purchases
  /merchants/{id}/purchases:
    get:
      summary: Get all purchases by merchant
      description: Returns the purchases that a merchant is involved in.
      operationId: returns-the-purchases-that-a-merchant-is-involved-in
      x-api-path-slug: merchantsidpurchases-get
      parameters:
      - in: path
        name: id
        description: ID of the merchant associated with all the purchases
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Merchants
      - ""
      - Purchases
  /merchants/{id}/accounts/{accountId}/purchases:
    get:
      summary: Get all purchases by account and merchant
      description: Returns the purchases that a merchant is involved in.
      operationId: returns-the-purchases-that-a-merchant-is-involved-in
      x-api-path-slug: merchantsidaccountsaccountidpurchases-get
      parameters:
      - in: path
        name: accountId
        description: ID of the account associated with all the purchases
      - in: path
        name: id
        description: ID of the merchant associated with all the purchases
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Merchants
      - ""
      - Accounts
      - Account
      - Purchases
  /accounts/{id}/transfers:
    get:
      summary: Get all transfers
      description: Returns the transfers that you are involved in.
      operationId: returns-the-transfers-that-you-are-involved-in
      x-api-path-slug: accountsidtransfers-get
      parameters:
      - in: path
        name: id
        description: ID of account associated with the transfer
      - in: query
        name: type
        description: When param is empty, will return transfers associated with account
          where account is payer AND payee
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Transfers
    post:
      summary: Create a transfer
      description: Creates a transfer where the account with the ID specified is the
        payer.
      operationId: creates-a-transfer-where-the-account-with-the-id-specified-is-the-payer
      x-api-path-slug: accountsidtransfers-post
      parameters:
      - in: body
        name: body
        description: Transfer to be created
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of account payer in transfer
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Transfers
  /transfers/{transferId}:
    get:
      summary: Get transfer by id
      description: Returns the transfer with the specific id
      operationId: returns-the-transfer-with-the-specific-id
      x-api-path-slug: transferstransferid-get
      parameters:
      - in: path
        name: transferId
        description: ID of the transfer that is being fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Transfers
      - Transfer
    put:
      summary: Update a specific existing transfer
      description: Updates the specific transfer
      operationId: updates-the-specific-transfer
      x-api-path-slug: transferstransferid-put
      parameters:
      - in: body
        name: body
        description: Transfer to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: transferId
        description: ID of the transfer that is being updated
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Transfers
      - Transfer
    delete:
      summary: Delete a specific existing transfer
      description: Deletes the specific transfer
      operationId: deletes-the-specific-transfer
      x-api-path-slug: transferstransferid-delete
      parameters:
      - in: path
        name: transferId
        description: ID of the transfer that is being deleted
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Transfers
      - Transfer
  /accounts/{id}/withdrawals:
    get:
      summary: Get all withdrawals
      description: Returns the withdrawals that you are involved in.
      operationId: returns-the-withdrawals-that-you-are-involved-in
      x-api-path-slug: accountsidwithdrawals-get
      parameters:
      - in: path
        name: id
        description: ID of account associated with the withdrawal
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Withdrawals
    post:
      summary: Create a withdrawal
      description: Creates a withdrawal where the account with the ID specified is
        debitted.
      operationId: creates-a-withdrawal-where-the-account-with-the-id-specified-is-debitted
      x-api-path-slug: accountsidwithdrawals-post
      parameters:
      - in: body
        name: body
        description: Withdrawal to be created
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of account receiver of withdrawal
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Withdrawals
  /withdrawals/{id}:
    get:
      summary: Get withdrawal by id
      description: Returns the withdrawal with the specific id
      operationId: returns-the-withdrawal-with-the-specific-id
      x-api-path-slug: withdrawalsid-get
      parameters:
      - in: path
        name: id
        description: ID of the withdrawal that is being fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Withdrawals
    put:
      summary: Update a specific existing withdrawal
      description: Updates the specific withdrawal
      operationId: updates-the-specific-withdrawal
      x-api-path-slug: withdrawalsid-put
      parameters:
      - in: body
        name: body
        description: withdrawal to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of the withdrawal that is being updated
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Withdrawals
    delete:
      summary: Delete a specific existing withdrawal
      description: Deletes the specific withdrawal
      operationId: deletes-the-specific-withdrawal
      x-api-path-slug: withdrawalsid-delete
      parameters:
      - in: path
        name: id
        description: ID of the withdrawal that is being deleted
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Withdrawals