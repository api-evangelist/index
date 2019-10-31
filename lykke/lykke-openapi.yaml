swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/AccountExist:
    get:
      summary: Get API Account Exist
      description: Get api account exist.
      operationId: ApiAccountExistGet
      x-api-path-slug: apiaccountexist-get
      parameters:
      - in: query
        name: email
      - in: query
        name: partnerId
      responses:
        200:
          description: OK
      tags:
      - Account
      - Exist
  /api/AllAssetDescription/{id}:
    get:
      summary: Get API All Asset Description
      description: Get api all asset description.
      operationId: ApiAllAssetDescriptionByIdGet
      x-api-path-slug: apiallassetdescriptionid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Description
  /api/AllAssetPairRates:
    get:
      summary: Get API All Asset Pair Rates
      description: Get api all asset pair rates.
      operationId: ApiAllAssetPairRatesGet
      x-api-path-slug: apiallassetpairrates-get
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Pair
      - Rates
  /api/AllAssetPairRates/{id}:
    get:
      summary: Get API All Asset Pair Rates
      description: Get api all asset pair rates.
      operationId: ApiAllAssetPairRatesByIdGet
      x-api-path-slug: apiallassetpairratesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Pair
      - Rates
  /api/AllAssetPairs:
    get:
      summary: Get API All Asset Pairs
      description: Get api all asset pairs.
      operationId: ApiAllAssetPairsGet
      x-api-path-slug: apiallassetpairs-get
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Pairs
  /api/AllAssetPairs/{id}:
    get:
      summary: Get API All Asset Pairs
      description: Get api all asset pairs.
      operationId: ApiAllAssetPairsByIdGet
      x-api-path-slug: apiallassetpairsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Pairs
  /api/ApplicationInfo:
    get:
      summary: Get API Application Information
      description: Get api application information.
      operationId: ApiApplicationInfoGet
      x-api-path-slug: apiapplicationinfo-get
      responses:
        200:
          description: OK
      tags:
      - Application
      - Information
  /api/AppSettings:
    get:
      summary: Get API Application Settings
      description: Get api application settings.
      operationId: ApiAppSettingsGet
      x-api-path-slug: apiappsettings-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Application
      - Settings
  /api/assetcategories:
    get:
      summary: Get API Asset Categories
      description: Get api asset categories.
      operationId: ApiAssetcategoriesGet
      x-api-path-slug: apiassetcategories-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Categories
  /api/AssetDescription/{id}:
    get:
      summary: Get API Assetdescription
      description: Get api assetdescription.
      operationId: ApiAssetDescriptionByIdGet
      x-api-path-slug: apiassetdescriptionid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Assetdescription
  /api/AssetDisclaimers:
    get:
      summary: Get API Asset Dsclaimers
      description: Get api asset dsclaimers.
      operationId: AssetDisclaimersGet
      x-api-path-slug: apiassetdisclaimers-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Dsclaimers
  /api/AssetDisclaimers/{disclaimerId}/approve:
    post:
      summary: Add API Asset Dsclaimers Disclaimer Approve
      description: Add api asset dsclaimers disclaimer approve.
      operationId: AssetDisclaimersApprove
      x-api-path-slug: apiassetdisclaimersdisclaimeridapprove-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: disclaimerId
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Dsclaimers
      - Disclaimer
      - Approve
  /api/AssetDisclaimers/{disclaimerId}/decline:
    post:
      summary: Add API Asset Dsclaimers Disclaimer Decline
      description: Add api asset dsclaimers disclaimer decline.
      operationId: AssetDisclaimersDecline
      x-api-path-slug: apiassetdisclaimersdisclaimeriddecline-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: disclaimerId
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Dsclaimers
      - Disclaimer
      - Decline
  /api/AssetPair/{id}:
    get:
      summary: Get API Assetpair
      description: Get api assetpair.
      operationId: ApiAssetPairByIdGet
      x-api-path-slug: apiassetpairid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Assetpair
  /api/AssetPairDetailedRates:
    get:
      summary: Get API Assetpairdetailedrates
      description: Get api assetpairdetailedrates.
      operationId: ApiAssetPairDetailedRatesGet
      x-api-path-slug: apiassetpairdetailedrates-get
      parameters:
      - in: query
        name: assetId
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: period
      - in: query
        name: points
      - in: query
        name: withBid
      responses:
        200:
          description: OK
      tags:
      - Assetpairdetailedrates
  /api/AssetPairRates:
    get:
      summary: Get API Assetpairrates
      description: Get api assetpairrates.
      operationId: ApiAssetPairRatesGet
      x-api-path-slug: apiassetpairrates-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: ignoreBase
      responses:
        200:
          description: OK
      tags:
      - Assetpairrates
  /api/AssetPairRates/{id}:
    get:
      summary: Get API Assetpairrates
      description: Get api assetpairrates.
      operationId: ApiAssetPairRatesByIdGet
      x-api-path-slug: apiassetpairratesid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Assetpairrates
  /api/AssetPairs:
    get:
      summary: Get API Assetpairs
      description: Get api assetpairs.
      operationId: ApiAssetPairsGet
      x-api-path-slug: apiassetpairs-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Assetpairs
  /api/Assets:
    get:
      summary: Get API Assets
      description: Get api assets.
      operationId: ApiAssetsGet
      x-api-path-slug: apiassets-get
      responses:
        200:
          description: OK
      tags:
      - Assets
  /api/Assets/{id}:
    get:
      summary: Get API Assets
      description: Get api assets.
      operationId: ApiAssetsByIdGet
      x-api-path-slug: apiassetsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Assets
  /api/Assets/description/list:
    post:
      summary: Add API Assets Description List
      description: Add api assets description list.
      operationId: ApiAssetsDescriptionListPost
      x-api-path-slug: apiassetsdescriptionlist-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Assets
      - Description
      - List
  /api/Assets/{assetId}/attributes:
    get:
      summary: Get API Assets Asset Attributes
      description: Get api assets asset attributes.
      operationId: ApiAssetsByAssetIdAttributesGet
      x-api-path-slug: apiassetsassetidattributes-get
      parameters:
      - in: path
        name: assetId
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Assets
      - Asset
      - Attributes
  /api/Assets/{assetId}/attributes/{key}:
    get:
      summary: Get API Assets Asset Attributes Key
      description: Get api assets asset attributes key.
      operationId: ApiAssetsByAssetIdAttributesByKeyGet
      x-api-path-slug: apiassetsassetidattributeskey-get
      parameters:
      - in: path
        name: assetId
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - Assets
      - Asset
      - Attributes
      - Key
  /api/Auth:
    post:
      summary: Add API Auth
      description: Add api auth.
      operationId: ApiAuthPost
      x-api-path-slug: apiauth-post
      parameters:
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Auth
  /api/Auth/LogOut:
    post:
      summary: Add API Auth Logout
      description: Add api auth logout.
      operationId: ApiAuthLogOutPost
      x-api-path-slug: apiauthlogout-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Auth
      - Logout
  /api/BackupCompleted:
    post:
      summary: Add API Backup Completed
      description: Add api backup completed.
      operationId: ApiBackupCompletedPost
      x-api-path-slug: apibackupcompleted-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Backup
      - Completed
  /api/BankCardPaymentUrl:
    post:
      summary: Add API Bankcardpaymenturl
      description: Add api bankcardpaymenturl.
      operationId: ApiBankCardPaymentUrlPost
      x-api-path-slug: apibankcardpaymenturl-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: input
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bankcardpaymenturl
  /api/BankCardPaymentUrlFormValues:
    get:
      summary: Get API Bankcardpaymenturlformvalues
      description: Get api bankcardpaymenturlformvalues.
      operationId: ApiBankCardPaymentUrlFormValuesGet
      x-api-path-slug: apibankcardpaymenturlformvalues-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Bankcardpaymenturlformvalues
  /api/BankTransferRequest:
    post:
      summary: Add API Banktransferrequest
      description: Add api banktransferrequest.
      operationId: ApiBankTransferRequestPost
      x-api-path-slug: apibanktransferrequest-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: transferReq
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Banktransferrequest
  /api/BaseAsset:
    get:
      summary: Get API Baseasset
      description: Get api baseasset.
      operationId: ApiBaseAssetGet
      x-api-path-slug: apibaseasset-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Baseasset
    post:
      summary: Add API Baseasset
      description: Add api baseasset.
      operationId: ApiBaseAssetPost
      x-api-path-slug: apibaseasset-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Baseasset
  /api/BaseAssets:
    get:
      summary: Get API Baseassets
      description: Get api baseassets.
      operationId: ApiBaseAssetsGet
      x-api-path-slug: apibaseassets-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Baseassets
  /api/BcnTransaction:
    get:
      summary: Get API Bcntransaction
      description: Get api bcntransaction.
      operationId: ApiBcnTransactionGet
      x-api-path-slug: apibcntransaction-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: id
      responses:
        200:
          description: OK
      tags:
      - Bcntransaction
  /api/BcnTransaction/offchain-trade:
    get:
      summary: Get API Bcntransaction Offchain Trade
      description: Get api bcntransaction offchain trade.
      operationId: ApiBcnTransactionOffchain-tradeGet
      x-api-path-slug: apibcntransactionoffchaintrade-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: id
      responses:
        200:
          description: OK
      tags:
      - Bcntransaction
      - Offchain
      - Trade
  /api/BcnTransactionByCashOperation/{id}:
    get:
      summary: Get API Bcntransactionbycashoperation
      description: Get api bcntransactionbycashoperation.
      operationId: ApiBcnTransactionByCashOperationByIdGet
      x-api-path-slug: apibcntransactionbycashoperationid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Bcntransactionbycashoperation
  /api/BcnTransactionByExchange/{id}:
    get:
      summary: Get API Bcntransactionbyexchange
      description: Get api bcntransactionbyexchange.
      operationId: ApiBcnTransactionByExchangeByIdGet
      x-api-path-slug: apibcntransactionbyexchangeid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Bcntransactionbyexchange
  /api/BcnTransactionByTransfer/{id}:
    get:
      summary: Get API Bcntransactionbytransfer
      description: Get api bcntransactionbytransfer.
      operationId: ApiBcnTransactionByTransferByIdGet
      x-api-path-slug: apibcntransactionbytransferid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Bcntransactionbytransfer
  /api/BitcoinCash/multisig/balance:
    get:
      summary: Get API Bitcoincash Multisig Balance
      description: Get api bitcoincash multisig balance.
      operationId: ApiBitcoinCashMultisigBalanceGet
      x-api-path-slug: apibitcoincashmultisigbalance-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Bitcoincash
      - Multisig
      - Balance
  /api/BitcoinCash/multisig/transaction:
    get:
      summary: Get API Bitcoincash Multisig Transaction
      description: Get api bitcoincash multisig transaction.
      operationId: ApiBitcoinCashMultisigTransactionGet
      x-api-path-slug: apibitcoincashmultisigtransaction-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: destinationAddress
      responses:
        200:
          description: OK
      tags:
      - Bitcoincash
      - Multisig
      - Transaction
  /api/BitcoinCash/private/balance:
    get:
      summary: Get API Bitcoincash Private Balance
      description: Get api bitcoincash private balance.
      operationId: ApiBitcoinCashPrivateBalanceGet
      x-api-path-slug: apibitcoincashprivatebalance-get
      parameters:
      - in: query
        name: address
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Bitcoincash
      - Private
      - Balance
  /api/BitcoinCash/private/transaction:
    get:
      summary: Get API Bitcoincash Private Transaction
      description: Get api bitcoincash private transaction.
      operationId: ApiBitcoinCashPrivateTransactionGet
      x-api-path-slug: apibitcoincashprivatetransaction-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: destinationAddress
      - in: query
        name: fee
      - in: query
        name: sourceAddress
      responses:
        200:
          description: OK
      tags:
      - Bitcoincash
      - Private
      - Transaction
  /api/BitcoinCash/broadcast:
    post:
      summary: Add API Bitcoincash Broadcast
      description: Add api bitcoincash broadcast.
      operationId: ApiBitcoinCashBroadcastPost
      x-api-path-slug: apibitcoincashbroadcast-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bitcoincash
      - Broadcast
  /api/BlockchainTransaction:
    get:
      summary: Get API Blockchaintransaction
      description: Get api blockchaintransaction.
      operationId: ApiBlockchainTransactionGet
      x-api-path-slug: apiblockchaintransaction-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: blockChainHash
      responses:
        200:
          description: OK
      tags:
      - Blockchaintransaction
  /api/BroadcastTransaction:
    post:
      summary: Add API Broadcasttransaction
      description: Add api broadcasttransaction.
      operationId: ApiBroadcastTransactionPost
      x-api-path-slug: apibroadcasttransaction-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: transaction
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Broadcasttransaction
  /api/CashOut:
    post:
      summary: Add API Cashout
      description: Add api cashout.
      operationId: ApiCashOutPost
      x-api-path-slug: apicashout-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cashout
  /api/CashOutSwiftRequest:
    post:
      summary: Add API Cashout Swift Request
      description: Add api cashout swift request.
      operationId: ApiCashOutSwiftRequestPost
      x-api-path-slug: apicashoutswiftrequest-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cashout
      - Swift
      - Request
  /api/ChangePinAndPassword:
    post:
      summary: Add API Changepinandpassword
      description: Add api changepinandpassword.
      operationId: ApiChangePinAndPasswordPost
      x-api-path-slug: apichangepinandpassword-post
      parameters:
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Changepinandpassword
  /api/CheckDocumentsToUpload:
    get:
      summary: Get API Checkdocumentstoupload
      description: Get api checkdocumentstoupload.
      operationId: ApiCheckDocumentsToUploadGet
      x-api-path-slug: apicheckdocumentstoupload-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Checkdocumentstoupload
  /api/CheckMobilePhone:
    get:
      summary: Get API Checkmobilephone
      description: Get api checkmobilephone.
      operationId: ApiCheckMobilePhoneGet
      x-api-path-slug: apicheckmobilephone-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: code
      - in: query
        name: phoneNumber
      responses:
        200:
          description: OK
      tags:
      - Checkmobilephone
    post:
      summary: Add API Checkmobilephone
      description: Add api checkmobilephone.
      operationId: ApiCheckMobilePhonePost
      x-api-path-slug: apicheckmobilephone-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: phoneModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Checkmobilephone
  /api/Client/codes:
    get:
      summary: Get API Client Codes
      description: Get api client codes.
      operationId: ApiClientCodesGet
      x-api-path-slug: apiclientcodes-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Client
      - Codes
    post:
      summary: Add API Client Codes
      description: Add api client codes.
      operationId: ApiClientCodesPost
      x-api-path-slug: apiclientcodes-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Client
      - Codes
  /api/Client/keys/encodedmainkey:
    post:
      summary: Add API Client Keys Encodedmainkey
      description: Add api client keys encodedmainkey.
      operationId: ApiClientKeysEncodedmainkeyPost
      x-api-path-slug: apiclientkeysencodedmainkey-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Client
      - Keys
      - Encodedmainkey
  /api/Client/balances/{baseAsset}:
    get:
      summary: Get API Client Balances Baseasset
      description: Get api client balances baseasset.
      operationId: ApiClientBalancesByBaseAssetGet
      x-api-path-slug: apiclientbalancesbaseasset-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: baseAsset
      responses:
        200:
          description: OK
      tags:
      - Client
      - Balances
      - Baseasset
  /api/Client/pushTxDialogOk:
    post:
      summary: Add API Client Pushtxdialogok
      description: Add api client pushtxdialogok.
      operationId: ApiClientPushTxDialogOkPost
      x-api-path-slug: apiclientpushtxdialogok-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Client
      - Pushtxdialogok
  /api/Client/dictionary/{key}:
    get:
      summary: Get API Client Dictionary Key
      description: Get api client dictionary key.
      operationId: ApiClientDictionaryByKeyGet
      x-api-path-slug: apiclientdictionarykey-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dictionary
      - Key
    delete:
      summary: Delete API Client Dictionary Key
      description: Delete api client dictionary key.
      operationId: ApiClientDictionaryByKeyDelete
      x-api-path-slug: apiclientdictionarykey-delete
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dictionary
      - Key
  /api/Client/dictionary:
    put:
      summary: Put API Client Dictionary
      description: Put api client dictionary.
      operationId: ApiClientDictionaryPut
      x-api-path-slug: apiclientdictionary-put
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: keyValue
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dictionary
    post:
      summary: Add API Client Dictionary
      description: Add api client dictionary.
      operationId: ApiClientDictionaryPost
      x-api-path-slug: apiclientdictionary-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: keyValue
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dictionary
  /api/Client/properties/isUserFromUS:
    get:
      summary: Get API Client Properties Isuserfromus
      description: Get api client properties isuserfromus.
      operationId: ApiClientPropertiesIsUserFromUSGet
      x-api-path-slug: apiclientpropertiesisuserfromus-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Client
      - Properties
      - Isuserfromus
    post:
      summary: Add API Client Properties Isuserfromus
      description: Add api client properties isuserfromus.
      operationId: ApiClientPropertiesIsUserFromUSPost
      x-api-path-slug: apiclientpropertiesisuserfromus-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Client
      - Properties
      - Isuserfromus
  /api/Client/pendingActions:
    get:
      summary: Get API Client Pendingactions
      description: Get api client pendingactions.
      operationId: ApiClientPendingActionsGet
      x-api-path-slug: apiclientpendingactions-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Client
      - Pendingactions
  /api/ClientFirstNameLastName:
    post:
      summary: Add API Clientfirstnamelastname
      description: Add api clientfirstnamelastname.
      operationId: ApiClientFirstNameLastNamePost
      x-api-path-slug: apiclientfirstnamelastname-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Clientfirstnamelastname
  /api/ClientFullName:
    post:
      summary: Add API Clientfullname
      description: Add api clientfullname.
      operationId: ApiClientFullNamePost
      x-api-path-slug: apiclientfullname-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: fullNameModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Clientfullname
  /api/ClientKeys:
    post:
      summary: Add API Clientkeys
      description: Add api clientkeys.
      operationId: ApiClientKeysPost
      x-api-path-slug: apiclientkeys-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Clientkeys
  /api/ClientLog:
    post:
      summary: Add API Clientlog
      description: Add api clientlog.
      operationId: ApiClientLogPost
      x-api-path-slug: apiclientlog-post
      parameters:
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Clientlog
  /api/ClientPhone:
    post:
      summary: Add API Clientphone
      description: Add api clientphone.
      operationId: ApiClientPhonePost
      x-api-path-slug: apiclientphone-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: phoneModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Clientphone
  /api/ClientState:
    get:
      summary: Get API Clientstate
      description: Get api clientstate.
      operationId: ApiClientStateGet
      x-api-path-slug: apiclientstate-get
      parameters:
      - in: query
        name: email
      - in: query
        name: partnerId
      responses:
        200:
          description: OK
      tags:
      - Clientstate
  /api/ClientTrading/termsOfUse:
    get:
      summary: Get API Clienttrading Termsofuse
      description: Get api clienttrading termsofuse.
      operationId: ApiClientTradingTermsOfUseGet
      x-api-path-slug: apiclienttradingtermsofuse-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Clienttrading
      - Termsofuse
  /api/ClientTrading/termsOfUse/margin/agree:
    post:
      summary: Add API Clienttrading Termsofuse Margin Agree
      description: Add api clienttrading termsofuse margin agree.
      operationId: ApiClientTradingTermsOfUseMarginAgreePost
      x-api-path-slug: apiclienttradingtermsofusemarginagree-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Clienttrading
      - Termsofuse
      - Margin
      - Agree
  /api/CountryPhoneCodes:
    get:
      summary: Get API Countryphonecodes
      description: Get api countryphonecodes.
      operationId: ApiCountryPhoneCodesGet
      x-api-path-slug: apicountryphonecodes-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Countryphonecodes
  /api/client/Dialogs:
    get:
      summary: Get API Client Dialogs
      description: Get api client dialogs.
      operationId: ApiClientDialogsGet
      x-api-path-slug: apiclientdialogs-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dialogs
    post:
      summary: Add API Client Dialogs
      description: Add api client dialogs.
      operationId: ApiClientDialogsPost
      x-api-path-slug: apiclientdialogs-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Client
      - Dialogs
  /api/Dictionary/{key}:
    get:
      summary: Get API Dictionary Key
      description: Get api dictionary key.
      operationId: ApiDictionaryByKeyGet
      x-api-path-slug: apidictionarykey-get
      parameters:
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - Dictionary
      - Key
  /api/Dictionary:
    get:
      summary: Get API Dictionary
      description: Get api dictionary.
      operationId: ApiDictionaryGet
      x-api-path-slug: apidictionary-get
      responses:
        200:
          description: OK
      tags:
      - Dictionary
  /api/Dicts:
    get:
      summary: Get API Dicts
      description: Get api dicts.
      operationId: ApiDictsGet
      x-api-path-slug: apidicts-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Dicts
  /api/Dicts/assets:
    get:
      summary: Get API Dicts Assets
      description: Get api dicts assets.
      operationId: ApiDictsAssetsGet
      x-api-path-slug: apidictsassets-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Dicts
      - Assets
  /api/Dicts/updates:
    get:
      summary: Get API Dicts Updates
      description: Get api dicts updates.
      operationId: ApiDictsUpdatesGet
      x-api-path-slug: apidictsupdates-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Dicts
      - S
  /api/Email/PrivateWalletAddress:
    post:
      summary: Add API Email Privatewalletaddress
      description: Add api email privatewalletaddress.
      operationId: ApiEmailPrivateWalletAddressPost
      x-api-path-slug: apiemailprivatewalletaddress-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Email
      - Privatewalletaddress
  /api/EmailMeWalletAddress:
    post:
      summary: Add API Emailmewalletaddress
      description: Add api emailmewalletaddress.
      operationId: ApiEmailMeWalletAddressPost
      x-api-path-slug: apiemailmewalletaddress-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: reqModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Emailmewalletaddress
  /api/EmailVerification:
    get:
      summary: Get API Emailverification
      description: Get api emailverification.
      operationId: ApiEmailVerificationGet
      x-api-path-slug: apiemailverification-get
      parameters:
      - in: query
        name: code
      - in: query
        name: email
      - in: query
        name: partnerId
      responses:
        200:
          description: OK
      tags:
      - Emailverification
    post:
      summary: Add API Emailverification
      description: Add api emailverification.
      operationId: ApiEmailVerificationPost
      x-api-path-slug: apiemailverification-post
      parameters:
      - in: body
        name: email
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Emailverification
  /api/EncodedPrivateKey:
    post:
      summary: Add API Encodedprivatekey
      description: Add api encodedprivatekey.
      operationId: ApiEncodedPrivateKeyPost
      x-api-path-slug: apiencodedprivatekey-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Encodedprivatekey
  /api/Ethereum/{operationId}/transfer:
    post:
      summary: Add API Ethereum Operation Transfer
      description: Add api ethereum operation transfer.
      operationId: ApiEthereumByOperationIdTransferPost
      x-api-path-slug: apiethereumoperationidtransfer-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: operationId
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Operation
      - Transfer
  /api/Ethereum/trade:
    post:
      summary: Add API Ethereum Trade
      description: Add api ethereum trade.
      operationId: ApiEthereumTradePost
      x-api-path-slug: apiethereumtrade-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Trade
  /api/Ethereum/cashout:
    post:
      summary: Add API Ethereum Cashout
      description: Add api ethereum cashout.
      operationId: ApiEthereumCashoutPost
      x-api-path-slug: apiethereumcashout-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Cashout
  /api/Ethereum/{operationId}/hash:
    post:
      summary: Add API Ethereum Operation Hash
      description: Add api ethereum operation hash.
      operationId: ApiEthereumByOperationIdHashPost
      x-api-path-slug: apiethereumoperationidhash-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: operationId
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Operation
      - Hash
  /api/Ethereum/transfers:
    get:
      summary: Get API Ethereum Transfers
      description: Get api ethereum transfers.
      operationId: ApiEthereumTransfersGet
      x-api-path-slug: apiethereumtransfers-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Transfers
    post:
      summary: Add API Ethereum Transfers
      description: Add api ethereum transfers.
      operationId: ApiEthereumTransfersPost
      x-api-path-slug: apiethereumtransfers-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: operations
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Transfers
  /api/Ethereum/hash:
    post:
      summary: Add API Ethereum Hash
      description: Add api ethereum hash.
      operationId: ApiEthereumHashPost
      x-api-path-slug: apiethereumhash-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Hash
  /api/Ethereum/privateWallet/generateTransaction:
    post:
      summary: Add API Ethereum Privatewallet Generatetransaction
      description: Add api ethereum privatewallet generatetransaction.
      operationId: ApiEthereumPrivateWalletGenerateTransactionPost
      x-api-path-slug: apiethereumprivatewalletgeneratetransaction-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Privatewallet
      - Generatetransaction
  /api/Ethereum/privateWallet/broadcastTransaction:
    post:
      summary: Add API Ethereum Privatewallet Broadcasttransaction
      description: Add api ethereum privatewallet broadcasttransaction.
      operationId: ApiEthereumPrivateWalletBroadcastTransactionPost
      x-api-path-slug: apiethereumprivatewalletbroadcasttransaction-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: transaction
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Privatewallet
      - Broadcasttransaction
  /api/Ethereum/privateWallet/estimateTransaction:
    post:
      summary: Add API Ethereum Privatewallet Estimatetransaction
      description: Add api ethereum privatewallet estimatetransaction.
      operationId: ApiEthereumPrivateWalletEstimateTransactionPost
      x-api-path-slug: apiethereumprivatewalletestimatetransaction-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: transaction
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Privatewallet
      - Estimatetransaction
  /api/Ethereum/getCurrentNetworkGas:
    get:
      summary: Get API Ethereum Getcurrentnetworkgas
      description: Get api ethereum getcurrentnetworkgas.
      operationId: ApiEthereumGetCurrentNetworkGasGet
      x-api-path-slug: apiethereumgetcurrentnetworkgas-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Currentnetworkgas
  /api/Ethereum/tx/{transactionHash}:
    get:
      summary: Get API Ethereum Tx Transactionhash
      description: Get api ethereum tx transactionhash.
      operationId: ApiEthereumTxByTransactionHashGet
      x-api-path-slug: apiethereumtxtransactionhash-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: transactionHash
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Tx
      - Transactionhash
  /api/Ethereum/history/{address}:
    get:
      summary: Get API Ethereum History Address
      description: Get api ethereum history address.
      operationId: ApiEthereumHistoryByAddressGet
      x-api-path-slug: apiethereumhistoryaddress-get
      parameters:
      - in: path
        name: address
      - in: query
        name: assetId
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: count
      - in: query
        name: start
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - History
      - Ress
  /api/Ethereum/settings:
    get:
      summary: Get API Ethereum Settings
      description: Get api ethereum settings.
      operationId: ApiEthereumSettingsGet
      x-api-path-slug: apiethereumsettings-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - Settings
  /api/ExchangeInfo:
    get:
      summary: Get API Exchangeinfo
      description: Get api exchangeinfo.
      operationId: ApiExchangeInfoGet
      x-api-path-slug: apiexchangeinfo-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: exchangeId
      responses:
        200:
          description: OK
      tags:
      - Exchangeinfo
  /api/FormatCreditVouchersContent:
    post:
      summary: Add API Formatcreditvoucherscontent
      description: Add api formatcreditvoucherscontent.
      operationId: ApiFormatCreditVouchersContentPost
      x-api-path-slug: apiformatcreditvoucherscontent-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Formatcreditvoucherscontent
  /api/operations/ForwardWithdrawal:
    post:
      summary: Add API Operations Forwardwithdrawal
      description: Add api operations forwardwithdrawal.
      operationId: ApiOperationsForwardWithdrawalPost
      x-api-path-slug: apioperationsforwardwithdrawal-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Forwardwithdrawal
  /api/GenerateTransferTransaction:
    post:
      summary: Add API Generatetransfertransaction
      description: Add api generatetransfertransaction.
      operationId: ApiGenerateTransferTransactionPost
      x-api-path-slug: apigeneratetransfertransaction-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Generatetransfertransaction
  /api/GraphPeriods:
    get:
      summary: Get API Graphperiods
      description: Get api graphperiods.
      operationId: ApiGraphPeriodsGet
      x-api-path-slug: apigraphperiods-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Graphperiods
  /api/HashedPwd:
    post:
      summary: Add API Hashedpwd
      description: Add api hashedpwd.
      operationId: ApiHashedPwdPost
      x-api-path-slug: apihashedpwd-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Hashedpwd
  /api/History:
    get:
      summary: Get API History
      description: Get api history.
      operationId: ApiHistoryGet
      x-api-path-slug: apihistory-get
      parameters:
      - in: query
        name: assetId
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - History
  /api/History/limit/trades:
    get:
      summary: Get API History Limit Trades
      description: Get api history limit trades.
      operationId: ApiHistoryLimitTradesGet
      x-api-path-slug: apihistorylimittrades-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - History
      - Limit
      - Trades
  /api/History/limit/order:
    get:
      summary: Get API History Limit Order
      description: Get api history limit order.
      operationId: ApiHistoryLimitOrderGet
      x-api-path-slug: apihistorylimitorder-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - History
      - Limit
      - Order
  /api/History/limit/history:
    get:
      summary: Get API History Limit History
      description: Get api history limit history.
      operationId: ApiHistoryLimitHistoryGet
      x-api-path-slug: apihistorylimithistory-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - History
      - Limit
      - History
  /api/HotWallet/marketOrder:
    post:
      summary: Add API Hotwallet Marketorder
      description: Add api hotwallet marketorder.
      operationId: MarketOrder
      x-api-path-slug: apihotwalletmarketorder-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SignatureVerificationToken
        description: signature verification token
      responses:
        200:
          description: OK
      tags:
      - Hotwallet
      - Marketorder
  /api/HotWallet/limitOrder:
    post:
      summary: Add API Hotwallet Limitorder
      description: Add api hotwallet limitorder.
      operationId: LimitOrder
      x-api-path-slug: apihotwalletlimitorder-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SignatureVerificationToken
        description: signature verification token
      responses:
        200:
          description: OK
      tags:
      - Hotwallet
      - Limitorder
  /api/HotWallet/cashout:
    post:
      summary: Add API Hotwallet Cashout
      description: Add api hotwallet cashout.
      operationId: Cashout
      x-api-path-slug: apihotwalletcashout-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SignatureVerificationToken
        description: signature verification token
      responses:
        200:
          description: OK
      tags:
      - Hotwallet
      - Cashout
  /api/HotWallet/addresses/{destinationAddress}/{assetId}/validity:
    get:
      summary: Get API Hotwallet Addresses Destinationaddress Asset Vality
      description: Get api hotwallet addresses destinationaddress asset vality.
      operationId: AddressValidity
      x-api-path-slug: apihotwalletaddressesdestinationaddressassetidvalidity-get
      parameters:
      - in: path
        name: assetId
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: destinationAddress
      responses:
        200:
          description: OK
      tags:
      - Hotwallet
      - Resses
      - Destinationaddress
      - Asset
      - Vality
  /api/IcoCoinsSold:
    get:
      summary: Get API Icocoinssold
      description: Get api icocoinssold.
      operationId: ApiIcoCoinsSoldGet
      x-api-path-slug: apiicocoinssold-get
      responses:
        200:
          description: OK
      tags:
      - Icocoinssold
  /api/InvertedAssetPairs:
    post:
      summary: Add API Invertedassetpairs
      description: Add api invertedassetpairs.
      operationId: ApiInvertedAssetPairsPost
      x-api-path-slug: apiinvertedassetpairs-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Invertedassetpairs
  /api/IsAlive:
    get:
      summary: Get API Isalive
      description: Get api isalive.
      operationId: ApiIsAliveGet
      x-api-path-slug: apiisalive-get
      responses:
        200:
          description: OK
      tags:
      - Isalive
  /api/IsPinEntered:
    get:
      summary: Get API Ispinentered
      description: Get api ispinentered.
      operationId: ApiIsPinEnteredGet
      x-api-path-slug: apiispinentered-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Ispinentered
  /api/Issuers:
    get:
      summary: Get API Issuers
      description: Get api issuers.
      operationId: ApiIssuersGet
      x-api-path-slug: apiissuers-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Issuers
  /api/Issuers/{id}:
    get:
      summary: Get API Issuers
      description: Get api issuers.
      operationId: ApiIssuersByIdGet
      x-api-path-slug: apiissuersid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Issuers
  /api/KycDocuments:
    get:
      summary: Get API Kycdocuments
      description: Get api kycdocuments.
      operationId: ApiKycDocumentsGet
      x-api-path-slug: apikycdocuments-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Kycdocuments
    post:
      summary: Add API Kycdocuments
      description: Add api kycdocuments.
      operationId: ApiKycDocumentsPost
      x-api-path-slug: apikycdocuments-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Kycdocuments
  /api/KycDocumentsBin/{id}:
    get:
      summary: Get API Kycdocumentsbin
      description: Get api kycdocumentsbin.
      operationId: ApiKycDocumentsBinByIdGet
      x-api-path-slug: apikycdocumentsbinid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: height
      - in: path
        name: id
      - in: query
        name: width
      responses:
        200:
          description: OK
      tags:
      - Kycdocumentsbin
  /api/KycDocumentsBin:
    post:
      summary: Add API Kycdocumentsbin
      description: Add api kycdocumentsbin.
      operationId: ApiKycDocumentsBinPost
      x-api-path-slug: apikycdocumentsbin-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: ext
      - in: query
        name: idType
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - Kycdocumentsbin
  /api/KycDocumentUpload:
    post:
      summary: Add API Kycdocumentupload
      description: Add api kycdocumentupload.
      operationId: ApiKycDocumentUploadPost
      x-api-path-slug: apikycdocumentupload-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: idType
      - in: formfile
        name: photo
      - in: query
        name: type
      - in: formfile
        name: userFile
      responses:
        200:
          description: OK
      tags:
      - Kycdocumentupload
  /api/KycForAsset/{id}:
    get:
      summary: Get API Kycforasset
      description: Get api kycforasset.
      operationId: ApiKycForAssetByIdGet
      x-api-path-slug: apikycforassetid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Kycforasset
  /api/KycStatus:
    get:
      summary: Get API Kycstatus
      description: Get api kycstatus.
      operationId: ApiKycStatusGet
      x-api-path-slug: apikycstatus-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Kycstatus
    post:
      summary: Add API Kycstatus
      description: Add api kycstatus.
      operationId: ApiKycStatusPost
      x-api-path-slug: apikycstatus-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Kycstatus
  /api/LastBaseAssets:
    get:
      summary: Get API Lastbaseassets
      description: Get api lastbaseassets.
      operationId: ApiLastBaseAssetsGet
      x-api-path-slug: apilastbaseassets-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: "n"
      responses:
        200:
          description: OK
      tags:
      - Lastbaseassets
  /api/offchain/limit/list:
    get:
      summary: Get API Offchain Limit List
      description: Get api offchain limit list.
      operationId: ApiOffchainLimitListGet
      x-api-path-slug: apioffchainlimitlist-get
      parameters:
      - in: query
        name: assetPair
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Limit
      - List
  /api/offchain/limit/count:
    get:
      summary: Get API Offchain Limit Count
      description: Get api offchain limit count.
      operationId: ApiOffchainLimitCountGet
      x-api-path-slug: apioffchainlimitcount-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Limit
      - Count
  /api/LykkeNews:
    get:
      summary: Get API Lykkenews
      description: Get api lykkenews.
      operationId: ApiLykkeNewsGet
      x-api-path-slug: apilykkenews-get
      parameters:
      - in: query
        name: skip
      - in: query
        name: take
      responses:
        200:
          description: OK
      tags:
      - Lykkenews
  /api/MarginTrading/account/balance:
    post:
      summary: Add API Margintrading Account Balance
      description: Add api margintrading account balance.
      operationId: ApiMarginTradingAccountBalancePost
      x-api-path-slug: apimargintradingaccountbalance-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Margintrading
      - Account
      - Balance
  /api/MarginTrading/account/reset/{accountId}:
    delete:
      summary: Delete API Margintrading Account Reset Account
      description: Delete api margintrading account reset account.
      operationId: ApiMarginTradingAccountResetByAccountIdDelete
      x-api-path-slug: apimargintradingaccountresetaccountid-delete
      parameters:
      - in: path
        name: accountId
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Margintrading
      - Account
      - Reset
      - Account
  /api/MarginTrading/cashOutSwift:
    post:
      summary: Add API Margintrading Cashoutswift
      description: Add api margintrading cashoutswift.
      operationId: ApiMarginTradingCashOutSwiftPost
      x-api-path-slug: apimargintradingcashoutswift-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Margintrading
      - Cashoutswift
  /api/Market/converter/tobase:
    post:
      summary: Add API Market Converter Tobase
      description: Add api market converter tobase.
      operationId: ApiMarketConverterTobasePost
      x-api-path-slug: apimarketconvertertobase-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market
      - Converter
      - Tobase
  /api/MyLykkeCashInEmail:
    post:
      summary: Add API Mylykkecashinemail
      description: Add api mylykkecashinemail.
      operationId: ApiMyLykkeCashInEmailPost
      x-api-path-slug: apimylykkecashinemail-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: reqModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Mylykkecashinemail
  /api/MyLykkeInfo:
    get:
      summary: Get API Mylykkeinfo
      description: Get api mylykkeinfo.
      operationId: ApiMyLykkeInfoGet
      x-api-path-slug: apimylykkeinfo-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Mylykkeinfo
  /api/MyLykkeSettings:
    get:
      summary: Get API Mylykkesettings
      description: Get api mylykkesettings.
      operationId: ApiMyLykkeSettingsGet
      x-api-path-slug: apimylykkesettings-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Mylykkesettings
  /api/offchain/requests:
    get:
      summary: Get API Offchain Requests
      description: Get api offchain requests.
      operationId: ApiOffchainRequestsGet
      x-api-path-slug: apioffchainrequests-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Requests
  /api/offchain/trade:
    post:
      summary: Add API Offchain Trade
      description: Add api offchain trade.
      operationId: ApiOffchainTradePost
      x-api-path-slug: apioffchaintrade-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Trade
  /api/offchain/limit/trade:
    post:
      summary: Add API Offchain Limit Trade
      description: Add api offchain limit trade.
      operationId: ApiOffchainLimitTradePost
      x-api-path-slug: apioffchainlimittrade-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Limit
      - Trade
  /api/offchain/limit/cancel:
    post:
      summary: Add API Offchain Limit Cancel
      description: Add api offchain limit cancel.
      operationId: ApiOffchainLimitCancelPost
      x-api-path-slug: apioffchainlimitcancel-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Limit
      - Cancel
  /api/offchain/processchannel:
    post:
      summary: Add API Offchain Processchannel
      description: Add api offchain processchannel.
      operationId: ApiOffchainProcesschannelPost
      x-api-path-slug: apioffchainprocesschannel-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Processchannel
  /api/offchain/finalizetransfer:
    post:
      summary: Add API Offchain Finalizetransfer
      description: Add api offchain finalizetransfer.
      operationId: ApiOffchainFinalizetransferPost
      x-api-path-slug: apioffchainfinalizetransfer-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Finalizetransfer
  /api/offchain/requestTransfer:
    post:
      summary: Add API Offchain Requesttransfer
      description: Add api offchain requesttransfer.
      operationId: ApiOffchainRequestTransferPost
      x-api-path-slug: apioffchainrequesttransfer-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Requesttransfer
  /api/offchain/channelkey:
    get:
      summary: Get API Offchain Channelkey
      description: Get api offchain channelkey.
      operationId: ApiOffchainChannelkeyGet
      x-api-path-slug: apioffchainchannelkey-get
      parameters:
      - in: query
        name: asset
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Channelkey
  /api/offchain/transferToMargin:
    post:
      summary: Add API Offchain Transfertomargin
      description: Add api offchain transfertomargin.
      operationId: ApiOffchainTransferToMarginPost
      x-api-path-slug: apioffchaintransfertomargin-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Transfertomargin
  /api/offchain/{operationId}/transferToTrusted:
    post:
      summary: Add API Offchain Operation Transfertotrusted
      description: Add api offchain operation transfertotrusted.
      operationId: ApiOffchainByOperationIdTransferToTrustedPost
      x-api-path-slug: apioffchainoperationidtransfertotrusted-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: operationId
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Operation
      - Transfertotrusted
  /api/offchain/cashout:
    post:
      summary: Add API Offchain Cashout
      description: Add api offchain cashout.
      operationId: ApiOffchainCashoutPost
      x-api-path-slug: apioffchaincashout-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Cashout
  /api/offchain/cashout/swift:
    get:
      summary: Get API Offchain Cashout Swift
      description: Get api offchain cashout swift.
      operationId: ApiOffchainCashoutSwiftGet
      x-api-path-slug: apioffchaincashoutswift-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Cashout
      - Swift
    post:
      summary: Add API Offchain Cashout Swift
      description: Add api offchain cashout swift.
      operationId: ApiOffchainCashoutSwiftPost
      x-api-path-slug: apioffchaincashoutswift-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Cashout
      - Swift
  /api/offchain/cashout/forward:
    post:
      summary: Add API Offchain Cashout Forward
      description: Add api offchain cashout forward.
      operationId: ApiOffchainCashoutForwardPost
      x-api-path-slug: apioffchaincashoutforward-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Cashout
      - Forward
  /api/Operations/unsignedTransactions:
    get:
      summary: Get API Operations Unsignedtransactions
      description: Get api operations unsignedtransactions.
      operationId: ApiOperationsUnsignedTransactionsGet
      x-api-path-slug: apioperationsunsignedtransactions-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Unsignedtransactions
    post:
      summary: Add API Operations Unsignedtransactions
      description: Add api operations unsignedtransactions.
      operationId: ApiOperationsUnsignedTransactionsPost
      x-api-path-slug: apioperationsunsignedtransactions-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Unsignedtransactions
  /api/Operations/list/{status}:
    get:
      summary: Get API Operations List Status
      description: Get api operations list status.
      operationId: ApiOperationsListByStatusGet
      x-api-path-slug: apioperationsliststatus-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: status
      responses:
        200:
          description: OK
      tags:
      - Operations
      - List
      - Status
  /api/Operations/{id}:
    get:
      summary: Get API Operations
      description: Get api operations.
      operationId: ApiOperationsByIdGet
      x-api-path-slug: apioperationsid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Operations
  /api/Operations/{id}/cancel:
    post:
      summary: Add API Operations  Cancel
      description: Add api operations  cancel.
      operationId: ApiOperationsByIdCancelPost
      x-api-path-slug: apioperationsidcancel-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Operations
      - ""
      - Cancel
  /api/Operations/cancel:
    post:
      summary: Add API Operations Cancel
      description: Add api operations cancel.
      operationId: ApiOperationsCancelPost
      x-api-path-slug: apioperationscancel-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Operations
      - Cancel
  /api/OrderBook/{id}:
    get:
      summary: Get API Orderbook
      description: Get api orderbook.
      operationId: ApiOrderBookByIdGet
      x-api-path-slug: apiorderbookid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Orderbook
  /api/PersonalData:
    get:
      summary: Get API Personaldata
      description: Get api personaldata.
      operationId: ApiPersonalDataGet
      x-api-path-slug: apipersonaldata-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Personaldata
  /api/PinSecurity:
    get:
      summary: Get API Pinsecurity
      description: Get api pinsecurity.
      operationId: ApiPinSecurityGet
      x-api-path-slug: apipinsecurity-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: pin
      responses:
        200:
          description: OK
      tags:
      - Pinsecurity
    post:
      summary: Add API Pinsecurity
      description: Add api pinsecurity.
      operationId: ApiPinSecurityPost
      x-api-path-slug: apipinsecurity-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Pinsecurity
  /api/PrivateKeyOwnershipMsg:
    get:
      summary: Get API Privatekeyownershipmsg
      description: Get api privatekeyownershipmsg.
      operationId: ApiPrivateKeyOwnershipMsgGet
      x-api-path-slug: apiprivatekeyownershipmsg-get
      parameters:
      - in: query
        name: email
      - in: query
        name: partnerId
      responses:
        200:
          description: OK
      tags:
      - Privatekeyownershipmsg
    post:
      summary: Add API Privatekeyownershipmsg
      description: Add api privatekeyownershipmsg.
      operationId: ApiPrivateKeyOwnershipMsgPost
      x-api-path-slug: apiprivatekeyownershipmsg-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Privatekeyownershipmsg
  /api/PrivateWallet:
    get:
      summary: Get API Privatewallet
      description: Get api privatewallet.
      operationId: ApiPrivateWalletGet
      x-api-path-slug: apiprivatewallet-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Privatewallet
    put:
      summary: Put API Privatewallet
      description: Put api privatewallet.
      operationId: ApiPrivateWalletPut
      x-api-path-slug: apiprivatewallet-put
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: editModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Privatewallet
    post:
      summary: Add API Privatewallet
      description: Add api privatewallet.
      operationId: ApiPrivateWalletPost
      x-api-path-slug: apiprivatewallet-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: createWalletModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Privatewallet
    delete:
      summary: Delete API Privatewallet
      description: Delete api privatewallet.
      operationId: ApiPrivateWalletDelete
      x-api-path-slug: apiprivatewallet-delete
      parameters:
      - in: query
        name: address
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Privatewallet
  /api/PrivateWallet/{id}:
    get:
      summary: Get API Privatewallet
      description: Get api privatewallet.
      operationId: ApiPrivateWalletByIdGet
      x-api-path-slug: apiprivatewalletid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Privatewallet
  /api/PrivateWallet/key:
    post:
      summary: Add API Privatewallet Key
      description: Add api privatewallet key.
      operationId: ApiPrivateWalletKeyPost
      x-api-path-slug: apiprivatewalletkey-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Privatewallet
      - Key
  /api/PrivateWalletBackup:
    post:
      summary: Add API Privatewalletbackup
      description: Add api privatewalletbackup.
      operationId: ApiPrivateWalletBackupPost
      x-api-path-slug: apiprivatewalletbackup-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: backupModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Privatewalletbackup
  /api/PrivateWalletBalance:
    get:
      summary: Get API Privatewalletbalance
      description: Get api privatewalletbalance.
      operationId: ApiPrivateWalletBalanceGet
      x-api-path-slug: apiprivatewalletbalance-get
      parameters:
      - in: query
        name: address
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Privatewalletbalance
  /api/PrivateWalletHistory:
    get:
      summary: Get API Privatewallethistory
      description: Get api privatewallethistory.
      operationId: ApiPrivateWalletHistoryGet
      x-api-path-slug: apiprivatewallethistory-get
      parameters:
      - in: query
        name: address
      - in: query
        name: assetId
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Privatewallethistory
  /api/PubkeyAddressValidation:
    get:
      summary: Get API Pubkeyaddressvalation
      description: Get api pubkeyaddressvalation.
      operationId: ApiPubkeyAddressValidationGet
      x-api-path-slug: apipubkeyaddressvalidation-get
      parameters:
      - in: query
        name: pubkeyAddress
      responses:
        200:
          description: OK
      tags:
      - Pubkeyaddressvalation
  /api/PurchaseAsset:
    post:
      summary: Add API Purchaseasset
      description: Add api purchaseasset.
      operationId: ApiPurchaseAssetPost
      x-api-path-slug: apipurchaseasset-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Purchaseasset
  /api/PushSettings:
    get:
      summary: Get API Pushsettings
      description: Get api pushsettings.
      operationId: ApiPushSettingsGet
      x-api-path-slug: apipushsettings-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Pushsettings
    post:
      summary: Add API Pushsettings
      description: Add api pushsettings.
      operationId: ApiPushSettingsPost
      x-api-path-slug: apipushsettings-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Pushsettings
  /api/RecoverySmsConfirmation:
    post:
      summary: Add API Recoverysmsconfirmation
      description: Add api recoverysmsconfirmation.
      operationId: ApiRecoverySmsConfirmationPost
      x-api-path-slug: apirecoverysmsconfirmation-post
      parameters:
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recoverysmsconfirmation
  /api/RefundAddress:
    get:
      summary: Get API Refundaddress
      description: Get api refundaddress.
      operationId: ApiRefundAddressGet
      x-api-path-slug: apirefundaddress-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Refundaddress
    post:
      summary: Add API Refundaddress
      description: Add api refundaddress.
      operationId: ApiRefundAddressPost
      x-api-path-slug: apirefundaddress-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: refundAddressModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Refundaddress
  /api/RefundSettings:
    get:
      summary: Get API Refundsettings
      description: Get api refundsettings.
      operationId: ApiRefundSettingsGet
      x-api-path-slug: apirefundsettings-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Refundsettings
    post:
      summary: Add API Refundsettings
      description: Add api refundsettings.
      operationId: ApiRefundSettingsPost
      x-api-path-slug: apirefundsettings-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: refundAddressModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Refundsettings
  /api/Registration:
    get:
      summary: Get API Registration
      description: Get api registration.
      operationId: ApiRegistrationGet
      x-api-path-slug: apiregistration-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Registration
    post:
      summary: Add API Registration
      description: Add api registration.
      operationId: ApiRegistrationPost
      x-api-path-slug: apiregistration-post
      parameters:
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Registration
  /api/RemindPasswordEmail:
    post:
      summary: Add API Remindpasswordemail
      description: Add api remindpasswordemail.
      operationId: ApiRemindPasswordEmailPost
      x-api-path-slug: apiremindpasswordemail-post
      parameters:
      - in: body
        name: reqModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Remindpasswordemail
  /api/RequestVoiceCall:
    post:
      summary: Add API Requestvoicecall
      description: Add api requestvoicecall.
      operationId: ApiRequestVoiceCallPost
      x-api-path-slug: apirequestvoicecall-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Requestvoicecall
  /api/RestrictedCountries:
    get:
      summary: Get API Restrictedcountries
      description: Get api restrictedcountries.
      operationId: ApiRestrictedCountriesGet
      x-api-path-slug: apirestrictedcountries-get
      responses:
        200:
          description: OK
      tags:
      - Restrictedcountries
  /api/SendBlockchainEmail:
    post:
      summary: Add API Sendblockchainemail
      description: Add api sendblockchainemail.
      operationId: ApiSendBlockchainEmailPost
      x-api-path-slug: apisendblockchainemail-post
      parameters:
      - in: query
        name: assetId
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Sendblockchainemail
  /api/ServerTime:
    get:
      summary: Get API Servertime
      description: Get api servertime.
      operationId: ApiServerTimeGet
      x-api-path-slug: apiservertime-get
      responses:
        200:
          description: OK
      tags:
      - Servertime
  /api/SettingSignOrder:
    post:
      summary: Add API Settingsignorder
      description: Add api settingsignorder.
      operationId: ApiSettingSignOrderPost
      x-api-path-slug: apisettingsignorder-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Settingsignorder
  /api/signatureVerificationToken/KeyConfirmation:
    get:
      summary: Get API Signatureverificationtoken Keyconfirmation
      description: Get api signatureverificationtoken keyconfirmation.
      operationId: ApiSignatureVerificationTokenKeyConfirmationGet
      x-api-path-slug: apisignatureverificationtokenkeyconfirmation-get
      parameters:
      - in: query
        name: email
      responses:
        200:
          description: OK
      tags:
      - Signatureverificationtoken
      - Keyconfirmation
    post:
      summary: Add API Signatureverificationtoken Keyconfirmation
      description: Add api signatureverificationtoken keyconfirmation.
      operationId: ApiSignatureVerificationTokenKeyConfirmationPost
      x-api-path-slug: apisignatureverificationtokenkeyconfirmation-post
      parameters:
      - in: body
        name: response
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Signatureverificationtoken
      - Keyconfirmation
  /api/SignRequest:
    get:
      summary: Get API Signrequest
      description: Get api signrequest.
      operationId: ApiSignRequestGet
      x-api-path-slug: apisignrequest-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Signrequest
    post:
      summary: Add API Signrequest
      description: Add api signrequest.
      operationId: ApiSignRequestPost
      x-api-path-slug: apisignrequest-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Signrequest
  /api/SwiftCredentials/{assetId}:
    get:
      summary: Get API Swiftcredentials Asset
      description: Get api swiftcredentials asset.
      operationId: ApiSwiftCredentialsByAssetIdGet
      x-api-path-slug: apiswiftcredentialsassetid-get
      parameters:
      - in: path
        name: assetId
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Swiftcredentials
      - Asset
  /api/SwiftCredentials:
    get:
      summary: Get API Swiftcredentials
      description: Get api swiftcredentials.
      operationId: ApiSwiftCredentialsGet
      x-api-path-slug: apiswiftcredentials-get
      responses:
        200:
          description: OK
      tags:
      - Swiftcredentials
  /api/Transactions:
    get:
      summary: Get API Transactions
      description: Get api transactions.
      operationId: ApiTransactionsGet
      x-api-path-slug: apitransactions-get
      parameters:
      - in: query
        name: assetId
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Transactions
  /api/TransferInfo:
    get:
      summary: Get API Transferinfo
      description: Get api transferinfo.
      operationId: ApiTransferInfoGet
      x-api-path-slug: apitransferinfo-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: transferId
      responses:
        200:
          description: OK
      tags:
      - Transferinfo
  /api/TrustedWallets/{operationId}/transfer:
    post:
      summary: Add API Trustedwallets Operation Transfer
      description: Add api trustedwallets operation transfer.
      operationId: Transfer
      x-api-path-slug: apitrustedwalletsoperationidtransfer-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: operationId
      responses:
        200:
          description: OK
      tags:
      - Trustedwallets
      - Operation
      - Transfer
  /api/Utils/isUSorCanadaNumber/{phoneNumber}:
    get:
      summary: Get API Utils Isusorcanadanumber Phonenumber
      description: Get api utils isusorcanadanumber phonenumber.
      operationId: ApiUtilsIsUSorCanadaNumberByPhoneNumberGet
      x-api-path-slug: apiutilsisusorcanadanumberphonenumber-get
      parameters:
      - in: path
        name: phoneNumber
      responses:
        200:
          description: OK
      tags:
      - Utils
      - Isusorcanadanumber
      - Phonenumber
  /home/Version:
    get:
      summary: Get Home Version
      description: Get home version.
      operationId: HomeVersionGet
      x-api-path-slug: homeversion-get
      responses:
        200:
          description: OK
      tags:
      - Home
      - Version
  /api/WalletMigration:
    post:
      summary: Add API Walletmigration
      description: Add api walletmigration.
      operationId: ApiWalletMigrationPost
      x-api-path-slug: apiwalletmigration-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Walletmigration
  /api/Wallets:
    get:
      summary: Get API Wallets
      description: Get api wallets.
      operationId: ApiWalletsGet
      x-api-path-slug: apiwallets-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Wallets
    post:
      summary: Add API Wallets
      description: Add api wallets.
      operationId: ApiWalletsPost
      x-api-path-slug: apiwallets-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Wallets
  /api/Wallets/{id}:
    get:
      summary: Get API Wallets
      description: Get api wallets.
      operationId: ApiWalletsByIdGet
      x-api-path-slug: apiwalletsid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Wallets
  /api/Wallets/depositaddress/{assetId}:
    post:
      summary: Add API Wallets Depositaddress Asset
      description: Add api wallets depositaddress asset.
      operationId: ApiWalletsDepositaddressByAssetIdPost
      x-api-path-slug: apiwalletsdepositaddressassetid-post
      parameters:
      - in: path
        name: assetId
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Wallets
      - Depositaddress
      - Asset
  /api/WatchLists:
    get:
      summary: Get API Watchlists
      description: Get api watchlists.
      operationId: ApiWatchListsGet
      x-api-path-slug: apiwatchlists-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Watchlists
    post:
      summary: Add API Watchlists
      description: Add api watchlists.
      operationId: ApiWatchListsPost
      x-api-path-slug: apiwatchlists-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Watchlists
  /api/WatchLists/{id}:
    get:
      summary: Get API Watchlists
      description: Get api watchlists.
      operationId: ApiWatchListsByIdGet
      x-api-path-slug: apiwatchlistsid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Watchlists
    put:
      summary: Put API Watchlists
      description: Put api watchlists.
      operationId: ApiWatchListsByIdPut
      x-api-path-slug: apiwatchlistsid-put
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Watchlists
    delete:
      summary: Delete API Watchlists
      description: Delete api watchlists.
      operationId: ApiWatchListsByIdDelete
      x-api-path-slug: apiwatchlistsid-delete
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Watchlists