swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 1
info:
  title: ChainGenie = DLT + Blockchain + Magic
  description: chaingenie-is-here-to-help-companies-enjoy-the-benefits-of-blockchain-technology-distributed-tamper-proof-record-keeping-consensus-between-distrusting-nodes-when-you-do-not-have-the-expensive-blockchain-resources-chaingenie-offers-a-hook-to-connect-your-existing-it-applications-to-popular-blockchain-networks-like-ethereum-bitcoin-blockchain-etc-with-great-ease---want-to-know-how-chaingenie-works-under-the-hood-download-our-flyer--httpchaingenie-comchaingenieflyer-pdfthe-following-is-only-teaser-documentation--for-full-information-email--a-hrefmailtomagicchaingenie-commagicchaingenie-comahrupdate-09262016-brullibanking-micro-services-addedliliapikey-is-required-for-invoking-any-micro-serviceliulemail-a-hrefmailtomagicchaingenie-commagicchaingenie-coma-for-your-sandbox-apikey-hrcoming-soon-brmagic-canvas--drag-and-drop-microservices-to-create-a-blockchain-application---iblockchain-made-easyihrwant-to-connect-with-me-on-linkedin-send-me-an-invite--a-hrefhttplinkedin-cominupriya-target-blankhttplinkedin-cominupriyaahrscript----function-i-s-o-g-r-a-m---------igoogleanalyticsobject--r-ir--ir--function--------------ir-q--ir-q---pusharguments---------ir-l--1--new-date-a--s-createelemento--m--s-getelementsbytagnameo0-a-async--1-a-src--g-m-parentnode-insertbeforea-m----window-document-script-httpswww-googleanalytics-comanalytics-js-ga----gacreate-ua825523031-auto----gasend-pageviewscript
  version: "1.0"
host: api.chaingenie.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ethbank/deposit:
    post:
      summary: Deposit into bank account
      description: Deposit crypto currency into the bank.  In sandbox mode, the account
        used is the demo account on the blockchain server.
      operationId: EthbankDepositPost
      x-api-path-slug: ethbankdeposit-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: value
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Deposit
      - Into
      - Bank
      - Account
  /ethbank/withdraw:
    post:
      summary: Withdraw from bank account
      description: Withdraw crypto currency into the bank.  In sandbox mode, the account
        used is the demo account on the blockchain server. Of course, you can only
        withdraw if there is money in the account!
      operationId: EthbankWithdrawPost
      x-api-path-slug: ethbankwithdraw-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: value
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Withdraw
      - From
      - Bank
      - Account
  /ethbank/passbook:
    get:
      summary: Bank passbook (user)
      description: Displays all transactions made by the user
      operationId: EthbankPassbookGet
      x-api-path-slug: ethbankpassbook-get
      parameters:
      - in: header
        name: ApiKey
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Bank
      - Passbook
      - (user)
  /ethbank/balance:
    get:
      summary: Bank balance (user)
      description: Displays user bank balance information
      operationId: EthbankBalanceGet
      x-api-path-slug: ethbankbalance-get
      parameters:
      - in: header
        name: ApiKey
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Bank
      - Balance
      - (user)
  /ethledger/invokecontract:
    post:
      summary: Generate, Sign & Route Document (Advanced)
      description: "This API is the generic version of the \"Generate document from
        template\" API. Any template file can be uploaded (sample available as link
        for testing).  If you just want to see how this would work - use the other
        call and just run it without any uploaded certificate. \nUpload a templated
        pdf with editable / filable fields and generate a document with automated
        sign and routing to a recipient.  Every attribute that needs to be filled
        will need to be passed in the format - ex. course field to be substituted
        - field = attrib; value = [\"course\",\"course value\"] or date field to be
        substituted - field = attrib; value = [\"date\",\"12/12/2016\"].  If your
        fillable form has the field named \"today\", current time will be used for
        filling the value of that field.\nYou will need to upload for the file attribute
        a real template file with fillable fields. For the sample values as configured,
        you can use the demo template available at http://chaingenie.com/cert.pdf.
        \ Download this certificate and add it as your input file\nTo route the document
        to recipient (optional) add field recipient with \"key\" of the recipient
        - available recipient in the system - 0xb3A214341df9560a3e09E256BfacefD6648f5Ca9
        for your testing\nUse case - Upload an invoice template with fillable fields,
        add attrib values for all the fields that needs to be filled, add the recipient
        field - your invoice will be created, signed with your key (in production
        / in test it will be signed with the local admin key) and will be routed to
        the recipient (in production you can add your recipient / in sandbox - use
        recipient 0xb3A214341df9560a3e09E256BfacefD6648f5Ca9)\nResponse will contain
        the document name, signatories, timestamps, recipient, IPFS hash (handle to
        retrieve the actual document)\nThe document hash will be posted on blockchain
        and the actual document will be added to IPFS.  Want to retrieve your document?
        Check out the API - Write & Retrieve - Docs (IPFS)."
      operationId: EthledgerInvokecontractPost
      x-api-path-slug: ethledgerinvokecontract-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: attribs
      - in: formData
        name: file
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Generate
      - ""
      - Sign
      - '&'
      - Route
      - Document
      - (Advanced)
  /ethledger/docert:
    post:
      summary: Generate and Manage Document (Basic)
      description: "This is an over simplified version for testing this API for its
        powers a template - uses an inbuilt into ChainGenie template and values are
        preconfigured - just running this will work and provide you an IPFS handle
        to retrieve the document you generated with your variables / values from the
        template.\nUse an existing document on our server and generate a document
        with automated sign and routing to a recipient.  Ex. this configured api will
        generate a certificate for a student name (name) with the completed certificate
        course (course) and dated (date). \nThe document hash will be posted on blockchain
        and the actual document will be added to IPFS.  Want to retrieve your document?
        Check out the API - Write & Retrieve - Docs (IPFS)."
      operationId: EthledgerDocertPost2
      x-api-path-slug: ethledgerdocert-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: course
      - in: formData
        name: date
      - in: formData
        name: students
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Generate
      - Manage
      - Document
      - (Basic)
  /ethledger/sendforsign:
    post:
      summary: Send document
      description: Route the document for signature.  The document history and status
        is updated for querying.
      operationId: EthledgerSendforsignPost
      x-api-path-slug: ethledgersendforsign-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: files
      - in: formData
        name: recipient
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Send
      - Document
  /ethledger/sign:
    post:
      summary: Sign document
      description: Cryptographically sign the document and add the record to blockchain.  The
        document history and status is updated for querying.
      operationId: EthledgerSignPost
      x-api-path-slug: ethledgersign-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: files
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Sign
      - Document
  /ethledger/docstatus:
    post:
      summary: Get document status with file
      description: Review the document status - existence, hash, block info, signatories,
        routing to users and details
      operationId: EthledgerDocstatusPost
      x-api-path-slug: ethledgerdocstatus-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: files
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Document
      - Status
      - File
  /ethledger/existsdoc:
    post:
      summary: Check document exists on blockchain
      description: Check if your documents exists in the eth blockchain
      operationId: EthledgerExistsdocPost
      x-api-path-slug: ethledgerexistsdoc-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: files
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Check
      - Document
      - Exists
      - "On"
      - Blockchain
  /ethledger/postdoc:
    post:
      summary: Post document to IPFS + blockchain
      description: Post document hash into eth chain for POE (proof of existence)
        and post the document into ipfs for safekeep!
      operationId: EthledgerPostdocPost
      x-api-path-slug: ethledgerpostdoc-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: files
      - in: formData
        name: filetypes
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Document
      - To
      - IPFS
      - +
      - Blockchain
  /ethledger/sendcert:
    post:
      summary: Send document using hash (min fn; no return)
      description: Route the document to a recipient.  The document history and status
        is updated for querying.  The API call does not return any document properties.  This
        is a <b>minimalistic function</b> for stringing with other functions
      operationId: EthledgerSendcertPost
      x-api-path-slug: ethledgersendcert-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: recipient
      - in: formData
        name: strHash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Send
      - Document
      - Using
      - Hash
      - (min
      - Fn;
      - "No"
      - Return)
  /ethledger/signcert:
    post:
      summary: Sign document using hash (min fn; no return)
      description: Cryptographically sign the document and add the record to blockchain.  The
        document history and status is updated for querying.  The API call does not
        return any document properties.  This is a <b>minimalistic function</b> for
        stringing with other functions
      operationId: EthledgerSigncertPost
      x-api-path-slug: ethledgersigncert-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: strHash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Sign
      - Document
      - Using
      - Hash
      - (min
      - Fn;
      - "No"
      - Return)
  /ethledger/getdocstate:
    post:
      summary: Get document status using hash
      description: Review the document status - existence, hash, block info, signatories,
        routing to users and details
      operationId: EthledgerGetdocstatePost
      x-api-path-slug: ethledgergetdocstate-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: strHash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Document
      - Status
      - Using
      - Hash
  /ethledger/posthash:
    post:
      summary: Write hash to blockchain
      description: Post string hash into eth chain for POE (proof of existence)
      operationId: EthledgerPosthashPost
      x-api-path-slug: ethledgerposthash-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: hash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Write
      - Hash
      - To
      - Blockchain
  /ethledger/existshash:
    post:
      summary: Check hash exists on blockchain
      description: Check if your hash exists in the eth blockchain
      operationId: EthledgerExistshashPost
      x-api-path-slug: ethledgerexistshash-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: hash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Check
      - Hash
      - Exists
      - "On"
      - Blockchain
  /ethledger/poststr:
    post:
      summary: Write message to blockchain
      description: Post string hash into eth chain for POE (proof of existence)
      operationId: EthledgerPoststrPost
      x-api-path-slug: ethledgerpoststr-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: str
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Write
      - Message
      - To
      - Blockchain
  /ethledger/existsstr:
    post:
      summary: Check message exists on blockchain
      description: Check if your string exists in the eth blockchain
      operationId: EthledgerExistsstrPost
      x-api-path-slug: ethledgerexistsstr-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: str
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Check
      - Message
      - Exists
      - "On"
      - Blockchain
  /ethledger/gettrans:
    get:
      summary: Document transactions
      description: Displays all transactions connected to this project / smart contract
      operationId: EthledgerGettransGet
      x-api-path-slug: ethledgergettrans-get
      parameters:
      - in: header
        name: ApiKey
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Document
      - Transactions
  /tradechain/CreateTradeContract:
    post:
      summary: List product for sale
      description: "List product on marketplace: <br/>\r\n- Seller initiates sale
        - CreateTradeContract<br/>\r\n- Escrow from seller added for value of contract<br/>\r\n-
        End transaction state = Smart Contract Created<br/>"
      operationId: TradechainCreateTradeContractPost
      x-api-path-slug: tradechaincreatetradecontract-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemName
      - in: formData
        name: itemPartNum
      - in: formData
        name: itemSellerName
      - in: formData
        name: itemValidUntil
      - in: formData
        name: itemValue
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - List
      - Productsale
  /tradechain/ConfirmAbort:
    post:
      summary: Remove Listing (by Seller)
      description: "Remove Listing (by Seller)<br/>\r\n- Seller cancels the market
        trade after listing but before bid/buy<br/>\r\n- Escrow from seller is returned
        back to the seller<br/>\r\n- End transaction state = Smart contract is rendered
        inactive<br/>"
      operationId: TradechainConfirmAbortPost
      x-api-path-slug: tradechainconfirmabort-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemContractId
      - in: formData
        name: itemSellerName
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Remove
      - Listing
      - (by
      - Seller)
  /tradechain/ConfirmPurchase:
    post:
      summary: Bid / buy listed item (by Buyer)
      description: "Bid / buy the item listed on the marketplace: <br/>\r\n- Buyer
        confirms interest in buying<br/>\r\n- Escrow from buyer added to value of
        contract<br/>\r\n- Invoice document is created with all details using invoice
        template<br/>\r\n- Invoice is added IPFS and invoice hash into blockchain<br/>\r\n-
        End transaction state = Trade is actively locked between the seller and buyer<br/>"
      operationId: TradechainConfirmPurchasePost
      x-api-path-slug: tradechainconfirmpurchase-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemBuyerName
      - in: formData
        name: itemContractId
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Bid
      - ""
      - ""
      - Buy
      - Listed
      - Item
      - (by
      - Buyer)
  /tradechain/ConfirmRefund:
    post:
      summary: Refund buyer and stop trade (by Seller)
      description: "Seller can cancel the market trade after bid/buy by refunding
        the seller<br/>\r\nEscrow from buyer is returned back to the buyer<br/>\r\nEscrow
        from seller is returned back to the seller (optional: penalties can be imposed)<br/>\r\nEnd
        transaction state = Escrow returned, smart contract cancelled and become inactive<br/>"
      operationId: TradechainConfirmRefundPost
      x-api-path-slug: tradechainconfirmrefund-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemContractId
      - in: formData
        name: itemSellerName
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Refund
      - Buyer
      - Stop
      - Trade
      - (by
      - Seller)
  /tradechain/ConfirmReceived:
    post:
      summary: Delivery of item confirmed (by Buyer)
      description: "Delivery of item confirmed by the buyer \r\n-Escrow is fully sent
        to seller\r\n- End transaction state = TRANSACTION COMPLETE"
      operationId: TradechainConfirmReceivedPost
      x-api-path-slug: tradechainconfirmreceived-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemBuyerName
      - in: formData
        name: itemContractId
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Delivery
      - Of
      - Item
      - Confirmed
      - (by
      - Buyer)
  /tradechain/GetStateOfContract:
    post:
      summary: Get contract details & state
      description: "Get contract details & state\n- Provide full information including\n
        - Escrow amount in contract\n - Contract state \n - Buyer & Seller information\n
        - Links to contract / invoice documents\n - and other contract / sale specific
        information"
      operationId: TradechainGetStateOfContractPost
      x-api-path-slug: tradechaingetstateofcontract-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemContractId
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Contract
      - Details
      - '&'
      - State
  /tradechain/GetFundsLockedInContract:
    post:
      summary: Get contract escrow details
      description: "Get contract escrow details -\n- Retrieves full information including
        but not limited to\n - Escrow amount in contract\n - Contract state \n - Buyer
        & Seller information\n - Links to contract / invoice documents\n - and other
        contract / sale specific information"
      operationId: TradechainGetFundsLockedInContractPost
      x-api-path-slug: tradechaingetfundslockedincontract-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemContractId
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Contract
      - Escrow
      - Details
  /tradechain/WhoIsSeller:
    post:
      summary: Get seller information
      description: Get full information about the seller by providing the contract
        id.  Response will also include some contract details.
      operationId: TradechainWhoIsSellerPost
      x-api-path-slug: tradechainwhoisseller-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemContractId
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Seller
      - Information
  /tradechain/WhoIsBuyer:
    post:
      summary: Get buyer information
      description: Get full information about the seller by providing the contract
        id.  Response will also include some contract details.
      operationId: TradechainWhoIsBuyerPost
      x-api-path-slug: tradechainwhoisbuyer-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemContractId
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Buyer
      - Information
  /tradechain/GetItemsFilterSort:
    post:
      summary: Report / list of marketplace transactions
      description: "Use a combination of fields to get any type of report.  Ex. send
        specific seller name or id to get active for sale items by seller; send specific
        filehash to get status of a particular item/invoice; send itemPartNum to get
        a list of all products of that partnumber and send sort order as itemValue
        ascending to cheapest top list) . . . \r\n-\tfilterField (accepted items below,
        default \u2013 none)\r\no\titemSellerId\r\no\titemSellerName\r\no\titemBuyerId\r\no\titemBuyerName\r\no\titemId\r\no\titemName\r\no\titemPartNum\r\no\tfileHash\r\no\tFileHash\r\n-\tsortField
        (accepted items below, default \u2013 itemValidUntil)\r\no\titemSellerId\r\no\titemSellerName\r\no\titemBuyerId\r\no\titemBuyerName\r\no\titemId\r\no\titemName\r\no\titemValue\r\no\titemPartNum\r\no\titemValidUntil\r\n-\tsortOrder
        (default \u2013 desc)\r\no\tasc\r\no\tdesc\r\n-\tonSaleOnly (default \u2013
        true, only if not \u201CInactive\u201D)\r\no\ttrue\r\no\tfalse\r\n-\tmaxPrice
        (double; default - 0)"
      operationId: TradechainGetItemsFilterSortPost
      x-api-path-slug: tradechaingetitemsfiltersort-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: filterField
      - in: formData
        name: filterValue
      - in: formData
        name: maxPrice
      - in: formData
        name: onSaleOnly
      - in: formData
        name: sortField
      - in: formData
        name: sortOrder
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Report
      - ""
      - ""
      - List
      - Of
      - Marketplace
      - Transactions
  /basicfns/GetAccountBalance:
    post:
      summary: Get user's account balance (*)
      description: Get information about an user's account balance.  The call is restricted
        to the unlocked user's account / query only. <br/>* In this sandbox, you can
        query any user's account balance for testing purposes.  All accounts are test
        accounts and no actual value or account is exposed in the sandbox.
      operationId: BasicfnsGetAccountBalancePost
      x-api-path-slug: basicfnsgetaccountbalance-post
      parameters:
      - in: formData
        name: accountId
      - in: header
        name: ApiKey
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Users
      - Account
      - Balance
      - (*)
  /ethledger/ipfsadd:
    post:
      summary: Write document to IPFS
      description: Post the document into ipfs for safekeep!
      operationId: EthledgerIpfsaddPost
      x-api-path-slug: ethledgeripfsadd-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: files
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Write
      - Document
      - To
      - IPFS
  /ethledger/ipfsget:
    post:
      summary: Retrieve document from IPFS
      description: Retrieve the document stream from IPFS node
      operationId: EthledgerIpfsgetPost
      x-api-path-slug: ethledgeripfsget-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: hash
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Retrieve
      - Document
      - From
      - IPFS