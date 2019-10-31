swagger: "2.0"
x-collection-name: OpenCorporates
x-complete: 1
info:
  title: OpenCorporates
  description: the-api-for-managing-opencorporates-data-
  termsOfService: https://opencorporates.com/info/licence
  version: v.04
host: api.opencorporates.com
basePath: v0.4/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account_status:
    get:
      summary: Account Status
      description: nThis returns the status of your API Account (this information
        may also be retrieved at https://OpenCorporates
      operationId: account-status
      x-api-path-slug: account-status-get
      parameters:
      - in: query
        name: calls_remaining
        description: this has two subvalues - today and this_month
      - in: query
        name: expiry_date
        description: when the api_plan runs out
      - in: query
        name: plan
        description: the type of plan that you are on
      - in: query
        name: status
        description: status of the API account
      - in: query
        name: usage
        description: this has two subvalues - today and this_month
      responses:
        200:
          description: OK
      tags:
      - Businesses
      - Account
      - Status
  /companies/:jurisdiction_code/:company_number/data:
    get:
      summary: Companies  Jurisdiction Code  Company Number Data
      description: nThis returns the data held for the given company
      operationId: companies--jurisdiction-code--company-number-data
      x-api-path-slug: companiesjurisdiction-codecompany-numberdata-get
      parameters:
      - in: query
        name: data_type
        description: this is a string value denoting the type of data, e
      - in: query
        name: description
        description: the given description of the datum as displayed on OpenCorporates
      - in: query
        name: id
        description: the id given to the filing by the company registry
      - in: query
        name: title
        description: this is the title of the datum as displayed on OpenCorporates
      responses:
        200:
          description: OK
      tags:
      - Businesses
      - Companies
      - :jurisdiction
      - Code
      - :company
      - Number
      - Data
  /companies/:jurisdiction_code/:company_number/network:
    get:
      summary: Companies  Jurisdiction Code  Company Number Network
      description: nThis returns the immediate &#39;computed corporate network&#39;
        for the given company as a set of control relationships (i
      operationId: companies--jurisdiction-code--company-number-network
      x-api-path-slug: companiesjurisdiction-codecompany-numbernetwork-get
      parameters:
      - in: query
        name: child_name
        description: the name of the child entity
      - in: query
        name: child_opencorporates_url
        description: the OpenCorporates URL of the child entity
      - in: query
        name: child_type
        description: the type of entity the child is
      - in: query
        name: confidence
        description: a computed confidence in the relationship based on the underlying
          statements
      - in: query
        name: parent_name
        description: the name of the parent entity
      - in: query
        name: parent_opencorporates_url
        description: the OpenCorporates URL of the parent entity
      - in: query
        name: parent_type
        description: the type of entity the parent is
      - in: query
        name: relationship_properties
        description: any additional properties of the relationship, e
      - in: query
        name: relationship_type
        description: the type of relationship, e
      responses:
        200:
          description: OK
      tags:
      - Businesses
      - Companies
      - :jurisdiction
      - Code
      - :company
      - Number
      - Network
  /companies/search:
    get:
      summary: Companies Search
      description: nThis returns a collection of companies whose name matches the
        given search term (submitted as :q in the query parameters)
      operationId: companies-search
      x-api-path-slug: companiessearch-get
      parameters:
      - in: query
        name: branch
        description: Filter by branch status (boolean)
      - in: query
        name: company_type
        description: The type of the company, as defined by the company register
      - in: query
        name: country_code
        description: NEWThe companies searched for can be restricted to a given country
          by passing a country_code query parameter
      - in: query
        name: created_since
        description: companies added to OpenCorporates after the given date
      - in: query
        name: current_status
        description: The current status of the company, as defined by the company
          register
      - in: query
        name: dissolution_date
        description: NEWas with all date fields, dissolution_date can be supplied
          either as a specific date or as a span of dates
      - in: query
        name: dissolved_before
        description: DeprecatedRestrict to companies with a dissolution_date before
          the given date
      - in: query
        name: dissolved_since
        description: DeprecatedRestrict to companies with a dissolution_date after
          the given date
      - in: query
        name: exclude_inactive
        description: DeprecatedRestrict to companies that are active/inactive
      - in: query
        name: fields
        description: NEWBy default when searching with a term (e
      - in: query
        name: inactive
        description: Filter by inactive status (boolean)
      - in: query
        name: incorporated_before
        description: DeprecatedRestrict to companies with an incorporation_date before
          the given date
      - in: query
        name: incorporated_since
        description: DeprecatedRestrict to companies with an incorporation_date after
          the given date
      - in: query
        name: incorporation_date
        description: NEWAs with all date fields, incorporation_date can be supplied
          either as a specific date or as a span of dates
      - in: query
        name: industry_codes
        description: NEWOne or more industry codes representing the industries the
          company operates in
      - in: query
        name: jurisdiction_code
        description: The companies searched for can be restricted to a given jurisdiction
          by passing a jurisdiction_code query parameter
      - in: query
        name: nonprofit
        description: NEWFilter by nonprofit company type (boolean)
      - in: query
        name: registered_address
        description: NEWThe companies searched for can be restricted by passing in
          an address or parts of an address
      responses:
        200:
          description: OK
      tags:
      - Businesses
      - Companies
      - Search
  /corporate_groupings/search:
    get:
      summary: Corporate Groupings Search
      description: nThis returns a collection of corporate_groupings whose name matches
        the given search term (submitted as :q in the query parameters)
      operationId: corporate-groupings-search
      x-api-path-slug: corporate-groupingssearch-get
      responses:
        200:
          description: OK
      tags:
      - Businesses
      - Corporate
      - Groupings
      - Search
  /data/:id:
    get:
      summary: Data  ID
      description: nThis returns information on a given datum
      operationId: data--id
      x-api-path-slug: dataid-get
      responses:
        200:
          description: OK
      tags:
      - Businesses
      - Data
  /industry_codes/:code_scheme_id:
    get:
      summary: Industry Codes  Code Scheme ID
      description: nThis call returns further details about the code_scheme, together
        with the list of industry codes associated with it
      operationId: get-industry-codes--code-scheme-id
      x-api-path-slug: industry-codescode-scheme-id-get
      responses:
        200:
          description: OK
      tags:
      - Businesses
      - Industry
      - Codes
      - :code
      - Scheme
      - Id
  /jurisdictions/match:
    get:
      summary: Jurisdictions Match
      description: nThis matches the name of a jurisdiction to the jurisdiction
      operationId: get-jurisdictions-match
      x-api-path-slug: jurisdictionsmatch-get
      responses:
        200:
          description: OK
      tags:
      - Businesses
      - Jurisdictions
      - Match
  /officers/:id:
    get:
      summary: Officers  ID
      description: nThis returns information on a particular officer (a director or
        an agent for a company)
      operationId: officers--id
      x-api-path-slug: officersid-get
      parameters:
      - in: query
        name: address
        description: NEWthe given address of the officer, if known (only for users
          with API key)
      - in: query
        name: date_of_birth
        description: NEWthe date of birth of the officer, if known (only for users
          with API key)
      - in: query
        name: end_date
        description: this is date on which the officership ended
      - in: query
        name: position
        description: the position held (e
      - in: query
        name: start_date
        description: this is date on which the officership started
      - in: query
        name: uid
        description: the id given to the officer by the company registry
      responses:
        200:
          description: OK
      tags:
      - Businesses
      - Officers
  /placeholder/:id:
    get:
      summary: Placeholder  ID
      description: nA placeholder is we call something we believe is probably a company
      operationId: placeholder--id
      x-api-path-slug: placeholderid-get
      parameters:
      - in: query
        name: company
        description: if the placeholder has been matched to a company, the company
          will be included, together with basic information for the company
      - in: query
        name: identifier
        description: an identifier that is associated with the placeholder, for example
          an SEC CIK code
      - in: query
        name: jurisdiction_code
        description: the code for the jurisdiction in which the placeholder is believed
          to be incorporated (see [GET company](#company))
      - in: query
        name: jurisdiction_string
        description: A plain text representation for the jurisdiction in which the
          placeholder is believed to be incorporated - this may be the name of a jurisdiction,
          of a country, or possibly an ISO 3166-2 code
      - in: query
        name: name
        description: the name of the entity
      - in: query
        name: opencorporates_url
        description: the url of the placeholder
      responses:
        200:
          description: OK
      tags:
      - Businesses
      - Placeholder
  /placeholders/:id/statements:
    get:
      summary: Placeholders  ID Statements
      description: nThis returns the statements associated with a given placeholder
      operationId: placeholders--id-statements
      x-api-path-slug: placeholdersidstatements-get
      responses:
        200:
          description: OK
      tags:
      - Businesses
      - Placeholders
      - Statements
  /versions:
    get:
      summary: Versions
      description: nThis returns the current version of the API and supported versions
      operationId: versions
      x-api-path-slug: versions-get
      responses:
        200:
          description: OK
      tags:
      - Businesses
      - Versions