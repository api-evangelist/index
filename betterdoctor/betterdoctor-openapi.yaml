swagger: "2.0"
x-collection-name: BetterDoctor
x-complete: 1
info:
  title: BetterDoctor
  description: betterdoctor-helps-people-find-and-connect-to-the-best-doctors-through-our-consumer-app-doctor-marketing-services-and-api--our-mission-is-to-help-increase-transparency-in-healthcare-and-help-consumers-make-better-decisions-
  version: 1.0.0
host: api.betterdoctor.com
basePath: /2016-03-01
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /doctors:
    get:
      summary: Doctor search
      description: Doctor search
      operationId: doctor-search
      x-api-path-slug: doctors-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: query
        name: first_name
        description: The doctors first name; partial (type-ahead) characters/names
          are accepted
      - in: query
        name: gender
        description: The doctors gender (male or female)
      - in: query
        name: insurance_uid
        description: UID of an insurance plan (e
      - in: query
        name: last_name
        description: The doctors last name; partial (type-ahead) characters/names
          are accepted
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: location
        description: Search area - Either Circular (lat,lon,range (miles)) or Bounding
          box (top-right, bottom-left) (lat,lon,lat,lon)
      - in: query
        name: name
        description: The doctors name; searches in both first and last names
      - in: query
        name: practice_uid
        description: BetterDoctor Practice UID
      - in: query
        name: query
        description: Search all fields by a keyword query (e
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: sort
        description: 'Sort order for the search results (full-name-asc: Alphabetical
          sort by full provider name ascending'
      - in: query
        name: specialty_uid
        description: UID of a specialty (e
      - in: query
        name: user_key
        description: Your API access key
      - in: query
        name: user_location
        description: Users current location
      responses:
        200:
          description: OK
      tags:
      - Doctor
      - Search
  /doctors/{uid}:
    get:
      summary: Retrieve a specific doctor description
      description: Returns a doctor object based on an uid or a slug
      operationId: returns-a-doctor-object-based-on-an-uid-or-a-slug
      x-api-path-slug: doctorsuid-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: path
        name: uid
        description: BetterDoctor Doctor UID
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Doctors
  /doctors/npi/{npi}:
    get:
      summary: Retrieve a specific doctor description using NPI
      description: Returns a doctor object using NPI
      operationId: returns-a-doctor-object-using-npi
      x-api-path-slug: doctorsnpinpi-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: path
        name: npi
        description: The National Provider Identifier of the doctor to retrieve
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Doctors
  /practices:
    get:
      summary: Practice Search
      description: Results are provider service locations, commonly referred as practices
        or doctor's offices.
      operationId: results-are-provider-service-locations-commonly-referred-as-practices-or-doctors-offices
      x-api-path-slug: practices-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: location
        description: Search area - Either Circular (lat,lon,range (miles)) or Bounding
          box (top-right, bottom-left) (lat,lon,lat,lon)
      - in: query
        name: name
        description: The practice???s name
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: sort
        description: 'Sort order for the search results (full-name-asc: Alphabetical
          sort by full provider name ascending'
      - in: query
        name: user_key
        description: Your API access key
      - in: query
        name: user_location
        description: 'Users current location: lat, lon'
      responses:
        200:
          description: OK
      tags:
      - Practices
      - Search
  /practices/{uid}:
    get:
      summary: Retrieve a specific practice description
      description: Returns a practice object based on an uid or a slug
      operationId: returns-a-practice-object-based-on-an-uid-or-a-slug
      x-api-path-slug: practicesuid-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: path
        name: uid
        description: BetterDoctor Practice UID
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Practices
  /practices/npi/{npi}:
    get:
      summary: Retrieve a specific practice description using NPI
      description: Returns a practice object based on an NPI. The office returned
        is registered in the NPI directory. There may be additional offices with this
        NPI registered at this location. Use the /practices search to find additional
        locations.
      operationId: returns-a-practice-object-based-on-an-npi-the-office-returned-is-registered-in-the-npi-directory-the
      x-api-path-slug: practicesnpinpi-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: path
        name: npi
        description: National Provider Identifier (NPI)
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Practices
  /practices/{uid}/doctors:
    get:
      summary: Retrieve a list of doctors in this practice.
      description: Returns a paginated list of doctors in the specified practice.
        This is a convenience endpoint, you may also use /doctors search for all doctors.
      operationId: returns-a-paginated-list-of-doctors-in-the-specified-practice-this-is-a-convenience-endpoint-you-may
      x-api-path-slug: practicesuiddoctors-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: path
        name: uid
        description: BetterDoctor Practice UID
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Practices
      - Doctors
  /practices/npi/{npi}/doctors:
    get:
      summary: Retrieve a list of doctors in this practice using NPI
      description: Returns a paginated list of doctors in the specified practice.
        This is a convenience endpoint, you may also use /doctors search for all doctors.
      operationId: returns-a-paginated-list-of-doctors-in-the-specified-practice-this-is-a-convenience-endpoint-you-may
      x-api-path-slug: practicesnpinpidoctors-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: path
        name: npi
        description: National Provider Identifier (NPI)
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Practices
      - Doctors
  /specialties:
    get:
      summary: Retrieve a list of all specialties
      description: Specialty group list
      operationId: specialty-group-list
      x-api-path-slug: specialties-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Specialties
  /insurances:
    get:
      summary: Retrieve insurance providers and plans
      description: Insurance provider & plan list
      operationId: insurance-provider--plan-list
      x-api-path-slug: insurances-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Insurance
  /conditions:
    get:
      summary: Retrieve a list of known conditions
      description: List all conditions
      operationId: list-all-conditions
      x-api-path-slug: conditions-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Conditions
  /validations:
    post:
      summary: Add a new record
      description: 'Creates validation document using the request body, and returns
        the document created with unique identifier in Location header for reference.
        This is how validation data is submitted to BetterDoctor for addition to the
        API. The posted document must conform to BetterDoctor???s JSON schema for
        validation objects, see included model specification for more information.
        <br><h4 style=''margin-bottom: 0px !important;''> Return Headers </h4> <div>Location:
        The uid of the created document. This can be used to access the document again
        without executing a search.</div>'
      operationId: creates-validation-document-using-the-request-body-and-returns-the-document-created-with-unique-iden
      x-api-path-slug: validations-post
      parameters:
      - in: query
        name: user_key
        description: Your API access key
      - in: body
        name: validation
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Record
      - Search
      - Validations
    get:
      summary: Record search
      description: 'The endpoint can be used to identify providers with validation
        data. The search supports BetterDoctor unique provider identifier, National
        Provider Identifier (NPI) or reference uid based provider lookups. BetterDoctor
        identifiers and NPIs for doctors and practices can be discovered using BetterDoctor
        API???s search functionalities. <br><h4 style=''margin-bottom: 0px !important;''>
        Return Headers </h4> <div>Last-Modified: Timestamp of the last validation
        made over the matching validations. The value can be used to query changes
        in the validation status for the provider using since parameter in collaboration
        with HEAD method.</div>'
      operationId: the-endpoint-can-be-used-to-identify-providers-with-validation-data-the-search-supports-betterdoctor
      x-api-path-slug: validations-get
      parameters:
      - in: query
        name: data_type
        description: Provider type to search validations for
      - in: query
        name: data_uid
        description: Paired with data_type
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: npi
        description: Paired with data_type
      - in: query
        name: ref_uid
        description: Optional to data_type style queries
      - in: query
        name: since
        description: Limits validations returned to the validations after the given
          timestamp value (ISO 8601)
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: user_key
        description: Your API access key
      - in: query
        name: validation_method
        description: Limits validations returned to a validation method wanted
      responses:
        200:
          description: OK
      tags:
      - Record
      - Search
      - Validations
    head:
      summary: Check if new records exists
      description: 'The endpoint can be used to identify providers with validation
        data, and discover changes. It providers search functionalities like its GET
        method alternative, but does not return any validation data. Instead of the
        data itself, it returns 200 OK if matching validation documents based on the
        given query are found. And it returns 304 if no validation documents are found
        after the timestamp given using If-Modified-Since HTTP header or since parameter.
        <br><h4 style=''margin-bottom: 0px !important;''> Return Headers </h4> <div>Last-Modified:
        Timestamp of the last validation made over the matching validations. </div>'
      operationId: the-endpoint-can-be-used-to-identify-providers-with-validation-data-and-discover-changes-it-provider
      x-api-path-slug: validations-head
      parameters:
      - in: query
        name: data_type
        description: Provider type to search validations for
      - in: query
        name: data_uid
        description: Paired with data_type
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: npi
        description: Paired with data_type
      - in: query
        name: ref_uid
        description: Optional to data_type style queries
      - in: query
        name: since
        description: Limits validations returned to the validations after the given
          timestamp value (ISO 8601)
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: user_key
        description: Your API access key
      - in: query
        name: validation_method
        description: Limits validations returned to a validation method wanted
      responses:
        200:
          description: OK
      tags:
      - Record
      - Search
      - Validations
  /validations/{uid}:
    get:
      summary: Retrieve a specific record
      description: 'Returns requested validation document. The endpoint is a conveniece
        method to check status and accepted data of a specific validation, like after
        creation of a validation. The response consist of raw data from the validation
        event and related validation information. <br><h4 style=''margin-bottom: 0px
        !important;''> Return Headers </h4> <div>Last-Modified: Timestamp of the validation
        made.</div>'
      operationId: returns-requested-validation-document-the-endpoint-is-a-conveniece-method-to-check-status-and-accept
      x-api-path-slug: validationsuid-get
      parameters:
      - in: path
        name: uid
        description: Unique identifier of a validation document
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Record
      - Search
      - Validations
    head:
      summary: Check if a specific record exists
      description: 'The endpoint can be used to discover if a validation document
        exists in the API. <br><h4 style=''margin-bottom: 0px !important;''> Return
        Headers </h4> <div>Last-Modified: Timestamp of the validation made.</div>'
      operationId: the-endpoint-can-be-used-to-discover-if-a-validation-document-exists-in-the-api-brh4-stylemarginbott
      x-api-path-slug: validationsuid-head
      parameters:
      - in: path
        name: uid
        description: Unique identifier of a validation document
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Record
      - Search
      - Validations
  /info:
    get:
      summary: API Health Check
      description: Returns basic API health information for monitoring
      operationId: returns-basic-api-health-information-for-monitoring
      x-api-path-slug: info-get
      parameters:
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - API
      - Health
      - Check