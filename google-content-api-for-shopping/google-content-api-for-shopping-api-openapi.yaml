swagger: "2.0"
x-collection-name: Google Content API for Shopping
x-complete: 1
info:
  title: Content API for Shopping
  description: manages-product-items-inventory-and-merchant-center-accounts-for-google-shopping-
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /content/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/authinfo:
    get:
      summary: Authenticated User
      description: Returns information about the authenticated user.
      operationId: content.accounts.authinfo
      x-api-path-slug: accountsauthinfo-get
      responses:
        200:
          description: OK
      tags:
      - Authenticated
      - User
  /accounts/batch:
    post:
      summary: Account Batch
      description: Retrieves, inserts, updates, and deletes multiple Merchant Center
        (sub-)accounts in a single request.
      operationId: content.accounts.custombatch
      x-api-path-slug: accountsbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      responses:
        200:
          description: OK
      tags:
      - Account
      - Batch
  /accountshipping/batch:
    post:
      summary: Account Batches
      description: Retrieves and updates the shipping settings of multiple accounts
        in a single request.
      operationId: content.accountshipping.custombatch
      x-api-path-slug: accountshippingbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      responses:
        200:
          description: OK
      tags:
      - Account
      - Batches
  /accountstatuses/batch:
    post:
      summary: Account Status Batch
      description: Retrieves account batch status.
      operationId: content.accountstatuses.custombatch
      x-api-path-slug: accountstatusesbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Status
      - Batch
  /accounttax/batch:
    post:
      summary: Account Taxes
      description: Retrieves and updates tax settings of multiple accounts in a single
        request.
      operationId: content.accounttax.custombatch
      x-api-path-slug: accounttaxbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      responses:
        200:
          description: OK
      tags:
      - Account
      - Taxes
  /datafeeds/batch:
    post:
      summary: Data Feeds
      description: Retrieves data feed batches.
      operationId: content.datafeeds.custombatch
      x-api-path-slug: datafeedsbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feeds
  /datafeedstatuses/batch:
    post:
      summary: Data Feed Status
      description: Retrieves data feed batch status.
      operationId: content.datafeedstatuses.custombatch
      x-api-path-slug: datafeedstatusesbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
      - Status
  /inventory/batch:
    post:
      summary: Inventory
      description: Updates price and availability for multiple products or stores
        in a single request. This operation does not update the expiration date of
        the products. This method can only be called for non-multi-client accounts.
      operationId: content.inventory.custombatch
      x-api-path-slug: inventorybatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      responses:
        200:
          description: OK
      tags:
      - Inventory
  /orders/batch:
    post:
      summary: Orders
      description: Retrieves or modifies multiple orders in a single request. This
        method can only be called for non-multi-client accounts.
      operationId: content.orders.custombatch
      x-api-path-slug: ordersbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Orders
  /products/batch:
    post:
      summary: Product Batches
      description: Retrieves, inserts, and deletes multiple products in a single request.
        This method can only be called for non-multi-client accounts.
      operationId: content.products.custombatch
      x-api-path-slug: productsbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      responses:
        200:
          description: OK
      tags:
      - Product
      - Batches
  /productstatuses/batch:
    post:
      summary: Product Batch
      description: Gets the statuses of multiple products in a single request. This
        method can only be called for non-multi-client accounts.
      operationId: content.productstatuses.custombatch
      x-api-path-slug: productstatusesbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Product
      - Batch
  /shippingsettings/batch:
    post:
      summary: Shipping Settings
      description: Retrieves and updates the shipping settings of multiple accounts
        in a single request.
      operationId: content.shippingsettings.custombatch
      x-api-path-slug: shippingsettingsbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Settings
  /{merchantId}/accounts:
    get:
      summary: Get Accounts
      description: Lists the sub-accounts in your Merchant Center account. This method
        can only be called for multi-client accounts.
      operationId: content.accounts.list
      x-api-path-slug: merchantidaccounts-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of accounts to return in the response, used
          for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Accounts
    post:
      summary: Create Accounts
      description: Creates a Merchant Center sub-account. This method can only be
        called for multi-client accounts.
      operationId: content.accounts.insert
      x-api-path-slug: merchantidaccounts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /{merchantId}/accounts/{accountId}:
    delete:
      summary: Delete Account
      description: Deletes a Merchant Center sub-account. This method can only be
        called for multi-client accounts.
      operationId: content.accounts.delete
      x-api-path-slug: merchantidaccountsaccountid-delete
      parameters:
      - in: path
        name: accountId
        description: The ID of the account
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
    get:
      summary: Get Account
      description: 'Retrieves a Merchant Center account. This method can only be called
        for accounts to which the managing account has access: either the managing
        account itself or sub-accounts if the managing account is a multi-client account.'
      operationId: content.accounts.get
      x-api-path-slug: merchantidaccountsaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The ID of the account
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
    patch:
      summary: Update Account
      description: 'Updates a Merchant Center account. This method can only be called
        for accounts to which the managing account has access: either the managing
        account itself or sub-accounts if the managing account is a multi-client account.
        This method supports patch semantics.'
      operationId: content.accounts.patch
      x-api-path-slug: merchantidaccountsaccountid-patch
      parameters:
      - in: path
        name: accountId
        description: The ID of the account
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
    put:
      summary: Update Account
      description: 'Updates a Merchant Center account. This method can only be called
        for accounts to which the managing account has access: either the managing
        account itself or sub-accounts if the managing account is a multi-client account.'
      operationId: content.accounts.update
      x-api-path-slug: merchantidaccountsaccountid-put
      parameters:
      - in: path
        name: accountId
        description: The ID of the account
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
  /{merchantId}/accountshipping:
    get:
      summary: Get Account Shipping
      description: Lists the shipping settings of the sub-accounts in your Merchant
        Center account. This method can only be called for multi-client accounts.
      operationId: content.accountshipping.list
      x-api-path-slug: merchantidaccountshipping-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of shipping settings to return in the response,
          used for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Account
      - Shipping
  /{merchantId}/accountshipping/{accountId}:
    get:
      summary: Get Account Shipping
      description: 'Retrieves the shipping settings of the account. This method can
        only be called for accounts to which the managing account has access: either
        the managing account itself or sub-accounts if the managing account is a multi-client
        account.'
      operationId: content.accountshipping.get
      x-api-path-slug: merchantidaccountshippingaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update account shipping
          settings
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
      - Shipping
    patch:
      summary: Updat Account Shipping
      description: 'Updates the shipping settings of the account. This method can
        only be called for accounts to which the managing account has access: either
        the managing account itself or sub-accounts if the managing account is a multi-client
        account. This method supports patch semantics.'
      operationId: content.accountshipping.patch
      x-api-path-slug: merchantidaccountshippingaccountid-patch
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update account shipping
          settings
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Updat
      - Account
      - Shipping
    put:
      summary: Updat Account Shipping
      description: 'Updates the shipping settings of the account. This method can
        only be called for accounts to which the managing account has access: either
        the managing account itself or sub-accounts if the managing account is a multi-client
        account.'
      operationId: content.accountshipping.update
      x-api-path-slug: merchantidaccountshippingaccountid-put
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update account shipping
          settings
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Updat
      - Account
      - Shipping
  /{merchantId}/accountstatuses:
    get:
      summary: Get Account Status
      description: Lists the statuses of the sub-accounts in your Merchant Center
        account. This method can only be called for multi-client accounts.
      operationId: content.accountstatuses.list
      x-api-path-slug: merchantidaccountstatuses-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of account statuses to return in the response,
          used for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Account
      - Status
  /{merchantId}/accountstatuses/{accountId}:
    get:
      summary: Get Account Status
      description: 'Retrieves the status of a Merchant Center account. This method
        can only be called for accounts to which the managing account has access:
        either the managing account itself or sub-accounts if the managing account
        is a multi-client account.'
      operationId: content.accountstatuses.get
      x-api-path-slug: merchantidaccountstatusesaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The ID of the account
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
      - Status
  /{merchantId}/accounttax:
    get:
      summary: Get Account Taxes
      description: Lists the tax settings of the sub-accounts in your Merchant Center
        account. This method can only be called for multi-client accounts.
      operationId: content.accounttax.list
      x-api-path-slug: merchantidaccounttax-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of tax settings to return in the response,
          used for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Account
      - Taxes
  /{merchantId}/accounttax/{accountId}:
    get:
      summary: Get Account Tax
      description: 'Retrieves the tax settings of the account. This method can only
        be called for accounts to which the managing account has access: either the
        managing account itself or sub-accounts if the managing account is a multi-client
        account.'
      operationId: content.accounttax.get
      x-api-path-slug: merchantidaccounttaxaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update account tax settings
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
      - Tax
    patch:
      summary: Update Account Tax
      description: 'Updates the tax settings of the account. This method can only
        be called for accounts to which the managing account has access: either the
        managing account itself or sub-accounts if the managing account is a multi-client
        account. This method supports patch semantics.'
      operationId: content.accounttax.patch
      x-api-path-slug: merchantidaccounttaxaccountid-patch
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update account tax settings
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
      - Tax
    put:
      summary: Update Account Tax
      description: 'Updates the tax settings of the account. This method can only
        be called for accounts to which the managing account has access: either the
        managing account itself or sub-accounts if the managing account is a multi-client
        account.'
      operationId: content.accounttax.update
      x-api-path-slug: merchantidaccounttaxaccountid-put
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update account tax settings
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Account
      - Tax
  /{merchantId}/datafeeds:
    get:
      summary: Get Data Feeds
      description: Lists the datafeeds in your Merchant Center account. This method
        can only be called for non-multi-client accounts.
      operationId: content.datafeeds.list
      x-api-path-slug: merchantiddatafeeds-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of products to return in the response, used
          for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feeds
    post:
      summary: Create Data Feed
      description: Registers a datafeed with your Merchant Center account. This method
        can only be called for non-multi-client accounts.
      operationId: content.datafeeds.insert
      x-api-path-slug: merchantiddatafeeds-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
  /{merchantId}/datafeeds/{datafeedId}:
    delete:
      summary: Delete Data Feed
      description: Deletes a datafeed from your Merchant Center account. This method
        can only be called for non-multi-client accounts.
      operationId: content.datafeeds.delete
      x-api-path-slug: merchantiddatafeedsdatafeedid-delete
      parameters:
      - in: path
        name: datafeedId
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
    get:
      summary: Get Data Feed
      description: Retrieves a datafeed from your Merchant Center account. This method
        can only be called for non-multi-client accounts.
      operationId: content.datafeeds.get
      x-api-path-slug: merchantiddatafeedsdatafeedid-get
      parameters:
      - in: path
        name: datafeedId
      - in: path
        name: merchantId
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
    patch:
      summary: Update Data Feed
      description: Updates a datafeed of your Merchant Center account. This method
        can only be called for non-multi-client accounts. This method supports patch
        semantics.
      operationId: content.datafeeds.patch
      x-api-path-slug: merchantiddatafeedsdatafeedid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: datafeedId
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
    put:
      summary: Update Data Feed
      description: Updates a datafeed of your Merchant Center account. This method
        can only be called for non-multi-client accounts.
      operationId: content.datafeeds.update
      x-api-path-slug: merchantiddatafeedsdatafeedid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: datafeedId
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
  /{merchantId}/datafeedstatuses:
    get:
      summary: Get Data Feed Status
      description: Lists the statuses of the datafeeds in your Merchant Center account.
        This method can only be called for non-multi-client accounts.
      operationId: content.datafeedstatuses.list
      x-api-path-slug: merchantiddatafeedstatuses-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of products to return in the response, used
          for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
      - Status
  /{merchantId}/datafeedstatuses/{datafeedId}:
    get:
      summary: Get Data Feed Status
      description: Retrieves the status of a datafeed from your Merchant Center account.
        This method can only be called for non-multi-client accounts.
      operationId: content.datafeedstatuses.get
      x-api-path-slug: merchantiddatafeedstatusesdatafeedid-get
      parameters:
      - in: path
        name: datafeedId
      - in: path
        name: merchantId
      responses:
        200:
          description: OK
      tags:
      - Data
      - Feed
      - Status
  /{merchantId}/inventory/{storeCode}/products/{productId}:
    post:
      summary: Update Price
      description: Updates price and availability of a product in your Merchant Center
        account. This operation does not update the expiration date of the product.
        This method can only be called for non-multi-client accounts.
      operationId: content.inventory.set
      x-api-path-slug: merchantidinventorystorecodeproductsproductid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: productId
        description: The ID of the product for which to update price and availability
      - in: path
        name: storeCode
        description: The code of the store for which to update price and availability
      responses:
        200:
          description: OK
      tags:
      - Price
  /{merchantId}/orders:
    get:
      summary: Get Orders
      description: Lists the orders in your Merchant Center account. This method can
        only be called for non-multi-client accounts.
      operationId: content.orders.list
      x-api-path-slug: merchantidorders-get
      parameters:
      - in: query
        name: acknowledged
        description: Obtains orders that match the acknowledgement status
      - in: query
        name: maxResults
        description: The maximum number of orders to return in the response, used
          for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: orderBy
        description: The ordering of the returned list
      - in: query
        name: pageToken
        description: The token returned by the previous request
      - in: query
        name: placedDateEnd
        description: Obtains orders placed before this date (exclusively), in ISO
          8601 format
      - in: query
        name: placedDateStart
        description: Obtains orders placed after this date (inclusively), in ISO 8601
          format
      - in: query
        name: statuses
        description: Obtains orders that match any of the specified statuses
      responses:
        200:
          description: OK
      tags:
      - Orders
  /{merchantId}/orders/{orderId}:
    get:
      summary: Get Order
      description: Retrieves an order from your Merchant Center account. This method
        can only be called for non-multi-client accounts.
      operationId: content.orders.get
      x-api-path-slug: merchantidordersorderid-get
      parameters:
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order
      responses:
        200:
          description: OK
      tags:
      - Order
  /{merchantId}/orders/{orderId}/acknowledge:
    post:
      summary: Acknowledge Order
      description: Marks an order as acknowledged. This method can only be called
        for non-multi-client accounts.
      operationId: content.orders.acknowledge
      x-api-path-slug: merchantidordersorderidacknowledge-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order
      responses:
        200:
          description: OK
      tags:
      - Acknowledge
      - Order
  /{merchantId}/orders/{orderId}/cancel:
    post:
      summary: Cancel Order
      description: Cancels all line items in an order. This method can only be called
        for non-multi-client accounts.
      operationId: content.orders.cancel
      x-api-path-slug: merchantidordersorderidcancel-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order to cancel
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Order
  /{merchantId}/orders/{orderId}/cancelLineItem:
    post:
      summary: Cancel Order Line Item
      description: Cancels a line item. This method can only be called for non-multi-client
        accounts.
      operationId: content.orders.cancellineitem
      x-api-path-slug: merchantidordersorderidcancellineitem-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Order
      - Line
      - Item
  /{merchantId}/orders/{orderId}/refund:
    post:
      summary: Refund Order
      description: Refund a portion of the order, up to the full amount paid. This
        method can only be called for non-multi-client accounts.
      operationId: content.orders.refund
      x-api-path-slug: merchantidordersorderidrefund-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order to refund
      responses:
        200:
          description: OK
      tags:
      - Refund
      - Order
  /{merchantId}/orders/{orderId}/returnLineItem:
    post:
      summary: Return Line Item
      description: Returns a line item. This method can only be called for non-multi-client
        accounts.
      operationId: content.orders.returnlineitem
      x-api-path-slug: merchantidordersorderidreturnlineitem-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order
      responses:
        200:
          description: OK
      tags:
      - Return
      - Line
      - Item
  /{merchantId}/orders/{orderId}/shipLineItems:
    post:
      summary: Ship Line Item
      description: Marks line item(s) as shipped. This method can only be called for
        non-multi-client accounts.
      operationId: content.orders.shiplineitems
      x-api-path-slug: merchantidordersorderidshiplineitems-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order
      responses:
        200:
          description: OK
      tags:
      - Ship
      - Line
      - Item
  /{merchantId}/orders/{orderId}/updateMerchantOrderId:
    post:
      summary: Update Merchant Order ID
      description: Updates the merchant order ID for a given order. This method can
        only be called for non-multi-client accounts.
      operationId: content.orders.updatemerchantorderid
      x-api-path-slug: merchantidordersorderidupdatemerchantorderid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order
      responses:
        200:
          description: OK
      tags:
      - Merchant
      - Order
      - ID
  /{merchantId}/orders/{orderId}/updateShipment:
    post:
      summary: Update order Shippment
      description: Updates a shipment's status, carrier, and/or tracking ID. This
        method can only be called for non-multi-client accounts.
      operationId: content.orders.updateshipment
      x-api-path-slug: merchantidordersorderidupdateshipment-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order
      responses:
        200:
          description: OK
      tags:
      - order
      - Shippment
  /{merchantId}/ordersbymerchantid/{merchantOrderId}:
    get:
      summary: Get Order
      description: Retrieves an order using merchant order id. This method can only
        be called for non-multi-client accounts.
      operationId: content.orders.getbymerchantorderid
      x-api-path-slug: merchantidordersbymerchantidmerchantorderid-get
      parameters:
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: merchantOrderId
        description: The merchant order id to be looked for
      responses:
        200:
          description: OK
      tags:
      - Order
  /{merchantId}/products:
    get:
      summary: Get Prudcts
      description: Lists the products in your Merchant Center account. This method
        can only be called for non-multi-client accounts.
      operationId: content.products.list
      x-api-path-slug: merchantidproducts-get
      parameters:
      - in: query
        name: includeInvalidInsertedItems
        description: Flag to include the invalid inserted items in the result of the
          list request
      - in: query
        name: maxResults
        description: The maximum number of products to return in the response, used
          for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Prudcts
    post:
      summary: Upload Product
      description: Uploads a product to your Merchant Center account. If an item with
        the same channel, contentLanguage, offerId, and targetCountry already exists,
        this method updates that entry. This method can only be called for non-multi-client
        accounts.
      operationId: content.products.insert
      x-api-path-slug: merchantidproducts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Product
  /{merchantId}/products/{productId}:
    delete:
      summary: Delete Product
      description: Deletes a product from your Merchant Center account. This method
        can only be called for non-multi-client accounts.
      operationId: content.products.delete
      x-api-path-slug: merchantidproductsproductid-delete
      parameters:
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: productId
        description: The ID of the product
      responses:
        200:
          description: OK
      tags:
      - Product
    get:
      summary: Get Product
      description: Retrieves a product from your Merchant Center account. This method
        can only be called for non-multi-client accounts.
      operationId: content.products.get
      x-api-path-slug: merchantidproductsproductid-get
      parameters:
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: productId
        description: The ID of the product
      responses:
        200:
          description: OK
      tags:
      - Product
  /{merchantId}/productstatuses:
    get:
      summary: Get Product Status
      description: Lists the statuses of the products in your Merchant Center account.
        This method can only be called for non-multi-client accounts.
      operationId: content.productstatuses.list
      x-api-path-slug: merchantidproductstatuses-get
      parameters:
      - in: query
        name: includeInvalidInsertedItems
        description: Flag to include the invalid inserted items in the result of the
          list request
      - in: query
        name: maxResults
        description: The maximum number of product statuses to return in the response,
          used for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Product
      - Status
  /{merchantId}/productstatuses/{productId}:
    get:
      summary: Get Product Status
      description: Gets the status of a product from your Merchant Center account.
        This method can only be called for non-multi-client accounts.
      operationId: content.productstatuses.get
      x-api-path-slug: merchantidproductstatusesproductid-get
      parameters:
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: productId
        description: The ID of the product
      responses:
        200:
          description: OK
      tags:
      - Product
      - Status
  /{merchantId}/shippingsettings:
    get:
      summary: Get Shipping Settings
      description: Lists the shipping settings of the sub-accounts in your Merchant
        Center account. This method can only be called for multi-client accounts.
      operationId: content.shippingsettings.list
      x-api-path-slug: merchantidshippingsettings-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of shipping settings to return in the response,
          used for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Settings
  /{merchantId}/shippingsettings/{accountId}:
    get:
      summary: Get Shipping Settings
      description: 'Retrieves the shipping settings of the account. This method can
        only be called for accounts to which the managing account has access: either
        the managing account itself or sub-accounts if the managing account is a multi-client
        account.'
      operationId: content.shippingsettings.get
      x-api-path-slug: merchantidshippingsettingsaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update shipping settings
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Settings
    patch:
      summary: Update Shipping Settings
      description: 'Updates the shipping settings of the account. This method can
        only be called for accounts to which the managing account has access: either
        the managing account itself or sub-accounts if the managing account is a multi-client
        account. This method supports patch semantics.'
      operationId: content.shippingsettings.patch
      x-api-path-slug: merchantidshippingsettingsaccountid-patch
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update shipping settings
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Settings
    put:
      summary: Update Shipping Settings
      description: 'Updates the shipping settings of the account. This method can
        only be called for accounts to which the managing account has access: either
        the managing account itself or sub-accounts if the managing account is a multi-client
        account.'
      operationId: content.shippingsettings.update
      x-api-path-slug: merchantidshippingsettingsaccountid-put
      parameters:
      - in: path
        name: accountId
        description: The ID of the account for which to get/update shipping settings
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dryRun
        description: Flag to run the request in dry-run mode
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Settings
  /{merchantId}/supportedCarriers:
    get:
      summary: Get Supported Carriers
      description: Retrieves supported carriers and carrier services for an account.
      operationId: content.shippingsettings.getsupportedcarriers
      x-api-path-slug: merchantidsupportedcarriers-get
      parameters:
      - in: path
        name: merchantId
        description: The ID of the account for which to retrieve the supported carriers
      responses:
        200:
          description: OK
      tags:
      - Supported
      - Carriers
  /{merchantId}/testorders:
    post:
      summary: Create Test Order
      description: Sandbox only. Creates a test order. This method can only be called
        for non-multi-client accounts.
      operationId: content.orders.createtestorder
      x-api-path-slug: merchantidtestorders-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Test
      - Order
  /{merchantId}/testorders/{orderId}/advance:
    post:
      summary: Update Test Order
      description: Sandbox only. Moves a test order from state "inProgress" to state
        "pendingShipment". This method can only be called for non-multi-client accounts.
      operationId: content.orders.advancetestorder
      x-api-path-slug: merchantidtestordersorderidadvance-post
      parameters:
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the test order to modify
      responses:
        200:
          description: OK
      tags:
      - Test
      - Order
  /{merchantId}/testordertemplates/{templateName}:
    get:
      summary: Get Test Order
      description: Sandbox only. Retrieves an order template that can be used to quickly
        create a new order in sandbox. This method can only be called for non-multi-client
        accounts.
      operationId: content.orders.gettestordertemplate
      x-api-path-slug: merchantidtestordertemplatestemplatename-get
      parameters:
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: templateName
        description: The name of the template to retrieve
      responses:
        200:
          description: OK
      tags:
      - Test
      - Order