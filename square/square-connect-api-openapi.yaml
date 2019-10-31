swagger: "2.0"
x-collection-name: Square
x-complete: 1
info:
  title: Square Connect
  description: client-library-for-accessing-the-square-connect-apis
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/me:
    get:
      summary: Get a business's information.
      description: Get a business's information.
      operationId: RetrieveBusiness
      x-api-path-slug: v1me-get
      responses:
        200:
          description: OK
      tags:
      - Businesss
      - Information
  /v1/me/employees:
    get:
      summary: Provides summary information for all of a business's employees.
      description: Provides summary information for all of a business's employees.
      operationId: ListEmployees
      x-api-path-slug: v1meemployees-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: begin_created_at
        description: If filtering results by their created_at field, the beginning
          of the requested reporting period, in ISO 8601 format
      - in: query
        name: begin_updated_at
        description: If filtering results by their updated_at field, the beginning
          of the requested reporting period, in ISO 8601 format
      - in: query
        name: end_created_at
        description: If filtering results by their created_at field, the end of the
          requested reporting period, in ISO 8601 format
      - in: query
        name: end_updated_at
        description: If filtering results by there updated_at field, the end of the
          requested reporting period, in ISO 8601 format
      - in: query
        name: external_id
        description: If provided, the endpoint returns only employee entities with
          the specified external_id
      - in: query
        name: limit
        description: The maximum integer number of employee entities to return in
          a single response
      - in: query
        name: order
        description: The order in which employees are listed in the response, based
          on their created_at field
      - in: query
        name: status
        description: If provided, the endpoint returns only employee entities with
          the specified status (ACTIVE or INACTIVE)
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Of
      - Businesss
      - Employees
    post:
      summary: Creates an employee for a business.
      description: Creates an employee for a business.
      operationId: CreateEmployee
      x-api-path-slug: v1meemployees-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Employeea
      - Business
  /v1/me/employees/{employee_id}:
    get:
      summary: Provides the details for a single employee.
      description: Provides the details for a single employee.
      operationId: RetrieveEmployee
      x-api-path-slug: v1meemployeesemployee-id-get
      parameters:
      - in: path
        name: employee_id
        description: The employees ID
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Detailsa
      - Single
      - Employee
    put:
      summary: Update Employee
      description: Update Employee
      operationId: UpdateEmployee
      x-api-path-slug: v1meemployeesemployee-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: employee_id
        description: The ID of the role to modify
      responses:
        200:
          description: OK
      tags:
      - Employee
  /v1/me/locations:
    get:
      summary: Provides details for a business's locations, including their IDs.
      description: Provides details for a business's locations, including their IDs.
      operationId: v1.me.locations.get
      x-api-path-slug: v1melocations-get
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Detailsa
      - Businesss
      - Locations
      - ""
      - Including
      - Their
      - IDs
  /v1/me/roles:
    get:
      summary: Provides summary information for all of a business's employee roles.
      description: Provides summary information for all of a business's employee roles.
      operationId: ListEmployeeRoles
      x-api-path-slug: v1meroles-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: limit
        description: The maximum integer number of employee entities to return in
          a single response
      - in: query
        name: order
        description: The order in which employees are listed in the response, based
          on their created_at field
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Of
      - Businesss
      - Employee
      - Roles
    post:
      summary: Creates an employee role you can then assign to employees.
      description: Creates an employee role you can then assign to employees.
      operationId: CreateEmployeeRole
      x-api-path-slug: v1meroles-post
      parameters:
      - in: body
        name: EmployeeRole
        description: An EmployeeRole object with a name and permissions, and an optional
          owner flag
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Employee
      - Role
      - You
      - Can
      - Then
      - Assign
      - To
      - Employees
  /v1/me/roles/{role_id}:
    get:
      summary: Provides the details for a single employee role.
      description: Provides the details for a single employee role.
      operationId: RetrieveEmployeeRole
      x-api-path-slug: v1merolesrole-id-get
      parameters:
      - in: path
        name: role_id
        description: The roles ID
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Detailsa
      - Single
      - Employee
      - Role
    put:
      summary: Modifies the details of an employee role.
      description: Modifies the details of an employee role.
      operationId: UpdateEmployeeRole
      x-api-path-slug: v1merolesrole-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: role_id
        description: The ID of the role to modify
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Employee
      - Role
  /v1/me/timecards:
    get:
      summary: Provides summary information for all of a business's employee timecards.
      description: Provides summary information for all of a business's employee timecards.
      operationId: ListTimecards
      x-api-path-slug: v1metimecards-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: begin_clockin_time
        description: If filtering results by their clockin_time field, the beginning
          of the requested reporting period, in ISO 8601 format
      - in: query
        name: begin_clockout_time
        description: If filtering results by their clockout_time field, the beginning
          of the requested reporting period, in ISO 8601 format
      - in: query
        name: begin_updated_at
        description: If filtering results by their updated_at field, the beginning
          of the requested reporting period, in ISO 8601 format
      - in: query
        name: deleted
        description: If true, only deleted timecards are returned
      - in: query
        name: employee_id
        description: If provided, the endpoint returns only timecards for the employee
          with the specified ID
      - in: query
        name: end_clockin_time
        description: If filtering results by their clockin_time field, the end of
          the requested reporting period, in ISO 8601 format
      - in: query
        name: end_clockout_time
        description: If filtering results by their clockout_time field, the end of
          the requested reporting period, in ISO 8601 format
      - in: query
        name: end_updated_at
        description: If filtering results by their updated_at field, the end of the
          requested reporting period, in ISO 8601 format
      - in: query
        name: limit
        description: The maximum integer number of employee entities to return in
          a single response
      - in: query
        name: order
        description: The order in which timecards are listed in the response, based
          on their created_at field
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Of
      - Businesss
      - Employee
      - Timecards
    post:
      summary: Creates a timecard for an employee. Each timecard corresponds to a
        single shift.
      description: Creates a timecard for an employee. Each timecard corresponds to
        a single shift.
      operationId: CreateTimecard
      x-api-path-slug: v1metimecards-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Timecardan
      - Employee
      - ""
      - Each
      - Timecard
      - Corresponds
      - To
      - Single
      - Shift
  /v1/me/timecards/{timecard_id}:
    delete:
      summary: Deletes a timecard. Deleted timecards are still accessible from Connect
        API endpoints, but the value of their deleted field is set to true. See Handling
        deleted timecards for more information.
      description: Deletes a timecard. Deleted timecards are still accessible from
        Connect API endpoints, but the value of their deleted field is set to true.
        See Handling deleted timecards for more information.
      operationId: DeleteTimecard
      x-api-path-slug: v1metimecardstimecard-id-delete
      parameters:
      - in: path
        name: timecard_id
        description: The ID of the timecard to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Timecard
      - ""
      - D
      - Timecards
      - Are
      - Still
      - Accessible
      - From
      - Connect
      - Endpoints
      - ""
      - But
      - Value
      - Of
      - Their
      - Deleted
      - Field
      - Is
      - Set
      - To
      - "True"
      - ""
      - See
      - Handling
      - Deleted
      - Timecardsmore
      - Information
    get:
      summary: Provides the details for a single timecard.
      description: Provides the details for a single timecard.
      operationId: RetrieveTimecard
      x-api-path-slug: v1metimecardstimecard-id-get
      parameters:
      - in: path
        name: timecard_id
        description: The timecards ID
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Detailsa
      - Single
      - Timecard
    put:
      summary: Modifies a timecard's details. This creates an API_EDIT event for the
        timecard. You can view a timecard's event history with the List Timecard Events
        endpoint.
      description: Modifies a timecard's details. This creates an API_EDIT event for
        the timecard. You can view a timecard's event history with the List Timecard
        Events endpoint.
      operationId: UpdateTimecard
      x-api-path-slug: v1metimecardstimecard-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: timecard_id
        description: TThe ID of the timecard to modify
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Timecards
      - Details
      - ""
      - This
      - Creates
      - EDIT
      - Eventthe
      - Timecard
      - ""
      - You
      - Can
      - View
      - Timecards
      - Event
      - History
      - List
      - Timecard
      - Events
      - Endpoint
  /v1/me/timecards/{timecard_id}/events:
    get:
      summary: Provides summary information for all events associated with a particular
        timecard.
      description: Provides summary information for all events associated with a particular
        timecard.
      operationId: ListTimecardEvents
      x-api-path-slug: v1metimecardstimecard-idevents-get
      parameters:
      - in: path
        name: timecard_id
        description: The ID of the timecard to list events for
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Events
      - Associated
      - Particular
      - Timecard
  /v1/{location_id}/bank-accounts:
    get:
      summary: Provides non-confidential details for all of a location's associated
        bank accounts. This endpoint does not provide full bank account numbers, and
        there is no way to obtain a full bank account number with the Connect API.
      description: Provides non-confidential details for all of a location's associated
        bank accounts. This endpoint does not provide full bank account numbers, and
        there is no way to obtain a full bank account number with the Connect API.
      operationId: ListBankAccounts
      x-api-path-slug: v1location-idbankaccounts-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list bank accounts for
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Non-confidential
      - Details
      - Of
      - Locations
      - Associated
      - Bank
      - Accounts
      - ""
      - This
      - Endpoint
      - Does
      - Not
      - Provide
      - Full
      - Bank
      - Account
      - Numbers
      - ""
      - There
      - Is
      - "No"
      - Way
      - To
      - Obtain
      - Full
      - Bank
      - Account
      - Number
      - Connect
  /v1/{location_id}/bank-accounts/{bank_account_id}:
    get:
      summary: Provides non-confidential details for a merchant's associated bank
        account. This endpoint does not provide full bank account numbers, and there
        is no way to obtain a full bank account number with the Connect API.
      description: Provides non-confidential details for a merchant's associated bank
        account. This endpoint does not provide full bank account numbers, and there
        is no way to obtain a full bank account number with the Connect API.
      operationId: RetrieveBankAccount
      x-api-path-slug: v1location-idbankaccountsbank-account-id-get
      parameters:
      - in: path
        name: bank_account_id
        description: The bank accounts Square-issued ID
      - in: path
        name: location_id
        description: The ID of the bank accounts associated location
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Non-confidential
      - Detailsa
      - Merchants
      - Associated
      - Bank
      - Account
      - ""
      - This
      - Endpoint
      - Does
      - Not
      - Provide
      - Full
      - Bank
      - Account
      - Numbers
      - ""
      - There
      - Is
      - "No"
      - Way
      - To
      - Obtain
      - Full
      - Bank
      - Account
      - Number
      - Connect
  /v1/{location_id}/cash-drawer-shifts:
    get:
      summary: Provides the details for all of a location's cash drawer shifts during
        a date range. The date range you specify cannot exceed 90 days.
      description: Provides the details for all of a location's cash drawer shifts
        during a date range. The date range you specify cannot exceed 90 days.
      operationId: ListCashDrawerShifts
      x-api-path-slug: v1location-idcashdrawershifts-get
      parameters:
      - in: query
        name: begin_time
        description: The beginning of the requested reporting period, in ISO 8601
          format
      - in: query
        name: end_time
        description: The beginning of the requested reporting period, in ISO 8601
          format
      - in: path
        name: location_id
        description: The ID of the location to list cash drawer shifts for
      - in: query
        name: order
        description: The order in which cash drawer shifts are listed in the response,
          based on their created_at field
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Details
      - Of
      - Locations
      - Cash
      - Drawer
      - Shifts
      - During
      - Date
      - Range
      - ""
      - Date
      - Range
      - You
      - Specify
      - Cannot
      - Exceed
      - "90"
      - Days
  /v1/{location_id}/cash-drawer-shifts/{shift_id}:
    get:
      summary: Provides the details for a single cash drawer shift, including all
        events that occurred during the shift.
      description: Provides the details for a single cash drawer shift, including
        all events that occurred during the shift.
      operationId: RetrieveCashDrawerShift
      x-api-path-slug: v1location-idcashdrawershiftsshift-id-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list cash drawer shifts for
      - in: path
        name: shift_id
        description: The shifts ID
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Detailsa
      - Single
      - Cash
      - Drawer
      - Shift
      - ""
      - Including
      - ""
      - Events
      - That
      - Occurred
      - During
      - Shift
  /v1/{location_id}/categories:
    get:
      summary: Lists all of a location's item categories.
      description: Lists all of a location's item categories.
      operationId: ListCategories
      x-api-path-slug: v1location-idcategories-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list categories for
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Locations
      - Item
      - Categories
    post:
      summary: Creates an item category.
      description: Creates an item category.
      operationId: CreateCategory
      x-api-path-slug: v1location-idcategories-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to create an item for
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Item
      - Category
  /v1/{location_id}/categories/{category_id}:
    delete:
      summary: Deletes an existing item category.
      description: Deletes an existing item category.
      operationId: DeleteCategory
      x-api-path-slug: v1location-idcategoriescategory-id-delete
      parameters:
      - in: path
        name: category_id
        description: The ID of the category to delete
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - Category
    put:
      summary: Modifies the details of an existing item category.
      description: Modifies the details of an existing item category.
      operationId: UpdateCategory
      x-api-path-slug: v1location-idcategoriescategory-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: category_id
        description: The ID of the category to edit
      - in: path
        name: location_id
        description: The ID of the categorys associated location
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Item
      - Category
  /v1/{location_id}/discounts:
    get:
      summary: Lists all of a location's discounts.
      description: Lists all of a location's discounts.
      operationId: ListDiscounts
      x-api-path-slug: v1location-iddiscounts-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list categories for
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Locations
      - Discounts
    post:
      summary: Creates a discount.
      description: Creates a discount.
      operationId: CreateDiscount
      x-api-path-slug: v1location-iddiscounts-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to create an item for
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Discount
  /v1/{location_id}/discounts/{discount_id}:
    delete:
      summary: Deletes an existing discount.
      description: Deletes an existing discount.
      operationId: DeleteDiscount
      x-api-path-slug: v1location-iddiscountsdiscount-id-delete
      parameters:
      - in: path
        name: discount_id
        description: The ID of the discount to delete
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Discount
    put:
      summary: Modifies the details of an existing discount.
      description: Modifies the details of an existing discount.
      operationId: UpdateDiscount
      x-api-path-slug: v1location-iddiscountsdiscount-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: discount_id
        description: The ID of the discount to edit
      - in: path
        name: location_id
        description: The ID of the categorys associated location
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Discount
  /v1/{location_id}/fees:
    get:
      summary: Lists all of a location's fees (taxes).
      description: Lists all of a location's fees (taxes).
      operationId: ListFees
      x-api-path-slug: v1location-idfees-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list fees for
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Locations
      - Fees
      - (taxes)
    post:
      summary: Creates a fee (tax).
      description: Creates a fee (tax).
      operationId: CreateFee
      x-api-path-slug: v1location-idfees-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to create a fee for
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Fee
      - (tax)
  /v1/{location_id}/fees/{fee_id}:
    delete:
      summary: Deletes an existing fee (tax).
      description: Deletes an existing fee (tax).
      operationId: DeleteFee
      x-api-path-slug: v1location-idfeesfee-id-delete
      parameters:
      - in: path
        name: fee_id
        description: The ID of the fee to delete
      - in: path
        name: location_id
        description: The ID of the fees associated location
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Fee
      - (tax)
    put:
      summary: Modifies the details of an existing fee (tax).
      description: Modifies the details of an existing fee (tax).
      operationId: UpdateFee
      x-api-path-slug: v1location-idfeesfee-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: fee_id
        description: The ID of the fee to edit
      - in: path
        name: location_id
        description: The ID of the fees associated location
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Fee
      - (tax)
  /v1/{location_id}/inventory:
    get:
      summary: Provides inventory information for all of a merchant's inventory-enabled
        item variations.
      description: Provides inventory information for all of a merchant's inventory-enabled
        item variations.
      operationId: ListInventory
      x-api-path-slug: v1location-idinventory-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: limit
        description: The maximum number of inventory entries to return in a single
          response
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Inventory
      - Information
      - Of
      - Merchants
      - Inventory-enabled
      - Item
      - Variations
  /v1/{location_id}/inventory/{variation_id}:
    post:
      summary: Adjusts an item variation's current available inventory.
      description: Adjusts an item variation's current available inventory.
      operationId: AdjustInventory
      x-api-path-slug: v1location-idinventoryvariation-id-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: variation_id
        description: The ID of the variation to adjust inventory information for
      responses:
        200:
          description: OK
      tags:
      - Adjusts
      - Item
      - Variations
      - Current
      - Available
      - Inventory
  /v1/{location_id}/items:
    get:
      summary: Provides summary information for all of a location's items.
      description: Provides summary information for all of a location's items.
      operationId: ListItems
      x-api-path-slug: v1location-iditems-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: path
        name: location_id
        description: The ID of the location to list items for
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Of
      - Locations
      - Items
    post:
      summary: Creates an item and at least one variation for it.
      description: Creates an item and at least one variation for it.
      operationId: CreateItem
      x-api-path-slug: v1location-iditems-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to create an item for
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Item
      - At
      - Least
      - Variationit
  /v1/{location_id}/items/{item_id}:
    delete:
      summary: Deletes an existing item and all item variations associated with it.
      description: Deletes an existing item and all item variations associated with
        it.
      operationId: DeleteItem
      x-api-path-slug: v1location-iditemsitem-id-delete
      parameters:
      - in: path
        name: item_id
        description: The ID of the item to modify
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - ""
      - Item
      - Variations
      - Associated
      - It
    get:
      summary: Provides the details for a single item, including associated modifier
        lists and fees.
      description: Provides the details for a single item, including associated modifier
        lists and fees.
      operationId: RetrieveItem
      x-api-path-slug: v1location-iditemsitem-id-get
      parameters:
      - in: path
        name: item_id
        description: The items ID
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Detailsa
      - Single
      - Item
      - ""
      - Including
      - Associated
      - Modifier
      - Lists
      - Fees
    put:
      summary: Modifies the core details of an existing item.
      description: Modifies the core details of an existing item.
      operationId: UpdateItem
      x-api-path-slug: v1location-iditemsitem-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: item_id
        description: The ID of the item to modify
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Core
      - Details
      - Of
      - Existing
      - Item
  /v1/{location_id}/items/{item_id}/fees/{fee_id}:
    delete:
      summary: Removes a fee assocation from an item, meaning the fee is no longer
        automatically applied to the item in Square Register.
      description: Removes a fee assocation from an item, meaning the fee is no longer
        automatically applied to the item in Square Register.
      operationId: RemoveFee
      x-api-path-slug: v1location-iditemsitem-idfeesfee-id-delete
      parameters:
      - in: path
        name: fee_id
        description: The ID of the fee to apply
      - in: path
        name: item_id
        description: The ID of the item to add the fee to
      - in: path
        name: location_id
        description: The ID of the fees associated location
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Fee
      - Assocation
      - From
      - Item
      - ""
      - Meaning
      - Fee
      - Is
      - "No"
      - Longer
      - Automatically
      - Applied
      - To
      - Item
      - In
      - Square
      - Register
    put:
      summary: Associates a fee with an item, meaning the fee is automatically applied
        to the item in Square Register.
      description: Associates a fee with an item, meaning the fee is automatically
        applied to the item in Square Register.
      operationId: ApplyFee
      x-api-path-slug: v1location-iditemsitem-idfeesfee-id-put
      parameters:
      - in: path
        name: fee_id
        description: The ID of the fee to apply
      - in: path
        name: item_id
        description: The ID of the item to add the fee to
      - in: path
        name: location_id
        description: The ID of the fees associated location
      responses:
        200:
          description: OK
      tags:
      - Associates
      - Fee
      - Item
      - ""
      - Meaning
      - Fee
      - Is
      - Automatically
      - Applied
      - To
      - Item
      - In
      - Square
      - Register
  /v1/{location_id}/items/{item_id}/modifier-lists/{modifier_list_id}:
    delete:
      summary: Removes a modifier list association from an item, meaning modifier
        options from the list can no longer be applied to the item.
      description: Removes a modifier list association from an item, meaning modifier
        options from the list can no longer be applied to the item.
      operationId: RemoveModifierList
      x-api-path-slug: v1location-iditemsitem-idmodifierlistsmodifier-list-id-delete
      parameters:
      - in: path
        name: item_id
        description: The ID of the item to remove the modifier list from
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to remove
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Modifier
      - List
      - Association
      - From
      - Item
      - ""
      - Meaning
      - Modifier
      - Options
      - From
      - List
      - Can
      - "No"
      - Longer
      - Be
      - Applied
      - To
      - Item
    put:
      summary: Associates a modifier list with an item, meaning modifier options from
        the list can be applied to the item.
      description: Associates a modifier list with an item, meaning modifier options
        from the list can be applied to the item.
      operationId: ApplyModifierList
      x-api-path-slug: v1location-iditemsitem-idmodifierlistsmodifier-list-id-put
      parameters:
      - in: path
        name: item_id
        description: The ID of the item to add the modifier list to
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to apply
      responses:
        200:
          description: OK
      tags:
      - Associates
      - Modifier
      - List
      - Item
      - ""
      - Meaning
      - Modifier
      - Options
      - From
      - List
      - Can
      - Be
      - Applied
      - To
      - Item
  /v1/{location_id}/items/{item_id}/variations:
    post:
      summary: Creates an item variation for an existing item.
      description: Creates an item variation for an existing item.
      operationId: CreateVariation
      x-api-path-slug: v1location-iditemsitem-idvariations-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: item_id
        description: The items ID
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Item
      - Variationan
      - Existing
      - Item
  /v1/{location_id}/items/{item_id}/variations/{variation_id}:
    delete:
      summary: Deletes an existing item variation from an item.
      description: Deletes an existing item variation from an item.
      operationId: DeleteVariation
      x-api-path-slug: v1location-iditemsitem-idvariationsvariation-id-delete
      parameters:
      - in: path
        name: item_id
        description: The ID of the item to delete
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: variation_id
        description: The ID of the variation to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - Variation
      - From
      - Item
    put:
      summary: Modifies the details of an existing item variation.
      description: Modifies the details of an existing item variation.
      operationId: UpdateVariation
      x-api-path-slug: v1location-iditemsitem-idvariationsvariation-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: item_id
        description: The ID of the item to modify
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: variation_id
        description: The ID of the variation to modify
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Item
      - Variation
  /v1/{location_id}/modifier-lists:
    get:
      summary: Lists all of a location's modifier lists.
      description: Lists all of a location's modifier lists.
      operationId: ListModifierLists
      x-api-path-slug: v1location-idmodifierlists-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list modifier lists for
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Locations
      - Modifier
      - Lists
    post:
      summary: Creates an item modifier list and at least one modifier option for
        it.
      description: Creates an item modifier list and at least one modifier option
        for it.
      operationId: CreateModifierList
      x-api-path-slug: v1location-idmodifierlists-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to create a modifier list for
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Item
      - Modifier
      - List
      - At
      - Least
      - Modifier
      - Optionit
  /v1/{location_id}/modifier-lists/{modifier_list_id}:
    delete:
      summary: Deletes an existing item modifier list and all modifier options associated
        with it.
      description: Deletes an existing item modifier list and all modifier options
        associated with it.
      operationId: DeleteModifierList
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-id-delete
      parameters:
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - Modifier
      - List
      - ""
      - Modifier
      - Options
      - Associated
      - It
    get:
      summary: Provides the details for a single modifier list.
      description: Provides the details for a single modifier list.
      operationId: RetrieveModifierList
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-id-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The modifier lists ID
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Detailsa
      - Single
      - Modifier
      - List
    put:
      summary: Modifies the details of an existing item modifier list.
      description: Modifies the details of an existing item modifier list.
      operationId: UpdateModifierList
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to edit
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Item
      - Modifier
      - List
  /v1/{location_id}/modifier-lists/{modifier_list_id}/modifier-options:
    post:
      summary: Creates an item modifier option and adds it to a modifier list.
      description: Creates an item modifier option and adds it to a modifier list.
      operationId: CreateModifierOption
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-idmodifieroptions-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to edit
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Item
      - Modifier
      - Option
      - Adds
      - It
      - To
      - Modifier
      - List
  /v1/{location_id}/modifier-lists/{modifier_list_id}/modifier-options/{modifier_option_id}:
    delete:
      summary: Deletes an existing item modifier option from a modifier list.
      description: Deletes an existing item modifier option from a modifier list.
      operationId: DeleteModifierOption
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-idmodifieroptionsmodifier-option-id-delete
      parameters:
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to delete
      - in: path
        name: modifier_option_id
        description: The ID of the modifier list to edit
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - Modifier
      - Option
      - From
      - Modifier
      - List
    put:
      summary: Modifies the details of an existing item modifier option.
      description: Modifies the details of an existing item modifier option.
      operationId: UpdateModifierOption
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-idmodifieroptionsmodifier-option-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to edit
      - in: path
        name: modifier_option_id
        description: The ID of the modifier list to edit
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Existing
      - Item
      - Modifier
      - Option
  /v1/{location_id}/orders:
    get:
      summary: Provides summary information for a merchant's online store orders.
      description: Provides summary information for a merchant's online store orders.
      operationId: ListOrders
      x-api-path-slug: v1location-idorders-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: limit
        description: The maximum number of payments to return in a single response
      - in: path
        name: location_id
        description: The ID of the location to list online store orders for
      - in: query
        name: order
        description: TThe order in which payments are listed in the response
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Informationa
      - Merchants
      - Online
      - Store
      - Orders
  /v1/{location_id}/orders/{order_id}:
    get:
      summary: Provides comprehensive information for a single online store order,
        including the order's history.
      description: Provides comprehensive information for a single online store order,
        including the order's history.
      operationId: RetrieveOrder
      x-api-path-slug: v1location-idordersorder-id-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the orders associated location
      - in: path
        name: order_id
        description: The orders Square-issued ID
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Comprehensive
      - Informationa
      - Single
      - Online
      - Store
      - Order
      - ""
      - Including
      - Orders
      - History
    put:
      summary: 'Updates the details of an online store order. Every update you perform
        on an order corresponds to one of three actions:'
      description: 'Updates the details of an online store order. Every update you
        perform on an order corresponds to one of three actions:'
      operationId: UpdateOrder
      x-api-path-slug: v1location-idordersorder-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the orders associated location
      - in: path
        name: order_id
        description: The orders Square-issued ID
      responses:
        200:
          description: OK
      tags:
      - S
      - Details
      - Of
      - Online
      - Store
      - Order
      - ""
      - Every
      - Update
      - You
      - Perform
      - "On"
      - Order
      - Corresponds
      - To
      - Of
      - Three
      - 'Actions:'
  /v1/{location_id}/pages:
    get:
      summary: Lists all of a location's Favorites pages in Square Register.
      description: Lists all of a location's Favorites pages in Square Register.
      operationId: ListPages
      x-api-path-slug: v1location-idpages-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list Favorites pages for
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Locations
      - Favorites
      - Pages
      - In
      - Square
      - Register
    post:
      summary: Creates a Favorites page in Square Register.
      description: Creates a Favorites page in Square Register.
      operationId: CreatePage
      x-api-path-slug: v1location-idpages-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to create an item for
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Favorites
      - Page
      - In
      - Square
      - Register
  /v1/{location_id}/pages/{page_id}:
    delete:
      summary: Deletes an existing Favorites page and all of its cells.
      description: Deletes an existing Favorites page and all of its cells.
      operationId: DeletePage
      x-api-path-slug: v1location-idpagespage-id-delete
      parameters:
      - in: path
        name: location_id
        description: The ID of the Favorites pages associated location
      - in: path
        name: page_id
        description: The ID of the page to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Favorites
      - Page
      - ""
      - Of
      - Its
      - Cells
    put:
      summary: Modifies the details of a Favorites page in Square Register.
      description: Modifies the details of a Favorites page in Square Register.
      operationId: UpdatePage
      x-api-path-slug: v1location-idpagespage-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the Favorites pages associated location
      - in: path
        name: page_id
        description: The ID of the page to modify
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Favorites
      - Page
      - In
      - Square
      - Register
  /v1/{location_id}/pages/{page_id}/cells:
    delete:
      summary: Deletes a cell from a Favorites page in Square Register.
      description: Deletes a cell from a Favorites page in Square Register.
      operationId: DeletePageCell
      x-api-path-slug: v1location-idpagespage-idcells-delete
      parameters:
      - in: query
        name: column
        description: The column of the cell to clear
      - in: path
        name: location_id
        description: The ID of the Favorites pages associated location
      - in: path
        name: page_id
        description: The ID of the page to delete
      - in: query
        name: row
        description: The row of the cell to clear
      responses:
        200:
          description: OK
      tags:
      - S
      - Cell
      - From
      - Favorites
      - Page
      - In
      - Square
      - Register
    put:
      summary: Modifies a cell of a Favorites page in Square Register.
      description: Modifies a cell of a Favorites page in Square Register.
      operationId: UpdatePageCell
      x-api-path-slug: v1location-idpagespage-idcells-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the Favorites pages associated location
      - in: path
        name: page_id
        description: The ID of the page the cell belongs to
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Cell
      - Of
      - Favorites
      - Page
      - In
      - Square
      - Register
  /v1/{location_id}/payments:
    get:
      summary: Provides summary information for all payments taken by a merchant or
        any of the merchant's mobile staff during a date range. Date ranges cannot
        exceed one year in length. See Date ranges for details of inclusive and exclusive
        dates.
      description: Provides summary information for all payments taken by a merchant
        or any of the merchant's mobile staff during a date range. Date ranges cannot
        exceed one year in length. See Date ranges for details of inclusive and exclusive
        dates.
      operationId: ListPayments
      x-api-path-slug: v1location-idpayments-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: begin_time
        description: The beginning of the requested reporting period, in ISO 8601
          format
      - in: query
        name: end_time
        description: The end of the requested reporting period, in ISO 8601 format
      - in: query
        name: limit
        description: The maximum number of payments to return in a single response
      - in: path
        name: location_id
        description: The ID of the location to list payments for
      - in: query
        name: order
        description: The order in which payments are listed in the response
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Payments
      - Taken
      - By
      - Merchant
      - Any
      - Of
      - Merchants
      - Mobile
      - Staff
      - During
      - Date
      - Range
      - ""
      - Date
      - Ranges
      - Cannot
      - Exceed
      - Year
      - In
      - Length
      - ""
      - See
      - Date
      - Rangesdetails
      - Of
      - Inclusive
      - Exclusive
      - Dates
  /v1/{location_id}/payments/{payment_id}:
    get:
      summary: Provides comprehensive information for a single payment.
      description: Provides comprehensive information for a single payment.
      operationId: RetrievePayment
      x-api-path-slug: v1location-idpaymentspayment-id-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the payments associated location
      - in: path
        name: payment_id
        description: The payments Square-issued ID
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Comprehensive
      - Informationa
      - Single
      - Payment
  /v1/{location_id}/refunds:
    get:
      summary: Provides the details for all refunds initiated by a merchant or any
        of the merchant's mobile staff during a date range. Date ranges cannot exceed
        one year in length.
      description: Provides the details for all refunds initiated by a merchant or
        any of the merchant's mobile staff during a date range. Date ranges cannot
        exceed one year in length.
      operationId: v1.location_id.refunds.get
      x-api-path-slug: v1location-idrefunds-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: begin_time
        description: The beginning of the requested reporting period, in ISO 8601
          format
      - in: query
        name: end_time
        description: The end of the requested reporting period, in ISO 8601 format
      - in: query
        name: limit
        description: The maximum number of payments to return in a single response
      - in: path
        name: location_id
        description: The ID of the location to list refunds for
      - in: query
        name: order
        description: TThe order in which payments are listed in the response
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Details
      - Refunds
      - Initiated
      - By
      - Merchant
      - Any
      - Of
      - Merchants
      - Mobile
      - Staff
      - During
      - Date
      - Range
      - ""
      - Date
      - Ranges
      - Cannot
      - Exceed
      - Year
      - In
      - Length
    post:
      summary: Issues a refund for a previously processed payment. You must issue
        a refund within 60 days of the associated payment.
      description: Issues a refund for a previously processed payment. You must issue
        a refund within 60 days of the associated payment.
      operationId: v1.location_id.refunds.post
      x-api-path-slug: v1location-idrefunds-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the original payments associated location
      responses:
        200:
          description: OK
      tags:
      - Issues
      - Refunda
      - Previously
      - Processed
      - Payment
      - ""
      - You
      - Must
      - Issue
      - Refund
      - Within
      - "60"
      - Days
      - Of
      - Associated
      - Payment
  /v1/{location_id}/settlements:
    get:
      summary: Provides summary information for all deposits and withdrawals initiated
        by Square to a merchant's bank account during a date range. Date ranges cannot
        exceed one year in length.
      description: Provides summary information for all deposits and withdrawals initiated
        by Square to a merchant's bank account during a date range. Date ranges cannot
        exceed one year in length.
      operationId: ListSettlements
      x-api-path-slug: v1location-idsettlements-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: begin_time
        description: The beginning of the requested reporting period, in ISO 8601
          format
      - in: query
        name: end_time
        description: The end of the requested reporting period, in ISO 8601 format
      - in: query
        name: limit
        description: The maximum number of payments to return in a single response
      - in: path
        name: location_id
        description: The ID of the location to list settlements for
      - in: query
        name: order
        description: TThe order in which payments are listed in the response
      - in: query
        name: status
        description: Provide this parameter to retrieve only settlements with a particular
          status (SENT or FAILED)
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Deposits
      - Withdrawals
      - Initiated
      - By
      - Square
      - To
      - Merchants
      - Bank
      - Account
      - During
      - Date
      - Range
      - ""
      - Date
      - Ranges
      - Cannot
      - Exceed
      - Year
      - In
      - Length
  /v1/{location_id}/settlements/{settlement_id}:
    get:
      summary: Provides comprehensive information for a single settlement, including
        the entries that contribute to the settlement's total.
      description: Provides comprehensive information for a single settlement, including
        the entries that contribute to the settlement's total.
      operationId: RetrieveSettlement
      x-api-path-slug: v1location-idsettlementssettlement-id-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the settlementss associated location
      - in: path
        name: settlement_id
        description: The settlements Square-issued ID
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Comprehensive
      - Informationa
      - Single
      - Settlement
      - ""
      - Including
      - Entries
      - That
      - Contribute
      - To
      - Settlements
      - Total
  /v2/catalog/batch-delete:
    post:
      summary: BatchDeleteCatalogObjects
      description: |-
        Deletes a set of [CatalogItem](#type-catalogitem)s based on the
        provided list of target IDs and returns a set of successfully deleted IDs in
        the response. Deletion is a cascading event such that all children of the
        targeted object are also deleted. For example, deleting a CatalogItem will
        also delete all of its [CatalogItemVariation](#type-catalogitemvariation)
        children.

        `BatchDeleteCatalogObjects` succeeds even if only a portion of the targeted
        IDs can be deleted. The response will only include IDs that were
        actually deleted.
      operationId: BatchDeleteCatalogObjects
      x-api-path-slug: v2catalogbatchdelete-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - BatchCatalogObjects
  /v2/catalog/batch-retrieve:
    post:
      summary: BatchRetrieveCatalogObjects
      description: |-
        Returns a set of objects based on the provided ID.
        Each [CatalogItem](#type-catalogitem) returned in the set includes all of its
        child information including: all of its
        [CatalogItemVariation](#type-catalogitemvariation) objects, references to
        its [CatalogModifierList](#type-catalogmodifierlist) objects, and the ids of
        any [CatalogTax](#type-catalogtax) objects that apply to it.
      operationId: BatchRetrieveCatalogObjects
      x-api-path-slug: v2catalogbatchretrieve-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - BatchRetrieveCatalogObjects
  /v2/catalog/batch-upsert:
    post:
      summary: BatchUpsertCatalogObjects
      description: |-
        Creates or updates up to 10,000 target objects based on the provided
        list of objects. The target objects are grouped into batches and each batch is
        inserted/updated in an all-or-nothing manner. If an object within a batch is
        malformed in some way, or violates a database constraint, the entire batch
        containing that item will be disregarded. However, other batches in the same
        request may still succeed. Each batch may contain up to 1,000 objects, and
        batches will be processed in order as long as the total object count for the
        request (items, variations, modifier lists, discounts, and taxes) is no more
        than 10,000.
      operationId: BatchUpsertCatalogObjects
      x-api-path-slug: v2catalogbatchupsert-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - BatchUpsertCatalogObjects
  /v2/catalog/info:
    get:
      summary: CatalogInfo
      description: |-
        Returns information about the Square Catalog API, such as batch size
        limits for `BatchUpsertCatalogObjects`.
      operationId: CatalogInfo
      x-api-path-slug: v2cataloginfo-get
      responses:
        200:
          description: OK
      tags:
      - CatalogInfo
  /v2/catalog/list:
    get:
      summary: ListCatalog
      description: |-
        Returns a list of [CatalogObject](#type-catalogobject)s that includes
        all objects of a set of desired types (for example, all [CatalogItem](#type-catalogitem)
        and [CatalogTax](#type-catalogtax) objects) in the catalog. The types parameter
        is specified as a comma-separated list of valid [CatalogObject](#type-catalogobject) types:
        `ITEM`, `ITEM_VARIATION`, `MODIFIER`, `MODIFIER_LIST`, `CATEGORY`, `DISCOUNT`, `TAX`.
      operationId: ListCatalog
      x-api-path-slug: v2cataloglist-get
      parameters:
      - in: query
        name: cursor
        description: The pagination cursor returned in the previous response
      - in: query
        name: types
        description: An optional case-insensitive, comma-separated list of object
          types to retrieve, for example`ITEM,ITEM_VARIATION,CATEGORY`
      responses:
        200:
          description: OK
      tags:
      - ListCatalog
  /v2/catalog/object:
    post:
      summary: UpsertCatalogObject
      description: Creates or updates the target [CatalogObject](#type-catalogobject).
      operationId: UpsertCatalogObject
      x-api-path-slug: v2catalogobject-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - UpsertCatalogObject
  /v2/catalog/object/{object_id}:
    delete:
      summary: DeleteCatalogObject
      description: |-
        Deletes a single [CatalogObject](#type-catalogobject) based on the
        provided ID and returns the set of successfully deleted IDs in the response.
        Deletion is a cascading event such that all children of the targeted object
        are also deleted. For example, deleting a [CatalogItem](#type-catalogitem)
        will also delete all of its
        [CatalogItemVariation](#type-catalogitemvariation) children.
      operationId: DeleteCatalogObject
      x-api-path-slug: v2catalogobjectobject-id-delete
      parameters:
      - in: path
        name: object_id
        description: The ID of the [CatalogObject](#type-catalogobject) to be deleted
      responses:
        200:
          description: OK
      tags:
      - CatalogObject
    get:
      summary: RetrieveCatalogObject
      description: |-
        Returns a single [CatalogItem](#type-catalogitem) as a
        [CatalogObject](#type-catalogobject) based on the provided ID. The returned
        object includes all of the relevant [CatalogItem](#type-catalogitem)
        information including: [CatalogItemVariation](#type-catalogitemvariation)
        children, references to its
        [CatalogModifierList](#type-catalogmodifierlist) objects, and the ids of
        any [CatalogTax](#type-catalogtax) objects that apply to it.
      operationId: RetrieveCatalogObject
      x-api-path-slug: v2catalogobjectobject-id-get
      parameters:
      - in: query
        name: include_related_objects
        description: If `true`, the response will include additional objects that
          are related to therequested object, as follows:If the `object` field of
          the response contains a [CatalogItem](#type-catalogitem),its associated
          [CatalogCategory](#type-catalogcategory), [CatalogTax](#type-catalogtax)es,
          and[CatalogModifierList](#type-catalogmodifierlist)s will be returned in
          the `related_objects` field of theresponse
      - in: path
        name: object_id
        description: The object ID of any type of [CatalogObject](#type-catalogobject)s
          to be retrieved
      responses:
        200:
          description: OK
      tags:
      - RetrieveCatalogObject
  /v2/catalog/search:
    post:
      summary: SearchCatalogObjects
      description: |-
        Queries the targeted catalog using a variety of query types
        ([CatalogQuerySortedAttribute](#type-catalogquerysortedattribute),
        ([CatalogQueryExact](#type-catalogqueryexact),
        ([CatalogQueryRange](#type-catalogqueryrange),
        ([CatalogQueryText](#type-catalogquerytext),
        ([CatalogQueryItemsForTax](#type-catalogqueryitemsfortax),
        ([CatalogQueryItemsForModifierList](#type-catalogqueryitemsformodifierlist)).
      operationId: SearchCatalogObjects
      x-api-path-slug: v2catalogsearch-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - SearchCatalogObjects
  /v2/catalog/update-item-modifier-lists:
    post:
      summary: UpdateItemModifierLists
      description: |-
        Updates the [CatalogModifierList](#type-catalogmodifierlist) objects
        that apply to the targeted [CatalogItem](#type-catalogitem) without having
        to perform an upsert on the entire item.
      operationId: UpdateItemModifierLists
      x-api-path-slug: v2catalogupdateitemmodifierlists-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - ItemModifierLists
  /v2/catalog/update-item-taxes:
    post:
      summary: UpdateItemTaxes
      description: |-
        Updates the [CatalogTax](#type-catalogtax) objects that apply to the
        targeted [CatalogItem](#type-catalogitem) without having to perform an
        upsert on the entire item.
      operationId: UpdateItemTaxes
      x-api-path-slug: v2catalogupdateitemtaxes-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - ItemTaxes
  /v2/customers:
    get:
      summary: ListCustomers
      description: Lists a business's customers.
      operationId: ListCustomers
      x-api-path-slug: v2customers-get
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: query
        name: cursor
        description: A pagination cursor returned by a previous call to this endpoint
      responses:
        200:
          description: OK
      tags:
      - ListCustomers
    post:
      summary: CreateCustomer
      description: |-
        Creates a new customer for a business, which can have associated cards on file.

        You must provide __at least one__ of the following values in your request to this
        endpoint:

        - `given_name`
        - `family_name`
        - `company_name`
        - `email_address`
        - `phone_number`

        This endpoint does not accept an idempotency key. If you accidentally create
        a duplicate customer, you can delete it with the
        [DeleteCustomer](#endpoint-deletecustomer) endpoint.
      operationId: CreateCustomer
      x-api-path-slug: v2customers-post
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - CreateCustomer
  /v2/customers/{customer_id}:
    delete:
      summary: DeleteCustomer
      description: Deletes a customer from a business, along with any linked cards
        on file.
      operationId: DeleteCustomer
      x-api-path-slug: v2customerscustomer-id-delete
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: path
        name: customer_id
        description: The ID of the customer to delete
      responses:
        200:
          description: OK
      tags:
      - Customer
    get:
      summary: RetrieveCustomer
      description: Returns details for a single customer.
      operationId: RetrieveCustomer
      x-api-path-slug: v2customerscustomer-id-get
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: path
        name: customer_id
        description: The ID of the customer to retrieve
      responses:
        200:
          description: OK
      tags:
      - RetrieveCustomer
    put:
      summary: UpdateCustomer
      description: |-
        Updates the details of an existing customer.
        The ID of the customer may change if the customer has been merged into another customer.

        You cannot edit a customer's cards on file with this endpoint. To make changes
        to a card on file, you must delete the existing card on file with the
        [DeleteCustomerCard](#endpoint-deletecustomercard) endpoint, then create a new one with the
        [CreateCustomerCard](#endpoint-createcustomercard) endpoint.
      operationId: UpdateCustomer
      x-api-path-slug: v2customerscustomer-id-put
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customer_id
        description: The ID of the customer to update
      responses:
        200:
          description: OK
      tags:
      - Customer
  /v2/customers/{customer_id}/cards:
    post:
      summary: CreateCustomerCard
      description: |-
        Adds a card on file to an existing customer. In the United States
        Square takes care of automatically updating any cards on file that might
        have expired since you first attached them to a customer.
      operationId: CreateCustomerCard
      x-api-path-slug: v2customerscustomer-idcards-post
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customer_id
        description: The ID of the customer to link the card on file to
      responses:
        200:
          description: OK
      tags:
      - CreateCustomerCard
  /v2/customers/{customer_id}/cards/{card_id}:
    delete:
      summary: DeleteCustomerCard
      description: Removes a card on file from a customer.
      operationId: DeleteCustomerCard
      x-api-path-slug: v2customerscustomer-idcardscard-id-delete
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: path
        name: card_id
        description: The ID of the card on file to delete
      - in: path
        name: customer_id
        description: The ID of the customer that the card on file belongs to
      responses:
        200:
          description: OK
      tags:
      - CustomerCard
  /v2/locations:
    get:
      summary: ListLocations
      description: |-
        Provides the details for all of a business's locations.

        Most other Connect API endpoints have a required `location_id` path parameter.
        The `id` field of the [`Location`](#type-location) objects returned by this
        endpoint correspond to that `location_id` parameter.
      operationId: v2.locations.get
      x-api-path-slug: v2locations-get
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      responses:
        200:
          description: OK
      tags:
      - ListLocations
  /v2/locations/{location_id}/checkouts:
    post:
      summary: CreateCheckout
      description: |-
        Creates a [Checkout](#type-checkout) response that links a
        `checkoutId` and `checkout_page_url` that customers can be directed to in
        order to provide their payment information using a payment processing
        workflow hosted on connect.squareup.com.
      operationId: CreateCheckout
      x-api-path-slug: v2locationslocation-idcheckouts-post
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the business location to associate the checkout with
      responses:
        200:
          description: OK
      tags:
      - CreateCheckout
  /v2/locations/{location_id}/refunds:
    get:
      summary: ListRefunds
      description: |-
        Lists refunds for one of a business's locations.

        Refunds with a `status` of `PENDING` are not currently included in this
        endpoint's response.

        Max results per [page](#paginatingresults): 50
      operationId: v2.locations.location_id.refunds.get
      x-api-path-slug: v2locationslocation-idrefunds-get
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: query
        name: begin_time
        description: The beginning of the requested reporting period, in RFC 3339
          format
      - in: query
        name: cursor
        description: A pagination cursor returned by a previous call to this endpoint
      - in: query
        name: end_time
        description: The end of the requested reporting period, in RFC 3339 format
      - in: path
        name: location_id
        description: The ID of the location to list refunds for
      - in: query
        name: sort_order
        description: The order in which results are listed in the response (`ASC`
          foroldest first, `DESC` for newest first)
      responses:
        200:
          description: OK
      tags:
      - ListRefunds
  /v2/locations/{location_id}/transactions:
    get:
      summary: ListTransactions
      description: |-
        Lists transactions for a particular location.

        Max results per [page](#paginatingresults): 50
      operationId: ListTransactions
      x-api-path-slug: v2locationslocation-idtransactions-get
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: query
        name: begin_time
        description: The beginning of the requested reporting period, in RFC 3339
          format
      - in: query
        name: cursor
        description: A pagination cursor returned by a previous call to this endpoint
      - in: query
        name: end_time
        description: The end of the requested reporting period, in RFC 3339 format
      - in: path
        name: location_id
        description: The ID of the location to list transactions for
      - in: query
        name: sort_order
        description: The order in which results are listed in the response (`ASC`
          foroldest first, `DESC` for newest first)
      responses:
        200:
          description: OK
      tags:
      - ListTransactions
    post:
      summary: Charge
      description: |-
        Charges a card represented by a card nonce or a customer's card on file.

        Your request to this endpoint must include _either_:

        - A value for the `card_nonce` parameter (to charge a card nonce generated
        with the `SqPaymentForm`)
        - Values for the `customer_card_id` and `customer_id` parameters (to charge
        a customer's card on file)

        In order for an e-commerce payment to potentially qualify for
        [Square chargeback protection](https://squareup.com/help/article/5394), you
        _must_ provide values for the following parameters in your request:

        - `buyer_email_address`
        - At least one of `billing_address` or `shipping_address`

        When this response is returned, the amount of Square's processing fee might not yet be
        calculated. To obtain the processing fee, wait about ten seconds and call
        [RetrieveTransaction](#endpoint-retrievetransaction). See the `processing_fee_money`
        field of each [Tender included](#type-tender) in the transaction.
      operationId: Charge
      x-api-path-slug: v2locationslocation-idtransactions-post
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to associate the created transaction with
      responses:
        200:
          description: OK
      tags:
      - Charge
  /v2/locations/{location_id}/transactions/{transaction_id}:
    get:
      summary: RetrieveTransaction
      description: Retrieves details for a single transaction.
      operationId: RetrieveTransaction
      x-api-path-slug: v2locationslocation-idtransactionstransaction-id-get
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: path
        name: location_id
        description: The ID of the transactions associated location
      - in: path
        name: transaction_id
        description: The ID of the transaction to retrieve
      responses:
        200:
          description: OK
      tags:
      - RetrieveTransaction
  /v2/locations/{location_id}/transactions/{transaction_id}/capture:
    post:
      summary: CaptureTransaction
      description: |-
        Captures a transaction that was created with the [Charge](#endpoint-charge)
        endpoint with a `delay_capture` value of `true`.

        See [Delayed capture transactions](/articles/delayed-capture-transactions/)
        for more information.
      operationId: CaptureTransaction
      x-api-path-slug: v2locationslocation-idtransactionstransaction-idcapture-post
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: path
        name: location_id
      - in: path
        name: transaction_id
      responses:
        200:
          description: OK
      tags:
      - CaptureTransaction
  /v2/locations/{location_id}/transactions/{transaction_id}/refund:
    post:
      summary: CreateRefund
      description: |-
        Initiates a refund for a previously charged tender.

        You must issue a refund within 120 days of the associated payment. See
        (this article)[https://squareup.com/help/us/en/article/5060] for more information
        on refund behavior.
      operationId: v2.locations.location_id.transactions.transaction_id.refund.post
      x-api-path-slug: v2locationslocation-idtransactionstransaction-idrefund-post
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the original transactions associated location
      - in: path
        name: transaction_id
        description: The ID of the original transaction that includes the tender to
          refund
      responses:
        200:
          description: OK
      tags:
      - CreateRefund
  /v2/locations/{location_id}/transactions/{transaction_id}/void:
    post:
      summary: VoidTransaction
      description: |-
        Cancels a transaction that was created with the [Charge](#endpoint-charge)
        endpoint with a `delay_capture` value of `true`.

        See [Delayed capture transactions](/articles/delayed-capture-transactions/)
        for more information.
      operationId: VoidTransaction
      x-api-path-slug: v2locationslocation-idtransactionstransaction-idvoid-post
      parameters:
      - in: header
        name: Authorization
        description: The value to provide in the Authorization header ofyour request
      - in: path
        name: location_id
      - in: path
        name: transaction_id
      responses:
        200:
          description: OK
      tags:
      - VoidTransaction