swagger: "2.0"
x-collection-name: Bureau of Economic Analysis
x-complete: 1
info:
  title: The Bureau of Economic Analysis (BEA) API
  description: he-data-api-provides-programmatic-access-to-bea-published-economic-statistics-using-industrystandard-methods-and-procedures--beas-data-api-includes-methods-for-retrieving-a-subset-of-our-statistical-data-and-the-metadata-that-describes-it-
  version: v1
host: www.bea.gov/api/data?&UserID=Your-36CharacterKey&method=getparameterlist&datasetname=RegionalData&
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  data/:
    get:
      summary: Economic Statistics
      description: Economic Statistics
      operationId: getData
      x-api-path-slug: data-get
      parameters:
      - in: query
        name: datasetname
      - in: query
        name: method
      - in: query
        name: ParameterName
      - in: query
        name: ResultFormat
      - in: query
        name: UserID
        description: Your user id
      responses:
        200:
          description: OK
      tags:
      - Economic
      - Statistics