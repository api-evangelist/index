swagger: "2.0"
x-collection-name: Infermedica
x-complete: 1
info:
  title: Infermedica
  description: empower-your-healthcare-services-with-intelligent-diagnostic-insights-of-infermedica-api-
  version: v2
host: api.infermedica.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /conditions:
    get:
      summary: Get Conditions
      description: Returns a list of all available conditions.
      operationId: getConditions
      x-api-path-slug: conditions-get
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Conditions
  /conditions/{id}:
    get:
      summary: Get Conditions
      description: Returns details of a single condition specified by id parameter.
      operationId: getConditions
      x-api-path-slug: conditionsid-get
      parameters:
      - in: path
        name: id
        description: condition id
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Conditions
      - Id
  /diagnosis:
    post:
      summary: Post Diagnosis
      description: Suggests possible diagnoses and relevant observations based on
        provided patient information.
      operationId: postDiagnosis
      x-api-path-slug: diagnosis-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Diagnosis
  /explain:
    post:
      summary: Post Explain
      description: Explains which evidence impact probability of selected condition.
      operationId: postExplain
      x-api-path-slug: explain-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Explain
  /info:
    get:
      summary: Get Info
      description: Returns information about data used by diagnostic engine.
      operationId: getInfo
      x-api-path-slug: info-get
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Info
  /lab_tests:
    get:
      summary: Get Lab Tests
      description: Returns a list of all available lab tests.
      operationId: getLabTests
      x-api-path-slug: lab-tests-get
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Lab
      - Tests
  /lab_tests/{id}:
    get:
      summary: Get Lab Tests
      description: Returns details of a single lab test specified by id parameter.
      operationId: getLabTests
      x-api-path-slug: lab-testsid-get
      parameters:
      - in: path
        name: id
        description: lab test id
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Lab
      - Tests
  /lookup:
    get:
      summary: Get Lookup
      description: Returns a single observation matching given phrase.
      operationId: getLookup
      x-api-path-slug: lookup-get
      parameters:
      - in: query
        name: phrase
        description: phrase to match
      - in: query
        name: sex
        description: sex filter
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Lookup
  /parse:
    post:
      summary: Post Parse
      description: Returns list of mentions of observation found in given text.
      operationId: postParse
      x-api-path-slug: parse-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Parse
  /risk_factors:
    get:
      summary: Get Risk Factors
      description: Returns a list of all available risk factors.
      operationId: getRiskFactors
      x-api-path-slug: risk-factors-get
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Risk
      - Factors
  /risk_factors/{id}:
    get:
      summary: Get Risk Factors
      description: Returns details of a single risk factor specified by id parameter.
      operationId: getRiskFactors
      x-api-path-slug: risk-factorsid-get
      parameters:
      - in: path
        name: id
        description: risk factor id
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Risk
      - Factors
  /search:
    get:
      summary: Get Search
      description: Returns list of observations matching the given phrase.
      operationId: getSearch
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: max_results
        description: maximum number of results
      - in: query
        name: phrase
        description: phrase to match
      - in: query
        name: sex
        description: sex filter
      - in: query
        name: type
        description: type of results
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Search
  /suggest:
    post:
      summary: Post Suggest
      description: Suggests possible symptoms based on provided patient information.
      operationId: postSuggest
      x-api-path-slug: suggest-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: max_results
        description: maximum number of results
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Suggest
  /symptoms:
    get:
      summary: Get Symptoms
      description: Returns a list of all available symptoms.
      operationId: getSymptoms
      x-api-path-slug: symptoms-get
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Symptoms
  /symptoms/{id}:
    get:
      summary: Get Symptoms
      description: Returns details of a single symptom specified by id parameter.
      operationId: getSymptoms
      x-api-path-slug: symptomsid-get
      parameters:
      - in: path
        name: id
        description: symptoms id
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Symptoms
  /triage:
    post:
      summary: Post Triage
      description: Estimates triage level based on provided patient information.
      operationId: postTriage
      x-api-path-slug: triage-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Triage
  /observations:
    get:
      summary: List all observations
      description: Returns a list of all available observations.
      operationId: getAllObservations
      x-api-path-slug: observations-get
      responses:
        200:
          description: OK
      tags:
      - Observations
  /observations/{id}:
    get:
      summary: Get observation by id
      description: Returns details of a single observation specified by id parameter.
      operationId: getObservation
      x-api-path-slug: observationsid-get
      parameters:
      - in: path
        name: id
        description: observation id
      responses:
        200:
          description: OK
      tags:
      - Observations