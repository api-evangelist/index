swagger: "2.0"
x-collection-name: School Digger
x-complete: 1
info:
  title: School Digger API V1
  description: get-detailed-data-on-over-120000-schools-and-18500-districts-in-the-u-s-
  termsOfService: https://developer.schooldigger.com/termsofservice
  contact:
    name: SchoolDigger
    email: api@schooldigger.com
  version: v1
host: api.schooldigger.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/districts:
    get:
      summary: Returns a list of districts
      description: Search the SchoolDigger database for districts. You may use any
        combination of criteria as query parameters.
      operationId: Districts_GetAllDistricts
      x-api-path-slug: v1districts-get
      parameters:
      - in: query
        name: appID
        description: Your API app id
      - in: query
        name: appKey
        description: Your API app key
      - in: query
        name: boundaryAddress
        description: Full U
      - in: query
        name: boxLatitudeNW
        description: Search for districts within a box defined by (BoxLatitudeNW/BoxLongitudeNW)
          to (BoxLongitudeSE/BoxLatitudeSE) (optional)
      - in: query
        name: boxLatitudeSE
        description: Search for districts within a box defined by (BoxLatitudeNW/BoxLongitudeNW)
          to (BoxLongitudeSE/BoxLatitudeSE) (optional)
      - in: query
        name: boxLongitudeNW
        description: Search for districts within a box defined by (BoxLatitudeNW/BoxLongitudeNW)
          to (BoxLongitudeSE/BoxLatitudeSE) (optional)
      - in: query
        name: boxLongitudeSE
        description: Search for districts within a box defined by (BoxLatitudeNW/BoxLongitudeNW)
          to (BoxLongitudeSE/BoxLatitudeSE) (optional)
      - in: query
        name: city
        description: Search for districts in this city (optional)
      - in: query
        name: distanceMiles
        description: Search for districts within (distanceMiles) of (nearLatitude)/(nearLongitude)
          (Default 5 miles) (optional) (Pro, Enterprise API levels only)
      - in: query
        name: isInBoundaryOnly
        description: Return only the districts that include given location (nearLatitdue/nearLongitude)
          or (nearAddress) in its attendance boundary (Enterprise API level only)
      - in: query
        name: nearLatitude
        description: Search for districts within (distanceMiles) of (nearLatitude)/(nearLongitude)
          (e
      - in: query
        name: nearLongitude
        description: Search for districts within (distanceMiles) of (nearLatitude)/(nearLongitude)
          (e
      - in: query
        name: page
        description: 'Page number to retrieve (optional, default: 1)'
      - in: query
        name: perPage
        description: 'Number of districts to retrieve on a page (50 max) (optional,
          default: 10)'
      - in: query
        name: q
        description: 'Search term - note: will match district name or city (optional)'
      - in: query
        name: sortBy
        description: Sort list
      - in: query
        name: st
        description: Two character state (e
      - in: query
        name: zip
        description: Search for districts in this 5-digit zip code (optional)
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/districts/{id}:
    get:
      summary: Returns a detailed record for one district
      description: Retrieve a single district record from the SchoolDigger database
      operationId: Districts_GetDistrict
      x-api-path-slug: v1districtsid-get
      parameters:
      - in: query
        name: appID
        description: Your API app id
      - in: query
        name: appKey
        description: Your API app key
      - in: path
        name: id
        description: The 7 digit District ID (e
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/rankings/districts/{st}:
    get:
      summary: Returns a SchoolDigger district ranking list
      description: ""
      operationId: v1.rankings.districts.st.get
      x-api-path-slug: v1rankingsdistrictsst-get
      parameters:
      - in: query
        name: appID
        description: Your API app id
      - in: query
        name: appKey
        description: Your API app key
      - in: query
        name: page
        description: 'Page number to retrieve (optional, default: 1)'
      - in: query
        name: perPage
        description: 'Number of districts to retrieve on a page (50 max) (optional,
          default: 10)'
      - in: path
        name: st
        description: Two character state (e
      - in: query
        name: year
        description: The ranking year (leave blank for most recent year)
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/rankings/schools/{st}:
    get:
      summary: Returns a SchoolDigger school ranking list
      description: ""
      operationId: v1.rankings.schools.st.get
      x-api-path-slug: v1rankingsschoolsst-get
      parameters:
      - in: query
        name: appID
        description: Your API app id
      - in: query
        name: appKey
        description: Your API app key
      - in: query
        name: level
        description: 'Level of ranking: Elementary, Middle, or High'
      - in: query
        name: page
        description: 'Page number to retrieve (optional, default: 1)'
      - in: query
        name: perPage
        description: 'Number of schools to retrieve on a page (50 max) (optional,
          default: 10)'
      - in: path
        name: st
        description: Two character state (e
      - in: query
        name: year
        description: The ranking year (leave blank for most recent year)
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/schools:
    get:
      summary: Returns a list of schools
      description: Search the SchoolDigger database for schools. You may use any combination
        of criteria as query parameters.
      operationId: Schools_GetAllSchools
      x-api-path-slug: v1schools-get
      parameters:
      - in: query
        name: appID
        description: Your API app id
      - in: query
        name: appKey
        description: Your API app key
      - in: query
        name: boundaryAddress
        description: Full U
      - in: query
        name: boxLatitudeNW
        description: Search for schools within a box defined by (boxLatitudeNW/boxLongitudeNW)
          to (boxLongitudeSE/boxLatitudeSE) (optional)
      - in: query
        name: boxLatitudeSE
        description: Search for schools within a box defined by (boxLatitudeNW/boxLongitudeNW)
          to (boxLongitudeSE/boxLatitudeSE) (optional)
      - in: query
        name: boxLongitudeNW
        description: Search for schools within a box defined by (boxLatitudeNW/boxLongitudeNW)
          to (boxLongitudeSE/boxLatitudeSE) (optional)
      - in: query
        name: boxLongitudeSE
        description: Search for schools within a box defined by (boxLatitudeNW/boxLongitudeNW)
          to (boxLongitudeSE/boxLatitudeSE) (optional)
      - in: query
        name: city
        description: Search for schools in this city (optional)
      - in: query
        name: distanceMiles
        description: Search for schools within (distanceMiles) of (nearLatitude)/(nearLongitude)
          (Default 5 miles) (optional) (Pro, Enterprise API levels only)
      - in: query
        name: districtID
        description: Search for schools within this district (7 digit district id)
          (optional)
      - in: query
        name: isCharter
        description: True = return only charter schools, False = return only non-charter
          schools (optional) (Pro, Enterprise API levels only)
      - in: query
        name: isInBoundaryOnly
        description: Return only the schools that include given location (nearLatitdue/nearLongitude)
          or (nearAddress) in its attendance boundary (Enterprise API level only)
      - in: query
        name: isMagnet
        description: True = return only magnet schools, False = return only non-magnet
          schools (optional) (Pro, Enterprise API levels only)
      - in: query
        name: isTitleI
        description: True = return only Title I schools, False = return only non-Title
          I schools (optional) (Pro, Enterprise API levels only)
      - in: query
        name: isTitleISchoolwide
        description: True = return only Title I schoolwide schools, False = return
          only non-Title I Schoolwide schools (optional) (Pro, Enterprise API levels
          only)
      - in: query
        name: isVirtual
        description: True = return only virtual schools, False = return only non-virtual
          schools (optional) (Pro, Enterprise API levels only)
      - in: query
        name: level
        description: Search for schools at this level
      - in: query
        name: nearLatitude
        description: Search for schools within (distanceMiles) of (nearLatitude)/(nearLongitude)
          (e
      - in: query
        name: nearLongitude
        description: Search for schools within (distanceMiles) of (nearLatitude)/(nearLongitude)
          (e
      - in: query
        name: page
        description: 'Page number to retrieve (optional, default: 1)'
      - in: query
        name: perPage
        description: 'Number of schools to retrieve on a page (50 max) (optional,
          default: 10)'
      - in: query
        name: q
        description: 'Search term - note: will match school name or city (optional)'
      - in: query
        name: sortBy
        description: Sort list
      - in: query
        name: st
        description: Two character state (e
      - in: query
        name: zip
        description: Search for schools in this 5-digit zip code (optional)
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/schools/{id}:
    get:
      summary: Returns a detailed record for one school
      description: Retrieve a school record from the SchoolDigger database
      operationId: Schools_GetSchool
      x-api-path-slug: v1schoolsid-get
      parameters:
      - in: query
        name: appID
        description: Your API app id
      - in: query
        name: appKey
        description: Your API app key
      - in: path
        name: id
        description: The 12 digit School ID (e
      responses:
        200:
          description: OK
      tags:
      - ""