swagger: "2.0"
x-collection-name: Bookeo
x-complete: 1
info:
  title: Bookeo
  version: 1.0.0
host: api.bookeo.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /availability/matchingslots:
    post:
      summary: Find available slots matching given search parameters
      description: |-
        Create a search for available slots that match the given search parameters.
         Note that there are two different searches possible, /availability/slots and /availability/matchingslots (this endpoint).
         The former simply shows the number of available seats for each available slot. The latter (this one) takes as input the participant numbers, and shows the slots that are available for those numbers, and an estimate of the price.
         Parameters include product code, number of people and options.
         The successful response also contains a "Location" HTTP header, which can be invoked to navigate the results of the search.
      operationId: postAvailabilityMatchingslots
      x-api-path-slug: availabilitymatchingslots-post
      parameters:
      - in: query
        name: itemsPerPage
      - in: body
        name: search
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Availability
      - Matchingslots
  /availability/matchingslots/{pageNavigationToken}:
    get:
      summary: Navigate results of a matching slots search
      description: Navigate results of a matching slots search.
      operationId: getAvailabilityMatchingslotsPagenavigationtoken
      x-api-path-slug: availabilitymatchingslotspagenavigationtoken-get
      parameters:
      - in: path
        name: pageNavigationToken
      - in: query
        name: pageNumber
      responses:
        200:
          description: OK
      tags:
      - Availability
      - Matchingslots
      - PageNavigationToken
  /availability/slots:
    get:
      summary: Get information about the availability of products
      description: |-
        Performs a basic search to find available slots and number of seats in each.
         Note that there are two different searches possible, /availability/slots (this endpoint) and /availability/matchingslots .
         The former simply shows the number of available seats for each available slot. The latter takes as input the participant numbers, and shows the slots that are available for those numbers, and an estimate of the price.
         /availability/slots cannot be used for products of type flexibleTime . For those products, use /availability/matchingslots .
      operationId: getAvailabilitySlots
      x-api-path-slug: availabilityslots-get
      parameters:
      - in: query
        name: endTime
        description: the end time to search to
      - in: query
        name: itemsPerPage
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      - in: query
        name: productId
        description: the product id (see /settings/products)
      - in: query
        name: startTime
        description: the start time to search from
      responses:
        200:
          description: OK
      tags:
      - Availability
      - Slots
  /bookings:
    get:
      summary: Retrieve bookings
      description: |-
        Retrieve existing bookings
         The result is limited by the permissions of the apiKey.
         <p/>
         It is possible to filter by time booked and/or time of the last change.
         To filter by time booked, the parameters startTime and endTime are required.
         To filter by last time changed, the parameters lastUpdatedStartTime and lastUpdatedEndTime are required.
         It is possible to filter by both at the same time. At least one of the two filters must be used.
         <p/>
         It is further possible to filter by product id.
         <p/>
         Do not use this method to periodically poll for new/changed bookings. Use webhooks (see API general documentation) instead.
      operationId: getBookings
      x-api-path-slug: bookings-get
      parameters:
      - in: query
        name: endTime
        description: if specified, only include bookings that start on or before this
          time
      - in: query
        name: expandCustomer
        description: if true, the full details of the customer are included (provided
          the application has read permission over the customer)
      - in: query
        name: expandParticipants
        description: if true, full details of the participants are included (provided
          the application has read permission over the participant)
      - in: query
        name: includeCanceled
        description: if true, canceled bookings are included
      - in: query
        name: itemsPerPage
        description: 'maximum: 100'
      - in: query
        name: lastUpdatedEndTime
        description: if specified, only include bookings that were last changed (or
          created) on or before this time
      - in: query
        name: lastUpdatedStartTime
        description: if specified, only include bookings that were last changed (or
          created) on or after this time
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      - in: query
        name: productId
        description: if not specified, include bookings for all products
      - in: query
        name: startTime
        description: if specified, only include bookings that start on or after this
          time
      responses:
        200:
          description: OK
      tags:
      - Bookings
    post:
      summary: Create a new booking
      description: |-
        When creating a booking for a product of type "fixed" or "fixedCourse", the eventId is required. eventIds are obtained by calling /availability/slots or /availability/matchingSlots .
         When creating a booking for a product of type "flexibleTime", you can either specify the eventId or the startTime (in which case you can optionally specify the endTime. If no endTime is specified, Bookeo will automatically calculate the duration based on the options chosen)
      operationId: postBookings
      x-api-path-slug: bookings-post
      parameters:
      - in: body
        name: booking
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: mode
        description: if present and set to backend, treats the operation as if it
          was done by a manager
      - in: query
        name: notifyCustomer
        description: whether to send a confirmation email to the customer
      - in: query
        name: notifyUsers
        description: whether to send a notification email (and possibly SMS, depending
          on settings) to eligible users
      - in: query
        name: previousHoldId
        description: if specified, deletes the hold with the given id
      - in: query
        name: sendCustomerReminders
      - in: query
        name: sendCustomerThankyou
      responses:
        200:
          description: OK
      tags:
      - Bookings
  /bookings/{bookingNumber}:
    get:
      summary: Retrieve a booking
      description: Retrieve a booking by its booking number
      operationId: getBookingsBookingnumber
      x-api-path-slug: bookingsbookingnumber-get
      parameters:
      - in: path
        name: bookingNumber
      - in: query
        name: expandCustomer
        description: if true, the full details of the customer are included (provided
          the application has read permission over the customer)
      - in: query
        name: expandParticipants
        description: if true, full details of the participants are included (provided
          the application has read permission over the participant)
      responses:
        200:
          description: OK
      tags:
      - Bookings
      - BookingNumber
    put:
      summary: Update an existing booking
      description: Update an existing booking.
      operationId: putBookingsBookingnumber
      x-api-path-slug: bookingsbookingnumber-put
      parameters:
      - in: body
        name: booking
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bookingNumber
      - in: query
        name: mode
        description: if present and set to backend, treats the operation as if it
          was done by a manager
      - in: query
        name: notifyCustomer
      - in: query
        name: notifyUsers
      responses:
        200:
          description: OK
      tags:
      - Bookings
      - BookingNumber
    delete:
      summary: Cancel a booking
      description: Cancel a booking. Cancelled bookings remain in the system, but
        no longer show up in the calendar or take up seats.
      operationId: deleteBookingsBookingnumber
      x-api-path-slug: bookingsbookingnumber-delete
      parameters:
      - in: query
        name: applyCancellationPolicy
        description: if true, the default cancellation policy is applied
      - in: path
        name: bookingNumber
      - in: query
        name: cancelRemainingSeries
        description: if true, and this booking is part of a recurring series, all
          following bookings will be cancelled as well
      - in: query
        name: notifyCustomer
        description: if true, a notification email is sent to the customer
      - in: query
        name: notifyUsers
        description: if true, notification emails and SMS are sent to authorized users
      - in: query
        name: reason
        description: an optional reason that explains why the booking was cancelled
      - in: query
        name: trackInCustomerHistory
        description: if true, the cancellation will be tracked in the customers stats
      responses:
        200:
          description: OK
      tags:
      - Bookings
      - BookingNumber
  /bookings/{bookingNumber}/customer:
    get:
      summary: Retrieve the customer associated with a booking
      description: Retrieve the customer associated with a booking.
      operationId: getBookingsBookingnumberCustomer
      x-api-path-slug: bookingsbookingnumbercustomer-get
      parameters:
      - in: path
        name: bookingNumber
      responses:
        200:
          description: OK
      tags:
      - Bookings
      - BookingNumber
      - Customer
  /bookings/{bookingNumber}/payments:
    get:
      summary: Get the payments received for a booking
      description: Get a list of all payments received for a booking. Only payments
        for which the apiKey has at least read permission will be included
      operationId: getBookingsBookingnumberPayments
      x-api-path-slug: bookingsbookingnumberpayments-get
      parameters:
      - in: path
        name: bookingNumber
      - in: query
        name: itemsPerPage
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      responses:
        200:
          description: OK
      tags:
      - Bookings
      - BookingNumber
      - Payments
    post:
      summary: Add a payment to a booking
      description: Create a payment record associated with a booking
      operationId: postBookingsBookingnumberPayments
      x-api-path-slug: bookingsbookingnumberpayments-post
      parameters:
      - in: body
        name: apiPayment
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: bookingNumber
      responses:
        200:
          description: OK
      tags:
      - Bookings
      - BookingNumber
      - Payments
  /customers:
    get:
      summary: Retrieve customers
      description: Get a list of customers.
      operationId: getCustomers
      x-api-path-slug: customers-get
      parameters:
      - in: query
        name: createdSince
        description: if present, only include customers created since the given time
      - in: query
        name: currentMembers
        description: if true, include customers that are current members
      - in: query
        name: currentNonMembers
        description: if true, include customers that are not current members
      - in: query
        name: itemsPerPage
        description: number of items per page
      - in: query
        name: pageNavigationToken
        description: if present, continues navigation after a previous call
      - in: query
        name: pageNumber
      - in: query
        name: searchField
        description: a field on which to apply the search filter
      - in: query
        name: searchText
        description: the text to search for
      responses:
        200:
          description: OK
      tags:
      - Customers
    post:
      summary: Create a new customer.
      description: |-
        Create a new customer.
         Please note there is a limit to the number of customers that can be imported in Bookeo. Bookeo is primarily a booking system, not a CRM.
      operationId: postCustomers
      x-api-path-slug: customers-post
      parameters:
      - in: body
        name: customer
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customers
  /customers/{customerid}/linkedpeople/{id}:
    get:
      summary: Retrieve a person linked to a customer
      description: Retrieve a person linked to a customer.
      operationId: getCustomersCustomerLinkedpeople
      x-api-path-slug: customerscustomeridlinkedpeopleid-get
      parameters:
      - in: path
        name: customerid
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Customerid
      - Linkedpeople
    put:
      summary: Update the details of a person linked to a customer
      description: Update the details of a person linked to a customer.
      operationId: putCustomersCustomerLinkedpeople
      x-api-path-slug: customerscustomeridlinkedpeopleid-put
      parameters:
      - in: body
        name: apiLinkedPerson
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerid
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Customerid
      - Linkedpeople
    delete:
      summary: Delete a person linked to a customer
      description: Delete a person linked to a customer.
      operationId: deleteCustomersCustomerLinkedpeople
      x-api-path-slug: customerscustomeridlinkedpeopleid-delete
      parameters:
      - in: path
        name: customerid
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Customerid
      - Linkedpeople
  /customers/{id}:
    get:
      summary: Retrieve a customer
      description: Retrieve a customer by its id
      operationId: getCustomers
      x-api-path-slug: customersid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Customers
    put:
      summary: Update an existing customer
      description: Update an existing customer.
      operationId: putCustomers
      x-api-path-slug: customersid-put
      parameters:
      - in: body
        name: customer
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Customers
    delete:
      summary: Delete a customer
      description: |-
        Delete a customer.
         Please note it is not possible to delete customers that have bookings in the future, and that are not cancelled.
         If your application needs to delete a customer with future bookings, make sure to cancel all future bookings for that customer first.
      operationId: deleteCustomers
      x-api-path-slug: customersid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Customers
  /customers/{id}/authenticate:
    get:
      summary: Check a customer's password
      description: |-
        The customer's email address is the "username" used by Bookeo to authenticate customers.
         So to authenticate a customer your application would typically use GET /customers to search for customers with a given email address, and then GET /customers/{id}/authenticate to authenticate.
         Remember that there may be duplicate customer records with the same email address, ex. due to duplicate importing or manual record creation.
      operationId: getCustomersAuthenticate
      x-api-path-slug: customersidauthenticate-get
      parameters:
      - in: path
        name: id
      - in: query
        name: password
        description: remember to use URL encoding
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Authenticate
  /customers/{id}/bookings:
    get:
      summary: Retrieve a customer's bookings
      description: Retrieve a customer's bookings.
      operationId: getCustomersBookings
      x-api-path-slug: customersidbookings-get
      parameters:
      - in: query
        name: beginDate
        description: if specified, only bookings on or after this date will be included
      - in: query
        name: endDate
        description: if specified, only bookings on or before this date will be included
      - in: query
        name: expandParticipants
        description: if true, full details of the participants are included (provided
          the application has read permission over the participant)
      - in: path
        name: id
      - in: query
        name: itemsPerPage
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Bookings
  /customers/{id}/linkedpeople:
    get:
      summary: Get the people linked to a customer
      description: Get the people linked to a customer.
      operationId: getCustomersLinkedpeople
      x-api-path-slug: customersidlinkedpeople-get
      parameters:
      - in: path
        name: id
      - in: query
        name: itemsPerPage
        description: 'maximum: 100'
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Linkedpeople
  /holds:
    post:
      summary: Create a temporary hold to finalize the booking
      description: |-
        Performs a final check of the booking, and reserves required resources/seats to allow finalization of the booking process (ex. process payment).
         The returned object also contains the updated price calculations.
         Normally your application should have no more than one hold in place during a customer booking process.
         Make sure to not leave many holds around. In any case, holds are deleted automatically after a fixed time from creation.
         Note that when creating a hold, the customer field of the booking can be missing, in which case Bookeo will assume a default customer coming from the same country as the account.
         The successful response also contains a "Location" HTTP header, which can be used to access the created resource in future invocations.
      operationId: postHolds
      x-api-path-slug: holds-post
      parameters:
      - in: body
        name: booking
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: holdDurationSeconds
        description: the required seats/resources will be reserved for the specified
          time, ensuring that they cannot be taken by other bookings during this time
      - in: query
        name: previousHoldId
        description: if a previous hold was created during the same session with the
          customer, it will be automatically removed and replaced by the new one
      responses:
        200:
          description: OK
      tags:
      - Holds
  /holds/{id}:
    get:
      summary: Retrieve a hold previously generated
      description: Retrieve a hold previously generated.
      operationId: getHolds
      x-api-path-slug: holdsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Holds
    delete:
      summary: Delete a temporary hold
      description: |-
        Delete a temporary hold previously created.
         Note that you can also delete a hold when creating a new hold (ex. when the customer goes back in the booking process and selects a different time), or when creating a booking (i.e. when the customer checks out), without having to make a separate call to this endpoint.
      operationId: deleteHolds
      x-api-path-slug: holdsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Holds
  /payments:
    get:
      summary: Get a list of payments received
      description: Get a list of payments received.
      operationId: getPayments
      x-api-path-slug: payments-get
      parameters:
      - in: query
        name: endTime
      - in: query
        name: itemsPerPage
        description: 'maximum: 300'
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      - in: query
        name: paymentMethod
      - in: query
        name: paymentMethodOther
      - in: query
        name: startTime
      responses:
        200:
          description: OK
      tags:
      - Payments
  /payments/{id}:
    get:
      summary: Retrieve a specific payment
      description: Retrieve a specific payment.
      operationId: getPayments
      x-api-path-slug: paymentsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Payments
  /resourceblocks:
    get:
      summary: Retrieve resource blocks
      description: |-
        Retrieve existing resource blocks
         The result is limited by the permissions of the apiKey.
         <p/>
         It is possible to filter by time blocked and/or time of the last change.
         To filter by time blocked, the parameters startTime and endTime are required.
         To filter by last time changed, the parameters lastUpdatedStartTime and lastUpdatedEndTime are required.
         It is possible to filter by both at the same time. At least one of the two filters must be used.
         <p/>
         It is further possible to filter by resource.
      operationId: getResourceblocks
      x-api-path-slug: resourceblocks-get
      parameters:
      - in: query
        name: endTime
        description: if specified, only include blocks that start on or before this
          time
      - in: query
        name: itemsPerPage
        description: 'maximum: 100'
      - in: query
        name: lastUpdatedEndTime
        description: if specified, only include blocks that were last changed (or
          created) on or before this time
      - in: query
        name: lastUpdatedStartTime
        description: if specified, only include blocks that were last changed (or
          created) on or after this time
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      - in: query
        name: resourceId
        description: if specified, only include blocks that affect this resource
      - in: query
        name: startTime
        description: if specified, only include blocks that start on or after this
          time
      responses:
        200:
          description: OK
      tags:
      - Resourceblocks
    post:
      summary: Create a new resource block
      description: |-
        "blocks" time for one or more resources, so that they're not available for booking.
         A resource block must be for at least one resource, but it can block more than one.
         When setting the resources in the block, only the id is required.
      operationId: postResourceblocks
      x-api-path-slug: resourceblocks-post
      parameters:
      - in: body
        name: block
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Resourceblocks
  /resourceblocks/{id}:
    get:
      summary: Retrieve a block
      description: Retrieve a block by its id
      operationId: getResourceblocks
      x-api-path-slug: resourceblocksid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Resourceblocks
    put:
      summary: Update an existing block
      description: |-
        A resource block must be for at least one resource, but it can block more than one.
         When setting the resources in the block, only the id is required.
      operationId: putResourceblocks
      x-api-path-slug: resourceblocksid-put
      parameters:
      - in: body
        name: block
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Resourceblocks
    delete:
      summary: Delete a block
      description: Delete a block.
      operationId: deleteResourceblocks
      x-api-path-slug: resourceblocksid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Resourceblocks
  /seatblocks:
    get:
      summary: Retrieve seat blocks
      description: |-
        Retrieve existing seat blocks
         The result is limited by the permissions of the apiKey.
         <p/>
         It is possible to filter by time blocked and/or time of the last change.
         To filter by time blocked, the parameters startTime and endTime are required.
         To filter by last time changed, the parameters lastUpdatedStartTime and lastUpdatedEndTime are required.
         It is possible to filter by both at the same time. At least one of the two filters must be used.
         <p/>
         It is further possible to filter by product id.
      operationId: getSeatblocks
      x-api-path-slug: seatblocks-get
      parameters:
      - in: query
        name: endTime
        description: if specified, only include blocks that start on or before this
          time
      - in: query
        name: itemsPerPage
        description: 'maximum: 100'
      - in: query
        name: lastUpdatedEndTime
        description: if specified, only include blocks that were last changed (or
          created) on or before this time
      - in: query
        name: lastUpdatedStartTime
        description: if specified, only include blocks that were last changed (or
          created) on or after this time
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      - in: query
        name: productId
        description: if specified, only include blocks for this product
      - in: query
        name: startTime
        description: if specified, only include blocks that start on or after this
          time
      responses:
        200:
          description: OK
      tags:
      - Seatblocks
    post:
      summary: Create a new seat block
      description: '"blocks" a given number of seats, so that they''re not available
        for booking.'
      operationId: postSeatblocks
      x-api-path-slug: seatblocks-post
      parameters:
      - in: body
        name: block
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Seatblocks
  /seatblocks/{id}:
    get:
      summary: Retrieve a block
      description: Retrieve a block by its id
      operationId: getSeatblocks
      x-api-path-slug: seatblocksid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Seatblocks
    put:
      summary: Update an existing block
      description: Updates an existing seat block
      operationId: putSeatblocks
      x-api-path-slug: seatblocksid-put
      parameters:
      - in: body
        name: block
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Seatblocks
    delete:
      summary: Delete a block
      description: Delete a block.
      operationId: deleteSeatblocks
      x-api-path-slug: seatblocksid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Seatblocks
  /settings/apikeyinfo:
    get:
      summary: Get information about your own API Key
      description: Get information about your own api key.
      operationId: getSettingsApikeyinfo
      x-api-path-slug: settingsapikeyinfo-get
      responses:
        200:
          description: OK
      tags:
      - Settings
      - Apikeyinfo
  /settings/business:
    get:
      summary: Get information, location and contact details about the business
      description: Get information, location and contact details about the business.
      operationId: getSettingsBusiness
      x-api-path-slug: settingsbusiness-get
      responses:
        200:
          description: OK
      tags:
      - Settings
      - Business
  /settings/languages:
    get:
      summary: Retrieve all supported languages
      description: Retrieve all supported languages.
      operationId: getSettingsLanguages
      x-api-path-slug: settingslanguages-get
      responses:
        200:
          description: OK
      tags:
      - Settings
      - Languages
  /settings/peoplecategories:
    get:
      summary: Retrieve all supported people categories
      description: |-
        Retrieve the people categories supported by this account.
         This can include the default ones ("Adults","Children","Infants") and also custom ones defined by the account ("Students", ...)
      operationId: getSettingsPeoplecategories
      x-api-path-slug: settingspeoplecategories-get
      responses:
        200:
          description: OK
      tags:
      - Settings
      - Peoplecategories
  /settings/products:
    get:
      summary: Get information about the products offered
      description: |-
        Get information about all the products (things that can be booked) offered.
         3 types of product are available:
         - fixed are products with a fixed schedule and a given number of seats. Ex a group tour, a class, a workshop
         - fixedCourse are fixed products that are defined as a course, i.e. comprise of a series of dates
         - flexibleTime are products that describe private appointments, i.e. when one booking uses one resource (teacher, consultant, etc)

         Although Bookeo applies a minimum amount of caching, it is recommended to cache these results for 10-15 minutes to improve the performance of your application, as product settings change rarely.
      operationId: getSettingsProducts
      x-api-path-slug: settingsproducts-get
      parameters:
      - in: query
        name: itemsPerPage
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      - in: query
        name: type
        description: if not specified, get all products
      responses:
        200:
          description: OK
      tags:
      - Settings
      - Products
  /settings/resources:
    get:
      summary: Retrieve all available resources
      description: Retrieve all available resources.
      operationId: getSettingsResources
      x-api-path-slug: settingsresources-get
      parameters:
      - in: query
        name: itemsPerPage
        description: 'maximum: 100'
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      responses:
        200:
          description: OK
      tags:
      - Settings
      - Resources
  /settings/taxes:
    get:
      summary: Retrieve all taxes used by this business
      description: Retrieve all taxes used by this business.
      operationId: getSettingsTaxes
      x-api-path-slug: settingstaxes-get
      responses:
        200:
          description: OK
      tags:
      - Settings
      - Taxes
  /subaccounts:
    get:
      summary: List all subaccounts in the portal
      description: Retrieve all the webhooks for this api key
      operationId: getSubaccounts
      x-api-path-slug: subaccounts-get
      parameters:
      - in: query
        name: itemsPerPage
        description: 'maximum: 300'
      - in: query
        name: pageNavigationToken
      - in: query
        name: pageNumber
      responses:
        200:
          description: OK
      tags:
      - Subaccounts
  /subaccounts/{subaccountId}/apikeys:
    post:
      summary: Create a new API Key for this application to access a subaccount
      description: |-
        Install this application in a subaccount.
         Note that the API key used in this call must be that of the portal manager account. The application installed in the subaccount will be the same as this one, with the same permissions.
         If this application was already installed in the subaccount, its API key will be replaced by the one created in this call.
      operationId: postSubaccountsSubaccountApikeys
      x-api-path-slug: subaccountssubaccountidapikeys-post
      parameters:
      - in: path
        name: subaccountId
        description: the id of the subaccount where to install this application
      responses:
        200:
          description: OK
      tags:
      - Subaccounts
      - SubaccountId
      - Apikeys
  /subaccounts/{subaccountId}/apikeys/{apiKey}:
    delete:
      summary: Delete the API Key for this application from a subaccount
      description: Delete the api key for this application from a subaccount.
      operationId: deleteSubaccountsSubaccountApikeysApikey
      x-api-path-slug: subaccountssubaccountidapikeysapikey-delete
      parameters:
      - in: path
        name: apiKey
      - in: path
        name: subaccountId
      responses:
        200:
          description: OK
      tags:
      - Subaccounts
      - SubaccountId
      - Apikeys
      - ApiKey
  /webhooks:
    get:
      summary: List all webhooks
      description: Retrieve all the webhooks for this api key
      operationId: getWebhooks
      x-api-path-slug: webhooks-get
      responses:
        200:
          description: OK
      tags:
      - Webhooks
    post:
      summary: Create a new webhook
      description: |-
        Note that if an existing webhook for the same domain and type was already set for this api key, it will be automatically replaced by this new webhook.
         In other words, there can be only one webhook for each combination of domain and type, for an API key.
         So to upgrade an existing webhook URL, simply create a new one with the same domain and type, but a different URL.

         For webhook with domain "bookings" and type "deleted", the notification will be sent whether the booking is canceled or completely deleted.
         Users can delete bookings by, for example, deleting their associated customer.
         Also note that these "bookings" "deleted" notifications are sent even for bookings in the past.
      operationId: postWebhooks
      x-api-path-slug: webhooks-post
      parameters:
      - in: body
        name: webhook
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Webhooks
  /webhooks/{webhookId}:
    get:
      summary: Retrieve a webhook
      description: Retrieve a webhook.
      operationId: getWebhooksWebhook
      x-api-path-slug: webhookswebhookid-get
      parameters:
      - in: path
        name: webhookId
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - WebhookId
    delete:
      summary: Delete a webhook
      description: Delete a webhook.
      operationId: deleteWebhooksWebhook
      x-api-path-slug: webhookswebhookid-delete
      parameters:
      - in: path
        name: webhookId
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - WebhookId