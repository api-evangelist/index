swagger: "2.0"
x-collection-name: CoinFabrik
x-complete: 1
info:
  title: Coinbase API
  description: the-coinbase-v2-api
  contact:
    name: CoinFabrik
    url: http://www.coinfabrik.com/
  version: 1.0.0
host: api.coinbase.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}:
    get:
      summary: Show a user
      description: "Get any user\u2019s public information with their ID."
      operationId: get-any-users-public-information-with-their-id
      x-api-path-slug: usersuser-id-get
      parameters:
      - in: path
        name: user_id
        description: The user id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Show
      - User
  /user:
    get:
      summary: Show current user
      description: "Get current user\u2019s public information. To get user\u2019s
        email or private information, use permissions wallet:user:email and wallet:user:read."
      operationId: get-current-users-public-information-to-get-users-email-or-private-information-use-permissions-walle
      x-api-path-slug: user-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Show
      - Current
      - User
    put:
      summary: Update current user
      description: Modify current user and their preferences.
      operationId: modify-current-user-and-their-preferences
      x-api-path-slug: user-put
      parameters:
      - in: body
        name: body
        description: Properties to update
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Current
      - User
  /user/auth:
    get:
      summary: Show authorization information
      description: "Get current user\u2019s authorization information including granted
        scopes and send limits when using OAuth2 authentication."
      operationId: get-current-users-authorization-information-including-granted-scopes-and-send-limits-when-using-oaut
      x-api-path-slug: userauth-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Show
      - Authorization
      - Information
  /accounts:
    get:
      summary: List accounts
      description: "Lists current user\u2019s accounts to which the authentication
        method has access to."
      operationId: lists-current-users-accounts-to-which-the-authentication-method-has-access-to
      x-api-path-slug: accounts-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - List
      - Accounts
    post:
      summary: Create account
      description: Creates a new account for user.
      operationId: creates-a-new-account-for-user
      x-api-path-slug: accounts-post
      parameters:
      - in: body
        name: account_properties
        description: Account properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Account
  /accounts/{account_id}:
    get:
      summary: Show an account
      description: "Show current user\u2019s account. To access user\u2019s primary
        account, primary keyword can be used instead of the account id in the URL."
      operationId: show-current-users-account-to-access-users-primary-account-primary-keyword-can-be-used-instead-of-th
      x-api-path-slug: accountsaccount-id-get
      parameters:
      - in: path
        name: account_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Show
      - Account
    put:
      summary: Update account
      description: "Modifies user\u2019s account name."
      operationId: modifies-users-account-name
      x-api-path-slug: accountsaccount-id-put
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: body
        name: account_properties
        description: Properties to update
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Account
    delete:
      summary: Delete account
      description: "Removes user\u2019s account. In order to remove an account it
        can\u2019t be\n\n- Primary account\n- Account with non-zero balance\n- Fiat
        account\n- Vault with a pending withdrawal"
      operationId: removes-users-account-in-order-to-remove-an-account-it-cant-be-primary-account-account-with-nonzero-
      x-api-path-slug: accountsaccount-id-delete
      parameters:
      - in: path
        name: account_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Account
  /accounts/{account_id}/primary:
    get:
      summary: Set account as primary
      description: Promote an account as primary account.
      operationId: promote-an-account-as-primary-account
      x-api-path-slug: accountsaccount-idprimary-get
      parameters:
      - in: path
        name: account_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Set
      - Account
      - As
      - Primary
  /accounts/{account_id}/addresses:
    get:
      summary: List addresses
      description: |-
        Lists addresses for an account.

        *Important*: Addresses should be considered one time use only.
      operationId: lists-addresses-for-an-accountimportant-addresses-should-be-considered-one-time-use-only
      x-api-path-slug: accountsaccount-idaddresses-get
      parameters:
      - in: path
        name: account_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - List
      - Addresses
    post:
      summary: Create address
      description: "Creates a new address for an account. As all the arguments are
        optinal, it\u2019s possible just to do a empty POST which will create a new
        address. This is handy if you need to create new receive addresses for an
        account on-demand.\nAddresses can be created for all account types. With fiat
        accounts, funds will be received with Instant Exchange."
      operationId: creates-a-new-address-for-an-account-as-all-the-arguments-are-optinal-its-possible-just-to-do-a-empt
      x-api-path-slug: accountsaccount-idaddresses-post
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: body
        name: address_properties
        description: Properties to update
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Address
  /accounts/{account_id}/addresses/{address_id}:
    get:
      summary: Show an address
      description: "Show an individual address for an account.\nRegular bitcoin address
        can be used in place of address_id but the address has to be associated to
        the correct account.\n  \n*Important* Addresses should be considered one time
        use only."
      operationId: show-an-individual-address-for-an-accountregular-bitcoin-address-can-be-used-in-place-of-address-id-
      x-api-path-slug: accountsaccount-idaddressesaddress-id-get
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: path
        name: address_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Show
      - Address
  /accounts/{account_id}/addresses/{address_id}/transactions:
    get:
      summary: "List address\u2019s transactions"
      description: list transactions that have been sent to a specific address. Regular
        bitcoin address can be used in place of address_id but the address has to
        be associated to the correct account.
      operationId: list-transactions-that-have-been-sent-to-a-specific-address-regular-bitcoin-address-can-be-used-in-p
      x-api-path-slug: accountsaccount-idaddressesaddress-idtransactions-get
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: path
        name: address_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - List
      - "Address\u2019s"
      - Transactions
  /accounts/{account_id}/transactions:
    get:
      summary: List transactions
      description: "Lists account\u2019s transactions. See Transaction resource for
        more information."
      operationId: lists-accounts-transactions-see-transaction-resource-for-more-information
      x-api-path-slug: accountsaccount-idtransactions-get
      parameters:
      - in: path
        name: account_id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - List
      - Transactions
    post:
      summary: Send or request money
      description: |-
        Type=send
        =========

        Send funds to a bitcoin address or email address. No transaction fees are required for off blockchain transactions, and Coinbase waives fees for on-blockchain transactions greater than 0.0001 BTC, up to a threshold of 25 per day. Read more about free transactions.

        When used with OAuth2 authentication, this endpoint requires two factor authentication unless used with wallet:transactions:send:bypass-2fa scope.

        If the user is able to buy bitcoin, they can send funds from their fiat account using instant exchange feature. Buy fees will be included in the created transaction and the recipient will receive the user defined amount.

        To create a multisig transaction, visit Multisig documentation.

        Type=request
        ============

        Requests money from an email address.
      operationId: typesendsend-funds-to-a-bitcoin-address-or-email-address-no-transaction-fees-are-required-for-off-bl
      x-api-path-slug: accountsaccount-idtransactions-post
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: body
        name: transaction_options
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Send
      - Request
      - Money
  /accounts/{account_id}/transactions/{transaction_id}:
    get:
      summary: Show a transaction
      description: Show an individual transaction for an account. See Transaction
        resource for more information.
      operationId: show-an-individual-transaction-for-an-account-see-transaction-resource-for-more-information
      x-api-path-slug: accountsaccount-idtransactionstransaction-id-get
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: path
        name: transaction_id
        description: The transaction id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Show
      - Transaction
    delete:
      summary: Cancel request money
      description: Lets a user cancel a money request. Money requests can be canceled
        by the sender or the recipient.
      operationId: lets-a-user-cancel-a-money-request-money-requests-can-be-canceled-by-the-sender-or-the-recipient
      x-api-path-slug: accountsaccount-idtransactionstransaction-id-delete
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: path
        name: transaction_id
        description: The transaction id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Cancel
      - Request
      - Money
  /accounts/{account_id}/transactions/{transaction_id}/complete:
    post:
      summary: Complete request money
      description: Lets the recipient of a money request complete the request by sending
        money to the user who requested the money. This can only be completed by the
        user to whom the request was made, not the user who sent the request.
      operationId: lets-the-recipient-of-a-money-request-complete-the-request-by-sending-money-to-the-user-who-requeste
      x-api-path-slug: accountsaccount-idtransactionstransaction-idcomplete-post
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: path
        name: transaction_id
        description: The transaction id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Complete
      - Request
      - Money
  /accounts/{account_id}/transactions/{transaction_id}/resend:
    post:
      summary: Re-send request money
      description: Lets the user resend a money request. This will notify recipient
        with a new email.
      operationId: lets-the-user-resend-a-money-request-this-will-notify-recipient-with-a-new-email
      x-api-path-slug: accountsaccount-idtransactionstransaction-idresend-post
      parameters:
      - in: path
        name: account_id
        description: The account id
      - in: path
        name: transaction_id
        description: The transaction id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Re-send
      - Request
      - Money