swagger: "2.0"
x-collection-name: Google Partners
x-complete: 1
info:
  title: Google Partners
  description: searches-certified-companies-and-creates-contact-leads-with-them-and-also-audits-the-usage-of-clients-
  contact:
    name: Google
    url: https://google.com
  version: v2
host: partners.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/analytics:
    get:
      summary: Get Analytics
      description: |-
        Lists analytics data for a user's associated company.
        Should only be called within the context of an authorized logged in user.
      operationId: partners.analytics.list
      x-api-path-slug: v2analytics-get
      parameters:
      - in: query
        name: pageSize
        description: Requested page size
      - in: query
        name: pageToken
        description: A token identifying a page of results that the server returns
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      responses:
        200:
          description: OK
      tags:
      - Analytics
  /v2/clientMessages:log:
    post:
      summary: Get Generic Message Log
      description: |-
        Logs a generic message from the client, such as
        `Failed to render component`, `Profile page is running slow`,
        `More than 500 users have accessed this result.`, etc.
      operationId: partners.clientMessages.log
      x-api-path-slug: v2clientmessageslog-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Message
  /v2/companies:
    get:
      summary: Get Companies
      description: Lists companies.
      operationId: partners.companies.list
      x-api-path-slug: v2companies-get
      parameters:
      - in: query
        name: address
        description: The address to use when searching for companies
      - in: query
        name: companyName
        description: Company name to search for
      - in: query
        name: gpsMotivations
        description: List of reasons for using Google Partner Search to get companies
      - in: query
        name: industries
        description: List of industries the company can help with
      - in: query
        name: languageCodes
        description: List of language codes that company can support
      - in: query
        name: maxMonthlyBudget.currencyCode
        description: The 3-letter currency code defined in ISO 4217
      - in: query
        name: maxMonthlyBudget.nanos
        description: Number of nano (10^-9) units of the amount
      - in: query
        name: maxMonthlyBudget.units
        description: The whole units of the amount
      - in: query
        name: minMonthlyBudget.currencyCode
        description: The 3-letter currency code defined in ISO 4217
      - in: query
        name: minMonthlyBudget.nanos
        description: Number of nano (10^-9) units of the amount
      - in: query
        name: minMonthlyBudget.units
        description: The whole units of the amount
      - in: query
        name: orderBy
        description: How to order addresses within the returned companies
      - in: query
        name: pageSize
        description: Requested page size
      - in: query
        name: pageToken
        description: A token identifying a page of results that the server returns
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      - in: query
        name: services
        description: List of services that the returned agencies should provide
      - in: query
        name: specializations
        description: List of specializations that the returned agencies should provide
      - in: query
        name: view
        description: The view of the `Company` resource to be returned
      - in: query
        name: websiteUrl
        description: Website URL that will help to find a better matched company
      responses:
        200:
          description: OK
      tags:
      - Company
    patch:
      summary: Update Company
      description: |-
        Update company.
        Should only be called within the context of an authorized logged in user.
      operationId: partners.updateCompanies
      x-api-path-slug: v2companies-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      - in: query
        name: updateMask
        description: Standard field mask for the set of fields to be updated
      responses:
        200:
          description: OK
      tags:
      - Company
  /v2/companies/{companyId}:
    get:
      summary: Get Company
      description: Gets a company.
      operationId: partners.companies.get
      x-api-path-slug: v2companiescompanyid-get
      parameters:
      - in: query
        name: address
        description: The address to use for sorting the companys addresses by proximity
      - in: path
        name: companyId
        description: The ID of the company to retrieve
      - in: query
        name: currencyCode
        description: If the companys budget is in a different currency code than this
          one, thenthe converted budget is converted to this currency code
      - in: query
        name: orderBy
        description: How to order addresses within the returned company
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      - in: query
        name: view
        description: The view of `Company` resource to be returned
      responses:
        200:
          description: OK
      tags:
      - Company
  /v2/companies/{companyId}/leads:
    post:
      summary: Get Company Leads
      description: Creates an advertiser lead for the given company ID.
      operationId: partners.companies.leads.create
      x-api-path-slug: v2companiescompanyidleads-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: companyId
        description: The ID of the company to contact
      responses:
        200:
          description: OK
      tags:
      - Lead
  /v2/exams/{examType}/token:
    get:
      summary: Get Exam Token
      description: Gets an Exam Token for a Partner's user to take an exam in the
        Exams System
      operationId: partners.exams.getToken
      x-api-path-slug: v2examsexamtypetoken-get
      parameters:
      - in: path
        name: examType
        description: The exam type we are requesting a token for
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      responses:
        200:
          description: OK
      tags:
      - Token
  /v2/leads:
    get:
      summary: Get Leads
      description: |-
        Lists advertiser leads for a user's associated company.
        Should only be called within the context of an authorized logged in user.
      operationId: partners.leads.list
      x-api-path-slug: v2leads-get
      parameters:
      - in: query
        name: orderBy
        description: How to order Leads
      - in: query
        name: pageSize
        description: Requested page size
      - in: query
        name: pageToken
        description: A token identifying a page of results that the server returns
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      responses:
        200:
          description: OK
      tags:
      - Lead
    patch:
      summary: Update Lead
      description: Updates the specified lead.
      operationId: partners.updateLeads
      x-api-path-slug: v2leads-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      - in: query
        name: updateMask
        description: Standard field mask for the set of fields to be updated
      responses:
        200:
          description: OK
      tags:
      - Lead
  /v2/offers:
    get:
      summary: Get Offers
      description: Lists the Offers available for the current user
      operationId: partners.offers.list
      x-api-path-slug: v2offers-get
      parameters:
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      responses:
        200:
          description: OK
      tags:
      - Offer
  /v2/offers/history:
    get:
      summary: Get Historical Offers
      description: Lists the Historical Offers for the current user (or user's entire
        company)
      operationId: partners.offers.history.list
      x-api-path-slug: v2offershistory-get
      parameters:
      - in: query
        name: entireCompany
        description: if true, show history for the entire company
      - in: query
        name: orderBy
        description: Comma-separated list of fields to order by, e
      - in: query
        name: pageSize
        description: Maximum number of rows to return per page
      - in: query
        name: pageToken
        description: Token to retrieve a specific page
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      responses:
        200:
          description: OK
      tags:
      - Lead
  /v2/partnersstatus:
    get:
      summary: Get Partner Status
      description: |-
        Gets Partners Status of the logged in user's agency.
        Should only be called if the logged in user is the admin of the agency.
      operationId: partners.getPartnersstatus
      x-api-path-slug: v2partnersstatus-get
      parameters:
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      responses:
        200:
          description: OK
      tags:
      - Status
  /v2/userEvents:log:
    post:
      summary: Log User Event
      description: Logs a user event.
      operationId: partners.userEvents.log
      x-api-path-slug: v2usereventslog-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Log
  /v2/userStates:
    get:
      summary: Get States For User
      description: Lists states for current user.
      operationId: partners.userStates.list
      x-api-path-slug: v2userstates-get
      parameters:
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      responses:
        200:
          description: OK
      tags:
      - User
  /v2/users/profile:
    patch:
      summary: Update User Profile
      description: |-
        Updates a user's profile. A user can only update their own profile and
        should only be called within the context of a logged in user.
      operationId: partners.users.updateProfile
      x-api-path-slug: v2usersprofile-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      responses:
        200:
          description: OK
      tags:
      - Profile
  /v2/users/{userId}:
    get:
      summary: Get User
      description: Gets a user.
      operationId: partners.users.get
      x-api-path-slug: v2usersuserid-get
      parameters:
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      - in: path
        name: userId
        description: Identifier of the user
      - in: query
        name: userView
        description: Specifies what parts of the user information to return
      responses:
        200:
          description: OK
      tags:
      - User
  /v2/users/{userId}/companyRelation:
    delete:
      summary: Delete user Company Relation
      description: Deletes a user's company relation. Unaffiliaites the user from
        a company.
      operationId: partners.users.deleteCompanyRelation
      x-api-path-slug: v2usersuseridcompanyrelation-delete
      parameters:
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Relation
    put:
      summary: Create user Company Relation
      description: Creates a user's company relation. Affiliates the user to a company.
      operationId: partners.users.createCompanyRelation
      x-api-path-slug: v2usersuseridcompanyrelation-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Relation