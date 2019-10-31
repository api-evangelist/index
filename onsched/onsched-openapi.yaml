swagger: "2.0"
x-collection-name: OnSched
x-complete: 1
info:
  title: OnSched API
  description: build-secure-and-scalable-custom-apps-for-online-booking--our-flexible-api-provides-many-options-for-availability-and-booking--take-the-api-for-a-test-drive--just-click-on-the-authorize-button-above-and-authenticate---you-can-access-our-demo-company-profile-if-you-are-not-a-customer-or-your-own-profile-by-using-your-assigned-clientid-and-secret---------------------
  termsOfService: None
  contact:
    name: OnSched.com
    url: https://onsched.com
    email: info@onsched.com
  version: 1.0.0
host: api.onsched.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /consumer/v1/appointments:
    get:
      summary: Returns a list of appointments.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list."
      operationId: ConsumerV1AppointmentsGet
      x-api-path-slug: consumerv1appointments-get
      parameters:
      - in: query
        name: customerId
        description: Filter appointments by customer
      - in: query
        name: email
        description: Filter appointments by email address
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: offset
        description: Starting row of page, default 0
      - in: query
        name: resourceId
        description: Filter appointments by resource
      - in: query
        name: serviceId
        description: Filter appointments by service
      - in: query
        name: status
        description: 'Filter appointments by status: IN, BK, CN, RE, RS'
      responses:
        200:
          description: OK
      tags:
      - Appointments
    post:
      summary: Returns an appointment object
      description: "This end point creates a new appointment in an Initial \"IN\"
        status. \r\n\r\nA valid serviceId is required. Use GET consumer/v1/services
        to retrieve a list of your services.\r\n\r\nA valid resourceId is required
        if your calendar is a resource based calendar. Use consumer/v1/resources to
        retrieve a list of your resources.\r\n\r\nStartDateTime and EndDateTime are
        required. Use the ISO 8601 format for DateTime Timezone. e.g. 2016-10-30T9:00:00-5:00"
      operationId: ConsumerV1AppointmentsPost
      x-api-path-slug: consumerv1appointments-post
      parameters:
      - in: body
        name: appointmentIM
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Appointments
  /consumer/v1/appointments/{id}:
    get:
      summary: Returns an appointment object.
      description: "The result returned is a single appointment object. A valid id
        is required to find the appointment. \r\n\r\nFind appointment id's using the
        GET consumer/v1/appointments end point."
      operationId: ConsumerV1AppointmentsByIdGet
      x-api-path-slug: consumerv1appointmentsid-get
      parameters:
      - in: path
        name: id
        description: The id of the appointment object
      responses:
        200:
          description: OK
      tags:
      - Appointments
    delete:
      summary: Returns an appointment object
      description: "This end point deletes a booking. Only appointments in a \"IN\"
        initial status can be deleted.\r\nPast dated appointments cannot be cancelled.\r\n\r\nA
        valid appointment id is required. Use the appointmentId returned from GET
        /consumer/v1/appointments"
      operationId: ConsumerV1AppointmentsByIdDelete
      x-api-path-slug: consumerv1appointmentsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Appointments
  /consumer/v1/appointments/{id}/book:
    put:
      summary: Returns an appointment object
      description: "This end point completes a new booking. Only appointments in the
        \"IN\" initial status can be booked.\r\nby saving all the relevant details
        of the booking.\r\n\r\nA valid appointment id is required. Use the appointmentId
        returned from POST /consumer/v1/appointments\r\n\r\nTo update appointment
        custom field values, use the GET /consumer/v1/appointments/customfields information\r\nto
        understand your definitions of custom fields and what key and values to update."
      operationId: ConsumerV1AppointmentsByIdBookPut
      x-api-path-slug: consumerv1appointmentsidbook-put
      parameters:
      - in: body
        name: appointmentBookModel
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Appointments
      - Book
  /consumer/v1/appointments/{id}/cancel:
    put:
      summary: Returns an appointment object
      description: "This end point cancels a booking or reservation. Only appointments
        in a \"BK\" booked, or \"RS\" reserved status can be cancelled.\r\nPast dated
        appointments cannot be cancelled.\r\n\r\nA valid appointment id is required.
        Use the appointmentId returned from POST /consumer/v1/appointments"
      operationId: ConsumerV1AppointmentsByIdCancelPut
      x-api-path-slug: consumerv1appointmentsidcancel-put
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Appointments
      - Cancel
  /consumer/v1/appointments/{id}/reschedule:
    put:
      summary: Returns an appointment object
      description: "This end point reschedules a booking. Only appointments in a \"BK\"
        booked status can be rescheduled.\r\nPast dated appointments cannot be cancelled.\r\n\r\nA
        valid appointment id is required. Use the appointmentId returned from GET
        /consumer/v1/appointments.\r\n\r\nThe serviceId and resourceId are optional.
        If you want your users to change the resource or service on a reschedule\r\nyou
        will have to use the regular availability endpoint rather than the reschedule
        availability end point.\r\n\r\nUse the GET /consumer/v1/availability/{id}/reschedule
        endpoint to display a list of available times\r\nfor the end user to choose
        from to reschedule the original appointment."
      operationId: ConsumerV1AppointmentsByIdReschedulePut
      x-api-path-slug: consumerv1appointmentsidreschedule-put
      parameters:
      - in: body
        name: appointmentRM
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: appointment id
      responses:
        200:
          description: OK
      tags:
      - Appointments
      - Reschedule
  /consumer/v1/appointments/customfields:
    get:
      summary: Returns a list of appointment custom field definitions
      description: "This end point returns your Appointment custom field definitions.\r\n\r\nAppointment
        custom fields are different than Customer custom fields. Appointment custom
        fields are\r\nstored with each appointment. They are used when the information
        collected during the booking is specific\r\nto a particular visit.\r\n\r\nUse
        the field, and type to determine how to update field values\r\nin PUT /consumer/v1/appointments/{id}/book"
      operationId: ConsumerV1AppointmentsCustomfieldsGet
      x-api-path-slug: consumerv1appointmentscustomfields-get
      parameters:
      - in: query
        name: locationId
        description: The id of the business location
      responses:
        200:
          description: OK
      tags:
      - Appointments
      - Customfields
  /consumer/v1/appointments/bookingfields:
    get:
      summary: ""
      description: ""
      operationId: ConsumerV1AppointmentsBookingfieldsGet
      x-api-path-slug: consumerv1appointmentsbookingfields-get
      parameters:
      - in: query
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Appointments
      - Bookingfields
  /consumer/v1/availability/{serviceId}/{startDate}/{endDate}:
    get:
      summary: Returns a list of available times.
      description: "Choose your search criteria carefully. Availability is an expensive
        call. If you search availability for all resources\r\nthen you should only
        do so for a single date. If you decide to search availability for multiple
        dates you should only do so\r\nfor a specific resource by specifying the optional
        resourceId parameter.\r\n\r\nStart and End times are specified as military
        times e.g. 800 = 8:00am, 2230 = 10:30pm. \r\nYou will only see availability
        within the boundary of your business start and end times.\r\n\r\ndayAvailability
        will return day availablility for the number of days requested from the start
        date.\r\n\r\nfirstDayAvailable only works with day availability. If set to
        true it will look for the first day available within the range specified\r\nby
        the dayAvailability parameter. The two parameters together can be a clever
        way to display availability for a week or month.\r\nTip - pass in the beginning
        of the week or month, and available times are displayed for the first available
        date if exists.\r\n\r\nYou should only specify the duration parameter if you
        let your customers choose the duration of the appointment. e.g. from a list.\r\n\r\nThe
        tz parameter allows you to select a suitable timezone for the customer to
        book in. Your app should be timezone aware if you \r\nuse this option. The
        requested timezone is specified as an offset(plus or minus) from GMT time."
      operationId: ConsumerV1AvailabilityByServiceIdByStartDateByEndDateGet
      x-api-path-slug: consumerv1availabilityserviceidstartdateenddate-get
      parameters:
      - in: query
        name: dayAvailability
        description: Return day availability for number of days specified
      - in: query
        name: duration
        description: Duration of the service if different than the default
      - in: path
        name: endDate
        description: End Date for availability search
      - in: query
        name: endTime
        description: End Time for availability search
      - in: query
        name: firstDayAvailable
        description: Return available times for the first available day
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: resourceGroupId
        description: Resource Group Id for availability search
      - in: query
        name: resourceId
        description: Resource Id for availability search
      - in: query
        name: resourceIds
        description: Comma separated Resource Ids for availability search
      - in: path
        name: serviceId
        description: Service Id for availability search
      - in: path
        name: startDate
        description: Start Date for availability search
      - in: query
        name: startTime
        description: Start Time for availability search
      - in: query
        name: tzOffset
        description: Request timezone offset to view availability
      responses:
        200:
          description: OK
      tags:
      - Availability
      - ServiceId
      - StartDate
      - EndDate
  /consumer/v1/availability/{serviceId}/{startDate}/{endDate}/days:
    get:
      summary: Returns a list of available days.
      description: "This end point is used to show day level availability. For example
        if the business is closed, or there is a public holiday.\r\n\r\nDay level
        availability is a good way to restrict your choices of dates in your app and
        improve usability."
      operationId: ConsumerV1AvailabilityByServiceIdByStartDateByEndDateDaysGet
      x-api-path-slug: consumerv1availabilityserviceidstartdateenddatedays-get
      parameters:
      - in: path
        name: endDate
        description: End Date for availability search
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: resourceId
        description: Resource Id to filter on
      - in: path
        name: serviceId
        description: Service Id for availability search
      - in: path
        name: startDate
        description: Start Date for availability search
      - in: query
        name: tzOffset
        description: Request timezone offset to view availability
      responses:
        200:
          description: OK
      tags:
      - Availability
      - ServiceId
      - StartDate
      - EndDate
      - Days
  /consumer/v1/availability/{serviceId}/{startDate}/{endDate}/unavailable:
    get:
      summary: Returns a list of unavailable times.
      description: This endpoint is used to show unavailable times and provides information
        why the timeslot is unavailable.
      operationId: ConsumerV1AvailabilityByServiceIdByStartDateByEndDateUnavailableGet
      x-api-path-slug: consumerv1availabilityserviceidstartdateenddateunavailable-get
      parameters:
      - in: query
        name: duration
        description: Duration of the service if different than the default
      - in: path
        name: endDate
        description: End Date for unavailable time search
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: resourceId
        description: Resource Id to filter on
      - in: path
        name: serviceId
        description: Service Id for availability search
      - in: path
        name: startDate
        description: Start Date for unavailable time search
      - in: query
        name: tzOffset
        description: Request timezone offset to view unavailable times
      responses:
        200:
          description: OK
      tags:
      - Availability
      - ServiceId
      - StartDate
      - EndDate
      - Unavailable
  /consumer/v1/availability/{appointmentId}/reschedule:
    get:
      summary: Returns a list of available times.
      description: "This end point is used to find availability for the purpose of
        rescheduling an appointment.\r\nAvailability defaults to the serviceId, resourceId
        and timezone from the original appointment.\r\nAfter choosing from the availability,
        you can call the appointment reschedule endpoint."
      operationId: ConsumerV1AvailabilityByAppointmentIdRescheduleGet
      x-api-path-slug: consumerv1availabilityappointmentidreschedule-get
      parameters:
      - in: path
        name: appointmentId
        description: Appointment Id of the original appointment being rescheduled
      - in: query
        name: tzOffset
        description: Request timezone offset to view availability
      responses:
        200:
          description: OK
      tags:
      - Availability
      - AppointmentId
      - Reschedule
  /consumer/v1/customers:
    get:
      summary: Returns a list of customers.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list."
      operationId: ConsumerV1CustomersGet
      x-api-path-slug: consumerv1customers-get
      parameters:
      - in: query
        name: deleted
        description: Filter customers by deleted status
      - in: query
        name: email
        description: Filter customers by email address
      - in: query
        name: groupId
        description: Filter customers by group
      - in: query
        name: lastname
        description: Search customers by lastname
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: offset
        description: Starting row of page, default 0
      responses:
        200:
          description: OK
      tags:
      - Customers
    post:
      summary: Creates a new customer object.
      description: "Use this endpoint to create a new customer. If not specified the
        business location id defaults to the first location in the company.\r\nEmail
        Address and a lastname are required for creating a new customer."
      operationId: ConsumerV1CustomersPost
      x-api-path-slug: consumerv1customers-post
      parameters:
      - in: body
        name: customerIM
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customers
  /consumer/v1/customers/{id}:
    get:
      summary: Returns a customer object.
      description: "The result returned is a single customer object. An id is required
        to find the customer. Find customer id's using either the GET consumer/v1/customers
        end point,\r\nor the GET consumer/v1/appointments end point. A customer object
        is automatically created with the first booking if it doesn't already exist."
      operationId: ConsumerV1CustomersByIdGet
      x-api-path-slug: consumerv1customersid-get
      parameters:
      - in: path
        name: id
        description: The id of the customer object
      responses:
        200:
          description: OK
      tags:
      - Customers
    put:
      summary: Updates a customer object.
      description: "Use this endpoint to update customer information. If not specified
        the business location id defaults to the first location in the company.\r\nBlank
        fields are not changed"
      operationId: ConsumerV1CustomersByIdPut
      x-api-path-slug: consumerv1customersid-put
      parameters:
      - in: body
        name: customerUM
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
      summary: Deletes a customer subscription object.
      description: Deletes a customer subscription object.
      operationId: ConsumerV1CustomersByIdDelete
      x-api-path-slug: consumerv1customersid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Customers
  /consumer/v1/customers/customfields:
    get:
      summary: Returns a list of customField objects
      description: "This end point returns your Customer custom field definitions.\r\n\r\nCustomer
        custom fields are different than Appointment custom fields. Appointment custom
        fields are\r\nstored with each appointment. They are used when the information
        collected during the booking is specific\r\nto a particular visit, where as
        Customer custom fields are stored with the customer profile. \r\n\r\nUse the
        key field, and type to determine how to update field values\r\nin POST /consumer/v1/customers
        and PUT /consumer/v1/customers/{id}"
      operationId: ConsumerV1CustomersCustomfieldsGet
      x-api-path-slug: consumerv1customerscustomfields-get
      parameters:
      - in: query
        name: leadQuestions
        description: A true/false indicator to filter on custom fields used for lead
          questions
      - in: query
        name: locationId
        description: The id of the business location
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Customfields
  /consumer/v1/customers/registrationfields:
    get:
      summary: Returns a list of lead questions
      description: "This end point returns your Customer Registration fields.\r\n\r\nCustomer
        custom fields are different than Appointment custom fields. Appointment custom
        fields are\r\nstored with each appointment. They are used when the information
        collected during the booking is specific\r\nto a particular visit, where as
        Customer custom fields are stored with the customer profile."
      operationId: ConsumerV1CustomersRegistrationfieldsGet
      x-api-path-slug: consumerv1customersregistrationfields-get
      parameters:
      - in: query
        name: locationId
        description: The id of the business location
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Registrationfields
  /consumer/v1/customers/plans:
    get:
      summary: Returns a list of customers.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list."
      operationId: ConsumerV1CustomersPlansGet
      x-api-path-slug: consumerv1customersplans-get
      parameters:
      - in: query
        name: groupId
        description: Filter customers by group
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: offset
        description: Starting row of page, default 0
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Plans
  /consumer/v1/customers/plans/{id}:
    get:
      summary: Returns a customer object.
      description: "The result returned is a single customer object. An id is required
        to find the customer. Find customer id's using either the GET consumer/v1/customers
        end point,\r\nor the GET consumer/v1/appointments end point. A customer object
        is automatically created with the first booking if it doesn't already exist."
      operationId: ConsumerV1CustomersPlansByIdGet
      x-api-path-slug: consumerv1customersplansid-get
      parameters:
      - in: path
        name: id
        description: The id of the customer object
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Plans
  /consumer/v1/customers/{id}/planlimits/{serviceId}/{resourceId}/{dateTimeTz}:
    get:
      summary: Returns a list of customer booking limits.
      description: "The result returned is list of limit rules as defined by the subscribed
        customer plan along with Booking Counts/Minutes\r\nThe results indicate the
        remaining bookings count / minutes. Use the results in your app to determine
        if the customer should continue booking.\r\nYou can enforce Limits in periods:
        Daily,Weekly,Monthly and for maximum total limits. Maximum total limits is
        based on six months prior to\r\nthe DateTimeTz and six months after the DateTimeTz.
        Daily, Weekly and Monthly limits are based on the calculated period relative
        to the\r\nsubscription plan start. Daily,Weekly and Monthly limits can be
        setup on a per interval basis e.g. to biweekly, or daily every 10 days.\r\nSee
        customer plans setup in the Portal for more information.\r\nAll parameters
        are required. If resourceId is not applicable for a non-resource calendar,
        pass zero.\r\nFormat of the dateTimeTz field is 2018-10-30T10:00-5:00"
      operationId: ConsumerV1CustomersByIdPlanlimitsByServiceIdByResourceIdByDateTimeTzGet
      x-api-path-slug: consumerv1customersidplanlimitsserviceidresourceiddatetimetz-get
      parameters:
      - in: path
        name: dateTimeTz
        description: The DateTimeTz to check
      - in: path
        name: id
        description: The id of the customer object
      - in: path
        name: resourceId
        description: The id of the resource object
      - in: path
        name: serviceId
        description: The id of the service object
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Planlimits
      - ServiceId
      - ResourceId
      - DateTimeTz
  /consumer/v1/customers/subscriptions:
    get:
      summary: Returns a list of customer subscriptions.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list."
      operationId: ConsumerV1CustomersSubscriptionsGet
      x-api-path-slug: consumerv1customerssubscriptions-get
      parameters:
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: offset
        description: Starting row of page, default 0
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Subscriptions
  /consumer/v1/customers/{id}/subscriptions:
    get:
      summary: Returns a customer subscription object.
      description: The result returned is a single customer subscription object. A
        customer can only be subsribed to a single Customer Plan
      operationId: ConsumerV1CustomersByIdSubscriptionsGet
      x-api-path-slug: consumerv1customersidsubscriptions-get
      parameters:
      - in: path
        name: id
        description: The id of the customer object
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Subscriptions
    post:
      summary: Creates a new customer subscription object.
      description: Use this endpoint to create a new customer subscription.
      operationId: ConsumerV1CustomersByIdSubscriptionsPost
      x-api-path-slug: consumerv1customersidsubscriptions-post
      parameters:
      - in: body
        name: customerSubscriptionIM
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The id of the customer object
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Subscriptions
  /consumer/v1/customers/subscriptions/{id}:
    get:
      summary: Returns a customer subscription object.
      description: The result returned is a single customer subscription object.
      operationId: ConsumerV1CustomersSubscriptionsByIdGet
      x-api-path-slug: consumerv1customerssubscriptionsid-get
      parameters:
      - in: path
        name: id
        description: The id of the customer subscription object
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Subscriptions
    put:
      summary: Updates a customer subscription object.
      description: Use this endpoint to update customer subscription information.
      operationId: ConsumerV1CustomersSubscriptionsByIdPut
      x-api-path-slug: consumerv1customerssubscriptionsid-put
      parameters:
      - in: body
        name: customerSubscriptionUM
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The id of the customer subscription object
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Subscriptions
    delete:
      summary: Deletes a list of lead questions
      description: Deletes a list of lead questions
      operationId: ConsumerV1CustomersSubscriptionsByIdDelete
      x-api-path-slug: consumerv1customerssubscriptionsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Subscriptions
  /consumer/v1/customers/countries:
    get:
      summary: Returns a list of country objects
      description: Returns a list of countries with the associated country code. Country
        codes are based on the 2 character ANSI standard.
      operationId: ConsumerV1CustomersCountriesGet
      x-api-path-slug: consumerv1customerscountries-get
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Countries
  /consumer/v1/customers/states:
    get:
      summary: Returns a list of state objects
      description: "Returns a list of states with the associated state code and country.
        \r\n\r\nContact us if states for your countries of operation are not currently
        loaded."
      operationId: ConsumerV1CustomersStatesGet
      x-api-path-slug: consumerv1customersstates-get
      parameters:
      - in: query
        name: country
      responses:
        200:
          description: OK
      tags:
      - Customers
      - States
  /consumer/v1/locations:
    get:
      summary: Returns a list of business locations.
      description: "Use this api end point if you have multiple business locations
        in your company.\r\nThe results are returned in pages. Use the offset and
        limit parameters to control the page start and size. Default offset is 0,
        and limit is 20.\r\nUse the other query parameters to optionally filter the
        results list."
      operationId: ConsumerV1LocationsGet
      x-api-path-slug: consumerv1locations-get
      parameters:
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: name
        description: Location name(full or partial) to filter on
      - in: query
        name: offset
        description: Starting row of page, default 0
      responses:
        200:
          description: OK
      tags:
      - Locations
  /consumer/v1/locations/{id}:
    get:
      summary: Returns a business location object.
      description: The result returned is a single location object. An id is required
        to find the location. Find location id's using the GET consumer/v1/locations
        end point,
      operationId: ConsumerV1LocationsByIdGet
      x-api-path-slug: consumerv1locationsid-get
      parameters:
      - in: path
        name: id
        description: The id of the business location object
      responses:
        200:
          description: OK
      tags:
      - Locations
  /consumer/v1/resources:
    get:
      summary: Returns a list of resources.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list."
      operationId: ConsumerV1ResourcesGet
      x-api-path-slug: consumerv1resources-get
      parameters:
      - in: query
        name: email
        description: Filter resources by email address
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: name
        description: Search resources by name
      - in: query
        name: offset
        description: Starting row of page, default 0
      - in: query
        name: resourceGroupId
        description: Filter resources by group
      - in: query
        name: sortOrder
        description: Specify sort order of response
      responses:
        200:
          description: OK
      tags:
      - Resources
  /consumer/v1/resources/{id}:
    get:
      summary: Returns a resource object.
      description: "The result returned is a single resource object. An id is required
        to find the resource. Find customer id's using either the GET consumer/v1/resources
        end point,\r\nor the GET consumer/v1/appointments end point."
      operationId: ConsumerV1ResourcesByIdGet
      x-api-path-slug: consumerv1resourcesid-get
      parameters:
      - in: path
        name: id
        description: The id of the resource object
      responses:
        200:
          description: OK
      tags:
      - Resources
  /consumer/v1/resources/{id}/services:
    get:
      summary: Returns a list of resource services.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list.\r\nResource
        services are used to explicitly define the services that can be booked for
        a resource. If no resource services are defined then by\r\ndefault all services
        can be booked for the resource."
      operationId: ConsumerV1ResourcesByIdServicesGet
      x-api-path-slug: consumerv1resourcesidservices-get
      parameters:
      - in: path
        name: id
        description: The id of the resource object
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: offset
        description: Starting row of page, default 0
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Services
  /consumer/v1/servicegroups:
    get:
      summary: Returns a list of service groups.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list."
      operationId: ConsumerV1ServiceGroupsGet
      x-api-path-slug: consumerv1servicegroups-get
      parameters:
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: offset
        description: Starting row of page, default 0
      responses:
        200:
          description: OK
      tags:
      - Servicegroups
  /consumer/v1/servicegroups/{id}:
    get:
      summary: Returns a serviceGroup object.
      description: "The result returned is a single serviceGroup object. An id is
        required to find the serviceGroup. Find serviceGroup id's using \r\nthe GET
        consumer/v1/servicegroups end point,"
      operationId: ConsumerV1ServiceGroupsByIdGet
      x-api-path-slug: consumerv1servicegroupsid-get
      parameters:
      - in: path
        name: id
        description: The id of the serviceGroup object
      responses:
        200:
          description: OK
      tags:
      - Servicegroups
  /consumer/v1/services:
    get:
      summary: Returns a list of services.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list."
      operationId: ConsumerV1ServicesGet
      x-api-path-slug: consumerv1services-get
      parameters:
      - in: query
        name: defaultService
        description: Filter services by default service
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: locationId
        description: The id of the business location
      - in: query
        name: offset
        description: Starting row of page, default 0
      - in: query
        name: serviceGroupId
        description: Filter services by group
      responses:
        200:
          description: OK
      tags:
      - Services
  /consumer/v1/services/{id}:
    get:
      summary: Returns a service object.
      description: "The result returned is a single service object. An id is required
        to find the service. Find service id's using either the GET consumer/v1/service
        end point,\r\nor the GET consumer/v1/appointments end point."
      operationId: ConsumerV1ServicesByIdGet
      x-api-path-slug: consumerv1servicesid-get
      parameters:
      - in: path
        name: id
        description: The id of the service object
      responses:
        200:
          description: OK
      tags:
      - Services
  /consumer/v1/services/{id}/resources:
    get:
      summary: Returns a list of resources.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list."
      operationId: ConsumerV1ServicesByIdResourcesGet
      x-api-path-slug: consumerv1servicesidresources-get
      parameters:
      - in: path
        name: id
        description: The id of the service object
      - in: query
        name: limit
        description: Page limit, default 20
      - in: query
        name: offset
        description: Starting row of page, default 0
      responses:
        200:
          description: OK
      tags:
      - Services
      - Resources
  /consumer/v1/settings:
    get:
      summary: Returns a list of customers.
      description: "The results are returned in pages. Use the offset and limit parameters
        to control the page start and size. Default offset is 0, and limit is 20.\r\nUse
        the other query parameters to optionally filter the results list."
      operationId: ConsumerV1SettingsGet
      x-api-path-slug: consumerv1settings-get
      parameters:
      - in: query
        name: locationId
        description: The id of the business location
      responses:
        200:
          description: OK
      tags:
      - Settings