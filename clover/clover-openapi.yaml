swagger: "2.0"
x-collection-name: Clover
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}:
    get:
      summary: Get a single merchant
      description: Get a single merchant.
      operationId: GetMerchant
      x-api-path-slug: v3merchantsmid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [employees, bankProcessing, externalMerchant,
          merchantBoarding, deviceBoarding, programExpress, hierarchy, shifts, orders,
          address, logos, owner, items, tags, tenders, payments, gateway, printers,
          modifierGroups, properties, tipSuggestions, openingHours, partnerApp, selfBoardingApplication]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - MId
    post:
      summary: Update a merchant
      description: Update a merchant.
      operationId: UpdateMerchant
      x-api-path-slug: v3merchantsmid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [employees, bankProcessing, externalMerchant,
          merchantBoarding, deviceBoarding, programExpress, hierarchy, shifts, orders,
          address, logos, owner, items, tags, tenders, payments, gateway, printers,
          modifierGroups, properties, tipSuggestions, openingHours, partnerApp, selfBoardingApplication]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - MId
  /v3/merchants/{mId}/address:
    get:
      summary: Get a merchant's address
      description: Get a merchant's address.
      operationId: GetMerchantAddress
      x-api-path-slug: v3merchantsmidaddress-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Address
  /v3/merchants/{mId}/gateway:
    get:
      summary: Get a merchant's payment gateway configuration
      description: Get a merchant's payment gateway configuration.
      operationId: GetMerchantGateway
      x-api-path-slug: v3merchantsmidgateway-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Gateway
  /v3/merchants/{mId}/properties:
    get:
      summary: Get a merchant's properties
      description: Get a merchant's properties.
      operationId: GetMerchantProperties
      x-api-path-slug: v3merchantsmidproperties-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Properties
    post:
      summary: Update merchant properties
      description: Update merchant properties.
      operationId: UpdateMerchantProperties
      x-api-path-slug: v3merchantsmidproperties-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Properties
  /v3/merchants/{mId}/default_service_charge:
    get:
      summary: Get default service charge for a merchant
      description: The Merchant's default service charge, set via the Setup App (https://www.clover.com/setupapp).
      operationId: GetDefaultServiceCharge
      x-api-path-slug: v3merchantsmiddefault-service-charge-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Default
      - Service
      - Charge
  /v3/merchants/{mId}/sync/{table}:
    get:
      summary: Get a sync token (deprecated)
      description: Get a sync token (deprecated).
      operationId: GetSyncToken
      x-api-path-slug: v3merchantsmidsynctable-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: table
        description: Table Name
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Sync
      - Table
  /v3/merchants/{mId}/tip_suggestions:
    get:
      summary: Get all tip suggestions for a merchant
      description: Get all tip suggestions for a merchant.
      operationId: GetTipSuggestions
      x-api-path-slug: v3merchantsmidtip-suggestions-get
      parameters:
      - in: query
        name: filter
        description: 'Filter fields: [id, name, percentage, enabled]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tip
      - Suggestions
  /v3/merchants/{mId}/tip_suggestions/{tId}:
    get:
      summary: Get a single tip suggestion
      description: Get a single tip suggestion.
      operationId: GetTipSuggestion
      x-api-path-slug: v3merchantsmidtip-suggestionstid-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: tId
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tip
      - Suggestions
      - TId
    post:
      summary: Update a single tip suggestion
      description: Update a single tip suggestion.
      operationId: UpdateTipSuggestion
      x-api-path-slug: v3merchantsmidtip-suggestionstid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: tId
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tip
      - Suggestions
      - TId
  /v3/merchants/{mId}/order_types:
    get:
      summary: Get all order types for a merchant
      description: Merchants have the ability to create custom order types via the
        Setup App (https://www.clover.com/setupapp). These custom order types can
        be associated with a System Order Type (see /v3/merchants/{mId}/system_order_types).
        Custom Order Types can support items in all categories (filterCategories=false)
        or a subset of the merchant's categories (filterCategories=true and categories
        property contains the list of supported categories). Note that when expanding
        the categories for an order type, they will only be returned if this orderType
        only supports a subset of the categories (filterCategories=true). If the orderType
        supports all categories (filterCategories=false) then you should make a GET
        request to /v3/merchants/{mId}/categories.
      operationId: GetOrderTypes
      x-api-path-slug: v3merchantsmidorder-types-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [hours, attributes, categories]'
      - in: query
        name: filter
        description: 'Filter fields: [id, deletedTime]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Order
      - Types
    post:
      summary: Create Order Type For Merchant
      description: Create order type for merchant.
      operationId: CreateOrderType
      x-api-path-slug: v3merchantsmidorder-types-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [hours, attributes, categories]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Order
      - Types
  /v3/merchants/{mId}/order_types/{orderTypeId}:
    get:
      summary: Get a single order type
      description: Get a single order type.
      operationId: GetOrderType
      x-api-path-slug: v3merchantsmidorder-typesordertypeid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [hours, attributes, categories]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderTypeId
        description: Order Type Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Order
      - Types
      - OrderTypeId
    post:
      summary: Update a single order type
      description: Update a single order type.
      operationId: UpdateOrderType
      x-api-path-slug: v3merchantsmidorder-typesordertypeid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [hours, attributes, categories]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderTypeId
        description: Order Type Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Order
      - Types
      - OrderTypeId
    delete:
      summary: Delete an order type
      description: Delete an order type.
      operationId: DeleteOrderType
      x-api-path-slug: v3merchantsmidorder-typesordertypeid-delete
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderTypeId
        description: Order Type Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Order
      - Types
      - OrderTypeId
  /v3/merchants/{mId}/order_type_categories:
    post:
      summary: Create or delete a order type category
      description: Create or delete a order type category.
      operationId: CreateOrDeleteOrderTypeCategories
      x-api-path-slug: v3merchantsmidorder-type-categories-post
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Order
      - Type
      - Categories
  /v3/merchants/{mId}/system_order_types:
    get:
      summary: Return a list of system order types
      description: Merchants can create custom Order Types via "/v3/merchants/{mId}/order_types".
        It is useful to associate these custom order types with particular system
        order types in order to group things functionally. For example, a merchant
        may have a "Lunch Take-Out" order type and a "Dinner Take-Out" order type.
        These two order types can be associated with the "TAKE-OUT-TYPE" system order
        type so that applications can understand that they are both take-out order
        types.
      operationId: GetSystemOrderTypes
      x-api-path-slug: v3merchantsmidsystem-order-types-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - System
      - Order
      - Types
  /v3/merchants/{mId}/roles:
    get:
      summary: Get all roles from a merchant
      description: Get all roles from a merchant.
      operationId: GetRoles
      x-api-path-slug: v3merchantsmidroles-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [employees]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, systemRole, name, id, deletedTime]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Roles
    post:
      summary: Create a role
      description: Create a role.
      operationId: CreateRole
      x-api-path-slug: v3merchantsmidroles-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Roles
  /v3/merchants/{mId}/roles/{rId}:
    get:
      summary: Get a single role
      description: Get a single role.
      operationId: GetRole
      x-api-path-slug: v3merchantsmidrolesrid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [employees]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: rId
        description: Role Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Roles
      - RId
    post:
      summary: Update a single role
      description: Update a single role.
      operationId: UpdateRole
      x-api-path-slug: v3merchantsmidrolesrid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [employees]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: rId
        description: Role Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Roles
      - RId
    delete:
      summary: Delete a role
      description: Delete a role.
      operationId: DeleteRole
      x-api-path-slug: v3merchantsmidrolesrid-delete
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: rId
        description: Role Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Roles
      - RId
  /v3/merchants/{mId}/tenders:
    get:
      summary: Get all tenders for a merchant
      description: Get all tenders for a merchant.
      operationId: GetMerchantTenders
      x-api-path-slug: v3merchantsmidtenders-get
      parameters:
      - in: query
        name: filter
        description: 'Filter fields: [labelKey, label, opensCashDrawer, enabled, visible,
          instruction, id, merchantId, systemTenderId, deletedTime, modifiedTime]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tenders
    post:
      summary: Adds a new tender
      description: Returns an object representing newly added merchant tender, with
        a generated ID.
      operationId: CreateMerchantTender
      x-api-path-slug: v3merchantsmidtenders-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tenders
  /v3/merchants/{mId}/tenders/{tenderId}:
    get:
      summary: Get a single merchant tender
      description: Get a single merchant tender.
      operationId: GetMerchantTender
      x-api-path-slug: v3merchantsmidtenderstenderid-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: tenderId
        description: Tender Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tenders
      - TenderId
    post:
      summary: Updates an existing tender
      description: Returns an object representing updated merchant tender.
      operationId: UpdateMerchantTender
      x-api-path-slug: v3merchantsmidtenderstenderid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: tenderId
        description: Tender Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tenders
      - TenderId
    delete:
      summary: Deletes an existing tender
      description: Deletes an existing tender.
      operationId: DeleteMerchantTender
      x-api-path-slug: v3merchantsmidtenderstenderid-delete
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: tenderId
        description: Tender Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tenders
      - TenderId
  /v3/merchants/{mId}/opening_hours:
    get:
      summary: Get a list this merchant opening hours
      description: Get a list this merchant opening hours.
      operationId: GetAllMerchantOpeningHours
      x-api-path-slug: v3merchantsmidopening-hours-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Opening
      - Hours
    post:
      summary: Create a set of merchant opening hours
      description: Create a set of merchant opening hours.
      operationId: CreateMerchantOpeningHours
      x-api-path-slug: v3merchantsmidopening-hours-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Opening
      - Hours
  /v3/merchants/{mId}/opening_hours/{hId}:
    get:
      summary: Get a specific set of merchant opening hours
      description: Get a specific set of merchant opening hours.
      operationId: GetMerchantOpeningHours
      x-api-path-slug: v3merchantsmidopening-hourshid-get
      parameters:
      - in: path
        name: hId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Opening
      - Hours
      - HId
    post:
      summary: Update a set of merchant opening hours
      description: Update a set of merchant opening hours.
      operationId: UpdateMerchantOpeningHours
      x-api-path-slug: v3merchantsmidopening-hourshid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: hId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Opening
      - Hours
      - HId
    delete:
      summary: Delete a set of merchant opening hours
      description: Delete a set of merchant opening hours.
      operationId: DeleteMerchantOpeningHours
      x-api-path-slug: v3merchantsmidopening-hourshid-delete
      parameters:
      - in: path
        name: hId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Opening
      - Hours
      - HId
  /v3/merchants/{mId}/devices:
    get:
      summary: Get all devices provisioned to a merchant
      description: Returns a list of all devices that are provisioned to the a merchant.
        This list can be viewed from the Setup App on the merchant's device or web
        dashboard (https://www.clover.com/setupapp/m/{mId}/devices).
      operationId: GetMerchantDevices
      x-api-path-slug: v3merchantsmiddevices-get
      parameters:
      - in: query
        name: filter
        description: 'Filter fields: [id, model, name, orderPrefix, serial, deleted_time,
          merchant'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Devices
  /v3/merchants/{mId}/devices/{deviceId}:
    get:
      summary: Get a single device provisioned to a merchant
      description: Returns a single device that is provisioned to a merchant.
      operationId: GetMerchantDevice
      x-api-path-slug: v3merchantsmiddevicesdeviceid-get
      parameters:
      - in: path
        name: deviceId
        description: Device Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Devices
      - DeviceId
  /v3/merchants/{mId}/cash_events:
    get:
      summary: Get all cash events
      description: Retrieve all cash events for this merchant. Cash events can also
        be consumed by registering a Webhook callback. See https://docs.clover.com/build/webhooks/
      operationId: GetAllCashEvents
      x-api-path-slug: v3merchantsmidcash-events-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [employee, device]'
      - in: query
        name: filter
        description: 'Filter fields: [employee'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Cash
      - Events
  /v3/merchants/{mId}/employees/{empId}/cash_events:
    get:
      summary: Get all cash events for an employee
      description: Retrieve cash events filtered by employee ID. Cash events can also
        be consumed by registering a Webhook callback. See https://docs.clover.com/build/webhooks/
      operationId: GetEmployeeCashEvents
      x-api-path-slug: v3merchantsmidemployeesempidcash-events-get
      parameters:
      - in: path
        name: empId
        description: Employee Id
      - in: query
        name: expand
        description: 'Expandable fields: [employee, device]'
      - in: query
        name: filter
        description: 'Filter fields: [employee'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employees
      - EmpId
      - Cash
      - Events
  /v3/merchants/{mId}/devices/{deviceId}/cash_events:
    get:
      summary: Get all cash events for a device
      description: Retrieve cash events filtered by device ID. Cash events can also
        be consumed by registering a Webhook callback. See https://docs.clover.com/build/webhooks/
      operationId: GetDeviceCashEvents
      x-api-path-slug: v3merchantsmiddevicesdeviceidcash-events-get
      parameters:
      - in: path
        name: deviceId
        description: Device Id
      - in: query
        name: expand
        description: 'Expandable fields: [employee, device]'
      - in: query
        name: filter
        description: 'Filter fields: [employee'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Devices
      - DeviceId
      - Cash
      - Events
  /v3/merchants/{mId}/customers.csv:
    get:
      summary: Get a list of customers
      description: Gives information for every customer of a merchant by default.
      operationId: DelegatedGetCustomers
      x-api-path-slug: v3merchantsmidcustomers-csv-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [addresses, emailAddresses, phoneNumbers,
          cards, metadata]'
      - in: query
        name: filter
        description: 'Filter fields: [id, firstName, lastName, fullName, customerSince,
          marketingAllowed, deletedTime, phoneNumber, emailAddress]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - Csv
  /v3/merchants/{mId}/customers:
    get:
      summary: Get a list of customers
      description: Gives information for every customer of a merchant by default.
      operationId: DelegatedGetCustomers
      x-api-path-slug: v3merchantsmidcustomers-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [addresses, emailAddresses, phoneNumbers,
          cards, metadata]'
      - in: query
        name: filter
        description: 'Filter fields: [id, firstName, lastName, fullName, customerSince,
          marketingAllowed, deletedTime, phoneNumber, emailAddress]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
    post:
      summary: Create a customer
      description: Creates an customer for a merchant.
      operationId: DelegatedCreateCustomer
      x-api-path-slug: v3merchantsmidcustomers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [addresses, emailAddresses, phoneNumbers,
          cards, metadata]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
  /v3/merchants/{mId}/customers/{customerId}:
    get:
      summary: Get a single customer
      description: Returns information for a single customer.
      operationId: DelegatedGetCustomer
      x-api-path-slug: v3merchantsmidcustomerscustomerid-get
      parameters:
      - in: path
        name: customerId
      - in: query
        name: expand
        description: 'Expandable fields: [addresses, emailAddresses, phoneNumbers,
          cards, metadata]'
      - in: query
        name: filter
        description: 'Filter fields: [id, firstName, lastName, fullName, customerSince,
          marketingAllowed, deletedTime, phoneNumber, emailAddress]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
    post:
      summary: Update a customer
      description: Updates information for a single customer. Only specified fields
        are overwritten.
      operationId: DelegatedUpdateCustomer
      x-api-path-slug: v3merchantsmidcustomerscustomerid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: query
        name: expand
        description: 'Expandable fields: [addresses, emailAddresses, phoneNumbers,
          cards, metadata]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
    delete:
      summary: Delete a customer
      description: Deletes a single customer from a merchant.
      operationId: DelegatedDeleteCustomer
      x-api-path-slug: v3merchantsmidcustomerscustomerid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
  /v3/merchants/{mId}/employees:
    get:
      summary: Get all employees
      description: Gives information for every employee associated to a merchant by
        default. Accepts optional filter and expand query parameters.
      operationId: GetEmployees
      x-api-path-slug: v3merchantsmidemployees-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [roles, shifts]'
      - in: query
        name: filter
        description: 'Filter fields: [id, name, email, role, customId, role'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employees
    post:
      summary: Create an employee
      description: Creates an employee for a merchant. Accepts optional expand parameters.
      operationId: CreateEmployee
      x-api-path-slug: v3merchantsmidemployees-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [shifts, payments, orders, roles]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employees
  /v3/merchants/{mId}/customers/{customerId}/phone_numbers:
    post:
      summary: Create a phone number for a customer
      description: Creates a phone number associated to a merchant's customer.
      operationId: DelegatedCreateCustomerPhoneNumber
      x-api-path-slug: v3merchantsmidcustomerscustomeridphone-numbers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Phone
      - Numbers
  /v3/merchants/{mId}/employees/{empId}:
    get:
      summary: Get a single employee
      description: Returns information for a single employee.  Accepts optional expand
        query parameters
      operationId: GetEmployee
      x-api-path-slug: v3merchantsmidemployeesempid-get
      parameters:
      - in: path
        name: empId
        description: Employee Id
      - in: query
        name: expand
        description: 'Expandable fields: [roles, shifts]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employees
      - EmpId
    post:
      summary: Update an employee
      description: Updates information for a single employee. Accepts optional expand
        query params.
      operationId: UpdateEmployee
      x-api-path-slug: v3merchantsmidemployeesempid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: empId
        description: Employee Id
      - in: query
        name: expand
        description: 'Expandable fields: [shifts, payments, orders, roles]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employees
      - EmpId
    delete:
      summary: Delete an employee
      description: Deletes a single employee from a merchant. Third party developers
        cannot delete the 'owner' employee.
      operationId: DeleteEmployee
      x-api-path-slug: v3merchantsmidemployeesempid-delete
      parameters:
      - in: path
        name: empId
        description: Employee Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employees
      - EmpId
  /v3/merchants/{mId}/customers/{customerId}/phone_numbers/{phoneId}:
    post:
      summary: Update a phone number for a customer
      description: Updates a merchant's customer's phone number.
      operationId: DelegatedUpdateCustomerPhoneNumber
      x-api-path-slug: v3merchantsmidcustomerscustomeridphone-numbersphoneid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: phoneId
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Phone
      - Numbers
      - PhoneId
    delete:
      summary: Delete a customer phone number
      description: Deletes a merchant's customer's phone number.
      operationId: DelegatedDeleteCustomerPhoneNumber
      x-api-path-slug: v3merchantsmidcustomerscustomeridphone-numbersphoneid-delete
      parameters:
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: phoneId
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Phone
      - Numbers
      - PhoneId
  /v3/merchants/{mId}/items:
    get:
      summary: Get all inventory items
      description: Get all inventory items.
      operationId: GetItems
      x-api-path-slug: v3merchantsmiditems-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [tags, categories, taxRates, modifierGroups,
          itemStock, options]'
      - in: query
        name: filter
        description: 'Filter fields: [id, name, sku, modifiedTime, deleted, hidden,
          price, alternateName, itemCode, item'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
    post:
      summary: Create an inventory item
      description: Create an inventory item.
      operationId: CreateItem
      x-api-path-slug: v3merchantsmiditems-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [tags, categories, taxRates, modifierGroups,
          itemStock, options]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
    delete:
      summary: Bulk delete inventory items
      description: Bulk delete inventory items.
      operationId: BulkDeleteItems
      x-api-path-slug: v3merchantsmiditems-delete
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
  /v3/merchants/{mId}/customers/{customerId}/email_addresses:
    post:
      summary: Create an email address for a customer
      description: Creates an email address associated to a merchant's customer.
      operationId: DelegatedCreateCustomerEmailAddress
      x-api-path-slug: v3merchantsmidcustomerscustomeridemail-addresses-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Email
      - Addresses
  /v3/merchants/{mId}/shifts:
    get:
      summary: Get all shifts
      description: Get all shifts.
      operationId: GetAllShifts
      x-api-path-slug: v3merchantsmidshifts-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [employee, overrideInEmployee, overrideOutEmployee]'
      - in: query
        name: filter
        description: 'Filter fields: [id, employee'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Shifts
  /v3/merchants/{mId}/customers/{customerId}/email_addresses/{emailId}:
    post:
      summary: Update an email address for a customer
      description: Updates a merchant's customer's email address.
      operationId: DelegatedUpdateCustomerEmailAddress
      x-api-path-slug: v3merchantsmidcustomerscustomeridemail-addressesemailid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: emailId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Email
      - Addresses
      - EmailId
    delete:
      summary: Delete a customer email address
      description: Deletes a merchant's customer's email address.
      operationId: DelegatedDeleteCustomerEmailAddress
      x-api-path-slug: v3merchantsmidcustomerscustomeridemail-addressesemailid-delete
      parameters:
      - in: path
        name: customerId
      - in: path
        name: emailId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Email
      - Addresses
      - EmailId
  /v3/merchants/{mId}/shifts/{shiftId}:
    get:
      summary: Get a single shift
      description: Get a single shift.
      operationId: GetShift
      x-api-path-slug: v3merchantsmidshiftsshiftid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [employee, overrideInEmployee, overrideOutEmployee]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: shiftId
        description: Employee Shift Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Shifts
      - ShiftId
  /v3/merchants/{mId}/items/{itemId}:
    get:
      summary: Get a single inventory item
      description: Get a single inventory item.
      operationId: GetItem
      x-api-path-slug: v3merchantsmiditemsitemid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [tags, categories, taxRates, modifierGroups,
          itemStock, options]'
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
      - ItemId
    post:
      summary: Update an existing inventory item
      description: Update an existing inventory item.
      operationId: UpdateItem
      x-api-path-slug: v3merchantsmiditemsitemid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [tags, categories, taxRates, modifierGroups,
          itemStock, options]'
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
      - ItemId
    delete:
      summary: Delete an inventory item
      description: Delete an inventory item.
      operationId: DeleteItem
      x-api-path-slug: v3merchantsmiditemsitemid-delete
      parameters:
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
      - ItemId
  /v3/merchants/{mId}/shifts.csv:
    get:
      summary: Get .csv of all shifts
      description: Get .csv of all shifts.
      operationId: GetAllShiftsCSV
      x-api-path-slug: v3merchantsmidshifts-csv-get
      parameters:
      - in: query
        name: filter
        description: 'Filter fields: [id, employee'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Shifts
      - Csv
  /v3/apps/{aId}/merchants/{mId}/notifications:
    post:
      summary: Create a notification for an app
      description: 'Push a message to all merchant devices that have your app installed
        and are listening for notifications.  For details on how to use Clover''s
        Android SDK to receive notifications see: https://github.com/clover/android-examples/tree/master/pushnotificationexample'
      operationId: CreateMerchantAppNotification
      x-api-path-slug: v3appsaidmerchantsmidnotifications-post
      parameters:
      - in: path
        name: aId
        description: App Id
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Apps
      - Merchants
      - Notifications
  /v3/merchants/{mId}/employees/{empId}/shifts:
    get:
      summary: Get all shifts for an employee
      description: Get all shifts for an employee.
      operationId: GetEmployeeShifts
      x-api-path-slug: v3merchantsmidemployeesempidshifts-get
      parameters:
      - in: path
        name: empId
        description: Employee Id
      - in: query
        name: expand
        description: 'Expandable fields: [employee, overrideInEmployee, overrideOutEmployee]'
      - in: query
        name: filter
        description: 'Filter fields: [id, employee'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employees
      - EmpId
      - Shifts
    post:
      summary: Create shift for an employee
      description: Create shift for an employee.
      operationId: CreateShift
      x-api-path-slug: v3merchantsmidemployeesempidshifts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: empId
        description: Employee Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employees
      - EmpId
      - Shifts
  /v3/merchants/{mId}/customers/{customerId}/addresses:
    post:
      summary: Create an address for a customer
      description: Creates an address associated to a merchant's customer.
      operationId: DelegatedCreateCustomerAddress
      x-api-path-slug: v3merchantsmidcustomerscustomeridaddresses-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Addresses
  /v3/apps/{aId}/devices/{dId}/notifications:
    post:
      summary: Create a notification for a device
      description: 'Push a message to a device that has your app installed and is
        listening for notifications.  For details on how to use Clover''s Android
        SDK to receive notifications see: https://github.com/clover/android-examples/tree/master/pushnotificationexample'
      operationId: CreateDeviceAppNotification
      x-api-path-slug: v3appsaiddevicesdidnotifications-post
      parameters:
      - in: path
        name: aId
        description: App Id
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: dId
        description: Developer Id
      responses:
        200:
          description: OK
      tags:
      - Apps
      - Devices
      - DId
      - Notifications
  /v3/merchants/{mId}/customers/{customerId}/addresses/{addressId}:
    post:
      summary: Update an address for a customer
      description: Updates a merchant's customer's address.
      operationId: DelegatedUpdateCustomerAddress
      x-api-path-slug: v3merchantsmidcustomerscustomeridaddressesaddressid-post
      parameters:
      - in: path
        name: addressId
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Addresses
      - AddressId
    delete:
      summary: Delete a customer address
      description: Deletes a merchant's customer's address.
      operationId: DelegatedDeleteCustomerAddress
      x-api-path-slug: v3merchantsmidcustomerscustomeridaddressesaddressid-delete
      parameters:
      - in: path
        name: addressId
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Addresses
      - AddressId
  /v3/merchants/{mId}/bulk_items:
    post:
      summary: Create multiple inventory items.
      description: This API is to create multiple inventory items.  Use the PATCH
        HTTP method to update existing inventory items.
      operationId: BulkCreateInventoryItems
      x-api-path-slug: v3merchantsmidbulk-items-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Bulk
      - Items
    put:
      summary: Update existing inventory items.
      description: This API is to going to update only the changes present in the
        payload. Not going to replace the existing inventory items. Use the POST HTTP
        method to create inventory items.
      operationId: BulkPatchInventoryItems
      x-api-path-slug: v3merchantsmidbulk-items-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Bulk
      - Items
  /v3/merchants/{mId}/employees/{empId}/shifts/{shiftId}:
    get:
      summary: Get a single shift
      description: Get a single shift.
      operationId: GetEmployeeShift
      x-api-path-slug: v3merchantsmidemployeesempidshiftsshiftid-get
      parameters:
      - in: path
        name: empId
        description: Employee Id
      - in: query
        name: expand
        description: 'Expandable fields: [employee, overrideInEmployee, overrideOutEmployee]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: shiftId
        description: Employee Shift Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employees
      - EmpId
      - Shifts
      - ShiftId
    post:
      summary: Update a single shift
      description: Update a single shift.
      operationId: UpdateShift
      x-api-path-slug: v3merchantsmidemployeesempidshiftsshiftid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: empId
        description: Employee Id
      - in: query
        name: expand
        description: 'Expandable fields: [employee, overrideInEmployee, overrideOutEmployee]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: shiftId
        description: Employee Shift Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employees
      - EmpId
      - Shifts
      - ShiftId
    delete:
      summary: Delete a single shift
      description: Delete a single shift.
      operationId: DeleteShift
      x-api-path-slug: v3merchantsmidemployeesempidshiftsshiftid-delete
      parameters:
      - in: path
        name: empId
        description: Employee Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: shiftId
        description: Employee Shift Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employees
      - EmpId
      - Shifts
      - ShiftId
  /v3/merchants/{mId}/item_stocks:
    get:
      summary: Get the stock of all inventory items
      description: Get the stock of all inventory items.
      operationId: GetItemStocks
      x-api-path-slug: v3merchantsmiditem-stocks-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Stocks
  /v3/merchants/{mId}/customers/{customerId}/cards:
    post:
      summary: Create a credit/debit card entry for a customer
      description: Create a credit/debit card entry for a customer.
      operationId: DelegatedCreateCustomerCard
      x-api-path-slug: v3merchantsmidcustomerscustomeridcards-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Cards
  /v3/merchants/{mId}/item_stocks/{itemId}:
    get:
      summary: Get the stock of an inventory item
      description: Get the stock of an inventory item.
      operationId: GetItemStock
      x-api-path-slug: v3merchantsmiditem-stocksitemid-get
      parameters:
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Stocks
      - ItemId
    post:
      summary: Update the stock of an inventory item
      description: Update the stock of an inventory item.
      operationId: UpdateItemStock
      x-api-path-slug: v3merchantsmiditem-stocksitemid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Stocks
      - ItemId
    delete:
      summary: Delete the stock of an inventory item
      description: Delete the stock of an inventory item.
      operationId: DeleteItemStock
      x-api-path-slug: v3merchantsmiditem-stocksitemid-delete
      parameters:
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Stocks
      - ItemId
  /v3/merchants/{mId}/customers/{customerId}/cards/{cardId}:
    post:
      summary: Update a credit/debit card record for a customer
      description: Update a credit/debit card record for a customer.
      operationId: DelegatedUpdateCustomerCard
      x-api-path-slug: v3merchantsmidcustomerscustomeridcardscardid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: cardId
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Cards
      - CardId
    delete:
      summary: Delete a customer card
      description: Delete a customer card.
      operationId: DelegatedDeleteCustomerCard
      x-api-path-slug: v3merchantsmidcustomerscustomeridcardscardid-delete
      parameters:
      - in: path
        name: cardId
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Cards
      - CardId
  /v3/merchants/{mId}/orders:
    get:
      summary: Gets a list of orders
      description: Returns a list of orders. See https://docs.clover.com/build/working-with-orders/
        for more details.
      operationId: GetOrders
      x-api-path-slug: v3merchantsmidorders-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [lineItems, serviceCharge, discounts, credits,
          payments, refunds]'
      - in: query
        name: filter
        description: 'Filter fields: [employee'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
    post:
      summary: Create an order
      description: Only supports basic order creation. Valid fields are limited to
        taxRemoved, note, title, and orderType. Adding line items must be done in
        separate calls.
      operationId: CreateOrder
      x-api-path-slug: v3merchantsmidorders-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
  /v3/merchants/{mId}/item_groups:
    get:
      summary: Get all item groups
      description: |-
        Item Groups help merchants create and manage large groups of related items. This is described to merchants as an 'Item with variants'.

        For example a merchants may sell a t-shirt that is available in numerous various sizes and colors. Each of the t-shirt variations is an item and belongs to the t-shirt item group. Once an item group is created it appears in Register as a single button and tapping it brings up a choice of which variation is to be sold. Before adding items to an item group you first need to create the item group, then create attributes ('size', 'color') and then options for each attribute ('small', 'blue'), then associate options with an item and then associate items with an item group.

        The name of an item which is a member of an item group is automatically generated by the Clover server as a combination of the item group name and the name of all the options associated with that item. It cannot be changed. If the item group name is changed, or if an option name is changed, then the item names will be automatically regenerated.

        An item can only be a member of a single item group and once it is part of an item group it can never be removed or moved to another item group, it can only be deleted.
      operationId: GetItemGroups
      x-api-path-slug: v3merchantsmiditem-groups-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items, attributes]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, name, id, deletedTime]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Groups
    post:
      summary: Create an item group
      description: Create an item group.
      operationId: CreateItemGroup
      x-api-path-slug: v3merchantsmiditem-groups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [items, attributes]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Groups
  /v3/merchants/{mId}/employees/{empId}/orders:
    get:
      summary: Get all orders for an employee
      description: Get all orders for an employee.
      operationId: GetEmployeeOrders
      x-api-path-slug: v3merchantsmidemployeesempidorders-get
      parameters:
      - in: path
        name: empId
        description: Employee Id
      - in: query
        name: expand
        description: 'Expandable fields: [lineItems, customers, payments, credits,
          refunds, serviceCharge, discounts]'
      - in: query
        name: filter
        description: 'Filter fields: [lineItems, customers, payments, credits, refunds,
          serviceCharge, discounts]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employees
      - EmpId
      - Orders
  /v3/merchants/{mId}/customers/{customerId}/metadata:
    post:
      summary: Create note, birthday, business name for a customer
      description: Creates note, birthday, business name associated to a merchant's
        customer.
      operationId: DelegatedCreateOrUpdateCustomerMetadata
      x-api-path-slug: v3merchantsmidcustomerscustomeridmetadata-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - CustomerId
      - Metadata
  /v3/merchants/{mId}/orders/{orderId}:
    get:
      summary: Get a single order
      description: Returns a single order. See https://docs.clover.com/build/working-with-orders/
        for more details.
      operationId: GetOrder
      x-api-path-slug: v3merchantsmidordersorderid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [lineItems, customers, payments, credits,
          refunds, serviceCharge, discounts]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
    post:
      summary: Update an order
      description: Update an order.
      operationId: UpdateOrder
      x-api-path-slug: v3merchantsmidordersorderid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [lineItems, customers, payments, credits,
          refunds, serviceCharge, discounts]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
    delete:
      summary: Delete an order
      description: Delete an order.
      operationId: DeleteOrder
      x-api-path-slug: v3merchantsmidordersorderid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
  /v3/merchants/{mId}/authorizations:
    get:
      summary: Get all authorizations.
      description: An authorization is a promise by a card issuer that a merchant
        can charge the customer up to the specified amount in the future. These are
        typically created when a merchant uses the "Bar Tabs" app and "Authorizations"
        app.
      operationId: GetAuthorizations
      x-api-path-slug: v3merchantsmidauthorizations-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [payment]'
      - in: query
        name: filter
        description: 'Filter fields: [last4, note, amount, tabName, orderId, cardType,
          orderModifiedTime, type, device'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Authorizations
    post:
      summary: Create an authorization on a Payment
      description: Authorization must reference a payment, have an amount greater
        than 0, and have a type.
      operationId: CreateAuthorization
      x-api-path-slug: v3merchantsmidauthorizations-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Authorizations
  /v3/merchants/{mId}/item_groups/{itemGroupId}:
    get:
      summary: Get a single item group
      description: Get a single item group.
      operationId: GetItemGroup
      x-api-path-slug: v3merchantsmiditem-groupsitemgroupid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items, attributes]'
      - in: path
        name: itemGroupId
        description: Item Group Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Groups
      - ItemGroupId
    post:
      summary: Update an item group
      description: Update an item group.
      operationId: UpdateItemGroup
      x-api-path-slug: v3merchantsmiditem-groupsitemgroupid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [items, attributes]'
      - in: path
        name: itemGroupId
        description: Item Group Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Groups
      - ItemGroupId
    delete:
      summary: Delete an item group
      description: Delete an item group.
      operationId: DeleteItemGroup
      x-api-path-slug: v3merchantsmiditem-groupsitemgroupid-delete
      parameters:
      - in: path
        name: itemGroupId
        description: Item Group Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Groups
      - ItemGroupId
  /v3/apps/{aId}/merchants/{mId}/billing_info:
    get:
      summary: Get merchant's billing information for an app
      description: Gives detailed information about the status of the merchant's billing
        for the app including current subscription tier and trial status. Requires
        an OAuth generated token.
      operationId: GetMerchantBillingInfo
      x-api-path-slug: v3appsaidmerchantsmidbilling-info-get
      parameters:
      - in: path
        name: aId
        description: App Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Apps
      - Merchants
      - Billing
      - Info
  /v3/merchants/{mId}/authorizations/{authId}:
    get:
      summary: Get a single authorization
      description: Get a single authorization.
      operationId: GetAuthorization
      x-api-path-slug: v3merchantsmidauthorizationsauthid-get
      parameters:
      - in: path
        name: authId
      - in: query
        name: expand
        description: 'Expandable fields: [cardTransaction, dccInfo, germanInfo, appTracking,
          taxRates, lineItemPayments, refunds, order, tender, employee, transactionInfo]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Authorizations
      - AuthId
    post:
      summary: Add a single authorization
      description: .Add a single authorization
      operationId: UpdateAuthorization
      x-api-path-slug: v3merchantsmidauthorizationsauthid-post
      parameters:
      - in: path
        name: authId
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Authorizations
      - AuthId
    delete:
      summary: Delete a single authorization
      description: .Delete a single authorization
      operationId: DeleteAuthorization
      x-api-path-slug: v3merchantsmidauthorizationsauthid-delete
      parameters:
      - in: path
        name: authId
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Authorizations
      - AuthId
  /v3/apps/{aId}/merchants/{mId}/metereds/{meteredId}:
    post:
      summary: Create an app billing metered event
      description: This creates an app billing metered event. The amount Clover will
        charge the specified merchant is based on the cost specified for this metered
        object in the Developer Dashboard. The merchant will be billed during their
        next scheduled billing cycle. Passing "count" as a query parameter will bill
        the merchant for that number of metered events. "count" must be passed as
        a query parameter in order to function properly ??? if passed in the request
        body, it will be ignored. If not specified, "count" will default to 1. See
        https://docs.clover.com/launch/billing/ for more information. Requires an
        OAuth generated token.
      operationId: CreateMerchantAppMeteredEvent
      x-api-path-slug: v3appsaidmerchantsmidmeteredsmeteredid-post
      parameters:
      - in: path
        name: aId
        description: App Id
      - in: path
        name: meteredId
        description: Metered Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Apps
      - Merchants
      - Metereds
      - MeteredId
    get:
      summary: Get the app metered billing events for an app metered, e.g. all the
        billing events for the event 'reservation'
      description: Get the app metered billing events for an app metered, e.g. all
        the billing events for the event 'reservation'.
      operationId: GetMerchantAppMeteredEvents
      x-api-path-slug: v3appsaidmerchantsmidmeteredsmeteredid-get
      parameters:
      - in: path
        name: aId
        description: App Id
      - in: path
        name: meteredId
        description: Metered Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Apps
      - Merchants
      - Metereds
      - MeteredId
  /v3/merchants/{mId}/tags:
    get:
      summary: Get all tags
      description: Similarly to how they are described by wikipedia, tags are an informal
        way of establishing a relationship. Tags currently may be associated with
        items and printers. When an tag is associated with both an item and a printer
        that establishes a special relationship that results in those items being
        printed out on the associated printer when printing an order. Other than that
        special case there is no effect when an item is associated with a tag. Developers
        may use tags to establish a relationship meaningful for their needs.
      operationId: GetTags
      x-api-path-slug: v3merchantsmidtags-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items, printers]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, deleted, name, id]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tags
    post:
      summary: Create a tag
      description: Create a tag.
      operationId: CreateTag
      x-api-path-slug: v3merchantsmidtags-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tags
  /v3/merchants/{mId}/orders/{orderId}/discounts:
    get:
      summary: Get all discounts for an order
      description: Get all discounts for an order.
      operationId: GetOrderDiscounts
      x-api-path-slug: v3merchantsmidordersorderiddiscounts-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Discounts
    post:
      summary: Create a discount on an order or line item
      description: Create a discount on an order or line item.
      operationId: CreateDiscount
      x-api-path-slug: v3merchantsmidordersorderiddiscounts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Discounts
  /v3/apps/{aId}/merchants/{mId}/metereds/{meteredId}/events/{eventId}:
    get:
      summary: Get an app billing metered event
      description: This enables you to fetch the details on a merchants app billing
        metered event. Requires an OAuth generated token.
      operationId: GetMerchantAppMeteredEvent
      x-api-path-slug: v3appsaidmerchantsmidmeteredsmeteredideventseventid-get
      parameters:
      - in: path
        name: aId
        description: App Id
      - in: path
        name: eventId
      - in: path
        name: meteredId
        description: Metered Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Apps
      - Merchants
      - Metereds
      - MeteredId
      - Events
      - EventId
    delete:
      summary: Delete an app billing metered event, if not charged.
      description: This deletes an app billing metered event, if the event has not
        been charged yet. See https://docs.clover.com/launch/billing/ for more information.
        Requires an OAuth generated token.
      operationId: DeleteMerchantAppMeteredEvent
      x-api-path-slug: v3appsaidmerchantsmidmeteredsmeteredideventseventid-delete
      parameters:
      - in: path
        name: aId
        description: App Id
      - in: path
        name: eventId
      - in: path
        name: meteredId
        description: Metered Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Apps
      - Merchants
      - Metereds
      - MeteredId
      - Events
      - EventId
  /v3/merchants/{mId}/orders/{orderId}/discounts/{discountId}:
    delete:
      summary: Delete a discount
      description: Delete a discount.
      operationId: RemoveDiscount
      x-api-path-slug: v3merchantsmidordersorderiddiscountsdiscountid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: discountId
        description: Discount Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Discounts
      - DiscountId
  /v3/merchants/{mId}/tags/{tagId}:
    get:
      summary: Get a single tag
      description: Get a single tag.
      operationId: GetTag
      x-api-path-slug: v3merchantsmidtagstagid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items, printers]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: tagId
        description: Tag Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tags
      - TagId
    post:
      summary: Update a single tag
      description: Update a single tag.
      operationId: UpdateTag
      x-api-path-slug: v3merchantsmidtagstagid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [items, printers]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: tagId
        description: Tag Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tags
      - TagId
    delete:
      summary: Delete a tag
      description: Delete a tag.
      operationId: DeleteTag
      x-api-path-slug: v3merchantsmidtagstagid-delete
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: tagId
        description: Tag Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tags
      - TagId
  /v3/merchants/{mId}/orders/{orderId}/line_items:
    get:
      summary: Get all line items for an order
      description: Get all line items for an order.
      operationId: GetOrderLineItems
      x-api-path-slug: v3merchantsmidordersorderidline-items-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [employee, orderType, discounts, modifications,
          taxRates, payments]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
    post:
      summary: Create a new line item
      description: Create a new line item.
      operationId: CreateLineItem
      x-api-path-slug: v3merchantsmidordersorderidline-items-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
  /v3/merchants/{mId}/items/{itemId}/tags:
    get:
      summary: Get tags for a single item
      description: Get tags for a single item.
      operationId: GetItemTags
      x-api-path-slug: v3merchantsmiditemsitemidtags-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items, printers]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, deleted, name, id]'
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
      - ItemId
      - Tags
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}:
    get:
      summary: Get a line item
      description: Get a line item.
      operationId: GetOrderLineItem
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [employee, orderType, discounts, modifications,
          taxRates, payments]'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
    post:
      summary: Update a line item
      description: Update a line item.
      operationId: UpdateOrderLineItem
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [employee, orderType, discounts, modifications,
          taxRates, payments]'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
    delete:
      summary: Void a line item
      description: Void a line item.
      operationId: DeleteOrderLineItem
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
  /v3/merchants/{mId}/tags/{tagId}/items:
    get:
      summary: Get all items for a single tag
      description: Get all items for a single tag.
      operationId: GetTaggedItems
      x-api-path-slug: v3merchantsmidtagstagiditems-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items, printers]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, hidden, itemCode, alternateName,
          option'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: tagId
        description: Tag Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tags
      - TagId
      - Items
  /v3/merchants/{mId}/tag_items:
    post:
      summary: Create or delete tag items
      description: Create or delete tag items.
      operationId: CreateOrDeleteTagItems
      x-api-path-slug: v3merchantsmidtag-items-post
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tag
      - Items
  /v3/merchants/{mId}/tax_rates:
    get:
      summary: Get all tax rates
      description: Get all tax rates.
      operationId: GetTaxRates
      x-api-path-slug: v3merchantsmidtax-rates-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: query
        name: filter
        description: 'Filter fields: [isDefault, rate, items'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tax
      - Rates
    post:
      summary: Create a tax rate for a merchant
      description: Create a tax rate for a merchant.
      operationId: CreateTaxRate
      x-api-path-slug: v3merchantsmidtax-rates-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tax
      - Rates
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}/discounts:
    post:
      summary: Create a discount on an order or line item
      description: Create a discount on an order or line item.
      operationId: CreateDiscount
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemiddiscounts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
      - Discounts
  /v3/merchants/{mId}/tax_rates/{taxId}:
    get:
      summary: Get a single tax rate
      description: Get a single tax rate.
      operationId: GetTaxRate
      x-api-path-slug: v3merchantsmidtax-ratestaxid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: taxId
        description: Tax Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tax
      - Rates
      - TaxId
    post:
      summary: Update a single tax rate
      description: Update a single tax rate.
      operationId: UpdateTaxRate
      x-api-path-slug: v3merchantsmidtax-ratestaxid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: taxId
        description: Tax Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tax
      - Rates
      - TaxId
    delete:
      summary: Delete a single tax rate
      description: Delete a single tax rate.
      operationId: DeleteTaxRate
      x-api-path-slug: v3merchantsmidtax-ratestaxid-delete
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: taxId
        description: Tax Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tax
      - Rates
      - TaxId
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}/discounts/{discountId}:
    delete:
      summary: Delete a discount
      description: Delete a discount.
      operationId: RemoveDiscount
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemiddiscountsdiscountid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: discountId
        description: Discount Id
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
      - Discounts
      - DiscountId
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}/modifications:
    post:
      summary: Apply a modification to a line item
      description: 'Create a modification, a record of a modifier as it exists at
        the time it is applied to the lineItem. To view current modifications use
        an ''expand=modifications'' query parameter on the lineItem. To learn more
        about applying a modification see: https://docs.clover.com/build/working-with-orders/#add-item-modifiers'
      operationId: ApplyModification
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemidmodifications-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
      - Modifications
  /v3/merchants/{mId}/categories:
    get:
      summary: Get all categories
      description: Categories alter the user experience of the Register app. Items
        will appear in the Register app within the categories they are members of.
        Items may be associated with no, one or multiple categories. Items are displayed
        in Register in the order in which they are added to a category. Categories
        are displayed in Register using the sort order value for each category.
      operationId: GetCategories
      x-api-path-slug: v3merchantsmidcategories-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, deleted, sortOrder, name, id]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Categories
    post:
      summary: Create an item category
      description: Create an item category.
      operationId: CreateCategory
      x-api-path-slug: v3merchantsmidcategories-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Categories
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}/modifications/{modificationId}:
    delete:
      summary: Remove a modification from a line item
      description: Delete a modification by UUID, removing the record of an applied
        modification
      operationId: RemoveModification
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemidmodificationsmodificationid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modificationId
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
      - Modifications
      - ModificationId
  /v3/merchants/{mId}/categories/{catId}:
    get:
      summary: Get a category
      description: Get a category.
      operationId: GetCategory
      x-api-path-slug: v3merchantsmidcategoriescatid-get
      parameters:
      - in: path
        name: catId
        description: Category Id
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Categories
      - CatId
    post:
      summary: Update a category
      description: Update a category.
      operationId: UpdateCategory
      x-api-path-slug: v3merchantsmidcategoriescatid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: catId
        description: Category Id
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Categories
      - CatId
    delete:
      summary: Delete a single item category
      description: Delete a single item category.
      operationId: DeleteCategory
      x-api-path-slug: v3merchantsmidcategoriescatid-delete
      parameters:
      - in: path
        name: catId
        description: Category Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Categories
      - CatId
  /v3/merchants/{mId}/orders/{orderId}/bulk_line_items:
    post:
      summary: Create multiple line items in bulk.
      description: Create multiple line items in bulk..
      operationId: BulkCreateLineItems
      x-api-path-slug: v3merchantsmidordersorderidbulk-line-items-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Bulk
      - Line
      - Items
  /v3/merchants/{mId}/orders/{orderId}/payments:
    post:
      summary: Create a payment record on an order
      description: Create a payment record on an order.
      operationId: CreatePaymentForOrder
      x-api-path-slug: v3merchantsmidordersorderidpayments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Payments
    get:
      summary: Get all payments for an order
      description: Get all payments for an order.
      operationId: GetOrderPayments
      x-api-path-slug: v3merchantsmidordersorderidpayments-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [cardTransaction, dccInfo, germanInfo, appTracking,
          taxRates, lineItemPayments, refunds, order, tender, employee, transactionInfo]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, voidReason, cardTransaction'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Payments
  /v3/merchants/{mId}/categories/{catId}/items:
    get:
      summary: Get all items in a single category
      description: Get all items in a single category.
      operationId: GetCategoryItems
      x-api-path-slug: v3merchantsmidcategoriescatiditems-get
      parameters:
      - in: path
        name: catId
        description: Category Id
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, deleted, sortOrder, name, id]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Categories
      - CatId
      - Items
  /v3/merchants/{mId}/items/{itemId}/categories:
    get:
      summary: Get all categories of a single item
      description: Get all categories of a single item.
      operationId: GetItemCategories
      x-api-path-slug: v3merchantsmiditemsitemidcategories-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, deleted, sortOrder, name, id]'
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
      - ItemId
      - Categories
  /v3/merchants/{mId}/category_items:
    post:
      summary: Create or delete an item/category association
      description: Create or delete an item/category association.
      operationId: CreateOrDeleteCategoryItems
      x-api-path-slug: v3merchantsmidcategory-items-post
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Category
      - Items
  /v3/merchants/{mId}/tax_rate_items:
    post:
      summary: Create or delete a tax rate item
      description: Create or delete a tax rate item.
      operationId: CreateOrDeleteTaxRateItems
      x-api-path-slug: v3merchantsmidtax-rate-items-post
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tax
      - Rate
      - Items
  /v3/merchants/{mId}/tax_rates/{taxId}/items:
    get:
      summary: Get items by tax rate
      description: Get items by tax rate.
      operationId: GetItemsByTaxRate
      x-api-path-slug: v3merchantsmidtax-ratestaxiditems-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: query
        name: filter
        description: 'Filter fields: [id, name, sku, modifiedTime, deleted, hidden,
          price, alternateName, itemCode, item'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: taxId
        description: Tax Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Tax
      - Rates
      - TaxId
      - Items
  /v3/merchants/{mId}/modifier_groups:
    get:
      summary: Get all modifier groups
      description: These groupings are the categories different modifiers belong to.
        Modifier groups can be made available for specific inventory Items by creating
        an item to modifier group association.
      operationId: GetModifierGroups
      x-api-path-slug: v3merchantsmidmodifier-groups-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [modifiers, items]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, item'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
    post:
      summary: Create a modifier group
      description: Create a new modifier group. Modifiers can be associated with a
        modifier group after it has been created.
      operationId: CreateModifierGroup
      x-api-path-slug: v3merchantsmidmodifier-groups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [modifiers, items]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
  /v3/merchants/{mId}/modifier_groups/{modGroupId}:
    get:
      summary: Get a modifier group
      description: Get a single modifier group by it's UUID
      operationId: GetModifierGroup
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [modifiers, items]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
    post:
      summary: Update a modifier group
      description: Update a modifier group. In order to add modifiers use the create
        modifiers endpoint.
      operationId: UpdateModifierGroup
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [modifiers, items]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
    delete:
      summary: Delete a modifier group
      description: Delete an existing modifier group, identified by UUID. This also
        deletes all modifiers within that group.
      operationId: DeleteModifierGroup
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupid-delete
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
  /v3/merchants/{mId}/item_modifier_groups:
    post:
      summary: Create or delete item to modifier group associations
      description: 'Create or delete one or more association objects (item modifier
        groups). Modifiers can only be applied to items associated with that modifier''s
        group. Learn more about object associations here: https://docs.clover.com/build/web-api/#object-associations'
      operationId: CreateOrDeleteItemModifierGroups
      x-api-path-slug: v3merchantsmiditem-modifier-groups-post
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Modifier
      - Groups
  /v3/merchants/{mId}/modifier_group_sort_orders:
    post:
      summary: Update the priorities for a collection of up to 200 modifier groups
        at a time
      description: Update the priorities for a collection of up to 200 modifier groups
        at a time.
      operationId: UpdateModifierGroupSortOrders
      x-api-path-slug: v3merchantsmidmodifier-group-sort-orders-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Group
      - Sort
      - Orders
  /v3/merchants/{mId}/payments:
    get:
      summary: Get all payments
      description: 'Retrieve payment information including total amount, tipAmount,
        taxAmount, and result status.To POST a payment see: https://docs.clover.com/build/developer-pay-api/'
      operationId: GetPayments
      x-api-path-slug: v3merchantsmidpayments-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [tender, taxRates, germanInfo, lineItemPayments,
          cardTransaction, dccInfo, appTracking, refunds, order, transactionInfo]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, voidReason, cardTransaction'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Payments
  /v3/merchants/{mId}/modifiers:
    get:
      summary: Get all modifiers
      description: Get all modifiers regardless of their modifier group.
      operationId: GetModifiers
      x-api-path-slug: v3merchantsmidmodifiers-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [modifierGroup]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, price, name, alternateName, id,
          modifierGroup'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifiers
  /v3/merchants/{mId}/payments/{payId}:
    get:
      summary: Get a single payment
      description: Get a single payment.
      operationId: GetPayment
      x-api-path-slug: v3merchantsmidpaymentspayid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [cardTransaction, dccInfo, germanInfo, appTracking,
          taxRates, lineItemPayments, refunds, order, tender, employee, transactionInfo]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: payId
        description: Payment Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Payments
      - PayId
    post:
      summary: ""
      description: .
      operationId: UpdatePayment
      x-api-path-slug: v3merchantsmidpaymentspayid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: payId
        description: Payment Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Payments
      - PayId
  /v3/merchants/{mId}/modifier_groups/{modGroupId}/modifiers:
    get:
      summary: Get all modifiers belonging to a single modifier group
      description: Get an array containing the modifiers in a single modifier group.
      operationId: GetModifiersByGroup
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [modifiers, items]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, price, name, alternateName, id,
          modifierGroup'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
      - Modifiers
    post:
      summary: Create a modifier
      description: Create a modifier object belonging to the modifier group identified
        in the URL.
      operationId: CreateModifier
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [modifierGroup]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
      - Modifiers
  /v3/merchants/{mId}/modifier_groups/{modGroupId}/modifiers/{modId}:
    get:
      summary: Get a single modifier
      description: Get a single modifier by it's group, and it's UUID
      operationId: GetModifier
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [modifierGroup]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      - in: path
        name: modId
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
      - Modifiers
      - ModId
    post:
      summary: Update a single modifier
      description: Update a modifier. Note that once it has been created, it is not
        possible to change a modifier's group.
      operationId: UpdateModifier
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [modifierGroup]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      - in: path
        name: modId
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
      - Modifiers
      - ModId
    delete:
      summary: Delete a single modifier
      description: Delete a single modifier by it's UUID
      operationId: DeleteModifier
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      - in: path
        name: modId
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
      - Modifiers
      - ModId
  /v3/merchants/{mId}/employees/{empId}/payments:
    get:
      summary: Get all payments under an employee
      description: Get all payments under an employee.
      operationId: GetEmployeePayments
      x-api-path-slug: v3merchantsmidemployeesempidpayments-get
      parameters:
      - in: path
        name: empId
        description: Employee Id
      - in: query
        name: expand
        description: 'Expandable fields: [cardTransaction, dccInfo, germanInfo, appTracking,
          taxRates, lineItemPayments, refunds, order, tender, employee, transactionInfo]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, voidReason, cardTransaction'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employees
      - EmpId
      - Payments
  /v3/merchants/{mId}/refunds:
    get:
      summary: Get all refunds for a merchant
      description: Get all refunds for a merchant.
      operationId: GetRefunds
      x-api-path-slug: v3merchantsmidrefunds-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [payment, germanInfo, appTracking, employee,
          overrideMerchantTender, serviceCharge, lineItems]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Refunds
  /v3/merchants/{mId}/refunds/{refundId}:
    get:
      summary: Get a single refund
      description: Get a single refund.
      operationId: GetRefund
      x-api-path-slug: v3merchantsmidrefundsrefundid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [payment, germanInfo, appTracking, employee,
          overrideMerchantTender, serviceCharge, lineItems]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: refundId
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Refunds
      - RefundId
  /v3/merchants/{mId}/credits:
    get:
      summary: Get a list of credits
      description: Get a list of credits.
      operationId: GetCredits
      x-api-path-slug: v3merchantsmidcredits-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [dccInfo, germanInfo, appTracking, tender,
          employee, cardTransaction, order, taxRates]'
      - in: query
        name: filter
        description: 'Filter fields: [device'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Credits
  /v3/merchants/{mId}/attributes:
    get:
      summary: Get all attributes
      description: See the description for 'get all item groups'.
      operationId: GetAttributes
      x-api-path-slug: v3merchantsmidattributes-get
      parameters:
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, name, id, deletedTime, itemGroup'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Attributes
    post:
      summary: Create an attribute
      description: Create an attribute.
      operationId: CreateAttribute
      x-api-path-slug: v3merchantsmidattributes-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [options]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Attributes
  /v3/merchants/{mId}/credits/{cId}:
    get:
      summary: Get a single credit
      description: Get a single credit.
      operationId: GetCredit
      x-api-path-slug: v3merchantsmidcreditscid-get
      parameters:
      - in: path
        name: cId
      - in: query
        name: expand
        description: 'Expandable fields: [dccInfo, germanInfo, appTracking, tender,
          employee, cardTransaction, order, taxRates]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Credits
      - CId
  /v3/merchants/{mId}/credit_refunds:
    get:
      summary: Get a list of credit refunds
      description: Get a list of credit refunds.
      operationId: GetCreditRefunds
      x-api-path-slug: v3merchantsmidcredit-refunds-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [credit, germanInfo, appTracking]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Credit
      - Refunds
  /v3/merchants/{mId}/attributes/{attributeId}:
    get:
      summary: Get a single attribute
      description: Get a single attribute.
      operationId: GetAttribute
      x-api-path-slug: v3merchantsmidattributesattributeid-get
      parameters:
      - in: path
        name: attributeId
        description: Attribute Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Attributes
      - AttributeId
    post:
      summary: Update a single attribute
      description: Update a single attribute.
      operationId: UpdateAttribute
      x-api-path-slug: v3merchantsmidattributesattributeid-post
      parameters:
      - in: path
        name: attributeId
        description: Attribute Id
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [options]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Attributes
      - AttributeId
    delete:
      summary: Delete a single attribute
      description: Delete a single attribute.
      operationId: DeleteAttribute
      x-api-path-slug: v3merchantsmidattributesattributeid-delete
      parameters:
      - in: path
        name: attributeId
        description: Attribute Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Attributes
      - AttributeId
  /v3/merchants/{mId}/credit_refunds/{crId}:
    get:
      summary: Get a credit refund
      description: Get a credit refund.
      operationId: GetCreditRefund
      x-api-path-slug: v3merchantsmidcredit-refundscrid-get
      parameters:
      - in: path
        name: crId
      - in: query
        name: expand
        description: 'Expandable fields: [credit, germanInfo, appTracking]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Credit
      - Refunds
      - CrId
  /v3/merchants/{mId}/employee_cards:
    post:
      summary: Add employee cards
      description: .Add employee cards
      operationId: CreateOrUpdateEmployeeCard
      x-api-path-slug: v3merchantsmidemployee-cards-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employee
      - Cards
    get:
      summary: Get employee cards
      description: .Get employee cards
      operationId: GetEmployeeCards
      x-api-path-slug: v3merchantsmidemployee-cards-get
      parameters:
      - in: query
        name: filter
        description: 'Filter fields: [id, employee'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employee
      - Cards
  /v3/merchants/{mId}/options:
    get:
      summary: Get all options
      description: See the description for 'get all item groups'.
      operationId: GetOptions
      x-api-path-slug: v3merchantsmidoptions-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: []'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, item'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Options
  /v3/merchants/{mId}/employee_cards/{employeeCardId}:
    get:
      summary: Get employee card
      description: .Get employee card
      operationId: GetEmployeeCard
      x-api-path-slug: v3merchantsmidemployee-cardsemployeecardid-get
      parameters:
      - in: path
        name: employeeCardId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employee
      - Cards
      - EmployeeCardId
    delete:
      summary: Delete employee cards
      description: .Delete employee cards
      operationId: DeleteEmployeeCard
      x-api-path-slug: v3merchantsmidemployee-cardsemployeecardid-delete
      parameters:
      - in: path
        name: employeeCardId
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employee
      - Cards
      - EmployeeCardId
  /v3/merchants/{mId}/attributes/{attributeId}/options:
    get:
      summary: Get all options with a given attribute
      description: Get all options with a given attribute.
      operationId: GetOptionsByAttribute
      x-api-path-slug: v3merchantsmidattributesattributeidoptions-get
      parameters:
      - in: path
        name: attributeId
        description: Attribute Id
      - in: query
        name: expand
        description: 'Expandable fields: []'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, item'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Attributes
      - AttributeId
      - Options
    post:
      summary: Create an option
      description: Create an option.
      operationId: CreateOption
      x-api-path-slug: v3merchantsmidattributesattributeidoptions-post
      parameters:
      - in: path
        name: attributeId
        description: Attribute Id
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: []'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Attributes
      - AttributeId
      - Options
  /v3/merchants/{mId}/orders/{orderId}/service_charge/:
    post:
      summary: ""
      description: .
      operationId: ApplyServiceCharge
      x-api-path-slug: v3merchantsmidordersorderidservice-charge-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Service
      - Charge
  /v3/merchants/{mId}/attributes/{attributeId}/options/{optionId}:
    get:
      summary: Get all options with a given attribute
      description: Get all options with a given attribute.
      operationId: GetOptionsByAttribute
      x-api-path-slug: v3merchantsmidattributesattributeidoptionsoptionid-get
      parameters:
      - in: path
        name: attributeId
        description: Attribute Id
      - in: query
        name: expand
        description: 'Expandable fields: []'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, item'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: optionId
        description: Option Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Attributes
      - AttributeId
      - Options
      - OptionId
    post:
      summary: Update an option
      description: Update an option.
      operationId: UpdateOption
      x-api-path-slug: v3merchantsmidattributesattributeidoptionsoptionid-post
      parameters:
      - in: path
        name: attributeId
        description: Attribute Id
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: []'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: optionId
        description: Option Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Attributes
      - AttributeId
      - Options
      - OptionId
    delete:
      summary: Delete an option
      description: Delete an option.
      operationId: DeleteOption
      x-api-path-slug: v3merchantsmidattributesattributeidoptionsoptionid-delete
      parameters:
      - in: path
        name: attributeId
        description: Attribute Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: optionId
        description: Option Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Attributes
      - AttributeId
      - Options
      - OptionId
  /v3/merchants/{mId}/orders/{orderId}/service_charge/{chargeId}:
    delete:
      summary: Remove service charge from an order
      description: Remove service charge from an order.
      operationId: RemoveServiceCharge
      x-api-path-slug: v3merchantsmidordersorderidservice-chargechargeid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: chargeId
        description: Service Charge Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Service
      - Charge
      - ChargeId
  /v3/merchants/{mId}/orders/{orderId}/voided_line_items:
    post:
      summary: Void a line item
      description: Void a line item.
      operationId: VoidOrderLineItem
      x-api-path-slug: v3merchantsmidordersorderidvoided-line-items-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Voided
      - Line
      - Items
  /v3/merchants/{mId}/voided_line_items:
    get:
      summary: Get order line items that were recorded after a void
      description: Get order line items that were recorded after a void.
      operationId: GetVoidedOrderLineItems
      x-api-path-slug: v3merchantsmidvoided-line-items-get
      parameters:
      - in: query
        name: filter
        description: 'Filter fields: [reason, id, name, price, quantity, printed,
          deletedTime, merchantId, orderId, removedById]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Voided
      - Line
      - Items
  /v3/merchants/{mId}/orders/{orderId}/line_items/{oldLineItemId}/exchange/{lineItemId}:
    post:
      summary: Create or exchange a line item
      description: Create or exchange a line item.
      operationId: SetOrderLineItem
      x-api-path-slug: v3merchantsmidordersorderidline-itemsoldlineitemidexchangelineitemid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: oldLineItemId
        description: Old Line Item Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - OldLineItemId
      - Exchange
      - LineItemId
  /v3/merchants/{mId}/option_items:
    post:
      summary: Create or delete item/option association
      description: See the description for 'get all item groups'.
      operationId: CreateOrDeleteOptionItems
      x-api-path-slug: v3merchantsmidoption-items-post
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Option
      - Items
  /v3/merchants/{mId}/discounts:
    get:
      summary: Get all discounts
      description: Get all discounts.
      operationId: GetDiscounts
      x-api-path-slug: v3merchantsmiddiscounts-get
      parameters:
      - in: query
        name: filter
        description: 'Filter fields: [id, amount, percentage, modifiedtime]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Discounts
    post:
      summary: Create an discount
      description: Create an discount.
      operationId: CreateDiscount
      x-api-path-slug: v3merchantsmiddiscounts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Discounts
  /v3/merchants/{mId}/discounts/{discountId}:
    get:
      summary: Get a single discount
      description: Get a single discount.
      operationId: GetDiscount
      x-api-path-slug: v3merchantsmiddiscountsdiscountid-get
      parameters:
      - in: path
        name: discountId
        description: Discount Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Discounts
      - DiscountId
    post:
      summary: Update an discount
      description: Update an discount.
      operationId: UpdateDiscount
      x-api-path-slug: v3merchantsmiddiscountsdiscountid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: discountId
        description: Discount Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Discounts
      - DiscountId
    delete:
      summary: Delete a discount
      description: Delete a discount.
      operationId: DeleteDiscount
      x-api-path-slug: v3merchantsmiddiscountsdiscountid-delete
      parameters:
      - in: path
        name: discountId
        description: Discount Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Discounts
      - DiscountId