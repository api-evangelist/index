swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 1
info:
  title: Google Doubleclick Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts:
    get:
      summary: Get Accounts
      description: Retrieves the authenticated user's list of accounts.
      operationId: adexchangebuyer.accounts.list
      x-api-path-slug: accounts-get
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Account
  /accounts/{id}:
    get:
      summary: Get Account
      description: Gets one account by ID.
      operationId: adexchangebuyer.accounts.get
      x-api-path-slug: accountsid-get
      parameters:
      - in: path
        name: id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Account
    patch:
      summary: Update Account
      description: Updates an existing account. This method supports patch semantics.
      operationId: adexchangebuyer.accounts.patch
      x-api-path-slug: accountsid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: confirmUnsafeAccountChange
        description: Confirmation for erasing bidder and cookie matching urls
      - in: path
        name: id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Account
    put:
      summary: Update Account
      description: Updates an existing account.
      operationId: adexchangebuyer.accounts.update
      x-api-path-slug: accountsid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: confirmUnsafeAccountChange
        description: Confirmation for erasing bidder and cookie matching urls
      - in: path
        name: id
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Account
  /billinginfo:
    get:
      summary: Get Billing Info
      description: Retrieves a list of billing information for all accounts of the
        authenticated user.
      operationId: adexchangebuyer.billingInfo.list
      x-api-path-slug: billinginfo-get
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Billing
  /billinginfo/{accountId}:
    get:
      summary: Get Billing Info
      description: Returns the billing information for one account specified by account
        ID.
      operationId: adexchangebuyer.billingInfo.get
      x-api-path-slug: billinginfoaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The account id
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Billing
  /billinginfo/{accountId}/{billingId}:
    get:
      summary: Get Budget Info
      description: Returns the budget information for the adgroup specified by the
        accountId and billingId.
      operationId: adexchangebuyer.budget.get
      x-api-path-slug: billinginfoaccountidbillingid-get
      parameters:
      - in: path
        name: accountId
        description: The account id to get the budget information for
      - in: path
        name: billingId
        description: The billing id to get the budget information for
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Budget
    patch:
      summary: Get Budget Amount
      description: Updates the budget amount for the budget of the adgroup specified
        by the accountId and billingId, with the budget amount in the request. This
        method supports patch semantics.
      operationId: adexchangebuyer.budget.patch
      x-api-path-slug: billinginfoaccountidbillingid-patch
      parameters:
      - in: path
        name: accountId
        description: The account id associated with the budget being updated
      - in: path
        name: billingId
        description: The billing id associated with the budget being updated
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Budget
    put:
      summary: Update Budget Amount
      description: Updates the budget amount for the budget of the adgroup specified
        by the accountId and billingId, with the budget amount in the request.
      operationId: adexchangebuyer.budget.update
      x-api-path-slug: billinginfoaccountidbillingid-put
      parameters:
      - in: path
        name: accountId
        description: The account id associated with the budget being updated
      - in: path
        name: billingId
        description: The billing id associated with the budget being updated
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Budget
  /creatives:
    get:
      summary: Get Creatives
      description: Retrieves a list of the authenticated user's active creatives.
        A creative will be available 30-40 minutes after submission.
      operationId: adexchangebuyer.creatives.list
      x-api-path-slug: creatives-get
      parameters:
      - in: query
        name: accountId
        description: When specified, only creatives for the given account ids are
          returned
      - in: query
        name: buyerCreativeId
        description: When specified, only creatives for the given buyer creative ids
          are returned
      - in: query
        name: dealsStatusFilter
        description: When specified, only creatives having the given deals status
          are returned
      - in: query
        name: maxResults
        description: Maximum number of entries returned on one result page
      - in: query
        name: openAuctionStatusFilter
        description: When specified, only creatives having the given open auction
          status are returned
      - in: query
        name: pageToken
        description: A continuation token, used to page through ad clients
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative
    post:
      summary: Submit Creative
      description: Submit a new creative.
      operationId: adexchangebuyer.creatives.insert
      x-api-path-slug: creatives-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative
  /creatives/{accountId}/{buyerCreativeId}:
    get:
      summary: Get Creative Status
      description: Gets the status for a single creative. A creative will be available
        30-40 minutes after submission.
      operationId: adexchangebuyer.creatives.get
      x-api-path-slug: creativesaccountidbuyercreativeid-get
      parameters:
      - in: path
        name: accountId
        description: The id for the account that will serve this creative
      - in: path
        name: buyerCreativeId
        description: The buyer-specific id for this creative
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative
  /creatives/{accountId}/{buyerCreativeId}/addDeal/{dealId}:
    post:
      summary: Create Deal
      description: Add a deal id association for the creative.
      operationId: adexchangebuyer.creatives.addDeal
      x-api-path-slug: creativesaccountidbuyercreativeidadddealdealid-post
      parameters:
      - in: path
        name: accountId
        description: The id for the account that will serve this creative
      - in: path
        name: buyerCreativeId
        description: The buyer-specific id for this creative
      - in: path
        name: dealId
        description: The id of the deal id to associate with this creative
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /creatives/{accountId}/{buyerCreativeId}/listDeals:
    get:
      summary: List Deals
      description: Lists the external deal ids associated with the creative.
      operationId: adexchangebuyer.creatives.listDeals
      x-api-path-slug: creativesaccountidbuyercreativeidlistdeals-get
      parameters:
      - in: path
        name: accountId
        description: The id for the account that will serve this creative
      - in: path
        name: buyerCreativeId
        description: The buyer-specific id for this creative
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /creatives/{accountId}/{buyerCreativeId}/removeDeal/{dealId}:
    post:
      summary: Remove Deal
      description: Remove a deal id associated with the creative.
      operationId: adexchangebuyer.creatives.removeDeal
      x-api-path-slug: creativesaccountidbuyercreativeidremovedealdealid-post
      parameters:
      - in: path
        name: accountId
        description: The id for the account that will serve this creative
      - in: path
        name: buyerCreativeId
        description: The buyer-specific id for this creative
      - in: path
        name: dealId
        description: The id of the deal id to disassociate with this creative
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /performancereport:
    get:
      summary: Get Performance Report
      description: Retrieves the authenticated user's list of performance metrics.
      operationId: adexchangebuyer.performanceReport.list
      x-api-path-slug: performancereport-get
      parameters:
      - in: query
        name: accountId
        description: The account id to get the reports
      - in: query
        name: endDateTime
        description: The end time of the report in ISO 8601 timestamp format using
          UTC
      - in: query
        name: maxResults
        description: Maximum number of entries returned on one result page
      - in: query
        name: pageToken
        description: A continuation token, used to page through performance reports
      - in: query
        name: startDateTime
        description: The start time of the report in ISO 8601 timestamp format using
          UTC
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Performance Report
  /pretargetingconfigs/{accountId}:
    get:
      summary: Get Pretargeting Configs
      description: Retrieves a list of the authenticated user's pretargeting configurations.
      operationId: adexchangebuyer.pretargetingConfig.list
      x-api-path-slug: pretargetingconfigsaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The account id to get the pretargeting configs for
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Pretargeting Config
    post:
      summary: Update Pretargeting Config
      description: Inserts a new pretargeting configuration.
      operationId: adexchangebuyer.pretargetingConfig.insert
      x-api-path-slug: pretargetingconfigsaccountid-post
      parameters:
      - in: path
        name: accountId
        description: The account id to insert the pretargeting config for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Pretargeting Config
  /pretargetingconfigs/{accountId}/{configId}:
    delete:
      summary: Delete Pretargeting Config
      description: Deletes an existing pretargeting config.
      operationId: adexchangebuyer.pretargetingConfig.delete
      x-api-path-slug: pretargetingconfigsaccountidconfigid-delete
      parameters:
      - in: path
        name: accountId
        description: The account id to delete the pretargeting config for
      - in: path
        name: configId
        description: The specific id of the configuration to delete
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Pretargeting Config
    get:
      summary: Get Pretargeting Config
      description: Gets a specific pretargeting configuration
      operationId: adexchangebuyer.pretargetingConfig.get
      x-api-path-slug: pretargetingconfigsaccountidconfigid-get
      parameters:
      - in: path
        name: accountId
        description: The account id to get the pretargeting config for
      - in: path
        name: configId
        description: The specific id of the configuration to retrieve
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Pretargeting Config
    patch:
      summary: Update Pretargeting Config
      description: Updates an existing pretargeting config. This method supports patch
        semantics.
      operationId: adexchangebuyer.pretargetingConfig.patch
      x-api-path-slug: pretargetingconfigsaccountidconfigid-patch
      parameters:
      - in: path
        name: accountId
        description: The account id to update the pretargeting config for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: configId
        description: The specific id of the configuration to update
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Pretargeting Config
    put:
      summary: Update Pretargeting Config
      description: Updates an existing pretargeting config.
      operationId: adexchangebuyer.pretargetingConfig.update
      x-api-path-slug: pretargetingconfigsaccountidconfigid-put
      parameters:
      - in: path
        name: accountId
        description: The account id to update the pretargeting config for
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: configId
        description: The specific id of the configuration to update
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Pretargeting Config
  /privateauction/{privateAuctionId}/updateproposal:
    post:
      summary: Update Proposal
      description: Update a given private auction proposal
      operationId: adexchangebuyer.marketplaceprivateauction.updateproposal
      x-api-path-slug: privateauctionprivateauctionidupdateproposal-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: privateAuctionId
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Proposal
  /products/search:
    get:
      summary: Search
      description: Gets the requested product.
      operationId: adexchangebuyer.products.search
      x-api-path-slug: productssearch-get
      parameters:
      - in: query
        name: pqlQuery
        description: The pql query used to query for products
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Search
  /products/{productId}:
    get:
      summary: Get Product
      description: Gets the requested product by id.
      operationId: adexchangebuyer.products.get
      x-api-path-slug: productsproductid-get
      parameters:
      - in: path
        name: productId
        description: The id for the product to get the head revision for
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Product
  /proposals/insert:
    post:
      summary: Insert Proposal
      description: Create the given list of proposals
      operationId: adexchangebuyer.proposals.insert
      x-api-path-slug: proposalsinsert-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Proposal
  /proposals/search:
    get:
      summary: Search Proposal
      description: Search for proposals using pql query
      operationId: adexchangebuyer.proposals.search
      x-api-path-slug: proposalssearch-get
      parameters:
      - in: query
        name: pqlQuery
        description: Query string to retrieve specific proposals
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Proposal
  /proposals/{proposalId}:
    get:
      summary: Get Proposal
      description: Get a proposal given its id
      operationId: adexchangebuyer.proposals.get
      x-api-path-slug: proposalsproposalid-get
      parameters:
      - in: path
        name: proposalId
        description: Id of the proposal to retrieve
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Proposal
  /proposals/{proposalId}/deals:
    get:
      summary: Get Proposal Deals
      description: List all the deals for a given proposal
      operationId: adexchangebuyer.marketplacedeals.list
      x-api-path-slug: proposalsproposaliddeals-get
      parameters:
      - in: query
        name: pqlQuery
        description: Query string to retrieve specific deals
      - in: path
        name: proposalId
        description: The proposalId to get deals for
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /proposals/{proposalId}/deals/delete:
    post:
      summary: Delete Proposal Deal
      description: Delete the specified deals from the proposal
      operationId: adexchangebuyer.marketplacedeals.delete
      x-api-path-slug: proposalsproposaliddealsdelete-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: proposalId
        description: The proposalId to delete deals from
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /proposals/{proposalId}/deals/insert:
    post:
      summary: Insert Proposal Deal
      description: Add new deals for the specified proposal
      operationId: adexchangebuyer.marketplacedeals.insert
      x-api-path-slug: proposalsproposaliddealsinsert-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: proposalId
        description: proposalId for which deals need to be added
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /proposals/{proposalId}/deals/update:
    post:
      summary: Update Proposal Deal
      description: Replaces all the deals in the proposal with the passed in deals
      operationId: adexchangebuyer.marketplacedeals.update
      x-api-path-slug: proposalsproposaliddealsupdate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: proposalId
        description: The proposalId to edit deals on
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /proposals/{proposalId}/notes:
    get:
      summary: Get Proposal Notes
      description: Get all the notes associated with a proposal
      operationId: adexchangebuyer.marketplacenotes.list
      x-api-path-slug: proposalsproposalidnotes-get
      parameters:
      - in: query
        name: pqlQuery
        description: Query string to retrieve specific notes
      - in: path
        name: proposalId
        description: The proposalId to get notes for
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Note
  /proposals/{proposalId}/notes/insert:
    post:
      summary: Insert Proposal Notes
      description: Add notes to the proposal
      operationId: adexchangebuyer.marketplacenotes.insert
      x-api-path-slug: proposalsproposalidnotesinsert-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: proposalId
        description: The proposalId to add notes for
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Note
  /proposals/{proposalId}/setupcomplete:
    post:
      summary: Update Proposal To Complete
      description: Update the given proposal to indicate that setup has been completed.
      operationId: adexchangebuyer.proposals.setupcomplete
      x-api-path-slug: proposalsproposalidsetupcomplete-post
      parameters:
      - in: path
        name: proposalId
        description: The proposal id for which the setup is complete
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Proposal
  /proposals/{proposalId}/{revisionNumber}/{updateAction}:
    patch:
      summary: Update Proposal Revision Number
      description: Update the given proposal. This method supports patch semantics.
      operationId: adexchangebuyer.proposals.patch
      x-api-path-slug: proposalsproposalidrevisionnumberupdateaction-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: proposalId
        description: The proposal id to update
      - in: path
        name: revisionNumber
        description: The last known revision number to update
      - in: path
        name: updateAction
        description: The proposed action to take on the proposal
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Proposal
    put:
      summary: Update Proposal Revision Number
      description: Update the given proposal
      operationId: adexchangebuyer.proposals.update
      x-api-path-slug: proposalsproposalidrevisionnumberupdateaction-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: proposalId
        description: The proposal id to update
      - in: path
        name: revisionNumber
        description: The last known revision number to update
      - in: path
        name: updateAction
        description: The proposed action to take on the proposal
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Proposal
  /publisher/{accountId}/profiles:
    get:
      summary: Get Publish Profiles
      description: Gets the requested publisher profile(s) by publisher accountId.
      operationId: adexchangebuyer.pubprofiles.list
      x-api-path-slug: publisheraccountidprofiles-get
      parameters:
      - in: path
        name: accountId
        description: The accountId of the publisher to get profiles for
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Profile
  /accounts/{accountId}:
    get:
      summary: Get Account
      description: Get information about the selected Ad Exchange account.
      operationId: adexchangeseller.accounts.get
      x-api-path-slug: accountsaccountid-get
      parameters:
      - in: path
        name: accountId
        description: Account to get information about
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Account
  /accounts/{accountId}/adclients:
    get:
      summary: Get Ad Clients
      description: List all ad clients in this Ad Exchange account.
      operationId: adexchangeseller.accounts.adclients.list
      x-api-path-slug: accountsaccountidadclients-get
      parameters:
      - in: path
        name: accountId
        description: Account to which the ad client belongs
      - in: query
        name: maxResults
        description: The maximum number of ad clients to include in the response,
          used for paging
      - in: query
        name: pageToken
        description: A continuation token, used to page through ad clients
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Clients
  /accounts/{accountId}/adclients/{adClientId}/customchannels:
    get:
      summary: Get Custom Channels
      description: List all custom channels in the specified ad client for this Ad
        Exchange account.
      operationId: adexchangeseller.accounts.customchannels.list
      x-api-path-slug: accountsaccountidadclientsadclientidcustomchannels-get
      parameters:
      - in: path
        name: accountId
        description: Account to which the ad client belongs
      - in: path
        name: adClientId
        description: Ad client for which to list custom channels
      - in: query
        name: maxResults
        description: The maximum number of custom channels to include in the response,
          used for paging
      - in: query
        name: pageToken
        description: A continuation token, used to page through custom channels
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
  /accounts/{accountId}/adclients/{adClientId}/customchannels/{customChannelId}:
    get:
      summary: Get Custom Channels
      description: Get the specified custom channel from the specified ad client.
      operationId: adexchangeseller.accounts.customchannels.get
      x-api-path-slug: accountsaccountidadclientsadclientidcustomchannelscustomchannelid-get
      parameters:
      - in: path
        name: accountId
        description: Account to which the ad client belongs
      - in: path
        name: adClientId
        description: Ad client which contains the custom channel
      - in: path
        name: customChannelId
        description: Custom channel to retrieve
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
  /accounts/{accountId}/adclients/{adClientId}/urlchannels:
    get:
      summary: Get URL Channels
      description: List all URL channels in the specified ad client for this Ad Exchange
        account.
      operationId: adexchangeseller.accounts.urlchannels.list
      x-api-path-slug: accountsaccountidadclientsadclientidurlchannels-get
      parameters:
      - in: path
        name: accountId
        description: Account to which the ad client belongs
      - in: path
        name: adClientId
        description: Ad client for which to list URL channels
      - in: query
        name: maxResults
        description: The maximum number of URL channels to include in the response,
          used for paging
      - in: query
        name: pageToken
        description: A continuation token, used to page through URL channels
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Channels
  /accounts/{accountId}/alerts:
    get:
      summary: Get Alerts
      description: List the alerts for this Ad Exchange account.
      operationId: adexchangeseller.accounts.alerts.list
      x-api-path-slug: accountsaccountidalerts-get
      parameters:
      - in: path
        name: accountId
        description: Account owning the alerts
      - in: query
        name: locale
        description: The locale to use for translating alert messages
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Alert
  /accounts/{accountId}/metadata/dimensions:
    get:
      summary: Get Dimensions
      description: List the metadata for the dimensions available to this AdExchange
        account.
      operationId: adexchangeseller.accounts.metadata.dimensions.list
      x-api-path-slug: accountsaccountidmetadatadimensions-get
      parameters:
      - in: path
        name: accountId
        description: Account with visibility to the dimensions
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Dimension
  /accounts/{accountId}/metadata/metrics:
    get:
      summary: Get Metrics
      description: List the metadata for the metrics available to this AdExchange
        account.
      operationId: adexchangeseller.accounts.metadata.metrics.list
      x-api-path-slug: accountsaccountidmetadatametrics-get
      parameters:
      - in: path
        name: accountId
        description: Account with visibility to the metrics
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Metric
  /accounts/{accountId}/preferreddeals:
    get:
      summary: Get Preferred Deals
      description: List the preferred deals for this Ad Exchange account.
      operationId: adexchangeseller.accounts.preferreddeals.list
      x-api-path-slug: accountsaccountidpreferreddeals-get
      parameters:
      - in: path
        name: accountId
        description: Account owning the deals
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /accounts/{accountId}/preferreddeals/{dealId}:
    get:
      summary: Get Preferred Deal
      description: Get information about the selected Ad Exchange Preferred Deal.
      operationId: adexchangeseller.accounts.preferreddeals.get
      x-api-path-slug: accountsaccountidpreferreddealsdealid-get
      parameters:
      - in: path
        name: accountId
        description: Account owning the deal
      - in: path
        name: dealId
        description: Preferred deal to get information about
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /accounts/{accountId}/reports:
    get:
      summary: Get Reports
      description: Generate an Ad Exchange report based on the report request sent
        in the query parameters. Returns the result as JSON; to retrieve output in
        CSV format specify "alt=csv" as a query parameter.
      operationId: adexchangeseller.accounts.reports.generate
      x-api-path-slug: accountsaccountidreports-get
      parameters:
      - in: path
        name: accountId
        description: Account which owns the generated report
      - in: query
        name: dimension
        description: Dimensions to base the report on
      - in: query
        name: endDate
        description: End of the date range to report on in YYYY-MM-DD format, inclusive
      - in: query
        name: filter
        description: Filters to be run on the report
      - in: query
        name: locale
        description: Optional locale to use for translating report output to a local
          language
      - in: query
        name: maxResults
        description: The maximum number of rows of report data to return
      - in: query
        name: metric
        description: Numeric columns to include in the report
      - in: query
        name: sort
        description: The name of a dimension or metric to sort the resulting report
          on, optionally prefixed with + to sort ascending or - to sort descending
      - in: query
        name: startDate
        description: Start of the date range to report on in YYYY-MM-DD format, inclusive
      - in: query
        name: startIndex
        description: Index of the first row of report data to return
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /accounts/{accountId}/reports/saved:
    get:
      summary: Get Saved Reports
      description: List all saved reports in this Ad Exchange account.
      operationId: adexchangeseller.accounts.reports.saved.list
      x-api-path-slug: accountsaccountidreportssaved-get
      parameters:
      - in: path
        name: accountId
        description: Account owning the saved reports
      - in: query
        name: maxResults
        description: The maximum number of saved reports to include in the response,
          used for paging
      - in: query
        name: pageToken
        description: A continuation token, used to page through saved reports
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /accounts/{accountId}/reports/{savedReportId}:
    get:
      summary: Get Saved Report
      description: Generate an Ad Exchange report based on the saved report ID sent
        in the query parameters.
      operationId: adexchangeseller.accounts.reports.saved.generate
      x-api-path-slug: accountsaccountidreportssavedreportid-get
      parameters:
      - in: path
        name: accountId
        description: Account owning the saved report
      - in: query
        name: locale
        description: Optional locale to use for translating report output to a local
          language
      - in: query
        name: maxResults
        description: The maximum number of rows of report data to return
      - in: path
        name: savedReportId
        description: The saved report to retrieve
      - in: query
        name: startIndex
        description: Index of the first row of report data to return
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /reports/{reportId}/files/{fileId}:
    get:
      summary: Get Report
      description: Retrieves a report file by its report ID and file ID.
      operationId: dfareporting.files.get
      x-api-path-slug: reportsreportidfilesfileid-get
      parameters:
      - in: path
        name: fileId
        description: The ID of the report file
      - in: path
        name: reportId
        description: The ID of the report
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /userprofiles:
    get:
      summary: Get User Profiles
      description: Retrieves list of user profiles for a user.
      operationId: dfareporting.userProfiles.list
      x-api-path-slug: userprofiles-get
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - User
  /userprofiles/{profileId}:
    get:
      summary: Get User Profile
      description: Gets one user profile by ID.
      operationId: dfareporting.userProfiles.get
      x-api-path-slug: userprofilesprofileid-get
      parameters:
      - in: path
        name: profileId
        description: The user profile ID
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - User
  /userprofiles/{profileId}/accountActiveAdSummaries/{summaryAccountId}:
    get:
      summary: Get Account Active Ad Summary
      description: Gets the account's active ad summary by account ID.
      operationId: dfareporting.accountActiveAdSummaries.get
      x-api-path-slug: userprofilesprofileidaccountactiveadsummariessummaryaccountid-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: path
        name: summaryAccountId
        description: Account ID
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Ad
  /userprofiles/{profileId}/accountPermissionGroups:
    get:
      summary: Get Account Permission Groups
      description: Retrieves the list of account permission groups.
      operationId: dfareporting.accountPermissionGroups.list
      x-api-path-slug: userprofilesprofileidaccountpermissiongroups-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Permissions Group
  /userprofiles/{profileId}/accountPermissionGroups/{id}:
    get:
      summary: Get Account Permission Group
      description: Gets one account permission group by ID.
      operationId: dfareporting.accountPermissionGroups.get
      x-api-path-slug: userprofilesprofileidaccountpermissiongroupsid-get
      parameters:
      - in: path
        name: id
        description: Account permission group ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Permissions Group
  /userprofiles/{profileId}/accountPermissions:
    get:
      summary: Get Account Permissions
      description: Retrieves the list of account permissions.
      operationId: dfareporting.accountPermissions.list
      x-api-path-slug: userprofilesprofileidaccountpermissions-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Permissions
  /userprofiles/{profileId}/accountPermissions/{id}:
    get:
      summary: Get Account Permissions
      description: Gets one account permission by ID.
      operationId: dfareporting.accountPermissions.get
      x-api-path-slug: userprofilesprofileidaccountpermissionsid-get
      parameters:
      - in: path
        name: id
        description: Account permission ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Permissions
  /userprofiles/{profileId}/accountUserProfiles:
    get:
      summary: Get Account Users
      description: Retrieves a list of account user profiles, possibly filtered. This
        method supports paging.
      operationId: dfareporting.accountUserProfiles.list
      x-api-path-slug: userprofilesprofileidaccountuserprofiles-get
      parameters:
      - in: query
        name: active
        description: Select only active user profiles
      - in: query
        name: ids
        description: Select only user profiles with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name, ID or email
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      - in: query
        name: subaccountId
        description: Select only user profiles with the specified subaccount ID
      - in: query
        name: userRoleId
        description: Select only user profiles with the specified user role ID
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - User
    patch:
      summary: Update Account User
      description: Updates an existing account user profile. This method supports
        patch semantics.
      operationId: dfareporting.accountUserProfiles.patch
      x-api-path-slug: userprofilesprofileidaccountuserprofiles-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: User profile ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - User
    post:
      summary: Add Account User
      description: Inserts a new account user profile.
      operationId: dfareporting.accountUserProfiles.insert
      x-api-path-slug: userprofilesprofileidaccountuserprofiles-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - User
    put:
      summary: Update Account User
      description: Updates an existing account user profile.
      operationId: dfareporting.accountUserProfiles.update
      x-api-path-slug: userprofilesprofileidaccountuserprofiles-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - User
  /userprofiles/{profileId}/accountUserProfiles/{id}:
    get:
      summary: Get Account User
      description: Gets one account user profile by ID.
      operationId: dfareporting.accountUserProfiles.get
      x-api-path-slug: userprofilesprofileidaccountuserprofilesid-get
      parameters:
      - in: path
        name: id
        description: User profile ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - User
  /userprofiles/{profileId}/accounts:
    get:
      summary: Get Accounts
      description: Retrieves the list of accounts, possibly filtered. This method
        supports paging.
      operationId: dfareporting.accounts.list
      x-api-path-slug: userprofilesprofileidaccounts-get
      parameters:
      - in: query
        name: active
        description: Select only active accounts
      - in: query
        name: ids
        description: Select only accounts with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Account
    patch:
      summary: Update Account
      description: Updates an existing account. This method supports patch semantics.
      operationId: dfareporting.accounts.patch
      x-api-path-slug: userprofilesprofileidaccounts-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Account ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Account
    put:
      summary: Update Account
      description: Updates an existing account.
      operationId: dfareporting.accounts.update
      x-api-path-slug: userprofilesprofileidaccounts-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Account
  /userprofiles/{profileId}/accounts/{id}:
    get:
      summary: Get Account
      description: Gets one account by ID.
      operationId: dfareporting.accounts.get
      x-api-path-slug: userprofilesprofileidaccountsid-get
      parameters:
      - in: path
        name: id
        description: Account ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Account
  /userprofiles/{profileId}/ads:
    get:
      summary: Get Ads
      description: Retrieves a list of ads, possibly filtered. This method supports
        paging.
      operationId: dfareporting.ads.list
      x-api-path-slug: userprofilesprofileidads-get
      parameters:
      - in: query
        name: active
        description: Select only active ads
      - in: query
        name: advertiserId
        description: Select only ads with this advertiser ID
      - in: query
        name: archived
        description: Select only archived ads
      - in: query
        name: audienceSegmentIds
        description: Select only ads with these audience segment IDs
      - in: query
        name: campaignIds
        description: Select only ads with these campaign IDs
      - in: query
        name: compatibility
        description: Select default ads with the specified compatibility
      - in: query
        name: creativeIds
        description: Select only ads with these creative IDs assigned
      - in: query
        name: creativeOptimizationConfigurationIds
        description: Select only ads with these creative optimization configuration
          IDs
      - in: query
        name: dynamicClickTracker
        description: Select only dynamic click trackers
      - in: query
        name: ids
        description: Select only ads with these IDs
      - in: query
        name: landingPageIds
        description: Select only ads with these landing page IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: overriddenEventTagId
        description: Select only ads with this event tag override ID
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: query
        name: placementIds
        description: Select only ads with these placement IDs assigned
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: remarketingListIds
        description: Select only ads whose list targeting expression use these remarketing
          list IDs
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sizeIds
        description: Select only ads with these size IDs
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      - in: query
        name: sslCompliant
        description: Select only ads that are SSL-compliant
      - in: query
        name: sslRequired
        description: Select only ads that require SSL
      - in: query
        name: type
        description: Select only ads with these types
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Ad
    patch:
      summary: Update Ad
      description: Updates an existing ad. This method supports patch semantics.
      operationId: dfareporting.ads.patch
      x-api-path-slug: userprofilesprofileidads-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Ad ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Ad
    post:
      summary: Create Ad
      description: Inserts a new ad.
      operationId: dfareporting.ads.insert
      x-api-path-slug: userprofilesprofileidads-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Ad
    put:
      summary: Update Ad
      description: Updates an existing ad.
      operationId: dfareporting.ads.update
      x-api-path-slug: userprofilesprofileidads-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Ad
  /userprofiles/{profileId}/ads/{id}:
    get:
      summary: Get Ad
      description: Gets one ad by ID.
      operationId: dfareporting.ads.get
      x-api-path-slug: userprofilesprofileidadsid-get
      parameters:
      - in: path
        name: id
        description: Ad ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Ad
  /userprofiles/{profileId}/advertiserGroups:
    get:
      summary: Get Advertiser Groups
      description: Retrieves a list of advertiser groups, possibly filtered. This
        method supports paging.
      operationId: dfareporting.advertiserGroups.list
      x-api-path-slug: userprofilesprofileidadvertisergroups-get
      parameters:
      - in: query
        name: ids
        description: Select only advertiser groups with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Advertiser Group
    patch:
      summary: Update Advertiser Group
      description: Updates an existing advertiser group. This method supports patch
        semantics.
      operationId: dfareporting.advertiserGroups.patch
      x-api-path-slug: userprofilesprofileidadvertisergroups-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Advertiser group ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Advertiser Group
    post:
      summary: Create Advertiser Group
      description: Inserts a new advertiser group.
      operationId: dfareporting.advertiserGroups.insert
      x-api-path-slug: userprofilesprofileidadvertisergroups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Advertiser Group
    put:
      summary: Update Advertiser Group
      description: Updates an existing advertiser group.
      operationId: dfareporting.advertiserGroups.update
      x-api-path-slug: userprofilesprofileidadvertisergroups-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Advertiser Group
  /userprofiles/{profileId}/advertiserGroups/{id}:
    delete:
      summary: Update Advertiser Delete
      description: Deletes an existing advertiser group.
      operationId: dfareporting.advertiserGroups.delete
      x-api-path-slug: userprofilesprofileidadvertisergroupsid-delete
      parameters:
      - in: path
        name: id
        description: Advertiser group ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Advertiser Group
    get:
      summary: Get Advertiser Group
      description: Gets one advertiser group by ID.
      operationId: dfareporting.advertiserGroups.get
      x-api-path-slug: userprofilesprofileidadvertisergroupsid-get
      parameters:
      - in: path
        name: id
        description: Advertiser group ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Advertiser Group
  /userprofiles/{profileId}/advertisers:
    get:
      summary: Get Advertisers
      description: Retrieves a list of advertisers, possibly filtered. This method
        supports paging.
      operationId: dfareporting.advertisers.list
      x-api-path-slug: userprofilesprofileidadvertisers-get
      parameters:
      - in: query
        name: advertiserGroupIds
        description: Select only advertisers with these advertiser group IDs
      - in: query
        name: floodlightConfigurationIds
        description: Select only advertisers with these floodlight configuration IDs
      - in: query
        name: ids
        description: Select only advertisers with these IDs
      - in: query
        name: includeAdvertisersWithoutGroupsOnly
        description: Select only advertisers which do not belong to any advertiser
          group
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: onlyParent
        description: Select only advertisers which use another advertisers floodlight
          configuration
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      - in: query
        name: status
        description: Select only advertisers with the specified status
      - in: query
        name: subaccountId
        description: Select only advertisers with these subaccount IDs
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Advertiser
    patch:
      summary: Update Advertiser
      description: Updates an existing advertiser. This method supports patch semantics.
      operationId: dfareporting.advertisers.patch
      x-api-path-slug: userprofilesprofileidadvertisers-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Advertiser ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Advertiser
    post:
      summary: Create Advertiser
      description: Inserts a new advertiser.
      operationId: dfareporting.advertisers.insert
      x-api-path-slug: userprofilesprofileidadvertisers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Advertiser
    put:
      summary: Update Advertiser
      description: Updates an existing advertiser.
      operationId: dfareporting.advertisers.update
      x-api-path-slug: userprofilesprofileidadvertisers-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Advertiser
  /userprofiles/{profileId}/advertisers/{id}:
    get:
      summary: Get Advertiser
      description: Gets one advertiser by ID.
      operationId: dfareporting.advertisers.get
      x-api-path-slug: userprofilesprofileidadvertisersid-get
      parameters:
      - in: path
        name: id
        description: Advertiser ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Advertiser
  /userprofiles/{profileId}/browsers:
    get:
      summary: Get Browsers
      description: Retrieves a list of browsers.
      operationId: dfareporting.browsers.list
      x-api-path-slug: userprofilesprofileidbrowsers-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Browser
  /userprofiles/{profileId}/campaigns:
    get:
      summary: Get Campaigns
      description: Retrieves a list of campaigns, possibly filtered. This method supports
        paging.
      operationId: dfareporting.campaigns.list
      x-api-path-slug: userprofilesprofileidcampaigns-get
      parameters:
      - in: query
        name: advertiserGroupIds
        description: Select only campaigns whose advertisers belong to these advertiser
          groups
      - in: query
        name: advertiserIds
        description: Select only campaigns that belong to these advertisers
      - in: query
        name: archived
        description: Select only archived campaigns
      - in: query
        name: atLeastOneOptimizationActivity
        description: Select only campaigns that have at least one optimization activity
      - in: query
        name: excludedIds
        description: Exclude campaigns with these IDs
      - in: query
        name: ids
        description: Select only campaigns with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: overriddenEventTagId
        description: Select only campaigns that have overridden this event tag ID
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for campaigns by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      - in: query
        name: subaccountId
        description: Select only campaigns that belong to this subaccount
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Campaign
    patch:
      summary: Update Campaign
      description: Updates an existing campaign. This method supports patch semantics.
      operationId: dfareporting.campaigns.patch
      x-api-path-slug: userprofilesprofileidcampaigns-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Campaign ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Campaign
    post:
      summary: Create Campaign
      description: Inserts a new campaign.
      operationId: dfareporting.campaigns.insert
      x-api-path-slug: userprofilesprofileidcampaigns-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: defaultLandingPageName
        description: Default landing page name for this new campaign
      - in: query
        name: defaultLandingPageUrl
        description: Default landing page URL for this new campaign
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Campaign
    put:
      summary: Update Campaign
      description: Updates an existing campaign.
      operationId: dfareporting.campaigns.update
      x-api-path-slug: userprofilesprofileidcampaigns-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Campaign
  /userprofiles/{profileId}/campaigns/{campaignId}/campaignCreativeAssociations:
    get:
      summary: Get Campaign Creatives
      description: Retrieves the list of creative IDs associated with the specified
        campaign. This method supports paging.
      operationId: dfareporting.campaignCreativeAssociations.list
      x-api-path-slug: userprofilesprofileidcampaignscampaignidcampaigncreativeassociations-get
      parameters:
      - in: path
        name: campaignId
        description: Campaign ID in this association
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Campaign Creatives
    post:
      summary: Add Campaign Creative
      description: Associates a creative with the specified campaign. This method
        creates a default ad with dimensions matching the creative in the campaign
        if such a default ad does not exist already.
      operationId: dfareporting.campaignCreativeAssociations.insert
      x-api-path-slug: userprofilesprofileidcampaignscampaignidcampaigncreativeassociations-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: campaignId
        description: Campaign ID in this association
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Campaign Creatives
  /userprofiles/{profileId}/campaigns/{campaignId}/landingPages:
    get:
      summary: Get Landing Pages
      description: Retrieves the list of landing pages for the specified campaign.
      operationId: dfareporting.landingPages.list
      x-api-path-slug: userprofilesprofileidcampaignscampaignidlandingpages-get
      parameters:
      - in: path
        name: campaignId
        description: Landing page campaign ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Landing Page
    patch:
      summary: Update Landing Page
      description: Updates an existing campaign landing page. This method supports
        patch semantics.
      operationId: dfareporting.landingPages.patch
      x-api-path-slug: userprofilesprofileidcampaignscampaignidlandingpages-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: campaignId
        description: Landing page campaign ID
      - in: query
        name: id
        description: Landing page ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Landing Page
    post:
      summary: Add Landing Page
      description: Inserts a new landing page for the specified campaign.
      operationId: dfareporting.landingPages.insert
      x-api-path-slug: userprofilesprofileidcampaignscampaignidlandingpages-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: campaignId
        description: Landing page campaign ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Landing Page
    put:
      summary: Update Landing Page
      description: Updates an existing campaign landing page.
      operationId: dfareporting.landingPages.update
      x-api-path-slug: userprofilesprofileidcampaignscampaignidlandingpages-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: campaignId
        description: Landing page campaign ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Landing Page
  /userprofiles/{profileId}/campaigns/{campaignId}/landingPages/{id}:
    delete:
      summary: Delete Landing Page
      description: Deletes an existing campaign landing page.
      operationId: dfareporting.landingPages.delete
      x-api-path-slug: userprofilesprofileidcampaignscampaignidlandingpagesid-delete
      parameters:
      - in: path
        name: campaignId
        description: Landing page campaign ID
      - in: path
        name: id
        description: Landing page ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Landing Page
    get:
      summary: Get Landing Page
      description: Gets one campaign landing page by ID.
      operationId: dfareporting.landingPages.get
      x-api-path-slug: userprofilesprofileidcampaignscampaignidlandingpagesid-get
      parameters:
      - in: path
        name: campaignId
        description: Landing page campaign ID
      - in: path
        name: id
        description: Landing page ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Landing Page
  /userprofiles/{profileId}/campaigns/{id}:
    get:
      summary: Get Campaign
      description: Gets one campaign by ID.
      operationId: dfareporting.campaigns.get
      x-api-path-slug: userprofilesprofileidcampaignsid-get
      parameters:
      - in: path
        name: id
        description: Campaign ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Campaign
  /userprofiles/{profileId}/changeLogs:
    get:
      summary: Get Change Logs
      description: Retrieves a list of change logs. This method supports paging.
      operationId: dfareporting.changeLogs.list
      x-api-path-slug: userprofilesprofileidchangelogs-get
      parameters:
      - in: query
        name: action
        description: Select only change logs with the specified action
      - in: query
        name: ids
        description: Select only change logs with these IDs
      - in: query
        name: maxChangeTime
        description: Select only change logs whose change time is before the specified
          maxChangeTime
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: minChangeTime
        description: Select only change logs whose change time is before the specified
          minChangeTime
      - in: query
        name: objectIds
        description: Select only change logs with these object IDs
      - in: query
        name: objectType
        description: Select only change logs with the specified object type
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Select only change logs whose object ID, user name, old or new
          values match the search string
      - in: query
        name: userProfileIds
        description: Select only change logs with these user profile IDs
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Change Log
  /userprofiles/{profileId}/changeLogs/{id}:
    get:
      summary: Get Change Log
      description: Gets one change log by ID.
      operationId: dfareporting.changeLogs.get
      x-api-path-slug: userprofilesprofileidchangelogsid-get
      parameters:
      - in: path
        name: id
        description: Change log ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Change Log
  /userprofiles/{profileId}/cities:
    get:
      summary: Get Cities
      description: Retrieves a list of cities, possibly filtered.
      operationId: dfareporting.cities.list
      x-api-path-slug: userprofilesprofileidcities-get
      parameters:
      - in: query
        name: countryDartIds
        description: Select only cities from these countries
      - in: query
        name: dartIds
        description: Select only cities with these DART IDs
      - in: query
        name: namePrefix
        description: Select only cities with names starting with this prefix
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: regionDartIds
        description: Select only cities from these regions
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - City
  /userprofiles/{profileId}/connectionTypes:
    get:
      summary: Get Connection Types
      description: Retrieves a list of connection types.
      operationId: dfareporting.connectionTypes.list
      x-api-path-slug: userprofilesprofileidconnectiontypes-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Connection Type
  /userprofiles/{profileId}/connectionTypes/{id}:
    get:
      summary: Get Connection Type
      description: Gets one connection type by ID.
      operationId: dfareporting.connectionTypes.get
      x-api-path-slug: userprofilesprofileidconnectiontypesid-get
      parameters:
      - in: path
        name: id
        description: Connection type ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Connection Type
  /userprofiles/{profileId}/contentCategories:
    get:
      summary: Get Content Categories
      description: Retrieves a list of content categories, possibly filtered. This
        method supports paging.
      operationId: dfareporting.contentCategories.list
      x-api-path-slug: userprofilesprofileidcontentcategories-get
      parameters:
      - in: query
        name: ids
        description: Select only content categories with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Content Category
    patch:
      summary: Get Content Category
      description: Updates an existing content category. This method supports patch
        semantics.
      operationId: dfareporting.contentCategories.patch
      x-api-path-slug: userprofilesprofileidcontentcategories-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Content category ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Content Category
    post:
      summary: Create Content Category
      description: Inserts a new content category.
      operationId: dfareporting.contentCategories.insert
      x-api-path-slug: userprofilesprofileidcontentcategories-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Content Category
    put:
      summary: Update Content Category
      description: Updates an existing content category.
      operationId: dfareporting.contentCategories.update
      x-api-path-slug: userprofilesprofileidcontentcategories-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Content Category
  /userprofiles/{profileId}/contentCategories/{id}:
    delete:
      summary: Delete Content Category
      description: Deletes an existing content category.
      operationId: dfareporting.contentCategories.delete
      x-api-path-slug: userprofilesprofileidcontentcategoriesid-delete
      parameters:
      - in: path
        name: id
        description: Content category ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Content Category
    get:
      summary: Get Content Category
      description: Gets one content category by ID.
      operationId: dfareporting.contentCategories.get
      x-api-path-slug: userprofilesprofileidcontentcategoriesid-get
      parameters:
      - in: path
        name: id
        description: Content category ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Content Category
  /userprofiles/{profileId}/conversions/batchinsert:
    post:
      summary: Insert Conversions
      description: Inserts conversions.
      operationId: dfareporting.conversions.batchinsert
      x-api-path-slug: userprofilesprofileidconversionsbatchinsert-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Conversion
  /userprofiles/{profileId}/countries:
    get:
      summary: Get Countries
      description: Retrieves a list of countries.
      operationId: dfareporting.countries.list
      x-api-path-slug: userprofilesprofileidcountries-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Country
  /userprofiles/{profileId}/countries/{dartId}:
    get:
      summary: Get Country
      description: Gets one country by ID.
      operationId: dfareporting.countries.get
      x-api-path-slug: userprofilesprofileidcountriesdartid-get
      parameters:
      - in: path
        name: dartId
        description: Country DART ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Country
  /userprofiles/{profileId}/creativeAssets/{advertiserId}/creativeAssets:
    post:
      summary: Insert Creative Asset
      description: Inserts a new creative asset.
      operationId: dfareporting.creativeAssets.insert
      x-api-path-slug: userprofilesprofileidcreativeassetsadvertiseridcreativeassets-post
      parameters:
      - in: path
        name: advertiserId
        description: Advertiser ID of this creative
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Asset
  /userprofiles/{profileId}/creativeFields:
    get:
      summary: Get Creative Fields
      description: Retrieves a list of creative fields, possibly filtered. This method
        supports paging.
      operationId: dfareporting.creativeFields.list
      x-api-path-slug: userprofilesprofileidcreativefields-get
      parameters:
      - in: query
        name: advertiserIds
        description: Select only creative fields that belong to these advertisers
      - in: query
        name: ids
        description: Select only creative fields with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for creative fields by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Field
    patch:
      summary: Update Creative Fields
      description: Updates an existing creative field. This method supports patch
        semantics.
      operationId: dfareporting.creativeFields.patch
      x-api-path-slug: userprofilesprofileidcreativefields-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Creative Field ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Field
    post:
      summary: Create Creative Fields
      description: Inserts a new creative field.
      operationId: dfareporting.creativeFields.insert
      x-api-path-slug: userprofilesprofileidcreativefields-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Field
    put:
      summary: Update Creative Fields
      description: Updates an existing creative field.
      operationId: dfareporting.creativeFields.update
      x-api-path-slug: userprofilesprofileidcreativefields-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Field
  /userprofiles/{profileId}/creativeFields/{creativeFieldId}/creativeFieldValues:
    get:
      summary: Get Creative Field Values
      description: Retrieves a list of creative field values, possibly filtered. This
        method supports paging.
      operationId: dfareporting.creativeFieldValues.list
      x-api-path-slug: userprofilesprofileidcreativefieldscreativefieldidcreativefieldvalues-get
      parameters:
      - in: path
        name: creativeFieldId
        description: Creative field ID for this creative field value
      - in: query
        name: ids
        description: Select only creative field values with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for creative field values by their values
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Field
    patch:
      summary: Update Creative Field Value
      description: Updates an existing creative field value. This method supports
        patch semantics.
      operationId: dfareporting.creativeFieldValues.patch
      x-api-path-slug: userprofilesprofileidcreativefieldscreativefieldidcreativefieldvalues-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: creativeFieldId
        description: Creative field ID for this creative field value
      - in: query
        name: id
        description: Creative Field Value ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Field
    post:
      summary: Insert Creative Field Value
      description: Inserts a new creative field value.
      operationId: dfareporting.creativeFieldValues.insert
      x-api-path-slug: userprofilesprofileidcreativefieldscreativefieldidcreativefieldvalues-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: creativeFieldId
        description: Creative field ID for this creative field value
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Field
    put:
      summary: Update Creative Field Value
      description: Updates an existing creative field value.
      operationId: dfareporting.creativeFieldValues.update
      x-api-path-slug: userprofilesprofileidcreativefieldscreativefieldidcreativefieldvalues-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: creativeFieldId
        description: Creative field ID for this creative field value
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Field
  /userprofiles/{profileId}/creativeFields/{creativeFieldId}/creativeFieldValues/{id}:
    delete:
      summary: Delete Creative Field Value
      description: Deletes an existing creative field value.
      operationId: dfareporting.creativeFieldValues.delete
      x-api-path-slug: userprofilesprofileidcreativefieldscreativefieldidcreativefieldvaluesid-delete
      parameters:
      - in: path
        name: creativeFieldId
        description: Creative field ID for this creative field value
      - in: path
        name: id
        description: Creative Field Value ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Field
    get:
      summary: UpGetdate Creative Field Value
      description: Gets one creative field value by ID.
      operationId: dfareporting.creativeFieldValues.get
      x-api-path-slug: userprofilesprofileidcreativefieldscreativefieldidcreativefieldvaluesid-get
      parameters:
      - in: path
        name: creativeFieldId
        description: Creative field ID for this creative field value
      - in: path
        name: id
        description: Creative Field Value ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Field
  /userprofiles/{profileId}/creativeFields/{id}:
    delete:
      summary: Delete Creative Field
      description: Deletes an existing creative field.
      operationId: dfareporting.creativeFields.delete
      x-api-path-slug: userprofilesprofileidcreativefieldsid-delete
      parameters:
      - in: path
        name: id
        description: Creative Field ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Field
    get:
      summary: Get Creative Field
      description: Gets one creative field by ID.
      operationId: dfareporting.creativeFields.get
      x-api-path-slug: userprofilesprofileidcreativefieldsid-get
      parameters:
      - in: path
        name: id
        description: Creative Field ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Field
  /userprofiles/{profileId}/creativeGroups:
    get:
      summary: Get Creative Groups
      description: Retrieves a list of creative groups, possibly filtered. This method
        supports paging.
      operationId: dfareporting.creativeGroups.list
      x-api-path-slug: userprofilesprofileidcreativegroups-get
      parameters:
      - in: query
        name: advertiserIds
        description: Select only creative groups that belong to these advertisers
      - in: query
        name: groupNumber
        description: Select only creative groups that belong to this subgroup
      - in: query
        name: ids
        description: Select only creative groups with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for creative groups by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Group
    patch:
      summary: Update Creative Group
      description: Updates an existing creative group. This method supports patch
        semantics.
      operationId: dfareporting.creativeGroups.patch
      x-api-path-slug: userprofilesprofileidcreativegroups-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Creative group ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Group
    post:
      summary: Insert Creative Group
      description: Inserts a new creative group.
      operationId: dfareporting.creativeGroups.insert
      x-api-path-slug: userprofilesprofileidcreativegroups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Group
    put:
      summary: Update Creative Group
      description: Updates an existing creative group.
      operationId: dfareporting.creativeGroups.update
      x-api-path-slug: userprofilesprofileidcreativegroups-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Group
  /userprofiles/{profileId}/creativeGroups/{id}:
    get:
      summary: Get Creative Group
      description: Gets one creative group by ID.
      operationId: dfareporting.creativeGroups.get
      x-api-path-slug: userprofilesprofileidcreativegroupsid-get
      parameters:
      - in: path
        name: id
        description: Creative group ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative Group
  /userprofiles/{profileId}/creatives:
    get:
      summary: Get Creatives
      description: Retrieves a list of creatives, possibly filtered. This method supports
        paging.
      operationId: dfareporting.creatives.list
      x-api-path-slug: userprofilesprofileidcreatives-get
      parameters:
      - in: query
        name: active
        description: Select only active creatives
      - in: query
        name: advertiserId
        description: Select only creatives with this advertiser ID
      - in: query
        name: archived
        description: Select only archived creatives
      - in: query
        name: campaignId
        description: Select only creatives with this campaign ID
      - in: query
        name: companionCreativeIds
        description: Select only in-stream video creatives with these companion IDs
      - in: query
        name: creativeFieldIds
        description: Select only creatives with these creative field IDs
      - in: query
        name: ids
        description: Select only creatives with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: renderingIds
        description: Select only creatives with these rendering IDs
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sizeIds
        description: Select only creatives with these size IDs
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      - in: query
        name: studioCreativeId
        description: Select only creatives corresponding to this Studio creative ID
      - in: query
        name: types
        description: Select only creatives with these creative types
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative
    patch:
      summary: Update Creative
      description: Updates an existing creative. This method supports patch semantics.
      operationId: dfareporting.creatives.patch
      x-api-path-slug: userprofilesprofileidcreatives-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Creative ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative
    post:
      summary: Insert Creative
      description: Inserts a new creative.
      operationId: dfareporting.creatives.insert
      x-api-path-slug: userprofilesprofileidcreatives-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative
    put:
      summary: Update Creative
      description: Updates an existing creative.
      operationId: dfareporting.creatives.update
      x-api-path-slug: userprofilesprofileidcreatives-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative
  /userprofiles/{profileId}/creatives/{id}:
    get:
      summary: Get Creative
      description: Gets one creative by ID.
      operationId: dfareporting.creatives.get
      x-api-path-slug: userprofilesprofileidcreativesid-get
      parameters:
      - in: path
        name: id
        description: Creative ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Creative
  /userprofiles/{profileId}/dimensionvalues/query:
    post:
      summary: Get Report Dimension
      description: Retrieves list of report dimension values for a list of filters.
      operationId: dfareporting.dimensionValues.query
      x-api-path-slug: userprofilesprofileiddimensionvaluesquery-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous result page
      - in: path
        name: profileId
        description: The DFA user profile ID
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /userprofiles/{profileId}/directorySiteContacts:
    get:
      summary: Get Directory Site Contacts
      description: Retrieves a list of directory site contacts, possibly filtered.
        This method supports paging.
      operationId: dfareporting.directorySiteContacts.list
      x-api-path-slug: userprofilesprofileiddirectorysitecontacts-get
      parameters:
      - in: query
        name: directorySiteIds
        description: Select only directory site contacts with these directory site
          IDs
      - in: query
        name: ids
        description: Select only directory site contacts with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name, ID or email
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Contact
  /userprofiles/{profileId}/directorySiteContacts/{id}:
    get:
      summary: Get Directory Site Contact
      description: Gets one directory site contact by ID.
      operationId: dfareporting.directorySiteContacts.get
      x-api-path-slug: userprofilesprofileiddirectorysitecontactsid-get
      parameters:
      - in: path
        name: id
        description: Directory site contact ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Contact
  /userprofiles/{profileId}/directorySites:
    get:
      summary: Get Directory Sites
      description: Retrieves a list of directory sites, possibly filtered. This method
        supports paging.
      operationId: dfareporting.directorySites.list
      x-api-path-slug: userprofilesprofileiddirectorysites-get
      parameters:
      - in: query
        name: acceptsInStreamVideoPlacements
        description: This search filter is no longer supported and will have no effect
          on the results returned
      - in: query
        name: acceptsInterstitialPlacements
        description: This search filter is no longer supported and will have no effect
          on the results returned
      - in: query
        name: acceptsPublisherPaidPlacements
        description: Select only directory sites that accept publisher paid placements
      - in: query
        name: active
        description: Select only active directory sites
      - in: query
        name: countryId
        description: Select only directory sites with this country ID
      - in: query
        name: dfp_network_code
        description: Select only directory sites with this DFP network code
      - in: query
        name: ids
        description: Select only directory sites with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: query
        name: parentId
        description: Select only directory sites with this parent ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name, ID or URL
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Directory Site
    post:
      summary: Insert Directory Site
      description: Inserts a new directory site.
      operationId: dfareporting.directorySites.insert
      x-api-path-slug: userprofilesprofileiddirectorysites-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Directory Site
  /userprofiles/{profileId}/directorySites/{id}:
    get:
      summary: Get Directory Site
      description: Gets one directory site by ID.
      operationId: dfareporting.directorySites.get
      x-api-path-slug: userprofilesprofileiddirectorysitesid-get
      parameters:
      - in: path
        name: id
        description: Directory site ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Directory Site
  /userprofiles/{profileId}/dynamicTargetingKeys:
    get:
      summary: Get Dynamic Targeting Keys
      description: Retrieves a list of dynamic targeting keys.
      operationId: dfareporting.dynamicTargetingKeys.list
      x-api-path-slug: userprofilesprofileiddynamictargetingkeys-get
      parameters:
      - in: query
        name: advertiserId
        description: Select only dynamic targeting keys whose object has this advertiser
          ID
      - in: query
        name: names
        description: Select only dynamic targeting keys exactly matching these names
      - in: query
        name: objectId
        description: Select only dynamic targeting keys with this object ID
      - in: query
        name: objectType
        description: Select only dynamic targeting keys with this object type
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Dynamic Targeting Key
    post:
      summary: Insert Dynamic Targeting Key
      description: Inserts a new dynamic targeting key. Keys must be created at the
        advertiser level before being assigned to the advertiser's ads, creatives,
        or placements. There is a maximum of 1000 keys per advertiser, out of which
        a maximum of 20 keys can be assigned per ad, creative, or placement.
      operationId: dfareporting.dynamicTargetingKeys.insert
      x-api-path-slug: userprofilesprofileiddynamictargetingkeys-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Dynamic Targeting Key
  /userprofiles/{profileId}/dynamicTargetingKeys/{objectId}:
    delete:
      summary: Delete Dynamic Targeting Key
      description: Deletes an existing dynamic targeting key.
      operationId: dfareporting.dynamicTargetingKeys.delete
      x-api-path-slug: userprofilesprofileiddynamictargetingkeysobjectid-delete
      parameters:
      - in: query
        name: name
        description: Name of this dynamic targeting key
      - in: path
        name: objectId
        description: ID of the object of this dynamic targeting key
      - in: query
        name: objectType
        description: Type of the object of this dynamic targeting key
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Dynamic Targeting Key
  /userprofiles/{profileId}/eventTags:
    get:
      summary: Get Event Tags
      description: Retrieves a list of event tags, possibly filtered.
      operationId: dfareporting.eventTags.list
      x-api-path-slug: userprofilesprofileideventtags-get
      parameters:
      - in: query
        name: adId
        description: Select only event tags that belong to this ad
      - in: query
        name: advertiserId
        description: Select only event tags that belong to this advertiser
      - in: query
        name: campaignId
        description: Select only event tags that belong to this campaign
      - in: query
        name: definitionsOnly
        description: Examine only the specified campaign or advertisers event tags
          for matching selector criteria
      - in: query
        name: enabled
        description: Select only enabled event tags
      - in: query
        name: eventTagTypes
        description: Select only event tags with the specified event tag types
      - in: query
        name: ids
        description: Select only event tags with these IDs
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Event Tag
    patch:
      summary: Update Event Tag
      description: Updates an existing event tag. This method supports patch semantics.
      operationId: dfareporting.eventTags.patch
      x-api-path-slug: userprofilesprofileideventtags-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Event tag ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Event Tag
    post:
      summary: Insert Event Tag
      description: Inserts a new event tag.
      operationId: dfareporting.eventTags.insert
      x-api-path-slug: userprofilesprofileideventtags-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Event Tag
    put:
      summary: Update Event Tag
      description: Updates an existing event tag.
      operationId: dfareporting.eventTags.update
      x-api-path-slug: userprofilesprofileideventtags-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Event Tag
  /userprofiles/{profileId}/eventTags/{id}:
    delete:
      summary: Delete Event Tag
      description: Deletes an existing event tag.
      operationId: dfareporting.eventTags.delete
      x-api-path-slug: userprofilesprofileideventtagsid-delete
      parameters:
      - in: path
        name: id
        description: Event tag ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Event Tag
    get:
      summary: Get Event Tag
      description: Gets one event tag by ID.
      operationId: dfareporting.eventTags.get
      x-api-path-slug: userprofilesprofileideventtagsid-get
      parameters:
      - in: path
        name: id
        description: Event tag ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Event Tag
  /userprofiles/{profileId}/files:
    get:
      summary: Get Files
      description: Lists files for a user profile.
      operationId: dfareporting.files.list
      x-api-path-slug: userprofilesprofileidfiles-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous result page
      - in: path
        name: profileId
        description: The DFA profile ID
      - in: query
        name: scope
        description: The scope that defines which results are returned, default is
          MINE
      - in: query
        name: sortField
        description: The field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is DESCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - File
  /userprofiles/{profileId}/floodlightActivities:
    get:
      summary: Get Floodlight Activities
      description: Retrieves a list of floodlight activities, possibly filtered. This
        method supports paging.
      operationId: dfareporting.floodlightActivities.list
      x-api-path-slug: userprofilesprofileidfloodlightactivities-get
      parameters:
      - in: query
        name: advertiserId
        description: Select only floodlight activities for the specified advertiser
          ID
      - in: query
        name: floodlightActivityGroupIds
        description: Select only floodlight activities with the specified floodlight
          activity group IDs
      - in: query
        name: floodlightActivityGroupName
        description: Select only floodlight activities with the specified floodlight
          activity group name
      - in: query
        name: floodlightActivityGroupTagString
        description: Select only floodlight activities with the specified floodlight
          activity group tag string
      - in: query
        name: floodlightActivityGroupType
        description: Select only floodlight activities with the specified floodlight
          activity group type
      - in: query
        name: floodlightConfigurationId
        description: Select only floodlight activities for the specified floodlight
          configuration ID
      - in: query
        name: ids
        description: Select only floodlight activities with the specified IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      - in: query
        name: tagString
        description: Select only floodlight activities with the specified tag string
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Floodlight Activity
    patch:
      summary: Update Floodlight Activity
      description: Updates an existing floodlight activity. This method supports patch
        semantics.
      operationId: dfareporting.floodlightActivities.patch
      x-api-path-slug: userprofilesprofileidfloodlightactivities-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Floodlight activity ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Floodlight Activity
    post:
      summary: Insert Floodlight Activity
      description: Inserts a new floodlight activity.
      operationId: dfareporting.floodlightActivities.insert
      x-api-path-slug: userprofilesprofileidfloodlightactivities-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Floodlight Activity
    put:
      summary: Update Floodlight Activity
      description: Updates an existing floodlight activity.
      operationId: dfareporting.floodlightActivities.update
      x-api-path-slug: userprofilesprofileidfloodlightactivities-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Floodlight Activity
  /userprofiles/{profileId}/floodlightActivities/generatetag:
    post:
      summary: Generate Tag for Floodlight Activity
      description: Generates a tag for a floodlight activity.
      operationId: dfareporting.floodlightActivities.generatetag
      x-api-path-slug: userprofilesprofileidfloodlightactivitiesgeneratetag-post
      parameters:
      - in: query
        name: floodlightActivityId
        description: Floodlight activity ID for which we want to generate a tag
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Floodlight Activity
  /userprofiles/{profileId}/floodlightActivities/{id}:
    delete:
      summary: Delete Floodlight Activity
      description: Deletes an existing floodlight activity.
      operationId: dfareporting.floodlightActivities.delete
      x-api-path-slug: userprofilesprofileidfloodlightactivitiesid-delete
      parameters:
      - in: path
        name: id
        description: Floodlight activity ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Floodlight Activity
    get:
      summary: Get Floodlight Activity
      description: Gets one floodlight activity by ID.
      operationId: dfareporting.floodlightActivities.get
      x-api-path-slug: userprofilesprofileidfloodlightactivitiesid-get
      parameters:
      - in: path
        name: id
        description: Floodlight activity ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Floodlight Activity
  /userprofiles/{profileId}/floodlightActivityGroups:
    get:
      summary: Get Floodlight Activity Groups
      description: Retrieves a list of floodlight activity groups, possibly filtered.
        This method supports paging.
      operationId: dfareporting.floodlightActivityGroups.list
      x-api-path-slug: userprofilesprofileidfloodlightactivitygroups-get
      parameters:
      - in: query
        name: advertiserId
        description: Select only floodlight activity groups with the specified advertiser
          ID
      - in: query
        name: floodlightConfigurationId
        description: Select only floodlight activity groups with the specified floodlight
          configuration ID
      - in: query
        name: ids
        description: Select only floodlight activity groups with the specified IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      - in: query
        name: type
        description: Select only floodlight activity groups with the specified floodlight
          activity group type
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Floodlight Activity Group
    patch:
      summary: Update Floodlight Activity Group
      description: Updates an existing floodlight activity group. This method supports
        patch semantics.
      operationId: dfareporting.floodlightActivityGroups.patch
      x-api-path-slug: userprofilesprofileidfloodlightactivitygroups-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Floodlight activity Group ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Floodlight Activity Group
    post:
      summary: Create Floodlight Activity Group
      description: Inserts a new floodlight activity group.
      operationId: dfareporting.floodlightActivityGroups.insert
      x-api-path-slug: userprofilesprofileidfloodlightactivitygroups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Floodlight Activity Group
    put:
      summary: Update Floodlight Activity Group
      description: Updates an existing floodlight activity group.
      operationId: dfareporting.floodlightActivityGroups.update
      x-api-path-slug: userprofilesprofileidfloodlightactivitygroups-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Floodlight Activity Group
  /userprofiles/{profileId}/floodlightActivityGroups/{id}:
    get:
      summary: Get Floodlight Activity Group
      description: Gets one floodlight activity group by ID.
      operationId: dfareporting.floodlightActivityGroups.get
      x-api-path-slug: userprofilesprofileidfloodlightactivitygroupsid-get
      parameters:
      - in: path
        name: id
        description: Floodlight activity Group ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Floodlight Activity Group
  /userprofiles/{profileId}/floodlightConfigurations:
    get:
      summary: Get Floodlight Configurations
      description: Retrieves a list of floodlight configurations, possibly filtered.
      operationId: dfareporting.floodlightConfigurations.list
      x-api-path-slug: userprofilesprofileidfloodlightconfigurations-get
      parameters:
      - in: query
        name: ids
        description: Set of IDs of floodlight configurations to retrieve
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Floodlight Activity Group
    patch:
      summary: Update Floodlight Configuration
      description: Updates an existing floodlight configuration. This method supports
        patch semantics.
      operationId: dfareporting.floodlightConfigurations.patch
      x-api-path-slug: userprofilesprofileidfloodlightconfigurations-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Floodlight configuration ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Floodlight
    put:
      summary: Update Floodlight Configuration
      description: Updates an existing floodlight configuration.
      operationId: dfareporting.floodlightConfigurations.update
      x-api-path-slug: userprofilesprofileidfloodlightconfigurations-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Floodlight
  /userprofiles/{profileId}/floodlightConfigurations/{id}:
    get:
      summary: Get Floodlight Configuration
      description: Gets one floodlight configuration by ID.
      operationId: dfareporting.floodlightConfigurations.get
      x-api-path-slug: userprofilesprofileidfloodlightconfigurationsid-get
      parameters:
      - in: path
        name: id
        description: Floodlight configuration ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Floodlight
  /userprofiles/{profileId}/languages:
    get:
      summary: Get Languages
      description: Retrieves a list of languages.
      operationId: dfareporting.languages.list
      x-api-path-slug: userprofilesprofileidlanguages-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Language
  /userprofiles/{profileId}/metros:
    get:
      summary: Get Metros
      description: Retrieves a list of metros.
      operationId: dfareporting.metros.list
      x-api-path-slug: userprofilesprofileidmetros-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Metro
  /userprofiles/{profileId}/mobileCarriers:
    get:
      summary: Get Mobile Carriers
      description: Retrieves a list of mobile carriers.
      operationId: dfareporting.mobileCarriers.list
      x-api-path-slug: userprofilesprofileidmobilecarriers-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Mobile Carrier
  /userprofiles/{profileId}/mobileCarriers/{id}:
    get:
      summary: Get Mobile Carrier
      description: Gets one mobile carrier by ID.
      operationId: dfareporting.mobileCarriers.get
      x-api-path-slug: userprofilesprofileidmobilecarriersid-get
      parameters:
      - in: path
        name: id
        description: Mobile carrier ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Mobile Carrier
  /userprofiles/{profileId}/operatingSystemVersions:
    get:
      summary: Get Operating System Versions
      description: Retrieves a list of operating system versions.
      operationId: dfareporting.operatingSystemVersions.list
      x-api-path-slug: userprofilesprofileidoperatingsystemversions-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Operating System
  /userprofiles/{profileId}/operatingSystemVersions/{id}:
    get:
      summary: Get Operating System Version
      description: Gets one operating system version by ID.
      operationId: dfareporting.operatingSystemVersions.get
      x-api-path-slug: userprofilesprofileidoperatingsystemversionsid-get
      parameters:
      - in: path
        name: id
        description: Operating system version ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Operating System
  /userprofiles/{profileId}/operatingSystems:
    get:
      summary: Get Operating Systems
      description: Retrieves a list of operating systems.
      operationId: dfareporting.operatingSystems.list
      x-api-path-slug: userprofilesprofileidoperatingsystems-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Operating System
  /userprofiles/{profileId}/operatingSystems/{dartId}:
    get:
      summary: Get Operating System
      description: Gets one operating system by DART ID.
      operationId: dfareporting.operatingSystems.get
      x-api-path-slug: userprofilesprofileidoperatingsystemsdartid-get
      parameters:
      - in: path
        name: dartId
        description: Operating system DART ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Operating System
  /userprofiles/{profileId}/placementGroups:
    get:
      summary: Get Placement Groups
      description: Retrieves a list of placement groups, possibly filtered. This method
        supports paging.
      operationId: dfareporting.placementGroups.list
      x-api-path-slug: userprofilesprofileidplacementgroups-get
      parameters:
      - in: query
        name: advertiserIds
        description: Select only placement groups that belong to these advertisers
      - in: query
        name: archived
        description: Select only archived placements
      - in: query
        name: campaignIds
        description: Select only placement groups that belong to these campaigns
      - in: query
        name: contentCategoryIds
        description: Select only placement groups that are associated with these content
          categories
      - in: query
        name: directorySiteIds
        description: Select only placement groups that are associated with these directory
          sites
      - in: query
        name: ids
        description: Select only placement groups with these IDs
      - in: query
        name: maxEndDate
        description: Select only placements or placement groups whose end date is
          on or before the specified maxEndDate
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: maxStartDate
        description: Select only placements or placement groups whose start date is
          on or before the specified maxStartDate
      - in: query
        name: minEndDate
        description: Select only placements or placement groups whose end date is
          on or after the specified minEndDate
      - in: query
        name: minStartDate
        description: Select only placements or placement groups whose start date is
          on or after the specified minStartDate
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: query
        name: placementGroupType
        description: Select only placement groups belonging with this group type
      - in: query
        name: placementStrategyIds
        description: Select only placement groups that are associated with these placement
          strategies
      - in: query
        name: pricingTypes
        description: Select only placement groups with these pricing types
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for placement groups by name or ID
      - in: query
        name: siteIds
        description: Select only placement groups that are associated with these sites
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement Group
    patch:
      summary: Update Placement Group
      description: Updates an existing placement group. This method supports patch
        semantics.
      operationId: dfareporting.placementGroups.patch
      x-api-path-slug: userprofilesprofileidplacementgroups-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Placement group ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement Group
    post:
      summary: Insert Placement Group
      description: Inserts a new placement group.
      operationId: dfareporting.placementGroups.insert
      x-api-path-slug: userprofilesprofileidplacementgroups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement Group
    put:
      summary: Update Placement Group
      description: Updates an existing placement group.
      operationId: dfareporting.placementGroups.update
      x-api-path-slug: userprofilesprofileidplacementgroups-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement Group
  /userprofiles/{profileId}/placementGroups/{id}:
    get:
      summary: Get Placement Group
      description: Gets one placement group by ID.
      operationId: dfareporting.placementGroups.get
      x-api-path-slug: userprofilesprofileidplacementgroupsid-get
      parameters:
      - in: path
        name: id
        description: Placement group ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement Group
  /userprofiles/{profileId}/placementStrategies:
    get:
      summary: Get Placement Strategies
      description: Retrieves a list of placement strategies, possibly filtered. This
        method supports paging.
      operationId: dfareporting.placementStrategies.list
      x-api-path-slug: userprofilesprofileidplacementstrategies-get
      parameters:
      - in: query
        name: ids
        description: Select only placement strategies with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement Strategy
    patch:
      summary: Update Placement Strategy
      description: Updates an existing placement strategy. This method supports patch
        semantics.
      operationId: dfareporting.placementStrategies.patch
      x-api-path-slug: userprofilesprofileidplacementstrategies-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Placement strategy ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement Strategy
    post:
      summary: Insert Placement Strategy
      description: Inserts a new placement strategy.
      operationId: dfareporting.placementStrategies.insert
      x-api-path-slug: userprofilesprofileidplacementstrategies-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement Strategy
    put:
      summary: Update Placement Strategy
      description: Updates an existing placement strategy.
      operationId: dfareporting.placementStrategies.update
      x-api-path-slug: userprofilesprofileidplacementstrategies-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement Strategy
  /userprofiles/{profileId}/placementStrategies/{id}:
    delete:
      summary: Delete Placement Strategy
      description: Deletes an existing placement strategy.
      operationId: dfareporting.placementStrategies.delete
      x-api-path-slug: userprofilesprofileidplacementstrategiesid-delete
      parameters:
      - in: path
        name: id
        description: Placement strategy ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement Strategy
    get:
      summary: Get Placement Strategy
      description: Gets one placement strategy by ID.
      operationId: dfareporting.placementStrategies.get
      x-api-path-slug: userprofilesprofileidplacementstrategiesid-get
      parameters:
      - in: path
        name: id
        description: Placement strategy ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement Strategy
  /userprofiles/{profileId}/placements:
    get:
      summary: Get Placements
      description: Retrieves a list of placements, possibly filtered. This method
        supports paging.
      operationId: dfareporting.placements.list
      x-api-path-slug: userprofilesprofileidplacements-get
      parameters:
      - in: query
        name: advertiserIds
        description: Select only placements that belong to these advertisers
      - in: query
        name: archived
        description: Select only archived placements
      - in: query
        name: campaignIds
        description: Select only placements that belong to these campaigns
      - in: query
        name: compatibilities
        description: Select only placements that are associated with these compatibilities
      - in: query
        name: contentCategoryIds
        description: Select only placements that are associated with these content
          categories
      - in: query
        name: directorySiteIds
        description: Select only placements that are associated with these directory
          sites
      - in: query
        name: groupIds
        description: Select only placements that belong to these placement groups
      - in: query
        name: ids
        description: Select only placements with these IDs
      - in: query
        name: maxEndDate
        description: Select only placements or placement groups whose end date is
          on or before the specified maxEndDate
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: maxStartDate
        description: Select only placements or placement groups whose start date is
          on or before the specified maxStartDate
      - in: query
        name: minEndDate
        description: Select only placements or placement groups whose end date is
          on or after the specified minEndDate
      - in: query
        name: minStartDate
        description: Select only placements or placement groups whose start date is
          on or after the specified minStartDate
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: query
        name: paymentSource
        description: Select only placements with this payment source
      - in: query
        name: placementStrategyIds
        description: Select only placements that are associated with these placement
          strategies
      - in: query
        name: pricingTypes
        description: Select only placements with these pricing types
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for placements by name or ID
      - in: query
        name: siteIds
        description: Select only placements that are associated with these sites
      - in: query
        name: sizeIds
        description: Select only placements that are associated with these sizes
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement
    patch:
      summary: Update Placement
      description: Updates an existing placement. This method supports patch semantics.
      operationId: dfareporting.placements.patch
      x-api-path-slug: userprofilesprofileidplacements-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Placement ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement
    post:
      summary: Insert Placement
      description: Inserts a new placement.
      operationId: dfareporting.placements.insert
      x-api-path-slug: userprofilesprofileidplacements-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement
    put:
      summary: Update Placement
      description: Updates an existing placement.
      operationId: dfareporting.placements.update
      x-api-path-slug: userprofilesprofileidplacements-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement
  /userprofiles/{profileId}/placements/generatetags:
    post:
      summary: Generate Placement Tag
      description: Generates tags for a placement.
      operationId: dfareporting.placements.generatetags
      x-api-path-slug: userprofilesprofileidplacementsgeneratetags-post
      parameters:
      - in: query
        name: campaignId
        description: Generate placements belonging to this campaign
      - in: query
        name: placementIds
        description: Generate tags for these placements
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: tagFormats
        description: Tag formats to generate for these placements
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement
  /userprofiles/{profileId}/placements/{id}:
    get:
      summary: Get Placement
      description: Gets one placement by ID.
      operationId: dfareporting.placements.get
      x-api-path-slug: userprofilesprofileidplacementsid-get
      parameters:
      - in: path
        name: id
        description: Placement ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement
  /userprofiles/{profileId}/platformTypes:
    get:
      summary: Get Platform Types
      description: Retrieves a list of platform types.
      operationId: dfareporting.platformTypes.list
      x-api-path-slug: userprofilesprofileidplatformtypes-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement Type
  /userprofiles/{profileId}/platformTypes/{id}:
    get:
      summary: Get Platform Type
      description: Gets one platform type by ID.
      operationId: dfareporting.platformTypes.get
      x-api-path-slug: userprofilesprofileidplatformtypesid-get
      parameters:
      - in: path
        name: id
        description: Platform type ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Placement Type
  /userprofiles/{profileId}/postalCodes:
    get:
      summary: Get Postal Codes
      description: Retrieves a list of postal codes.
      operationId: dfareporting.postalCodes.list
      x-api-path-slug: userprofilesprofileidpostalcodes-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Postal Code
  /userprofiles/{profileId}/postalCodes/{code}:
    get:
      summary: Get Postal Code
      description: Gets one postal code by ID.
      operationId: dfareporting.postalCodes.get
      x-api-path-slug: userprofilesprofileidpostalcodescode-get
      parameters:
      - in: path
        name: code
        description: Postal code ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Postal Code
  /userprofiles/{profileId}/projects:
    get:
      summary: Get Projects
      description: Retrieves a list of projects, possibly filtered. This method supports
        paging.
      operationId: dfareporting.projects.list
      x-api-path-slug: userprofilesprofileidprojects-get
      parameters:
      - in: query
        name: advertiserIds
        description: Select only projects with these advertiser IDs
      - in: query
        name: ids
        description: Select only projects with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for projects by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Project
  /userprofiles/{profileId}/projects/{id}:
    get:
      summary: Get Project
      description: Gets one project by ID.
      operationId: dfareporting.projects.get
      x-api-path-slug: userprofilesprofileidprojectsid-get
      parameters:
      - in: path
        name: id
        description: Project ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Project
  /userprofiles/{profileId}/projects/{projectId}/inventoryItems:
    get:
      summary: Get Inventory Items
      description: Retrieves a list of inventory items, possibly filtered. This method
        supports paging.
      operationId: dfareporting.inventoryItems.list
      x-api-path-slug: userprofilesprofileidprojectsprojectidinventoryitems-get
      parameters:
      - in: query
        name: ids
        description: Select only inventory items with these IDs
      - in: query
        name: inPlan
        description: Select only inventory items that are in plan
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: orderId
        description: Select only inventory items that belong to specified orders
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: path
        name: projectId
        description: Project ID for order documents
      - in: query
        name: siteId
        description: Select only inventory items that are associated with these sites
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      - in: query
        name: type
        description: Select only inventory items with this type
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Inventory Item
  /userprofiles/{profileId}/projects/{projectId}/inventoryItems/{id}:
    get:
      summary: Get Inventory Item
      description: Gets one inventory item by ID.
      operationId: dfareporting.inventoryItems.get
      x-api-path-slug: userprofilesprofileidprojectsprojectidinventoryitemsid-get
      parameters:
      - in: path
        name: id
        description: Inventory item ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: path
        name: projectId
        description: Project ID for order documents
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Inventory Item
  /userprofiles/{profileId}/projects/{projectId}/orderDocuments:
    get:
      summary: Get Order Documents
      description: Retrieves a list of order documents, possibly filtered. This method
        supports paging.
      operationId: dfareporting.orderDocuments.list
      x-api-path-slug: userprofilesprofileidprojectsprojectidorderdocuments-get
      parameters:
      - in: query
        name: approved
        description: Select only order documents that have been approved by at least
          one user
      - in: query
        name: ids
        description: Select only order documents with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: orderId
        description: Select only order documents for specified orders
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: path
        name: projectId
        description: Project ID for order documents
      - in: query
        name: searchString
        description: Allows searching for order documents by name or ID
      - in: query
        name: siteId
        description: Select only order documents that are associated with these sites
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Order Document
  /userprofiles/{profileId}/projects/{projectId}/orderDocuments/{id}:
    get:
      summary: Get Order Document
      description: Gets one order document by ID.
      operationId: dfareporting.orderDocuments.get
      x-api-path-slug: userprofilesprofileidprojectsprojectidorderdocumentsid-get
      parameters:
      - in: path
        name: id
        description: Order document ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: path
        name: projectId
        description: Project ID for order documents
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Order Document
  /userprofiles/{profileId}/projects/{projectId}/orders:
    get:
      summary: Get Orders
      description: Retrieves a list of orders, possibly filtered. This method supports
        paging.
      operationId: dfareporting.orders.list
      x-api-path-slug: userprofilesprofileidprojectsprojectidorders-get
      parameters:
      - in: query
        name: ids
        description: Select only orders with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: path
        name: projectId
        description: Project ID for orders
      - in: query
        name: searchString
        description: Allows searching for orders by name or ID
      - in: query
        name: siteId
        description: Select only orders that are associated with these site IDs
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Order
  /userprofiles/{profileId}/projects/{projectId}/orders/{id}:
    get:
      summary: Get Order
      description: Gets one order by ID.
      operationId: dfareporting.orders.get
      x-api-path-slug: userprofilesprofileidprojectsprojectidordersid-get
      parameters:
      - in: path
        name: id
        description: Order ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: path
        name: projectId
        description: Project ID for orders
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Order
  /userprofiles/{profileId}/regions:
    get:
      summary: Get Regions
      description: Retrieves a list of regions.
      operationId: dfareporting.regions.list
      x-api-path-slug: userprofilesprofileidregions-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Region
  /userprofiles/{profileId}/remarketingListShares:
    patch:
      summary: Update Remarketing List Shares
      description: Updates an existing remarketing list share. This method supports
        patch semantics.
      operationId: dfareporting.remarketingListShares.patch
      x-api-path-slug: userprofilesprofileidremarketinglistshares-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: remarketingListId
        description: Remarketing list ID
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Remarketing List
    put:
      summary: Update Remarketing List Shares
      description: Updates an existing remarketing list share.
      operationId: dfareporting.remarketingListShares.update
      x-api-path-slug: userprofilesprofileidremarketinglistshares-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Remarketing List
  /userprofiles/{profileId}/remarketingListShares/{remarketingListId}:
    get:
      summary: Get Remarketing List Shares
      description: Gets one remarketing list share by remarketing list ID.
      operationId: dfareporting.remarketingListShares.get
      x-api-path-slug: userprofilesprofileidremarketinglistsharesremarketinglistid-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: path
        name: remarketingListId
        description: Remarketing list ID
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Remarketing List
  /userprofiles/{profileId}/remarketingLists:
    get:
      summary: Get Remarketing Lists
      description: Retrieves a list of remarketing lists, possibly filtered. This
        method supports paging.
      operationId: dfareporting.remarketingLists.list
      x-api-path-slug: userprofilesprofileidremarketinglists-get
      parameters:
      - in: query
        name: active
        description: Select only active or only inactive remarketing lists
      - in: query
        name: advertiserId
        description: Select only remarketing lists owned by this advertiser
      - in: query
        name: floodlightActivityId
        description: Select only remarketing lists that have this floodlight activity
          ID
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: name
        description: Allows searching for objects by name or ID
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Remarketing List
    patch:
      summary: Update Remarketing List
      description: Updates an existing remarketing list. This method supports patch
        semantics.
      operationId: dfareporting.remarketingLists.patch
      x-api-path-slug: userprofilesprofileidremarketinglists-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Remarketing list ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Remarketing List
    post:
      summary: Insert Remarketing List
      description: Inserts a new remarketing list.
      operationId: dfareporting.remarketingLists.insert
      x-api-path-slug: userprofilesprofileidremarketinglists-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Remarketing List
    put:
      summary: Update Remarketing List
      description: Updates an existing remarketing list.
      operationId: dfareporting.remarketingLists.update
      x-api-path-slug: userprofilesprofileidremarketinglists-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Remarketing List
  /userprofiles/{profileId}/remarketingLists/{id}:
    get:
      summary: Get Remarketing List
      description: Gets one remarketing list by ID.
      operationId: dfareporting.remarketingLists.get
      x-api-path-slug: userprofilesprofileidremarketinglistsid-get
      parameters:
      - in: path
        name: id
        description: Remarketing list ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Remarketing List
  /userprofiles/{profileId}/reports:
    get:
      summary: Get Reports
      description: Retrieves list of reports.
      operationId: dfareporting.reports.list
      x-api-path-slug: userprofilesprofileidreports-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous result page
      - in: path
        name: profileId
        description: The DFA user profile ID
      - in: query
        name: scope
        description: The scope that defines which results are returned, default is
          MINE
      - in: query
        name: sortField
        description: The field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is DESCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
    post:
      summary: Get Report
      description: Creates a report.
      operationId: dfareporting.reports.insert
      x-api-path-slug: userprofilesprofileidreports-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: The DFA user profile ID
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /userprofiles/{profileId}/reports/compatiblefields/query:
    post:
      summary: Return Compatible Fields
      description: Returns the fields that are compatible to be selected in the respective
        sections of a report criteria, given the fields already selected in the input
        report and user permissions.
      operationId: dfareporting.reports.compatibleFields.query
      x-api-path-slug: userprofilesprofileidreportscompatiblefieldsquery-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: The DFA user profile ID
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Field
  /userprofiles/{profileId}/reports/{reportId}:
    delete:
      summary: Delete Report
      description: Deletes a report by its ID.
      operationId: dfareporting.reports.delete
      x-api-path-slug: userprofilesprofileidreportsreportid-delete
      parameters:
      - in: path
        name: profileId
        description: The DFA user profile ID
      - in: path
        name: reportId
        description: The ID of the report
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
    get:
      summary: Get Report
      description: Retrieves a report by its ID.
      operationId: dfareporting.reports.get
      x-api-path-slug: userprofilesprofileidreportsreportid-get
      parameters:
      - in: path
        name: profileId
        description: The DFA user profile ID
      - in: path
        name: reportId
        description: The ID of the report
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
    patch:
      summary: Update Report
      description: Updates a report. This method supports patch semantics.
      operationId: dfareporting.reports.patch
      x-api-path-slug: userprofilesprofileidreportsreportid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: The DFA user profile ID
      - in: path
        name: reportId
        description: The ID of the report
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
    put:
      summary: Update Report
      description: Updates a report.
      operationId: dfareporting.reports.update
      x-api-path-slug: userprofilesprofileidreportsreportid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: The DFA user profile ID
      - in: path
        name: reportId
        description: The ID of the report
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /userprofiles/{profileId}/reports/{reportId}/files:
    get:
      summary: Get Report Files
      description: Lists files for a report.
      operationId: dfareporting.reports.files.list
      x-api-path-slug: userprofilesprofileidreportsreportidfiles-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous result page
      - in: path
        name: profileId
        description: The DFA profile ID
      - in: path
        name: reportId
        description: The ID of the parent report
      - in: query
        name: sortField
        description: The field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is DESCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report File
  /userprofiles/{profileId}/reports/{reportId}/files/{fileId}:
    get:
      summary: Get Report File
      description: Retrieves a report file.
      operationId: dfareporting.reports.files.get
      x-api-path-slug: userprofilesprofileidreportsreportidfilesfileid-get
      parameters:
      - in: path
        name: fileId
        description: The ID of the report file
      - in: path
        name: profileId
        description: The DFA profile ID
      - in: path
        name: reportId
        description: The ID of the report
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report File
  /userprofiles/{profileId}/reports/{reportId}/run:
    post:
      summary: Run Report
      description: Runs a report.
      operationId: dfareporting.reports.run
      x-api-path-slug: userprofilesprofileidreportsreportidrun-post
      parameters:
      - in: path
        name: profileId
        description: The DFA profile ID
      - in: path
        name: reportId
        description: The ID of the report
      - in: query
        name: synchronous
        description: If set and true, tries to run the report synchronously
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /userprofiles/{profileId}/sites:
    get:
      summary: Get Sites
      description: Retrieves a list of sites, possibly filtered. This method supports
        paging.
      operationId: dfareporting.sites.list
      x-api-path-slug: userprofilesprofileidsites-get
      parameters:
      - in: query
        name: acceptsInStreamVideoPlacements
        description: This search filter is no longer supported and will have no effect
          on the results returned
      - in: query
        name: acceptsInterstitialPlacements
        description: This search filter is no longer supported and will have no effect
          on the results returned
      - in: query
        name: acceptsPublisherPaidPlacements
        description: Select only sites that accept publisher paid placements
      - in: query
        name: adWordsSite
        description: Select only AdWords sites
      - in: query
        name: approved
        description: Select only approved sites
      - in: query
        name: campaignIds
        description: Select only sites with these campaign IDs
      - in: query
        name: directorySiteIds
        description: Select only sites with these directory site IDs
      - in: query
        name: ids
        description: Select only sites with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name, ID or keyName
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      - in: query
        name: subaccountId
        description: Select only sites with this subaccount ID
      - in: query
        name: unmappedSite
        description: Select only sites that have not been mapped to a directory site
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Site
    patch:
      summary: Update Site
      description: Updates an existing site. This method supports patch semantics.
      operationId: dfareporting.sites.patch
      x-api-path-slug: userprofilesprofileidsites-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Site ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Site
    post:
      summary: Create Site
      description: Inserts a new site.
      operationId: dfareporting.sites.insert
      x-api-path-slug: userprofilesprofileidsites-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Site
    put:
      summary: Update Site
      description: Updates an existing site.
      operationId: dfareporting.sites.update
      x-api-path-slug: userprofilesprofileidsites-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Site
  /userprofiles/{profileId}/sites/{id}:
    get:
      summary: Get Site
      description: Gets one site by ID.
      operationId: dfareporting.sites.get
      x-api-path-slug: userprofilesprofileidsitesid-get
      parameters:
      - in: path
        name: id
        description: Site ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Site
  /userprofiles/{profileId}/sizes:
    get:
      summary: Get Sizes
      description: Retrieves a list of sizes, possibly filtered.
      operationId: dfareporting.sizes.list
      x-api-path-slug: userprofilesprofileidsizes-get
      parameters:
      - in: query
        name: height
        description: Select only sizes with this height
      - in: query
        name: iabStandard
        description: Select only IAB standard sizes
      - in: query
        name: ids
        description: Select only sizes with these IDs
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: width
        description: Select only sizes with this width
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Size
    post:
      summary: Insert Size
      description: Inserts a new size.
      operationId: dfareporting.sizes.insert
      x-api-path-slug: userprofilesprofileidsizes-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Size
  /userprofiles/{profileId}/sizes/{id}:
    get:
      summary: Get Size
      description: Gets one size by ID.
      operationId: dfareporting.sizes.get
      x-api-path-slug: userprofilesprofileidsizesid-get
      parameters:
      - in: path
        name: id
        description: Size ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Size
  /userprofiles/{profileId}/subaccounts:
    get:
      summary: Get Subaccounts
      description: Gets a list of subaccounts, possibly filtered. This method supports
        paging.
      operationId: dfareporting.subaccounts.list
      x-api-path-slug: userprofilesprofileidsubaccounts-get
      parameters:
      - in: query
        name: ids
        description: Select only subaccounts with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Subaccount
    patch:
      summary: Update Subaccount
      description: Updates an existing subaccount. This method supports patch semantics.
      operationId: dfareporting.subaccounts.patch
      x-api-path-slug: userprofilesprofileidsubaccounts-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Subaccount ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Subaccount
    post:
      summary: Insert Subaccount
      description: Inserts a new subaccount.
      operationId: dfareporting.subaccounts.insert
      x-api-path-slug: userprofilesprofileidsubaccounts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Subaccount
    put:
      summary: Update Subaccount
      description: Updates an existing subaccount.
      operationId: dfareporting.subaccounts.update
      x-api-path-slug: userprofilesprofileidsubaccounts-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Subaccount
  /userprofiles/{profileId}/subaccounts/{id}:
    get:
      summary: Get Subaccount
      description: Gets one subaccount by ID.
      operationId: dfareporting.subaccounts.get
      x-api-path-slug: userprofilesprofileidsubaccountsid-get
      parameters:
      - in: path
        name: id
        description: Subaccount ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Subaccount
  /userprofiles/{profileId}/targetableRemarketingLists:
    get:
      summary: Get Targetable Remarketing Lists
      description: Retrieves a list of targetable remarketing lists, possibly filtered.
        This method supports paging.
      operationId: dfareporting.targetableRemarketingLists.list
      x-api-path-slug: userprofilesprofileidtargetableremarketinglists-get
      parameters:
      - in: query
        name: active
        description: Select only active or only inactive targetable remarketing lists
      - in: query
        name: advertiserId
        description: Select only targetable remarketing lists targetable by these
          advertisers
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: name
        description: Allows searching for objects by name or ID
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Remarketing List
  /userprofiles/{profileId}/targetableRemarketingLists/{id}:
    get:
      summary: Get Targetable Remarketing List
      description: Gets one remarketing list by ID.
      operationId: dfareporting.targetableRemarketingLists.get
      x-api-path-slug: userprofilesprofileidtargetableremarketinglistsid-get
      parameters:
      - in: path
        name: id
        description: Remarketing list ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Remarketing List
  /userprofiles/{profileId}/targetingTemplates:
    get:
      summary: Get Targeting Templates
      description: Retrieves a list of targeting templates, optionally filtered. This
        method supports paging.
      operationId: dfareporting.targetingTemplates.list
      x-api-path-slug: userprofilesprofileidtargetingtemplates-get
      parameters:
      - in: query
        name: advertiserId
        description: Select only targeting templates with this advertiser ID
      - in: query
        name: ids
        description: Select only targeting templates with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Targeting Template
    patch:
      summary: Update Targeting Template
      description: Updates an existing targeting template. This method supports patch
        semantics.
      operationId: dfareporting.targetingTemplates.patch
      x-api-path-slug: userprofilesprofileidtargetingtemplates-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Targeting template ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Targeting Template
    post:
      summary: Create Targeting Template
      description: Inserts a new targeting template.
      operationId: dfareporting.targetingTemplates.insert
      x-api-path-slug: userprofilesprofileidtargetingtemplates-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Targeting Template
    put:
      summary: Update Targeting Template
      description: Updates an existing targeting template.
      operationId: dfareporting.targetingTemplates.update
      x-api-path-slug: userprofilesprofileidtargetingtemplates-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Targeting Template
  /userprofiles/{profileId}/targetingTemplates/{id}:
    get:
      summary: Get Targeting Template
      description: Gets one targeting template by ID.
      operationId: dfareporting.targetingTemplates.get
      x-api-path-slug: userprofilesprofileidtargetingtemplatesid-get
      parameters:
      - in: path
        name: id
        description: Targeting template ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Targeting Template
  /userprofiles/{profileId}/userRolePermissionGroups:
    get:
      summary: Get User Role Permission Groups
      description: Gets a list of all supported user role permission groups.
      operationId: dfareporting.userRolePermissionGroups.list
      x-api-path-slug: userprofilesprofileiduserrolepermissiongroups-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Users
      - Roles
      - Permissions Group
  /userprofiles/{profileId}/userRolePermissionGroups/{id}:
    get:
      summary: Get User Role Permission Group
      description: Gets one user role permission group by ID.
      operationId: dfareporting.userRolePermissionGroups.get
      x-api-path-slug: userprofilesprofileiduserrolepermissiongroupsid-get
      parameters:
      - in: path
        name: id
        description: User role permission group ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Users
      - Roles
      - Permissions Group
  /userprofiles/{profileId}/userRolePermissions:
    get:
      summary: Get User Role Permissions
      description: Gets a list of user role permissions, possibly filtered.
      operationId: dfareporting.userRolePermissions.list
      x-api-path-slug: userprofilesprofileiduserrolepermissions-get
      parameters:
      - in: query
        name: ids
        description: Select only user role permissions with these IDs
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Users
      - Roles
      - Permissions
  /userprofiles/{profileId}/userRolePermissions/{id}:
    get:
      summary: Get User Role Permission
      description: Gets one user role permission by ID.
      operationId: dfareporting.userRolePermissions.get
      x-api-path-slug: userprofilesprofileiduserrolepermissionsid-get
      parameters:
      - in: path
        name: id
        description: User role permission ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Users
      - Roles
      - Permissions
  /userprofiles/{profileId}/userRoles:
    get:
      summary: Get User Roles
      description: Retrieves a list of user roles, possibly filtered. This method
        supports paging.
      operationId: dfareporting.userRoles.list
      x-api-path-slug: userprofilesprofileiduserroles-get
      parameters:
      - in: query
        name: accountUserRoleOnly
        description: Select only account level user roles not associated with any
          specific subaccount
      - in: query
        name: ids
        description: Select only user roles with the specified IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      - in: query
        name: subaccountId
        description: Select only user roles that belong to this subaccount
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Users
      - Roles
    patch:
      summary: Update User Role
      description: Updates an existing user role. This method supports patch semantics.
      operationId: dfareporting.userRoles.patch
      x-api-path-slug: userprofilesprofileiduserroles-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: User role ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Users
      - Roles
    post:
      summary: Insert User Role
      description: Inserts a new user role.
      operationId: dfareporting.userRoles.insert
      x-api-path-slug: userprofilesprofileiduserroles-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Users
      - Roles
    put:
      summary: Update User Role
      description: Updates an existing user role.
      operationId: dfareporting.userRoles.update
      x-api-path-slug: userprofilesprofileiduserroles-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Users
      - Roles
  /userprofiles/{profileId}/userRoles/{id}:
    delete:
      summary: Delete User Role
      description: Deletes an existing user role.
      operationId: dfareporting.userRoles.delete
      x-api-path-slug: userprofilesprofileiduserrolesid-delete
      parameters:
      - in: path
        name: id
        description: User role ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Users
      - Roles
    get:
      summary: Get User Role
      description: Gets one user role by ID.
      operationId: dfareporting.userRoles.get
      x-api-path-slug: userprofilesprofileiduserrolesid-get
      parameters:
      - in: path
        name: id
        description: User role ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Users
      - Roles
  /userprofiles/{profileId}/videoFormats:
    get:
      summary: Get Video Formats
      description: Lists available video formats.
      operationId: dfareporting.videoFormats.list
      x-api-path-slug: userprofilesprofileidvideoformats-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Video
  /userprofiles/{profileId}/videoFormats/{id}:
    get:
      summary: Get Video
      description: Gets one video format by ID.
      operationId: dfareporting.videoFormats.get
      x-api-path-slug: userprofilesprofileidvideoformatsid-get
      parameters:
      - in: path
        name: id
        description: Video format ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Video
  /lineitems/downloadlineitems:
    post:
      summary: Download CSV
      description: Retrieves line items in CSV format.
      operationId: doubleclickbidmanager.lineitems.downloadlineitems
      x-api-path-slug: lineitemsdownloadlineitems-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - CSV
  /lineitems/uploadlineitems:
    post:
      summary: Upload CSV
      description: Uploads line items in CSV format.
      operationId: doubleclickbidmanager.lineitems.uploadlineitems
      x-api-path-slug: lineitemsuploadlineitems-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - CSV
  /queries:
    get:
      summary: Get Stored Queries
      description: Retrieves stored queries.
      operationId: doubleclickbidmanager.queries.listqueries
      x-api-path-slug: queries-get
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Query
  /queries/{queryId}/reports:
    get:
      summary: Get Stored Reports
      description: Retrieves stored reports.
      operationId: doubleclickbidmanager.reports.listreports
      x-api-path-slug: queriesqueryidreports-get
      parameters:
      - in: path
        name: queryId
        description: Query ID with which the reports are associated
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Query
  /query:
    post:
      summary: Create Query
      description: Creates a query.
      operationId: doubleclickbidmanager.queries.createquery
      x-api-path-slug: query-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Query
  /query/{queryId}:
    delete:
      summary: Delete Stored Query
      description: Deletes a stored query as well as the associated stored reports.
      operationId: doubleclickbidmanager.queries.deletequery
      x-api-path-slug: queryqueryid-delete
      parameters:
      - in: path
        name: queryId
        description: Query ID to delete
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Query
    get:
      summary: Get Stored Query
      description: Retrieves a stored query.
      operationId: doubleclickbidmanager.queries.getquery
      x-api-path-slug: queryqueryid-get
      parameters:
      - in: path
        name: queryId
        description: Query ID to retrieve
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Query
    post:
      summary: Run Stored Query
      description: Runs a stored query to generate a report.
      operationId: doubleclickbidmanager.queries.runquery
      x-api-path-slug: queryqueryid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: queryId
        description: Query ID to run
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Query
  /sdf/download:
    post:
      summary: Get Entities in SDF Format
      description: Retrieves entities in SDF format.
      operationId: doubleclickbidmanager.sdf.download
      x-api-path-slug: sdfdownload-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - SDF
  /agency/{agencyId}/advertiser/{advertiserId}/engine/{engineAccountId}/conversion:
    get:
      summary: Get Conversions
      description: Retrieves a list of conversions from a DoubleClick Search engine
        account.
      operationId: doubleclicksearch.conversion.get
      x-api-path-slug: agencyagencyidadvertiseradvertiseridengineengineaccountidconversion-get
      parameters:
      - in: query
        name: adGroupId
        description: Numeric ID of the ad group
      - in: query
        name: adId
        description: Numeric ID of the ad
      - in: path
        name: advertiserId
        description: Numeric ID of the advertiser
      - in: path
        name: agencyId
        description: Numeric ID of the agency
      - in: query
        name: campaignId
        description: Numeric ID of the campaign
      - in: query
        name: criterionId
        description: Numeric ID of the criterion
      - in: query
        name: endDate
        description: Last date (inclusive) on which to retrieve conversions
      - in: path
        name: engineAccountId
        description: Numeric ID of the engine account
      - in: query
        name: rowCount
        description: The number of conversions to return per call
      - in: query
        name: startDate
        description: First date (inclusive) on which to retrieve conversions
      - in: query
        name: startRow
        description: The 0-based starting index for retrieving conversions results
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Conversion
  /agency/{agencyId}/advertiser/{advertiserId}/savedcolumns:
    get:
      summary: Get Saved Columns
      description: Retrieve the list of saved columns for a specified advertiser.
      operationId: doubleclicksearch.savedColumns.list
      x-api-path-slug: agencyagencyidadvertiseradvertiseridsavedcolumns-get
      parameters:
      - in: path
        name: advertiserId
        description: DS ID of the advertiser
      - in: path
        name: agencyId
        description: DS ID of the agency
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Colum
  /conversion:
    patch:
      summary: Update Conversions
      description: Updates a batch of conversions in DoubleClick Search. This method
        supports patch semantics.
      operationId: doubleclicksearch.conversion.patch
      x-api-path-slug: conversion-patch
      parameters:
      - in: query
        name: advertiserId
        description: Numeric ID of the advertiser
      - in: query
        name: agencyId
        description: Numeric ID of the agency
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: endDate
        description: Last date (inclusive) on which to retrieve conversions
      - in: query
        name: engineAccountId
        description: Numeric ID of the engine account
      - in: query
        name: rowCount
        description: The number of conversions to return per call
      - in: query
        name: startDate
        description: First date (inclusive) on which to retrieve conversions
      - in: query
        name: startRow
        description: The 0-based starting index for retrieving conversions results
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Conversion
    post:
      summary: Insert Conversion
      description: Inserts a batch of new conversions into DoubleClick Search.
      operationId: doubleclicksearch.conversion.insert
      x-api-path-slug: conversion-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Conversion
    put:
      summary: Update Conversions
      description: Updates a batch of conversions in DoubleClick Search.
      operationId: doubleclicksearch.conversion.update
      x-api-path-slug: conversion-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Conversion
  /conversion/updateAvailability:
    post:
      summary: Update Availability
      description: Updates the availabilities of a batch of floodlight activities
        in DoubleClick Search.
      operationId: doubleclicksearch.conversion.updateAvailability
      x-api-path-slug: conversionupdateavailability-post
      parameters:
      - in: body
        name: empty
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Conversion
  /reports:
    post:
      summary: Insert Report
      description: Inserts a report request into the reporting system.
      operationId: doubleclicksearch.reports.request
      x-api-path-slug: reports-post
      parameters:
      - in: body
        name: reportRequest
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /reports/generate:
    post:
      summary: Generate Report
      description: Generates and returns a report immediately.
      operationId: doubleclicksearch.reports.generate
      x-api-path-slug: reportsgenerate-post
      parameters:
      - in: body
        name: reportRequest
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /reports/{reportId}:
    get:
      summary: Get Report Status
      description: Polls for the status of a report request.
      operationId: doubleclicksearch.reports.get
      x-api-path-slug: reportsreportid-get
      parameters:
      - in: path
        name: reportId
        description: ID of the report request being polled
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /reports/{reportId}/files/{reportFragment}:
    get:
      summary: Download Report
      description: Downloads a report file encoded in UTF-8.
      operationId: doubleclicksearch.reports.getFile
      x-api-path-slug: reportsreportidfilesreportfragment-get
      parameters:
      - in: path
        name: reportFragment
        description: The index of the report fragment to download
      - in: path
        name: reportId
        description: ID of the report
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report