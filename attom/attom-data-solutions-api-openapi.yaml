swagger: "2.0"
x-collection-name: ATTOM
x-complete: 1
info:
  title: Attom Data Solutions API
  description: attom-empowers-customers-with-better-property-data--we-warehouse-property-data-nationwide-with-myriad-data-points-on-each-parcel-including-ownership-information-latlong-square-footage-loan-types-sales-history-sales-comps-crime-schools-and-more-
  version: 1.0.0
host: search.onboard-apis.com
basePath: /communityapi/v2.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /property/id:
    get:
      summary: Returns a list of properties that fit a criteria.
      description: Get a list of property IDs within a specific geography that have
        a specific number of beds. Use orderby to choose how you want your results
        sorted.
      operationId: getPropertyIdList
      x-api-path-slug: propertyid-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: geoid
        description: A list of geographies that this property belongs to
      - in: query
        name: maxBeds
        description: The max Bed size to search from
      - in: query
        name: minBeds
        description: The min Bed size to search from
      - in: query
        name: orderby
        description: Sort Options
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Properties
      - That
      - Fit
      - Criteria
  /property/detail:
    get:
      summary: Returns property details based on an ID.
      description: Get property details based on its Onboard property ID.
      operationId: propertyDetails
      x-api-path-slug: propertydetail-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address
        description: The mailing address
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: id
        description: property id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Property
      - Details
      - Based
      - "On"
      - ID
  /property/address:
    get:
      summary: Returns properties within a zip code.
      description: Get a list of properties within a zip code. Use propertytype and
        order by to narrow down your results.
      operationId: adressList
      x-api-path-slug: propertyaddress-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: orderby
        description: Sorting Options
      - in: query
        name: page
        description: The current view index based on the pagesize and the total number
          of records available
      - in: query
        name: pagesize
        description: The number of records to be returned with the request
      - in: query
        name: postalcode
        description: The zip code or postal code to search
      - in: query
        name: propertytype
        description: A specific property classification such as Detached Single Family
      - in: query
        name: radius
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Properties
      - Within
      - Zip
      - Code
  /property/snapshot:
    get:
      summary: Returns properties and their characteristics that fit a criteria.
      description: Get a list of property snapshots within a specific city that are
        within a desired size range and a specific property type.
      operationId: propertySnapshot
      x-api-path-slug: propertysnapshot-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: cityname
        description: The name of the city to search from
      - in: query
        name: latitude
        description: The property latitude coordinate
      - in: query
        name: longitude
        description: The property longitude coordinate
      - in: query
        name: maxavmvalue
        description: The maximum AVM Valuey
      - in: query
        name: maxLotSize1
        description: The max Lot size 1 to search from
      - in: query
        name: maxtaxamt
        description: The total amount of taxes paid to the local taxing authority
      - in: query
        name: minavmvalue
        description: The minimum AVM Value
      - in: query
        name: minLotSize1
        description: The min Lot size 1 to search from
      - in: query
        name: mintaxamt
        description: The total amount of taxes paid to the local taxing authority
      - in: query
        name: orderby
        description: Sorting Options
      - in: query
        name: postalcode
      - in: query
        name: propertytype
        description: A specific property classification such as Detached Single Family
      - in: query
        name: radius
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Properties
      - Their
      - Characteristics
      - That
      - Fit
      - Criteria
  /property/basicprofile:
    get:
      summary: Returns basic property information and most recent transaction and
        taxes.
      description: Get basic property information and most recent transaction and
        taxes for a specific attom id.
      operationId: propertyBasicProfile
      x-api-path-slug: propertybasicprofile-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: attomid
        description: attom id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Basic
      - Property
      - Information
      - Most
      - Recent
      - Transaction
      - Taxes
  /property/expandedprofile:
    get:
      summary: Returns detailed property information and most recent transaction and
        taxes.
      description: Get a detailed property information and most recent transaction
        and taxes for a specific address.
      operationId: propertyExpandedProfile
      x-api-path-slug: propertyexpandedprofile-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Detailed
      - Property
      - Information
      - Most
      - Recent
      - Transaction
      - Taxes
  /property/detailwithschools:
    get:
      summary: Return schools within the attendance boundary of a property.
      description: Search for a property to have the property details returned, along
        with the schools in the associated attendance zones.
      operationId: propertyDetailsWithSchools
      x-api-path-slug: propertydetailwithschools-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: id
        description: property id
      responses:
        200:
          description: OK
      tags:
      - Return
      - Schools
      - Within
      - Attendance
      - Boundary
      - Of
      - Property
  /school/snapshot:
    get:
      summary: Return all schools within a defined radius from a point.
      description: Search for all schools that are located within a given radius around
        a given latitude and longitude.
      operationId: propertySchoolSnapshot
      x-api-path-slug: schoolsnapshot-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: filetypetext
        description: The type of school (public, private, or catholic can be selected)
      - in: query
        name: latitude
        description: The property latitude coordinate
      - in: query
        name: longitude
        description: The property longitude coordinate
      - in: query
        name: radius
      responses:
        200:
          description: OK
      tags:
      - Return
      - ""
      - Schools
      - Within
      - Defined
      - Radius
      - From
      - Point
  /school/detail:
    get:
      summary: Return details about a particular school.
      description: Search by school ID to return all of the available details about
        a school
      operationId: propertyDetails
      x-api-path-slug: schooldetail-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: id
        description: school id
      responses:
        200:
          description: OK
      tags:
      - Return
      - Details
      - About
      - Particular
      - School
  /school/districtdetail:
    get:
      summary: Return details about a particular school district.
      description: Search by district number to return all of the available details
        about a school district
      operationId: propertySchoolDistrictDetail
      x-api-path-slug: schooldistrictdetail-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: id
        description: district number
      responses:
        200:
          description: OK
      tags:
      - Return
      - Details
      - About
      - Particular
      - School
      - District
  /allevents/detail:
    get:
      summary: Returns all the events that have occurred on a specific address.
      description: Get a detail of all the events on a specific property based on
        its address.
      operationId: getAllEventsDetailAddress
      x-api-path-slug: alleventsdetail-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: API Security Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - ""
      - Events
      - That
      - Have
      - Occurred
      - "On"
      - Specific
      - Address
  /property/detailmortgage:
    get:
      summary: Returns property details mortgage based on ID.
      description: Get property details mortgage based on its Onboard property ID.
      operationId: propertyDetailsMortage
      x-api-path-slug: propertydetailmortgage-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: id
        description: property id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Property
      - Details
      - Mortgage
      - Based
      - "On"
      - ID
  /property/detailowner:
    get:
      summary: Returns property details owner based on an ID.
      description: Get property details owner based on its Onboard property ID.
      operationId: propertyDetailsOwner
      x-api-path-slug: propertydetailowner-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: id
        description: property id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Property
      - Details
      - Owner
      - Based
      - "On"
      - ID
  /property/detailmortgageowner:
    get:
      summary: Returns property details mortgageowner based on an ID.
      description: Get property details mortgageowner based on its Onboard property
        ID.
      operationId: propertyDetailsMortgageOwner
      x-api-path-slug: propertydetailmortgageowner-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: id
        description: property id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Property
      - Details
      - Mortgageowner
      - Based
      - "On"
      - ID
  /assessment/snapshot:
    get:
      summary: Returns assessment details for properties within a radius.
      description: Get snapshots of the properties within a radius of a property that
        have a total market value within a specified range.
      operationId: getAssessmentSnapshotTotal
      x-api-path-slug: assessmentsnapshot-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: maxmktttlvalue
        description: The estimated total market value from the local taxing authority
      - in: query
        name: minmktttlvalue
        description: The estimated total market value from the local taxing authority
      - in: query
        name: radius
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Assessment
      - Detailsproperties
      - Within
      - Radius
  /assessment/detail:
    get:
      summary: Returns assessment details for properties within a zip code.
      description: Get assessment details for properties within a zip code. Use propertytpe
        to select a specific property type for your search.
      operationId: assessmenDetailPropertyId
      x-api-path-slug: assessmentdetail-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: postalcode
        description: The postal code or zip code
      - in: query
        name: propertytype
        description: A specific property classification such as Detached Single Family
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Assessment
      - Detailsproperties
      - Within
      - Zip
      - Code
  /assessmenthistory/detail:
    get:
      summary: Returns assessment history and property details.
      description: Get a full detail of property characteristics and assessment history
        information for a specific property.
      operationId: assessmentHistoryDetailID
      x-api-path-slug: assessmenthistorydetail-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: id
        description: property id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Assessment
      - History
      - Property
      - Details
  /avm/snapshot:
    get:
      summary: Returns AVM details within a geography.
      description: Get a list of AVM snapshot records that fall within an Onboard
        GeoID with a specific value range. Use propertytpe to select a specific property
        type for your search.
      operationId: avmSnapshotGeoID
      x-api-path-slug: avmsnapshot-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: geoid
        description: A list of geographies that this property belongs to
      - in: query
        name: maxavmvalue
        description: This represents the estimated max value for the property
      - in: query
        name: minavmvalue
        description: This represents the estimated low value for the property
      - in: query
        name: propertytype
        description: A specific property classification such as Detached Single Family
      responses:
        200:
          description: OK
      tags:
      - Returns
      - AVM
      - Details
      - Within
      - Geography
  /avm/detail:
    get:
      summary: Returns AVM details for a property.
      description: Get AVM details for a specific address.
      operationId: avmDetailPostal
      x-api-path-slug: avmdetail-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - AVM
      - Detailsa
      - Property
  /attomavm/detail:
    get:
      summary: Returns the Attomized AVM and other property details .
      description: Get Attomized AVM and other property details for a specific address.
      operationId: attomAvmDetail
      x-api-path-slug: attomavmdetail-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: attomid
        description: attom id
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Attomized
      - AVM
      - Other
      - Property
      - Details
  /sale/snapshot:
    get:
      summary: Returns home sale information for properties within a geography.
      description: Get a list of home sale snapshots within a Onboard GeoID that sold
        within a date range and specified sale amount.
      operationId: getHomeSaleSnapshotsGeoId
      x-api-path-slug: salesnapshot-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: endsalesearchdate
        description: The standardized date for search purposes
      - in: query
        name: geoid
        description: A list of geographies that this property belongs to
      - in: query
        name: maxsaleamt
        description: The recorded amount of the sale transaction
      - in: query
        name: minsaleamt
        description: The recorded amount of the sale transaction
      - in: query
        name: propertytype
        description: A specific property classification such as Detached Single Family
      - in: query
        name: radius
      - in: query
        name: startsalesearchdate
        description: The standardized date for search purposes
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Home
      - Sale
      - Informationproperties
      - Within
      - Geography
  /sale/detail:
    get:
      summary: Returns sale information for a property.
      description: Get sales information for a specific address.
      operationId: getSaleDetailPostal
      x-api-path-slug: saledetail-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Sale
      - Informationa
      - Property
  /saleshistory/snapshot:
    get:
      summary: Returns sales history for a property.
      description: Get a sales history snapshot of a property based on an Onboard
        property ID.
      operationId: getSaleHistorySnapshotPropertyId
      x-api-path-slug: saleshistorysnapshot-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: id
        description: Onboard-assigned unique property identifier
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Sales
      - Historya
      - Property
  /saleshistory/basichistory:
    get:
      summary: Returns basic transaction and loan history on a property.
      description: Get the basic transaction and loan history on a property for a
        specific address.
      operationId: saleHistoryBasicHistory
      x-api-path-slug: saleshistorybasichistory-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Basic
      - Transaction
      - Loan
      - History
      - "On"
      - Property
  /saleshistory/expandedhistory:
    get:
      summary: Returns detailed transaction, pre-foreclosure and loan history on a
        property.
      description: Get the detailed transaction, pre-foreclosure and loan history
        on a property for a specific address.
      operationId: saleHistoryExpandedHistory
      x-api-path-slug: saleshistoryexpandedhistory-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Detailed
      - Transaction
      - ""
      - Pre-foreclosure
      - Loan
      - History
      - "On"
      - Property
  /saleshistory/detail:
    get:
      summary: Returns sales history for a property.
      description: Get a sales history snapshot of a property based on an address.
      operationId: getSaleHistoryDetailAddress
      x-api-path-slug: saleshistorydetail-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Sales
      - Historya
      - Property
  /salestrend/snapshot:
    get:
      summary: Returns sales trends for a given zip code in yearly intervals
      description: Get the average sale price, median sale price, and count of sales
        for the past 2 years in yearly intervals.
      operationId: getSalesTrendByYear
      x-api-path-slug: salestrendsnapshot-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: endmonth
        description: The end month to search from
      - in: query
        name: endyear
        description: The end year to search from
      - in: query
        name: geoid
        description: A list of geographies that this property belongs to
      - in: query
        name: interval
        description: The interval to search from
      - in: query
        name: startmonth
        description: The start month to search from
      - in: query
        name: startyear
        description: The start year to search from
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Sales
      - Trendsa
      - Given
      - Zip
      - Code
      - In
      - Yearly
      - Intervals
  /hierarchy/lookup:
    get:
      summary: Returns all boundaries a point falls within.
      description: This method allows you to pass a latitude and longitude point and
        geo type to retrieve a list of geographies that point falls within. Required
        input is a valid WKT (Well Known Text) point.
      operationId: getAreaHierarchyLookup
      x-api-path-slug: hierarchylookup-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: geoType
        description: known Geo Type
      - in: query
        name: latitude
        description: The property latitude coordinate
      - in: query
        name: longitude
        description: The property longitude coordinate
      - in: query
        name: WKTString
        description: WKTString parameters
      responses:
        200:
          description: OK
      tags:
      - Returns
      - ""
      - Boundaries
      - Point
      - Falls
      - Within
  /poi/geography:
    get:
      summary: Returns POIs based on zip code.
      description: This search returns a list of Points of Interest in proximity to
        the centroid of a zip code.
      operationId: getPOISearchGeography
      x-api-path-slug: poigeography-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: ApiKey
        description: Application Key
      - in: query
        name: PostalCodeKey
        description: This is the Postal Code
      - in: query
        name: RecordLimit
        description: This is RecordLimit
      - in: query
        name: SearchDistance
        description: This is SearchDistance
      - in: query
        name: Sort
        description: This is for Sortable Columns
      responses:
        200:
          description: OK
      tags:
      - Returns
      - POIs
      - Based
      - "On"
      - Zip
      - Code
  /poi/point:
    get:
      summary: Returns POIs based on point.
      description: This search returns a list of POI in proximity to a latitude/longitude.
      operationId: getPOISearchPoint
      x-api-path-slug: poipoint-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: BusinessCategory
        description: This is Business Category as per Lookup separated by pipe |
      - in: query
        name: Point
        description: This is the Point value
      - in: query
        name: RecordLimit
        description: This is RecordLimit
      - in: query
        name: SearchDistance
        description: This is SearchDistance
      - in: query
        name: Sort
        description: This is for Sortable Columns
      responses:
        200:
          description: OK
      tags:
      - Returns
      - POIs
      - Based
      - "On"
      - Point
  /poi/street+address:
    get:
      summary: Returns POIs based on an address.
      description: This search returns a list of POI in proximity to an address.
      operationId: getPOISearchPoint
      x-api-path-slug: poistreetaddress-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: RecordLimit
        description: This is RecordLimit
      - in: query
        name: SearchDistance
        description: This is SearchDistance
      - in: query
        name: Sort
        description: This is for Sortable Columns
      - in: query
        name: StreetAddress
        description: This is the Point value
      responses:
        200:
          description: OK
      tags:
      - Returns
      - POIs
      - Based
      - "On"
      - Address
  /business+category/lookup:
    get:
      summary: Returns business categories.
      description: This lookup is used to obtain a full list of Business Categories.
      operationId: getPOIBusinessCategoryLookup
      x-api-path-slug: businesscategorylookup-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Business
      - Categories
  /lob/lookup:
    get:
      summary: Returns lines of business categories.
      description: This lookup can be used to show the full list of Lines of Businesses
        (LOB), and which categories they belong to.
      operationId: getPOIlob
      x-api-path-slug: loblookup-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Lines
      - Of
      - Business
      - Categories
  /area/full:
    get:
      summary: Returns community information.
      description: This search returns community information for a specific geography.
      operationId: getCommunityAPIAreaFull
      x-api-path-slug: areafull-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: ApiKey
        description: Application Key
      - in: query
        name: AreaId
        description: This is the Area ID to search
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Community
      - Information
  /attribute/lookup:
    get:
      summary: Returns available data fields.
      description: This lookup returns the full list of over 375 data fields that
        are available in the Community API.
      operationId: getCommunityAPIAttributeLookup
      x-api-path-slug: attributelookup-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Available
      - Data
      - Fields