swagger: "2.0"
x-collection-name: FullContact
x-complete: 1
info:
  title: FullContact Location API
  description: the-api-for-managing-fullcontact-locations
  termsOfService: https://www.fullcontact.com/terms/
  version: 1.0.0
host: api.fullcontact.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /batch.json:
    get:
      summary: Batch Process
      description: Batch Process
      operationId: batchProcess
      x-api-path-slug: batch-json-get
      parameters:
      - in: query
        name: apiKey
        description: This API key is assigned to you by FullContact
      - in: body
        name: Body
        description: '{     requests : [         https://api'
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Batch
  /stats.json:
    get:
      summary: Get Account Stats
      description: Get Account Stats
      operationId: getAccountStats
      x-api-path-slug: stats-json-get
      parameters:
      - in: query
        name: apiKey
        description: This API key is assigned to you by FullContact
      - in: query
        name: period
        description: You can define the month that you want to see usage stats for
          by using the period parameter
      responses:
        200:
          description: OK
      tags:
      - Statistics
  /email/disposable.json:
    get:
      summary: Lookup Email
      description: Lookup Email
      operationId: lookupEmail
      x-api-path-slug: emaildisposable-json-get
      parameters:
      - in: query
        name: apiKey
        description: This API key is assigned to you by FullContact
      - in: query
        name: email
        description: The email address that should be queried for being a disposable
          email address
      responses:
        200:
          description: OK
      tags:
      - Emails
  /company/lookup.json:
    get:
      summary: Get Company
      description: Get Company
      operationId: getCompany
      x-api-path-slug: companylookup-json-get
      parameters:
      - in: query
        name: apiKey
        description: This API key is assigned to you by FullContact
      - in: query
        name: callback
        description: If specified, the response will be wrapped as JSONP in a function
          call
      - in: query
        name: domain
        description: The domain of the company being looked up
      - in: query
        name: keyPeople
        description: If true, a list of Executive and VP level employees at this company
          will be returned under the keyPeople field
      - in: query
        name: prettyPrint
        description: The prettyPrint parameter can be used to disable prettyprint
          formatting on the API response
      responses:
        200:
          description: OK
      tags:
      - Companies
  /icon:
    get:
      summary: Get Icons
      description: Get Icons
      operationId: getIcons
      x-api-path-slug: icon-get
      parameters:
      - in: query
        name: apiKey
        description: This API key is assigned to you by FullContact
      responses:
        200:
          description: OK
      tags:
      - Icons
  /icon/{typeId}/{size}/{style}:
    get:
      summary: Get Icon
      description: Get Icon
      operationId: getIcon
      x-api-path-slug: icontypeidsizestyle-get
      parameters:
      - in: query
        name: apiKey
        description: This API key is assigned to you by FullContact
      - in: path
        name: size
        description: The size parameter allows you to specify the size of icon that
          you want
      - in: path
        name: style
        description: The style parameter allows you to pick from the available styles
          of the icons
      - in: path
        name: typeId
        description: The typeId is the name of the icon you want
      responses:
        200:
          description: OK
      tags:
      - Icons
  /v2/person.json:
    get:
      summary: ""
      description: Find out more about a person
      operationId: -v2-person
      x-api-path-slug: v2person-json-get
      parameters:
      - in: query
        name: email
        description: The email address you wish to query
      responses:
        200:
          description: OK
      tags:
      - People
  /cardReader:
    get:
      summary: Read Card
      description: Read Card
      operationId: readCard
      x-api-path-slug: cardreader-get
      parameters:
      - in: query
        name: apiKey
        description: This API key is assigned to you by FullContact
      - in: query
        name: casing
        description: Card Reader can alter the casing of certain fields in the final
          results
      - in: query
        name: Custom Params
        description: Card Reader has the ability to funnel your own custom params
          through requests
      - in: query
        name: format
        description: Used to specify response in json
      - in: body
        name: requestBody
        description: You can either send in the files as a multipart/form-data request
          or as a JSON object with BASE64 encoded images
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: returnedData
        description: A response can contain verified and unverified data, this parameter
          can be used to exclude unverified data from being returned in the response
      - in: query
        name: sandbox
        description: Card Reader Sandbox is a free, quick response mode for testing
          and development
      - in: query
        name: URID
        description: URID stands for Unique Request Identifier
      - in: query
        name: verified
        description: Used to specify the quality of transcription
      - in: query
        name: webhookUrl
        description: This is the URL that a request will be made to once the card
          has been processed
      responses:
        200:
          description: OK
      tags:
      - Card Reader
  /name/normalizer.json:
    get:
      summary: Name Normalization
      description: The Name Normalization method takes quasi-structured name data
        provided as a string and outputs the data in a structured manner. It also
        returns a likelihood based only on the order of the given name and family
        name as seen in the US population.
      operationId: normalizeName
      x-api-path-slug: namenormalizer-json-get
      parameters:
      - in: query
        name: casing
        description: Uppercase, lowercase, title case
      - in: query
        name: q
        description: The q parameter allows you to pass a quasi-structured full name
          string which can include standard prefix, first name, nickname, middle name,
          last name and suffix
      responses:
        200:
          description: OK
      tags:
      - Name
      - Normalizers
  /address/locationNormalizer.json:
    get:
      summary: Location Normalization
      description: The Location Normalization method takes semi-structured location
        data via the place parameter, provided as a string, and returns structured
        location data in either JSON or XML format.
      operationId: normalizeLocation
      x-api-path-slug: addresslocationnormalizer-json-get
      parameters:
      - in: query
        name: apiKey
        description: This API key is assigned to you by FullContact
      - in: query
        name: casing
        description: Uppercase, lowercase, title case
      - in: query
        name: includeZeroPopulation
        description: Appending includeZeroPopulation=true, will display 0 population
          census locations
      - in: query
        name: place
        description: The place parameter allows you to pass a semi-structured location
          string which can include continent, country, state, city, or county
      responses:
        200:
          description: OK
      tags:
      - Address
      - Locations