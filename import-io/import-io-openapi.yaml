swagger: "2.0"
x-collection-name: Import.io
x-complete: 1
info:
  title: import.io
  version: "1.0"
host: schedule.import.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /extractor/{extractorId}/csv/latest:
    get:
      summary: Get Extractor Extractorid Csv Latest
      description: Get the latest crawl run results as a csv.
      operationId: getExtractorExtractorCsvLatest
      x-api-path-slug: extractorextractoridcsvlatest-get
      parameters:
      - in: path
        name: extractorId
        description: the id of the extractor to start get the latest crawl run data
      responses:
        200:
          description: OK
      tags:
      - Extractor
      - ExtractorId
      - Csv
      - Latest
  /extractor/{extractorId}/json/latest:
    get:
      summary: Get Extractor Extractorid Json Latest
      description: Get the latest crawl run results as json.
      operationId: getExtractorExtractorJsonLatest
      x-api-path-slug: extractorextractoridjsonlatest-get
      parameters:
      - in: path
        name: extractorId
        description: The id of the extractor to start get the latest crawl run data
      responses:
        200:
          description: OK
      tags:
      - Extractor
      - ExtractorId
      - Json
      - Latest
  /extractor/{extractorId}:
    get:
      summary: Get Extractor Extractorid
      description: Query by extractor endpoint, adhoc runs only..
      operationId: getExtractorExtractor
      x-api-path-slug: extractorextractorid-get
      parameters:
      - in: path
        name: extractorId
        description: extractorId
      - in: query
        name: url
        description: url
      responses:
        200:
          description: OK
      tags:
      - Extractor
      - ExtractorId
  /extractor/{extractorId}/runs:
    get:
      summary: Get Extractor Extractorid Runs
      description: Get a feed of the runs performed on an extractor.
      operationId: getExtractorExtractorRuns
      x-api-path-slug: extractorextractoridruns-get
      parameters:
      - in: path
        name: extractorId
        description: The id of the extractor to start get the crawl run data
      responses:
        200:
          description: OK
      tags:
      - Extractor
      - ExtractorId
      - Runs
  /extractor/{extractorId}/cancel:
    post:
      summary: Post Extractor Extractorid Cancel
      description: Cancel an existing crawl..
      operationId: postExtractorExtractorCancel
      x-api-path-slug: extractorextractoridcancel-post
      parameters:
      - in: path
        name: extractorId
        description: extractorId
      responses:
        200:
          description: OK
      tags:
      - Extractor
      - ExtractorId
      - Cancel
  /extractor/{extractorId}/start:
    post:
      summary: Post Extractor Extractorid Start
      description: Launch a crawl from an extractor that a user owns..
      operationId: postExtractorExtractorStart
      x-api-path-slug: extractorextractoridstart-post
      parameters:
      - in: path
        name: extractorId
        description: the id of the extractor to start crawling with
      - in: query
        name: loginSessionId
        description: The loginSessionId required for authenticated extractors
      responses:
        200:
          description: OK
      tags:
      - Extractor
      - ExtractorId
      - Start
  /extractor:
    get:
      summary: Get Extractor
      description: Get the list of schedules for all your extractors.
      operationId: getExtractor
      x-api-path-slug: extractor-get
      responses:
        200:
          description: OK
      tags:
      - Extractor
    post:
      summary: Post Extractor
      description: Schedule and extractor to run at a specific time.
      operationId: postExtractor
      x-api-path-slug: extractor-post
      parameters:
      - in: body
        name: Schedule Request Body
        description: Request body with the schema defined on the left
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Extractor
  /extractor/{extractorId}/:
    delete:
      summary: Delete Extractor Extractorid
      description: Delete an existing schedule.
      operationId: deleteExtractorExtractor
      x-api-path-slug: extractorextractorid-delete
      parameters:
      - in: path
        name: extractorId
        description: the id of the extractor with a schedule
      responses:
        200:
          description: OK
      tags:
      - Extractor
      - ExtractorId
    get:
      summary: Get Extractor Extractorid
      description: Get the schedule of a particular extractor.
      operationId: getExtractorExtractor
      x-api-path-slug: extractorextractorid-get
      parameters:
      - in: path
        name: extractorId
        description: the id of the extractor with a schedule
      responses:
        200:
          description: OK
      tags:
      - Extractor
      - ExtractorId