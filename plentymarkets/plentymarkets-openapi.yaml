swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
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
  /export/{exportKey}:
    get:
      summary: Get Export Keys
      description: Get export keys.
      operationId: getExportExportkey
      x-api-path-slug: exportexportkey-get
      parameters:
      - in: path
        name: exportKey
      responses:
        200:
          description: OK
      tags:
      - Keys
  /export/{exportKey}/{token}:
    get:
      summary: Get Export Key
      description: Get export keys..
      operationId: getExportExportkeyToken
      x-api-path-slug: exportexportkeytoken-get
      parameters:
      - in: path
        name: exportKey
      - in: path
        name: token
      responses:
        200:
          description: OK
      tags:
      - Keys
  /rest/account/login:
    post:
      summary: Login
      description: Logs in to the online store with front end user credentials. The
        login call returns a JSON object that contains information, such as the access
        token and the refresh token.
      operationId: postRestAccountLogin
      x-api-path-slug: restaccountlogin-post
      parameters:
      - in: body
        name: /rest/account/login
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Login
  /rest/account/login/refresh:
    post:
      summary: Refresh
      description: Refreshes the access token using the refresh token. The refresh
        token is part of the login call response.
      operationId: postRestAccountLoginRefresh
      x-api-path-slug: restaccountloginrefresh-post
      responses:
        200:
          description: OK
      tags:
      - Refresh
  /rest/account/logout:
    post:
      summary: Logout
      description: Logs out the front end user from the online store. The access token
        expires.
      operationId: postRestAccountLogout
      x-api-path-slug: restaccountlogout-post
      responses:
        200:
          description: OK
      tags:
      - Logout
  /rest/accounting/locations:
    post:
      summary: Create an accounting location
      description: Creates an accounting location for a client. The plenty ID of the
        client must be specified.
      operationId: postRestAccountingLocations
      x-api-path-slug: restaccountinglocations-post
      parameters:
      - in: body
        name: /rest/accounting/locations
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Location
  /rest/accounting/locations/existing_accounts:
    get:
      summary: Get all unique posting accounts
      description: Get all unique posting accounts.
      operationId: getRestAccountingLocationsExistingAccounts
      x-api-path-slug: restaccountinglocationsexisting-accounts-get
      responses:
        200:
          description: OK
      tags:
      - Unique
      - Posting
      - Accounts
  /rest/accounting/locations/posting_accounts:
    get:
      summary: Get all posting accounts
      description: Get all posting accounts.
      operationId: getRestAccountingLocationsAddingAccounts
      x-api-path-slug: restaccountinglocationsposting-accounts-get
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Accounts
    post:
      summary: Save posting accounts
      description: Save posting accounts.
      operationId: postRestAccountingLocationsAddingAccounts
      x-api-path-slug: restaccountinglocationsposting-accounts-post
      responses:
        200:
          description: OK
      tags:
      - Save
      - Posting
      - Accounts
  /rest/accounting/locations/posting_accounts/{id}:
    delete:
      summary: Delete an posting account
      description: Delete an posting account.
      operationId: deleteRestAccountingLocationsAddingAccounts
      x-api-path-slug: restaccountinglocationsposting-accountsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Account
    get:
      summary: Gets posting account by the unique id
      description: Gets posting account by the unique id.
      operationId: getRestAccountingLocationsAddingAccounts
      x-api-path-slug: restaccountinglocationsposting-accountsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - S
      - Posting
      - Account
      - By
      - Unique
      - Id
  /rest/accounting/locations/revenue_account_configurations:
    get:
      summary: List revenue account configurations
      description: Lists revenue account configurations of a system. The revenue accounts
        are returned as paginated result. By default 50 revenue accounts are on one
        page.
      operationId: getRestAccountingLocationsRevenueAccountConfigurations
      x-api-path-slug: restaccountinglocationsrevenue-account-configurations-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of revenue accounts to be displayed per page
      - in: query
        name: page
        description: The page to get
      responses:
        200:
          description: OK
      tags:
      - List
      - Revenue
      - Account
      - Configurations
  /rest/accounting/locations/{locationId}:
    delete:
      summary: Delete an accounting location
      description: Deletes an accounting location. The ID of the accounting location
        must be specified. Standard accounting locations can not be deleted.
      operationId: deleteRestAccountingLocationsLocation
      x-api-path-slug: restaccountinglocationslocationid-delete
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Location
    get:
      summary: Get an accounting location
      description: Gets an accounting location. The ID of the accounting location
        must be specified.
      operationId: getRestAccountingLocationsLocation
      x-api-path-slug: restaccountinglocationslocationid-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Location
    put:
      summary: Update an accounting location
      description: Updates an accounting location. The ID of the accounting location
        must be specified.
      operationId: putRestAccountingLocationsLocation
      x-api-path-slug: restaccountinglocationslocationid-put
      parameters:
      - in: body
        name: /rest/accounting/locations/{locationId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Location
  /rest/accounting/locations/{locationId}/countries/{countryId}/revenue_accounts:
    get:
      summary: Get the revenue account configuration of a country
      description: Get the revenue account configuration of a country. The ID of the
        accounting location that the country is associated with as well as the ID
        of the country must be specified.
      operationId: getRestAccountingLocationsLocationCountriesCountryRevenueAccounts
      x-api-path-slug: restaccountinglocationslocationidcountriescountryidrevenue-accounts-get
      parameters:
      - in: path
        name: countryId
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Revenue
      - Account
      - Configuration
      - Of
      - Country
  /rest/accounting/locations/{locationId}/debtor_account_configurations:
    get:
      summary: Get debtor account configuration of an accounting location
      description: Gets the debtor account configuration of an accounting location.
        The ID of the accounting location has to be specified. The debtor account
        configuration can contain one standard debtor account only or e.g. several
        accounts for each country of delivery.
      operationId: getRestAccountingLocationsLocationDebtorAccountConfigurations
      x-api-path-slug: restaccountinglocationslocationiddebtor-account-configurations-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Debtor
      - Account
      - Configuration
      - Of
      - Accounting
      - Location
  /rest/accounting/locations/{locationId}/debtor_accounts/{mode}:
    get:
      summary: Lists the debtor accounts by mode.
      description: Lists the debtor accounts of an accounting location by mode. The
        ID of the accounting location and the mode have to be specified.
      operationId: getRestAccountingLocationsLocationDebtorAccountsMode
      x-api-path-slug: restaccountinglocationslocationiddebtor-accountsmode-get
      parameters:
      - in: path
        name: locationId
      - in: path
        name: mode
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Debtor
      - Accounts
      - By
      - Mode
  /rest/accounting/locations/{locationId}/posting_accounts:
    get:
      summary: Get all posting accounts by locationId
      description: Get all posting accounts by locationid.
      operationId: getRestAccountingLocationsLocationAddingAccounts
      x-api-path-slug: restaccountinglocationslocationidposting-accounts-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Accounts
      - By
      - LocationId
  /rest/accounting/locations/{locationId}/posting_key_configurations:
    get:
      summary: Get a posting key configuration of an accounting location
      description: Gets a posting key configuration of an accounting location. The
        ID of the accounting location has to be specified. The posting key configuration
        can contain up to 4 posting keys.
      operationId: getRestAccountingLocationsLocationAddingKeyConfigurations
      x-api-path-slug: restaccountinglocationslocationidposting-key-configurations-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Key
      - Configuration
      - Of
      - Accounting
      - Location
  /rest/accounting/locations/{locationId}/revenue_account_configurations:
    get:
      summary: Get the revenue account configuration of an accounting location
      description: Gets the revenue account configuration of an accounting location.
        A revenue account location configuration contains several revenue accounts.
        The ID of the accounting location has to be specified.
      operationId: getRestAccountingLocationsLocationRevenueAccountConfigurations
      x-api-path-slug: restaccountinglocationslocationidrevenue-account-configurations-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Revenue
      - Account
      - Configuration
      - Of
      - Accounting
      - Location
  /rest/accounting/locations/{locationId}/{type}/posting_accounts:
    get:
      summary: Get all posting accounts by locationId and type
      description: Get all posting accounts by locationid and type.
      operationId: getRestAccountingLocationsLocationTypeAddingAccounts
      x-api-path-slug: restaccountinglocationslocationidtypeposting-accounts-get
      parameters:
      - in: path
        name: locationId
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Accounts
      - By
      - LocationId
      - Type
  /rest/accounting/locations/{webstoreId}/{countryId}/posting_accounts:
    get:
      summary: Get all posting accounts for a country of a webstore
      description: Get all posting accounts for a country of a webstore.
      operationId: getRestAccountingLocationsWebstoreCountryAddingAccounts
      x-api-path-slug: restaccountinglocationswebstoreidcountryidposting-accounts-get
      parameters:
      - in: query
        name: $webstoreId
        description: The ID of the webstore
      - in: path
        name: countryId
      - in: path
        name: webstoreId
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Accountsa
      - Country
      - Of
      - Webstore
  /rest/accounting/stores/locations:
    get:
      summary: List all accounting locations
      description: List all accounting locations.
      operationId: getRestAccountingStoresLocations
      x-api-path-slug: restaccountingstoreslocations-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Accounting
      - Locations
  /rest/accounting/stores/{plentyId}/locations:
    get:
      summary: List accounting locations of a client
      description: Lists accounting locations of a client. The plenty ID of the client
        must be specified.
      operationId: getRestAccountingStoresPlentyLocations
      x-api-path-slug: restaccountingstoresplentyidlocations-get
      parameters:
      - in: query
        name: locationId
        description: The plenty ID
      - in: path
        name: plentyId
      responses:
        200:
          description: OK
      tags:
      - List
      - Accounting
      - Locations
      - Of
      - Client
  /rest/accounts:
    get:
      summary: List accounts
      description: List accounts.
      operationId: getRestAccounts
      x-api-path-slug: restaccounts-get
      parameters:
      - in: query
        name: createdAt
        description: Filter that restricts the search result to accounts that were
          created according to given filters
      - in: query
        name: updatedAt
        description: Filter that restricts the search result to accounts that were
          updated according to given filters
      responses:
        200:
          description: OK
      tags:
      - List
      - Accounts
    post:
      summary: Create an account
      description: Create an account.
      operationId: postRestAccounts
      x-api-path-slug: restaccounts-post
      parameters:
      - in: body
        name: /rest/accounts
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
  /rest/accounts/addresses:
    post:
      summary: Create an address
      description: Create an address.
      operationId: postRestAccountsAddresses
      x-api-path-slug: restaccountsaddresses-post
      parameters:
      - in: body
        name: /rest/accounts/addresses
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Address
  /rest/accounts/addresses/contact_relations:
    get:
      summary: List address contact relations
      description: List address contact relations.
      operationId: getRestAccountsAddressesContactRelations
      x-api-path-slug: restaccountsaddressescontact-relations-get
      parameters:
      - in: query
        name: addressId
        description: Filter that restricts the search result to addresses with a specific
          ID
      - in: query
        name: contactId
        description: Filter that restricts the search result to contacts with a specific
          ID
      - in: query
        name: id
        description: Filter that restricts the search result to address contact relations
          with a specific ID
      - in: query
        name: isPrimary
        description: Filter that restricts the search result depending on the flag
          used
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: typeId
        description: Filter that restricts the search result to address types with
          a specific ID
      - in: query
        name: with
        description: Includes the specified address contact relation information in
          the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Contact
      - Relations
    post:
      summary: Create address contact relations
      description: Create address contact relations.
      operationId: postRestAccountsAddressesContactRelations
      x-api-path-slug: restaccountsaddressescontact-relations-post
      parameters:
      - in: body
        name: /rest/accounts/addresses/contact_relations
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Address
      - Contact
      - Relations
    put:
      summary: Update address contact relations
      description: Update address contact relations.
      operationId: putRestAccountsAddressesContactRelations
      x-api-path-slug: restaccountsaddressescontact-relations-put
      parameters:
      - in: body
        name: /rest/accounts/addresses/contact_relations
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Address
      - Contact
      - Relations
  /rest/accounts/addresses/contact_relations/{addressContactRelationId}:
    delete:
      summary: Delete an address contact relation
      description: Deletes an address contact relation. The ID of the relation must
        be specified.
      operationId: deleteRestAccountsAddressesContactRelationsAddresscontactrelation
      x-api-path-slug: restaccountsaddressescontact-relationsaddresscontactrelationid-delete
      parameters:
      - in: path
        name: addressContactRelationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Contact
      - Relation
    get:
      summary: Get an address contact relation
      description: Gets an address contact relation. The ID of the address contact
        relation must be specified.
      operationId: getRestAccountsAddressesContactRelationsAddresscontactrelation
      x-api-path-slug: restaccountsaddressescontact-relationsaddresscontactrelationid-get
      parameters:
      - in: path
        name: addressContactRelationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Contact
      - Relation
  /rest/accounts/addresses/option_types:
    get:
      summary: List address option types
      description: List address option types.
      operationId: getRestAccountsAddressesOptionTypes
      x-api-path-slug: restaccountsaddressesoption-types-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Option
      - Types
    post:
      summary: Create an address option type
      description: Create an address option type.
      operationId: postRestAccountsAddressesOptionTypes
      x-api-path-slug: restaccountsaddressesoption-types-post
      parameters:
      - in: body
        name: /rest/accounts/addresses/option_types
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - Type
  /rest/accounts/addresses/option_types/{optionTypeId}:
    delete:
      summary: Delete an address option type
      description: Deletes an address option type. The ID of the option type must
        be specified.
      operationId: deleteRestAccountsAddressesOptionTypesOptiontype
      x-api-path-slug: restaccountsaddressesoption-typesoptiontypeid-delete
      parameters:
      - in: path
        name: optionTypeId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - Type
    get:
      summary: Get an address option type
      description: Gets an address option type. The ID of the option type must be
        specified.
      operationId: getRestAccountsAddressesOptionTypesOptiontype
      x-api-path-slug: restaccountsaddressesoption-typesoptiontypeid-get
      parameters:
      - in: path
        name: optionTypeId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - Type
    put:
      summary: Update an address option type
      description: Updates an address option type. The ID of the option type must
        be specified.
      operationId: putRestAccountsAddressesOptionTypesOptiontype
      x-api-path-slug: restaccountsaddressesoption-typesoptiontypeid-put
      parameters:
      - in: body
        name: /rest/accounts/addresses/option_types/{optionTypeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: optionTypeId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - Type
  /rest/accounts/addresses/options/{optionId}:
    delete:
      summary: Delete an address option by the option ID
      description: Deletes an address option. The ID of the option must be specified.
      operationId: deleteRestAccountsAddressesOptionsOption
      x-api-path-slug: restaccountsaddressesoptionsoptionid-delete
      parameters:
      - in: path
        name: optionId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - By
      - Option
      - ID
    get:
      summary: Get an address option
      description: Gets an address option. The ID of the option must be specified.
      operationId: getRestAccountsAddressesOptionsOption
      x-api-path-slug: restaccountsaddressesoptionsoptionid-get
      parameters:
      - in: path
        name: optionId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
    put:
      summary: Update an address option
      description: Updates an address option. The ID of the option must be specified.
      operationId: putRestAccountsAddressesOptionsOption
      x-api-path-slug: restaccountsaddressesoptionsoptionid-put
      parameters:
      - in: path
        name: optionId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
  /rest/accounts/addresses/pos_relations:
    get:
      summary: List address POS relations
      description: List address pos relations.
      operationId: getRestAccountsAddressesPosRelations
      x-api-path-slug: restaccountsaddressespos-relations-get
      parameters:
      - in: query
        name: itemsPerPage
        description: items per page
      - in: query
        name: page
        description: page
      - in: query
        name: with
        description: Includes the specified address pos relation information in the
          results
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - POS
      - Relations
    post:
      summary: Create an address POS relation
      description: Create an address pos relation.
      operationId: postRestAccountsAddressesPosRelations
      x-api-path-slug: restaccountsaddressespos-relations-post
      responses:
        200:
          description: OK
      tags:
      - Address
      - POS
      - Relation
  /rest/accounts/addresses/pos_relations/{addressPosRelationId}:
    delete:
      summary: Delete an address POS relation
      description: Deletes an address POS relation. The ID of the address POS relation
        must be specified.
      operationId: deleteRestAccountsAddressesPosRelationsAddressposrelation
      x-api-path-slug: restaccountsaddressespos-relationsaddressposrelationid-delete
      parameters:
      - in: path
        name: addressPosRelationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - POS
      - Relation
    get:
      summary: Get an address POS relation
      description: Gets an address POS relation. The ID of the address POS relation
        must be specified.
      operationId: getRestAccountsAddressesPosRelationsAddressposrelation
      x-api-path-slug: restaccountsaddressespos-relationsaddressposrelationid-get
      parameters:
      - in: path
        name: addressPosRelationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - POS
      - Relation
    put:
      summary: Update an address POS relation
      description: Updates an address POS relation. The ID of the address POS relation
        must be specified.
      operationId: putRestAccountsAddressesPosRelationsAddressposrelation
      x-api-path-slug: restaccountsaddressespos-relationsaddressposrelationid-put
      parameters:
      - in: path
        name: addressPosRelationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - POS
      - Relation
  /rest/accounts/addresses/relation_types:
    get:
      summary: List address relation types
      description: List address relation types.
      operationId: getRestAccountsAddressesRelationTypes
      x-api-path-slug: restaccountsaddressesrelation-types-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Relation
      - Types
  /rest/accounts/addresses/relations/types/applications/{application}/{lang}:
    get:
      summary: List address relation types
      description: |-
        Lists address relation types. The application and the language must be specified.
        <br>Possible applications:
        <ul>
        <li>contact</li>
        <li>order</li>
        <li>warehouse</li>
        <li>pos</li>
        </ul>
      operationId: getRestAccountsAddressesRelationsTypesApplicationsApplicationLang
      x-api-path-slug: restaccountsaddressesrelationstypesapplicationsapplicationlang-get
      parameters:
      - in: path
        name: application
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Relation
      - Types
  /rest/accounts/addresses/warehouse_relations:
    post:
      summary: Create an address warehouse relation
      description: Create an address warehouse relation.
      operationId: postRestAccountsAddressesWarehouseRelations
      x-api-path-slug: restaccountsaddresseswarehouse-relations-post
      responses:
        200:
          description: OK
      tags:
      - Address
      - Warehouse
      - Relation
  /rest/accounts/addresses/warehouse_relations/{relationId}:
    delete:
      summary: Delete an address warehouse relation
      description: Deletes an address warehouse relation. The ID of the relation must
        be specified.
      operationId: deleteRestAccountsAddressesWarehouseRelationsRelation
      x-api-path-slug: restaccountsaddresseswarehouse-relationsrelationid-delete
      parameters:
      - in: path
        name: relationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Warehouse
      - Relation
    put:
      summary: Update an address warehouse relation
      description: Updates an address warehouse relation. The ID of the relation must
        be specified.
      operationId: putRestAccountsAddressesWarehouseRelationsRelation
      x-api-path-slug: restaccountsaddresseswarehouse-relationsrelationid-put
      parameters:
      - in: path
        name: relationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Warehouse
      - Relation
  /rest/accounts/addresses/{addressId}:
    delete:
      summary: Delete an address
      description: Deletes an address. The ID of the address must be specified.
      operationId: deleteRestAccountsAddressesAddress
      x-api-path-slug: restaccountsaddressesaddressid-delete
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Address
    get:
      summary: Get an address
      description: Gets an address. The ID of the address must be specified.
      operationId: getRestAccountsAddressesAddress
      x-api-path-slug: restaccountsaddressesaddressid-get
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Address
    put:
      summary: Update an address
      description: Updates an address. The ID of the address must be specified.
      operationId: putRestAccountsAddressesAddress
      x-api-path-slug: restaccountsaddressesaddressid-put
      parameters:
      - in: body
        name: /rest/accounts/addresses/{addressId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Address
  /rest/accounts/addresses/{addressId}/options:
    delete:
      summary: Delete an address option by the address ID
      description: Deletes an address option. The ID of the address must be specified.
      operationId: deleteRestAccountsAddressesAddressOptions
      x-api-path-slug: restaccountsaddressesaddressidoptions-delete
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - By
      - Address
      - ID
    get:
      summary: List address options
      description: Lists address options. The ID of the address must be specified.
      operationId: getRestAccountsAddressesAddressOptions
      x-api-path-slug: restaccountsaddressesaddressidoptions-get
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Options
    post:
      summary: Create an address option
      description: Creates an address option. The ID of the address must be specified.
      operationId: postRestAccountsAddressesAddressOptions
      x-api-path-slug: restaccountsaddressesaddressidoptions-post
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
    put:
      summary: Update the address options for an address
      description: Update the address options for an address.
      operationId: putRestAccountsAddressesAddressOptions
      x-api-path-slug: restaccountsaddressesaddressidoptions-put
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Optionsan
      - Address
  /rest/accounts/addresses/{addressId}/related_data:
    get:
      summary: Find address data by address id
      description: Find address data by address id.
      operationId: getRestAccountsAddressesAddressRelatedData
      x-api-path-slug: restaccountsaddressesaddressidrelated-data-get
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Find
      - Address
      - Data
      - By
      - Address
      - Id
  /rest/accounts/contact_relations/{accountContactRelationId}:
    delete:
      summary: Deletes an account contact relation. The ID of the account contact
        relation must be specified.
      description: Deletes an account contact relation. the id of the account contact
        relation must be specified..
      operationId: deleteRestAccountsContactRelationsAccountcontactrelation
      x-api-path-slug: restaccountscontact-relationsaccountcontactrelationid-delete
      parameters:
      - in: path
        name: accountContactRelationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Account
      - Contact
      - Relation
      - ""
      - ID
      - Of
      - Account
      - Contact
      - Relation
      - Must
      - Be
      - Specified
    get:
      summary: Gets an account contact releation. The ID of the account contact relation
        must be specified.
      description: Gets an account contact releation. the id of the account contact
        relation must be specified..
      operationId: getRestAccountsContactRelationsAccountcontactrelation
      x-api-path-slug: restaccountscontact-relationsaccountcontactrelationid-get
      parameters:
      - in: path
        name: accountContactRelationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Account
      - Contact
      - Releation
      - ""
      - ID
      - Of
      - Account
      - Contact
      - Relation
      - Must
      - Be
      - Specified
  /rest/accounts/contacts:
    get:
      summary: List contacts
      description: List contacts.
      operationId: getRestAccountsContacts
      x-api-path-slug: restaccountscontacts-get
      parameters:
      - in: query
        name: billingAddressId
        description: Filter that restricts the search result to contacts with a billing
          address with the id provided
      - in: query
        name: contactAddress
        description: Filter that restricts the search result to contacts with a specific
          address
      - in: query
        name: contactEmail
        description: Filter that restricts the search result to contacts resembling
          to the given email address
      - in: query
        name: contactId
        description: Filter that restricts the search result to a specific contact
      - in: query
        name: countryId
        description: Filter that restricts the search result to contacts with a specific
          country
      - in: query
        name: createdAtAfter
        description: Filter that restricts the search result to contacts that were
          created after a specific date
      - in: query
        name: createdAtBefore
        description: Filter that restricts the search result to contacts that were
          created before a specific date
      - in: query
        name: deliveryAddressId
        description: Filter that restricts the search result to contacts with a delivery
          address with the id provided
      - in: query
        name: email
        description: Filter that restricts the search result to contacts with a specific
          email address
      - in: query
        name: externalId
        description: Filter that restricts the search result to contacts with a specific
          externalId
      - in: query
        name: fullText
        description: Filter for a fulltext search
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: name
        description: Filter that restricts the search result to contacts with a specific
          name
      - in: query
        name: newsletterAllowance
        description: Filter that restricts the search result to contacts who registered
          for the newsletter
      - in: query
        name: newsletterAllowanceAfter
        description: Filter that restricts the search result to contacts who registered
          for the newsletter after a specific date
      - in: query
        name: newsletterAllowanceBefore
        description: Filter that restricts the search result to contacts who registered
          for the newsletter before a specific date
      - in: query
        name: number
        description: Filter that restricts the search result to contacts with a specific
          number
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: plentyId
        description: Filter that restricts the search result to contacts with a specific
          plentyId
      - in: query
        name: postalCode
        description: Filter that restricts the search result to contacts with a specific
          postal code
      - in: query
        name: privatePhone
        description: Filter that restricts the search result to contacts with a private
          phone number
      - in: query
        name: referrerId
        description: Filter that restricts the search result to contacts with a specific
          referrer
      - in: query
        name: town
        description: Filter that restricts the search result to contacts with a specific
          town
      - in: query
        name: typeId
        description: Filter that restricts the search result to contacts with a specific
          contact type
      - in: query
        name: updatedAtAfter
        description: Filter that restricts the search result to contacts that were
          updated after a specific date
      - in: query
        name: updatedAtBefore
        description: Filter that restricts the search result to contacts that were
          updated before a specific date
      - in: query
        name: userId
        description: Filter that restricts the search result to contacts with a specific
          user
      - in: query
        name: with
        description: Includes the specified contact information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Contacts
    post:
      summary: Create a contact
      description: Create a contact.
      operationId: postRestAccountsContacts
      x-api-path-slug: restaccountscontacts-post
      parameters:
      - in: body
        name: /rest/accounts/contacts
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contact
  /rest/accounts/contacts/banks:
    post:
      summary: Create a bank account
      description: Create a bank account.
      operationId: postRestAccountsContactsBanks
      x-api-path-slug: restaccountscontactsbanks-post
      parameters:
      - in: body
        name: /rest/accounts/contacts/banks
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bank
      - Account
  /rest/accounts/contacts/banks/{contactBankId}:
    delete:
      summary: Delete a bank account
      description: Deletes a bank account. The ID of the bank account must be specified.
      operationId: deleteRestAccountsContactsBanksContactbank
      x-api-path-slug: restaccountscontactsbankscontactbankid-delete
      parameters:
      - in: path
        name: contactBankId
      responses:
        200:
          description: OK
      tags:
      - Bank
      - Account
    get:
      summary: Get a bank account
      description: Gets a bank account of the contact. The ID of the bank account
        must be specified.
      operationId: getRestAccountsContactsBanksContactbank
      x-api-path-slug: restaccountscontactsbankscontactbankid-get
      parameters:
      - in: path
        name: contactBankId
      responses:
        200:
          description: OK
      tags:
      - Bank
      - Account
    put:
      summary: Update a bank account
      description: Updates a bank account. The ID of the bank account must be specified.
      operationId: putRestAccountsContactsBanksContactbank
      x-api-path-slug: restaccountscontactsbankscontactbankid-put
      parameters:
      - in: body
        name: /rest/accounts/contacts/banks/{contactBankId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contactBankId
      responses:
        200:
          description: OK
      tags:
      - Bank
      - Account
  /rest/accounts/contacts/classes:
    get:
      summary: List contact classes
      description: List contact classes.
      operationId: getRestAccountsContactsClasses
      x-api-path-slug: restaccountscontactsclasses-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Classes
  /rest/accounts/contacts/classes/{contactClassId}:
    get:
      summary: Get a contact class
      description: Gets a contact class. The ID of the contact class must be specified.
      operationId: getRestAccountsContactsClassesContactclass
      x-api-path-slug: restaccountscontactsclassescontactclassid-get
      parameters:
      - in: path
        name: contactClassId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Class
  /rest/accounts/contacts/contact_events:
    get:
      summary: List contact events
      description: Lists contact events.
      operationId: getRestAccountsContactsContactEvents
      x-api-path-slug: restaccountscontactscontact-events-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Events
    post:
      summary: Create a contact event
      description: Creates a contact event.
      operationId: postRestAccountsContactsContactEvents
      x-api-path-slug: restaccountscontactscontact-events-post
      parameters:
      - in: body
        name: /rest/accounts/contacts/contact_events
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Event
  /rest/accounts/contacts/contact_events/{contactEventId}:
    delete:
      summary: Delete a contact event
      description: Deletes a contact event. The ID of the contact event must be specified.
      operationId: deleteRestAccountsContactsContactEventsContactevent
      x-api-path-slug: restaccountscontactscontact-eventscontacteventid-delete
      parameters:
      - in: path
        name: contactEventId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Event
    put:
      summary: Update a contact event
      description: Updates a contact event. The ID of the contact event must be specified.
      operationId: putRestAccountsContactsContactEventsContactevent
      x-api-path-slug: restaccountscontactscontact-eventscontacteventid-put
      parameters:
      - in: body
        name: /rest/accounts/contacts/contact_events/{contactEventId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contactEventId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Event
  /rest/accounts/contacts/departments:
    get:
      summary: List contact departments
      description: List contact departments.
      operationId: getRestAccountsContactsDepartments
      x-api-path-slug: restaccountscontactsdepartments-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Departments
    post:
      summary: Create a contact department
      description: Create a contact department.
      operationId: postRestAccountsContactsDepartments
      x-api-path-slug: restaccountscontactsdepartments-post
      parameters:
      - in: body
        name: /rest/accounts/contacts/departments
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Department
  /rest/accounts/contacts/departments/{departmentId}:
    delete:
      summary: Delete a contact department
      description: Deletes a contact department. The ID of the department must be
        specified.
      operationId: deleteRestAccountsContactsDepartmentsDepartment
      x-api-path-slug: restaccountscontactsdepartmentsdepartmentid-delete
      parameters:
      - in: path
        name: departmentId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Department
    get:
      summary: Get a contact department
      description: Gets a contact department. The ID of the department must be specified.
      operationId: getRestAccountsContactsDepartmentsDepartment
      x-api-path-slug: restaccountscontactsdepartmentsdepartmentid-get
      parameters:
      - in: path
        name: departmentId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Department
    put:
      summary: Update a contact department
      description: Updates a contact department. The ID of the department must be
        specified.
      operationId: putRestAccountsContactsDepartmentsDepartment
      x-api-path-slug: restaccountscontactsdepartmentsdepartmentid-put
      parameters:
      - in: body
        name: /rest/accounts/contacts/departments/{departmentId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: departmentId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Department
  /rest/accounts/contacts/group_functions:
    get:
      summary: List all group function related data
      description: Lists all data that is related to the contact group function contents.
      operationId: getRestAccountsContactsGroupFunctions
      x-api-path-slug: restaccountscontactsgroup-functions-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Group
      - Function
      - Related
      - Data
    post:
      summary: Apply selected group function options for given contact IDs
      description: Applies selected group function options for given contact IDs.
      operationId: postRestAccountsContactsGroupFunctions
      x-api-path-slug: restaccountscontactsgroup-functions-post
      parameters:
      - in: query
        name: addressLabelTemplate
        description: An address label template ID
      - in: query
        name: contactList
        description: A list of contact IDs
      - in: query
        name: emailTemplate
        description: An email template ID
      - in: query
        name: newsletter
        description: A newsletter folder ID
      responses:
        200:
          description: OK
      tags:
      - Apply
      - Selected
      - Group
      - Function
      - Optionsgiven
      - Contact
      - IDs
  /rest/accounts/contacts/option_sub_types:
    get:
      summary: List contact option sub-types
      description: List contact option sub-types.
      operationId: getRestAccountsContactsOptionSubTypes
      x-api-path-slug: restaccountscontactsoption-sub-types-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Option
      - Sub-types
    post:
      summary: Create a contact option sub-type
      description: Create a contact option sub-type.
      operationId: postRestAccountsContactsOptionSubTypes
      x-api-path-slug: restaccountscontactsoption-sub-types-post
      parameters:
      - in: body
        name: /rest/accounts/contacts/option_sub_types
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - Sub-type
  /rest/accounts/contacts/option_sub_types/{optionSubTypeId}:
    delete:
      summary: Delete a contact option sub-type
      description: Deletes a contact option sub-type. The ID of the option sub-type
        must be specified.
      operationId: deleteRestAccountsContactsOptionSubTypesOptionsubtype
      x-api-path-slug: restaccountscontactsoption-sub-typesoptionsubtypeid-delete
      parameters:
      - in: path
        name: optionSubTypeId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - Sub-type
    get:
      summary: Get a contact option sub-type
      description: Gets a contact option sub-type. The ID of the option sub-type must
        be specified.
      operationId: getRestAccountsContactsOptionSubTypesOptionsubtype
      x-api-path-slug: restaccountscontactsoption-sub-typesoptionsubtypeid-get
      parameters:
      - in: path
        name: optionSubTypeId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - Sub-type
    put:
      summary: Update a contact option sub-type
      description: Updates a contact option sub-type. The ID of the option sub-type
        must be specified.
      operationId: putRestAccountsContactsOptionSubTypesOptionsubtype
      x-api-path-slug: restaccountscontactsoption-sub-typesoptionsubtypeid-put
      parameters:
      - in: body
        name: /rest/accounts/contacts/option_sub_types/{optionSubTypeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: optionSubTypeId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - Sub-type
  /rest/accounts/contacts/option_types:
    get:
      summary: List contact option types
      description: List contact option types.
      operationId: getRestAccountsContactsOptionTypes
      x-api-path-slug: restaccountscontactsoption-types-get
      parameters:
      - in: query
        name: with
        description: Lists possible option sub-types for each listed option if the
          parameter subTypes is set
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Option
      - Types
    post:
      summary: Create a contact option type
      description: Create a contact option type.
      operationId: postRestAccountsContactsOptionTypes
      x-api-path-slug: restaccountscontactsoption-types-post
      parameters:
      - in: body
        name: /rest/accounts/contacts/option_types
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - Type
  /rest/accounts/contacts/option_types/{optionTypeId}:
    delete:
      summary: Delete a contact option type
      description: Deletes a contact option type. The ID of the option type must be
        specified.
      operationId: deleteRestAccountsContactsOptionTypesOptiontype
      x-api-path-slug: restaccountscontactsoption-typesoptiontypeid-delete
      parameters:
      - in: path
        name: optionTypeId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - Type
    get:
      summary: Get a contact option type
      description: Gets a contact option type. The ID of the option type must be specified.
      operationId: getRestAccountsContactsOptionTypesOptiontype
      x-api-path-slug: restaccountscontactsoption-typesoptiontypeid-get
      parameters:
      - in: path
        name: optionTypeId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - Type
    put:
      summary: Update a contact option type
      description: Updates a contact option type. The ID of the option type must be
        specified.
      operationId: putRestAccountsContactsOptionTypesOptiontype
      x-api-path-slug: restaccountscontactsoption-typesoptiontypeid-put
      parameters:
      - in: body
        name: /rest/accounts/contacts/option_types/{optionTypeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: optionTypeId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - Type
  /rest/accounts/contacts/options/{optionId}:
    delete:
      summary: Delete a contact option by the option ID
      description: Deletes a contact option. The ID of the option must be specified.
      operationId: deleteRestAccountsContactsOptionsOption
      x-api-path-slug: restaccountscontactsoptionsoptionid-delete
      parameters:
      - in: path
        name: optionId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - By
      - Option
      - ID
    get:
      summary: Get a contact option by the option ID
      description: Gets a contact option. The ID of the option must be specified.
      operationId: getRestAccountsContactsOptionsOption
      x-api-path-slug: restaccountscontactsoptionsoptionid-get
      parameters:
      - in: path
        name: optionId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - By
      - Option
      - ID
    put:
      summary: Update a contact option by the option ID
      description: Updates a contact option. The ID of the option must be specified.
      operationId: putRestAccountsContactsOptionsOption
      x-api-path-slug: restaccountscontactsoptionsoptionid-put
      parameters:
      - in: path
        name: optionId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - By
      - Option
      - ID
  /rest/accounts/contacts/positions:
    get:
      summary: List contact positions
      description: List contact positions.
      operationId: getRestAccountsContactsPositions
      x-api-path-slug: restaccountscontactspositions-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Positions
    post:
      summary: Create a contact position
      description: Create a contact position.
      operationId: postRestAccountsContactsPositions
      x-api-path-slug: restaccountscontactspositions-post
      parameters:
      - in: body
        name: /rest/accounts/contacts/positions
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Position
  /rest/accounts/contacts/positions/{positionId}:
    delete:
      summary: Delete a contact position
      description: Deletes a contact position. The ID of the position must be specified.
      operationId: deleteRestAccountsContactsPositionsPosition
      x-api-path-slug: restaccountscontactspositionspositionid-delete
      parameters:
      - in: path
        name: positionId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Position
    get:
      summary: Get a contact position
      description: Gets a contact position. The ID of the position must be specified.
      operationId: getRestAccountsContactsPositionsPosition
      x-api-path-slug: restaccountscontactspositionspositionid-get
      parameters:
      - in: path
        name: positionId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Position
    put:
      summary: Update a contact position
      description: Updates a contact position. The ID of the position must be specified.
      operationId: putRestAccountsContactsPositionsPosition
      x-api-path-slug: restaccountscontactspositionspositionid-put
      parameters:
      - in: body
        name: /rest/accounts/contacts/positions/{positionId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: positionId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Position
  /rest/accounts/contacts/types:
    get:
      summary: List contact types
      description: List contact types.
      operationId: getRestAccountsContactsTypes
      x-api-path-slug: restaccountscontactstypes-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Types
    post:
      summary: Create a contact type
      description: Create a contact type.
      operationId: postRestAccountsContactsTypes
      x-api-path-slug: restaccountscontactstypes-post
      parameters:
      - in: body
        name: /rest/accounts/contacts/types
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Type
  /rest/accounts/contacts/types/{typeId}:
    delete:
      summary: Delete a contact type
      description: Deletes a contact type. The ID of the contact type must be specified.
      operationId: deleteRestAccountsContactsTypesType
      x-api-path-slug: restaccountscontactstypestypeid-delete
      parameters:
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Type
    get:
      summary: Get a contact type
      description: Gets a contact type. The ID of the contact type must be specified.
      operationId: getRestAccountsContactsTypesType
      x-api-path-slug: restaccountscontactstypestypeid-get
      parameters:
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Type
    put:
      summary: Update a contact type
      description: Updates a contact type. The ID of the contact type must be specified.
      operationId: putRestAccountsContactsTypesType
      x-api-path-slug: restaccountscontactstypestypeid-put
      parameters:
      - in: body
        name: /rest/accounts/contacts/types/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Type
  /rest/accounts/contacts/{contactId}:
    delete:
      summary: Delete a contact
      description: Deletes a contact. The ID of the contact must be specified.
      operationId: deleteRestAccountsContactsContact
      x-api-path-slug: restaccountscontactscontactid-delete
      parameters:
      - in: query
        name: checkExistingOrders
        description: Flag that checks if the contact is linked to orders
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Contact
    get:
      summary: Get a contact
      description: Gets a contact. The ID of the contact must be specified.
      operationId: getRestAccountsContactsContact
      x-api-path-slug: restaccountscontactscontactid-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: with
        description: Includes the specified contact information in the results
      responses:
        200:
          description: OK
      tags:
      - Contact
    put:
      summary: Update a contact
      description: Updates a contact. The ID of the contact must be specified.
      operationId: putRestAccountsContactsContact
      x-api-path-slug: restaccountscontactscontactid-put
      parameters:
      - in: body
        name: /rest/accounts/contacts/{contactId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Contact
  /rest/accounts/contacts/{contactId}/access_data/login_url:
    get:
      summary: Get the login URL
      description: Gets the URL to login as the given contact. The ID of the contact
        must be specified.
      operationId: getRestAccountsContactsContactAccessDataLoginUrl
      x-api-path-slug: restaccountscontactscontactidaccess-datalogin-url-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Login
      - URL
  /rest/accounts/contacts/{contactId}/access_data/new_password:
    put:
      summary: Send password link for a contact
      description: Sends an email to a contact with a link to change the password.
        The ID of the contact must be specified.
      operationId: putRestAccountsContactsContactAccessDataNewPassword
      x-api-path-slug: restaccountscontactscontactidaccess-datanew-password-put
      parameters:
      - in: path
        name: contactId
      - in: query
        name: password
        description: The new password
      responses:
        200:
          description: OK
      tags:
      - Send
      - Password
      - Linka
      - Contact
  /rest/accounts/contacts/{contactId}/access_data/set_password:
    put:
      summary: Update the password for a contact
      description: Updates the password for a contact. The ID of the contact must
        be specified.
      operationId: putRestAccountsContactsContactAccessDataSetPassword
      x-api-path-slug: restaccountscontactscontactidaccess-dataset-password-put
      parameters:
      - in: path
        name: contactId
      - in: query
        name: password
        description: The new password
      responses:
        200:
          description: OK
      tags:
      - Passworda
      - Contact
  /rest/accounts/contacts/{contactId}/access_data/unblock_user:
    put:
      summary: Unblock a contact
      description: Unblocks a contact to allow this contact to log in again. The ID
        of the contact must be specified.
      operationId: putRestAccountsContactsContactAccessDataUnblockUser
      x-api-path-slug: restaccountscontactscontactidaccess-dataunblock-user-put
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Unblock
      - Contact
  /rest/accounts/contacts/{contactId}/accounts:
    post:
      summary: Create an account for existing contact
      description: Creates an account for an existing contact. The ID of the contact
        must be specified.
      operationId: postRestAccountsContactsContactAccounts
      x-api-path-slug: restaccountscontactscontactidaccounts-post
      parameters:
      - in: body
        name: /rest/accounts/contacts/{contactId}/accounts
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Accountexisting
      - Contact
  /rest/accounts/contacts/{contactId}/accounts/{accountId}:
    delete:
      summary: Delete an account of the contact
      description: Deletes an account of the contact. The ID of the contact and the
        ID of the account must be specified.
      operationId: deleteRestAccountsContactsContactAccountsAccount
      x-api-path-slug: restaccountscontactscontactidaccountsaccountid-delete
      parameters:
      - in: path
        name: accountId
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Account
      - Of
      - Contact
    get:
      summary: Get an account of the contact
      description: Gets an account of the contact. The ID of the contact and the ID
        of the account must be specified.
      operationId: getRestAccountsContactsContactAccountsAccount
      x-api-path-slug: restaccountscontactscontactidaccountsaccountid-get
      parameters:
      - in: path
        name: accountId
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Account
      - Of
      - Contact
    put:
      summary: Update an account
      description: Updates an account. The ID of the contact and the ID of the account
        must be specified.
      operationId: putRestAccountsContactsContactAccountsAccount
      x-api-path-slug: restaccountscontactscontactidaccountsaccountid-put
      parameters:
      - in: path
        name: accountId
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Account
  /rest/accounts/contacts/{contactId}/addresses:
    post:
      summary: Create an address for existing contact and type
      description: Creates an address. The ID of the contact must be specified.
      operationId: postRestAccountsContactsContactAddresses
      x-api-path-slug: restaccountscontactscontactidaddresses-post
      parameters:
      - in: body
        name: /rest/accounts/contacts/{contactId}/addresses
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contactId
      - in: query
        name: isPrimary
        description: Sets a contact address per address type as the primary address
      - in: query
        name: typeId
        description: The type ID of the address
      responses:
        200:
          description: OK
      tags:
      - Addressexisting
      - Contact
      - Type
  /rest/accounts/contacts/{contactId}/addresses/{addressId}:
    delete:
      summary: Delete an address of the contact
      description: Deletes an address of the contact. The ID of the contact and the
        ID of the address must be specified.
      operationId: deleteRestAccountsContactsContactAddressesAddress
      x-api-path-slug: restaccountscontactscontactidaddressesaddressid-delete
      parameters:
      - in: path
        name: addressId
      - in: path
        name: contactId
      - in: query
        name: typeId
        description: The type ID of the address
      responses:
        200:
          description: OK
      tags:
      - Address
      - Of
      - Contact
    put:
      summary: Update an address of the contact
      description: Updates an address of the contact. The ID of the contact and the
        ID of the address must be specified.
      operationId: putRestAccountsContactsContactAddressesAddress
      x-api-path-slug: restaccountscontactscontactidaddressesaddressid-put
      parameters:
      - in: path
        name: addressId
      - in: path
        name: contactId
      - in: query
        name: isPrimary
        description: Sets a contact address per address type as the primary address
      - in: query
        name: typeId
        description: The type ID of the address
      responses:
        200:
          description: OK
      tags:
      - Address
      - Of
      - Contact
  /rest/accounts/contacts/{contactId}/addresses/{addressId}/types/{addressTypeId}/primary:
    put:
      summary: Set a contact address per address type as the primary address
      description: Sets a contact address per address type as the primary address.
        The ID of the contact, the ID of the address and the ID of the address type
        must be specified. A primary address is also definable if you create or update
        a contact address.
      operationId: putRestAccountsContactsContactAddressesAddressTypesAddresstypePrimary
      x-api-path-slug: restaccountscontactscontactidaddressesaddressidtypesaddresstypeidprimary-put
      parameters:
      - in: path
        name: addressId
      - in: path
        name: addressTypeId
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Set
      - Contact
      - Address
      - Per
      - Address
      - Type
      - As
      - Primary
      - Address
  /rest/accounts/contacts/{contactId}/addresses/{addressId}/types/{addressTypeId}/reset_primary:
    put:
      summary: Resets a contact primary address
      description: Resets a contact primary address. The ID of the contact, the ID
        of the address and the ID of the address type must be specified.
      operationId: putRestAccountsContactsContactAddressesAddressTypesAddresstypeResetPrimary
      x-api-path-slug: restaccountscontactscontactidaddressesaddressidtypesaddresstypeidreset-primary-put
      parameters:
      - in: path
        name: addressId
      - in: path
        name: addressTypeId
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Resets
      - Contact
      - Primary
      - Address
  /rest/accounts/contacts/{contactId}/addresses/{addressTypeId?}:
    get:
      summary: List addresses that are linked with contacts
      description: Lists addresses of the contact. The ID of the contact must be specified.
      operationId: getRestAccountsContactsContactAddressesAddresstype
      x-api-path-slug: restaccountscontactscontactidaddressesaddresstypeid-get
      parameters:
      - in: path
        name: addressTypeId?
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - List
      - Addresses
      - That
      - Are
      - Linked
      - Contacts
  /rest/accounts/contacts/{contactId}/anonymize:
    put:
      summary: anonymize Contact
      description: anonymizes the given contact.
      operationId: putRestAccountsContactsContactAnonymize
      x-api-path-slug: restaccountscontactscontactidanonymize-put
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Anonymize
      - Contact
  /rest/accounts/contacts/{contactId}/banks:
    get:
      summary: List bank accounts
      description: Lists bank accounts of the contact. The ID of the contact must
        be specified.
      operationId: getRestAccountsContactsContactBanks
      x-api-path-slug: restaccountscontactscontactidbanks-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - List
      - Bank
      - Accounts
  /rest/accounts/contacts/{contactId}/contact_events:
    get:
      summary: List contact events by contact ID
      description: Lists contact events by contact ID. The ID of the contact must
        be specified.
      operationId: getRestAccountsContactsContactContactEvents
      x-api-path-slug: restaccountscontactscontactidcontact-events-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Events
      - By
      - Contact
      - ID
  /rest/accounts/contacts/{contactId}/document:
    get:
      summary: Get a single storage object from contact documents
      description: Get a single storage object from contact documents.
      operationId: getRestAccountsContactsContactDocument
      x-api-path-slug: restaccountscontactscontactiddocument-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: key
        description: The storage key of the object to get from contact documents
      responses:
        200:
          description: OK
      tags:
      - Single
      - Storage
      - Object
      - From
      - Contact
      - Documents
    post:
      summary: Upload a document to contact directory
      description: Upload a document to contact directory.
      operationId: postRestAccountsContactsContactDocument
      x-api-path-slug: restaccountscontactscontactiddocument-post
      parameters:
      - in: path
        name: contactId
      - in: query
        name: key
        description: The storage key for the file to upload
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Document
      - To
      - Contact
      - Directory
  /rest/accounts/contacts/{contactId}/document/url:
    get:
      summary: Get a temporary url for a single document
      description: Get a temporary url for a single document.
      operationId: getRestAccountsContactsContactDocumentUrl
      x-api-path-slug: restaccountscontactscontactiddocumenturl-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: key
        description: The storage key to get temporary url for
      responses:
        200:
          description: OK
      tags:
      - Temporary
      - Urla
      - Single
      - Document
  /rest/accounts/contacts/{contactId}/documents:
    delete:
      summary: Delete files from contact documents
      description: Delete files from contact documents.
      operationId: deleteRestAccountsContactsContactDocuments
      x-api-path-slug: restaccountscontactscontactiddocuments-delete
      parameters:
      - in: path
        name: contactId
      - in: query
        name: keyList
        description: List of storage keys to delete
      responses:
        200:
          description: OK
      tags:
      - Files
      - From
      - Contact
      - Documents
    get:
      summary: List documents for a single contact
      description: List documents for a single contact.
      operationId: getRestAccountsContactsContactDocuments
      x-api-path-slug: restaccountscontactscontactiddocuments-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: continuationToken
        description: token from previous request to continue listing documents
      responses:
        200:
          description: OK
      tags:
      - List
      - Documentsa
      - Single
      - Contact
  /rest/accounts/contacts/{contactId}/options:
    delete:
      summary: Delete a contact option by the contact ID
      description: Deletes a contact option for an existing contact. The ID of the
        contact must be specified.
      operationId: deleteRestAccountsContactsContactOptions
      x-api-path-slug: restaccountscontactscontactidoptions-delete
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - By
      - Contact
      - ID
    get:
      summary: List contact options by the contact ID
      description: Lists contact options. The ID of the contact must be specified.
      operationId: getRestAccountsContactsContactOptions
      x-api-path-slug: restaccountscontactscontactidoptions-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Options
      - By
      - Contact
      - ID
    post:
      summary: Create a contact option by the contact ID
      description: Creates a contact option for an existing contact. The ID of the
        contact must be specified.
      operationId: postRestAccountsContactsContactOptions
      x-api-path-slug: restaccountscontactscontactidoptions-post
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - By
      - Contact
      - ID
    put:
      summary: Update a contact option by the contact ID
      description: Updates a contact option for an existing contact. The ID of the
        contact must be specified.
      operationId: putRestAccountsContactsContactOptions
      x-api-path-slug: restaccountscontactscontactidoptions-put
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - By
      - Contact
      - ID
  /rest/accounts/contacts/{contactId}/options/validate:
    get:
      summary: Validate a contact option by a given value
      description: validates a contact option by a given value
      operationId: getRestAccountsContactsContactOptionsValate
      x-api-path-slug: restaccountscontactscontactidoptionsvalidate-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Validate
      - Contact
      - Option
      - By
      - Given
      - Value
  /rest/accounts/contacts/{contactId}/related_data:
    get:
      summary: Return all contact related data
      description: Returns all contact related data.
      operationId: getRestAccountsContactsContactRelatedData
      x-api-path-slug: restaccountscontactscontactidrelated-data-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Return
      - ""
      - Contact
      - Related
      - Data
  /rest/accounts/contacts/{contactId}/vcard:
    get:
      summary: get a filestream of vcard from customer
      description: Get a filestream of vcard from customer.
      operationId: getRestAccountsContactsContactVcard
      x-api-path-slug: restaccountscontactscontactidvcard-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Get
      - Filestream
      - Of
      - Vcard
      - From
      - Customer
  /rest/accounts/order_summaries:
    get:
      summary: List order summaries
      description: List order summaries.
      operationId: getRestAccountsOrderSummaries
      x-api-path-slug: restaccountsorder-summaries-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Summaries
    post:
      summary: Create an order summary
      description: Create an order summary.
      operationId: postRestAccountsOrderSummaries
      x-api-path-slug: restaccountsorder-summaries-post
      responses:
        200:
          description: OK
      tags:
      - Order
      - Summary
  /rest/accounts/order_summaries/contacts/{contactId}:
    get:
      summary: Get an order summary by the contact ID
      description: Gets an order summary. The ID of the contact must be specified.
      operationId: getRestAccountsOrderSummariesContactsContact
      x-api-path-slug: restaccountsorder-summariescontactscontactid-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Summary
      - By
      - Contact
      - ID
  /rest/accounts/order_summaries/orders/{addressId}:
    get:
      summary: Get an order summary by the address ID
      description: Gets an order summary. The ID of the address must be specified.
      operationId: getRestAccountsOrderSummariesOrdersAddress
      x-api-path-slug: restaccountsorder-summariesordersaddressid-get
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Summary
      - By
      - Address
      - ID
  /rest/accounts/order_summaries/{orderSummaryId}:
    delete:
      summary: Delete an order summary
      description: Deletes an order summary. The ID of the order summary must be specified.
      operationId: deleteRestAccountsOrderSummariesOrdersummary
      x-api-path-slug: restaccountsorder-summariesordersummaryid-delete
      parameters:
      - in: path
        name: orderSummaryId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Summary
    get:
      summary: Get an order summary by the order summary ID
      description: Gets an order summary. The ID of the order summary must be specified.
      operationId: getRestAccountsOrderSummariesOrdersummary
      x-api-path-slug: restaccountsorder-summariesordersummaryid-get
      parameters:
      - in: path
        name: orderSummaryId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Summary
      - By
      - Order
      - Summary
      - ID
    put:
      summary: Update an order summary
      description: Updates an order summary. The ID of the order summary must be specified.
      operationId: putRestAccountsOrderSummariesOrdersummary
      x-api-path-slug: restaccountsorder-summariesordersummaryid-put
      parameters:
      - in: path
        name: orderSummaryId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Summary
  /rest/accounts/{accountId}:
    delete:
      summary: Delete an account
      description: Deletes an account. The ID of the account must be specified.
      operationId: deleteRestAccountsAccount
      x-api-path-slug: restaccountsaccountid-delete
      parameters:
      - in: path
        name: accountId
      responses:
        200:
          description: OK
      tags:
      - Account
    get:
      summary: Get an account
      description: Gets an account. The ID of the account must be specified.
      operationId: getRestAccountsAccount
      x-api-path-slug: restaccountsaccountid-get
      parameters:
      - in: path
        name: accountId
      responses:
        200:
          description: OK
      tags:
      - Account
    put:
      summary: Update an account
      description: Updates an account. The ID of the account must be specified.
      operationId: putRestAccountsAccount
      x-api-path-slug: restaccountsaccountid-put
      parameters:
      - in: body
        name: /rest/accounts/{accountId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: accountId
      responses:
        200:
          description: OK
      tags:
      - Account
  /rest/accounts/{accountId}/contacts:
    get:
      summary: List contacts
      description: Lists contacts of the account. The ID of the account must be specified.
      operationId: getRestAccountsAccountContacts
      x-api-path-slug: restaccountsaccountidcontacts-get
      parameters:
      - in: path
        name: accountId
      responses:
        200:
          description: OK
      tags:
      - List
      - Contacts
  /rest/authorized_user:
    get:
      summary: Get authorized user
      description: Gets an authorized user. This call returns a JSON object with information
        about the user after login. This information is used for correctly displaying
        the plentymarkets back end.
      operationId: getRestAuthorizedUser
      x-api-path-slug: restauthorized-user-get
      responses:
        200:
          description: OK
      tags:
      - Authorized
      - User
  /rest/availabilities:
    get:
      summary: List item availabilities
      description: Lists all item availabilities.
      operationId: getRestAvailabilities
      x-api-path-slug: restavailabilities-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Availabilities
  /rest/availabilities/{id}:
    get:
      summary: Get an item availability
      description: Gets an item availability. The ID of the availability must be specified.
      operationId: getRestAvailabilities
      x-api-path-slug: restavailabilitiesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Item
      - Availability
    put:
      summary: Update an item availability
      description: Updates an item availability.
      operationId: putRestAvailabilities
      x-api-path-slug: restavailabilitiesid-put
      parameters:
      - in: body
        name: /rest/availabilities/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Item
      - Availability
  /rest/backend/user/{userId}:
    get:
      summary: ""
      description: .
      operationId: getRestBackendUserUser
      x-api-path-slug: restbackenduseruserid-get
      parameters:
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/backend/users:
    get:
      summary: ""
      description: .
      operationId: getRestBackendUsers
      x-api-path-slug: restbackendusers-get
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/backend/users/search_name/{name}:
    get:
      summary: Find all users having a name or username like the given one.
      description: Find all users having a name or username like the given one..
      operationId: getRestBackendUsersSearchNameName
      x-api-path-slug: restbackenduserssearch-namename-get
      parameters:
      - in: path
        name: name
      responses:
        200:
          description: OK
      tags:
      - Find
      - ""
      - Users
      - Having
      - Name
      - Username
      - Like
      - Given
  /rest/basket:
    get:
      summary: Get basket
      description: Gets the shopping cart for the current customer session.
      operationId: getRestBasket
      x-api-path-slug: restbasket-get
      responses:
        200:
          description: OK
      tags:
      - Basket
  /rest/basket/items:
    get:
      summary: List basket items
      description: Lists all items in the shopping cart for the current customer session.
      operationId: getRestBasketItems
      x-api-path-slug: restbasketitems-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Basket
      - Items
    post:
      summary: Add item to basket
      description: Adds a new item to the shopping cart using the request parameters.
      operationId: postRestBasketItems
      x-api-path-slug: restbasketitems-post
      parameters:
      - in: body
        name: /rest/basket/items
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Item
      - To
      - Basket
  /rest/basket/items/{id}:
    get:
      summary: Find a basket item by it's ID
      description: Find a basket item by it's id.
      operationId: getRestBasketItems
      x-api-path-slug: restbasketitemsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Find
      - Basket
      - Item
      - By
      - Its
      - ID
  /rest/batch:
    get:
      summary: Make batch requests
      description: Pass several operations into a single HTTP request.
      operationId: getRestBatch
      x-api-path-slug: restbatch-get
      parameters:
      - in: body
        name: /rest/batch
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Make
      - Batch
      - Requests
  /rest/boards:
    get:
      summary: Lists all boards.
      description: Lists all boards..
      operationId: getRestBoards
      x-api-path-slug: restboards-get
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Boards
    post:
      summary: Creates a new board.
      description: Creates a new board..
      operationId: postRestBoards
      x-api-path-slug: restboards-post
      parameters:
      - in: body
        name: /rest/boards
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Board
  /rest/boards/{boardId}:
    delete:
      summary: Deletes a specific board.
      description: Deletes a specific board..
      operationId: deleteRestBoardsBoard
      x-api-path-slug: restboardsboardid-delete
      parameters:
      - in: path
        name: boardId
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Board
    get:
      summary: Gets a single board by its ID
      description: Gets a single board by its id.
      operationId: getRestBoardsBoard
      x-api-path-slug: restboardsboardid-get
      parameters:
      - in: path
        name: boardId
      - in: query
        name: tasksPerPage
        description: Maximum number of tasks to list per column
      responses:
        200:
          description: OK
      tags:
      - S
      - Single
      - Board
      - By
      - Its
      - ID
    post:
      summary: Copies a specific board.
      description: Copies a specific board..
      operationId: postRestBoardsBoard
      x-api-path-slug: restboardsboardid-post
      parameters:
      - in: path
        name: boardId
      responses:
        200:
          description: OK
      tags:
      - Copies
      - Specific
      - Board
    put:
      summary: Updates a specific board.
      description: Updates a specific board..
      operationId: putRestBoardsBoard
      x-api-path-slug: restboardsboardid-put
      parameters:
      - in: body
        name: /rest/boards/{boardId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: boardId
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Board
  /rest/boards/{boardId}/columns:
    get:
      summary: Lists all columns for a given board
      description: Lists all columns for a given board.
      operationId: getRestBoardsBoardColumns
      x-api-path-slug: restboardsboardidcolumns-get
      parameters:
      - in: path
        name: boardId
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Columnsa
      - Given
      - Board
    post:
      summary: Creates a new column and assigns it to a given board
      description: Creates a new column and assigns it to a given board.
      operationId: postRestBoardsBoardColumns
      x-api-path-slug: restboardsboardidcolumns-post
      parameters:
      - in: body
        name: /rest/boards/{boardId}/columns
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: boardId
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Column
      - Assigns
      - It
      - To
      - Given
      - Board
  /rest/boards/{boardId}/columns/{columnId}:
    delete:
      summary: Deletes a specific column.
      description: Deletes a specific column..
      operationId: deleteRestBoardsBoardColumnsColumn
      x-api-path-slug: restboardsboardidcolumnscolumnid-delete
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Column
    post:
      summary: Copies a specific column.
      description: Copies a specific column..
      operationId: postRestBoardsBoardColumnsColumn
      x-api-path-slug: restboardsboardidcolumnscolumnid-post
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      responses:
        200:
          description: OK
      tags:
      - Copies
      - Specific
      - Column
    put:
      summary: Updates a specific column.
      description: Updates a specific column..
      operationId: putRestBoardsBoardColumnsColumn
      x-api-path-slug: restboardsboardidcolumnscolumnid-put
      parameters:
      - in: body
        name: /rest/boards/{boardId}/columns/{columnId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: boardId
      - in: path
        name: columnId
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Column
  /rest/boards/{boardId}/columns/{columnId}/position:
    put:
      summary: Updates the position of a specific column. Also updates the positions
        of all following columns on the same board.
      description: Updates the position of a specific column. also updates the positions
        of all following columns on the same board..
      operationId: putRestBoardsBoardColumnsColumnPosition
      x-api-path-slug: restboardsboardidcolumnscolumnidposition-put
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: query
        name: position
      responses:
        200:
          description: OK
      tags:
      - S
      - Position
      - Of
      - Specific
      - Column
      - ""
      - Also
      - Updates
      - Positions
      - Of
      - ""
      - Following
      - Columns
      - "On"
      - Same
      - Board
  /rest/boards/{boardId}/columns/{columnId}/tasks:
    get:
      summary: Lists all tasks for a given column.
      description: Lists all tasks for a given column..
      operationId: getRestBoardsBoardColumnsColumnTasks
      x-api-path-slug: restboardsboardidcolumnscolumnidtasks-get
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: query
        name: startAt
        description: Position of a task to start listing at
      - in: query
        name: tasksPerPage
        description: Number of tasks to list per page
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Tasksa
      - Given
      - Column
    post:
      summary: Creates a new tasks on a specified column.
      description: Creates a new tasks on a specified column..
      operationId: postRestBoardsBoardColumnsColumnTasks
      x-api-path-slug: restboardsboardidcolumnscolumnidtasks-post
      parameters:
      - in: body
        name: /rest/boards/{boardId}/columns/{columnId}/tasks
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: boardId
      - in: path
        name: columnId
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Tasks
      - "On"
      - Specified
      - Column
  /rest/boards/{boardId}/columns/{columnId}/tasks/{taskId}:
    delete:
      summary: Deletes a task.
      description: Deletes a task..
      operationId: deleteRestBoardsBoardColumnsColumnTasksTask
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskid-delete
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - S
      - Task
    get:
      summary: Gets a task by its ID.
      description: Gets a task by its id..
      operationId: getRestBoardsBoardColumnsColumnTasksTask
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskid-get
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - S
      - Task
      - By
      - Its
      - ID
    post:
      summary: Copies a specific task.
      description: Copies a specific task..
      operationId: postRestBoardsBoardColumnsColumnTasksTask
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskid-post
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Copies
      - Specific
      - Task
    put:
      summary: Updates a task.
      description: Updates a task..
      operationId: putRestBoardsBoardColumnsColumnTasksTask
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskid-put
      parameters:
      - in: body
        name: /rest/boards/{boardId}/columns/{columnId}/tasks/{taskId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - S
      - Task
  /rest/boards/{boardId}/columns/{columnId}/tasks/{taskId}/position:
    put:
      summary: Updates the position of a task.
      description: Updates the position of a task..
      operationId: putRestBoardsBoardColumnsColumnTasksTaskPosition
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskidposition-put
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: query
        name: position
        description: The new position of the task
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - S
      - Position
      - Of
      - Task
  /rest/boards/{boardId}/columns/{columnId}/tasks/{taskId}/references:
    post:
      summary: Creates a new reference from a given task to a contact or a ticket.
      description: Creates a new reference from a given task to a contact or a ticket..
      operationId: postRestBoardsBoardColumnsColumnTasksTaskReferences
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskidreferences-post
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: query
        name: referenceValue
        description: Reference type followed by foreign ID of the referenced object
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Reference
      - From
      - Given
      - Task
      - To
      - Contact
      - Ticket
  /rest/boards/{boardId}/columns/{columnId}/tasks/{taskId}/references/{referenceId}:
    delete:
      summary: Deletes a reference from a given task.
      description: Deletes a reference from a given task..
      operationId: deleteRestBoardsBoardColumnsColumnTasksTaskReferencesReference
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskidreferencesreferenceid-delete
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: path
        name: referenceId
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - S
      - Reference
      - From
      - Given
      - Task
  /rest/boards/{boardId}/columns/{columnId}/tasks/{taskId}/references/{referenceType}/{referenceKey}:
    get:
      summary: ""
      description: .
      operationId: getRestBoardsBoardColumnsColumnTasksTaskReferencesReferencetypeReferencekey
      x-api-path-slug: restboardsboardidcolumnscolumnidtaskstaskidreferencesreferencetypereferencekey-get
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: path
        name: referenceKey
      - in: path
        name: referenceType
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/categories:
    get:
      summary: List categories
      description: List categories.
      operationId: getRestCategories
      x-api-path-slug: restcategories-get
      parameters:
      - in: query
        name: categoryId
        description: The ID of the category
      - in: query
        name: itemsPerPage
        description: The number of results per page
      - in: query
        name: lang
        description: The languages of the category detail information
      - in: query
        name: level
        description: The level of the category
      - in: query
        name: linklist
        description: Filter for the linklist of categories
      - in: query
        name: name
        description: The name of the category
      - in: query
        name: page
        description: The requested page of results
      - in: query
        name: parentId
        description: The unique ID of the parent category
      - in: query
        name: plentyId
        description: The unique plenty ID of the client (store)
      - in: query
        name: type
        description: The category type
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      - in: query
        name: with
        description: Includes the detail information, the active clients (stores)
          list of the category and/or the linked Elmar category for each client
      responses:
        200:
          description: OK
      tags:
      - List
      - Categories
    post:
      summary: Creates new categories
      description: Creates new categories.
      operationId: postRestCategories
      x-api-path-slug: restcategories-post
      parameters:
      - in: body
        name: /rest/categories
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Categories
    put:
      summary: Updates categories
      description: Updates categories.
      operationId: putRestCategories
      x-api-path-slug: restcategories-put
      parameters:
      - in: body
        name: /rest/categories
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - Categories
  /rest/categories/{categoryId}/documents:
    get:
      summary: List documents of a category
      description: Lists the documents of a category. The ID of the category must
        be specified.
      operationId: getRestCategoriesCategoryDocuments
      x-api-path-slug: restcategoriescategoryiddocuments-get
      parameters:
      - in: path
        name: categoryId
      responses:
        200:
          description: OK
      tags:
      - List
      - Documents
      - Of
      - Category
    post:
      summary: Upload category documents
      description: Uploads documents to a category. The ID of the category must be
        specified.
      operationId: postRestCategoriesCategoryDocuments
      x-api-path-slug: restcategoriescategoryiddocuments-post
      parameters:
      - in: body
        name: /rest/categories/{categoryId}/documents
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryId
      - in: query
        name: directoryId
        description: The directory ID
      - in: query
        name: displayDate
        description: The date displayed on the document
      - in: query
        name: documents
        description: The array with the category documents
      - in: query
        name: number
        description: The document number
      - in: query
        name: numberWithPrefix
        description: Number with prefix
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Category
      - Documents
  /rest/categories/{categoryId}/documents/downloads:
    get:
      summary: Download category documents
      description: Downloads the documents of a category as a zip file. The ID of
        the category must be specified.
      operationId: getRestCategoriesCategoryDocumentsDownloads
      x-api-path-slug: restcategoriescategoryiddocumentsdownloads-get
      parameters:
      - in: path
        name: categoryId
      responses:
        200:
          description: OK
      tags:
      - Download
      - Category
      - Documents
  /rest/categories/{categoryId}/documents/{documentId}:
    delete:
      summary: Deletes a category document. The ID of the document must be specified.
      description: Deletes a category document. the id of the document must be specified..
      operationId: deleteRestCategoriesCategoryDocumentsDocument
      x-api-path-slug: restcategoriescategoryiddocumentsdocumentid-delete
      parameters:
      - in: path
        name: categoryId
      - in: path
        name: documentId
      responses:
        200:
          description: OK
      tags:
      - S
      - Category
      - Document
      - ""
      - ID
      - Of
      - Document
      - Must
      - Be
      - Specified
  /rest/categories/{id}:
    delete:
      summary: Deletes a category
      description: Deletes a category. The ID of the category must be specified.
      operationId: deleteRestCategories
      x-api-path-slug: restcategoriesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - S
      - Category
    get:
      summary: List categories
      description: List categories.
      operationId: getRestCategories
      x-api-path-slug: restcategoriesid-get
      parameters:
      - in: query
        name: categoryId
        description: The ID of the category
      - in: path
        name: id
      - in: query
        name: itemsPerPage
        description: The number of results per page
      - in: query
        name: lang
        description: The languages of the category detail information
      - in: query
        name: level
        description: The level of the category
      - in: query
        name: linklist
        description: Filter for the linklist of categories
      - in: query
        name: name
        description: The name of the category
      - in: query
        name: page
        description: The requested page of results
      - in: query
        name: parentId
        description: The unique ID of the parent category
      - in: query
        name: plentyId
        description: The unique plenty ID of the client (store)
      - in: query
        name: type
        description: The category type
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      - in: query
        name: with
        description: Includes the detail information, the active clients (stores)
          list of the category and/or the linked Elmar category for each client
      responses:
        200:
          description: OK
      tags:
      - List
      - Categories
    put:
      summary: Updates one category
      description: Updates an existing category. The ID of the category must be specified.
      operationId: putRestCategories
      x-api-path-slug: restcategoriesid-put
      parameters:
      - in: body
        name: /rest/categories/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - S
      - Category
  /rest/categories/{id}/clients:
    delete:
      summary: Deactivate availability for clients
      description: Deactivate availability for clients.
      operationId: deleteRestCategoriesClients
      x-api-path-slug: restcategoriesidclients-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Availabilityclients
  /rest/categories/{id}/details:
    delete:
      summary: Delete category details for the specified languages
      description: Delete category details for the specified languages.
      operationId: deleteRestCategoriesDetails
      x-api-path-slug: restcategoriesiddetails-delete
      parameters:
      - in: body
        name: /rest/categories/{id}/details
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Category
      - Detailsthe
      - Specified
      - Languages
  /rest/categories/{id}/templates:
    delete:
      summary: Delete a category template
      description: Deletes a category template. The ID of the category, the plenty
        ID of the client (store) and the language must be specified.
      operationId: deleteRestCategoriesTemplates
      x-api-path-slug: restcategoriesidtemplates-delete
      parameters:
      - in: body
        name: /rest/categories/{id}/templates
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Category
      - Template
    get:
      summary: Get a category template
      description: Gets a category template. The ID of the category, the plenty ID
        of the client (store) and the language must be specified.
      operationId: getRestCategoriesTemplates
      x-api-path-slug: restcategoriesidtemplates-get
      parameters:
      - in: body
        name: /rest/categories/{id}/templates
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: query
        name: lang
        description: The language of the template
      - in: query
        name: plentyId
        description: The unique plenty ID of the client (store)
      responses:
        200:
          description: OK
      tags:
      - Category
      - Template
    put:
      summary: Update a category template
      description: Updates a category template. The ID of the category, the plenty
        ID of the client (store) and the language must be specified.
      operationId: putRestCategoriesTemplates
      x-api-path-slug: restcategoriesidtemplates-put
      parameters:
      - in: body
        name: /rest/categories/{id}/templates
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Category
      - Template
  /rest/category_branches:
    get:
      summary: Get category trees
      description: Get category trees.
      operationId: getRestCategoryBranches
      x-api-path-slug: restcategory-branches-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of results per page
      - in: query
        name: page
        description: The requested page of results
      - in: query
        name: type
        description: The category type
      responses:
        200:
          description: OK
      tags:
      - Category
      - Trees
  /rest/category_branches/{id}:
    get:
      summary: Get category tree
      description: Gets the category tree of a category. The ID of the category must
        be specified.
      operationId: getRestCategoryBranches
      x-api-path-slug: restcategory-branchesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Category
      - Tree
  /rest/comments:
    post:
      summary: Create a comment
      description: Creates a comment.
      operationId: postRestComments
      x-api-path-slug: restcomments-post
      parameters:
      - in: body
        name: /rest/comments
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Comment
  /rest/comments/{commentId}:
    delete:
      summary: Delete a comment
      description: Deletes a comment. The ID of the comment must be specified.
      operationId: deleteRestCommentsComment
      x-api-path-slug: restcommentscommentid-delete
      parameters:
      - in: path
        name: commentId
      responses:
        200:
          description: OK
      tags:
      - Comment
    get:
      summary: Get a comment
      description: Gets a comment. The ID of the comment must be specified.
      operationId: getRestCommentsComment
      x-api-path-slug: restcommentscommentid-get
      parameters:
      - in: path
        name: commentId
      responses:
        200:
          description: OK
      tags:
      - Comment
    put:
      summary: ""
      description: .
      operationId: putRestCommentsComment
      x-api-path-slug: restcommentscommentid-put
      parameters:
      - in: path
        name: commentId
      - in: query
        name: isVisibleForContact
        description: If true, the comment is visible for the associated contact
      - in: query
        name: referenceType
        description: The reference type
      - in: query
        name: referenceValue
        description: The reference value
      - in: query
        name: userId
        description: The ID of the user the comment belongs to
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/comments/{referenceType}/{referenceValue}:
    get:
      summary: List comments
      description: Lists comments. The reference type and the reference value must
        be specified (e.g. the reference type is 'order' and the reference value is
        the ID of the order).
      operationId: getRestCommentsReferencetypeReferencevalue
      x-api-path-slug: restcommentsreferencetypereferencevalue-get
      parameters:
      - in: query
        name: isVisibleForContact
        description: If true, the comment is visible for the associated contact
      - in: path
        name: referenceType
      - in: path
        name: referenceValue
      - in: query
        name: userId
        description: The ID of the user the comment belongs to
      responses:
        200:
          description: OK
      tags:
      - List
      - Comments
  /rest/customer_contracts:
    get:
      summary: List contracts
      description: List contracts.
      operationId: getRestCustomerContracts
      x-api-path-slug: restcustomer-contracts-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Contracts
    post:
      summary: Creates a new contract
      description: Creates a new contract.
      operationId: postRestCustomerContracts
      x-api-path-slug: restcustomer-contracts-post
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Contract
  /rest/customer_contracts/{contractId}:
    get:
      summary: Returns a single contract
      description: Returns a single contract.
      operationId: getRestCustomerContractsContract
      x-api-path-slug: restcustomer-contractscontractid-get
      parameters:
      - in: path
        name: contractId
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Single
      - Contract
  /rest/customer_contracts/{contractId}/document:
    get:
      summary: Starts download of contract document
      description: Starts download of contract document.
      operationId: getRestCustomerContractsContractDocument
      x-api-path-slug: restcustomer-contractscontractiddocument-get
      parameters:
      - in: path
        name: contractId
      responses:
        200:
          description: OK
      tags:
      - Starts
      - Download
      - Of
      - Contract
      - Document
  /rest/customer_contracts/{contractId}/sign:
    get:
      summary: Returns signing of a contract
      description: Returns signing of a contract.
      operationId: getRestCustomerContractsContractSign
      x-api-path-slug: restcustomer-contractscontractidsign-get
      parameters:
      - in: path
        name: contractId
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Signing
      - Of
      - Contract
    post:
      summary: Sign a contract
      description: Sign a contract.
      operationId: postRestCustomerContractsContractSign
      x-api-path-slug: restcustomer-contractscontractidsign-post
      parameters:
      - in: path
        name: contractId
      responses:
        200:
          description: OK
      tags:
      - Sign
      - Contract
  /rest/customer_contracts/{contractId}/sign/document:
    get:
      summary: Starts download of signed contract document
      description: Starts download of signed contract document.
      operationId: getRestCustomerContractsContractSignDocument
      x-api-path-slug: restcustomer-contractscontractidsigndocument-get
      parameters:
      - in: path
        name: contractId
      responses:
        200:
          description: OK
      tags:
      - Starts
      - Download
      - Of
      - Signed
      - Contract
      - Document
  /rest/delete_log:
    get:
      summary: Search the delete log
      description: Searches the delete log.
      operationId: getRestDeleteLog
      x-api-path-slug: restdelete-log-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referenceType
        description: The type of deleted record
      - in: query
        name: updatedBetween
        description: Filter restricts the list of results to deleteLogs updated during
          the specified period
      - in: query
        name: userId
        description: The ID of the user who deleted the record
      responses:
        200:
          description: OK
      tags:
      - Search
      - Delete
      - Log
  /rest/documents/{documentId}:
    get:
      summary: Download the content of a document
      description: Downloads the content of a document. The ID of the document must
        be specified.
      operationId: getRestDocumentsDocument
      x-api-path-slug: restdocumentsdocumentid-get
      parameters:
      - in: path
        name: documentId
      responses:
        200:
          description: OK
      tags:
      - Download
      - Content
      - Of
      - Document
  /rest/exports:
    get:
      summary: List elastic exports
      description: Lists elastic exports.
      operationId: getRestExports
      x-api-path-slug: restexports-get
      parameters:
      - in: query
        name: formatKey
        description: The format of the export
      - in: query
        name: id
        description: The ID of the export
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: name
        description: The name of the export
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: type
        description: The type of the export
      responses:
        200:
          description: OK
      tags:
      - List
      - Elastic
      - Exports
    post:
      summary: Create an export
      description: Creates an export.
      operationId: postRestExports
      x-api-path-slug: restexports-post
      parameters:
      - in: body
        name: /rest/exports
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Export
  /rest/exports/format_keys:
    get:
      summary: Get format keys
      description: Shows all format keys registered by plugins in production state
      operationId: getRestExportsFormatKeys
      x-api-path-slug: restexportsformat-keys-get
      responses:
        200:
          description: OK
      tags:
      - Format
      - Keys
  /rest/exports/format_keys/{type}:
    get:
      summary: Get format keys
      description: Shows all format keys registered by plugins in production state
      operationId: getRestExportsFormatKeysType
      x-api-path-slug: restexportsformat-keystype-get
      parameters:
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Format
      - Keys
  /rest/exports/generate_token:
    get:
      summary: Generate a token
      description: Creates a new token which can be used as <code>OutputParam</code>
        entry.
      operationId: getRestExportsGenerateToken
      x-api-path-slug: restexportsgenerate-token-get
      responses:
        200:
          description: OK
      tags:
      - Generate
      - Token
  /rest/exports/{exportId}:
    delete:
      summary: Delete export
      description: Deletes an export. The ID of the export must be specified.
      operationId: deleteRestExportsExport
      x-api-path-slug: restexportsexportid-delete
      parameters:
      - in: path
        name: exportId
      responses:
        200:
          description: OK
      tags:
      - Export
    get:
      summary: Get export
      description: Gets detailed information about an export. The ID of the export
        must be specified.
      operationId: getRestExportsExport
      x-api-path-slug: restexportsexportid-get
      parameters:
      - in: path
        name: exportId
      responses:
        200:
          description: OK
      tags:
      - Export
    put:
      summary: Update an export
      description: Updates an export. The ID of the export must be specified.
      operationId: putRestExportsExport
      x-api-path-slug: restexportsexportid-put
      parameters:
      - in: body
        name: /rest/exports/{exportId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: exportId
      responses:
        200:
          description: OK
      tags:
      - Export
  /rest/exports/{exportId}/filters/{filterId}:
    delete:
      summary: ""
      description: .
      operationId: deleteRestExportsExportFiltersFilter
      x-api-path-slug: restexportsexportidfiltersfilterid-delete
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/exports/{exportId}/filters/{key}:
    delete:
      summary: ""
      description: .
      operationId: deleteRestExportsExportFiltersKey
      x-api-path-slug: restexportsexportidfilterskey-delete
      parameters:
      - in: path
        name: exportId
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/feedbacks/comment:
    post:
      summary: Create a feedback comment
      description: Creates a feedback comment.
      operationId: postRestFeedbacksComment
      x-api-path-slug: restfeedbackscomment-post
      parameters:
      - in: query
        name: commentRelationTargetId
        description: The ID of the comments target
      - in: query
        name: commentRelationTargetTypeId
        description: The type ID of the comments target
      - in: query
        name: message
        description: Feedback comment message
      responses:
        200:
          description: OK
      tags:
      - Feedback
      - Comment
  /rest/feedbacks/comment/{commentId}:
    delete:
      summary: Delete a feedback comment
      description: Deletes a feedback comment. The ID of the feedback comment must
        be specified.
      operationId: deleteRestFeedbacksCommentComment
      x-api-path-slug: restfeedbackscommentcommentid-delete
      parameters:
      - in: path
        name: commentId
      - in: query
        name: feedbackCommentId
        description: The ID of the feedback comment
      responses:
        200:
          description: OK
      tags:
      - Feedback
      - Comment
    get:
      summary: Get a feedback comment
      description: Gets a feedback comment. The ID of the feedback comment must be
        specified.
      operationId: getRestFeedbacksCommentComment
      x-api-path-slug: restfeedbackscommentcommentid-get
      parameters:
      - in: path
        name: commentId
      - in: query
        name: feedbackCommentId
        description: The ID of the feedback comment
      responses:
        200:
          description: OK
      tags:
      - Feedback
      - Comment
    put:
      summary: ""
      description: .
      operationId: putRestFeedbacksCommentComment
      x-api-path-slug: restfeedbackscommentcommentid-put
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/feedbacks/comments:
    get:
      summary: List feedback comments
      description: Lists feedback comments.
      operationId: getRestFeedbacksComments
      x-api-path-slug: restfeedbackscomments-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Feedback
      - Comments
  /rest/feedbacks/delete_feedbacks/{feedbackIds}:
    delete:
      summary: Delete multiple feedbacks
      description: Deletes multiple feedbacks. A list with IDs of feedbacks must be
        specified.
      operationId: deleteRestFeedbacksDeleteFeedbacksFeedbacks
      x-api-path-slug: restfeedbacksdelete-feedbacksfeedbackids-delete
      parameters:
      - in: path
        name: feedbackIds
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Feedbacks
  /rest/feedbacks/feedback:
    post:
      summary: Create a feedback
      description: Creates a feedback.
      operationId: postRestFeedbacksFeedback
      x-api-path-slug: restfeedbacksfeedback-post
      parameters:
      - in: query
        name: feedbackRelationSourceTypeId
        description: The type ID of the feedbacks source
      - in: query
        name: feedbackRelationTargetId
        description: The ID of the feedbacks target
      - in: query
        name: feedbackRelationTargetTypeId
        description: The type ID of the feedbacks target
      - in: query
        name: title
        description: Feedback title
      responses:
        200:
          description: OK
      tags:
      - Feedback
  /rest/feedbacks/feedback/replies/{feedbackId}:
    get:
      summary: List feedback replies
      description: Lists feedback replies. The ID of the feedback must be specified.
      operationId: getRestFeedbacksFeedbackRepliesFeedback
      x-api-path-slug: restfeedbacksfeedbackrepliesfeedbackid-get
      parameters:
      - in: path
        name: feedbackId
      responses:
        200:
          description: OK
      tags:
      - List
      - Feedback
      - Replies
  /rest/feedbacks/feedback/{feedbackId}:
    delete:
      summary: Delete a feedback
      description: Deletes a feedback. The ID of the feedback must be specified.
      operationId: deleteRestFeedbacksFeedbackFeedback
      x-api-path-slug: restfeedbacksfeedbackfeedbackid-delete
      parameters:
      - in: path
        name: feedbackId
      responses:
        200:
          description: OK
      tags:
      - Feedback
    get:
      summary: Get a feedback
      description: Gets a feedback. The ID of the feedback must be specified.
      operationId: getRestFeedbacksFeedbackFeedback
      x-api-path-slug: restfeedbacksfeedbackfeedbackid-get
      parameters:
      - in: path
        name: feedbackId
      responses:
        200:
          description: OK
      tags:
      - Feedback
    put:
      summary: Update a feedback
      description: Updates a feedback. The ID of the feedback must be specified.
      operationId: putRestFeedbacksFeedbackFeedback
      x-api-path-slug: restfeedbacksfeedbackfeedbackid-put
      parameters:
      - in: path
        name: feedbackId
      responses:
        200:
          description: OK
      tags:
      - Feedback
  /rest/feedbacks/feedbacks:
    get:
      summary: List feedbacks
      description: Lists feedbacks. The reference type and the reference value must
        be specified (e.g. the reference type is 'order' and the reference value is
        the ID of the order).
      operationId: getRestFeedbacksFeedbacks
      x-api-path-slug: restfeedbacksfeedbacks-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Feedbacks
  /rest/feedbacks/feedbacks_visibility:
    put:
      summary: Update the visibility of multiple feedbacks
      description: Updates the visibility of multiple feedbacks. A list with IDs of
        feedbacks must be specified.
      operationId: putRestFeedbacksFeedbacksVisibility
      x-api-path-slug: restfeedbacksfeedbacks-visibility-put
      parameters:
      - in: query
        name: feedbackIds
        description: The list of feedback IDs, separated by commas
      - in: query
        name: isVisible
        description: The visibility value
      responses:
        200:
          description: OK
      tags:
      - Visibility
      - Of
      - Multiple
      - Feedbacks
  /rest/feedbacks/migrate:
    post:
      summary: Migrate legacy feedbacks
      description: Migrate legacy feedbacks.
      operationId: postRestFeedbacksMigrate
      x-api-path-slug: restfeedbacksmigrate-post
      responses:
        200:
          description: OK
      tags:
      - Migrate
      - Legacy
      - Feedbacks
  /rest/feedbacks/rating:
    post:
      summary: Create a feedback rating
      description: Creates a feedback rating.
      operationId: postRestFeedbacksRating
      x-api-path-slug: restfeedbacksrating-post
      parameters:
      - in: query
        name: ratingRelationTargetId
        description: The ID of the ratings target
      - in: query
        name: ratingRelationTargetTypeId
        description: The type ID of the ratings target
      - in: query
        name: ratingValue
        description: The feedbacks comment message
      responses:
        200:
          description: OK
      tags:
      - Feedback
      - Rating
  /rest/feedbacks/rating/{ratingId}:
    delete:
      summary: Delete a feedback rating
      description: Deletes a feedback rating. The ID of the feedback rating must be
        specified.
      operationId: deleteRestFeedbacksRatingRating
      x-api-path-slug: restfeedbacksratingratingid-delete
      parameters:
      - in: query
        name: feedbackRatingId
        description: The ID of the feedback rating
      - in: path
        name: ratingId
      responses:
        200:
          description: OK
      tags:
      - Feedback
      - Rating
    get:
      summary: Get a feedback rating
      description: Gets a feedback rating. The ID of the feedback rating must be specified.
      operationId: getRestFeedbacksRatingRating
      x-api-path-slug: restfeedbacksratingratingid-get
      parameters:
      - in: query
        name: feedbackRatingId
        description: The ID of the feedback rating
      - in: path
        name: ratingId
      responses:
        200:
          description: OK
      tags:
      - Feedback
      - Rating
    put:
      summary: ""
      description: .
      operationId: putRestFeedbacksRatingRating
      x-api-path-slug: restfeedbacksratingratingid-put
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/feedbacks/ratings:
    get:
      summary: List feedback ratings
      description: Lists feedback ratings.
      operationId: getRestFeedbacksRatings
      x-api-path-slug: restfeedbacksratings-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Feedback
      - Ratings
  /rest/item_sets:
    delete:
      summary: Delete item sets
      description: Delete item sets.
      operationId: deleteRestItemSets
      x-api-path-slug: restitem-sets-delete
      responses:
        200:
          description: OK
      tags:
      - Item
      - Sets
    get:
      summary: List item sets
      description: Lists all item sets.
      operationId: getRestItemSets
      x-api-path-slug: restitem-sets-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Sets
    post:
      summary: Create item sets
      description: Create item sets.
      operationId: postRestItemSets
      x-api-path-slug: restitem-sets-post
      parameters:
      - in: query
        name: params
        description: includes the item sets that have to be created
      responses:
        200:
          description: OK
      tags:
      - Item
      - Sets
    put:
      summary: Update item sets
      description: Update item sets.
      operationId: putRestItemSets
      x-api-path-slug: restitem-sets-put
      responses:
        200:
          description: OK
      tags:
      - Item
      - Sets
  /rest/item_sets/{id}:
    delete:
      summary: Delete an item set
      description: Deletes an item set. The item ID of the item set must be specified.
      operationId: deleteRestItemSets
      x-api-path-slug: restitem-setsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
    get:
      summary: Get an item set
      description: Gets the configuration of an item set. The item ID of the item
        set must be specified.
      operationId: getRestItemSets
      x-api-path-slug: restitem-setsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
    put:
      summary: Update an item set
      description: Updates an item set. The item ID of the item set must be specified.
      operationId: putRestItemSets
      x-api-path-slug: restitem-setsid-put
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
  /rest/item_sets/{setId}/components:
    delete:
      summary: Delete item set components
      description: Delete item set components.
      operationId: deleteRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponents-delete
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Components
    get:
      summary: List item set components of an item set
      description: Lists the item set components of an item set. The ID of the item
        set must be specified.
      operationId: getRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponents-get
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Set
      - Components
      - Of
      - Item
      - Set
    post:
      summary: Create item set components
      description: Create item set components.
      operationId: postRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponents-post
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Components
    put:
      summary: Update item set components
      description: Update item set components.
      operationId: putRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponents-put
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Components
  /rest/item_sets/{setId}/components/{id}:
    delete:
      summary: Delete an item set component
      description: Deletes an item set component. The item set component ID of the
        item set component must be specified.
      operationId: deleteRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponentsid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Component
    get:
      summary: Get an item set component
      description: Get an item set component.
      operationId: getRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponentsid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Component
    put:
      summary: Update an item set component
      description: Update an item set component.
      operationId: putRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponentsid-put
      parameters:
      - in: path
        name: id
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Component
  /rest/item_sets/{setId}/config:
    get:
      summary: Get the item set configuration of an item set
      description: Get the item set configuration of an item set.
      operationId: getRestItemSetsSetConfig
      x-api-path-slug: restitem-setssetidconfig-get
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Configuration
      - Of
      - Item
      - Set
    put:
      summary: Update an item set configuration
      description: Update an item set configuration.
      operationId: putRestItemSetsSetConfig
      x-api-path-slug: restitem-setssetidconfig-put
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Item
      - Set
      - Configuration
  /rest/items:
    get:
      summary: Search item
      description: Search item.
      operationId: getRestItems
      x-api-path-slug: restitems-get
      parameters:
      - in: query
        name: flagOne
        description: Filter restricts the list of results to items with the specified
          flagOne
      - in: query
        name: flagTwo
        description: Filter restricts the list of results to items with the specified
          flagTwo
      - in: query
        name: itemsPerPage
        description: Limits the number of results listed per page to a specific number
      - in: query
        name: lang
        description: The language of the variation information
      - in: query
        name: manufacturerId
        description: Filter restricts the list of results to items with the specified
          manufacturerId
      - in: query
        name: name
        description: Filter restricts the list of results to items with the specified
          item name
      - in: query
        name: page
        description: Limits the results to a specific page
      - in: query
        name: tagId
        description: Filter restricts the list of results to items with the specified
          tagId
      - in: query
        name: updatedBetween
        description: Filter restricts the list of results to items updated during
          the specified period
      - in: query
        name: variationRelatedUpdatedBetween
        description: Filter restricts the list of results to items with variations
          for which related information was updated during the specified period
      - in: query
        name: variationUpdatedBetween
        description: Filter restricts the list of results to items with variations
          that were updated during the specified period
      - in: query
        name: with
        description: Includes the specified variation information in the results
      responses:
        200:
          description: OK
      tags:
      - Search
      - Item
    post:
      summary: Create new item
      description: Create new item.
      operationId: postRestItems
      x-api-path-slug: restitems-post
      parameters:
      - in: body
        name: /rest/items
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Item
  /rest/items/attribute_values/{valueId}/names:
    get:
      summary: Get name and language for an attribute value ID
      description: Gets name and language for an attribute value ID. The attribute
        value ID must be specified.
      operationId: getRestItemsAttributeValuesValueNames
      x-api-path-slug: restitemsattribute-valuesvalueidnames-get
      parameters:
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Name
      - Languagean
      - Attribute
      - Value
      - ID
    post:
      summary: Create an attribute value name
      description: Creates an attribute value name.
      operationId: postRestItemsAttributeValuesValueNames
      x-api-path-slug: restitemsattribute-valuesvalueidnames-post
      parameters:
      - in: body
        name: /rest/items/attribute_values/{valueId}/names
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Name
  /rest/items/attribute_values/{valueId}/names/{lang}:
    delete:
      summary: Delete an attribute value name
      description: Deletes an attribute value name. The attribute value ID and language
        must be specified.
      operationId: deleteRestItemsAttributeValuesValueNamesLang
      x-api-path-slug: restitemsattribute-valuesvalueidnameslang-delete
      parameters:
      - in: path
        name: lang
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Name
    get:
      summary: Get an attribute value name
      description: Gets the attribute value name. The attribute value ID and language
        must be specified.
      operationId: getRestItemsAttributeValuesValueNamesLang
      x-api-path-slug: restitemsattribute-valuesvalueidnameslang-get
      parameters:
      - in: path
        name: lang
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Name
    put:
      summary: Update an attribute value name
      description: Updates an attribute value name.
      operationId: putRestItemsAttributeValuesValueNamesLang
      x-api-path-slug: restitemsattribute-valuesvalueidnameslang-put
      parameters:
      - in: body
        name: /rest/items/attribute_values/{valueId}/names/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lang
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Name
  /rest/items/attributes:
    get:
      summary: List attributes
      description: Lists all attributes.
      operationId: getRestItemsAttributes
      x-api-path-slug: restitemsattributes-get
      parameters:
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      - in: query
        name: with
        description: Includes the specified attribute information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Attributes
    post:
      summary: Create an attribute
      description: Creates an attribute.
      operationId: postRestItemsAttributes
      x-api-path-slug: restitemsattributes-post
      parameters:
      - in: body
        name: /rest/items/attributes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Attribute
  /rest/items/attributes/maps:
    get:
      summary: Lists all attribute maps.
      description: Lists all attribute maps..
      operationId: getRestItemsAttributesMaps
      x-api-path-slug: restitemsattributesmaps-get
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Attribute
      - Maps
  /rest/items/attributes/markets/maps:
    post:
      summary: Creates a new attribute map.
      description: Creates a new attribute map..
      operationId: postRestItemsAttributesMarketsMaps
      x-api-path-slug: restitemsattributesmarketsmaps-post
      parameters:
      - in: body
        name: /rest/items/attributes/markets/maps
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Attribute
      - Map
  /rest/items/attributes/values/maps:
    get:
      summary: Lists all attribute value maps.
      description: Lists all attribute value maps..
      operationId: getRestItemsAttributesValuesMaps
      x-api-path-slug: restitemsattributesvaluesmaps-get
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Attribute
      - Value
      - Maps
  /rest/items/attributes/values/markets/maps:
    post:
      summary: Creates a new attribute value map.
      description: Creates a new attribute value map..
      operationId: postRestItemsAttributesValuesMarketsMaps
      x-api-path-slug: restitemsattributesvaluesmarketsmaps-post
      parameters:
      - in: body
        name: /rest/items/attributes/values/markets/maps
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Attribute
      - Value
      - Map
  /rest/items/attributes/{attributeId}/markets/{marketId}/maps:
    delete:
      summary: Deletes an attribute map.
      description: Deletes an attribute map. The ID of the attribute and the ID of
        the market must be specified.
      operationId: deleteRestItemsAttributesAttributeMarketsMarketMaps
      x-api-path-slug: restitemsattributesattributeidmarketsmarketidmaps-delete
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - S
      - Attribute
      - Map
    get:
      summary: Gets an attribute map.
      description: Gets an attribute map. The ID of the attribute and the ID of the
        market must be specified.
      operationId: getRestItemsAttributesAttributeMarketsMarketMaps
      x-api-path-slug: restitemsattributesattributeidmarketsmarketidmaps-get
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - S
      - Attribute
      - Map
    put:
      summary: Updates an attribute map.
      description: Updates an attribute map. The ID of the attribute and the ID of
        the market must be specified.
      operationId: putRestItemsAttributesAttributeMarketsMarketMaps
      x-api-path-slug: restitemsattributesattributeidmarketsmarketidmaps-put
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - S
      - Attribute
      - Map
  /rest/items/attributes/{attributeId}/names:
    get:
      summary: Get an attribute name
      description: Gets the attribute name in the specified language. The language
        code must be specified.
      operationId: getRestItemsAttributesAttributeNames
      x-api-path-slug: restitemsattributesattributeidnames-get
      parameters:
      - in: path
        name: attributeId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Name
    post:
      summary: Create an attribute name
      description: Creates an attribute name in the specified language. The language
        code must be specified.
      operationId: postRestItemsAttributesAttributeNames
      x-api-path-slug: restitemsattributesattributeidnames-post
      parameters:
      - in: body
        name: /rest/items/attributes/{attributeId}/names
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: attributeId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Name
  /rest/items/attributes/{attributeId}/names/{lang}:
    delete:
      summary: Delete an attribute name
      description: Deletes the attribute name in the specified language. The language
        code and attribute name must be specified.
      operationId: deleteRestItemsAttributesAttributeNamesLang
      x-api-path-slug: restitemsattributesattributeidnameslang-delete
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Name
    get:
      summary: List attribute names
      description: Lists the attribute names of an attribute.
      operationId: getRestItemsAttributesAttributeNamesLang
      x-api-path-slug: restitemsattributesattributeidnameslang-get
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - List
      - Attribute
      - Names
    put:
      summary: Update an attribute name
      description: Updates the attribute name in the specified language. The language
        code and attribute name must be specified.
      operationId: putRestItemsAttributesAttributeNamesLang
      x-api-path-slug: restitemsattributesattributeidnameslang-put
      parameters:
      - in: body
        name: /rest/items/attributes/{attributeId}/names/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: attributeId
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Name
  /rest/items/attributes/{attributeId}/value_market_names:
    get:
      summary: Search attribute value market names
      description: Search attribute value market names.
      operationId: getRestItemsAttributesAttributeValueMarketNames
      x-api-path-slug: restitemsattributesattributeidvalue-market-names-get
      parameters:
      - in: path
        name: attributeId
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: lang
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referenceType
      responses:
        200:
          description: OK
      tags:
      - Search
      - Attribute
      - Value
      - Market
      - Names
    post:
      summary: Create an attribute value market name
      description: Creates an attribute value market name.
      operationId: postRestItemsAttributesAttributeValueMarketNames
      x-api-path-slug: restitemsattributesattributeidvalue-market-names-post
      parameters:
      - in: body
        name: /rest/items/attributes/{attributeId}/value_market_names
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: attributeId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Market
      - Name
  /rest/items/attributes/{attributeId}/value_market_names/{valueId}/{lang}/{referenceType}:
    delete:
      summary: Delete an attribute value market name
      description: Deletes an attribute value market name. The attribute value ID
        and language must be specified.
      operationId: deleteRestItemsAttributesAttributeValueMarketNamesValueLangReferencetype
      x-api-path-slug: restitemsattributesattributeidvalue-market-namesvalueidlangreferencetype-delete
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: lang
      - in: path
        name: referenceType
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Market
      - Name
    put:
      summary: Update an attribute value market name
      description: Updates an attribute value market name. The attribute value ID
        and language must be specified.
      operationId: putRestItemsAttributesAttributeValueMarketNamesValueLangReferencetype
      x-api-path-slug: restitemsattributesattributeidvalue-market-namesvalueidlangreferencetype-put
      parameters:
      - in: body
        name: /rest/items/attributes/{attributeId}/value_market_names/{valueId}/{lang}/{referenceType}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: attributeId
      - in: path
        name: lang
      - in: path
        name: referenceType
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Market
      - Name
  /rest/items/attributes/{attributeId}/values:
    get:
      summary: List attribute values
      description: Lists the attribute values for an attribute. The attribute ID must
        be specified.
      operationId: getRestItemsAttributesAttributeValues
      x-api-path-slug: restitemsattributesattributeidvalues-get
      parameters:
      - in: path
        name: attributeId
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      - in: query
        name: with
        description: Includes the specified attribute value information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Attribute
      - Values
    post:
      summary: Create an attribute value
      description: Creates an attribute value.
      operationId: postRestItemsAttributesAttributeValues
      x-api-path-slug: restitemsattributesattributeidvalues-post
      parameters:
      - in: body
        name: /rest/items/attributes/{attributeId}/values
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: attributeId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
  /rest/items/attributes/{attributeId}/values/{attributeValueId}/markets/{marketId}/maps:
    delete:
      summary: Deletes an attribute value map.
      description: Deletes an attribute value map. The ID of the attribute, the ID
        of the attribute value and the ID of the market must be specified.
      operationId: deleteRestItemsAttributesAttributeValuesAttributevalueMarketsMarketMaps
      x-api-path-slug: restitemsattributesattributeidvaluesattributevalueidmarketsmarketidmaps-delete
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: attributeValueId
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - S
      - Attribute
      - Value
      - Map
    get:
      summary: Gets an attribute value map.
      description: Gets an attribute value map. The ID of the attribute, the ID of
        the attribute value and the ID of the market must be specified.
      operationId: getRestItemsAttributesAttributeValuesAttributevalueMarketsMarketMaps
      x-api-path-slug: restitemsattributesattributeidvaluesattributevalueidmarketsmarketidmaps-get
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: attributeValueId
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - S
      - Attribute
      - Value
      - Map
    put:
      summary: Updates an attribute value map.
      description: Updates an attribute value map. The ID of the attribute, the ID
        of the attribute value and the ID of the market must be specified.
      operationId: putRestItemsAttributesAttributeValuesAttributevalueMarketsMarketMaps
      x-api-path-slug: restitemsattributesattributeidvaluesattributevalueidmarketsmarketidmaps-put
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: attributeValueId
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - S
      - Attribute
      - Value
      - Map
  /rest/items/attributes/{attributeId}/values/{id}:
    delete:
      summary: Delete an attribute value
      description: Deletes an attribute value. The attribute ID must be specified.
      operationId: deleteRestItemsAttributesAttributeValues
      x-api-path-slug: restitemsattributesattributeidvaluesid-delete
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
    get:
      summary: Get an attribute value
      description: Get an attribute value. The ID of the attribute value must be specified.
      operationId: getRestItemsAttributesAttributeValues
      x-api-path-slug: restitemsattributesattributeidvaluesid-get
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: id
      - in: query
        name: with
        description: Includes the specified attribute value information in the results
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
    put:
      summary: Update an attribute value
      description: Updates an attribute value. The attribute value must be specified.
      operationId: putRestItemsAttributesAttributeValues
      x-api-path-slug: restitemsattributesattributeidvaluesid-put
      parameters:
      - in: body
        name: /rest/items/attributes/{attributeId}/values/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: attributeId
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
  /rest/items/attributes/{id}:
    delete:
      summary: Delete an attribute
      description: Deletes an attribute. The ID of the attribute must be specified.
      operationId: deleteRestItemsAttributes
      x-api-path-slug: restitemsattributesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Attribute
    get:
      summary: Get an attribute
      description: Gets an attribute. The ID of the attribute must be specified.
      operationId: getRestItemsAttributes
      x-api-path-slug: restitemsattributesid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: Includes the specified attribute information in the results
      responses:
        200:
          description: OK
      tags:
      - Attribute
    put:
      summary: Update an attribute
      description: Updates an attribute. The ID of the attribute must be specified.
      operationId: putRestItemsAttributes
      x-api-path-slug: restitemsattributesid-put
      parameters:
      - in: body
        name: /rest/items/attributes/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Attribute
  /rest/items/barcodes:
    get:
      summary: List barcodes
      description: Lists all barcodes.
      operationId: getRestItemsBarcodes
      x-api-path-slug: restitemsbarcodes-get
      parameters:
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      responses:
        200:
          description: OK
      tags:
      - List
      - Barcodes
    post:
      summary: Create a barcode
      description: Creates a barcode.
      operationId: postRestItemsBarcodes
      x-api-path-slug: restitemsbarcodes-post
      parameters:
      - in: body
        name: /rest/items/barcodes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Barcode
  /rest/items/barcodes/referrer/{referrerId}:
    get:
      summary: List barcodes by referrer
      description: Lists barcodes linked to the specified referrer. The ID of the
        referrer must be specified.
      operationId: getRestItemsBarcodesReferrerReferrer
      x-api-path-slug: restitemsbarcodesreferrerreferrerid-get
      parameters:
      - in: path
        name: referrerId
      responses:
        200:
          description: OK
      tags:
      - List
      - Barcodes
      - By
      - Referrer
  /rest/items/barcodes/type/{type}:
    get:
      summary: List barcodes by type
      description: Lists all barcodes of a specific type. The type must be specified.
      operationId: getRestItemsBarcodesTypeType
      x-api-path-slug: restitemsbarcodestypetype-get
      parameters:
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - List
      - Barcodes
      - By
      - Type
  /rest/items/barcodes/{barcodeId}:
    delete:
      summary: Delete a barcode
      description: Deletes a barcode. The ID of the barcode must be specified.
      operationId: deleteRestItemsBarcodesBarcode
      x-api-path-slug: restitemsbarcodesbarcodeid-delete
      parameters:
      - in: path
        name: barcodeId
      responses:
        200:
          description: OK
      tags:
      - Barcode
    get:
      summary: Get a barcode
      description: Gets a barcode. The ID of the barcode must be specified.
      operationId: getRestItemsBarcodesBarcode
      x-api-path-slug: restitemsbarcodesbarcodeid-get
      parameters:
      - in: path
        name: barcodeId
      responses:
        200:
          description: OK
      tags:
      - Barcode
    put:
      summary: Update a barcode
      description: Updates a barcode. The ID of the barcode must be specified.
      operationId: putRestItemsBarcodesBarcode
      x-api-path-slug: restitemsbarcodesbarcodeid-put
      parameters:
      - in: body
        name: /rest/items/barcodes/{barcodeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: barcodeId
      responses:
        200:
          description: OK
      tags:
      - Barcode
  /rest/items/barcodes/{barcodeId}/referrer:
    post:
      summary: Activate a referrer
      description: Activate a referrer for a barcode.
      operationId: postRestItemsBarcodesBarcodeReferrer
      x-api-path-slug: restitemsbarcodesbarcodeidreferrer-post
      parameters:
      - in: path
        name: barcodeId
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Referrer
  /rest/items/barcodes/{barcodeId}/referrer/{referrerId}:
    delete:
      summary: Deactivate a referrer
      description: Deactivate a referrer for a barcode. The ID of the barcode and
        the ID of the referrer must be specified.
      operationId: deleteRestItemsBarcodesBarcodeReferrerReferrer
      x-api-path-slug: restitemsbarcodesbarcodeidreferrerreferrerid-delete
      parameters:
      - in: path
        name: barcodeId
      - in: path
        name: referrerId
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Referrer
  /rest/items/item_shipping_profiles:
    get:
      summary: List all shipping profiles of all items
      description: |-
        Lists all shipping profiles of all items. Results can be filtered by the timestamp of the link between items and shipping profiles (eq, lt, lte, gt, gte, between).
        <ul>
        <li>eq = Equal to</li>
        <li>gte = Greater than or equal to</li>
        <li>gt = Greater than</li>
        <li>lte = Less than or equal to</li>
        <li>lt = Less than</li>
        <li>between = Date range</li>
        </ul>
        Example: updated=gt:2018-04-16 16:00:00 returns all items with shipping profiles that were activated after 4pm on the 16th of April 2018.
      operationId: getRestItemsItemShippingProfiles
      x-api-path-slug: restitemsitem-shipping-profiles-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Shipping
      - Profiles
      - Of
      - ""
      - Items
    post:
      summary: Bulk activate shipping profiles
      description: Activates up to 50 shipping profiles for items
      operationId: postRestItemsItemShippingProfiles
      x-api-path-slug: restitemsitem-shipping-profiles-post
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Activate
      - Shipping
      - Profiles
  /rest/items/labels:
    get:
      summary: List item label templates
      description: Lists the ID and name of all item label templates saved in the
        system.
      operationId: getRestItemsLabels
      x-api-path-slug: restitemslabels-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Label
      - Templates
  /rest/items/manufacturers:
    get:
      summary: List manufacturers
      description: |-
        Lists all manufacturers in the system.

        Display a listing of the resource.
      operationId: getRestItemsManufacturers
      x-api-path-slug: restitemsmanufacturers-get
      parameters:
      - in: query
        name: name
        description: Filter restricts the list of results to records with specified
          name
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to records updated after
          the specified date
      responses:
        200:
          description: OK
      tags:
      - List
      - Manufacturers
    post:
      summary: Create a manufacturer
      description: Creates a manufacturer.
      operationId: postRestItemsManufacturers
      x-api-path-slug: restitemsmanufacturers-post
      responses:
        200:
          description: OK
      tags:
      - Manufacturer
  /rest/items/manufacturers/{id}:
    delete:
      summary: Delete a manufacturer
      description: Deletes a manufacturer. The ID of the manufacturer must be specified.
      operationId: deleteRestItemsManufacturers
      x-api-path-slug: restitemsmanufacturersid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Manufacturer
    get:
      summary: Get a manufacturer
      description: Gets a manufacturer. The ID of the manufacturer must be specified.
      operationId: getRestItemsManufacturers
      x-api-path-slug: restitemsmanufacturersid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Manufacturer
    put:
      summary: Update a manufacturer
      description: Updates a manufacturer. The ID of the manufacturer must be specified.
      operationId: putRestItemsManufacturers
      x-api-path-slug: restitemsmanufacturersid-put
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Manufacturer
  /rest/items/manufacturers/{id}/commissions:
    get:
      summary: List commissions
      description: Lists all commissions associated with a manufacturer. The ID of
        the manufacturer must be specified.
      operationId: getRestItemsManufacturersCommissions
      x-api-path-slug: restitemsmanufacturersidcommissions-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Commissions
    post:
      summary: Create a commission
      description: Creates a commission for a manufacturer. The ID of the manufacturer
        must be specified.
      operationId: postRestItemsManufacturersCommissions
      x-api-path-slug: restitemsmanufacturersidcommissions-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Commission
  /rest/items/manufacturers/{id}/commissions/{manufacturerId}:
    delete:
      summary: Delete a commission
      description: Delete a commission. The ID of the commission must be specified.
      operationId: deleteRestItemsManufacturersCommissionsManufacturer
      x-api-path-slug: restitemsmanufacturersidcommissionsmanufacturerid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: manufacturerId
      responses:
        200:
          description: OK
      tags:
      - Commission
    get:
      summary: Get a commission
      description: Gets a commission for a manufacturer. The ID of the commission
        must be specified.
      operationId: getRestItemsManufacturersCommissionsManufacturer
      x-api-path-slug: restitemsmanufacturersidcommissionsmanufacturerid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: manufacturerId
      responses:
        200:
          description: OK
      tags:
      - Commission
    put:
      summary: Update a commission
      description: Updates a commission. The ID of the commission must be specified.
      operationId: putRestItemsManufacturersCommissionsManufacturer
      x-api-path-slug: restitemsmanufacturersidcommissionsmanufacturerid-put
      parameters:
      - in: path
        name: id
      - in: path
        name: manufacturerId
      responses:
        200:
          description: OK
      tags:
      - Commission
  /rest/items/properties:
    get:
      summary: List properties
      description: Lists all properties.
      operationId: getRestItemsProperties
      x-api-path-slug: restitemsproperties-get
      parameters:
      - in: query
        name: groupId
        description: Filter restricts the list of results to items linked to a specified
          property group
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      - in: query
        name: with
        description: Includes the specified property information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
    post:
      summary: Create a property
      description: Creates a property.
      operationId: postRestItemsProperties
      x-api-path-slug: restitemsproperties-post
      parameters:
      - in: body
        name: /rest/items/properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Property
  /rest/items/properties/{id}:
    delete:
      summary: Delete a property
      description: Deletes a property. The ID of the property must be specified.
      operationId: deleteRestItemsProperties
      x-api-path-slug: restitemspropertiesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
    get:
      summary: Get a property
      description: Gets a property. The ID of the property must be specified.
      operationId: getRestItemsProperties
      x-api-path-slug: restitemspropertiesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
    put:
      summary: Update a property
      description: Updates a property. The ID of the property must be specified.
      operationId: putRestItemsProperties
      x-api-path-slug: restitemspropertiesid-put
      parameters:
      - in: body
        name: /rest/items/properties/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
  /rest/items/properties/{id}/market_references:
    get:
      summary: List property market references
      description: Lists the property market references of a property. The ID of the
        property must be specified.
      operationId: getRestItemsPropertiesMarketReferences
      x-api-path-slug: restitemspropertiesidmarket-references-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Market
      - References
    post:
      summary: Create a property market reference
      description: Creates a property market reference.
      operationId: postRestItemsPropertiesMarketReferences
      x-api-path-slug: restitemspropertiesidmarket-references-post
      parameters:
      - in: body
        name: /rest/items/properties/{id}/market_references
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
      - Reference
  /rest/items/properties/{id}/market_references/{marketId}:
    delete:
      summary: Delete a property market reference
      description: Deletes a property market reference. The ID of the property and
        the ID of the market must be specified.
      operationId: deleteRestItemsPropertiesMarketReferencesMarket
      x-api-path-slug: restitemspropertiesidmarket-referencesmarketid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
      - Reference
    get:
      summary: Get a property market reference
      description: Gets a property market reference. The market ID and the property
        ID must be specified.
      operationId: getRestItemsPropertiesMarketReferencesMarket
      x-api-path-slug: restitemspropertiesidmarket-referencesmarketid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
      - Reference
    put:
      summary: Update a property market reference
      description: Updates a property market reference.
      operationId: putRestItemsPropertiesMarketReferencesMarket
      x-api-path-slug: restitemspropertiesidmarket-referencesmarketid-put
      parameters:
      - in: body
        name: /rest/items/properties/{id}/market_references/{marketId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
      - Reference
  /rest/items/properties/{id}/names:
    get:
      summary: List the property names
      description: Lists the names of a property in all languages. The ID of the property
        must be specified.
      operationId: getRestItemsPropertiesNames
      x-api-path-slug: restitemspropertiesidnames-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Names
    post:
      summary: Create a property name
      description: Creates a property name. The ID of the property must be specified.
      operationId: postRestItemsPropertiesNames
      x-api-path-slug: restitemspropertiesidnames-post
      parameters:
      - in: body
        name: /rest/items/properties/{id}/names
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Name
  /rest/items/properties/{id}/names/{lang}:
    delete:
      summary: Delete a property name
      description: Deletes a property name. The ID of the property must be specified.
      operationId: deleteRestItemsPropertiesNamesLang
      x-api-path-slug: restitemspropertiesidnameslang-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Property
      - Name
    get:
      summary: Get a property name
      description: Gets a property name in a specified language. The ID of the property
        and the language code must be specified.
      operationId: getRestItemsPropertiesNamesLang
      x-api-path-slug: restitemspropertiesidnameslang-get
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Property
      - Name
    put:
      summary: Update a property name
      description: Updates a property name. The ID of the property and the language
        code must be specified.
      operationId: putRestItemsPropertiesNamesLang
      x-api-path-slug: restitemspropertiesidnameslang-put
      parameters:
      - in: body
        name: /rest/items/properties/{id}/names/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Property
      - Name
  /rest/items/properties/{propertyId}/selections:
    get:
      summary: List property selections
      description: Lists the property selections of a property. The ID of the property
        must be specified.
      operationId: getRestItemsPropertiesPropertySelections
      x-api-path-slug: restitemspropertiespropertyidselections-get
      parameters:
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Selections
    post:
      summary: Create a property selection
      description: Creates a property selection.
      operationId: postRestItemsPropertiesPropertySelections
      x-api-path-slug: restitemspropertiespropertyidselections-post
      parameters:
      - in: body
        name: /rest/items/properties/{propertyId}/selections
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
  /rest/items/properties/{propertyId}/selections/{id}:
    delete:
      summary: Delete a property selection
      description: Deletes a property selection. The ID of the property must be specified.
      operationId: deleteRestItemsPropertiesPropertySelections
      x-api-path-slug: restitemspropertiespropertyidselectionsid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
    get:
      summary: Get a property selection
      description: Gets a property selection of a property.
      operationId: getRestItemsPropertiesPropertySelections
      x-api-path-slug: restitemspropertiespropertyidselectionsid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
    post:
      summary: Creates a property selection lang
      description: Creates a property selection lang.
      operationId: postRestItemsPropertiesPropertySelections
      x-api-path-slug: restitemspropertiespropertyidselectionsid-post
      parameters:
      - in: body
        name: /rest/items/properties/{propertyId}/selections/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Property
      - Selection
      - Lang
  /rest/items/properties/{propertyId}/selections/{id}/{lang}:
    delete:
      summary: Delete a property selection language
      description: Deletes a property selection language. The ID of the selection
        and the language must be specified.
      operationId: deleteRestItemsPropertiesPropertySelectionsLang
      x-api-path-slug: restitemspropertiespropertyidselectionsidlang-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
      - Language
    get:
      summary: List property selections by language
      description: Lists the property selections of a property for a specific language.
        The ID and language of the property must be specified.
      operationId: getRestItemsPropertiesPropertySelectionsLang
      x-api-path-slug: restitemspropertiespropertyidselectionsidlang-get
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Selections
      - By
      - Language
    put:
      summary: Update a property selection
      description: Updates a property selection.
      operationId: putRestItemsPropertiesPropertySelectionsLang
      x-api-path-slug: restitemspropertiespropertyidselectionsidlang-put
      parameters:
      - in: body
        name: /rest/items/properties/{propertyId}/selections/{id}/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: lang
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
  /rest/items/properties/{propertyId}/selections/{lang}:
    get:
      summary: List property selections
      description: Lists the property selections of a property. The ID of the property
        must be specified.
      operationId: getRestItemsPropertiesPropertySelectionsLang
      x-api-path-slug: restitemspropertiespropertyidselectionslang-get
      parameters:
      - in: path
        name: lang
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Selections
  /rest/items/property_groups:
    get:
      summary: List property groups
      description: Lists the property groups.
      operationId: getRestItemsPropertyGroups
      x-api-path-slug: restitemsproperty-groups-get
      parameters:
      - in: query
        name: with
        description: Includes the specified property group information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Groups
    post:
      summary: Create a property group
      description: Creates a property group.
      operationId: postRestItemsPropertyGroups
      x-api-path-slug: restitemsproperty-groups-post
      parameters:
      - in: body
        name: /rest/items/property_groups
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
  /rest/items/property_groups/{id}:
    delete:
      summary: Delete a property group
      description: Deletes a property group. The ID of the property group must be
        specified.
      operationId: deleteRestItemsPropertyGroups
      x-api-path-slug: restitemsproperty-groupsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
    get:
      summary: Get a property group
      description: Gets a property group. The ID of the property group must be specified.
      operationId: getRestItemsPropertyGroups
      x-api-path-slug: restitemsproperty-groupsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
    put:
      summary: Update a property group
      description: Updates an existing property group.
      operationId: putRestItemsPropertyGroups
      x-api-path-slug: restitemsproperty-groupsid-put
      parameters:
      - in: body
        name: /rest/items/property_groups/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
  /rest/items/property_groups/{id}/names:
    get:
      summary: List the property group names of a property group
      description: Lists the property group names of a property group in all languages.
        The ID of the property group must be specified.
      operationId: getRestItemsPropertyGroupsNames
      x-api-path-slug: restitemsproperty-groupsidnames-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Group
      - Names
      - Of
      - Property
      - Group
    post:
      summary: Create a property group name
      description: Creates a property group name. The ID of the property group must
        be specified.
      operationId: postRestItemsPropertyGroupsNames
      x-api-path-slug: restitemsproperty-groupsidnames-post
      parameters:
      - in: body
        name: /rest/items/property_groups/{id}/names
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
      - Name
  /rest/items/property_groups/{id}/names/{lang}:
    delete:
      summary: Delete a property group name
      description: Deletes a property group name. The ID of the property group must
        be specified.
      operationId: deleteRestItemsPropertyGroupsNamesLang
      x-api-path-slug: restitemsproperty-groupsidnameslang-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
      - Name
    get:
      summary: Get a property group name in a language
      description: Gets a property group name in the specified language. The ID of
        the property group name and the language code must be specified.
      operationId: getRestItemsPropertyGroupsNamesLang
      x-api-path-slug: restitemsproperty-groupsidnameslang-get
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
      - Name
      - In
      - Language
    put:
      summary: Update a property group name
      description: Updates a property group name. The ID of the property group and
        the language must be specified.
      operationId: putRestItemsPropertyGroupsNamesLang
      x-api-path-slug: restitemsproperty-groupsidnameslang-put
      parameters:
      - in: body
        name: /rest/items/property_groups/{id}/names/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
      - Name
  /rest/items/sales_prices:
    get:
      summary: List sales prices
      description: Lists all sales prices.
      operationId: getRestItemsSalesPrices
      x-api-path-slug: restitemssales-prices-get
      parameters:
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      responses:
        200:
          description: OK
      tags:
      - List
      - Sales
      - Prices
    post:
      summary: Create a sales price
      description: Creates a sales price.
      operationId: postRestItemsSalesPrices
      x-api-path-slug: restitemssales-prices-post
      parameters:
      - in: body
        name: /rest/items/sales_prices
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
  /rest/items/sales_prices/{id}:
    delete:
      summary: Delete a sales price
      description: |-
        Deletes a sales price. The ID of the sales price must be specified.

        Delete salesPrice
      operationId: deleteRestItemsSalesPrices
      x-api-path-slug: restitemssales-pricesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
    get:
      summary: Get a sales price
      description: Gets the data for a specific sales price. The ID of the sales price
        must be specified.
      operationId: getRestItemsSalesPrices
      x-api-path-slug: restitemssales-pricesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
    put:
      summary: Update a sales price
      description: Updates a sales price.
      operationId: putRestItemsSalesPrices
      x-api-path-slug: restitemssales-pricesid-put
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
  /rest/items/sales_prices/{id}/accounts:
    get:
      summary: List referrer accounts
      description: Lists all activated referrer accounts of a sales price.
      operationId: getRestItemsSalesPricesAccounts
      x-api-path-slug: restitemssales-pricesidaccounts-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Referrer
      - Accounts
    post:
      summary: Activate a referrer account
      description: Activates a referrer account for a sales price.
      operationId: postRestItemsSalesPricesAccounts
      x-api-path-slug: restitemssales-pricesidaccounts-post
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/accounts
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Referrer
      - Account
  /rest/items/sales_prices/{id}/accounts/{accountType}/{accountId}:
    delete:
      summary: Deactivate a referrer account
      description: Deactivates a referrer account for a sales price.
      operationId: deleteRestItemsSalesPricesAccountsAccounttypeAccount
      x-api-path-slug: restitemssales-pricesidaccountsaccounttypeaccountid-delete
      parameters:
      - in: path
        name: accountId
      - in: path
        name: accountType
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Referrer
      - Account
  /rest/items/sales_prices/{id}/countries:
    get:
      summary: List countries by sales price
      description: Lists active countries for a sales price. The ID of the sales price
        must be specified.
      operationId: getRestItemsSalesPricesCountries
      x-api-path-slug: restitemssales-pricesidcountries-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Countries
      - By
      - Sales
      - Price
    post:
      summary: Activate a country
      description: Activates a country for a sales price.
      operationId: postRestItemsSalesPricesCountries
      x-api-path-slug: restitemssales-pricesidcountries-post
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/countries
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Country
  /rest/items/sales_prices/{id}/countries/{countryId}:
    delete:
      summary: Deactivate a country
      description: Deactivates a country for a sales price.
      operationId: deleteRestItemsSalesPricesCountriesCountry
      x-api-path-slug: restitemssales-pricesidcountriescountryid-delete
      parameters:
      - in: path
        name: countryId
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Country
  /rest/items/sales_prices/{id}/currencies:
    get:
      summary: List activated currencies
      description: List all currencies activated for a sales price. The ID of the
        sales price must be specified.
      operationId: getRestItemsSalesPricesCurrencies
      x-api-path-slug: restitemssales-pricesidcurrencies-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Activated
      - Currencies
    post:
      summary: Activate a currency
      description: Activates a currency for a sales price. The ID of the sales price
        must be specified.
      operationId: postRestItemsSalesPricesCurrencies
      x-api-path-slug: restitemssales-pricesidcurrencies-post
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/currencies
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Currency
  /rest/items/sales_prices/{id}/currencies/{currency}:
    delete:
      summary: Deactivate a currency
      description: Deactivate a currency for a sales price. The ID of the sales price
        and the ISO code of the currency must be specified.
      operationId: deleteRestItemsSalesPricesCurrenciesCurrency
      x-api-path-slug: restitemssales-pricesidcurrenciescurrency-delete
      parameters:
      - in: path
        name: currency
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Currency
  /rest/items/sales_prices/{id}/customer_classes:
    get:
      summary: List activated customer classes
      description: Lists the activated customer classes for a sales price. The ID
        of the sales price must be specified.
      operationId: getRestItemsSalesPricesCustomerClasses
      x-api-path-slug: restitemssales-pricesidcustomer-classes-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Activated
      - Customer
      - Classes
    post:
      summary: Activate a customer class
      description: Activates a customer class for a sales price. The ID of the sales
        price and the ID of the customer class must be specified.
      operationId: postRestItemsSalesPricesCustomerClasses
      x-api-path-slug: restitemssales-pricesidcustomer-classes-post
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/customer_classes
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Customer
      - Class
  /rest/items/sales_prices/{id}/customer_classes/{customerClassId}:
    delete:
      summary: Activate a customer class
      description: Activates a customer class for a sales price. The ID of the sales
        price and the ID of the customer class must be specified.
      operationId: deleteRestItemsSalesPricesCustomerClassesCustomerclass
      x-api-path-slug: restitemssales-pricesidcustomer-classescustomerclassid-delete
      parameters:
      - in: path
        name: customerClassId
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Customer
      - Class
  /rest/items/sales_prices/{id}/names:
    get:
      summary: List names of a sales price
      description: Lists the names of a sales price in all languages. The ID of the
        sales price must be specified.
      operationId: getRestItemsSalesPricesNames
      x-api-path-slug: restitemssales-pricesidnames-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
      - Of
      - Sales
      - Price
    post:
      summary: Create a sales price name
      description: Creates a name for a sales price in the specified language. The
        ID of the sales price must be specified.
      operationId: postRestItemsSalesPricesNames
      x-api-path-slug: restitemssales-pricesidnames-post
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/names
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
      - Name
  /rest/items/sales_prices/{id}/names/{lang}:
    delete:
      summary: Delete a sales price name
      description: Deletes the name of a sales price in the specified language. The
        ID of the sales price and the language code must be specified.
      operationId: deleteRestItemsSalesPricesNamesLang
      x-api-path-slug: restitemssales-pricesidnameslang-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
      - Name
    get:
      summary: Gets a sales price name
      description: Gets the sales price name of a sales price in the specified langauge.
        The ID of the sales price and the language code must be specified.
      operationId: getRestItemsSalesPricesNamesLang
      x-api-path-slug: restitemssales-pricesidnameslang-get
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - S
      - Sales
      - Price
      - Name
    put:
      summary: Update a sales price name
      description: Updates a sales price name in the specified language. The ID of
        the sales price and the language code must be specified.
      operationId: putRestItemsSalesPricesNamesLang
      x-api-path-slug: restitemssales-pricesidnameslang-put
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/names/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
      - Name
  /rest/items/sales_prices/{id}/online_stores:
    get:
      summary: List activated clients (stores)
      description: Lists all activated clients (stores) for a sales price. The ID
        of the sales price must be specified.
      operationId: getRestItemsSalesPricesOnlineStores
      x-api-path-slug: restitemssales-pricesidonline-stores-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Activated
      - Clients
      - (stores)
    post:
      summary: Activate a client (store)
      description: Activates a client (store) for a sales price. The ID of the sales
        price must be specified.
      operationId: postRestItemsSalesPricesOnlineStores
      x-api-path-slug: restitemssales-pricesidonline-stores-post
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/online_stores
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Client
      - (store)
  /rest/items/sales_prices/{id}/online_stores/{webstoreId}:
    delete:
      summary: Deactivate a client (store)
      description: Deactivates a client (store) for a sales price. The ID of the sales
        price and the ID of the client (store) must be specified.
      operationId: deleteRestItemsSalesPricesOnlineStoresWebstore
      x-api-path-slug: restitemssales-pricesidonline-storeswebstoreid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: webstoreId
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Client
      - (store)
  /rest/items/sales_prices/{id}/referrers:
    get:
      summary: List activated referrers
      description: Lists all activated referrers for a sales price. The ID of the
        sales price must be specified.
      operationId: getRestItemsSalesPricesReferrers
      x-api-path-slug: restitemssales-pricesidreferrers-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Activated
      - Referrers
    post:
      summary: Activate a referrer
      description: Activates a referrer for a sales price. The ID of the sales price
        must be specified.
      operationId: postRestItemsSalesPricesReferrers
      x-api-path-slug: restitemssales-pricesidreferrers-post
      parameters:
      - in: body
        name: /rest/items/sales_prices/{id}/referrers
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Referrer
  /rest/items/sales_prices/{id}/referrers/{referrerId}:
    delete:
      summary: Deactivates a referrer
      description: Deactivates a referrer for a sales price. The ID of the sales price
        and the ID of the referrer must be specified.
      operationId: deleteRestItemsSalesPricesReferrersReferrer
      x-api-path-slug: restitemssales-pricesidreferrersreferrerid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: referrerId
      responses:
        200:
          description: OK
      tags:
      - Deactivates
      - Referrer
  /rest/items/units:
    get:
      summary: List units
      description: Lists all units.
      operationId: getRestItemsUnits
      x-api-path-slug: restitemsunits-get
      parameters:
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      responses:
        200:
          description: OK
      tags:
      - List
      - Units
    post:
      summary: Create a unit
      description: Creates a unit.
      operationId: postRestItemsUnits
      x-api-path-slug: restitemsunits-post
      parameters:
      - in: body
        name: /rest/items/units
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Unit
  /rest/items/units/{id}:
    delete:
      summary: Delete a unit
      description: Deletes a unit. The ID of the unit must be specified.
      operationId: deleteRestItemsUnits
      x-api-path-slug: restitemsunitsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Unit
    get:
      summary: Get a unit
      description: Gets a unit. The ID of the unit must be specified.
      operationId: getRestItemsUnits
      x-api-path-slug: restitemsunitsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Unit
    put:
      summary: Update a unit
      description: Updates a unit. The ID of the unit must be specified.
      operationId: putRestItemsUnits
      x-api-path-slug: restitemsunitsid-put
      parameters:
      - in: body
        name: /rest/items/units/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Unit
  /rest/items/units/{id}/names:
    get:
      summary: List unit names
      description: Lists the unit names of a unit. The ID of the unit must be specified.
      operationId: getRestItemsUnitsNames
      x-api-path-slug: restitemsunitsidnames-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Unit
      - Names
    post:
      summary: Create a unit name
      description: Creates a unit name. The ID of the unit and the language must be
        specified.
      operationId: postRestItemsUnitsNames
      x-api-path-slug: restitemsunitsidnames-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Unit
      - Name
  /rest/items/units/{id}/names/{lang}:
    delete:
      summary: Delete a unit name
      description: Deletes a unit name. The ID of the unit and the language must be
        specified.
      operationId: deleteRestItemsUnitsNamesLang
      x-api-path-slug: restitemsunitsidnameslang-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Unit
      - Name
    get:
      summary: Get a unit name
      description: Gets a unit name. The ID of the unit and the language must be specified.
      operationId: getRestItemsUnitsNamesLang
      x-api-path-slug: restitemsunitsidnameslang-get
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Unit
      - Name
    put:
      summary: Update a unit name
      description: Updates a unit name. The ID of the unit and the language must be
        specified.
      operationId: putRestItemsUnitsNamesLang
      x-api-path-slug: restitemsunitsidnameslang-put
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Unit
      - Name
  /rest/items/variations:
    get:
      summary: Search variations
      description: Search variations by different filters
      operationId: getRestItemsVariations
      x-api-path-slug: restitemsvariations-get
      parameters:
      - in: query
        name: barcode
        description: Filter restricts the list of results to variations with the specified
          barcode
      - in: query
        name: categoryId
        description: Filter restricts the list of results to variations with the specified
          category id
      - in: query
        name: createdBetween
        description: Filter restricts the list of results to variations created during
          the specified period
      - in: query
        name: flagOne
        description: Filter restricts the list of results to variations of items with
          the flag one
      - in: query
        name: flagTwo
        description: Filter restricts the list of results to variations of items with
          the flag two
      - in: query
        name: id
        description: Filter restricts the list of results to variations with the specified
          variation ID
      - in: query
        name: isActive
        description: Filter restricts the list of results to variations that are active
      - in: query
        name: isBundle
        description: Filter restricts the list of results to variations to which variations
          were added to create a bundle
      - in: query
        name: isMain
        description: Filter restricts the list of results to variations that are main
          variations
      - in: query
        name: itemId
        description: Filter restricts the list of results to variations with the specified
          item ID
      - in: query
        name: itemName
        description: Filter restricts the list of results to variations with the specified
          item name
      - in: query
        name: itemsPerPage
        description: Limits the number of results listed per page to a specific number
      - in: query
        name: itemTagId
        description: Filter restricts the list of results to variations with the specified
          tag ID
      - in: query
        name: lang
        description: The language of the variation information
      - in: query
        name: manufacturerId
        description: Filter restricts the list of results to variations with the specified
          manufacturer ID
      - in: query
        name: numberExact
        description: Filter restricts the list of results to the variation with the
          variation number specified
      - in: query
        name: numberFuzzy
        description: Filter restricts the list of results to variations with numbers
          that contain the variation number specified (SQL LIKE operator)
      - in: query
        name: page
        description: Limits the results to a specific page
      - in: query
        name: plentyId
        description: Filter restricts the list of results to variations to which variations
          were visible in specific Clients
      - in: query
        name: relatedUpdatedBetween
        description: Filter restricts the list of results to those variations for
          which related information was updated during the specified period
      - in: query
        name: sku
        description: Filter restricts the list of results to variations with the specified
          SKU
      - in: query
        name: storeSpecial
        description: Filter restricts the list of results to variations of items with
          the specified store special
      - in: query
        name: supplierNumber
        description: Filter restricts the list of results to variations with the specified
          supplier number
      - in: query
        name: updatedBetween
        description: Filter restricts the list of results to variations updated during
          the specified period
      - in: query
        name: with
        description: Includes the specified variation information in the results
      responses:
        200:
          description: OK
      tags:
      - Search
      - Variations
  /rest/items/variations/variation_categories:
    post:
      summary: Bulk create category links
      description: Creates up to 50 links between variations and categories. The ID
        of the variations and the ID of the categories must be specified.
      operationId: postRestItemsVariationsVariationCategories
      x-api-path-slug: restitemsvariationsvariation-categories-post
      parameters:
      - in: body
        name: /rest/items/variations/variation_categories
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Create
      - Category
      - Links
    put:
      summary: Bulk update category links
      description: Updates up to 50 links between variations and categories. The ID
        of the variations and the ID of the categories must be specified.
      operationId: putRestItemsVariationsVariationCategories
      x-api-path-slug: restitemsvariationsvariation-categories-put
      parameters:
      - in: body
        name: /rest/items/variations/variation_categories
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Update
      - Category
      - Links
  /rest/items/variations/variation_markets:
    get:
      summary: List all links between variations and markets
      description: |-
        Lists all links between variations and markets.
        Results can be filtered by the ID of the variation and by the ID of the market, e.g. "variationId=1030"
        lists all links of the variation with the ID 1030.
      operationId: getRestItemsVariationsVariationMarkets
      x-api-path-slug: restitemsvariationsvariation-markets-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Links
      - Between
      - Variations
      - Markets
    post:
      summary: Create up to 50 links between variations and markets
      description: Creates up to 50 links between variations and markets. The ID of
        the variation and the ID of the market must be specified.
      operationId: postRestItemsVariationsVariationMarkets
      x-api-path-slug: restitemsvariationsvariation-markets-post
      parameters:
      - in: body
        name: /rest/items/variations/variation_markets
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Up
      - To
      - "50"
      - Links
      - Between
      - Variations
      - Markets
  /rest/items/variations/variation_properties:
    post:
      summary: Bulk update properties
      description: Creates up to 50 properties of variations.
      operationId: postRestItemsVariationsVariationProperties
      x-api-path-slug: restitemsvariationsvariation-properties-post
      parameters:
      - in: body
        name: /rest/items/variations/variation_properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Update
      - Properties
    put:
      summary: Bulk update properties
      description: Updates up to 50 properties of variations.
      operationId: putRestItemsVariationsVariationProperties
      x-api-path-slug: restitemsvariationsvariation-properties-put
      parameters:
      - in: body
        name: /rest/items/variations/variation_properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Update
      - Properties
  /rest/items/variations/variation_sales_prices:
    get:
      summary: Get all sales price relations
      description: Gets all links between variations and sales prices including sales
        price data.
      operationId: getRestItemsVariationsVariationSalesPrices
      x-api-path-slug: restitemsvariationsvariation-sales-prices-get
      parameters:
      - in: query
        name: salesPriceId
        description: Filter that restricts the search result to the sales price data
          of variations linked to a specific sales price
      - in: query
        name: updatedAt
        description: Filter that restricts the search result to links between variations
          and sales prices updated after a specific point in time
      - in: query
        name: variationId
        description: Filter that restricts the search result to the sales price data
          of a specific variation
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
      - Relations
    post:
      summary: Bulk create prices
      description: Creates up to 50 prices of variations. The ID of the variation,
        the ID of the sales price and a price must be specified.
      operationId: postRestItemsVariationsVariationSalesPrices
      x-api-path-slug: restitemsvariationsvariation-sales-prices-post
      parameters:
      - in: body
        name: /rest/items/variations/variation_sales_prices
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Create
      - Prices
    put:
      summary: Bulk update prices
      description: Updates up to 50 prices of variations. The ID of the variation,
        the ID of the sales price and a price must be specified.
      operationId: putRestItemsVariationsVariationSalesPrices
      x-api-path-slug: restitemsvariationsvariation-sales-prices-put
      parameters:
      - in: body
        name: /rest/items/variations/variation_sales_prices
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Update
      - Prices
  /rest/items/{id}/images:
    get:
      summary: List images of an item
      description: Lists all images of an item. The item ID must be specified.
      operationId: getRestItemsImages
      x-api-path-slug: restitemsidimages-get
      parameters:
      - in: path
        name: id
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      responses:
        200:
          description: OK
      tags:
      - List
      - Images
      - Of
      - Item
  /rest/items/{id}/images/attribute_value_markets:
    get:
      summary: List attribute value image link
      description: Lists the images linked to an attribute value.
      operationId: getRestItemsImagesAttributeValueMarkets
      x-api-path-slug: restitemsidimagesattribute-value-markets-get
      parameters:
      - in: query
        name: attributeId
        description: The unique ID of the attribute
      - in: path
        name: id
      - in: query
        name: imageId
        description: The unique ID of the image
      - in: query
        name: itemId
        description: The unique ID of the item
      - in: query
        name: valueId
        description: The unique ID of the attribute value
      responses:
        200:
          description: OK
      tags:
      - List
      - Attribute
      - Value
      - Image
      - Link
  /rest/items/{id}/images/upload:
    post:
      summary: Upload a new image
      description: Uploads an image. The item ID must be specified.
      operationId: postRestItemsImagesUpload
      x-api-path-slug: restitemsidimagesupload-post
      parameters:
      - in: body
        name: /rest/items/{id}/images/upload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Upload
      - New
      - Image
  /rest/items/{id}/images/{imageId}:
    delete:
      summary: Delete an image
      description: Delete an image. The ID of the image must be specified.
      operationId: deleteRestItemsImagesImage
      x-api-path-slug: restitemsidimagesimageid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - Image
    get:
      summary: Get an image
      description: Gets an image. The ID of the image must be specified.
      operationId: getRestItemsImagesImage
      x-api-path-slug: restitemsidimagesimageid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - Image
    put:
      summary: Update an image
      description: Updates an image. The ID of the image must be specified.
      operationId: putRestItemsImagesImage
      x-api-path-slug: restitemsidimagesimageid-put
      parameters:
      - in: body
        name: /rest/items/{id}/images/{imageId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - Image
  /rest/items/{id}/images/{imageId}/attribute_value_markets:
    post:
      summary: Create an attribute value image link
      description: Creates a link between an image and an attribute value.
      operationId: postRestItemsImagesImageAttributeValueMarkets
      x-api-path-slug: restitemsidimagesimageidattribute-value-markets-post
      parameters:
      - in: body
        name: /rest/items/{id}/images/{imageId}/attribute_value_markets
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Image
      - Link
  /rest/items/{id}/images/{imageId}/attribute_value_markets/{valueId}:
    delete:
      summary: Delete an attribute value image link
      description: Deletes the link between an image and an attribute value. The attribute
        ID must be specified.
      operationId: deleteRestItemsImagesImageAttributeValueMarketsValue
      x-api-path-slug: restitemsidimagesimageidattribute-value-marketsvalueid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      - in: query
        name: itemId
        description: The unique ID of the item
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Image
      - Link
    get:
      summary: Get an attribute value image link
      description: 'Gets an attribute value image link. The following IDs must be
        specified: image ID, item ID and value ID.'
      operationId: getRestItemsImagesImageAttributeValueMarketsValue
      x-api-path-slug: restitemsidimagesimageidattribute-value-marketsvalueid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      - in: query
        name: itemId
        description: The unique ID of the item
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Image
      - Link
    put:
      summary: Update an attribute value image link
      description: 'Updates the link between an image and an attribute value. The
        following IDs must be specified: image ID, item ID and value ID.'
      operationId: putRestItemsImagesImageAttributeValueMarketsValue
      x-api-path-slug: restitemsidimagesimageidattribute-value-marketsvalueid-put
      parameters:
      - in: body
        name: /rest/items/{id}/images/{imageId}/attribute_value_markets/{valueId}
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: attributeId
        description: The unique ID of the attribute
      - in: path
        name: id
      - in: path
        name: imageId
      - in: query
        name: itemId
        description: The unique ID of the item
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Image
      - Link
  /rest/items/{id}/images/{imageId}/availabilities:
    delete:
      summary: Delete an availability
      description: Delete an availability for a specified value.
      operationId: deleteRestItemsImagesImageAvailabilities
      x-api-path-slug: restitemsidimagesimageidavailabilities-delete
      parameters:
      - in: body
        name: /rest/items/{id}/images/{imageId}/availabilities
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - Availability
    get:
      summary: List availabilities
      description: List all availabilities of an image. The image ID must be specified.
      operationId: getRestItemsImagesImageAvailabilities
      x-api-path-slug: restitemsidimagesimageidavailabilities-get
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - List
      - Availabilities
    post:
      summary: Create an availability
      description: Create an availability. The image ID must be specified.
      operationId: postRestItemsImagesImageAvailabilities
      x-api-path-slug: restitemsidimagesimageidavailabilities-post
      parameters:
      - in: body
        name: /rest/items/{id}/images/{imageId}/availabilities
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - Availability
  /rest/items/{id}/images/{imageId}/names:
    get:
      summary: List names of an image
      description: Lists all names of an image. The image ID must be specified.
      operationId: getRestItemsImagesImageNames
      x-api-path-slug: restitemsidimagesimageidnames-get
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
      - Of
      - Image
    post:
      summary: Create an image name
      description: Create an image name. The ID, language and name of the image must
        be specified.
      operationId: postRestItemsImagesImageNames
      x-api-path-slug: restitemsidimagesimageidnames-post
      parameters:
      - in: body
        name: /rest/items/{id}/images/{imageId}/names
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - Image
      - Name
  /rest/items/{id}/images/{imageId}/names/{lang}:
    delete:
      summary: Delete an image name
      description: Delete an image name. The ID and language of the image must be
        specified.
      operationId: deleteRestItemsImagesImageNamesLang
      x-api-path-slug: restitemsidimagesimageidnameslang-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Image
      - Name
    get:
      summary: Get an image name
      description: Gets an image name. The image ID and language must be specified.
      operationId: getRestItemsImagesImageNamesLang
      x-api-path-slug: restitemsidimagesimageidnameslang-get
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Image
      - Name
    put:
      summary: Update an image name
      description: Update an image name. The ID, language and name of the image must
        be specified.
      operationId: putRestItemsImagesImageNamesLang
      x-api-path-slug: restitemsidimagesimageidnameslang-put
      parameters:
      - in: body
        name: /rest/items/{id}/images/{imageId}/names/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: imageId
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Image
      - Name
  /rest/items/{id}/images/{imageId}/variation_images:
    get:
      summary: List image links of an image
      description: Lists all variations linked to an image. The image ID must be specified.
      operationId: getRestItemsImagesImageVariationImages
      x-api-path-slug: restitemsidimagesimageidvariation-images-get
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - List
      - Image
      - Links
      - Of
      - Image
  /rest/items/{id}/item_cross_selling:
    get:
      summary: List cross-selling links
      description: Lists all cross-selling items linked to an item. The ID of the
        item must be specified.
      operationId: getRestItemsItemCrossSelling
      x-api-path-slug: restitemsiditem-cross-selling-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Cross-selling
      - Links
    post:
      summary: Create a cross-selling link
      description: Creates a cross-selling link.
      operationId: postRestItemsItemCrossSelling
      x-api-path-slug: restitemsiditem-cross-selling-post
      parameters:
      - in: body
        name: /rest/items/{id}/item_cross_selling
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Cross-selling
      - Link
  /rest/items/{id}/item_cross_selling/{crossItemId}:
    delete:
      summary: Delete a cross-selling link
      description: Deletes a cross-selling link. The ID of the item and the ID of
        the cross-selling item must be specified.
      operationId: deleteRestItemsItemCrossSellingCrossitem
      x-api-path-slug: restitemsiditem-cross-sellingcrossitemid-delete
      parameters:
      - in: path
        name: crossItemId
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Cross-selling
      - Link
  /rest/items/{id}/variation_images:
    get:
      summary: List image links of an item
      description: Lists all images linked to an item. The item ID must be specified.
      operationId: getRestItemsVariationImages
      x-api-path-slug: restitemsidvariation-images-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Image
      - Links
      - Of
      - Item
  /rest/items/{id}/variations/{variationId}/descriptions:
    get:
      summary: List texts
      description: Lists the texts for an item in all available languages. The ID
        of the variation must be specified.
      operationId: getRestItemsVariationsVariationDescriptions
      x-api-path-slug: restitemsidvariationsvariationiddescriptions-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Texts
    post:
      summary: Create texts
      description: Creates texts for an item. The ID of the variation and the language
        code must be specified.
      operationId: postRestItemsVariationsVariationDescriptions
      x-api-path-slug: restitemsidvariationsvariationiddescriptions-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/descriptions
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Texts
  /rest/items/{id}/variations/{variationId}/descriptions/{lang}:
    delete:
      summary: Delete texts
      description: Deletes texts for an item in the specified language. The ID of
        the variation and the language code must be specified.
      operationId: deleteRestItemsVariationsVariationDescriptionsLang
      x-api-path-slug: restitemsidvariationsvariationiddescriptionslang-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Texts
    get:
      summary: Get texts
      description: Gets the texts for an item in the specified language. The ID of
        the variation and the language code must be specified.
      operationId: getRestItemsVariationsVariationDescriptionsLang
      x-api-path-slug: restitemsidvariationsvariationiddescriptionslang-get
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Texts
    put:
      summary: Update texts
      description: Updates texts for an item in the specified language. The ID of
        the variation and the language code must be specified.
      operationId: putRestItemsVariationsVariationDescriptionsLang
      x-api-path-slug: restitemsidvariationsvariationiddescriptionslang-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/descriptions/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: lang
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Texts
  /rest/items/{id}/variations/{variationId}/images:
    get:
      summary: List images of a variation
      description: Lists all images of a variation. The variation ID must be specified.
      operationId: getRestItemsVariationsVariationImages
      x-api-path-slug: restitemsidvariationsvariationidimages-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Images
      - Of
      - Variation
  /rest/items/{id}/variations/{variationId}/labels:
    post:
      summary: Get a variation label
      description: Gets a base64 encoded label for the specified variation ID. The
        labelId of the label template must be specified.
      operationId: postRestItemsVariationsVariationLabels
      x-api-path-slug: restitemsidvariationsvariationidlabels-post
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
      - Label
  /rest/items/{id}/variations/{variationId}/market_ident_numbers:
    get:
      summary: List ident number of a variation
      description: Lists the ident number (ASIN/ePID) of a variation. The ID of the
        item and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationMarketEntNumbers
      x-api-path-slug: restitemsidvariationsvariationidmarket-ident-numbers-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Ident
      - Number
      - Of
      - Variation
    post:
      summary: Create a market ident number
      description: Creates a market ident number (ASIN/ePID) for a variation.
      operationId: postRestItemsVariationsVariationMarketEntNumbers
      x-api-path-slug: restitemsidvariationsvariationidmarket-ident-numbers-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/market_ident_numbers
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Ident
      - Number
  /rest/items/{id}/variations/{variationId}/market_ident_numbers/{marketIdentNumberId}:
    delete:
      summary: Deletes a market ident number
      description: Deletes a market ident number (ASIN/ePID) of a variation.
      operationId: deleteRestItemsVariationsVariationMarketEntNumbersMarketentnumber
      x-api-path-slug: restitemsidvariationsvariationidmarket-ident-numbersmarketidentnumberid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: marketIdentNumberId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Market
      - Ident
      - Number
    get:
      summary: Get a market ident number
      description: Gets a market ident number (ASIN/ePID) of a variation.
      operationId: getRestItemsVariationsVariationMarketEntNumbersMarketentnumber
      x-api-path-slug: restitemsidvariationsvariationidmarket-ident-numbersmarketidentnumberid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: marketIdentNumberId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Ident
      - Number
    put:
      summary: Updates a market ident number
      description: Updates a market ident number (ASIN/ePID) of a variation.
      operationId: putRestItemsVariationsVariationMarketEntNumbersMarketentnumber
      x-api-path-slug: restitemsidvariationsvariationidmarket-ident-numbersmarketidentnumberid-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/market_ident_numbers/{marketIdentNumberId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: marketIdentNumberId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Market
      - Ident
      - Number
  /rest/items/{id}/variations/{variationId}/stock:
    get:
      summary: List stock of a variation per warehouse
      description: Lists stock of a variation per warehouse. The ID of the item and
        the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationStock
      x-api-path-slug: restitemsidvariationsvariationidstock-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: id
      - in: query
        name: itemId
        description: The ID of the item
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - Of
      - Variation
      - Per
      - Warehouse
  /rest/items/{id}/variations/{variationId}/stock/bookIncomingItems:
    put:
      summary: Book incoming stock
      description: Books incoming stock for a variation. The incoming stock will be
        added to the existing stock. The ID of the item and the ID of the variation
        must be specified.
      operationId: putRestItemsVariationsVariationStockBookincomingitems
      x-api-path-slug: restitemsidvariationsvariationidstockbookincomingitems-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/stock/bookIncomingItems
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: query
        name: itemId
        description: The ID of the item
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Book
      - Incoming
      - Stock
  /rest/items/{id}/variations/{variationId}/stock/correction:
    put:
      summary: Correct stock
      description: Corrects stock. The item ID and the variation ID must be specified.
      operationId: putRestItemsVariationsVariationStockCorrection
      x-api-path-slug: restitemsidvariationsvariationidstockcorrection-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/stock/correction
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: query
        name: itemId
        description: The ID of the item
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Correct
      - Stock
  /rest/items/{id}/variations/{variationId}/stock/movements:
    get:
      summary: List stock movements
      description: |-
        Lists stock movements for a variation. The ID of the item and the ID of the variation must be specified. To get movements older than 3 months, set the 'year' parameter.
        NOTE: You can either get archive entries or non-archive entries. You can not get entries for the current year that are younger and older than 3 months with one request. You need separate requests to get entries older and younger than 3 months. To get all entries younger than 3 month you do not need to specify a year or any createdAt parameter.
      operationId: getRestItemsVariationsVariationStockMovements
      x-api-path-slug: restitemsidvariationsvariationidstockmovements-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: createdAtFrom
        description: Get entries with createdAt date after this date
      - in: query
        name: createdAtTo
        description: Get entries with createdAt date before this date
      - in: path
        name: id
      - in: query
        name: itemId
        description: The ID of the item
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: variationId
      - in: query
        name: warehouseId
        description: The ID of the warehouse
      - in: query
        name: year
        description: Get entries from the archive for the given year
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - Movements
  /rest/items/{id}/variations/{variationId}/stock/redistribute:
    put:
      summary: Redistribute stock
      description: Redistributes the stock of one storage location among one or more
        storage locations. The item ID and the variation ID need to be specified.
      operationId: putRestItemsVariationsVariationStockRedistribute
      x-api-path-slug: restitemsidvariationsvariationidstockredistribute-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/stock/redistribute
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: query
        name: itemId
        description: The ID of the item
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Redistribute
      - Stock
  /rest/items/{id}/variations/{variationId}/stock/storageLocations:
    get:
      summary: List stock of a variation per storage locations
      description: Lists stock of a variation per storage location. The ID of the
        item and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationStockStoragelocations
      x-api-path-slug: restitemsidvariationsvariationidstockstoragelocations-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: id
      - in: query
        name: itemId
        description: The ID of the item
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - Of
      - Variation
      - Per
      - Storage
      - Locations
  /rest/items/{id}/variations/{variationId}/variation_additional_skus:
    get:
      summary: List additional SKUs
      description: Lists the additional SKUs of a variation. Filters must be specified.
      operationId: getRestItemsVariationsVariationVariationAdditionalSkus
      x-api-path-slug: restitemsidvariationsvariationidvariation-additional-skus-get
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_additional_skus
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Additional
      - SKUs
    post:
      summary: Create an additional SKU
      description: Creates an additional SKU. The ID of the variation must be specified.
      operationId: postRestItemsVariationsVariationVariationAdditionalSkus
      x-api-path-slug: restitemsidvariationsvariationidvariation-additional-skus-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_additional_skus
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Additional
      - SKU
  /rest/items/{id}/variations/{variationId}/variation_additional_skus/{additionalSkuId}:
    delete:
      summary: Delete an additional SKU
      description: Deletes an additional SKU. The ID of the additional SKU must be
        specified.
      operationId: deleteRestItemsVariationsVariationVariationAdditionalSkusAdditionalsku
      x-api-path-slug: restitemsidvariationsvariationidvariation-additional-skusadditionalskuid-delete
      parameters:
      - in: path
        name: additionalSkuId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Additional
      - SKU
    get:
      summary: Gets an additional SKU
      description: Gets an additional SKU. The ID of the additional SKU must be specified.
      operationId: getRestItemsVariationsVariationVariationAdditionalSkusAdditionalsku
      x-api-path-slug: restitemsidvariationsvariationidvariation-additional-skusadditionalskuid-get
      parameters:
      - in: path
        name: additionalSkuId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Additional
      - SKU
    put:
      summary: Update an additional SKU
      description: Updates an additional SKU. The ID of the additional SKU must be
        specified.
      operationId: putRestItemsVariationsVariationVariationAdditionalSkusAdditionalsku
      x-api-path-slug: restitemsidvariationsvariationidvariation-additional-skusadditionalskuid-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_additional_skus/{additionalSkuId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: additionalSkuId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Additional
      - SKU
  /rest/items/{id}/variations/{variationId}/variation_barcodes:
    get:
      summary: List variation barcodes
      description: Lists all barcodes of a variation. The ID of the item and the ID
        of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationBarcodes
      x-api-path-slug: restitemsidvariationsvariationidvariation-barcodes-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      - in: query
        name: with
        description: Includes the specified variation barcode information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Variation
      - Barcodes
    post:
      summary: Create a variation barcode
      description: Creates a variation barcode. The ID of the item, the ID of the
        variation, the ID of the barcode and the code must be specified.
      operationId: postRestItemsVariationsVariationVariationBarcodes
      x-api-path-slug: restitemsidvariationsvariationidvariation-barcodes-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_barcodes
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
      - Barcode
  /rest/items/{id}/variations/{variationId}/variation_barcodes/{barcodeId}:
    delete:
      summary: Delete a variation barcode
      description: Deletes a variation barcode. Unlinks the barcode from the variation
        and deletes the code saved for the variation.
      operationId: deleteRestItemsVariationsVariationVariationBarcodesBarcode
      x-api-path-slug: restitemsidvariationsvariationidvariation-barcodesbarcodeid-delete
      parameters:
      - in: path
        name: barcodeId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
      - Barcode
    get:
      summary: Get a variation barcode
      description: Get a specific variation barcode. The ID of the item, the ID of
        the variation and the ID of the barcode must be specified.
      operationId: getRestItemsVariationsVariationVariationBarcodesBarcode
      x-api-path-slug: restitemsidvariationsvariationidvariation-barcodesbarcodeid-get
      parameters:
      - in: path
        name: barcodeId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
      - Barcode
    put:
      summary: Update a variation barcode
      description: Updates a variation barcode. The ID of the item, the ID of the
        variation, the ID of the barcode and the code must be specified.
      operationId: putRestItemsVariationsVariationVariationBarcodesBarcode
      x-api-path-slug: restitemsidvariationsvariationidvariation-barcodesbarcodeid-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_barcodes/{barcodeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: barcodeId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
      - Barcode
  /rest/items/{id}/variations/{variationId}/variation_bundles:
    get:
      summary: List bundle components
      description: List all components of a bundle. The ID of the item and the ID
        of the variation to which bundle components were added must be specified.
      operationId: getRestItemsVariationsVariationVariationBundles
      x-api-path-slug: restitemsidvariationsvariationidvariation-bundles-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Bundle
      - Components
    post:
      summary: Add a variation to a bundle
      description: Adds a variation to a bundle variation as a bundle component.
      operationId: postRestItemsVariationsVariationVariationBundles
      x-api-path-slug: restitemsidvariationsvariationidvariation-bundles-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_bundles
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
      - To
      - Bundle
  /rest/items/{id}/variations/{variationId}/variation_bundles/{bundleId}:
    delete:
      summary: Remove a bundle component
      description: Removes a component from a bundle. The bundle ID must be specified.
      operationId: deleteRestItemsVariationsVariationVariationBundlesBundle
      x-api-path-slug: restitemsidvariationsvariationidvariation-bundlesbundleid-delete
      parameters:
      - in: path
        name: bundleId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Bundle
      - Component
    get:
      summary: Get a variation bundle
      description: Gets the bundle information for a specific bundle component.
      operationId: getRestItemsVariationsVariationVariationBundlesBundle
      x-api-path-slug: restitemsidvariationsvariationidvariation-bundlesbundleid-get
      parameters:
      - in: path
        name: bundleId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
      - Bundle
    put:
      summary: Update a variation bundle
      description: Updates a variation bundle component.
      operationId: putRestItemsVariationsVariationVariationBundlesBundle
      x-api-path-slug: restitemsidvariationsvariationidvariation-bundlesbundleid-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_bundles/{bundleId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bundleId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
      - Bundle
  /rest/items/{id}/variations/{variationId}/variation_categories:
    get:
      summary: List categories linked to a variation
      description: Lists all categories linked to a variation.
      operationId: getRestItemsVariationsVariationVariationCategories
      x-api-path-slug: restitemsidvariationsvariationidvariation-categories-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Categories
      - Linked
      - To
      - Variation
    post:
      summary: Link a category to a variation
      description: Creates a link between a category and a variation.
      operationId: postRestItemsVariationsVariationVariationCategories
      x-api-path-slug: restitemsidvariationsvariationidvariation-categories-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_categories
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Category
      - To
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_categories/{catId}:
    delete:
      summary: Remove a category from a variation
      description: Deletes the link between a category and a variation.
      operationId: deleteRestItemsVariationsVariationVariationCategoriesCat
      x-api-path-slug: restitemsidvariationsvariationidvariation-categoriescatid-delete
      parameters:
      - in: path
        name: catId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Category
      - From
      - Variation
    get:
      summary: Get link between category and variation
      description: Gets the link between a category and a variation.
      operationId: getRestItemsVariationsVariationVariationCategoriesCat
      x-api-path-slug: restitemsidvariationsvariationidvariation-categoriescatid-get
      parameters:
      - in: path
        name: catId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Category
      - Variation
    put:
      summary: Update variation category link
      description: Updates the link between a category and a variation.
      operationId: putRestItemsVariationsVariationVariationCategoriesCat
      x-api-path-slug: restitemsidvariationsvariationidvariation-categoriescatid-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_categories/{catId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: catId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
      - Category
      - Link
  /rest/items/{id}/variations/{variationId}/variation_clients:
    get:
      summary: List clients linked to a variation
      description: Lists all clients (stores) linked to a variation. The ID of the
        variation must be specified.
      operationId: getRestItemsVariationsVariationVariationClients
      x-api-path-slug: restitemsidvariationsvariationidvariation-clients-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Clients
      - Linked
      - To
      - Variation
    post:
      summary: Link a client to a variation
      description: Creates a link between a client (store) and a variation.
      operationId: postRestItemsVariationsVariationVariationClients
      x-api-path-slug: restitemsidvariationsvariationidvariation-clients-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_clients
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Client
      - To
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_clients/{plentyId}:
    delete:
      summary: Unlink a client from a variation
      description: Deletes the link between a client (store) and a variation.
      operationId: deleteRestItemsVariationsVariationVariationClientsPlenty
      x-api-path-slug: restitemsidvariationsvariationidvariation-clientsplentyid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: plentyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Unlink
      - Client
      - From
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_default_categories:
    get:
      summary: List default category links
      description: Lists the default category of a variation for all clients (stores).
        The ID of the item and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationDefaultCategories
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categories-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Default
      - Category
      - Links
    post:
      summary: Create a default category link
      description: Creates a link between a variation and a category that designates
        the category as the default category.
      operationId: postRestItemsVariationsVariationVariationDefaultCategories
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categories-post
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Default
      - Category
      - Link
  /rest/items/{id}/variations/{variationId}/variation_default_categories/{plentyId}:
    delete:
      summary: Delete a default category link
      description: Deletes a link between a variation and a category that designates
        this category as the default category.
      operationId: deleteRestItemsVariationsVariationVariationDefaultCategoriesPlenty
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categoriesplentyid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: plentyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Default
      - Category
      - Link
    get:
      summary: Gets a default category link
      description: Gets the default category linked to a variation for the specified
        client (store). The ID of the item, the ID of the variation and the ID of
        the client (store) must be specified.
      operationId: getRestItemsVariationsVariationVariationDefaultCategoriesPlenty
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categoriesplentyid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: plentyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Default
      - Category
      - Link
  /rest/items/{id}/variations/{variationId}/variation_images:
    get:
      summary: List image links of a variation
      description: Lists all images linked to a variation. The variation ID must be
        specified.
      operationId: getRestItemsVariationsVariationVariationImages
      x-api-path-slug: restitemsidvariationsvariationidvariation-images-get
      parameters:
      - in: path
        name: id
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to variation images updated
          after the specified date
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Image
      - Links
      - Of
      - Variation
    post:
      summary: Create an image link
      description: Creates a link between an image and a variation.
      operationId: postRestItemsVariationsVariationVariationImages
      x-api-path-slug: restitemsidvariationsvariationidvariation-images-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_images
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Image
      - Link
  /rest/items/{id}/variations/{variationId}/variation_images/{imageId}:
    delete:
      summary: Delete an image link
      description: Deletes a link between an image and a variation.
      operationId: deleteRestItemsVariationsVariationVariationImagesImage
      x-api-path-slug: restitemsidvariationsvariationidvariation-imagesimageid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Image
      - Link
  /rest/items/{id}/variations/{variationId}/variation_markets:
    delete:
      summary: Delete all market links of one variation
      description: Deletes all links of one variation. The ID of the variation must
        be specified.
      operationId: deleteRestItemsVariationsVariationVariationMarkets
      x-api-path-slug: restitemsidvariationsvariationidvariation-markets-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Links
      - Of
      - Variation
    get:
      summary: List markets linked to a variation
      description: Lists all markets linked to a variation. The ID of the item and
        the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationMarkets
      x-api-path-slug: restitemsidvariationsvariationidvariation-markets-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Markets
      - Linked
      - To
      - Variation
    post:
      summary: Create link between variation and market
      description: Creates a link between a variation and a market. The ID of the
        item, the ID of the variation and the ID of the market must be specified.
      operationId: postRestItemsVariationsVariationVariationMarkets
      x-api-path-slug: restitemsidvariationsvariationidvariation-markets-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_markets
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Market
  /rest/items/{id}/variations/{variationId}/variation_markets/{marketplaceId}:
    delete:
      summary: Delete link between variation and market
      description: Deletes a link between a variation and a market. The ID of the
        item, the ID of the variation and the ID of the market must be specified.
      operationId: deleteRestItemsVariationsVariationVariationMarketsMarketplace
      x-api-path-slug: restitemsidvariationsvariationidvariation-marketsmarketplaceid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: marketplaceId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Market
  /rest/items/{id}/variations/{variationId}/variation_properties:
    delete:
      summary: Deletes all links between a variation and its property values
      description: Deletes all links between a variation and its property values.
        The ID of the variation must be specified.
      operationId: deleteRestItemsVariationsVariationVariationProperties
      x-api-path-slug: restitemsidvariationsvariationidvariation-properties-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - S
      - ""
      - Links
      - Between
      - Variation
      - Its
      - Property
      - Values
    get:
      summary: List property values linked to a variation
      description: Lists the property values linked to a variation. The ID of the
        item and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationProperties
      x-api-path-slug: restitemsidvariationsvariationidvariation-properties-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Values
      - Linked
      - To
      - Variation
    post:
      summary: Create link between variation and property value
      description: Creates a link between a variation and a property value.
      operationId: postRestItemsVariationsVariationVariationProperties
      x-api-path-slug: restitemsidvariationsvariationidvariation-properties-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_properties
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Property
      - Value
  /rest/items/{id}/variations/{variationId}/variation_properties/{propertyId}:
    delete:
      summary: Delete link between variation and property value
      description: Delete a link between a variation and a property value. The ID
        of the item, the ID of the variation and the ID of the property must be specified.
      operationId: deleteRestItemsVariationsVariationVariationPropertiesProperty
      x-api-path-slug: restitemsidvariationsvariationidvariation-propertiespropertyid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Property
      - Value
    get:
      summary: Get a property value
      description: Gets a property value linked to a variation.
      operationId: getRestItemsVariationsVariationVariationPropertiesProperty
      x-api-path-slug: restitemsidvariationsvariationidvariation-propertiespropertyid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Value
    put:
      summary: Update a property value
      description: Update the data of a property value linked to a variation.
      operationId: putRestItemsVariationsVariationVariationPropertiesProperty
      x-api-path-slug: restitemsidvariationsvariationidvariation-propertiespropertyid-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_properties/{propertyId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Value
  /rest/items/{id}/variations/{variationId}/variation_sales_prices:
    delete:
      summary: Delete all links between a variation and its sales prices
      description: Deletes all links between a variation and its sales prices and
        deletes the sales price data. The ID of the variation must be specified.
      operationId: deleteRestItemsVariationsVariationVariationSalesPrices
      x-api-path-slug: restitemsidvariationsvariationidvariation-sales-prices-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Links
      - Between
      - Variation
      - Its
      - Sales
      - Prices
    get:
      summary: List sales prices of a variation
      description: Lists the sales prices of a variation. The ID of the variation
        must be specified.
      operationId: getRestItemsVariationsVariationVariationSalesPrices
      x-api-path-slug: restitemsidvariationsvariationidvariation-sales-prices-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Sales
      - Prices
      - Of
      - Variation
    post:
      summary: Create link between variation and sales price
      description: Creates a link between a variation and a sales price and adds sales
        price data.
      operationId: postRestItemsVariationsVariationVariationSalesPrices
      x-api-path-slug: restitemsidvariationsvariationidvariation-sales-prices-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_sales_prices
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Sales
      - Price
  /rest/items/{id}/variations/{variationId}/variation_sales_prices/{priceId}:
    delete:
      summary: Delete link between variation and sales price
      description: Deletes a link between a variation and a sales price and deletes
        the sales price data. The ID of the sales price and the ID of the variation
        must be specified.
      operationId: deleteRestItemsVariationsVariationVariationSalesPricesPrice
      x-api-path-slug: restitemsidvariationsvariationidvariation-sales-pricespriceid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: priceId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Sales
      - Price
    get:
      summary: Get sales price data for a variation
      description: Gets sales price data linked to a variation. The ID of the sales
        price and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationSalesPricesPrice
      x-api-path-slug: restitemsidvariationsvariationidvariation-sales-pricespriceid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: priceId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
      - Dataa
      - Variation
    put:
      summary: Update sales price data
      description: Updates sales price data linked to a variation. The ID of the sales
        price and the ID of the variation must be specified.
      operationId: putRestItemsVariationsVariationVariationSalesPricesPrice
      x-api-path-slug: restitemsidvariationsvariationidvariation-sales-pricespriceid-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_sales_prices/{priceId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: priceId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
      - Data
  /rest/items/{id}/variations/{variationId}/variation_skus:
    get:
      summary: List SKUs
      description: Lists the SKUs of a variation. Filters must be specified.
      operationId: getRestItemsVariationsVariationVariationSkus
      x-api-path-slug: restitemsidvariationsvariationidvariation-skus-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - SKUs
    post:
      summary: Create an SKU
      description: Creates an SKU. The ID of the variation must be specified.
      operationId: postRestItemsVariationsVariationVariationSkus
      x-api-path-slug: restitemsidvariationsvariationidvariation-skus-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_skus
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - SKU
  /rest/items/{id}/variations/{variationId}/variation_skus/{skuId}:
    delete:
      summary: Delete an SKU
      description: Deletes an SKU. The ID of the SKU must be specified.
      operationId: deleteRestItemsVariationsVariationVariationSkusSku
      x-api-path-slug: restitemsidvariationsvariationidvariation-skusskuid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: skuId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - SKU
    get:
      summary: Get an SKU
      description: Gets an SKU. The ID of the SKU must be specified.
      operationId: getRestItemsVariationsVariationVariationSkusSku
      x-api-path-slug: restitemsidvariationsvariationidvariation-skusskuid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: skuId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - SKU
    put:
      summary: Update an SKU
      description: Updates an SKU. The ID of the SKU must be specified.
      operationId: putRestItemsVariationsVariationVariationSkusSku
      x-api-path-slug: restitemsidvariationsvariationidvariation-skusskuid-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_skus/{skuId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: skuId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - SKU
  /rest/items/{id}/variations/{variationId}/variation_suppliers:
    get:
      summary: Lists suppliers for a variation
      description: Lists all supplier data linked to a variation. The ID of the variation
        must be specified.
      operationId: getRestItemsVariationsVariationVariationSuppliers
      x-api-path-slug: restitemsidvariationsvariationidvariation-suppliers-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Suppliersa
      - Variation
    post:
      summary: Create a link between variation and supplier
      description: Creates a link between a variation and a supplier and adds supplier
        data.
      operationId: postRestItemsVariationsVariationVariationSuppliers
      x-api-path-slug: restitemsidvariationsvariationidvariation-suppliers-post
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Supplier
  /rest/items/{id}/variations/{variationId}/variation_suppliers/{variationSupplierId}:
    delete:
      summary: Delete link between variation and supplier
      description: Deletes a link between a variation and a supplier. The ID of the
        variation and the ID of the link between the variation and the supplier must
        be specified.
      operationId: deleteRestItemsVariationsVariationVariationSuppliersVariationsupplier
      x-api-path-slug: restitemsidvariationsvariationidvariation-suppliersvariationsupplierid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      - in: path
        name: variationSupplierId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Supplier
    get:
      summary: Get supplier data for a variation
      description: Gets the data for a supplier linked to a variation. The ID of the
        variation and the ID of the link between the variation and the supplier must
        be specified.
      operationId: getRestItemsVariationsVariationVariationSuppliersVariationsupplier
      x-api-path-slug: restitemsidvariationsvariationidvariation-suppliersvariationsupplierid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      - in: path
        name: variationSupplierId
      responses:
        200:
          description: OK
      tags:
      - Supplier
      - Dataa
      - Variation
    put:
      summary: Updates supplier data for a variation
      description: Updates the data of a supplier linked to a variation.
      operationId: putRestItemsVariationsVariationVariationSuppliersVariationsupplier
      x-api-path-slug: restitemsidvariationsvariationidvariation-suppliersvariationsupplierid-put
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      - in: path
        name: variationSupplierId
      responses:
        200:
          description: OK
      tags:
      - S
      - Supplier
      - Dataa
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_warehouses:
    get:
      summary: List the warehouses linked to a variation
      description: Lists the warehouses linked to a variation. The ID of the item
        and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationWarehouses
      x-api-path-slug: restitemsidvariationsvariationidvariation-warehouses-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Warehouses
      - Linked
      - To
      - Variation
    post:
      summary: Create link between a variation and a warehouse
      description: Creates a link between a variation and a warehouse and adds warehouse
        data.
      operationId: postRestItemsVariationsVariationVariationWarehouses
      x-api-path-slug: restitemsidvariationsvariationidvariation-warehouses-post
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Variation
      - Warehouse
  /rest/items/{id}/variations/{variationId}/variation_warehouses/{warehouseId}:
    delete:
      summary: Delete link between a warehouse and a variation
      description: Deletes the link between a warehouse and a variation. The ID of
        the variation and the ID of the warehouse must be specified.
      operationId: deleteRestItemsVariationsVariationVariationWarehousesWarehouse
      x-api-path-slug: restitemsidvariationsvariationidvariation-warehouseswarehouseid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Warehouse
      - Variation
    get:
      summary: Get warehouse data for a variation
      description: Gets the data of a warehouse linked to a variation. The ID of the
        variation and the ID of the warehouse must be specified.
      operationId: getRestItemsVariationsVariationVariationWarehousesWarehouse
      x-api-path-slug: restitemsidvariationsvariationidvariation-warehouseswarehouseid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Dataa
      - Variation
    put:
      summary: Update warehouse data of a variation
      description: Updates the data of a warehouse linked to a variation. The ID of
        the variation and the ID of the warehouse must be specified.
      operationId: putRestItemsVariationsVariationVariationWarehousesWarehouse
      x-api-path-slug: restitemsidvariationsvariationidvariation-warehouseswarehouseid-put
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Data
      - Of
      - Variation
  /rest/items/{itemId}:
    delete:
      summary: Delete an item
      description: Deletes an item. The ID of the item must be specified.
      operationId: deleteRestItemsItem
      x-api-path-slug: restitemsitemid-delete
      parameters:
      - in: path
        name: itemId
      responses:
        200:
          description: OK
      tags:
      - Item
    get:
      summary: Show an item
      description: Show an item by itemId
      operationId: getRestItemsItem
      x-api-path-slug: restitemsitemid-get
      parameters:
      - in: path
        name: itemId
      - in: query
        name: lang
        description: The language of the variation information
      responses:
        200:
          description: OK
      tags:
      - Show
      - Item
    put:
      summary: Update a item
      description: Updates a item. The ID of the item must be specified.
      operationId: putRestItemsItem
      x-api-path-slug: restitemsitemid-put
      parameters:
      - in: body
        name: /rest/items/{itemId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: itemId
      responses:
        200:
          description: OK
      tags:
      - Item
  /rest/items/{itemId}/item_shipping_profiles:
    delete:
      summary: Deactivate shipping profiles of an item
      description: Deactivates all shipping profiles of an item. The ID of the item
        must be specified.
      operationId: deleteRestItemsItemItemShippingProfiles
      x-api-path-slug: restitemsitemiditem-shipping-profiles-delete
      parameters:
      - in: path
        name: itemId
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Shipping
      - Profiles
      - Of
      - Item
    get:
      summary: List shipping profiles of an item
      description: Lists the shipping profiles linked to an item. The ID of the item
        must be specified.
      operationId: getRestItemsItemItemShippingProfiles
      x-api-path-slug: restitemsitemiditem-shipping-profiles-get
      parameters:
      - in: path
        name: itemId
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Profiles
      - Of
      - Item
    post:
      summary: Activate a shipping profile
      description: Links a shipping profile to the item. The ID of the item and the
        ID of the shipping profile must be specified.
      operationId: postRestItemsItemItemShippingProfiles
      x-api-path-slug: restitemsitemiditem-shipping-profiles-post
      parameters:
      - in: path
        name: itemId
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Shipping
      - Profile
  /rest/items/{itemId}/item_shipping_profiles/{id}:
    delete:
      summary: Deactivate a shipping profile
      description: Unlinks a shipping profile from the item. The ID of the item must
        be specified.
      operationId: deleteRestItemsItemItemShippingProfiles
      x-api-path-slug: restitemsitemiditem-shipping-profilesid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: itemId
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Shipping
      - Profile
  /rest/items/{itemId}/variations:
    get:
      summary: List variations of an item
      description: Lists all variations of an item. The ID of the item must be specified.
      operationId: getRestItemsItemVariations
      x-api-path-slug: restitemsitemidvariations-get
      parameters:
      - in: query
        name: barcode
        description: Filter restricts the list of results to variations with the specified
          barcode
      - in: query
        name: createdBetween
        description: Filter restricts the list of results to variations created during
          the specified period
      - in: query
        name: isActive
        description: Filter restricts the list of results to variations that are active
      - in: query
        name: isBundle
        description: Filter restricts the list of results to variations to which variations
          were added to create a bundle
      - in: query
        name: isMain
        description: Filter restricts the list of results to variations that are main
          variations
      - in: path
        name: itemId
      - in: query
        name: itemsPerPage
        description: Limits the number of results listed per page to a specific number
      - in: query
        name: lang
        description: The language of the variation information
      - in: query
        name: manufacturerId
        description: Filter restricts the list of results to variations with the specified
          manufacturer ID
      - in: query
        name: numberExact
        description: Filter restricts the list of results to the variation with the
          variation number specified
      - in: query
        name: numberFuzzy
        description: Filter restricts the list of results to variations with numbers
          that contain the variation number specified (SQL LIKE operator)
      - in: query
        name: page
        description: Limits the results to a specific page
      - in: query
        name: relatedUpdatedBetween
        description: Filter restricts the list of results to those variations for
          which related information was updated during the specified period
      - in: query
        name: supplierNumber
        description: Filter restricts the list of results to variations with the specified
          supplier number
      - in: query
        name: updatedBetween
        description: Filter restricts the list of results to variations updated during
          the specified period
      - in: query
        name: with
        description: Includes the specified variation information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Variations
      - Of
      - Item
    post:
      summary: Create a variation
      description: Create a variation. The ID of the item must be specified.
      operationId: postRestItemsItemVariations
      x-api-path-slug: restitemsitemidvariations-post
      parameters:
      - in: body
        name: /rest/items/{itemId}/variations
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: itemId
      responses:
        200:
          description: OK
      tags:
      - Variation
  /rest/items/{itemId}/variations/{variationId}:
    delete:
      summary: Delete a variation
      description: Delete a variation. The ID of the item and the ID of the variation
        must be specified.
      operationId: deleteRestItemsItemVariationsVariation
      x-api-path-slug: restitemsitemidvariationsvariationid-delete
      parameters:
      - in: path
        name: itemId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
    get:
      summary: Get a variation
      description: Get a variation. The ID of the item and the ID of the variation
        must be specified.
      operationId: getRestItemsItemVariationsVariation
      x-api-path-slug: restitemsitemidvariationsvariationid-get
      parameters:
      - in: path
        name: itemId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
    put:
      summary: Update a variation
      description: Updates a variation. The ID of the variation must be specified.
      operationId: putRestItemsItemVariationsVariation
      x-api-path-slug: restitemsitemidvariationsvariationid-put
      parameters:
      - in: body
        name: /rest/items/{itemId}/variations/{variationId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: itemId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
  /rest/items/{itemId}/variations/{variationId}/variation_properties/{propertyId}/texts:
    get:
      summary: Get property value texts
      description: Gets the texts saved for a specific property of the type Text in
        all available languages. The ID of the property must be specified.
      operationId: getRestItemsItemVariationsVariationVariationPropertiesPropertyTexts
      x-api-path-slug: restitemsitemidvariationsvariationidvariation-propertiespropertyidtexts-get
      parameters:
      - in: path
        name: itemId
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Value
      - Texts
    post:
      summary: Create property value text by language
      description: Saves text for a specific property of the type Text in the specified
        language. The ID of the property and the language must be specified.
      operationId: postRestItemsItemVariationsVariationVariationPropertiesPropertyTexts
      x-api-path-slug: restitemsitemidvariationsvariationidvariation-propertiespropertyidtexts-post
      parameters:
      - in: body
        name: /rest/items/{itemId}/variations/{variationId}/variation_properties/{propertyId}/texts
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: itemId
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Value
      - Text
      - By
      - Language
  /rest/items/{itemId}/variations/{variationId}/variation_properties/{propertyId}/texts/{lang}:
    delete:
      summary: Delete property value text by language
      description: Deletes the text saved for a specific property of the type Text
        in the specified language. The ID of the property  and the language must be
        specified.
      operationId: deleteRestItemsItemVariationsVariationVariationPropertiesPropertyTextsLang
      x-api-path-slug: restitemsitemidvariationsvariationidvariation-propertiespropertyidtextslang-delete
      parameters:
      - in: path
        name: itemId
      - in: path
        name: lang
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Value
      - Text
      - By
      - Language
    get:
      summary: Get property value text by language
      description: Gets the value text saved for a specific property of the type Text
        in the specified language. The ID of the property  and the language must be
        specified.
      operationId: getRestItemsItemVariationsVariationVariationPropertiesPropertyTextsLang
      x-api-path-slug: restitemsitemidvariationsvariationidvariation-propertiespropertyidtextslang-get
      parameters:
      - in: path
        name: itemId
      - in: path
        name: lang
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Value
      - Text
      - By
      - Language
    put:
      summary: Update property value text by language
      description: Updates the text saved for a specific property of the type Text
        in the specified language. The ID of the property and the language must be
        specified.
      operationId: putRestItemsItemVariationsVariationVariationPropertiesPropertyTextsLang
      x-api-path-slug: restitemsitemidvariationsvariationidvariation-propertiespropertyidtextslang-put
      parameters:
      - in: body
        name: /rest/items/{itemId}/variations/{variationId}/variation_properties/{propertyId}/texts/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: itemId
      - in: path
        name: lang
      - in: path
        name: propertyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Value
      - Text
      - By
      - Language
  /rest/languages/translations:
    post:
      summary: Create a new translation
      description: Creates a new translation.
      operationId: postRestLanguagesTranslations
      x-api-path-slug: restlanguagestranslations-post
      parameters:
      - in: query
        name: $fileName
        description: The of the file
      - in: query
        name: $key
        description: The translation key
      - in: query
        name: $languageCode
        description: The language code for the translation
      - in: query
        name: $pluginName
        description: The name of the plugin
      - in: query
        name: $pluginSetId
        description: The ID of the plugin set
      - in: query
        name: $value
        description: The value of the translation
      responses:
        200:
          description: OK
      tags:
      - New
      - Translation
  /rest/languages/translations/{translationId}:
    delete:
      summary: Delete a translation
      description: Deletes a translation. The ID of the translation must be specified.
      operationId: deleteRestLanguagesTranslationsTranslation
      x-api-path-slug: restlanguagestranslationstranslationid-delete
      parameters:
      - in: query
        name: $translationId
        description: The ID of the translation
      - in: path
        name: translationId
      responses:
        200:
          description: OK
      tags:
      - Translation
    get:
      summary: Get a translation
      description: Gets a translation. The ID of the translation must be specified.
      operationId: getRestLanguagesTranslationsTranslation
      x-api-path-slug: restlanguagestranslationstranslationid-get
      parameters:
      - in: query
        name: $id
        description: The ID of the translation
      - in: path
        name: translationId
      responses:
        200:
          description: OK
      tags:
      - Translation
    put:
      summary: Update a translation
      description: Updates a translation. The ID of the translation must be specified
      operationId: putRestLanguagesTranslationsTranslation
      x-api-path-slug: restlanguagestranslationstranslationid-put
      parameters:
      - in: query
        name: $fileName
        description: The value of the translation
      - in: query
        name: $id
        description: The ID of the translation
      - in: query
        name: $key
        description: The translation key
      - in: query
        name: $languageCode
        description: The language code for the translation
      - in: query
        name: $pluginName
        description: The name of the plugin
      - in: query
        name: $pluginSetId
        description: The ID of the plugin set
      - in: query
        name: $value
        description: The value of the translation
      - in: path
        name: translationId
      responses:
        200:
          description: OK
      tags:
      - Translation
  /rest/legalinformation/{plentyId}/{lang}/{type}:
    get:
      summary: Get legal information of an online store
      description: Gets legal information of an online store. The plenty ID of the
        store , the language and the type of legal information must be specified.
        The language must be specified as ISO 639-1 code.
      operationId: getRestLegalinformationPlentyLangType
      x-api-path-slug: restlegalinformationplentyidlangtype-get
      parameters:
      - in: path
        name: lang
      - in: path
        name: plentyId
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Legal
      - Information
      - Of
      - Online
      - Store
    put:
      summary: Save legal information for an online store
      description: |-
        Saves a legal information for an online store. The plenty ID of the online store, the language of the legal information and the type of the legal information must be specified. The language must be specified as ISO 639-1 code.
        Existing legal information will be overwritten.
      operationId: putRestLegalinformationPlentyLangType
      x-api-path-slug: restlegalinformationplentyidlangtype-put
      parameters:
      - in: body
        name: /rest/legalinformation/{plentyId}/{lang}/{type}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lang
      - in: path
        name: plentyId
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Save
      - Legal
      - Informationan
      - Online
      - Store
  /rest/listings:
    get:
      summary: List listing
      description: Lists listings by filter options.
      operationId: getRestListings
      x-api-path-slug: restlistings-get
      parameters:
      - in: query
        name: id
        description: Filter that restricts the search result to listings with specific
          listing ID
      - in: query
        name: itemId
        description: Filter that restricts the search result to listings with specific
          item ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: stockDependenceTypeId
        description: Filter that restricts the search result to listings with specific
          stock dependence type ID
      - in: query
        name: typeId
        description: Filter that restricts the search result to listings with specific
          type ID
      - in: query
        name: unitCombinationId
        description: Filter that restricts the search result to listings with specific
          unit combination ID
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
    post:
      summary: Create new listing
      description: Creates a new listing.
      operationId: postRestListings
      x-api-path-slug: restlistings-post
      parameters:
      - in: body
        name: /rest/listings
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Listing
  /rest/listings/layout_templates:
    post:
      summary: Create new layout template
      description: Creates a new layout template.
      operationId: postRestListingsLayoutTemplates
      x-api-path-slug: restlistingslayout-templates-post
      parameters:
      - in: body
        name: /rest/listings/layout_templates
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Layout
      - Template
  /rest/listings/layout_templates/{id}:
    delete:
      summary: Delete a layout template
      description: Deletes a layout template by ID.
      operationId: deleteRestListingsLayoutTemplates
      x-api-path-slug: restlistingslayout-templatesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Layout
      - Template
    get:
      summary: Get a layout template
      description: Gets a layout template by providing its ID.
      operationId: getRestListingsLayoutTemplates
      x-api-path-slug: restlistingslayout-templatesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Layout
      - Template
  /rest/listings/markets:
    get:
      summary: List listing markets
      description: Lists listing market by filter options.
      operationId: getRestListingsMarkets
      x-api-path-slug: restlistingsmarkets-get
      parameters:
      - in: query
        name: credentialsId
        description: Filter that restricts the search result to listing markets with
          given credential ID
      - in: query
        name: directoryId
        description: Filter that restricts the search result to listing markets with
          a given directory ID
      - in: query
        name: duration
        description: Filter that restricts the search result to listing markets with
          given duration
      - in: query
        name: id
        description: Filter that restricts the search result to listing markets that
          match the given ID(s)
      - in: query
        name: itemId
        description: Filter that restricts the search result to listing markets that
          belong to a given item ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: listingId
        description: Filter that restricts the search result to listing markets that
          belong to a given listing ID
      - in: query
        name: listingTypeId
        description: Filter that restricts the search result to listing markets that
          belong to a listing of a custom type ID
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referrerId
        description: Filter that restricts the search result to listing markets with
          given referrer ID
      - in: query
        name: shippingProfileId
        description: Filter that restricts the search result to listing markets that
          belong to a given shipping profile ID
      - in: query
        name: status
        description: Filter that restricts the search result to listing markets with
          a custom status condition
      - in: query
        name: stockCondition
        description: Filter that restricts the search result to listing markets with
          a custom stock condition
      - in: query
        name: stockDependenceTypeId
        description: Filter that restricts the search result to listing markets that
          belong to a listing with a custom stock dependence type ID
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to listing markets that
          were last updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to listing markets that
          were last updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to listing markets that
          match the given variation ID(s)
      - in: query
        name: variations
        description: Filter that restricts the search result to listing markets with
          a custom variation condition
      - in: query
        name: verified
        description: Filter that restricts the search result to listing markets that
          are verified
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Markets
    post:
      summary: Create new listing market
      description: |-
        Creates a new listing market. Based on the given options this call can create multiple listing markets. If the
        'optionTemplateId' parameter is provided and the listing option template includes options for different markets
        than one listing market will be created for each market.
      operationId: postRestListingsMarkets
      x-api-path-slug: restlistingsmarkets-post
      parameters:
      - in: body
        name: /rest/listings/markets
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Listing
      - Market
  /rest/listings/markets/directories:
    get:
      summary: Get all listing market directories
      description: Gets all listing market directories.
      operationId: getRestListingsMarketsDirectories
      x-api-path-slug: restlistingsmarketsdirectories-get
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Directories
    post:
      summary: Create listing market directory
      description: Creates a listing market directory.
      operationId: postRestListingsMarketsDirectories
      x-api-path-slug: restlistingsmarketsdirectories-post
      parameters:
      - in: body
        name: /rest/listings/markets/directories
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Directory
  /rest/listings/markets/directories/{id}:
    delete:
      summary: Delete listing market directory
      description: Deletes a listing market directory by ID.
      operationId: deleteRestListingsMarketsDirectories
      x-api-path-slug: restlistingsmarketsdirectoriesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Directory
    get:
      summary: Get a listing market directory
      description: Gets a listing market directory by ID.
      operationId: getRestListingsMarketsDirectories
      x-api-path-slug: restlistingsmarketsdirectoriesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Directory
    put:
      summary: Update listing market directory
      description: Updates a listing market directory by ID.
      operationId: putRestListingsMarketsDirectories
      x-api-path-slug: restlistingsmarketsdirectoriesid-put
      parameters:
      - in: body
        name: /rest/listings/markets/directories/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Directory
  /rest/listings/markets/find:
    get:
      summary: Find listing markets
      description: Lists listing market by filter options.
      operationId: getRestListingsMarketsFind
      x-api-path-slug: restlistingsmarketsfind-get
      parameters:
      - in: query
        name: credentialsId
        description: Filter that restricts the search result to listing markets with
          given credential ID
      - in: query
        name: directoryId
        description: Filter that restricts the search result to listing markets with
          a given directory ID
      - in: query
        name: id
        description: Filter that restricts the search result to listing markets that
          match the given ID(s)
      - in: query
        name: itemId
        description: Filter that restricts the search result to listing markets that
          belong to a given item ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referrerId
        description: Filter that restricts the search result to listing markets with
          given referrer ID
      - in: query
        name: shippingProfileId
        description: Filter that restricts the search result to listing markets that
          belong to a given shipping profile ID
      - in: query
        name: variations
        description: Filter that restricts the search result to listing markets with
          a custom variation condition
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Find
      - Listing
      - Markets
  /rest/listings/markets/histories:
    get:
      summary: List listing market history
      description: Lists listing market history by filter options.
      operationId: getRestListingsMarketsHistories
      x-api-path-slug: restlistingsmarketshistories-get
      parameters:
      - in: query
        name: credentialsId
        description: Filter that restricts the search result to listing market histories
          with given credential ID
      - in: query
        name: directoryId
        description: Filter that restricts the search result to listing market histories
          with a given directory ID
      - in: query
        name: duration
        description: Filter that restricts the search result to listing market histories
          with given duration
      - in: query
        name: externalId
        description: Filter that restricts the search result to listing market histories
          with given external id
      - in: query
        name: firstPlatformCategoryId
        description: Filter that restricts the search result to listing market histories
          with first platform category ID equal to the given ID
      - in: query
        name: firstShopCategoryId
        description: Filter that restricts the search result to listing market histories
          with first shop category ID equal to the given ID
      - in: query
        name: isClickAndCollect
        description: Filter that restricts the search result to listing market histories
          that belong to eBay Click & Collect
      - in: query
        name: isEbayPlus
        description: Filter that restricts the search result to listing market histories
          that belong to eBay Plus
      - in: query
        name: itemId
        description: Filter that restricts the search result to listing market histories
          that belong to a given item ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: lastSale
        description: Filter that restricts the search result to listing market histories
          with last sale before given date
      - in: query
        name: listingId
        description: Filter that restricts the search result to listing market histories
          that belong to a given listing ID
      - in: query
        name: listingMarketId
        description: Filter that restricts the search result to listing market histories
          that match the given listing market ID(s)
      - in: query
        name: listingTypeId
        description: Filter that restricts the search result to listing market histories
          that belong to a listing of a custom type ID
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referrerId
        description: Filter that restricts the search result to listing market histories
          with given referrer ID
      - in: query
        name: secondPlatformCategoryId
        description: Filter that restricts the search result to listing market histories
          with second platform category ID equal to the given ID
      - in: query
        name: secondShopCategoryId
        description: Filter that restricts the search result to listing market histories
          with second shop category ID equal to the given ID
      - in: query
        name: shippingProfileId
        description: Filter that restricts the search result to listing market histories
          that belong to a given shipping profile
      - in: query
        name: statusId
        description: Filter that restricts the search result to listing market histories
          with a custom status status ID
      - in: query
        name: stockCondition
        description: Filter that restricts the search result to listing market histories
          with a custom stock condition
      - in: query
        name: stockDependenceTypeId
        description: Filter that restricts the search result to listing market histories
          that belong to a listing with a custom stock dependence type ID
      - in: query
        name: textData
        description: Filter that restricts the search result to listing market histories
          that match given text in listing title or description
      - in: query
        name: thirdShopCategoryId
        description: Filter that restricts the search result to listing market histories
          with third shop category ID equal to the given ID
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to listing market histories
          that were last updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to listing market histories
          that were last updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to listing market histories
          that match the given variation ID(s)
      - in: query
        name: variations
        description: Filter that restricts the search result to listing market histories
          with a custom variation condition
      - in: query
        name: verified
        description: Filter that restricts the search result to listing market histories
          that are verified
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Market
      - History
  /rest/listings/markets/histories/end/{id?}:
    delete:
      summary: End the listing
      description: Ends the listing on the designated market.
      operationId: deleteRestListingsMarketsHistoriesEnd
      x-api-path-slug: restlistingsmarketshistoriesendid-delete
      parameters:
      - in: query
        name: deleteOnSuccess
        description: Tells if the listing market history should also be deleted from
          the database
      - in: query
        name: id
        description: The ID of the listing market history that needs to be ended
      - in: path
        name: id?
      responses:
        200:
          description: OK
      tags:
      - End
      - Listing
  /rest/listings/markets/histories/relist/{id?}:
    post:
      summary: Relist the listing
      description: Relists the listing on the designated market.
      operationId: postRestListingsMarketsHistoriesRelist
      x-api-path-slug: restlistingsmarketshistoriesrelistid-post
      parameters:
      - in: query
        name: id
        description: The ID of the listing market history that needs to be relisted
      - in: path
        name: id?
      responses:
        200:
          description: OK
      tags:
      - Relist
      - Listing
  /rest/listings/markets/histories/update/{id?}:
    put:
      summary: Update listing market histories
      description: |-
        Updates listing market histories by given update options. The listing market histories are not directly revised,
        they are added to the batch processing lists, waiting to be revised by automated background processes.
      operationId: putRestListingsMarketsHistoriesUpdate
      x-api-path-slug: restlistingsmarketshistoriesupdateid-put
      parameters:
      - in: query
        name: id
        description: The ID of the listing market history that needs to be ended
      - in: path
        name: id?
      - in: query
        name: options
        description: Multiple update options
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Histories
  /rest/listings/markets/histories/{id}:
    get:
      summary: Get a listing market history
      description: Gets a listing market history by given ID.
      operationId: getRestListingsMarketsHistories
      x-api-path-slug: restlistingsmarketshistoriesid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - History
  /rest/listings/markets/infos:
    get:
      summary: Search listing market info
      description: Search listing market info by filter options.
      operationId: getRestListingsMarketsInfos
      x-api-path-slug: restlistingsmarketsinfos-get
      parameters:
      - in: query
        name: code
        description: Filter that restricts the search result to listing market info
          with given codes
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to listing markets that
          were last updated on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to listing markets that
          were last updated within a specified period of time
      - in: query
        name: id
        description: Filter that restricts the search result to listing market info
          that match the given ID(s)
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: listingMarketId
        description: Filter that restricts the search result to listing market info
          that match the given listing market ID(s)
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: type
        description: Filter that restricts the search result to listing market info
          with a custom type
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Search
      - Listing
      - Market
      - Info
  /rest/listings/markets/item_specifics:
    get:
      summary: Gets all ListingMarketItemSpecifics.
      description: Can be filtered by ID, listingMarketId, name and value.
      operationId: getRestListingsMarketsItemSpecifics
      x-api-path-slug: restlistingsmarketsitem-specifics-get
      parameters:
      - in: body
        name: /rest/listings/markets/item_specifics
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - ""
      - ListingMarketItemSpecifics
  /rest/listings/markets/item_specifics/{id}:
    delete:
      summary: Deletes a ListingMarketItemSpecific.
      description: Deletes a listingmarketitemspecific..
      operationId: deleteRestListingsMarketsItemSpecifics
      x-api-path-slug: restlistingsmarketsitem-specificsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - S
      - ListingMarketItemSpecific
    get:
      summary: Gets a ListingMarketItemSpecific.
      description: Gets a listingmarketitemspecific..
      operationId: getRestListingsMarketsItemSpecifics
      x-api-path-slug: restlistingsmarketsitem-specificsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - S
      - ListingMarketItemSpecific
    put:
      summary: Updates a ListingMarketItemSpecific.
      description: Updates a listingmarketitemspecific..
      operationId: putRestListingsMarketsItemSpecifics
      x-api-path-slug: restlistingsmarketsitem-specificsid-put
      parameters:
      - in: body
        name: /rest/listings/markets/item_specifics/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - S
      - ListingMarketItemSpecific
  /rest/listings/markets/start/{id?}:
    post:
      summary: Start the market listing on the designated market.
      description: Starts the market listing on the designated markets.
      operationId: postRestListingsMarketsStart
      x-api-path-slug: restlistingsmarketsstartid-post
      parameters:
      - in: query
        name: distribution
        description: The number of minutes that the listing should be started
      - in: query
        name: id
        description: The ID of the listing market that needs to be started
      - in: path
        name: id?
      - in: query
        name: startAt
        description: When should the listings be started
      responses:
        200:
          description: OK
      tags:
      - Start
      - Market
      - Listing
      - "On"
      - Designated
      - Market
  /rest/listings/markets/texts:
    get:
      summary: List listing market texts
      description: Lists listing market texts by filter options.
      operationId: getRestListingsMarketsTexts
      x-api-path-slug: restlistingsmarketstexts-get
      parameters:
      - in: query
        name: contains
        description: Filter that restricts the search result to listing market texts
          which title, subtitle or description contain the given value
      - in: query
        name: id
        description: Filter that restricts the search result to listing market texts
          with specific ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: language
        description: Filter that restricts the search result to listing market texts
          for a specific language
      - in: query
        name: listingMarketId
        description: Filter that restricts the search result to listing market texts
          with specific listing market IDs
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Market
      - Texts
    post:
      summary: Create a listing market text
      description: Creates a listing market text for a given listing market ID. If
        an entry with same data already exists the request will be ignored and the
        old entry will be returned.
      operationId: postRestListingsMarketsTexts
      x-api-path-slug: restlistingsmarketstexts-post
      parameters:
      - in: body
        name: /rest/listings/markets/texts
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: listingMarketId
        description: The listing market ID this text belongs to
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Text
  /rest/listings/markets/texts/{id}:
    delete:
      summary: Delete a listing market text
      description: Deletes a listing market text for a given listing market text ID.
      operationId: deleteRestListingsMarketsTexts
      x-api-path-slug: restlistingsmarketstextsid-delete
      parameters:
      - in: path
        name: id
      - in: query
        name: lang
        description: The listing market text language that should be updated
      - in: query
        name: listingMarketId
        description: The listing market ID this text belongs to
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Text
    get:
      summary: Get a listing market text
      description: Gets a listing market text by providing its ID.
      operationId: getRestListingsMarketsTexts
      x-api-path-slug: restlistingsmarketstextsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Text
  /rest/listings/markets/texts/{listingMarketId}/{lang}:
    put:
      summary: Update a listing market text
      description: Updates a listing market text for a given listing market ID and
        language.
      operationId: putRestListingsMarketsTextsListingmarketLang
      x-api-path-slug: restlistingsmarketstextslistingmarketidlang-put
      parameters:
      - in: body
        name: /rest/listings/markets/texts/{listingMarketId}/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lang
      - in: path
        name: listingMarketId
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - Text
  /rest/listings/markets/verify/{id?}:
    post:
      summary: Verify listing markets
      description: Verifies the listing markets.
      operationId: postRestListingsMarketsVerify
      x-api-path-slug: restlistingsmarketsverifyid-post
      parameters:
      - in: query
        name: id
        description: The ID of the listing market that need to be verified
      - in: path
        name: id?
      responses:
        200:
          description: OK
      tags:
      - Verify
      - Listing
      - Markets
  /rest/listings/markets/{id}:
    delete:
      summary: Delete listing market
      description: Deletes a listing market by ID.
      operationId: deleteRestListingsMarkets
      x-api-path-slug: restlistingsmarketsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
    get:
      summary: Get a listing market
      description: Gets a listing market by given ID.
      operationId: getRestListingsMarkets
      x-api-path-slug: restlistingsmarketsid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
    put:
      summary: Update a listing market
      description: Updates a listing market by ID.
      operationId: putRestListingsMarkets
      x-api-path-slug: restlistingsmarketsid-put
      parameters:
      - in: body
        name: /rest/listings/markets/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: query
        name: referrerId
        description: The referrer ID
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
  /rest/listings/option_templates:
    post:
      summary: Create option template
      description: Creates an option template.
      operationId: postRestListingsOptionTemplates
      x-api-path-slug: restlistingsoption-templates-post
      parameters:
      - in: body
        name: /rest/listings/option_templates
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Option
      - Template
  /rest/listings/option_templates/preview:
    get:
      summary: Get a preview list of option templates
      description: Gets a preview list of all available listing option templates.
      operationId: getRestListingsOptionTemplatesPreview
      x-api-path-slug: restlistingsoption-templatespreview-get
      responses:
        200:
          description: OK
      tags:
      - Preview
      - List
      - Of
      - Option
      - Templates
  /rest/listings/option_templates/{id}:
    delete:
      summary: Delete option template
      description: Deletes an option template by ID.
      operationId: deleteRestListingsOptionTemplates
      x-api-path-slug: restlistingsoption-templatesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Option
      - Template
    get:
      summary: Get option template
      description: Gets an option template by ID.
      operationId: getRestListingsOptionTemplates
      x-api-path-slug: restlistingsoption-templatesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Option
      - Template
    put:
      summary: Update option template
      description: Updates an option template by ID.
      operationId: putRestListingsOptionTemplates
      x-api-path-slug: restlistingsoption-templatesid-put
      parameters:
      - in: body
        name: /rest/listings/option_templates/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Option
      - Template
  /rest/listings/shipping_profiles:
    get:
      summary: List listing shipping profiles
      description: Lists listing shipping profiles.
      operationId: getRestListingsShippingProfiles
      x-api-path-slug: restlistingsshipping-profiles-get
      parameters:
      - in: query
        name: credentialsId
        description: Filter that restricts the search result to listing shipping profiles
          with given credential ID(s)
      - in: query
        name: id
        description: Filter that restricts the search result to listing shipping profiles
          that match the given ID(s)
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referrerId
        description: Filter that restricts the search result to listing shipping profiles
          with given referrer ID(s)
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Shipping
      - Profiles
  /rest/listings/shipping_profiles/{id}:
    get:
      summary: Get a shipping profile
      description: Gets a shipping profile by providing its ID.
      operationId: getRestListingsShippingProfiles
      x-api-path-slug: restlistingsshipping-profilesid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Profile
  /rest/listings/stock_dependence_types:
    get:
      summary: List listing stock dependence types
      description: Lists listing stock dependence types.
      operationId: getRestListingsStockDependenceTypes
      x-api-path-slug: restlistingsstock-dependence-types-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Stock
      - Dependence
      - Types
  /rest/listings/stock_dependence_types/{id}:
    get:
      summary: Get a listing stock dependence type
      description: Gets a listing stock dependence type by given ID.
      operationId: getRestListingsStockDependenceTypes
      x-api-path-slug: restlistingsstock-dependence-typesid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Stock
      - Dependence
      - Type
  /rest/listings/types:
    get:
      summary: List listing types
      description: Lists all listing types.
      operationId: getRestListingsTypes
      x-api-path-slug: restlistingstypes-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Types
  /rest/listings/types/{id}:
    get:
      summary: Get a listing type
      description: Gets a listing type by given ID.
      operationId: getRestListingsTypes
      x-api-path-slug: restlistingstypesid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Type
  /rest/listings/{id}:
    delete:
      summary: Delete a listing
      description: Deletes a listing by given ID.
      operationId: deleteRestListings
      x-api-path-slug: restlistingsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
    get:
      summary: Get a listing
      description: Gets a listing by given ID.
      operationId: getRestListings
      x-api-path-slug: restlistingsid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Listing
    put:
      summary: Update a listing
      description: Updates a listing by given ID.
      operationId: putRestListings
      x-api-path-slug: restlistingsid-put
      parameters:
      - in: body
        name: /rest/listings/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listing
  /rest/login:
    post:
      summary: Login
      description: Logs in to plentymarkets with your back end user credentials. The
        login call returns a JSON object that contains information, such as the access
        token and the refresh token.
      operationId: postRestLogin
      x-api-path-slug: restlogin-post
      parameters:
      - in: body
        name: /rest/login
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Login
  /rest/login/refresh:
    post:
      summary: Refresh
      description: Refreshes the access token using the refresh token. The refresh
        token is part of the login call response.
      operationId: postRestLoginRefresh
      x-api-path-slug: restloginrefresh-post
      responses:
        200:
          description: OK
      tags:
      - Refresh
  /rest/logout:
    post:
      summary: Logout
      description: Logs out the back end user from plentymarkets. The access token
        expires.
      operationId: postRestLogout
      x-api-path-slug: restlogout-post
      responses:
        200:
          description: OK
      tags:
      - Logout
  /rest/logs:
    get:
      summary: Perform a search operation.
      description: Perform a search operation..
      operationId: getRestLogs
      x-api-path-slug: restlogs-get
      parameters:
      - in: query
        name: additionalInfo
        description: Filter that restricts the search result to log entries that match
          an additional info
      - in: query
        name: code
        description: Filter that restricts the search result to log entries with a
          custom code
      - in: query
        name: fromDate
        description: Filter that restricts the search result to log entries created
          after this date
      - in: query
        name: identifier
        description: Filter that restricts the search result to log entries with custom
          identifier(s)
      - in: query
        name: integration
        description: Filter that restricts the search result to log entries with custom
          integration key(s)
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: level
        description: Filter that restricts the search result to log entries of a custom
          level
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referenceType
        description: Filter that restricts the search result to log entries with custom
          reference types
      - in: query
        name: referenceValue
        description: Filter that restricts the search result to log entries with custom
          reference values
      - in: query
        name: toDate
        description: Filter that restricts the search result to log entries created
          before this date
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Perform
      - Search
      - Operation
    post:
      summary: Create a log entry.
      description: Create a log entry..
      operationId: postRestLogs
      x-api-path-slug: restlogs-post
      parameters:
      - in: body
        name: /rest/logs
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Log
      - Entry
  /rest/logs/integration_keys:
    get:
      summary: ""
      description: .
      operationId: getRestLogsIntegrationKeys
      x-api-path-slug: restlogsintegration-keys-get
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/logs/reference_types:
    get:
      summary: Get all registered reference types.
      description: Get all registered reference types..
      operationId: getRestLogsReferenceTypes
      x-api-path-slug: restlogsreference-types-get
      responses:
        200:
          description: OK
      tags:
      - Registered
      - Reference
      - Types
  /rest/logs/settings:
    get:
      summary: Show config.
      description: Show config..
      operationId: getRestLogsSettings
      x-api-path-slug: restlogssettings-get
      responses:
        200:
          description: OK
      tags:
      - Show
      - Config
    post:
      summary: Save config.
      description: Save config..
      operationId: postRestLogsSettings
      x-api-path-slug: restlogssettings-post
      responses:
        200:
          description: OK
      tags:
      - Save
      - Config
  /rest/logs/{id}:
    get:
      summary: Get Log entry by ID.
      description: Get log entry by id..
      operationId: getRestLogs
      x-api-path-slug: restlogsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Log
      - Entry
      - By
      - ID
  /rest/markets/credentials:
    get:
      summary: List credentials
      description: List credentials.
      operationId: getRestMarketsCredentials
      x-api-path-slug: restmarketscredentials-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The items per page to search for
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Credentials
    post:
      summary: Create a credential
      description: Create a new credential with the given data.
      operationId: postRestMarketsCredentials
      x-api-path-slug: restmarketscredentials-post
      parameters:
      - in: body
        name: /rest/markets/credentials
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Credential
  /rest/markets/credentials/{credentialsId}:
    delete:
      summary: Delete a credential
      description: Deletes a credential by given ID.
      operationId: deleteRestMarketsCredentialsCredentials
      x-api-path-slug: restmarketscredentialscredentialsid-delete
      parameters:
      - in: path
        name: credentialsId
      - in: query
        name: id
        description: The ID of the credentials to be deleted
      responses:
        200:
          description: OK
      tags:
      - Credential
    get:
      summary: Get a credential
      description: Get a credential.
      operationId: getRestMarketsCredentialsCredentials
      x-api-path-slug: restmarketscredentialscredentialsid-get
      parameters:
      - in: path
        name: credentialsId
      - in: query
        name: id
        description: The ID of the credentials to be found
      responses:
        200:
          description: OK
      tags:
      - Credential
    put:
      summary: Update a credential
      description: Update a credential with the given data and ID.
      operationId: putRestMarketsCredentialsCredentials
      x-api-path-slug: restmarketscredentialscredentialsid-put
      parameters:
      - in: body
        name: /rest/markets/credentials/{credentialsId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: credentialsId
      responses:
        200:
          description: OK
      tags:
      - Credential
  /rest/markets/ebay/auth/login:
    get:
      summary: Get the login url.
      description: Get the login url..
      operationId: getRestMarketsEbayAuthLogin
      x-api-path-slug: restmarketsebayauthlogin-get
      responses:
        200:
          description: OK
      tags:
      - Login
      - Url
  /rest/markets/ebay/auth/refresh-token:
    put:
      summary: Refresh an expired access token.
      description: Refresh an expired access token..
      operationId: putRestMarketsEbayAuthRefreshToken
      x-api-path-slug: restmarketsebayauthrefreshtoken-put
      responses:
        200:
          description: OK
      tags:
      - Refresh
      - Expired
      - Access
      - Token
  /rest/markets/ebay/categories:
    get:
      summary: List categories
      description: Lists categories. By passing category ID as filter, only subcategories
        of that category will be returned. The marketplace ID filter is required.
      operationId: getRestMarketsEbayCategories
      x-api-path-slug: restmarketsebaycategories-get
      parameters:
      - in: query
        name: categoryId
        description: Filter that restricts the search result to categories that belong
          to the specified category ID
      - in: query
        name: marketplaceId
        description: Filter that restricts the search result to categories that belong
          to the specified marketplace ID
      responses:
        200:
          description: OK
      tags:
      - List
      - Categories
  /rest/markets/ebay/categories/{id}:
    get:
      summary: Get category
      description: Get category for given ID.
      operationId: getRestMarketsEbayCategories
      x-api-path-slug: restmarketsebaycategoriesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Category
  /rest/markets/ebay/fulfillment_policies/{id}:
    get:
      summary: Get fulfillment policy
      description: Get fulfillment policy for given ID.
      operationId: getRestMarketsEbayFulfillmentPolicies
      x-api-path-slug: restmarketsebayfulfillment-policiesid-get
      parameters:
      - in: query
        name: credentialsId
        description: The ID of credentials for which to get the policy
      - in: path
        name: id
      - in: query
        name: marketplaceId
        description: The ID of the marketplace for which to get the policy
      responses:
        200:
          description: OK
      tags:
      - Fulfillment
      - Policy
  /rest/markets/ebay/item_specifics:
    get:
      summary: List item specifics
      description: List item specifics for a given category Id and referrerId.
      operationId: getRestMarketsEbayItemSpecifics
      x-api-path-slug: restmarketsebayitem-specifics-get
      parameters:
      - in: query
        name: categoryId
        description: The ID of the category for which to list item specifics
      - in: query
        name: marketplaceId
        description: Filter that restricts the search result to categories that belong
          to the specified marketplace ID
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Specifics
  /rest/markets/ebay/marketplaces:
    get:
      summary: Get all eBay marketplaces.
      description: List eBay marketplaces. Use filters to find specific ones.
      operationId: getRestMarketsEbayMarketplaces
      x-api-path-slug: restmarketsebaymarketplaces-get
      parameters:
      - in: query
        name: marketId
        description: Get only marketplaces that match the given market ID
      - in: query
        name: marketplaceId
        description: Get only marketplaces that match the given marketplace ID
      - in: query
        name: referrerId
        description: Get only marketplaces that match the given referrer ID
      - in: query
        name: siteId
        description: Get only marketplaces that match the given site ID
      responses:
        200:
          description: OK
      tags:
      - EBay
      - Marketplaces
  /rest/markets/ebay/parts-fitments:
    get:
      summary: List fitments
      description: Lists fitments.
      operationId: getRestMarketsEbayPartsFitments
      x-api-path-slug: restmarketsebaypartsfitments-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Fitments
    post:
      summary: Create a fitment
      description: Create a new fitment for the given data.
      operationId: postRestMarketsEbayPartsFitments
      x-api-path-slug: restmarketsebaypartsfitments-post
      parameters:
      - in: body
        name: /rest/markets/ebay/parts-fitments
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Fitment
  /rest/markets/ebay/parts-fitments/search:
    get:
      summary: Search fitments
      description: Search fitments by filter options.
      operationId: getRestMarketsEbayPartsFitmentsSearch
      x-api-path-slug: restmarketsebaypartsfitmentssearch-get
      parameters:
      - in: query
        name: categoryId
        description: Filter that restricts the search result to fitments with specific
          eBay category ID
      - in: query
        name: id
        description: Filter that restricts the search result to fitments with specific
          ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: marketId
        description: Filter that restricts the search result to fitments with specific
          market ID
      - in: query
        name: name
        description: Filter that restricts the search result to fitments with specific
          name
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: propertyName
        description: Filter that restricts the search result to fitments with specific
          property name
      - in: query
        name: propertyValue
        description: Filter that restricts the search result to fitments with specific
          property value
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Search
      - Fitments
  /rest/markets/ebay/parts-fitments/{fitmentId}:
    delete:
      summary: Delete a fitment.
      description: Deletes a fitment. The ID of the fitment must be specified.
      operationId: deleteRestMarketsEbayPartsFitmentsFitment
      x-api-path-slug: restmarketsebaypartsfitmentsfitmentid-delete
      parameters:
      - in: path
        name: fitmentId
      - in: query
        name: id
        description: The fitment ID
      responses:
        200:
          description: OK
      tags:
      - Fitment
    get:
      summary: Get a fitment
      description: Gets a fitment. The id of the fitment must be specified.
      operationId: getRestMarketsEbayPartsFitmentsFitment
      x-api-path-slug: restmarketsebaypartsfitmentsfitmentid-get
      parameters:
      - in: path
        name: fitmentId
      - in: query
        name: id
        description: The fitment ID
      responses:
        200:
          description: OK
      tags:
      - Fitment
    put:
      summary: Update fitment.
      description: Updates a fitment. Items that do not occur anymore will be replaced.
      operationId: putRestMarketsEbayPartsFitmentsFitment
      x-api-path-slug: restmarketsebaypartsfitmentsfitmentid-put
      parameters:
      - in: body
        name: /rest/markets/ebay/parts-fitments/{fitmentId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: fitmentId
      - in: query
        name: id
        description: The ID of the fitment list
      responses:
        200:
          description: OK
      tags:
      - Fitment
  /rest/markets/ebay/payment_policies/{id}:
    get:
      summary: Get payment policy
      description: Get payment policy for given ID.
      operationId: getRestMarketsEbayPaymentPolicies
      x-api-path-slug: restmarketsebaypayment-policiesid-get
      parameters:
      - in: query
        name: credentialsId
        description: The ID of credentials for which to get the policy
      - in: path
        name: id
      - in: query
        name: marketplaceId
        description: The ID of the marketplace for which to get the policy
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Policy
  /rest/markets/ebay/return_policies/{id}:
    get:
      summary: Get return policy
      description: Get return policy for given ID.
      operationId: getRestMarketsEbayReturnPolicies
      x-api-path-slug: restmarketsebayreturn-policiesid-get
      parameters:
      - in: query
        name: credentialsId
        description: The ID of credentials for which to get the policy
      - in: path
        name: id
      - in: query
        name: marketplaceId
        description: The ID of the marketplace for which to get the policy
      responses:
        200:
          description: OK
      tags:
      - Return
      - Policy
  /rest/markets/ebay/shop_categories:
    get:
      summary: List all eBay shop categories
      description: Lists all eBay shop categories.
      operationId: getRestMarketsEbayShopCategories
      x-api-path-slug: restmarketsebayshop-categories-get
      parameters:
      - in: query
        name: credentialsId
        description: The credentials ID for whom to fetch eBay shop categories
      - in: query
        name: viewType
        description: How should the eBay shop categories be returned
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - EBay
      - Shop
      - Categories
  /rest/markets/settings:
    get:
      summary: List market settings
      description: Lists market settings. The marketplace ID and the type must be
        specified.
      operationId: getRestMarketsSettings
      x-api-path-slug: restmarketssettings-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Market
      - Settings
    post:
      summary: Create market settings
      description: Creates new market settings by given data. The marketplace ID and
        the type must be specified.
      operationId: postRestMarketsSettings
      x-api-path-slug: restmarketssettings-post
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
  /rest/markets/settings/bulk:
    post:
      summary: Create market settings
      description: Creates new market settings by given data. The marketplace ID and
        the type must be specified.
      operationId: postRestMarketsSettingsBulk
      x-api-path-slug: restmarketssettingsbulk-post
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
    put:
      summary: Update market settings
      description: Updates market settings. The market settings ID must be specified.
      operationId: putRestMarketsSettingsBulk
      x-api-path-slug: restmarketssettingsbulk-put
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
  /rest/markets/settings/correlations:
    get:
      summary: List correlation
      description: Lists correlations. The type, the market settings ID and the correlation
        ID must be specified.
      operationId: getRestMarketsSettingsCorrelations
      x-api-path-slug: restmarketssettingscorrelations-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Correlation
    post:
      summary: Create a correlation
      description: Creates a correlation. The type, the market settings ID and the
        correlation ID must be specified.
      operationId: postRestMarketsSettingsCorrelations
      x-api-path-slug: restmarketssettingscorrelations-post
      responses:
        200:
          description: OK
      tags:
      - Correlation
  /rest/markets/settings/correlations/bulk:
    post:
      summary: Create multiple correlations
      description: Creates multiple correlations. The type, market settings ID and
        the correlation ID for each param combination must be specified.
      operationId: postRestMarketsSettingsCorrelationsBulk
      x-api-path-slug: restmarketssettingscorrelationsbulk-post
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Correlations
  /rest/markets/settings/{settingId}:
    delete:
      summary: Delete market settings
      description: Deletes market settings. The market settings ID must be specified.
      operationId: deleteRestMarketsSettingsSetting
      x-api-path-slug: restmarketssettingssettingid-delete
      parameters:
      - in: path
        name: settingId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
    get:
      summary: Get market settings
      description: Gets market settings. The market settings ID must be specified.
      operationId: getRestMarketsSettingsSetting
      x-api-path-slug: restmarketssettingssettingid-get
      parameters:
      - in: path
        name: settingId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
    put:
      summary: Update market settings
      description: Updates market settings. The market settings ID must be specified.
      operationId: putRestMarketsSettingsSetting
      x-api-path-slug: restmarketssettingssettingid-put
      parameters:
      - in: path
        name: settingId
      responses:
        200:
          description: OK
      tags:
      - Market
      - Settings
  /rest/newsletters:
    delete:
      summary: Delete entries
      description: Delete entries.
      operationId: deleteRestNewsletters
      x-api-path-slug: restnewsletters-delete
      responses:
        200:
          description: OK
      tags:
      - Entries
    get:
      summary: List newsletter entries
      description: List newsletter entries.
      operationId: getRestNewsletters
      x-api-path-slug: restnewsletters-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Newsletter
      - Entries
    post:
      summary: Create an entry
      description: Create an entry.
      operationId: postRestNewsletters
      x-api-path-slug: restnewsletters-post
      parameters:
      - in: body
        name: /rest/newsletters
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: body
        description: The body of the newsletter entry
      - in: query
        name: kind
        description: The type of the entry
      - in: query
        name: subject
        description: The subject of the newsletter entry
      responses:
        200:
          description: OK
      tags:
      - Entry
  /rest/newsletters/folders:
    delete:
      summary: Delete folders
      description: Delete folders.
      operationId: deleteRestNewslettersFolders
      x-api-path-slug: restnewslettersfolders-delete
      responses:
        200:
          description: OK
      tags:
      - Folders
    get:
      summary: List newsletter folders
      description: List newsletter folders.
      operationId: getRestNewslettersFolders
      x-api-path-slug: restnewslettersfolders-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Newsletter
      - Folders
    post:
      summary: Create a folder
      description: Create a folder.
      operationId: postRestNewslettersFolders
      x-api-path-slug: restnewslettersfolders-post
      parameters:
      - in: body
        name: /rest/newsletters/folders
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: The ID of the newsletter folder
      - in: query
        name: isDeletable
        description: Flag that indicates if the newsletter folder can be deleted
      - in: query
        name: isSelectable
        description: Flag that indicates if the newsletter folder can be selected
          by customers in the online store
      - in: query
        name: name
        description: The name of the newsletter folder
      - in: query
        name: position
        description: The position of the newsletter folder
      responses:
        200:
          description: OK
      tags:
      - Folder
  /rest/newsletters/folders/{folderId}:
    delete:
      summary: Delete a folder
      description: Deletes a folder. The ID of the folder must be specified.
      operationId: deleteRestNewslettersFoldersFolder
      x-api-path-slug: restnewslettersfoldersfolderid-delete
      parameters:
      - in: path
        name: folderId
      responses:
        200:
          description: OK
      tags:
      - Folder
    get:
      summary: List details of a folder
      description: Lists details of a folder. The ID of the folder must be specified.
      operationId: getRestNewslettersFoldersFolder
      x-api-path-slug: restnewslettersfoldersfolderid-get
      parameters:
      - in: path
        name: folderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Details
      - Of
      - Folder
    put:
      summary: Update a folder
      description: Updates a folder. The ID of the folder must be specified.
      operationId: putRestNewslettersFoldersFolder
      x-api-path-slug: restnewslettersfoldersfolderid-put
      parameters:
      - in: query
        name: clientIds
        description: The IDs of the clients (stores)
      - in: path
        name: folderId
      - in: query
        name: isDeletable
        description: Flag that indicates if the newsletter folder can be deleted
      - in: query
        name: isSelectable
        description: Flag that indicates if the newsletter folder can be selected
          by customers in the online store
      - in: query
        name: name
        description: The name of the newsletter folder
      - in: query
        name: position
        description: The position of the newsletter folder
      responses:
        200:
          description: OK
      tags:
      - Folder
  /rest/newsletters/folders/{folderId}/recipients:
    get:
      summary: List all recipients of a folder
      description: Lists all recipients of a folder. The ID of the folder must be
        specified.
      operationId: getRestNewslettersFoldersFolderRecipients
      x-api-path-slug: restnewslettersfoldersfolderidrecipients-get
      parameters:
      - in: path
        name: folderId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Recipients
      - Of
      - Folder
  /rest/newsletters/list_recipients:
    get:
      summary: List recipients
      description: List recipients.
      operationId: getRestNewslettersListRecipients
      x-api-path-slug: restnewsletterslist-recipients-get
      parameters:
      - in: query
        name: columns
        description: Filter that restricts the search result to specific columns
      - in: query
        name: folderId
        description: Filter that restricts the search result to a specific folderId
      - in: query
        name: isConfirmed
        description: Filter that restricts the search result to confirmed recipients
      - in: query
        name: itemsPerPage
        description: The number of orders to be displayed per page
      - in: query
        name: page
        description: The page to get
      - in: query
        name: with
        description: Load additional relations for a Recipient
      responses:
        200:
          description: OK
      tags:
      - List
      - Recipients
  /rest/newsletters/recipients:
    delete:
      summary: Delete recipients
      description: Delete recipients.
      operationId: deleteRestNewslettersRecipients
      x-api-path-slug: restnewslettersrecipients-delete
      responses:
        200:
          description: OK
      tags:
      - Recipients
    get:
      summary: List recipients of a folder
      description: List recipients of a folder.
      operationId: getRestNewslettersRecipients
      x-api-path-slug: restnewslettersrecipients-get
      parameters:
      - in: query
        name: email
        description: Filter that restricts the search result to the email address
          of the recipient
      - in: query
        name: folderId
        description: Filter that restricts the search result to the folder ID
      - in: query
        name: recipientId
        description: Filter that restricts the search result to the recipient ID
      responses:
        200:
          description: OK
      tags:
      - List
      - Recipients
      - Of
      - Folder
    post:
      summary: Create a recipient
      description: Create a recipient.
      operationId: postRestNewslettersRecipients
      x-api-path-slug: restnewslettersrecipients-post
      parameters:
      - in: body
        name: /rest/newsletters/recipients
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: email
        description: The email address of the recipient
      - in: query
        name: firstName
        description: The first name of the recipient
      - in: query
        name: folderIds
        description: The IDs of the newsletter folders
      - in: query
        name: ignoreVisibility
        description: Value that indicates if the REST call considers folders without
          visibility
      - in: query
        name: ipAddress
        description: The IP address from where the customer has confirmed the newsletter
      - in: query
        name: isFrontend
        description: Value that indicates if the REST call was retrieved from the
          front end
      - in: query
        name: lastName
        description: The last name of the recipient
      responses:
        200:
          description: OK
      tags:
      - Recipient
  /rest/newsletters/recipients/{recipientId}:
    delete:
      summary: Delete a recipient
      description: Deletes a recipient. The ID of the recipient must be specified.
      operationId: deleteRestNewslettersRecipientsRecipient
      x-api-path-slug: restnewslettersrecipientsrecipientid-delete
      parameters:
      - in: path
        name: recipientId
      responses:
        200:
          description: OK
      tags:
      - Recipient
    get:
      summary: List a recipient
      description: Lists a recipient. The ID of the recipient must be specified.
      operationId: getRestNewslettersRecipientsRecipient
      x-api-path-slug: restnewslettersrecipientsrecipientid-get
      parameters:
      - in: path
        name: recipientId
      - in: query
        name: recipientsId
        description: The ID of the newsletter folder
      responses:
        200:
          description: OK
      tags:
      - List
      - Recipient
    put:
      summary: Update a recipient
      description: Updates a recipient that is assigned to a folder. The ID of the
        recipient must be specified.
      operationId: putRestNewslettersRecipientsRecipient
      x-api-path-slug: restnewslettersrecipientsrecipientid-put
      parameters:
      - in: body
        name: /rest/newsletters/recipients/{recipientId}
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: birthday
        description: The customer birthday as Date string (e
      - in: query
        name: email
        description: The email address of the newsletter recipient
      - in: query
        name: firstName
        description: The first name of the newsletter recipient
      - in: query
        name: folderId
        description: The ID of the newsletter folder
      - in: query
        name: folderIds
        description: 'DEPRECATED: The IDs of the newsletter folders'
      - in: query
        name: gender
        description: 'The gender of the customer, one of the following values: m,f'
      - in: query
        name: ipAddress
        description: The IP address from where the customer has confirmed the newsletter
      - in: query
        name: lastName
        description: The last name of the newsletter recipient
      - in: path
        name: recipientId
      responses:
        200:
          description: OK
      tags:
      - Recipient
  /rest/newsletters/{entryId}:
    delete:
      summary: Delete an entry
      description: Deletes an entry. The ID of the entry must be specified.
      operationId: deleteRestNewslettersEntry
      x-api-path-slug: restnewslettersentryid-delete
      parameters:
      - in: path
        name: entryId
      responses:
        200:
          description: OK
      tags:
      - Entry
    get:
      summary: List details of an entry
      description: Lists details of an entry. The ID of the entry must be specified.
      operationId: getRestNewslettersEntry
      x-api-path-slug: restnewslettersentryid-get
      parameters:
      - in: path
        name: entryId
      responses:
        200:
          description: OK
      tags:
      - List
      - Details
      - Of
      - Entry
    put:
      summary: Update an entry
      description: Updates an entry. The ID of the entry must be specified.
      operationId: putRestNewslettersEntry
      x-api-path-slug: restnewslettersentryid-put
      parameters:
      - in: query
        name: body
        description: The body of the entry
      - in: path
        name: entryId
      - in: query
        name: kind
        description: The type of the entry
      - in: query
        name: subject
        description: The subject of the entry
      responses:
        200:
          description: OK
      tags:
      - Entry
  /rest/orders:
    get:
      summary: List orders by filter options
      description: List orders by filter options.
      operationId: getRestOrders
      x-api-path-slug: restorders-get
      parameters:
      - in: query
        name: clientId
        description: Filter that restricts the search result to order from one client
      - in: query
        name: contactId
        description: Filter that restricts the search result to orders of one order
          contact
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to orders that were created
          on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to orders that were created
          within a certain period of time
      - in: query
        name: externalOrderId
        description: Filter that restricts the search result to an external order
          id
      - in: query
        name: hasDocument
        description: Filter that restricts the search result to orders which hold
          the given document type
      - in: query
        name: includedItem
        description: Filter that restricts the search result to orders with a certain
          item
      - in: query
        name: includedVariation
        description: Filter that restricts the search result to orders with a certain
          variation
      - in: query
        name: isEbayPlus
        description: Filter that restricts the search result to orders with ebay plus
      - in: query
        name: itemsPerPage
        description: The number of orders to be displayed per page
      - in: query
        name: orderIds
        description: Filter that restricts the search result to orders
      - in: query
        name: orderType
        description: Filter that restricts the search result to orders of specific
          order types
      - in: query
        name: outgoingItemsBookedAtFrom
        description: Filter that restricts the search result to orders where the outgoing
          items were booked on the specified date
      - in: query
        name: outgoingItemsBookedAtTo
        description: Filter that restricts the search result to orders where the outgoing
          items were booked within a specified period of time
      - in: query
        name: ownerUserId
        description: Filter that restricts the search result to orders of one owner
      - in: query
        name: page
        description: The page to get
      - in: query
        name: paidAtFrom
        description: Filter that restricts the search result to orders that received
          a payment on the specified date
      - in: query
        name: paidAtTo
        description: Filter that restricts the search result to orders that received
          a payment within a certain period of time
      - in: query
        name: paymentStatus
        description: Filter that restricts the search result to order with a specific
          payment status
      - in: query
        name: referrerId
        description: Filter that restricts the search result to orders from one order
          referrer
      - in: query
        name: shippingProfileId
        description: Filter that restricts the search result to orders with a specific
          shipping profile
      - in: query
        name: statusFrom
        description: Filter that restricts the search result to orders in a specific
          order status
      - in: query
        name: statusTo
        description: Filter that restricts the search result to orders within a range
          of order statuses
      - in: query
        name: supplierId
        description: Filter that restricts the search result to orders that include
          order items with variations from a supplier
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to orders that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to orders that were last
          updated within a specified period of time
      - in: query
        name: warehouseId
        description: Filter that restricts the search result to orders with a specific
          main warehouse
      - in: query
        name: with
        description: Load additional relations for an order
      responses:
        200:
          description: OK
      tags:
      - List
      - Orders
      - By
      - Filter
      - Options
    post:
      summary: Create an order
      description: Create an order.
      operationId: postRestOrders
      x-api-path-slug: restorders-post
      parameters:
      - in: body
        name: /rest/orders
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Order
  /rest/orders/addresses:
    post:
      summary: Create an address for existing order
      description: Creates an address for an existing order.
      operationId: postRestOrdersAddresses
      x-api-path-slug: restordersaddresses-post
      responses:
        200:
          description: OK
      tags:
      - Addressexisting
      - Order
  /rest/orders/contacts/{contactId}:
    get:
      summary: List orders of a contact
      description: Lists all orders of a contact. The ID of the contact must be specified.
      operationId: getRestOrdersContactsContact
      x-api-path-slug: restorderscontactscontactid-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: itemsPerPage
        description: The number of orders to be displayed per page
      - in: query
        name: page
        description: The page to get
      - in: query
        name: with
        description: Load additional relations for an order
      responses:
        200:
          description: OK
      tags:
      - List
      - Orders
      - Of
      - Contact
  /rest/orders/contacts/{contactId}/multi_order:
    post:
      summary: Create a multi-order
      description: "Creates a multi-order for a contact. The ID of the contact must
        be specified. Options chosen in the System \xBB Orders \xBB Order types \xBB
        Multi-order menu are relevant for this call."
      operationId: postRestOrdersContactsContactMultiOrder
      x-api-path-slug: restorderscontactscontactidmulti-order-post
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Multi-order
  /rest/orders/coupons/campaigns/codes/{code}:
    delete:
      summary: Delete a coupon
      description: Deletes a coupon by the coupon code.
      operationId: deleteRestOrdersCouponsCampaignsCodesCode
      x-api-path-slug: restorderscouponscampaignscodescode-delete
      parameters:
      - in: path
        name: code
      - in: query
        name: withoutUsed
        description: Do not delete used coupons
      responses:
        200:
          description: OK
      tags:
      - Coupon
    get:
      summary: Get coupon code information
      description: Gets coupon code information. The code must be specified.
      operationId: getRestOrdersCouponsCampaignsCodesCode
      x-api-path-slug: restorderscouponscampaignscodescode-get
      parameters:
      - in: path
        name: code
      - in: query
        name: with
        description: Load additional relations for a coupon code
      responses:
        200:
          description: OK
      tags:
      - Coupon
      - Code
      - Information
  /rest/orders/coupons/campaigns/codes/{code}/disabled/{isDisabled}:
    put:
      summary: Disable or enable coupon
      description: Sets the coupon disable field.
      operationId: putRestOrdersCouponsCampaignsCodesCodeDisabledIsdisabled
      x-api-path-slug: restorderscouponscampaignscodescodedisabledisdisabled-put
      parameters:
      - in: path
        name: code
      - in: path
        name: isDisabled
      responses:
        200:
          description: OK
      tags:
      - Disable
      - Enable
      - Coupon
  /rest/orders/coupons/campaigns/{campaignId}/codes:
    post:
      summary: Create a coupon code
      description: Creates a coupon code. The ID of the campaign must be specified.
        A code can optionally be specified. A random code will be generated if the
        code is not specified. A coupon value can also be optionally specified. The
        value of the campaign will be used if no individual value is specified.
      operationId: postRestOrdersCouponsCampaignsCampaignCodes
      x-api-path-slug: restorderscouponscampaignscampaignidcodes-post
      parameters:
      - in: body
        name: /rest/orders/coupons/campaigns/{campaignId}/codes
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: campaignId
      responses:
        200:
          description: OK
      tags:
      - Coupon
      - Code
  /rest/orders/coupons/codes/contacts/{contactId}:
    get:
      summary: List redeemed coupon codes of a contact
      description: Lists the redeemed coupon codes of contact. The ID of the contact
        must be specified.
      operationId: getRestOrdersCouponsCodesContactsContact
      x-api-path-slug: restorderscouponscodescontactscontactid-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: itemsPerPage
        description: The number of coupons to be displayed per page
      - in: query
        name: page
        description: The page to get
      responses:
        200:
          description: OK
      tags:
      - List
      - Redeemed
      - Coupon
      - Codes
      - Of
      - Contact
  /rest/orders/coupons/codes/{coupon}:
    post:
      summary: Validate a coupon
      description: Validates if a coupon code can be used for the specified items,
        contact ID, etc. The code must be specified. If the coupon code is invalid,
        a ValidationException will be thrown. If the coupon code is valid, a CouponCodeValidation
        object will be returned.
      operationId: postRestOrdersCouponsCodesCoupon
      x-api-path-slug: restorderscouponscodescoupon-post
      parameters:
      - in: body
        name: /rest/orders/coupons/codes/{coupon}
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: callFromScheduler
        description: Flag that indicates whether the validation is requested by a
          subscription order or not
      - in: query
        name: contactClass
        description: The contact class
      - in: query
        name: contactType
        description: The contact type
      - in: path
        name: coupon
      - in: query
        name: plentyId
        description: The plenty id
      - in: query
        name: shipToCountry
        description: The country of delivery
      - in: query
        name: taxIdNumber
        description: The tax id number
      responses:
        200:
          description: OK
      tags:
      - Validate
      - Coupon
  /rest/orders/currencies:
    get:
      summary: List currencies
      description: List currencies.
      operationId: getRestOrdersCurrencies
      x-api-path-slug: restorderscurrencies-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Currencies
  /rest/orders/currencies/countries/{countryId}:
    get:
      summary: Get a currency for a country
      description: Get a currency for a country. The ID of the country must be specified.
      operationId: getRestOrdersCurrenciesCountriesCountry
      x-api-path-slug: restorderscurrenciescountriescountryid-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: path
        name: countryId
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - Currencya
      - Country
  /rest/orders/currencies/{currencyIso}:
    get:
      summary: Get a currency
      description: Get a currency. The ISO 4217 code of the currency must be specified.
      operationId: getRestOrdersCurrenciesCurrencyiso
      x-api-path-slug: restorderscurrenciescurrencyiso-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: path
        name: currencyIso
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - Currency
  /rest/orders/currencies/{currencyIso}/countries:
    get:
      summary: List countries for a currency
      description: List countries for a currency. The ISO 4271 code of the currency
        must be specified.
      operationId: getRestOrdersCurrenciesCurrencyisoCountries
      x-api-path-slug: restorderscurrenciescurrencyisocountries-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: path
        name: currencyIso
      responses:
        200:
          description: OK
      tags:
      - List
      - Countriesa
      - Currency
  /rest/orders/dates/types:
    get:
      summary: List order date types
      description: List order date types.
      operationId: getRestOrdersDatesTypes
      x-api-path-slug: restordersdatestypes-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Date
      - Types
  /rest/orders/dates/types/{typeId}:
    get:
      summary: Find an order date type by it's ID
      description: Find an order date type by it's id.
      operationId: getRestOrdersDatesTypesType
      x-api-path-slug: restordersdatestypestypeid-get
      parameters:
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Find
      - Order
      - Date
      - Type
      - By
      - Its
      - ID
  /rest/orders/dates/types/{typeId}/names:
    get:
      summary: List names of an order date type
      description: Lists names in all languages available of an order date type. The
        ID of the date type must be specified.
      operationId: getRestOrdersDatesTypesTypeNames
      x-api-path-slug: restordersdatestypestypeidnames-get
      parameters:
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
      - Of
      - Order
      - Date
      - Type
  /rest/orders/dates/types/{typeId}/names/{lang}:
    get:
      summary: Get a name of an order date type
      description: Gets a name of an order date type. The ID of the date type and
        the language of the name must be specified.
      operationId: getRestOrdersDatesTypesTypeNamesLang
      x-api-path-slug: restordersdatestypestypeidnameslang-get
      parameters:
      - in: path
        name: lang
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Name
      - Of
      - Order
      - Date
      - Type
  /rest/orders/documents/accounting_summary:
    get:
      summary: List document accounting summaries
      description: Lists document accounting summaries. A document accounting summary
        is saved along with each reversal document (for invoice and credit note).
        It contains accounting information about the order for this point in time.
        The summary is saved because an order can be updated after a reversal_document
        is generated. The information about the order before the update is needed
        for accounting.
      operationId: getRestOrdersDocumentsAccountingSummary
      x-api-path-slug: restordersdocumentsaccounting-summary-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Get entries with createdAt date after this date
      - in: query
        name: createdAtTo
        description: Get entries with createdAt date before this date
      - in: query
        name: documentType
        description: The document type
      - in: query
        name: itemsPerPage
        description: The number of summaries to be displayed per page
      - in: query
        name: orderId
        description: The ID of the order
      - in: query
        name: page
        description: The page to get
      responses:
        200:
          description: OK
      tags:
      - List
      - Document
      - Accounting
      - Summaries
  /rest/orders/documents/downloads/{type}:
    get:
      summary: Download documents of a document type
      description: Downloads documents of the same document type as a zip file. The
        type of the documents must be specified.
      operationId: getRestOrdersDocumentsDownloadsType
      x-api-path-slug: restordersdocumentsdownloadstype-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to documents that were
          created on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to documents that were
          created within a certain period of time
      - in: query
        name: displayDateFrom
        description: Filter that restricts the search result to documents that were
          displayed on the specified date
      - in: query
        name: displayDateTo
        description: Filter that restricts the search result to documents that were
          displayed within a certain period of time
      - in: query
        name: itemsPerPage
        description: The number of documents to display per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: plentyId
        description: The plenty ID of the order documents
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Download
      - Documents
      - Of
      - Document
      - Type
  /rest/orders/documents/{type}:
    get:
      summary: List documents of a type
      description: Lists documents of a type. The type must be specified.
      operationId: getRestOrdersDocumentsType
      x-api-path-slug: restordersdocumentstype-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to documents that were
          created on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to documents that were
          created within a certain period of time
      - in: query
        name: displayDateFrom
        description: Filter that restricts the search result to documents that were
          displayed on the specified date
      - in: query
        name: displayDateTo
        description: Filter that restricts the search result to documents that were
          displayed within a certain period of time
      - in: query
        name: itemsPerPage
        description: The items per page to search for
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: type
      - in: query
        name: with
        description: Load additional relations for a document
      - in: query
        name: withContent
        description: Load also the document content as base64 encoded string
      responses:
        200:
          description: OK
      tags:
      - List
      - Documents
      - Of
      - Type
  /rest/orders/items/dates:
    post:
      summary: Create a date for an order item
      description: Creates a date for an order item. The ID of the order item must
        be specified
      operationId: postRestOrdersItemsDates
      x-api-path-slug: restordersitemsdates-post
      parameters:
      - in: body
        name: /rest/orders/items/dates
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datean
      - Order
      - Item
  /rest/orders/items/dates/{id}:
    delete:
      summary: Delete a date from an order item
      description: Deletes the date from an order item. The ID of the date must be
        specified.
      operationId: deleteRestOrdersItemsDates
      x-api-path-slug: restordersitemsdatesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Date
      - From
      - Order
      - Item
    get:
      summary: Get a date of an order item
      description: Gets a date of an order item. The ID of the date must be specified.
      operationId: getRestOrdersItemsDates
      x-api-path-slug: restordersitemsdatesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Order
      - Item
    put:
      summary: Update a date of an order item
      description: Updates a date of an order item. The ID of the date must be specified.
      operationId: putRestOrdersItemsDates
      x-api-path-slug: restordersitemsdatesid-put
      parameters:
      - in: body
        name: /rest/orders/items/dates/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Order
      - Item
  /rest/orders/items/properties:
    post:
      summary: Create an order item property.
      description: Create an order item property..
      operationId: postRestOrdersItemsProperties
      x-api-path-slug: restordersitemsproperties-post
      parameters:
      - in: body
        name: /rest/orders/items/properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
  /rest/orders/items/properties/{id}:
    delete:
      summary: Delete an order item property by ID.
      description: Delete an order item property by id..
      operationId: deleteRestOrdersItemsProperties
      x-api-path-slug: restordersitemspropertiesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - ID
    get:
      summary: Get an order item property by ID.
      description: Get an order item property by id..
      operationId: getRestOrdersItemsProperties
      x-api-path-slug: restordersitemspropertiesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - ID
    put:
      summary: Update an order item property by ID.
      description: Update an order item property by id..
      operationId: putRestOrdersItemsProperties
      x-api-path-slug: restordersitemspropertiesid-put
      parameters:
      - in: body
        name: /rest/orders/items/properties/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - ID
  /rest/orders/items/{orderItemId}/dates:
    get:
      summary: List dates of an order item
      description: Lists the dates of an order item. The ID of the order item must
        be specified.
      operationId: getRestOrdersItemsOrderitemDates
      x-api-path-slug: restordersitemsorderitemiddates-get
      parameters:
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - List
      - Dates
      - Of
      - Order
      - Item
  /rest/orders/items/{orderItemId}/dates/{typeId}:
    delete:
      summary: Delete a date from an order item by order item and date type
      description: Deletest a date from an order item. The ID of the order item and
        the ID of the date type must be specified.
      operationId: deleteRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-delete
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Date
      - From
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
    get:
      summary: Get a date of an order item by order item and date type
      description: Gets a date of an order item. The ID of the order item and the
        ID of the date type must be specified.
      operationId: getRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-get
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
    post:
      summary: Create a date for an order item by order item and date type
      description: Creates a date for an order item. The ID of the order item and
        the ID of the date type must be specified.
      operationId: postRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-post
      parameters:
      - in: body
        name: /rest/orders/items/{orderItemId}/dates/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Datean
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
    put:
      summary: Update a date of an order item by order item and date type
      description: Updates the date of an order item. The ID of the order item and
        the ID of the date type must be specified.
      operationId: putRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-put
      parameters:
      - in: body
        name: /rest/orders/items/{orderItemId}/dates/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
  /rest/orders/items/{orderItemId}/properties:
    get:
      summary: Get all order item propertys for one order item by its order item id.
      description: Get all order item propertys for one order item by its order item
        id..
      operationId: getRestOrdersItemsOrderitemProperties
      x-api-path-slug: restordersitemsorderitemidproperties-get
      parameters:
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Propertysone
      - Order
      - Item
      - By
      - Its
      - Order
      - Item
      - Id
  /rest/orders/items/{orderItemId}/properties/{typeId}:
    delete:
      summary: Delete an order item property by order item ID and order property type
        ID.
      description: Delete an order item property by order item id and order property
        type id..
      operationId: deleteRestOrdersItemsOrderitemPropertiesType
      x-api-path-slug: restordersitemsorderitemidpropertiestypeid-delete
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - Order
      - Item
      - ID
      - Order
      - Property
      - Type
      - ID
    get:
      summary: Get an order item property by order item ID and order property type
        ID.
      description: Get an order item property by order item id and order property
        type id..
      operationId: getRestOrdersItemsOrderitemPropertiesType
      x-api-path-slug: restordersitemsorderitemidpropertiestypeid-get
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - Order
      - Item
      - ID
      - Order
      - Property
      - Type
      - ID
    post:
      summary: Create an order item property by order item ID and order property type
        ID.
      description: Create an order item property by order item id and order property
        type id..
      operationId: postRestOrdersItemsOrderitemPropertiesType
      x-api-path-slug: restordersitemsorderitemidpropertiestypeid-post
      parameters:
      - in: body
        name: /rest/orders/items/{orderItemId}/properties/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - Order
      - Item
      - ID
      - Order
      - Property
      - Type
      - ID
    put:
      summary: Update an order item property by order item ID and order property type
        ID.
      description: Update an order item property by order item id and order property
        type id..
      operationId: putRestOrdersItemsOrderitemPropertiesType
      x-api-path-slug: restordersitemsorderitemidpropertiestypeid-put
      parameters:
      - in: body
        name: /rest/orders/items/{orderItemId}/properties/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - Order
      - Item
      - ID
      - Order
      - Property
      - Type
      - ID
  /rest/orders/items/{orderItemId}/transactions:
    get:
      summary: List transactions
      description: Lists transactions for an order item. The ID of the order item
        must be specified.
      operationId: getRestOrdersItemsOrderitemTransactions
      x-api-path-slug: restordersitemsorderitemidtransactions-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: orderItemId
      - in: query
        name: with
        description: Load additional relations for a transaction
      responses:
        200:
          description: OK
      tags:
      - List
      - Transactions
    post:
      summary: Create a transaction
      description: Create a transaction.
      operationId: postRestOrdersItemsOrderitemTransactions
      x-api-path-slug: restordersitemsorderitemidtransactions-post
      parameters:
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - Transaction
  /rest/orders/properties/types:
    get:
      summary: List order property types
      description: Lists property types and their names in all languages. Optionally
        one or more languages can be specified to get a limited response.
      operationId: getRestOrdersPropertiesTypes
      x-api-path-slug: restorderspropertiestypes-get
      parameters:
      - in: query
        name: lang
        description: Languages to be loaded with the type model
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Property
      - Types
    post:
      summary: Create an order property type
      description: Create an order property type.
      operationId: postRestOrdersPropertiesTypes
      x-api-path-slug: restorderspropertiestypes-post
      parameters:
      - in: body
        name: /rest/orders/properties/types
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Order
      - Property
      - Type
  /rest/orders/properties/types/{typeId}:
    delete:
      summary: Delete a property type.
      description: Deletes a property type and all names for it from the database.
        The ID of the type must be specified.
      operationId: deleteRestOrdersPropertiesTypesType
      x-api-path-slug: restorderspropertiestypestypeid-delete
      parameters:
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Type
    get:
      summary: Get a property type
      description: Gets a property type and its names in all languages. Optionally
        one or more languages can be specified to get a limited response.
      operationId: getRestOrdersPropertiesTypesType
      x-api-path-slug: restorderspropertiestypestypeid-get
      parameters:
      - in: query
        name: lang
        description: Languages to be loaded with the type model
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Type
    put:
      summary: Update a property type.
      description: Updates a property type and its names. The ID of the type must
        be specified. You can also create new names, if you provide data which does
        not yet exist.
      operationId: putRestOrdersPropertiesTypesType
      x-api-path-slug: restorderspropertiestypestypeid-put
      parameters:
      - in: body
        name: /rest/orders/properties/types/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Type
  /rest/orders/properties/{id}:
    delete:
      summary: Delete a property of an order by property ID
      description: Deletes a property of an order. The ID of the property must be
        specified.
      operationId: deleteRestOrdersProperties
      x-api-path-slug: restorderspropertiesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Of
      - Order
      - By
      - Property
      - ID
    put:
      summary: Update a property of an order by property ID
      description: Updates the value of a property. The ID of the property must be
        specified.
      operationId: putRestOrdersProperties
      x-api-path-slug: restorderspropertiesid-put
      parameters:
      - in: body
        name: /rest/orders/properties/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Of
      - Order
      - By
      - Property
      - ID
  /rest/orders/referrers:
    get:
      summary: List referrers
      description: Lists referrers with the desired columns/attributes.
      operationId: getRestOrdersReferrers
      x-api-path-slug: restordersreferrers-get
      parameters:
      - in: query
        name: columns
        description: The desired columns/attributes of the order referrer to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Referrers
  /rest/orders/referrers/{parentReferrerId?}:
    post:
      summary: Create an order referrer
      description: |-
        Create an order referrer. The ID can be specified, a parent ID can be specified to create a sub referrer or if no ID is specified, a referrer ID will be assigned automatically.
        If an ID is specified, the ID may not be used already. If the ID is used already, the referrer will only be created.
        If the ID is automatically assigned, the first ID that has not been used before will be set.
        If the ID is not specified, but a parent referrer ID is given, then the new referrer ID will be a sub referrer of the given parent.
      operationId: postRestOrdersReferrersParentreferrer
      x-api-path-slug: restordersreferrersparentreferrerid-post
      parameters:
      - in: query
        name: data
        description: The attributes of the order referrer to be created
      - in: path
        name: parentReferrerId?
      responses:
        200:
          description: OK
      tags:
      - Order
      - Referrer
  /rest/orders/shipping/countries:
    get:
      summary: List shipping countries
      description: List shipping countries.
      operationId: getRestOrdersShippingCountries
      x-api-path-slug: restordersshippingcountries-get
      parameters:
      - in: query
        name: active
        description: Returns only the active shipping countries
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Countries
  /rest/orders/shipping/export_documents/{orderId}:
    get:
      summary: List export documents by order ID
      description: List export documents by order id.
      operationId: getRestOrdersShippingExportDocumentsOrder
      x-api-path-slug: restordersshippingexport-documentsorderid-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Export
      - Documents
      - By
      - Order
      - ID
  /rest/orders/shipping/package_types:
    get:
      summary: List shipping package types
      description: List shipping package types.
      operationId: getRestOrdersShippingPackageTypes
      x-api-path-slug: restordersshippingpackage-types-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Package
      - Types
  /rest/orders/shipping/package_types/{shippingPackageTypeId}:
    get:
      summary: Get a shipping package type
      description: Gets a shipping package type. The ID of the shipping package type
        must be specified.
      operationId: getRestOrdersShippingPackageTypesShippingpackagetype
      x-api-path-slug: restordersshippingpackage-typesshippingpackagetypeid-get
      parameters:
      - in: path
        name: shippingPackageTypeId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Package
      - Type
  /rest/orders/shipping/parcel_service_regions/{parcelServiceRegionId}:
    get:
      summary: Get an  order parcel service region
      description: Gets an parcel service region. The ID of the parcel service region
        must be specified.
      operationId: getRestOrdersShippingParcelServiceRegionsParcelserviceregion
      x-api-path-slug: restordersshippingparcel-service-regionsparcelserviceregionid-get
      parameters:
      - in: query
        name: $parcelServiceRegionId
        description: The ID of the parcel service region
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: parcelServiceRegionId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Parcel
      - Service
      - Region
  /rest/orders/shipping/parcels/preview/{language?}:
    get:
      summary: Get a preview list for parcel services.
      description: Get a preview list for parcel services..
      operationId: getRestOrdersShippingParcelsPreviewLanguage
      x-api-path-slug: restordersshippingparcelspreviewlanguage-get
      parameters:
      - in: query
        name: language
      - in: path
        name: language?
      responses:
        200:
          description: OK
      tags:
      - Preview
      - Listparcel
      - Services
  /rest/orders/shipping/presets:
    get:
      summary: List shipping profiles
      description: List shipping profiles.
      operationId: getRestOrdersShippingPresets
      x-api-path-slug: restordersshippingpresets-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded in the shipping profile
      - in: query
        name: parcelServiceName
        description: Filter that restricts the search result to parcel service presets
          with a specified service name (e
      - in: query
        name: shippingServiceProvider
        description: Filter that restricts the search result to a shipping service
          provider
      - in: query
        name: updatedAtAfter
        description: Filter that restricts the search result to presets that were
          updated after a specific date
      - in: query
        name: updatedAtBefore
        description: Filter that restricts the search result to presets that were
          updated before a specific date
      - in: query
        name: with
        description: The name of an relation to the preset
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Profiles
  /rest/orders/shipping/presets/preview/{language?}:
    get:
      summary: Get a preview list for parcel service presets.
      description: Get a preview list for parcel service presets..
      operationId: getRestOrdersShippingPresetsPreviewLanguage
      x-api-path-slug: restordersshippingpresetspreviewlanguage-get
      parameters:
      - in: query
        name: language
      - in: path
        name: language?
      responses:
        200:
          description: OK
      tags:
      - Preview
      - Listparcel
      - Service
      - Presets
  /rest/orders/shipping/presets/{presetId}:
    get:
      summary: Get a shipping profile
      description: Gets a shipping profile. The ID of the shipping profile must be
        specified.
      operationId: getRestOrdersShippingPresetsPreset
      x-api-path-slug: restordersshippingpresetspresetid-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded in the shipping profile
      - in: path
        name: presetId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Profile
  /rest/orders/shipping/presets/{presetId}/parcel_service_regions:
    get:
      summary: Lists parcel service regions by parcel service preset id.
      description: Lists parcel service regions. The ID of the parcel service preset
        must be specified.
      operationId: getRestOrdersShippingPresetsPresetParcelServiceRegions
      x-api-path-slug: restordersshippingpresetspresetidparcel-service-regions-get
      parameters:
      - in: query
        name: $parcelServicePresetId
        description: The ID of the parcel service preset
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: presetId
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Parcel
      - Service
      - Regions
      - By
      - Parcel
      - Service
      - Preset
      - Id
  /rest/orders/shipping/returns/returns_service_providers:
    get:
      summary: ""
      description: .
      operationId: getRestOrdersShippingReturnsReturnsServiceProvers
      x-api-path-slug: restordersshippingreturnsreturns-service-providers-get
      parameters:
      - in: query
        name: isPlugin
        description: Possible values are 1 (true), 0 (false)
      - in: query
        name: pluginId
        description: The id of the plugin
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/orders/shipping/returns/returns_service_providers/plugins:
    get:
      summary: List shipping service provider plugins
      description: List shipping service provider plugins.
      operationId: getRestOrdersShippingReturnsReturnsServiceProversPlugins
      x-api-path-slug: restordersshippingreturnsreturns-service-providersplugins-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Service
      - Provider
      - Plugins
  /rest/orders/shipping/returns/returns_service_providers/{providerId}:
    get:
      summary: ""
      description: .
      operationId: getRestOrdersShippingReturnsReturnsServiceProversProver
      x-api-path-slug: restordersshippingreturnsreturns-service-providersproviderid-get
      parameters:
      - in: query
        name: $providerId
        description: The returns service provider id
      - in: path
        name: providerId
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/orders/shipping/returns/{returnsId}:
    get:
      summary: ""
      description: .
      operationId: getRestOrdersShippingReturnsReturns
      x-api-path-slug: restordersshippingreturnsreturnsid-get
      parameters:
      - in: path
        name: returnsId
      - in: query
        name: with
        description: Load additional relations for an order
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/orders/shipping/shipping_information:
    post:
      summary: Create shipping information
      description: Create shipping information.
      operationId: postRestOrdersShippingShippingInformation
      x-api-path-slug: restordersshippingshipping-information-post
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Information
  /rest/orders/shipping/shipping_service_providers:
    get:
      summary: List shipping service providers
      description: List shipping service providers.
      operationId: getRestOrdersShippingShippingServiceProvers
      x-api-path-slug: restordersshippingshipping-service-providers-get
      parameters:
      - in: query
        name: updatedAtAfter
        description: Filter that restricts the search result to shipping providers
          that were updated after a specific date
      - in: query
        name: updatedAtBefore
        description: Filter that restricts the search result to shipping providers
          that were updated before a specific date
      - in: query
        name: with
        description: The name of an relation to the shipping provider
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Service
      - Providers
    post:
      summary: Save a shipping service provider
      description: Saves a shipping service provider. The name of the shipping service
        provider must be specified.
      operationId: postRestOrdersShippingShippingServiceProvers
      x-api-path-slug: restordersshippingshipping-service-providers-post
      responses:
        200:
          description: OK
      tags:
      - Save
      - Shipping
      - Service
      - Provider
  /rest/orders/shipping/shipping_service_providers/plugins:
    get:
      summary: List shipping service provider plugins
      description: List shipping service provider plugins.
      operationId: getRestOrdersShippingShippingServiceProversPlugins
      x-api-path-slug: restordersshippingshipping-service-providersplugins-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Service
      - Provider
      - Plugins
  /rest/orders/shipping/shipping_service_providers/{shipping_service_provider_id}:
    get:
      summary: Get a shipping service provider
      description: Gets a shipping service provider. The ID of the shipping service
        provider must be specified.
      operationId: getRestOrdersShippingShippingServiceProversShippingServiceProver
      x-api-path-slug: restordersshippingshipping-service-providersshipping-service-provider-id-get
      parameters:
      - in: path
        name: shipping_service_provider_id
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Service
      - Provider
  /rest/orders/status-history:
    get:
      summary: List status histories of orders
      description: Lists the status histories of all orders. The result can be limited
        to an order, a status type, a period of time or a user.
      operationId: getRestOrdersStatusHistory
      x-api-path-slug: restordersstatushistory-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Get entries with createdAt date after this date
      - in: query
        name: createdAtTo
        description: Get entries with createdAt date before this date
      - in: query
        name: orderId
        description: The ID of the order
      - in: query
        name: statusId
        description: The ID of the status
      - in: query
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - List
      - Status
      - Histories
      - Of
      - Orders
  /rest/orders/statuses:
    get:
      summary: Searches order statuses.
      description: Searches for a list of order statuses, specified by the given filter
        parameters.
      operationId: getRestOrdersStatuses
      x-api-path-slug: restordersstatuses-get
      parameters:
      - in: query
        name: statusIdFrom
        description: Filter that restricts the search for order statuses to IDs from
          a defined value
      - in: query
        name: statusIdTo
        description: Filter that restricts the search for order statuses to IDs to
          a defined value
      responses:
        200:
          description: OK
      tags:
      - Searches
      - Order
      - Statuses
    post:
      summary: Creates an order status.
      description: Creates an order status, which is specified by the given ID.
      operationId: postRestOrdersStatuses
      x-api-path-slug: restordersstatuses-post
      parameters:
      - in: body
        name: /rest/orders/statuses
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Order
      - Status
  /rest/orders/statuses/all:
    get:
      summary: ""
      description: .
      operationId: getRestOrdersStatusesAll
      x-api-path-slug: restordersstatusesall-get
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/orders/statuses/{statusId}:
    delete:
      summary: Delete an order status.
      description: Deletes an order status, which is specified by the given ID.
      operationId: deleteRestOrdersStatusesStatus
      x-api-path-slug: restordersstatusesstatusid-delete
      parameters:
      - in: path
        name: statusId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Status
    get:
      summary: Get an order status.
      description: Gets an order status, which is specified by the given ID.
      operationId: getRestOrdersStatusesStatus
      x-api-path-slug: restordersstatusesstatusid-get
      parameters:
      - in: path
        name: statusId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Status
    put:
      summary: Update an order status.
      description: Updates an order status, which is specified by the given ID.
      operationId: putRestOrdersStatusesStatus
      x-api-path-slug: restordersstatusesstatusid-put
      parameters:
      - in: body
        name: /rest/orders/statuses/{statusId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: statusId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Status
  /rest/orders/{orderId}:
    delete:
      summary: Delete an order
      description: Deletes an order. The ID of the order must be specified.
      operationId: deleteRestOrdersOrder
      x-api-path-slug: restordersorderid-delete
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Order
    get:
      summary: Get an order
      description: Gets an order. The ID of the order must be specified.
      operationId: getRestOrdersOrder
      x-api-path-slug: restordersorderid-get
      parameters:
      - in: path
        name: orderId
      - in: query
        name: with
        description: Load additional relations for an order
      responses:
        200:
          description: OK
      tags:
      - Order
    put:
      summary: Update an order
      description: Updates an order. The ID of the order must be specified.
      operationId: putRestOrdersOrder
      x-api-path-slug: restordersorderid-put
      parameters:
      - in: body
        name: /rest/orders/{orderId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Order
  /rest/orders/{orderId}/addresses/{relationTypeId?}:
    get:
      summary: List order addresses
      description: Lists order addresses. The ID of the order must be specified.
      operationId: getRestOrdersOrderAddressesRelationtype
      x-api-path-slug: restordersorderidaddressesrelationtypeid-get
      parameters:
      - in: path
        name: orderId
      - in: path
        name: relationTypeId?
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Addresses
  /rest/orders/{orderId}/cancel:
    put:
      summary: Cancel an order
      description: Cancels an order. The ID of the order must be specified.
      operationId: putRestOrdersOrderCancel
      x-api-path-slug: restordersorderidcancel-put
      parameters:
      - in: body
        name: /rest/orders/{orderId}/cancel
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Order
  /rest/orders/{orderId}/contactWish:
    get:
      summary: Get a contact wish
      description: Gets the contact wish for an order. The ID of the order must be
        specified.
      operationId: getRestOrdersOrderContactwish
      x-api-path-slug: restordersorderidcontactwish-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Wish
  /rest/orders/{orderId}/coupons/{coupon}:
    post:
      summary: Redeem a coupon code
      description: Redeems a coupon code and applies it to an order. The ID of the
        order must be specified. If the coupon was successfully redeemed, the coupon
        data will be returned. If the coupon can not be redeemed, a validation exception
        will be thrown.
      operationId: postRestOrdersOrderCouponsCoupon
      x-api-path-slug: restordersorderidcouponscoupon-post
      parameters:
      - in: path
        name: coupon
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Redeem
      - Coupon
      - Code
  /rest/orders/{orderId}/dates:
    get:
      summary: List dates of an order
      description: Lists dates of an order. The ID of the order must be specified.
      operationId: getRestOrdersOrderDates
      x-api-path-slug: restordersorderiddates-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Dates
      - Of
      - Order
  /rest/orders/{orderId}/dates/{typeId}:
    get:
      summary: Get a date
      description: Gets a date. The ID of the order and the ID of the date type must
        be specified.
      operationId: getRestOrdersOrderDatesType
      x-api-path-slug: restordersorderiddatestypeid-get
      parameters:
      - in: path
        name: orderId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Date
  /rest/orders/{orderId}/documents/downloads/{type?}:
    get:
      summary: Download documents of an order
      description: Downloads documents of an order as a zip file. The ID of the order
        must be specified. In addition a type can be specified.
      operationId: getRestOrdersOrderDocumentsDownloadsType
      x-api-path-slug: restordersorderiddocumentsdownloadstype-get
      parameters:
      - in: path
        name: orderId
      - in: query
        name: type
        description: The type of the document
      - in: path
        name: type?
      responses:
        200:
          description: OK
      tags:
      - Download
      - Documents
      - Of
      - Order
  /rest/orders/{orderId}/documents/{type?}:
    get:
      summary: List documents of an order
      description: Lists documents of an order. The ID of the order must be specified.
        In addition a type can be specified.
      operationId: getRestOrdersOrderDocumentsType
      x-api-path-slug: restordersorderiddocumentstype-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to documents that were
          created on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to documents that were
          created within a certain period of time
      - in: query
        name: displayDateFrom
        description: Filter that restricts the search result to documents that were
          displayed on the specified date
      - in: query
        name: displayDateTo
        description: Filter that restricts the search result to documents that were
          displayed within a certain period of time
      - in: path
        name: orderId
      - in: query
        name: type
        description: The type of the order documents
      - in: path
        name: type?
      - in: query
        name: with
        description: Load additional relations for a document
      - in: query
        name: withContent
        description: Load also the document content as base64 encoded string
      responses:
        200:
          description: OK
      tags:
      - List
      - Documents
      - Of
      - Order
  /rest/orders/{orderId}/documents/{type}:
    post:
      summary: Upload order documents
      description: Uploads order documents. The ID of the order and the document type
        must be specified.
      operationId: postRestOrdersOrderDocumentsType
      x-api-path-slug: restordersorderiddocumentstype-post
      parameters:
      - in: body
        name: /rest/orders/{orderId}/documents/{type}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Order
      - Documents
  /rest/orders/{orderId}/items/serialNumbers:
    get:
      summary: List serial numbers of an order
      description: Lists all serial numbers of an order. The ID of the order must
        be specified.
      operationId: getRestOrdersOrderItemsSerialnumbers
      x-api-path-slug: restordersorderiditemsserialnumbers-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Serial
      - Numbers
      - Of
      - Order
  /rest/orders/{orderId}/items/{orderItemId}:
    delete:
      summary: Delete an order item
      description: Deletes an order item. The ID of the order and the ID of the order
        item must be specified.
      operationId: deleteRestOrdersOrderItemsOrderitem
      x-api-path-slug: restordersorderiditemsorderitemid-delete
      parameters:
      - in: path
        name: orderId
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
  /rest/orders/{orderId}/items/{orderItemId}/serialNumbers:
    get:
      summary: List serial numbers of an order item
      description: Lists all serial numbers of an order item. The ID of the order
        and the ID of the order item must be specified.
      operationId: getRestOrdersOrderItemsOrderitemSerialnumbers
      x-api-path-slug: restordersorderiditemsorderitemidserialnumbers-get
      parameters:
      - in: path
        name: orderId
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - List
      - Serial
      - Numbers
      - Of
      - Order
      - Item
  /rest/orders/{orderId}/outgoing_stocks:
    delete:
      summary: Revert outgoing stock
      description: Reverts the booking of order items of an order. The ID of the order
        must be specified.
      operationId: deleteRestOrdersOrderOutgoingStocks
      x-api-path-slug: restordersorderidoutgoing-stocks-delete
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Revert
      - Outgoing
      - Stock
    post:
      summary: Book out order items
      description: Books out the order items of an order. The ID of the order must
        be specified and a booking date can be specified. The current date and time
        will be used if no date is specified.
      operationId: postRestOrdersOrderOutgoingStocks
      x-api-path-slug: restordersorderidoutgoing-stocks-post
      parameters:
      - in: query
        name: date
        description: The date that is saved as booking date for the outgoing stock
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Book
      - Out
      - Order
      - Items
  /rest/orders/{orderId}/packagenumbers:
    get:
      summary: List package numbers of an order
      description: Lists the package numbers of an order. The ID of the order must
        be specified.
      operationId: getRestOrdersOrderPackagenumbers
      x-api-path-slug: restordersorderidpackagenumbers-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Package
      - Numbers
      - Of
      - Order
  /rest/orders/{orderId}/properties:
    post:
      summary: Create a property for an order
      description: Creates a property and attaches it to an order. The ID of the order
        must be specified.
      operationId: postRestOrdersOrderProperties
      x-api-path-slug: restordersorderidproperties-post
      parameters:
      - in: body
        name: /rest/orders/{orderId}/properties
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Propertyan
      - Order
  /rest/orders/{orderId}/properties/{typeId?}:
    get:
      summary: List properties of an order
      description: Lists properties of an order. The ID of the order must be specified.
      operationId: getRestOrdersOrderPropertiesType
      x-api-path-slug: restordersorderidpropertiestypeid-get
      parameters:
      - in: path
        name: orderId
      - in: query
        name: typeId
        description: The property type ID
      - in: path
        name: typeId?
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
      - Of
      - Order
  /rest/orders/{orderId}/properties/{typeId}:
    delete:
      summary: Delete a property of an order by order ID and type ID
      description: Deletes a property of an order. The composite key of the property
        must be specified. The composite key is composed of the ID of the order and
        the ID of the order property type.
      operationId: deleteRestOrdersOrderPropertiesType
      x-api-path-slug: restordersorderidpropertiestypeid-delete
      parameters:
      - in: body
        name: /rest/orders/{orderId}/properties/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Of
      - Order
      - By
      - Order
      - ID
      - Type
      - ID
    put:
      summary: Update a property of an order by order ID and property ID
      description: Updates the value of a property. The composite key of the property
        must be specified. The composite key is composed of the ID of the order and
        the ID of the order property type.
      operationId: putRestOrdersOrderPropertiesType
      x-api-path-slug: restordersorderidpropertiestypeid-put
      parameters:
      - in: body
        name: /rest/orders/{orderId}/properties/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Of
      - Order
      - By
      - Order
      - ID
      - Property
      - ID
  /rest/orders/{orderId}/shipping/packages:
    delete:
      summary: Delete all order shipping packages for an order
      description: Deletes all order shipping packages for an order. The ID of the
        order must be specified.
      operationId: deleteRestOrdersOrderShippingPackages
      x-api-path-slug: restordersorderidshippingpackages-delete
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Shipping
      - Packagesan
      - Order
    get:
      summary: List order shipping packages
      description: Lists order shipping packages. The ID of the order must be specified.
      operationId: getRestOrdersOrderShippingPackages
      x-api-path-slug: restordersorderidshippingpackages-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: orderId
      - in: query
        name: with
        description: Possible value is labelBase64
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Shipping
      - Packages
    post:
      summary: Create an order shipping package
      description: Creates an order shipping package. The ID of the order must be
        specified.
      operationId: postRestOrdersOrderShippingPackages
      x-api-path-slug: restordersorderidshippingpackages-post
      parameters:
      - in: body
        name: /rest/orders/{orderId}/shipping/packages
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Shipping
      - Package
  /rest/orders/{orderId}/shipping/packages/{orderShippingPackageId}:
    delete:
      summary: Delete an order shipping package
      description: Deletes an order shipping package. The ID of the order and the
        ID of the order shipping package must be specified.
      operationId: deleteRestOrdersOrderShippingPackagesOrdershippingpackage
      x-api-path-slug: restordersorderidshippingpackagesordershippingpackageid-delete
      parameters:
      - in: path
        name: orderId
      - in: path
        name: orderShippingPackageId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Shipping
      - Package
    get:
      summary: Get an order shipping package
      description: Gets an order shipping package. The ID of the order and the ID
        of the order shipping package must be specified.
      operationId: getRestOrdersOrderShippingPackagesOrdershippingpackage
      x-api-path-slug: restordersorderidshippingpackagesordershippingpackageid-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: orderId
      - in: path
        name: orderShippingPackageId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Shipping
      - Package
    put:
      summary: Update an order shipping package
      description: Updates an order shipping package. The ID of the order and the
        ID of the order shipping package must be specified.
      operationId: putRestOrdersOrderShippingPackagesOrdershippingpackage
      x-api-path-slug: restordersorderidshippingpackagesordershippingpackageid-put
      parameters:
      - in: body
        name: /rest/orders/{orderId}/shipping/packages/{orderShippingPackageId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      - in: path
        name: orderShippingPackageId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Shipping
      - Package
  /rest/orders/{orderId}/shipping/returns:
    get:
      summary: ""
      description: .
      operationId: getRestOrdersOrderShippingReturns
      x-api-path-slug: restordersorderidshippingreturns-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of orders to be displayed per page
      - in: path
        name: orderId
      - in: query
        name: page
        description: The page to get
      - in: query
        name: with
        description: Load additional relations for an order
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/orders/{orderId}/shipping/returns/assign_label/{returnsId}:
    put:
      summary: ""
      description: .
      operationId: putRestOrdersOrderShippingReturnsAssignLabelReturns
      x-api-path-slug: restordersorderidshippingreturnsassign-labelreturnsid-put
      parameters:
      - in: path
        name: orderId
      - in: path
        name: returnsId
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/orders/{orderId}/shipping/shipping_information:
    delete:
      summary: Delete shipping information
      description: Deletes the shipping information. The ID of the order must be specified.
      operationId: deleteRestOrdersOrderShippingShippingInformation
      x-api-path-slug: restordersorderidshippingshipping-information-delete
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Information
    get:
      summary: Get shipping information
      description: Gets the shipping information. The ID of the order must be specified.
      operationId: getRestOrdersOrderShippingShippingInformation
      x-api-path-slug: restordersorderidshippingshipping-information-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Information
  /rest/orders/{orderId}/shipping/shipping_information/additional_data:
    put:
      summary: Update additional data of the shipping information
      description: Updates additional data of the shipping information. The ID of
        the order must be specified.
      operationId: putRestOrdersOrderShippingShippingInformationAdditionalData
      x-api-path-slug: restordersorderidshippingshipping-informationadditional-data-put
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Additional
      - Data
      - Of
      - Shipping
      - Information
  /rest/orders/{orderId}/shipping/shipping_information/status:
    put:
      summary: Update the shipping status of the shipping information
      description: Updates the shipping status of the shipping information. The ID
        of the order must be specified.
      operationId: putRestOrdersOrderShippingShippingInformationStatus
      x-api-path-slug: restordersorderidshippingshipping-informationstatus-put
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Status
      - Of
      - Shipping
      - Information
  /rest/orders/{orderId}/status-history:
    get:
      summary: Get the status history of an order
      description: Gets the status of an order. The ID of the order must be specified.
      operationId: getRestOrdersOrderStatusHistory
      x-api-path-slug: restordersorderidstatushistory-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Status
      - History
      - Of
      - Order
  /rest/payment/properties/types/names:
    post:
      summary: Create a name of a property type
      description: Create a name of a property type.
      operationId: postRestPaymentPropertiesTypesNames
      x-api-path-slug: restpaymentpropertiestypesnames-post
      parameters:
      - in: body
        name: /rest/payment/properties/types/names
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Name
      - Of
      - Property
      - Type
    put:
      summary: Update a name of a property type
      description: Update a name of a property type.
      operationId: putRestPaymentPropertiesTypesNames
      x-api-path-slug: restpaymentpropertiestypesnames-put
      parameters:
      - in: body
        name: /rest/payment/properties/types/names
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Name
      - Of
      - Property
      - Type
  /rest/payment/properties/types/names/{lang?}:
    get:
      summary: List names of property types
      description: List names of property types.
      operationId: getRestPaymentPropertiesTypesNamesLang
      x-api-path-slug: restpaymentpropertiestypesnameslang-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: path
        name: lang?
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
      - Of
      - Property
      - Types
  /rest/payment/properties/types/names/{nameId}:
    get:
      summary: Get a name of a property type
      description: Gets a name of a property type. The ID of the name must be specified.
      operationId: getRestPaymentPropertiesTypesNamesName
      x-api-path-slug: restpaymentpropertiestypesnamesnameid-get
      parameters:
      - in: path
        name: nameId
      responses:
        200:
          description: OK
      tags:
      - Name
      - Of
      - Property
      - Type
  /rest/payment/{paymentId}/contact:
    delete:
      summary: Delete Payment-Contact-Relation
      description: Delete payment-contact-relation.
      operationId: deleteRestPaymentPaymentContact
      x-api-path-slug: restpaymentpaymentidcontact-delete
      parameters:
      - in: path
        name: paymentId
      responses:
        200:
          description: OK
      tags:
      - Payment-Contact-Relation
  /rest/payment/{paymentId}/contact/{contactId}:
    post:
      summary: Create Payment-Contact-Relation
      description: Create payment-contact-relation.
      operationId: postRestPaymentPaymentContactContact
      x-api-path-slug: restpaymentpaymentidcontactcontactid-post
      parameters:
      - in: path
        name: contactId
      - in: path
        name: paymentId
      responses:
        200:
          description: OK
      tags:
      - Payment-Contact-Relation
  /rest/payment/{paymentId}/order:
    delete:
      summary: Delete Payment-Order-Relation
      description: Delete payment-order-relation.
      operationId: deleteRestPaymentPaymentOrder
      x-api-path-slug: restpaymentpaymentidorder-delete
      parameters:
      - in: path
        name: paymentId
      responses:
        200:
          description: OK
      tags:
      - Payment-Order-Relation
  /rest/payment/{paymentId}/order/{orderId}:
    post:
      summary: Create Payment-Order-Relation
      description: Create payment-order-relation.
      operationId: postRestPaymentPaymentOrderOrder
      x-api-path-slug: restpaymentpaymentidorderorderid-post
      parameters:
      - in: path
        name: orderId
      - in: path
        name: paymentId
      responses:
        200:
          description: OK
      tags:
      - Payment-Order-Relation
  /rest/payments:
    get:
      summary: List payments
      description: List payments.
      operationId: getRestPayments
      x-api-path-slug: restpayments-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
    post:
      summary: Create a payment
      description: Create a payment.
      operationId: postRestPayments
      x-api-path-slug: restpayments-post
      parameters:
      - in: body
        name: /rest/payments
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
    put:
      summary: Update a payment
      description: Update a payment.
      operationId: putRestPayments
      x-api-path-slug: restpayments-put
      parameters:
      - in: body
        name: /rest/payments
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
  /rest/payments/entrydate:
    get:
      summary: List payments by entry date
      description: Lists all payments by entry date within a certain date range. The
        start and the end of the date range must be specified.
      operationId: getRestPaymentsEntrydate
      x-api-path-slug: restpaymentsentrydate-get
      parameters:
      - in: query
        name: endDate
        description: The end date of the date range for the entry date of the payment
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: startDate
        description: The start date of the date range for the entry date of the payment
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - By
      - Entry
      - Date
  /rest/payments/importdate:
    get:
      summary: List payments by import date
      description: Lists all payments by import date within a certain date range.
        The start and the end of the date range must be specified.
      operationId: getRestPaymentsImportdate
      x-api-path-slug: restpaymentsimportdate-get
      parameters:
      - in: query
        name: endDate
        description: The end date of the date range for the import date of the payment
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: startDate
        description: The start date of the date range for the import date of the payment
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - By
      - Import
      - Date
  /rest/payments/methodNames:
    get:
      summary: List payment methods names
      description: Lists all payment method names.
      operationId: getRestPaymentsMethodnames
      x-api-path-slug: restpaymentsmethodnames-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payment
      - Methods
      - Names
  /rest/payments/methodNames/{paymentMethodId}:
    get:
      summary: List all payment method names for a payment method id
      description: List all payment method names for a payment method id. The payment
        method id must be specified.
      operationId: getRestPaymentsMethodnamesPaymentmethod
      x-api-path-slug: restpaymentsmethodnamespaymentmethodid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: paymentMethodId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Payment
      - Method
      - Namesa
      - Payment
      - Method
      - Id
  /rest/payments/methodNames/{paymentMethodId}/{lang}:
    get:
      summary: Gets a payment method name by id and lang
      description: Gets a payment method name by id and lang. The ID and the requested
        lang of the payment method must be specified.
      operationId: getRestPaymentsMethodnamesPaymentmethodLang
      x-api-path-slug: restpaymentsmethodnamespaymentmethodidlang-get
      parameters:
      - in: path
        name: lang
      - in: path
        name: paymentMethodId
      responses:
        200:
          description: OK
      tags:
      - S
      - Payment
      - Method
      - Name
      - By
      - Id
      - Lang
  /rest/payments/methods:
    get:
      summary: List payment methods
      description: Lists all payment method plugins.
      operationId: getRestPaymentsMethods
      x-api-path-slug: restpaymentsmethods-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payment
      - Methods
    post:
      summary: Create a payment method
      description: Creates a payment method. The plugin key, the payment key and the
        name of the payment method must be specified.
      operationId: postRestPaymentsMethods
      x-api-path-slug: restpaymentsmethods-post
      parameters:
      - in: body
        name: /rest/payments/methods
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Method
    put:
      summary: Update a payment method
      description: Updates the name of the payment method. The name of the payment
        method must be specified.
      operationId: putRestPaymentsMethods
      x-api-path-slug: restpaymentsmethods-put
      parameters:
      - in: body
        name: /rest/payments/methods
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Method
  /rest/payments/methods/ebics:
    get:
      summary: Get EBICS Accounts
      description: Get ebics accounts.
      operationId: getRestPaymentsMethodsEbics
      x-api-path-slug: restpaymentsmethodsebics-get
      responses:
        200:
          description: OK
      tags:
      - EBICS
      - Accounts
    post:
      summary: Create an EBICS Account
      description: Create an ebics account.
      operationId: postRestPaymentsMethodsEbics
      x-api-path-slug: restpaymentsmethodsebics-post
      parameters:
      - in: query
        name: name
        description: The name of the EBICS Account
      responses:
        200:
          description: OK
      tags:
      - EBICS
      - Account
  /rest/payments/methods/hbci:
    get:
      summary: Returns the HBCI-Account count
      description: Returns the hbci-account count.
      operationId: getRestPaymentsMethodsHbci
      x-api-path-slug: restpaymentsmethodshbci-get
      responses:
        200:
          description: OK
      tags:
      - Returns
      - HBCI-Account
      - Count
  /rest/payments/methods/plugins/{pluginKey}:
    get:
      summary: Get a payment method
      description: Gets a payment method plugin. The plugin key must be specified.
      operationId: getRestPaymentsMethodsPluginsPluginkey
      x-api-path-slug: restpaymentsmethodspluginspluginkey-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: pluginKey
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Method
  /rest/payments/methods/preview/{language?}:
    get:
      summary: Get a preview list for parcel services.
      description: Get a preview list for parcel services..
      operationId: getRestPaymentsMethodsPreviewLanguage
      x-api-path-slug: restpaymentsmethodspreviewlanguage-get
      parameters:
      - in: query
        name: language
      - in: path
        name: language?
      responses:
        200:
          description: OK
      tags:
      - Preview
      - Listparcel
      - Services
  /rest/payments/methods/{methodId}:
    get:
      summary: List payments of a payment method
      description: Lists all payments of the a payment method. The ID of the payment
        method must be specified.
      operationId: getRestPaymentsMethodsMethod
      x-api-path-slug: restpaymentsmethodsmethodid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: path
        name: methodId
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Payment
      - Method
  /rest/payments/orders/{orderId}:
    get:
      summary: List payments of an order
      description: Lists all payments of an order. The ID of the order must be specified.
      operationId: getRestPaymentsOrdersOrder
      x-api-path-slug: restpaymentsordersorderid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: path
        name: orderId
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Order
  /rest/payments/properties:
    get:
      summary: List properties
      description: List properties.
      operationId: getRestPaymentsProperties
      x-api-path-slug: restpaymentsproperties-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
    post:
      summary: Create a payment property
      description: Create a payment property.
      operationId: postRestPaymentsProperties
      x-api-path-slug: restpaymentsproperties-post
      parameters:
      - in: body
        name: /rest/payments/properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Property
    put:
      summary: Update a payment property
      description: Update a payment property.
      operationId: putRestPaymentsProperties
      x-api-path-slug: restpaymentsproperties-put
      parameters:
      - in: body
        name: /rest/payments/properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Property
  /rest/payments/properties/date:
    get:
      summary: List properties by creation date
      description: Lists all properties by creation date. The start and the end of
        the date range must be specified.
      operationId: getRestPaymentsPropertiesDate
      x-api-path-slug: restpaymentspropertiesdate-get
      parameters:
      - in: query
        name: endDate
        description: The end date of the date range for the date of creation of the
          property
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: startDate
        description: The start date of the date range for the date of creation of
          the property
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
      - By
      - Creation
      - Date
  /rest/payments/properties/types:
    get:
      summary: List property types
      description: Lists all property types. The language must be specified.
      operationId: getRestPaymentsPropertiesTypes
      x-api-path-slug: restpaymentspropertiestypes-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Types
    post:
      summary: Create a property type
      description: Create a property type.
      operationId: postRestPaymentsPropertiesTypes
      x-api-path-slug: restpaymentspropertiestypes-post
      parameters:
      - in: body
        name: /rest/payments/properties/types
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Property
      - Type
    put:
      summary: Update a property type
      description: Update a property type.
      operationId: putRestPaymentsPropertiesTypes
      x-api-path-slug: restpaymentspropertiestypes-put
      parameters:
      - in: body
        name: /rest/payments/properties/types
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Property
      - Type
  /rest/payments/properties/types/{typeId}:
    get:
      summary: Get a property type
      description: Gets a property type. The ID of the type must be specified.
      operationId: getRestPaymentsPropertiesTypesType
      x-api-path-slug: restpaymentspropertiestypestypeid-get
      parameters:
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Type
  /rest/payments/properties/{propertyId}:
    get:
      summary: Get a property
      description: Gets a property. The ID of the property must be specified.
      operationId: getRestPaymentsPropertiesProperty
      x-api-path-slug: restpaymentspropertiespropertyid-get
      parameters:
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
  /rest/payments/property/{propertyTypeId}/{propertyValue}:
    get:
      summary: List payments by property type ID and value
      description: Lists all payments by the given property type ID and the value.
      operationId: getRestPaymentsPropertyPropertytypePropertyvalue
      x-api-path-slug: restpaymentspropertypropertytypeidpropertyvalue-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: propertyTypeId
      - in: path
        name: propertyValue
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - By
      - Property
      - Type
      - ID
      - Value
  /rest/payments/status/{statusId}:
    get:
      summary: List payments of a payment status
      description: Lists all payments of a payment status. The ID of the <a href='https://developers.plentymarkets.com/rest-doc/introduction#payment-statuses'  target='_blank'>payment
        status</a> must be specified.
      operationId: getRestPaymentsStatusStatus
      x-api-path-slug: restpaymentsstatusstatusid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: statusId
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Payment
      - Status
  /rest/payments/transactions/{transactionTypeId}:
    get:
      summary: List payments of a transaction type
      description: Lists all payments of a transaction type. The ID of the transaction
        type must be specified.
      operationId: getRestPaymentsTransactionsTransactiontype
      x-api-path-slug: restpaymentstransactionstransactiontypeid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: transactionTypeId
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Transaction
      - Type
  /rest/payments/{paymentId}:
    get:
      summary: Get a payment
      description: Gets a payment. The ID of the payment must be specified.
      operationId: getRestPaymentsPayment
      x-api-path-slug: restpaymentspaymentid-get
      parameters:
      - in: path
        name: paymentId
      responses:
        200:
          description: OK
      tags:
      - Payment
  /rest/payments/{paymentId}/properties:
    get:
      summary: List properties for a payment
      description: Lists all properties for a payment. The ID of the payment must
        be specified.
      operationId: getRestPaymentsPaymentProperties
      x-api-path-slug: restpaymentspaymentidproperties-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: paymentId
      responses:
        200:
          description: OK
      tags:
      - List
      - Propertiesa
      - Payment
  /rest/plugin_sets:
    get:
      summary: List all Sets
      description: Lists all available sets.
      operationId: getRestPluginSets
      x-api-path-slug: restplugin-sets-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Sets
    post:
      summary: Create a Set
      description: Creates a new plugin set with the given name. If a 'copyPluginSetId'
        is given, all set entries from that set will be copied into the new set
      operationId: postRestPluginSets
      x-api-path-slug: restplugin-sets-post
      parameters:
      - in: query
        name: copyPluginSetId
        description: The ID of the plugin set of which to copy the set entries from
          into the     * new set
      responses:
        200:
          description: OK
      tags:
      - Set
  /rest/plugin_sets/preview_hash:
    get:
      summary: Get the preview hash for a set
      description: Get the hash required to preview a plugin set. Response content
        will be in the form ['previewHash' => 'adf245o9nwu90sdfjw409u4'].
      operationId: getRestPluginSetsPreviewHash
      x-api-path-slug: restplugin-setspreview-hash-get
      responses:
        200:
          description: OK
      tags:
      - Preview
      - Hasha
      - Set
  /rest/plugin_sets/{pluginSetId}/languages:
    get:
      summary: List all the plugins translations for a plugin set
      description: Lists all the plugins translations for a plugin set
      operationId: getRestPluginSetsPluginsetLanguages
      x-api-path-slug: restplugin-setspluginsetidlanguages-get
      parameters:
      - in: query
        name: $pluginSetId
        description: The ID of the plugin set
      - in: path
        name: pluginSetId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Plugins
      - Translationsa
      - Plugin
      - Set
  /rest/plugin_sets/{pluginSetId}/languages/csv/{languageCode}:
    get:
      summary: ""
      description: .
      operationId: getRestPluginSetsPluginsetLanguagesCsvLanguagecode
      x-api-path-slug: restplugin-setspluginsetidlanguagescsvlanguagecode-get
      parameters:
      - in: query
        name: $languageCode
        description: The code of the language
      - in: query
        name: $pluginSetId
        description: The ID of the plugin set
      - in: path
        name: languageCode
      - in: path
        name: pluginSetId
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/plugin_sets/{pluginSetId}/languages/{languageCode}:
    delete:
      summary: Delete multiple translation
      description: Deletes multiple translation. The pluginSetId and languageCode
        must be specified.
      operationId: deleteRestPluginSetsPluginsetLanguagesLanguagecode
      x-api-path-slug: restplugin-setspluginsetidlanguageslanguagecode-delete
      parameters:
      - in: query
        name: $languageCode
        description: The code of the language
      - in: query
        name: $pluginSetId
        description: The ID of the plugin set
      - in: path
        name: languageCode
      - in: path
        name: pluginSetId
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Translation
  /rest/plugin_sets/{pluginSetId}/languages/{targetLanguage}:
    get:
      summary: ""
      description: .
      operationId: getRestPluginSetsPluginsetLanguagesTargetlanguage
      x-api-path-slug: restplugin-setspluginsetidlanguagestargetlanguage-get
      parameters:
      - in: query
        name: $pluginSetId
        description: The ID of the plugin set
      - in: query
        name: $targetLanguage
        description: The code of the language we target
      - in: path
        name: pluginSetId
      - in: path
        name: targetLanguage
      responses:
        200:
          description: OK
      tags:
      - ""
    post:
      summary: ""
      description: .
      operationId: postRestPluginSetsPluginsetLanguagesTargetlanguage
      x-api-path-slug: restplugin-setspluginsetidlanguagestargetlanguage-post
      parameters:
      - in: query
        name: $pluginSetId
        description: The ID of the plugin set
      - in: query
        name: $targetLanguage
        description: The code of the language
      - in: path
        name: pluginSetId
      - in: path
        name: targetLanguage
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/plugin_sets/{setId}:
    delete:
      summary: Delete a set
      description: Deletes a plugin set. Response content will be the number of sets
        deleted (i. e. '1' or '0').
      operationId: deleteRestPluginSetsSet
      x-api-path-slug: restplugin-setssetid-delete
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Set
    get:
      summary: Get a set
      description: Get a set.
      operationId: getRestPluginSetsSet
      x-api-path-slug: restplugin-setssetid-get
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Set
    put:
      summary: Update a set
      description: Updates a set. Response content will be 'true' if the update was
        successful, 'false' if not.
      operationId: putRestPluginSetsSet
      x-api-path-slug: restplugin-setssetid-put
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Set
  /rest/plugin_sets/{setId}/plugins:
    get:
      summary: List all Plugins of Set
      description: Lists all active Plugins of given Set.
      operationId: getRestPluginSetsSetPlugins
      x-api-path-slug: restplugin-setssetidplugins-get
      parameters:
      - in: query
        name: includeStage
        description: Include staged plugins in the result
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Plugins
      - Of
      - Set
  /rest/plugin_sets/{setId}/plugins/search:
    get:
      summary: Search plugins
      description: Searches for plugins. The search can be refined with numerous parameters.
      operationId: getRestPluginSetsSetPluginsSearch
      x-api-path-slug: restplugin-setssetidpluginssearch-get
      parameters:
      - in: query
        name: active
        description: Only search for plugins that are active / inactive
      - in: query
        name: checkRequirements
        description: Add the requirements to the response
      - in: query
        name: checkUpdate
        description: Check for updates
      - in: query
        name: in-productive
        description: Search for plugins that are in productive
      - in: query
        name: in-stage
        description: Search for plugins that are in stage
      - in: query
        name: installed
        description: Only search for installed / not installed plugins
      - in: query
        name: itemsPerPage
        description: How many plugins to include per page of the search result
      - in: query
        name: name
        description: Search for plugins with a specific name
      - in: query
        name: pluginSetId
        description: Search for plugins from a specific plugin set
      - in: path
        name: setId
      - in: query
        name: source
        description: Search for plugins from a specific source
      - in: query
        name: type
        description: Search for plugins of a given type
      responses:
        200:
          description: OK
      tags:
      - Search
      - Plugins
  /rest/plugin_sets/{setId}/plugins/{pluginId}:
    delete:
      summary: Remove a plugin from a set
      description: |-
        Removes a plugin from a set and deletes all plugin files. Response content will be 'true' if the deletion was successful,
        'false' if not. If no plugin set with the given id can be found or the plugin is not associated to the set, a 404 will be returned.
      operationId: deleteRestPluginSetsSetPluginsPlugin
      x-api-path-slug: restplugin-setssetidpluginspluginid-delete
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Plugin
      - From
      - Set
    post:
      summary: Add a plugin to a set
      description: Add a plugin to a set.
      operationId: postRestPluginSetsSetPluginsPlugin
      x-api-path-slug: restplugin-setssetidpluginspluginid-post
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Plugin
      - To
      - Set
    put:
      summary: Change a plugin's 'active' status for a set.
      description: Change a plugin's 'active' status for a set..
      operationId: putRestPluginSetsSetPluginsPlugin
      x-api-path-slug: restplugin-setssetidpluginspluginid-put
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Change
      - Plugins
      - Active
      - Statusa
      - Set
  /rest/plugin_sets/{setId}/plugins/{pluginId}/install_git_plugin:
    post:
      summary: Install a git plugin into a set
      description: Installs a git plugin into a set. Response content will be in the
        form ['gitPluginInstalled' => 'true' / 'false'].
      operationId: postRestPluginSetsSetPluginsPluginInstallGitPlugin
      x-api-path-slug: restplugin-setssetidpluginspluginidinstall-git-plugin-post
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Install
      - Git
      - Plugin
      - Into
      - Set
  /rest/plugin_sets/{setId}/plugins/{pluginId}/setPosition:
    post:
      summary: Set a plugin's position in a set
      description: Set a plugin's position in a set.
      operationId: postRestPluginSetsSetPluginsPluginSetposition
      x-api-path-slug: restplugin-setssetidpluginspluginidsetposition-post
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Set
      - Plugins
      - Position
      - In
      - Set
  /rest/plugin_sets/{setId}/set_entries:
    get:
      summary: List all SetEntries of Set
      description: List all setentries of set.
      operationId: getRestPluginSetsSetSetEntries
      x-api-path-slug: restplugin-setssetidset-entries-get
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - SetEntries
      - Of
      - Set
  /rest/plugins:
    get:
      summary: List plugins
      description: |-
        Lists all plugins saved in the inbox folder. Plugins that have not been provisioned to Stage or Productive will
        also be shown.
      operationId: getRestPlugins
      x-api-path-slug: restplugins-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Plugins
    post:
      summary: Create a plugin
      description: Creates a plugin with empty plugin folders and a plugin.json file.
      operationId: postRestPlugins
      x-api-path-slug: restplugins-post
      parameters:
      - in: body
        name: /rest/plugins
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Plugin
  /rest/plugins/plugin_sets/{pluginSetId}/plugins:
    get:
      summary: List all Plugins of Set
      description: Lists all active Plugins of given Set.
      operationId: getRestPluginsPluginSetsPluginsetPlugins
      x-api-path-slug: restpluginsplugin-setspluginsetidplugins-get
      parameters:
      - in: query
        name: includeStage
        description: Include staged plugins in the result
      - in: path
        name: pluginSetId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Plugins
      - Of
      - Set
  /rest/plugins/search:
    get:
      summary: List plugins
      description: |-
        Lists all plugins saved in the inbox folder. Plugins that have not been provisioned to Stage or Productive will
        also be shown.
      operationId: getRestPluginsSearch
      x-api-path-slug: restpluginssearch-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: name
        description: The name of the plugin
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: type
        description: The type of the plugin (template, theme, etc
      - in: query
        name: webstoreId
        description: The ID of the client (store)
      responses:
        200:
          description: OK
      tags:
      - List
      - Plugins
  /rest/plugins/seo/sitemap:
    get:
      summary: Load sitemap patterns
      description: Loads all given sitemap patterns from booted plugins.
      operationId: getRestPluginsSeoSitemap
      x-api-path-slug: restpluginsseositemap-get
      responses:
        200:
          description: OK
      tags:
      - Load
      - Sitemap
      - Patterns
  /rest/plugins/ui:
    get:
      summary: List plugins for backend UI
      description: Lists all plugins provisioned in Stage or Productive that contain
        a plugin.js file.
      operationId: getRestPluginsUi
      x-api-path-slug: restpluginsui-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Pluginsbackend
      - UI
  /rest/plugins/{pluginId}:
    delete:
      summary: Delete a plugin
      description: |-
        Deletes a plugin. This call also deletes all plugin files in the inbox folder! To commit the deletion, the
        plugin must be provisioned in Stage or Productive. The ID of the plugin must be specified.
      operationId: deleteRestPluginsPlugin
      x-api-path-slug: restpluginspluginid-delete
      parameters:
      - in: path
        name: pluginId
      responses:
        200:
          description: OK
      tags:
      - Plugin
    get:
      summary: Get a plugin
      description: Gets a plugin. The ID of the plugin must be specified.
      operationId: getRestPluginsPlugin
      x-api-path-slug: restpluginspluginid-get
      parameters:
      - in: path
        name: pluginId
      responses:
        200:
          description: OK
      tags:
      - Plugin
    put:
      summary: Update a plugin
      description: |-
        Updates a plugin. The plugin position can be changed. The plugin can be activated or deactivated for Stage or
        Productive. The plugin can be activated or deactivated for online stores. The ID of the plugin must be
        specified.
      operationId: putRestPluginsPlugin
      x-api-path-slug: restpluginspluginid-put
      parameters:
      - in: body
        name: /rest/plugins/{pluginId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: pluginId
      responses:
        200:
          description: OK
      tags:
      - Plugin
  /rest/plugins/{pluginId}/plugin_sets/{pluginSetId}:
    delete:
      summary: Delete a plugin
      description: |-
        Deletes a plugin. This call also deletes all plugin files in the inbox folder! To commit the deletion, the
        plugin must be provisioned in Stage or Productive. The ID of the plugin must be specified.
      operationId: deleteRestPluginsPluginPluginSetsPluginset
      x-api-path-slug: restpluginspluginidplugin-setspluginsetid-delete
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: pluginSetId
      responses:
        200:
          description: OK
      tags:
      - Plugin
  /rest/plugins/{pluginId}/plugin_sets/{pluginSetId}/configuration_layout:
    get:
      summary: ""
      description: .
      operationId: getRestPluginsPluginPluginSetsPluginsetConfigurationLayout
      x-api-path-slug: restpluginspluginidplugin-setspluginsetidconfiguration-layout-get
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: pluginSetId
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/plugins/{pluginId}/plugin_sets/{pluginSetId}/configurations:
    get:
      summary: ""
      description: .
      operationId: getRestPluginsPluginPluginSetsPluginsetConfigurations
      x-api-path-slug: restpluginspluginidplugin-setspluginsetidconfigurations-get
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: pluginSetId
      responses:
        200:
          description: OK
      tags:
      - ""
    put:
      summary: ""
      description: .
      operationId: putRestPluginsPluginPluginSetsPluginsetConfigurations
      x-api-path-slug: restpluginspluginidplugin-setspluginsetidconfigurations-put
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: pluginSetId
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/plugins_mail:
    post:
      summary: Send mail
      description: Send mail from booted plugins.
      operationId: postRestPluginsMail
      x-api-path-slug: restplugins-mail-post
      responses:
        200:
          description: OK
      tags:
      - Send
      - Mail
  /rest/properties:
    get:
      summary: List properties
      description: Lists properties.
      operationId: getRestProperties
      x-api-path-slug: restproperties-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
    post:
      summary: Create a property
      description: Creates a property
      operationId: postRestProperties
      x-api-path-slug: restproperties-post
      parameters:
      - in: body
        name: /rest/properties
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: cast
        description: The cast of the property
      - in: query
        name: position
        description: The position of the property
      - in: query
        name: typeIdentifier
        description: The identifier of the property type
      responses:
        200:
          description: OK
      tags:
      - Property
  /rest/properties/availabilities:
    get:
      summary: List availabilities
      description: Lists availabilities.
      operationId: getRestPropertiesAvailabilities
      x-api-path-slug: restpropertiesavailabilities-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Availabilities
    post:
      summary: Create an availability
      description: Creates an availability.
      operationId: postRestPropertiesAvailabilities
      x-api-path-slug: restpropertiesavailabilities-post
      parameters:
      - in: body
        name: /rest/properties/availabilities
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: propertyId
        description: The ID of the property
      - in: query
        name: type
        description: The type of the availability
      - in: query
        name: value
        description: The value of the availability
      responses:
        200:
          description: OK
      tags:
      - Availability
  /rest/properties/availabilities/{availabilityId}:
    delete:
      summary: Delete an availability
      description: Deletes an availability. The ID ot the availability must be specified.
      operationId: deleteRestPropertiesAvailabilitiesAvailability
      x-api-path-slug: restpropertiesavailabilitiesavailabilityid-delete
      parameters:
      - in: path
        name: availabilityId
      responses:
        200:
          description: OK
      tags:
      - Availability
    get:
      summary: Get an availability
      description: Gets an availability. The ID of the availability must be specified.
      operationId: getRestPropertiesAvailabilitiesAvailability
      x-api-path-slug: restpropertiesavailabilitiesavailabilityid-get
      parameters:
      - in: path
        name: availabilityId
      responses:
        200:
          description: OK
      tags:
      - Availability
    put:
      summary: Update an availability
      description: Updates an availability. The ID of the availabilty must be specified.
      operationId: putRestPropertiesAvailabilitiesAvailability
      x-api-path-slug: restpropertiesavailabilitiesavailabilityid-put
      parameters:
      - in: path
        name: availabilityId
      responses:
        200:
          description: OK
      tags:
      - Availability
  /rest/properties/destinations:
    get:
      summary: Get property destinations
      description: 'Returns a json with the destinations processed: data from providers
        and translations.'
      operationId: getRestPropertiesDestinations
      x-api-path-slug: restpropertiesdestinations-get
      responses:
        200:
          description: OK
      tags:
      - Property
      - Destinations
  /rest/properties/groups:
    get:
      summary: List property groups
      description: Lists property groups.
      operationId: getRestPropertiesGroups
      x-api-path-slug: restpropertiesgroups-get
      parameters:
      - in: query
        name: groupId
        description: The ID of the group
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Groups
    post:
      summary: Create a property group
      description: Creates a property group.
      operationId: postRestPropertiesGroups
      x-api-path-slug: restpropertiesgroups-post
      parameters:
      - in: body
        name: /rest/properties/groups
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: names
        description: The names of the group
      - in: query
        name: options
        description: The options of the group
      - in: query
        name: position
        description: The position  of the group
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
  /rest/properties/groups/names:
    get:
      summary: List group names
      description: Lists group names.
      operationId: getRestPropertiesGroupsNames
      x-api-path-slug: restpropertiesgroupsnames-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Group
      - Names
    post:
      summary: Create an group name
      description: Create an group name.
      operationId: postRestPropertiesGroupsNames
      x-api-path-slug: restpropertiesgroupsnames-post
      parameters:
      - in: body
        name: /rest/properties/groups/names
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: lang
        description: The lang of the group name
      - in: query
        name: name
        description: The name of the group name
      - in: query
        name: propertyId
        description: The ID of the property
      responses:
        200:
          description: OK
      tags:
      - Group
      - Name
  /rest/properties/groups/names/{groupNameId}:
    delete:
      summary: Delete a group name
      description: Deletes a group name. The ID of the group name must be specified.
      operationId: deleteRestPropertiesGroupsNamesGroupname
      x-api-path-slug: restpropertiesgroupsnamesgroupnameid-delete
      parameters:
      - in: path
        name: groupNameId
      responses:
        200:
          description: OK
      tags:
      - Group
      - Name
    get:
      summary: Get a group name
      description: Gets a group name. The ID of the group name must be specified.
      operationId: getRestPropertiesGroupsNamesGroupname
      x-api-path-slug: restpropertiesgroupsnamesgroupnameid-get
      parameters:
      - in: path
        name: groupNameId
      responses:
        200:
          description: OK
      tags:
      - Group
      - Name
    put:
      summary: Update a group name
      description: Updates a group name. The ID of the group name must be specified.
      operationId: putRestPropertiesGroupsNamesGroupname
      x-api-path-slug: restpropertiesgroupsnamesgroupnameid-put
      parameters:
      - in: path
        name: groupNameId
      responses:
        200:
          description: OK
      tags:
      - Group
      - Name
  /rest/properties/groups/options:
    get:
      summary: List group options
      description: Lists group options.
      operationId: getRestPropertiesGroupsOptions
      x-api-path-slug: restpropertiesgroupsoptions-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Group
      - Options
    post:
      summary: Create a group option
      description: Creates a group option
      operationId: postRestPropertiesGroupsOptions
      x-api-path-slug: restpropertiesgroupsoptions-post
      parameters:
      - in: body
        name: /rest/properties/groups/options
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: groupOptionIdentifier
        description: The groupOptionIdentifier of the group name
      - in: query
        name: propertyGroupId
        description: The ID of the property group
      - in: query
        name: value
        description: The value of the group name
      responses:
        200:
          description: OK
      tags:
      - Group
      - Option
  /rest/properties/groups/options/{groupOptionId}:
    delete:
      summary: Delete a group option
      description: Deletes a group option. The ID of the group option must be specified.
      operationId: deleteRestPropertiesGroupsOptionsGroupoption
      x-api-path-slug: restpropertiesgroupsoptionsgroupoptionid-delete
      parameters:
      - in: path
        name: groupOptionId
      responses:
        200:
          description: OK
      tags:
      - Group
      - Option
    get:
      summary: Get a group option
      description: Gets a group option. The ID of the group option must be specified.
      operationId: getRestPropertiesGroupsOptionsGroupoption
      x-api-path-slug: restpropertiesgroupsoptionsgroupoptionid-get
      parameters:
      - in: path
        name: groupOptionId
      responses:
        200:
          description: OK
      tags:
      - Group
      - Option
    put:
      summary: Update a group option
      description: Updates a group option. The ID of the group option must be specified.
      operationId: putRestPropertiesGroupsOptionsGroupoption
      x-api-path-slug: restpropertiesgroupsoptionsgroupoptionid-put
      parameters:
      - in: path
        name: groupOptionId
      responses:
        200:
          description: OK
      tags:
      - Group
      - Option
  /rest/properties/groups/surcharge/types:
    get:
      summary: Get surcharge types from module configuration
      description: Get surcharge types from module configuration.
      operationId: getRestPropertiesGroupsSurchargeTypes
      x-api-path-slug: restpropertiesgroupssurchargetypes-get
      responses:
        200:
          description: OK
      tags:
      - Surcharge
      - Types
      - From
      - Module
      - Configuration
  /rest/properties/groups/types:
    get:
      summary: Get group types from module configuration
      description: Get group types from module configuration.
      operationId: getRestPropertiesGroupsTypes
      x-api-path-slug: restpropertiesgroupstypes-get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Types
      - From
      - Module
      - Configuration
  /rest/properties/groups/{groupId}:
    get:
      summary: Get a property group
      description: Gets a property group. The ID of the property group must be specified.
      operationId: getRestPropertiesGroupsGroup
      x-api-path-slug: restpropertiesgroupsgroupid-get
      parameters:
      - in: path
        name: groupId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
    put:
      summary: Update a property group
      description: Updates a property group. The ID of the property group must be
        specified.
      operationId: putRestPropertiesGroupsGroup
      x-api-path-slug: restpropertiesgroupsgroupid-put
      parameters:
      - in: body
        name: /rest/properties/groups/{groupId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupId
      - in: query
        name: names
        description: The names of the group
      - in: query
        name: options
        description: The options of the group
      - in: query
        name: position
        description: The position  of the group
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
  /rest/properties/groups/{groupId}/properties:
    post:
      summary: Mass attach propertyId and groupId collection into the pivot table.
      description: Mass attach propertyid and groupid collection into the pivot table..
      operationId: postRestPropertiesGroupsGroupProperties
      x-api-path-slug: restpropertiesgroupsgroupidproperties-post
      parameters:
      - in: path
        name: groupId
      responses:
        200:
          description: OK
      tags:
      - Mass
      - Attach
      - PropertyId
      - GroupId
      - Collection
      - Into
      - Pivot
      - Table
  /rest/properties/groups/{groupId}/properties/{propertyId}:
    delete:
      summary: Detach a property from a property group.
      description: Detaches a property from a property group. The ID of the property
        and the ID of the property group must be specified.
      operationId: deleteRestPropertiesGroupsGroupPropertiesProperty
      x-api-path-slug: restpropertiesgroupsgroupidpropertiespropertyid-delete
      parameters:
      - in: path
        name: groupId
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Detach
      - Property
      - From
      - Property
      - Group
    post:
      summary: Attach a property to a property group
      description: Attaches a property to a property group. The ID of the property
        and the ID of the property group must be specified.
      operationId: postRestPropertiesGroupsGroupPropertiesProperty
      x-api-path-slug: restpropertiesgroupsgroupidpropertiespropertyid-post
      parameters:
      - in: path
        name: groupId
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Attach
      - Property
      - To
      - Property
      - Group
  /rest/properties/groups/{propertyId}:
    delete:
      summary: Delete a property group
      description: Deletes a property group. The ID of the property group must be
        specified.
      operationId: deleteRestPropertiesGroupsProperty
      x-api-path-slug: restpropertiesgroupspropertyid-delete
      parameters:
      - in: query
        name: groupId
        description: The ID of the group
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
  /rest/properties/markets:
    get:
      summary: List property markets
      description: Lists property markets
      operationId: getRestPropertiesMarkets
      x-api-path-slug: restpropertiesmarkets-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Markets
    post:
      summary: Create a property market
      description: Creates a property market.
      operationId: postRestPropertiesMarkets
      x-api-path-slug: restpropertiesmarkets-post
      parameters:
      - in: body
        name: /rest/properties/markets
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: propertyId
        description: Property id
      - in: query
        name: referrerId
        description: The referrer id of the property market
      - in: query
        name: referrerSubId
        description: The referrer sub id of the property market
      - in: query
        name: value
        description: The value of the property market
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
  /rest/properties/markets/{propertiesMarketId}:
    delete:
      summary: Delete a property market
      description: Deletes a property market. The ID of the property market must be
        specified.
      operationId: deleteRestPropertiesMarketsPropertiesmarket
      x-api-path-slug: restpropertiesmarketspropertiesmarketid-delete
      parameters:
      - in: path
        name: propertiesMarketId
      - in: query
        name: propertyMarketId
        description: The ID of the property market
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
    get:
      summary: Get a property market
      description: Gets a property market. The ID of the property market must be specified.
      operationId: getRestPropertiesMarketsPropertiesmarket
      x-api-path-slug: restpropertiesmarketspropertiesmarketid-get
      parameters:
      - in: path
        name: propertiesMarketId
      - in: query
        name: propertyMarketId
        description: The ID of the property market
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
    put:
      summary: Update a property market
      description: Updates a property market. The ID of the property market must be
        specified.
      operationId: putRestPropertiesMarketsPropertiesmarket
      x-api-path-slug: restpropertiesmarketspropertiesmarketid-put
      parameters:
      - in: body
        name: /rest/properties/markets/{propertiesMarketId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: propertiesMarketId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Market
  /rest/properties/names:
    get:
      summary: List names
      description: Lists names.
      operationId: getRestPropertiesNames
      x-api-path-slug: restpropertiesnames-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
    post:
      summary: Create a name
      description: Creates a name
      operationId: postRestPropertiesNames
      x-api-path-slug: restpropertiesnames-post
      parameters:
      - in: body
        name: /rest/properties/names
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: description
        description: The description of the property name
      - in: query
        name: lang
        description: The lang of the property name
      - in: query
        name: name
        description: The name of the property name
      - in: query
        name: propertyId
        description: The id of the property name
      responses:
        200:
          description: OK
      tags:
      - Name
  /rest/properties/names/{nameId}:
    delete:
      summary: Delete a property name
      description: Deletes a property name. The ID of the property name must be specified.
      operationId: deleteRestPropertiesNamesName
      x-api-path-slug: restpropertiesnamesnameid-delete
      parameters:
      - in: path
        name: nameId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Name
    get:
      summary: Get a property name
      description: Gets a proeprty name. The ID of the property name must be specified.
      operationId: getRestPropertiesNamesName
      x-api-path-slug: restpropertiesnamesnameid-get
      parameters:
      - in: path
        name: nameId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Name
    put:
      summary: Update a property name
      description: Updates a property name. The ID of the property name must be specified
      operationId: putRestPropertiesNamesName
      x-api-path-slug: restpropertiesnamesnameid-put
      parameters:
      - in: path
        name: nameId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Name
  /rest/properties/options:
    get:
      summary: List property options
      description: Lists property options.
      operationId: getRestPropertiesOptions
      x-api-path-slug: restpropertiesoptions-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Options
    post:
      summary: Create a property option
      description: Creates a property option.
      operationId: postRestPropertiesOptions
      x-api-path-slug: restpropertiesoptions-post
      parameters:
      - in: body
        name: /rest/properties/options
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: propertyId
        description: ID of the property
      - in: query
        name: typeOptionIdentifier
        description: The identifier of the property option type
      responses:
        200:
          description: OK
      tags:
      - Property
      - Option
  /rest/properties/options/{propertyOptionId}:
    delete:
      summary: Delete a property option
      description: Deletes a property option. The ID of the proeprty option must be
        specified.
      operationId: deleteRestPropertiesOptionsPropertyoption
      x-api-path-slug: restpropertiesoptionspropertyoptionid-delete
      parameters:
      - in: path
        name: propertyOptionId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Option
    get:
      summary: Get a property option
      description: Gets a property option. The ID of the property option must be specified.
      operationId: getRestPropertiesOptionsPropertyoption
      x-api-path-slug: restpropertiesoptionspropertyoptionid-get
      parameters:
      - in: path
        name: propertyOptionId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Option
    put:
      summary: Update a property option
      description: Updates a property option. The ID of the property option must be
        specified.
      operationId: putRestPropertiesOptionsPropertyoption
      x-api-path-slug: restpropertiesoptionspropertyoptionid-put
      parameters:
      - in: query
        name: $propertyOptionId
        description: The ID of the property option
      - in: path
        name: propertyOptionId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Option
  /rest/properties/relations:
    delete:
      summary: Delete property relations
      description: Deletes property relations. The ID of the property relations must
        be specified.
      operationId: deleteRestPropertiesRelations
      x-api-path-slug: restpropertiesrelations-delete
      parameters:
      - in: query
        name: relationId
        description: The ID of the property relation
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relations
    get:
      summary: List property relations
      description: Lists property relations.
      operationId: getRestPropertiesRelations
      x-api-path-slug: restpropertiesrelations-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Relations
    post:
      summary: Create a property relation
      description: Creates a property relation
      operationId: postRestPropertiesRelations
      x-api-path-slug: restpropertiesrelations-post
      parameters:
      - in: body
        name: /rest/properties/relations
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: propertyId
        description: The ID of the property
      - in: query
        name: relationTargetId
        description: The ID of the property relation target
      - in: query
        name: relationTypeIdentifier
        description: The identifier of the property relation type
      - in: query
        name: selectionRelationId
        description: The ID of the property selection relation
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
    put:
      summary: Update relations
      description: Updates relations
      operationId: putRestPropertiesRelations
      x-api-path-slug: restpropertiesrelations-put
      parameters:
      - in: query
        name: relationId
        description: The ID of the property relation
      responses:
        200:
          description: OK
      tags:
      - Relations
  /rest/properties/relations/markups:
    get:
      summary: List relation markups
      description: Lists relation markups.
      operationId: getRestPropertiesRelationsMarkups
      x-api-path-slug: restpropertiesrelationsmarkups-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Relation
      - Markups
    post:
      summary: Create a property relation markup
      description: Creates a property relation markup
      operationId: postRestPropertiesRelationsMarkups
      x-api-path-slug: restpropertiesrelationsmarkups-post
      parameters:
      - in: body
        name: /rest/properties/relations/markups
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: markup
        description: The property relation markup
      - in: query
        name: propertyRelationId
        description: The ID of the property elation
      - in: query
        name: variationSalesPriceId
        description: The ID of a variations sales price
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Markup
  /rest/properties/relations/markups/{relationMarkupId}:
    delete:
      summary: Delete a property relation markup
      description: Deletes a property relation markup
      operationId: deleteRestPropertiesRelationsMarkupsRelationmarkup
      x-api-path-slug: restpropertiesrelationsmarkupsrelationmarkupid-delete
      parameters:
      - in: path
        name: relationMarkupId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Markup
    get:
      summary: Get a property relation markup
      description: Gets a property relation markup. The ID of the property relation
        markup must be specified.
      operationId: getRestPropertiesRelationsMarkupsRelationmarkup
      x-api-path-slug: restpropertiesrelationsmarkupsrelationmarkupid-get
      parameters:
      - in: path
        name: relationMarkupId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Markup
    put:
      summary: Update a property relation markup
      description: Updates a property relation markup
      operationId: putRestPropertiesRelationsMarkupsRelationmarkup
      x-api-path-slug: restpropertiesrelationsmarkupsrelationmarkupid-put
      parameters:
      - in: path
        name: relationMarkupId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Markup
  /rest/properties/relations/values:
    get:
      summary: List property relation values
      description: Lists property relation values.
      operationId: getRestPropertiesRelationsValues
      x-api-path-slug: restpropertiesrelationsvalues-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Relation
      - Values
    post:
      summary: Create a property relation value
      description: Creates a property relation value.
      operationId: postRestPropertiesRelationsValues
      x-api-path-slug: restpropertiesrelationsvalues-post
      parameters:
      - in: body
        name: /rest/properties/relations/values
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: lang
        description: The lang of the property relation value
      - in: query
        name: propertyId
        description: The ID of the property
      - in: query
        name: value
        description: The value of the property relation
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Value
    put:
      summary: Update multiple property relation value
      description: Updates multiple property relation value
      operationId: putRestPropertiesRelationsValues
      x-api-path-slug: restpropertiesrelationsvalues-put
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Property
      - Relation
      - Value
  /rest/properties/relations/values/{propertiesRelationValueId}:
    delete:
      summary: Delete a property relation value
      description: Deletes a property relation value. The ID of the property relation
        value must be specified.
      operationId: deleteRestPropertiesRelationsValuesPropertiesrelationvalue
      x-api-path-slug: restpropertiesrelationsvaluespropertiesrelationvalueid-delete
      parameters:
      - in: path
        name: propertiesRelationValueId
      - in: query
        name: propertyRelationValueId
        description: The ID of the property relation value
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Value
    put:
      summary: Update a property relation value
      description: Updates a property relation value. The ID of the property relation
        value must be specified.
      operationId: putRestPropertiesRelationsValuesPropertiesrelationvalue
      x-api-path-slug: restpropertiesrelationsvaluespropertiesrelationvalueid-put
      parameters:
      - in: query
        name: $propertyRelationValueId
        description: The ID of the property relation value
      - in: path
        name: propertiesRelationValueId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Value
  /rest/properties/relations/values/{relationMarkupId}:
    get:
      summary: Get a property relation value
      description: Gets a property relation value. The ID of the property relation
        value must be specified.
      operationId: getRestPropertiesRelationsValuesRelationmarkup
      x-api-path-slug: restpropertiesrelationsvaluesrelationmarkupid-get
      parameters:
      - in: query
        name: propertyRelationId
        description: The ID of the property relation
      - in: path
        name: relationMarkupId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Value
  /rest/properties/relations/{relationId}:
    delete:
      summary: Delete a property relation
      description: Deletes a property relation. The ID of the property relation must
        be specified.
      operationId: deleteRestPropertiesRelationsRelation
      x-api-path-slug: restpropertiesrelationsrelationid-delete
      parameters:
      - in: path
        name: relationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
    get:
      summary: Get a property relation
      description: Gets a property relation. The ID of the property relation must
        be specified.
      operationId: getRestPropertiesRelationsRelation
      x-api-path-slug: restpropertiesrelationsrelationid-get
      parameters:
      - in: path
        name: relationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
    put:
      summary: Update a property relation
      description: Updates a property relation. The ID of the property relation must
        be specified.
      operationId: putRestPropertiesRelationsRelation
      x-api-path-slug: restpropertiesrelationsrelationid-put
      parameters:
      - in: path
        name: relationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
  /rest/properties/selections:
    get:
      summary: List property selections
      description: Lists property selections
      operationId: getRestPropertiesSelections
      x-api-path-slug: restpropertiesselections-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Selections
    post:
      summary: Create a property selection
      description: Creates a property selection.
      operationId: postRestPropertiesSelections
      x-api-path-slug: restpropertiesselections-post
      parameters:
      - in: body
        name: /rest/properties/selections
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: position
        description: The position of the property selection
      - in: query
        name: propertyId
        description: The ID of the property
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
  /rest/properties/selections/{propertySelectionId}:
    delete:
      summary: Delete a property selection
      description: Deletes a property selection
      operationId: deleteRestPropertiesSelectionsPropertyselection
      x-api-path-slug: restpropertiesselectionspropertyselectionid-delete
      parameters:
      - in: path
        name: propertySelectionId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
    get:
      summary: Get a property selection
      description: Gets a property selection. The ID of property selection must be
        specified.
      operationId: getRestPropertiesSelectionsPropertyselection
      x-api-path-slug: restpropertiesselectionspropertyselectionid-get
      parameters:
      - in: path
        name: propertySelectionId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
    put:
      summary: Update a property selection
      description: Updates a property selection. The ID of the property selection
        must be specifed.
      operationId: putRestPropertiesSelectionsPropertyselection
      x-api-path-slug: restpropertiesselectionspropertyselectionid-put
      parameters:
      - in: query
        name: $propertySelectionId
        description: The ID of the property selection
      - in: path
        name: propertySelectionId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Selection
  /rest/properties/systemlang:
    get:
      summary: Get system language
      description: Gets the system language.
      operationId: getRestPropertiesSystemlang
      x-api-path-slug: restpropertiessystemlang-get
      responses:
        200:
          description: OK
      tags:
      - System
      - Language
  /rest/properties/{propertyId}:
    delete:
      summary: Delete a property
      description: Deletes a property. The ID of the property must be specified
      operationId: deleteRestPropertiesProperty
      x-api-path-slug: restpropertiespropertyid-delete
      parameters:
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
    get:
      summary: Get a property.
      description: Gets a property. The ID of the property must be specified.
      operationId: getRestPropertiesProperty
      x-api-path-slug: restpropertiespropertyid-get
      parameters:
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
    put:
      summary: Update a property
      description: Updates a property. The ID of the property must be specified.
      operationId: putRestPropertiesProperty
      x-api-path-slug: restpropertiespropertyid-put
      parameters:
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
  /rest/shop_builder/content_links:
    get:
      summary: List all content links for a given plugin set
      description: List all content links for a given plugin set.
      operationId: getRestShopBuilderContentLinks
      x-api-path-slug: restshop-buildercontent-links-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Content
      - Linksa
      - Given
      - Plugin
      - Set
    post:
      summary: Link a content to a a layout container of a frontend plugin.
      description: Link a content to a a layout container of a frontend plugin..
      operationId: postRestShopBuilderContentLinks
      x-api-path-slug: restshop-buildercontent-links-post
      parameters:
      - in: body
        name: /rest/shop_builder/content_links
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Link
      - Content
      - To
      - A
      - Layout
      - Container
      - Of
      - Frontend
      - Plugin
  /rest/shop_builder/content_links/{contentLinkId}:
    delete:
      summary: Delete a content link.
      description: Delete a content link..
      operationId: deleteRestShopBuilderContentLinksContentlink
      x-api-path-slug: restshop-buildercontent-linkscontentlinkid-delete
      parameters:
      - in: path
        name: contentLinkId
      responses:
        200:
          description: OK
      tags:
      - Content
      - Link
    get:
      summary: Find a content link by id.
      description: Find a content link by id..
      operationId: getRestShopBuilderContentLinksContentlink
      x-api-path-slug: restshop-buildercontent-linkscontentlinkid-get
      parameters:
      - in: path
        name: contentLinkId
      responses:
        200:
          description: OK
      tags:
      - Find
      - Content
      - Link
      - By
      - Id
    put:
      summary: Update a content link.
      description: Update a content link..
      operationId: putRestShopBuilderContentLinksContentlink
      x-api-path-slug: restshop-buildercontent-linkscontentlinkid-put
      parameters:
      - in: body
        name: /rest/shop_builder/content_links/{contentLinkId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contentLinkId
      responses:
        200:
          description: OK
      tags:
      - Content
      - Link
  /rest/shop_builder/contents:
    get:
      summary: List all contents.
      description: List all contents..
      operationId: getRestShopBuilderContents
      x-api-path-slug: restshop-buildercontents-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Contents
    post:
      summary: Create a new content.
      description: Create a new content..
      operationId: postRestShopBuilderContents
      x-api-path-slug: restshop-buildercontents-post
      parameters:
      - in: body
        name: /rest/shop_builder/contents
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Content
  /rest/shop_builder/contents/{contentId}:
    delete:
      summary: Delete a content
      description: Delete a content.
      operationId: deleteRestShopBuilderContentsContent
      x-api-path-slug: restshop-buildercontentscontentid-delete
      parameters:
      - in: path
        name: contentId
      responses:
        200:
          description: OK
      tags:
      - Content
    get:
      summary: Find a content by id.
      description: Find a content by id..
      operationId: getRestShopBuilderContentsContent
      x-api-path-slug: restshop-buildercontentscontentid-get
      parameters:
      - in: path
        name: contentId
      responses:
        200:
          description: OK
      tags:
      - Find
      - Content
      - By
      - Id
    put:
      summary: Update a content.
      description: Update a content..
      operationId: putRestShopBuilderContentsContent
      x-api-path-slug: restshop-buildercontentscontentid-put
      parameters:
      - in: body
        name: /rest/shop_builder/contents/{contentId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contentId
      responses:
        200:
          description: OK
      tags:
      - Content
  /rest/shop_builder/pages:
    get:
      summary: List content pages from all plugins in a given plugin set.
      description: List content pages from all plugins in a given plugin set..
      operationId: getRestShopBuilderPages
      x-api-path-slug: restshop-builderpages-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Content
      - Pages
      - From
      - ""
      - Plugins
      - In
      - Given
      - Plugin
      - Set
  /rest/shop_builder/widgets:
    get:
      summary: List all widgets provided by all frontend plugins of a given plugin
        set.
      description: List all widgets provided by all frontend plugins of a given plugin
        set..
      operationId: getRestShopBuilderWgets
      x-api-path-slug: restshop-builderwidgets-get
      parameters:
      - in: query
        name: identifier
        description: Filter results by widget identifier
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Widgets
      - Provided
      - By
      - ""
      - Frontend
      - Plugins
      - Of
      - Given
      - Plugin
      - Set
    post:
      summary: Render the preview for widgets.
      description: Render the preview for widgets..
      operationId: postRestShopBuilderWgets
      x-api-path-slug: restshop-builderwidgets-post
      responses:
        200:
          description: OK
      tags:
      - Render
      - Previewwidgets
  /rest/stockmanagement/stock:
    get:
      summary: List stock
      description: Lists stock of all warehouses.
      operationId: getRestStockmanagementStock
      x-api-path-slug: reststockmanagementstock-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to stock that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to stock that were last
          updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to stock with a variation
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
  /rest/stockmanagement/stock/redistribute:
    put:
      summary: Redistribute stock
      description: Redistributes stock of one storage location among one or more storage
        locations.
      operationId: putRestStockmanagementStockRedistribute
      x-api-path-slug: reststockmanagementstockredistribute-put
      parameters:
      - in: body
        name: /rest/stockmanagement/stock/redistribute
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Redistribute
      - Stock
  /rest/stockmanagement/stock/types/{type}:
    get:
      summary: List stock by warehouse type
      description: Lists stock for all warehouses of the same warehouse type. The
        name of the type must be specified. Currently the only type available is 'sales'.
      operationId: getRestStockmanagementStockTypesType
      x-api-path-slug: reststockmanagementstocktypestype-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: type
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to stock that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to stock that were last
          updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to stock with a variation
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - By
      - Warehouse
      - Type
  /rest/stockmanagement/warehouses:
    get:
      summary: List warehouses
      description: Lists warehouses without applying any filters.
      operationId: getRestStockmanagementWarehouses
      x-api-path-slug: reststockmanagementwarehouses-get
      parameters:
      - in: query
        name: with
        description: Related objects to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Warehouses
    post:
      summary: Create a warehouse
      description: Create a warehouse.
      operationId: postRestStockmanagementWarehouses
      x-api-path-slug: reststockmanagementwarehouses-post
      parameters:
      - in: body
        name: /rest/stockmanagement/warehouses
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Warehouse
  /rest/stockmanagement/warehouses/addresses:
    post:
      summary: Create an address for existing warehouse
      description: Create an address for existing warehouse.
      operationId: postRestStockmanagementWarehousesAddresses
      x-api-path-slug: reststockmanagementwarehousesaddresses-post
      responses:
        200:
          description: OK
      tags:
      - Addressexisting
      - Warehouse
  /rest/stockmanagement/warehouses/{warehouseId}:
    get:
      summary: Get a warehouse
      description: Gets a warehouse. The id of the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouse
      x-api-path-slug: reststockmanagementwarehouseswarehouseid-get
      parameters:
      - in: path
        name: warehouseId
      - in: query
        name: with
        description: Related objects to be loaded
      responses:
        200:
          description: OK
      tags:
      - Warehouse
  /rest/stockmanagement/warehouses/{warehouseId}/addresses/{relationTypeId?}:
    get:
      summary: List warehouse addresses
      description: List warehouse addresses. The ID of the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseAddressesRelationtype
      x-api-path-slug: reststockmanagementwarehouseswarehouseidaddressesrelationtypeid-get
      parameters:
      - in: path
        name: relationTypeId?
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - List
      - Warehouse
      - Addresses
  /rest/stockmanagement/warehouses/{warehouseId}/management/racks:
    get:
      summary: List racks
      description: Lists racks for a warehouse. The id of the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseManagementRacks
      x-api-path-slug: reststockmanagementwarehouseswarehouseidmanagementracks-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: query
        name: itemsPerPage
        description: Number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: warehouseId
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Racks
    post:
      summary: Create a rack
      description: Creates a rack. The id of the warehouse must be specified.
      operationId: postRestStockmanagementWarehousesWarehouseManagementRacks
      x-api-path-slug: reststockmanagementwarehouseswarehouseidmanagementracks-post
      parameters:
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - Rack
  /rest/stockmanagement/warehouses/{warehouseId}/management/racks/{rackId}:
    get:
      summary: Get a rack
      description: Gets a rack. The id of the rack and the id of the warehouse must
        be specified.
      operationId: getRestStockmanagementWarehousesWarehouseManagementRacksRack
      x-api-path-slug: reststockmanagementwarehouseswarehouseidmanagementracksrackid-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: path
        name: rackId
      - in: path
        name: warehouseId
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - Rack
  /rest/stockmanagement/warehouses/{warehouseId}/management/racks/{rackId}/shelves:
    get:
      summary: List shelves
      description: Lists shelves for a warehouse. The id of the rack and the id of
        the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseManagementRacksRackShelves
      x-api-path-slug: reststockmanagementwarehouseswarehouseidmanagementracksrackidshelves-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: query
        name: itemsPerPage
        description: Number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: rackId
      - in: path
        name: warehouseId
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Shelves
    post:
      summary: Create a shelf
      description: Creates a shelf. The id of the warehouse and the id of the rack
        must be specified.
      operationId: postRestStockmanagementWarehousesWarehouseManagementRacksRackShelves
      x-api-path-slug: reststockmanagementwarehouseswarehouseidmanagementracksrackidshelves-post
      parameters:
      - in: path
        name: rackId
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - Shelf
  /rest/stockmanagement/warehouses/{warehouseId}/management/racks/{rackId}/shelves/{shelfId}:
    get:
      summary: Get a shelf
      description: Gets a shelf. The id of the shelf, the id of the rack and the id
        of the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseManagementRacksRackShelvesShelf
      x-api-path-slug: reststockmanagementwarehouseswarehouseidmanagementracksrackidshelvesshelfid-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: path
        name: rackId
      - in: path
        name: shelfId
      - in: path
        name: warehouseId
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - Shelf
  /rest/stockmanagement/warehouses/{warehouseId}/management/racks/{rackId}/shelves/{shelfId}/storageLocations:
    get:
      summary: List storage locations
      description: Lists storage locations. The id of the warehouse, the id of the
        rack and the id of the shelf must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseManagementRacksRackShelvesShelfStoragelocations
      x-api-path-slug: reststockmanagementwarehouseswarehouseidmanagementracksrackidshelvesshelfidstoragelocations-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: query
        name: itemsPerPage
        description: Number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: rackId
      - in: path
        name: shelfId
      - in: path
        name: warehouseId
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Storage
      - Locations
    post:
      summary: Create a storage location
      description: Creates a storage location. The id of the warehouse, the id of
        the rack and the id of the shelf must be specified.
      operationId: postRestStockmanagementWarehousesWarehouseManagementRacksRackShelvesShelfStoragelocations
      x-api-path-slug: reststockmanagementwarehouseswarehouseidmanagementracksrackidshelvesshelfidstoragelocations-post
      parameters:
      - in: path
        name: rackId
      - in: path
        name: shelfId
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Location
  /rest/stockmanagement/warehouses/{warehouseId}/management/racks/{rackId}/shelves/{shelfId}/storageLocations/{storageLocationId}:
    get:
      summary: Get a storage location
      description: Gets a storage location. The id of the warehouse, the id of the
        rack, the id of the shelf and the id of the storage location must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseManagementRacksRackShelvesShelfStoragelocationsStoragelocat
      x-api-path-slug: reststockmanagementwarehouseswarehouseidmanagementracksrackidshelvesshelfidstoragelocationsstoragelocationid-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: path
        name: rackId
      - in: path
        name: shelfId
      - in: path
        name: storageLocationId
      - in: path
        name: warehouseId
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Location
  /rest/stockmanagement/warehouses/{warehouseId}/management/storageLocations:
    get:
      summary: List storage locations
      description: Lists storage locations that belong to a warehouse. The id of the
        warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseManagementStoragelocations
      x-api-path-slug: reststockmanagementwarehouseswarehouseidmanagementstoragelocations-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: query
        name: itemsPerPage
        description: Number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: warehouseId
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Storage
      - Locations
  /rest/stockmanagement/warehouses/{warehouseId}/management/storageLocations/{storageLocationId}:
    get:
      summary: Get a storage location
      description: Gets a storage location. The id of the storage location and the
        id of the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseManagementStoragelocationsStoragelocation
      x-api-path-slug: reststockmanagementwarehouseswarehouseidmanagementstoragelocationsstoragelocationid-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: path
        name: storageLocationId
      - in: path
        name: warehouseId
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Location
  /rest/stockmanagement/warehouses/{warehouseId}/stock:
    get:
      summary: List stock by warehouse
      description: Lists stock for a warehouse. The ID of the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseStock
      x-api-path-slug: reststockmanagementwarehouseswarehouseidstock-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to stock that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to stock that were last
          updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to stock with a variation
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - By
      - Warehouse
  /rest/stockmanagement/warehouses/{warehouseId}/stock/bookIncomingItems:
    put:
      summary: Book incoming stock
      description: Books incoming stock for multiple variations. The incoming stock
        will be added to the existing stock. The ID of the warehouse must be specified.
      operationId: putRestStockmanagementWarehousesWarehouseStockBookincomingitems
      x-api-path-slug: reststockmanagementwarehouseswarehouseidstockbookincomingitems-put
      parameters:
      - in: body
        name: /rest/stockmanagement/warehouses/{warehouseId}/stock/bookIncomingItems
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - Book
      - Incoming
      - Stock
  /rest/stockmanagement/warehouses/{warehouseId}/stock/correction:
    put:
      summary: Correct stock
      description: Corrects stock. The ID of the warehouse must be specified.
      operationId: putRestStockmanagementWarehousesWarehouseStockCorrection
      x-api-path-slug: reststockmanagementwarehouseswarehouseidstockcorrection-put
      parameters:
      - in: body
        name: /rest/stockmanagement/warehouses/{warehouseId}/stock/correction
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - Correct
      - Stock
  /rest/stockmanagement/warehouses/{warehouseId}/stock/movements:
    get:
      summary: List stock movements
      description: |-
        Lists stock movements for a warehouse. The ID of the warehouse must be specified. To get movements older than 3 months, set the 'year' parameter.
        NOTE: You can either get archive entries or non-archive entries. You can not get entries for the current year that are younger and older than 3 months with one request. You need separate requests to get entries older and younger than 3 months. To get all entries younger than 3 month you do not need to specify a year or any createdAt parameter.
      operationId: getRestStockmanagementWarehousesWarehouseStockMovements
      x-api-path-slug: reststockmanagementwarehouseswarehouseidstockmovements-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: createdAtFrom
        description: Get entries with createdAt date after this date
      - in: query
        name: createdAtTo
        description: Get entries with createdAt date before this date
      - in: query
        name: itemId
        description: The ID of the item
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: query
        name: variationId
        description: The ID of the variation
      - in: path
        name: warehouseId
      - in: query
        name: year
        description: Get entries from the archive for the given year
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - Movements
  /rest/stockmanagement/warehouses/{warehouseId}/stock/storageLocations:
    get:
      summary: List stock of a warehouse per storage location
      description: Lists stock of a warehouse for each variation and storage location.
        The stock will only be listed if the stock is positive. Negative stock will
        not be listed. The ID of the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseStockStoragelocations
      x-api-path-slug: reststockmanagementwarehouseswarehouseidstockstoragelocations-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: query
        name: storageLocationId
        description: Filter that restricts the search result to stock of a storage
          location
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to stock that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to stock that were last
          updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to stock with a variation
      - in: path
        name: warehouseId
      - in: query
        name: with
        description: Load additional relations for a StockStorageLocation
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - Of
      - Warehouse
      - Per
      - Storage
      - Location
  /rest/storage/frontend/file:
    delete:
      summary: Remove a single object from frontend storage.
      description: Remove a single object from frontend storage..
      operationId: deleteRestStorageFrontendFile
      x-api-path-slug: reststoragefrontendfile-delete
      parameters:
      - in: query
        name: key
        description: The key of the object to delete
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Single
      - Object
      - From
      - Frontend
      - Storage
    get:
      summary: Get file information for a single object in frontend storage. Append
        public cloudfront url to retrieved object.
      description: Get file information for a single object in frontend storage. append
        public cloudfront url to retrieved object..
      operationId: getRestStorageFrontendFile
      x-api-path-slug: reststoragefrontendfile-get
      parameters:
      - in: query
        name: key
        description: The key of the object to get information about
      responses:
        200:
          description: OK
      tags:
      - File
      - Informationa
      - Single
      - Object
      - In
      - Frontend
      - Storage
      - ""
      - Append
      - Public
      - Cloudfront
      - Url
      - To
      - Retrieved
      - Object
    post:
      summary: Upload a single file to frontend storage.
      description: If file is an image, generate a thumbnail and store dimensions
        in metadata.
      operationId: postRestStorageFrontendFile
      x-api-path-slug: reststoragefrontendfile-post
      parameters:
      - in: query
        name: key
        description: The key for the uploaded object
      - in: query
        name: maxAge
        description: Number of seconds until the content of the file expires
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Single
      - File
      - To
      - Frontend
      - Storage
  /rest/storage/frontend/file/metadata:
    get:
      summary: Get assigend metadata for a single storage object
      description: Get assigend metadata for a single storage object.
      operationId: getRestStorageFrontendFileMetadata
      x-api-path-slug: reststoragefrontendfilemetadata-get
      parameters:
      - in: query
        name: key
        description: The key of the object to get metadata for
      responses:
        200:
          description: OK
      tags:
      - Assigend
      - Metadataa
      - Single
      - Storage
      - Object
    post:
      summary: Update metadata of an storage object
      description: Update metadata of an storage object.
      operationId: postRestStorageFrontendFileMetadata
      x-api-path-slug: reststoragefrontendfilemetadata-post
      parameters:
      - in: query
        name: key
        description: The key of the object to update metadata for
      - in: query
        name: metadata
        description: The metadata to assign to storage object
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Of
      - Storage
      - Object
  /rest/storage/frontend/files:
    delete:
      summary: Delete files from frontend storage.
      description: Deletes a list of files from frontend storage. A list of storage
        keys must be specified.
      operationId: deleteRestStorageFrontendFiles
      x-api-path-slug: reststoragefrontendfiles-delete
      parameters:
      - in: query
        name: keyList
        description: List of storage keys for the files to be deleted
      responses:
        200:
          description: OK
      tags:
      - Files
      - From
      - Frontend
      - Storage
    get:
      summary: List files from frontend storage. Append public cloudfront url to each
        retrieved object.
      description: List files from frontend storage. append public cloudfront url
        to each retrieved object..
      operationId: getRestStorageFrontendFiles
      x-api-path-slug: reststoragefrontendfiles-get
      parameters:
      - in: query
        name: continuationToken
        description: The continuationToken of a previous request to continue listing
          objects with
      responses:
        200:
          description: OK
      tags:
      - List
      - Files
      - From
      - Frontend
      - Storage
      - ""
      - Append
      - Public
      - Cloudfront
      - Url
      - To
      - Each
      - Retrieved
      - Object
  /rest/storage/frontend/object-url:
    get:
      summary: Get the URL for a layout document
      description: Gets the URL of a layout document. The storage key must be specified.
        The returned URL expires after 10 minutes.
      operationId: getRestStorageFrontendObjectUrl
      x-api-path-slug: reststoragefrontendobjecturl-get
      parameters:
      - in: query
        name: key
        description: The storage key for the frontend document to retrieve the URL
          for
      responses:
        200:
          description: OK
      tags:
      - URLa
      - Layout
      - Document
  /rest/storage/layout:
    delete:
      summary: Delete layout documents
      description: Deletes a list of layout documents from storage. A list of storage
        keys must be specified.
      operationId: deleteRestStorageLayout
      x-api-path-slug: reststoragelayout-delete
      parameters:
      - in: query
        name: keyList
        description: List of storage keys for the files to be deleted
      responses:
        200:
          description: OK
      tags:
      - Layout
      - Documents
    post:
      summary: Upload a layout document
      description: Uploads a layout document to storage. The storage key (i.e. file
        path) must be specified.
      operationId: postRestStorageLayout
      x-api-path-slug: reststoragelayout-post
      parameters:
      - in: query
        name: key
        description: The storage key for the layout document to upload
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Layout
      - Document
  /rest/storage/layout/list:
    get:
      summary: List layout documents
      description: |-
        Lists up to 1000 layout documents per request. If more than 1000 layout documents are available,
        a <code>nextContinuationToken</code> is returned. Use this token to get the next (up to) 1000 layout documents.
        Use the same request and include a field with the key <code>continuationToken</code> as well as the returned
        token from the previous call as the value.

        Check the <code>isTruncated</code> field in the response to see if more results are available. If <code>isTruncated</code> is true,
        repeat the request using the token from the <code>nextContinuationToken</code> field of the previous response to get all
        results.
      operationId: getRestStorageLayoutList
      x-api-path-slug: reststoragelayoutlist-get
      parameters:
      - in: query
        name: continuationToken
        description: Token for listing the next (up to) 1000 layout documents
      responses:
        200:
          description: OK
      tags:
      - List
      - Layout
      - Documents
  /rest/storage/layout/object-url:
    get:
      summary: Get the URL for a layout document
      description: Gets the URL of a layout document. The storage key must be specified.
        The returned URL expires after 10 minutes.
      operationId: getRestStorageLayoutObjectUrl
      x-api-path-slug: reststoragelayoutobjecturl-get
      parameters:
      - in: query
        name: key
        description: The storage key for the layout document to retrieve the URL for
      responses:
        200:
          description: OK
      tags:
      - URLa
      - Layout
      - Document
  /rest/storage/order-properties/object-url:
    get:
      summary: Get the URL for a order property file
      description: |-
        Gets the URL of a order property file. The storage key must be specified. The returned URL expires after 10
        minutes.
      operationId: getRestStorageOrderPropertiesObjectUrl
      x-api-path-slug: reststorageorderpropertiesobjecturl-get
      parameters:
      - in: query
        name: key
        description: The storage key for the order property     *                        file
          to retrieve the URL for
      responses:
        200:
          description: OK
      tags:
      - URLa
      - Order
      - Property
      - File
  /rest/storage/plugins/inbox:
    delete:
      summary: Delete files from the inbox
      description: Deletes a list of files from the inbox. A list of storage keys
        must be specified.
      operationId: deleteRestStoragePluginsInbox
      x-api-path-slug: reststoragepluginsinbox-delete
      parameters:
      - in: query
        name: keyList
        description: List of storage keys for the files to be deleted
      responses:
        200:
          description: OK
      tags:
      - Files
      - From
      - Inbox
    post:
      summary: Upload a file to the inbox
      description: Uploads a file to the inbox. The storage key (i.e. file path) must
        be specified.
      operationId: postRestStoragePluginsInbox
      x-api-path-slug: reststoragepluginsinbox-post
      parameters:
      - in: query
        name: key
        description: The storage key for the file to upload
      responses:
        200:
          description: OK
      tags:
      - Upload
      - File
      - To
      - Inbox
  /rest/storage/plugins/inbox/commit:
    post:
      summary: ""
      description: .
      operationId: postRestStoragePluginsInboxCommit
      x-api-path-slug: reststoragepluginsinboxcommit-post
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/storage/plugins/inbox/list:
    get:
      summary: List files from the inbox
      description: |-
        Lists all files of all plugins stored in the inbox. A prefix can be specified to list all files of a specific
        plugin folder only.
      operationId: getRestStoragePluginsInboxList
      x-api-path-slug: reststoragepluginsinboxlist-get
      parameters:
      - in: query
        name: prefix
        description: Prefix to list all files of a specific plugin folder only
      responses:
        200:
          description: OK
      tags:
      - List
      - Files
      - From
      - Inbox
  /rest/storage/plugins/inbox/object-url:
    get:
      summary: Get the content of a file from the inbox
      description: Gets the content of a file stored in the inbox. The storage key
        (i.e. file path) must be specified.
      operationId: getRestStoragePluginsInboxObjectUrl
      x-api-path-slug: reststoragepluginsinboxobjecturl-get
      parameters:
      - in: query
        name: key
        description: The storage key for the file to retrieve
      responses:
        200:
          description: OK
      tags:
      - Content
      - Of
      - File
      - From
      - Inbox
  /rest/stores/{plentyId}/locations:
    get:
      summary: Get the ID of an accounting location of a country
      description: Gets the ID of an accounting location of a country. The plenty
        ID of the client and the ID of the country must be specified.
      operationId: getRestStoresPlentyLocations
      x-api-path-slug: reststoresplentyidlocations-get
      parameters:
      - in: query
        name: countryId
        description: The ID of the country of the accounting location
      - in: path
        name: plentyId
      responses:
        200:
          description: OK
      tags:
      - ID
      - Of
      - Accounting
      - Location
      - Of
      - Country
  /rest/system/cloud/metrics:
    get:
      summary: Get the cloud metrics for this system
      description: Get the cloud metrics for this system.
      operationId: getRestSystemCloudMetrics
      x-api-path-slug: restsystemcloudmetrics-get
      responses:
        200:
          description: OK
      tags:
      - Cloud
      - Metricsthis
      - System
  /rest/system/metrics/{plentyId}/{date}:
    get:
      summary: Supply usage data for given plentymarkets system
      description: Supply usage data for given plentymarkets system.
      operationId: getRestSystemMetricsPlentyDate
      x-api-path-slug: restsystemmetricsplentyiddate-get
      parameters:
      - in: path
        name: date
      - in: path
        name: plentyId
      responses:
        200:
          description: OK
      tags:
      - Supply
      - Usage
      - Datagiven
      - Plentymarkets
      - System
  /rest/tickets:
    get:
      summary: List tickets by filters
      description: List tickets by filters.
      operationId: getRestTickets
      x-api-path-slug: resttickets-get
      parameters:
      - in: query
        name: confidential
        description: Filter that restricts the search result to tickets of a specific
          confidential value
      - in: query
        name: contactId
        description: Filter that restricts the search result to tickets with a specified
          contact ID
      - in: query
        name: customerClassId
        description: Filter that restricts the search result to tickets with a specified
          customer class ID
      - in: query
        name: deadlineAt
        description: Filter that restricts the search result to tickets with a specified
          deadline
      - in: query
        name: fulltext
        description: Filter that restricts the search result to tickets with full-text
          search
      - in: query
        name: id
        description: Filter that restricts the search result to tickets of a specific
          ticket ID
      - in: query
        name: ownerId
        description: Filter that restricts the search result to tickets with a specified
          owner ID
      - in: query
        name: parentTicketId
        description: Filter that restricts the search result to tickets with a specified
          parent ticket ID
      - in: query
        name: plentyId
        description: Filter that restricts the search result to tickets with a specified
          client (store) ID
      - in: query
        name: priorityId
        description: Filter that restricts the search result to tickets of a specific
          ticket priority ID
      - in: query
        name: progress
        description: Filter that restricts the search result to tickets with a specified
          progress in percent
      - in: query
        name: resubmissionAt
        description: Filter that restricts the search result to tickets with a specified
          resubmission date
      - in: query
        name: roleId
        description: Filter that restricts the search result to tickets with a specified
          role ID
      - in: query
        name: source
        description: Filter that restricts the search result to tickets with a specific
          source value
      - in: query
        name: statusGroupId
        description: Filter that restricts the search result to tickets with a specified
          status group ID
      - in: query
        name: statusId
        description: Filter that restricts the search result to tickets with a specified
          status ID
      - in: query
        name: title
        description: Filter that restricts the search result to tickets with a specified
          phrase in title
      - in: query
        name: typeId
        description: Filter that restricts the search result to tickets of specific
          ticket types
      responses:
        200:
          description: OK
      tags:
      - List
      - Tickets
      - By
      - Filters
    post:
      summary: Create a ticket
      description: Create a ticket.
      operationId: postRestTickets
      x-api-path-slug: resttickets-post
      parameters:
      - in: body
        name: /rest/tickets
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ticket
  /rest/tickets/status/names:
    get:
      summary: ""
      description: .
      operationId: getRestTicketsStatusNames
      x-api-path-slug: restticketsstatusnames-get
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/tickets/status/type/names:
    get:
      summary: ""
      description: .
      operationId: getRestTicketsStatusTypeNames
      x-api-path-slug: restticketsstatustypenames-get
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/tickets/types/names:
    get:
      summary: ""
      description: .
      operationId: getRestTicketsTypesNames
      x-api-path-slug: restticketstypesnames-get
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/tickets/{ticketId}:
    post:
      summary: Create a message
      description: Creates a message for the ticket. The ID of the ticket must be
        specified.
      operationId: postRestTicketsTicket
      x-api-path-slug: restticketsticketid-post
      parameters:
      - in: path
        name: ticketId
      responses:
        200:
          description: OK
      tags:
      - Message
    put:
      summary: Update a ticket
      description: Updates a ticket. The ID of the ticket must be specified.
      operationId: putRestTicketsTicket
      x-api-path-slug: restticketsticketid-put
      parameters:
      - in: path
        name: ticketId
      responses:
        200:
          description: OK
      tags:
      - Ticket
  /rest/user:
    get:
      summary: ""
      description: .
      operationId: getRestUser
      x-api-path-slug: restuser-get
      responses:
        200:
          description: OK
      tags:
      - ""
  /rest/user/authorized_user_with_ui_config:
    get:
      summary: Get authorized user with UiConfig
      description: Gets an authorized user with UiConfig. This call returns a JSON
        object with information about the user after login. This information is used
        for correctly displaying the plentymarkets back end.
      operationId: getRestUserAuthorizedUserWithUiConfig
      x-api-path-slug: restuserauthorized-user-with-ui-config-get
      responses:
        200:
          description: OK
      tags:
      - Authorized
      - User
      - UiConfig
  /rest/user/backend_pluginset:
    get:
      summary: get the backend plugin set for user
      description: Get the backend plugin set for user.
      operationId: getRestUserBackendPluginset
      x-api-path-slug: restuserbackend-pluginset-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Backend
      - Plugin
      - Setuser
    post:
      summary: set the backend plugin set for user
      description: Set the backend plugin set for user.
      operationId: postRestUserBackendPluginset
      x-api-path-slug: restuserbackend-pluginset-post
      responses:
        200:
          description: OK
      tags:
      - Set
      - Backend
      - Plugin
      - Setuser
  /rest/vat:
    get:
      summary: List VAT configurations.
      description: Lists the VAT configurations for the given filter. Possible filters
        are <code>locationId</code>, <code>countryId</code>, <code>taxIdNumber</code>
        and <code>startedAt</code>.
      operationId: getRestVat
      x-api-path-slug: restvat-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: query
        name: with
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - List
      - VAT
      - Configurations
    post:
      summary: Create a VAT configuration
      description: Create a vat configuration.
      operationId: postRestVat
      x-api-path-slug: restvat-post
      parameters:
      - in: body
        name: /rest/vat
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - VAT
      - Configuration
  /rest/vat/locations/{locationId}:
    get:
      summary: List VAT configurations of an accounting location
      description: Lists the VAT configurations for all countries of one accounting
        location
      operationId: getRestVatLocationsLocation
      x-api-path-slug: restvatlocationslocationid-get
      parameters:
      - in: query
        name: columns[]
        description: The attributes of the VAT configuration
      - in: path
        name: locationId
      - in: query
        name: with[]
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - List
      - VAT
      - Configurations
      - Of
      - Accounting
      - Location
  /rest/vat/locations/{locationId}/countries/{countryId}:
    get:
      summary: List VAT configurations for one country of delivery
      description: Lists the VAT configurations for a country of delivery of one accounting
        location. The ID of the accounting location and the ID of the country of delivery
        must be specified.
      operationId: getRestVatLocationsLocationCountriesCountry
      x-api-path-slug: restvatlocationslocationidcountriescountryid-get
      parameters:
      - in: query
        name: columns[]
        description: The attributes of the VAT configuration
      - in: path
        name: countryId
      - in: path
        name: locationId
      - in: query
        name: with[]
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - List
      - VAT
      - Configurationsone
      - Country
      - Of
      - Delivery
  /rest/vat/locations/{locationId}/countries/{countryId}/date/{date}:
    get:
      summary: Get a VAT configuration for a country in a location.
      description: Gets the VAT configuration found by matching the given location,
        delivery country and date of validity.
      operationId: getRestVatLocationsLocationCountriesCountryDateDate
      x-api-path-slug: restvatlocationslocationidcountriescountryiddatedate-get
      parameters:
      - in: query
        name: columns[]
        description: The attributes of the VAT configuration
      - in: path
        name: countryId
      - in: path
        name: date
      - in: path
        name: locationId
      - in: query
        name: startDate
        description: The date of validity
      - in: query
        name: with[]
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - VAT
      - Configurationa
      - Country
      - In
      - Location
  /rest/vat/standard:
    get:
      summary: Get a VAT configuration for the standard accounting location of a client
      description: Gets the VAT configuration currently used for the country of the
        standard accounting location of a client (store). The ID of the client (store)
        must be specified.
      operationId: getRestVatStandard
      x-api-path-slug: restvatstandard-get
      parameters:
      - in: query
        name: plentyId
        description: The plenty ID of the client (store)
      - in: query
        name: startedAt
        description: The date in the W3C format when the vat configuration went into
          effect
      responses:
        200:
          description: OK
      tags:
      - VAT
      - Configurationthe
      - Standard
      - Accounting
      - Location
      - Of
      - Client
  /rest/vat/{vatId}:
    get:
      summary: Get a VAT configuration by id
      description: Get a vat configuration by id.
      operationId: getRestVatVat
      x-api-path-slug: restvatvatid-get
      parameters:
      - in: path
        name: vatId
      responses:
        200:
          description: OK
      tags:
      - VAT
      - Configuration
      - By
      - Id
    put:
      summary: Update a VAT configuration
      description: Update a vat configuration.
      operationId: putRestVatVat
      x-api-path-slug: restvatvatid-put
      parameters:
      - in: body
        name: /rest/vat/{vatId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: vatId
      responses:
        200:
          description: OK
      tags:
      - VAT
      - Configuration
  /rest/warehouses/layouts:
    post:
      summary: Create a warehouse location layout
      description: Creates a warehouse location layout
      operationId: postRestWarehousesLayouts
      x-api-path-slug: restwarehouseslayouts-post
      parameters:
      - in: query
        name: dimensionId
        description: The warehouse location dimension ID of the warehouse location
          level
      - in: query
        name: isActiveForPickupPath
        description: Active flag for pickup path of the warehouse location dimension
      - in: query
        name: label
        description: The label of the warehouse location
      - in: query
        name: level
        description: The level of the warehouse location dimension
      - in: query
        name: levelId
        description: The warehouse location level ID of the warehouse location
      - in: query
        name: name
        description: The name of the warehouse location dimension
      - in: query
        name: parentId
        description: The parent ID of the warehouse location dimension
      - in: query
        name: position
        description: The position of the warehouse location level
      - in: query
        name: purposeKey
        description: The location type key of the warehouse location
      - in: query
        name: separator
        description: The separator of the warehouse location dimension
      - in: query
        name: shortcut
        description: The shortcut of the warehouse location dimension
      - in: query
        name: statusKey
        description: The location status key of the warehouse location
      - in: query
        name: warehouseId
        description: The warehouse ID of the warehouse location dimension
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
      - Layout
  /rest/warehouses/locations:
    delete:
      summary: Delete multiple warehouse locations
      description: Deletes multiple warehouse locations
      operationId: deleteRestWarehousesLocations
      x-api-path-slug: restwarehouseslocations-delete
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Warehouse
      - Locations
    post:
      summary: Create a warehouse location
      description: Creates a warehouse location.
      operationId: postRestWarehousesLocations
      x-api-path-slug: restwarehouseslocations-post
      parameters:
      - in: query
        name: label
        description: The label of the warehouse location
      - in: query
        name: levelId
        description: The warehouse location level ID of the warehouse location
      - in: query
        name: position
        description: The position of the warehouse location
      - in: query
        name: purposeKey
        description: The location type key of the warehouse location
      - in: query
        name: statusKey
        description: The location status key of the warehouse location
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
  /rest/warehouses/locations/details:
    get:
      summary: Get warehouse location details
      description: Gets warehouse location details
      operationId: getRestWarehousesLocationsDetails
      x-api-path-slug: restwarehouseslocationsdetails-get
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
      - Details
  /rest/warehouses/locations/dimensions:
    post:
      summary: Create a warehouse location dimension
      description: Creates a warehouse location dimension.
      operationId: postRestWarehousesLocationsDimensions
      x-api-path-slug: restwarehouseslocationsdimensions-post
      parameters:
      - in: query
        name: isActiveForPickupPath
        description: Active flag for pickup path of the warehouse location dimension
      - in: query
        name: level
        description: The level of the warehouse location dimension
      - in: query
        name: name
        description: The name of the warehouse location dimension
      - in: query
        name: parentId
        description: The parent ID of the warehouse location dimension
      - in: query
        name: separator
        description: The separator of the warehouse location dimension
      - in: query
        name: shortcut
        description: The shortcut of the warehouse location dimension
      - in: query
        name: warehouseId
        description: The warehouse ID of the warehouse location dimension
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
      - Dimension
  /rest/warehouses/locations/dimensions/{warehouseLocationDimensionId}:
    delete:
      summary: Delete a warehouse location dimension
      description: Deletes a warehouse location dimension
      operationId: deleteRestWarehousesLocationsDimensionsWarehouselocationdimension
      x-api-path-slug: restwarehouseslocationsdimensionswarehouselocationdimensionid-delete
      parameters:
      - in: path
        name: warehouseLocationDimensionId
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
      - Dimension
    get:
      summary: Get a warehouse location dimension
      description: Gets a warehouse location dimension by ID. The warehouse location
        ID is required.
      operationId: getRestWarehousesLocationsDimensionsWarehouselocationdimension
      x-api-path-slug: restwarehouseslocationsdimensionswarehouselocationdimensionid-get
      parameters:
      - in: path
        name: warehouseLocationDimensionId
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
      - Dimension
    put:
      summary: Update a warehouse location dimension
      description: Updates a warehouse location dimension
      operationId: putRestWarehousesLocationsDimensionsWarehouselocationdimension
      x-api-path-slug: restwarehouseslocationsdimensionswarehouselocationdimensionid-put
      parameters:
      - in: path
        name: warehouseLocationDimensionId
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
      - Dimension
  /rest/warehouses/locations/group:
    put:
      summary: Edit the purpose and status for a group of storage locations
      description: Edits the purpose and status for a group of storage locations by
        passing the group storage location ID (can be sent as mass assignment)
      operationId: putRestWarehousesLocationsGroup
      x-api-path-slug: restwarehouseslocationsgroup-put
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Purpose
      - Statusa
      - Group
      - Of
      - Storage
      - Locations
  /rest/warehouses/locations/levels:
    post:
      summary: Create a warehouse location level
      description: Creates a warehouse location level.
      operationId: postRestWarehousesLocationsLevels
      x-api-path-slug: restwarehouseslocationslevels-post
      parameters:
      - in: query
        name: dimensionId
        description: The warehouse location dimension ID of the warehouse location
          level
      - in: query
        name: name
        description: The name of the warehouse location level
      - in: query
        name: parentId
        description: The parent ID of the warehouse location level
      - in: query
        name: position
        description: The position of the warehouse location level
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
      - Level
  /rest/warehouses/locations/levels/{warehouseLocationLevelId}:
    delete:
      summary: Delete a warehouse location level
      description: Deletes a warehouse location level
      operationId: deleteRestWarehousesLocationsLevelsWarehouselocationlevel
      x-api-path-slug: restwarehouseslocationslevelswarehouselocationlevelid-delete
      parameters:
      - in: path
        name: warehouseLocationLevelId
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
      - Level
    get:
      summary: Get a warehouse location level
      description: Gets a warehouse location level by ID. The warehouse location ID
        is required.
      operationId: getRestWarehousesLocationsLevelsWarehouselocationlevel
      x-api-path-slug: restwarehouseslocationslevelswarehouselocationlevelid-get
      parameters:
      - in: path
        name: warehouseLocationLevelId
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
      - Level
    put:
      summary: Update a warehouse location level
      description: Updates a warehouse location level
      operationId: putRestWarehousesLocationsLevelsWarehouselocationlevel
      x-api-path-slug: restwarehouseslocationslevelswarehouselocationlevelid-put
      parameters:
      - in: path
        name: warehouseLocationLevelId
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
      - Level
  /rest/warehouses/locations/multiple_dimensions:
    post:
      summary: Create multiple warehouse location dimensions
      description: Creates multiple warehouse location dimension.
      operationId: postRestWarehousesLocationsMultipleDimensions
      x-api-path-slug: restwarehouseslocationsmultiple-dimensions-post
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Warehouse
      - Location
      - Dimensions
  /rest/warehouses/locations/previews:
    post:
      summary: Generate warehouse location preview and saves it
      description: Generates warehouse location preview and saves it
      operationId: postRestWarehousesLocationsPreviews
      x-api-path-slug: restwarehouseslocationspreviews-post
      responses:
        200:
          description: OK
      tags:
      - Generate
      - Warehouse
      - Location
      - Preview
      - Saves
      - It
  /rest/warehouses/locations/{warehouseId}/label:
    get:
      summary: Generate the warehouse location label
      description: Generates the warehouse location label
      operationId: getRestWarehousesLocationsWarehouseLabel
      x-api-path-slug: restwarehouseslocationswarehouseidlabel-get
      parameters:
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - Generate
      - Warehouse
      - Location
      - Label
  /rest/warehouses/locations/{warehouseLocationId}:
    delete:
      summary: Delete a warehouse location
      description: Deletes a warehouse location
      operationId: deleteRestWarehousesLocationsWarehouselocation
      x-api-path-slug: restwarehouseslocationswarehouselocationid-delete
      parameters:
      - in: path
        name: warehouseLocationId
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
    get:
      summary: Get a warehouse location
      description: Gets a warehouse location by ID. The warehouse location ID is required.
      operationId: getRestWarehousesLocationsWarehouselocation
      x-api-path-slug: restwarehouseslocationswarehouselocationid-get
      parameters:
      - in: path
        name: warehouseLocationId
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
    put:
      summary: Update a warehouse location
      description: Updates a warehouse location
      operationId: putRestWarehousesLocationsWarehouselocation
      x-api-path-slug: restwarehouseslocationswarehouselocationid-put
      parameters:
      - in: path
        name: warehouseLocationId
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
  /rest/warehouses/structure/{warehouseId}:
    get:
      summary: Get a warehouse location structure
      description: Gets a warehouse location structure by warehouse ID. The warehouse
        ID is required.
      operationId: getRestWarehousesStructureWarehouse
      x-api-path-slug: restwarehousesstructurewarehouseid-get
      parameters:
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - Warehouse
      - Location
      - Structure
  /rest/warehouses/{warehouseId}/locations:
    get:
      summary: List warehouse locations
      description: Lists all warehouse locations.
      operationId: getRestWarehousesWarehouseLocations
      x-api-path-slug: restwarehouseswarehouseidlocations-get
      parameters:
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - List
      - Warehouse
      - Locations
  /rest/warehouses/{warehouseId}/locations/dimensions:
    get:
      summary: List warehouse location dimensions
      description: Lists all warehouse location dimensions.
      operationId: getRestWarehousesWarehouseLocationsDimensions
      x-api-path-slug: restwarehouseswarehouseidlocationsdimensions-get
      parameters:
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - List
      - Warehouse
      - Location
      - Dimensions
  /rest/warehouses/{warehouseId}/locations/levels:
    get:
      summary: List warehouse location levels
      description: Lists all warehouse location levels.
      operationId: getRestWarehousesWarehouseLocationsLevels
      x-api-path-slug: restwarehouseswarehouseidlocationslevels-get
      parameters:
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - List
      - Warehouse
      - Location
      - Levels
  /rest/webstores:
    get:
      summary: List clients (stores)
      description: List clients (stores).
      operationId: getRestWebstores
      x-api-path-slug: restwebstores-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Clients
      - (stores)
  /rest/webstores/{webstoreId}/plugin_set:
    get:
      summary: ""
      description: .
      operationId: getRestWebstoresWebstorePluginSet
      x-api-path-slug: restwebstoreswebstoreidplugin-set-get
      parameters:
      - in: path
        name: webstoreId
      responses:
        200:
          description: OK
      tags:
      - ""
    post:
      summary: ""
      description: .
      operationId: postRestWebstoresWebstorePluginSet
      x-api-path-slug: restwebstoreswebstoreidplugin-set-post
      parameters:
      - in: path
        name: webstoreId
      responses:
        200:
          description: OK
      tags:
      - ""