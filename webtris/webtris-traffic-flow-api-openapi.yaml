swagger: "2.0"
x-collection-name: WebTRIS
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: webtris.highwaysengland.co.uk
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v{version}/areas:
    get:
      summary: Returns list of areas
      description: Returns list of areas.
      operationId: Areas_Get
      x-api-path-slug: vversionareas-get
      parameters:
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Areas
  /v{version}/areas/{area_Ids}:
    get:
      summary: Returns details of selected area
      description: Returns details of selected area.
      operationId: Areas_Get
      x-api-path-slug: vversionareasarea-ids-get
      parameters:
      - in: path
        name: area_Ids
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Details
      - Of
      - Selected
      - Area
  /v{version}/quality/overall:
    get:
      summary: Get Site OverallQuality
      description: Get site overallquality.
      operationId: Quality_GetOverallDataQualityForSites
      x-api-path-slug: vversionqualityoverall-get
      parameters:
      - in: query
        name: end_date
        description: The end date of the report in the format ddmmyyyy (i
      - in: query
        name: sites
        description: Get site quality by site id delimited by ,
      - in: query
        name: start_date
        description: The start date of the report in the format ddmmyyyy (i
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - Site
      - OverallQuality
  /v{version}/quality/daily:
    get:
      summary: Get Site DailyQuality
      description: Get site dailyquality.
      operationId: Quality_GetDailyDataQualityForSite
      x-api-path-slug: vversionqualitydaily-get
      parameters:
      - in: query
        name: end_date
        description: The end date of the report in the format ddmmyyyy (i
      - in: query
        name: siteId
      - in: query
        name: start_date
        description: The start date of the report in the format ddmmyyyy (i
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - Site
      - DailyQuality
  /v{version}/reports/{report_type}:
    get:
      summary: Gets the daily report.
      description: Gets the daily report..
      operationId: Reports_Index
      x-api-path-slug: vversionreportsreport-type-get
      parameters:
      - in: query
        name: end_date
        description: The end date of the report in the format ddmmyyyy (i
      - in: query
        name: page
        description: The page offset to return
      - in: query
        name: page_size
        description: The number of rows to return
      - in: query
        name: reportSubTypeId
      - in: path
        name: report_type
        description: Report Type Id (i
      - in: query
        name: sites
        description: Comma separated list of site Ids
      - in: query
        name: start_date
        description: The start date of the report in the format ddmmyyyy (i
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - S
      - Daily
      - Report
  /v{version}/reports/{start_date}/to/{end_date}/{report_type}:
    get:
      summary: Gets the daily report.
      description: Gets the daily report..
      operationId: Reports_Index
      x-api-path-slug: vversionreportsstart-datetoend-datereport-type-get
      parameters:
      - in: path
        name: end_date
        description: The end date of the report in the format ddmmyyyy (i
      - in: query
        name: page
        description: The page offset to return
      - in: query
        name: page_size
        description: The number of rows to return
      - in: query
        name: reportSubTypeId
      - in: path
        name: report_type
        description: Report Type Id (i
      - in: query
        name: sites
        description: Comma separated list of site Ids
      - in: path
        name: start_date
        description: The start date of the report in the format ddmmyyyy (i
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - S
      - Daily
      - Report
  /v{version}/sites:
    get:
      summary: Get a list of sites
      description: Get a list of sites.
      operationId: Sites_Index
      x-api-path-slug: vversionsites-get
      parameters:
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Sites
  /v{version}/sites/{site_Ids}:
    get:
      summary: Get selected sites
      description: Get selected sites.
      operationId: Sites_Index
      x-api-path-slug: vversionsitessite-ids-get
      parameters:
      - in: path
        name: site_Ids
        description: site id
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - Selected
      - Sites
  /v{version}/sitetypes:
    get:
      summary: Return list of site types
      description: Return list of site types.
      operationId: SiteTypes_Index
      x-api-path-slug: vversionsitetypes-get
      parameters:
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - Return
      - List
      - Of
      - Site
      - Types
  /v{version}/sitetypes/{siteType_Id}/sites:
    get:
      summary: Returns the layer metadata for the LayerId specified.
      description: Returns the layer metadata for the layerid specified..
      operationId: SiteTypes_GetSitesForPublicFacingAPI
      x-api-path-slug: vversionsitetypessitetype-idsites-get
      parameters:
      - in: path
        name: siteType_Id
        description: 1 = MIDAS, 2 = TAME, 3 = TMU, 4 = TRADS Legacy
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Layer
      - Metadatathe
      - LayerId
      - Specified