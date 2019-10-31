swagger: "2.0"
x-collection-name: Flowroute
x-complete: 1
info:
  title: Flowroute APIs
  description: the-flowroute-apis-are-organized-around-rest--our-apis-have-resourceoriented-urls-support-http-verbs-and-respond-with-http-status-codes--all-api-requests-and-responses-including-errors-will-be-represented-as-json-objects--you-can-use-the-flowroute-apis-to-manage-your-flowroute-phone-numbers-including-setting-primary-and-failover-routes-for-inbound-calls-and-sending-text-messages-sms-and-mms-using-longcode-or-tollfree-numbers-in-your-account-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2.1/messages:
    post:
      summary: Send a Message
      description: Sends an SMS or MMS from a Flowroute long code or toll-free phone
        number to another valid phone number.
      operationId: sends-an-sms-or-mms-from-a-flowroute-long-code-or-tollfree-phone-number-to-another-valid-phone-numbe
      x-api-path-slug: v2-1messages-post
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Send
      - Message
    get:
      summary: Look Up a Set of Messages
      description: Retrieves a list of Message Detail Records (MDRs) within a specified
        date range. Date and time is based on Coordinated Universal Time (UTC).
      operationId: retrieves-a-list-of-message-detail-records-mdrs-within-a-specified-date-range-date-and-time-is-based
      x-api-path-slug: v2-1messages-get
      parameters:
      - in: query
        name: end_date
        description: The ending date and time, in UTC, on which to perform an MDR
          search
      - in: query
        name: limit
        description: The number of MDRs to retrieve at one time
      - in: query
        name: offset
        description: The number of MDRs to skip when performing a query
      - in: query
        name: start_date
        description: The beginning date and time, in UTC, on which to perform an MDR
          search
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Look
      - Up
      - Set
      - Of
      - Messages
  /v2.1/messages/{id}:
    get:
      summary: Look Up a Message Detail Record
      description: Searches for a specific message record ID and returns a Message
        Detail Record (in MDR2 format).
      operationId: searches-for-a-specific-message-record-id-and-returns-a-message-detail-record-in-mdr2-format
      x-api-path-slug: v2-1messagesid-get
      parameters:
      - in: path
        name: id
        description: The unique message detail record identifier (MDR ID) of any message
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Look
      - Up
      - Message
      - Detail
      - Record
  /v2/numbers:
    get:
      summary: Account Phone Numbers
      description: Returns a list of all phone numbers currently on your Flowroute
        account. The response includes details such as the phone number's rate center,
        state, number type, and whether CNAM Lookup is enabled for that number.
      operationId: returns-a-list-of-all-phone-numbers-currently-on-your-flowroute-account-the-response-includes-detail
      x-api-path-slug: v2numbers-get
      parameters:
      - in: query
        name: contains
        description: Retrieves phone numbers containing the specified value
      - in: query
        name: ends_with
        description: Retrieves phone numbers that end with the specified value
      - in: query
        name: limit
        description: Limits the number of items to retrieve
      - in: query
        name: offset
        description: Offsets the list of phone numbers by your specified value
      - in: query
        name: starts_with
        description: Retrieves phone numbers that start with the specified value
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Account
      - Phone
      - Numbers
  /v2/numbers/{id}:
    get:
      summary: Phone Number Details
      description: Lists all of the information associated with any of the phone numbers
        in your account, including billing method, primary voice route, and failover
        voice route.
      operationId: lists-all-of-the-information-associated-with-any-of-the-phone-numbers-in-your-account-including-bill
      x-api-path-slug: v2numbersid-get
      parameters:
      - in: path
        name: id
        description: Phone number to search for which must be a number that you own
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Phone
      - Number
      - Details
    post:
      summary: Purchase a Phone Number
      description: Lets you purchase a phone number from available Flowroute inventory.
      operationId: lets-you-purchase-a-phone-number-from-available-flowroute-inventory
      x-api-path-slug: v2numbersid-post
      parameters:
      - in: path
        name: id
        description: Phone number to purchase
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Purchase
      - Phone
      - Number
  /v2/numbers/available:
    get:
      summary: Search for Purchasable Phone Numbers
      description: This endpoint lets you search for phone numbers by state or rate
        center, or by your specified search value.
      operationId: this-endpoint-lets-you-search-for-phone-numbers-by-state-or-rate-center-or-by-your-specified-search-
      x-api-path-slug: v2numbersavailable-get
      parameters:
      - in: query
        name: contains
        description: Retrieve phone numbers containing the specified value
      - in: query
        name: ends_with
        description: Retrieve phone numbers that end with the specified value
      - in: query
        name: limit
        description: Limits the number of items to retrieve
      - in: query
        name: offset
        description: Offsets the list of phone numbers by your specified value
      - in: query
        name: rate_center
        description: Filters by and displays phone numbers in the specified case-insensitive
          abbreviated rat    e center, not the full name as differentiated in the
          NPA Rate Center Reports
      - in: query
        name: starts_with
        description: Retrieve phone numbers that start with the specified value
      - in: query
        name: state
        description: Filters by and displays phone numbers in the specified case-insensitive
          abbreviated rat    e center, not the full name as differentiated in the
          NPA Rate Center Reports
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - SearchPurchasable
      - Phone
      - Numbers
  /v2/numbers/available/areacodes:
    get:
      summary: List Available Area Codes
      description: Returns a list of all Numbering Plan Area (NPA) codes containing
        purchasable phone numbers.
      operationId: returns-a-list-of-all-numbering-plan-area-npa-codes-containing-purchasable-phone-numbers
      x-api-path-slug: v2numbersavailableareacodes-get
      parameters:
      - in: query
        name: limit
        description: Limits the number of items to retrieve
      - in: query
        name: max_setup_cost
        description: Restricts the results to area codes that include at least one
          telephone number with a setup fee below or equal to the specified max_setup_cost
      - in: query
        name: offset
        description: Offsets the list of phone numbers by your specified value
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - List
      - Available
      - Area
      - Codes
  /v2/numbers/available/exchanges:
    get:
      summary: List Available Exchange Codes
      description: Returns a list of all Central Office (exchange) codes containing
        purchasable phone numbers.
      operationId: returns-a-list-of-all-central-office-exchange-codes-containing-purchasable-phone-numbers
      x-api-path-slug: v2numbersavailableexchanges-get
      parameters:
      - in: query
        name: areacode
        description: Restricts the results to the specified area code
      - in: query
        name: limit
        description: Limits the number of items to retrieve
      - in: query
        name: max_setup_cost
        description: Restricts the results to exchanges that include at least one
          telephone number with a setup fee below or equal to the specified max_setup_cost
      - in: query
        name: offset
        description: Offsets the list of phone numbers by your specified value
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - List
      - Available
      - Exchange
      - Codes
  /v2/numbers/{number_id}/relationships/primary_route:
    patch:
      summary: Update Primary Voice Route for a Phone Number
      description: Use this endpoint to update the primary voice route for a phone
        number. You must create the route first by following "Create an Inbound Route".
        You can then assign the created route by specifying its value in a PATCH request.
      operationId: use-this-endpoint-to-update-the-primary-voice-route-for-a-phone-number-you-must-create-the-route-fir
      x-api-path-slug: v2numbersnumber-idrelationshipsprimary-route-patch
      parameters:
      - in: path
        name: number_id
        description: The phone number in E
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Primary
      - Voice
      - Routea
      - Phone
      - Number
  /v2/numbers/{number_id}/relationships/failover_route:
    patch:
      summary: Update Failover Voice Route for a Phone Number
      description: Use this endpoint to update the failover voice route for a phone
        number. You must create the route first by following "Create an Inbound Route".
        You can then assign the created route by specifying its value in a PATCH request.
      operationId: use-this-endpoint-to-update-the-failover-voice-route-for-a-phone-number-you-must-create-the-route-fi
      x-api-path-slug: v2numbersnumber-idrelationshipsfailover-route-patch
      parameters:
      - in: path
        name: number_id
        description: The phone number in E
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Failover
      - Voice
      - Routea
      - Phone
      - Number
  /v2/routes:
    post:
      summary: Create an Inbound Route
      description: Creates a new inbound route which can then be associated with phone
        numbers. Please see "List Inbound Routes" to review the route values that
        you can associate with your Flowroute phone numbers.
      operationId: creates-a-new-inbound-route-which-can-then-be-associated-with-phone-numbers-please-see-list-inbound-
      x-api-path-slug: v2routes-post
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Inbound
      - Route
    get:
      summary: List Inbound Routes
      description: Returns a list of your inbound routes. From the list, you can then
        select routes to use as the primary and failover routes for a phone number,
        which you can do via "Update Primary Voice Route for a Phone Number" and "Update
        Failover Voice Route for a Phone Number".
      operationId: returns-a-list-of-your-inbound-routes-from-the-list-you-can-then-select-routes-to-use-as-the-primary
      x-api-path-slug: v2routes-get
      parameters:
      - in: query
        name: limit
        description: Limits the number of routes to retrieve
      - in: query
        name: offset
        description: Offsets the list of routes by your specified value
      - in: query
        name: route_type
        description: Restricts the results to inbound routes with your specified route
          type
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - List
      - Inbound
      - Routes