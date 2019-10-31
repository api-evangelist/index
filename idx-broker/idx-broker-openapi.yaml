swagger: "2.0"
x-collection-name: IDX Broker
x-complete: 1
info:
  title: IDX API 1.4.0 Test Runner
  description: idx-broker-api-calls-in-version-1-4-0required-environment-variable-url-environment-variable-for-request-headers-environment-variable-partner-key-client-account-with-at-least-one-featured-listingtests-are-in-this-order-as-variables-such-as-listing-id-and-approved-mls-are-passed-to-subsequent-api-calls-
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /mls/approvedmls:
    get:
      summary: Get Approved MLS
      description: |-
        This method provides all of the IDX IDs and names for all of the paperwork approved MLSs on the client's account.

        Note: This method was previously camelcased as "approvedMLS" but was made lower case to fit the API naming convention. Calls to "approvedMLS" will be forwarded to "approvedmls" and "approvedMLS" is listed as deprecated in the method list.
      operationId: MlsApprovedmlsGet
      x-api-path-slug: mlsapprovedmls-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Approved
      - MLS
  /mls/age/{approvedMLS}:
    get:
      summary: Get Mls Age Approved MLS
      description: 'TODO: Add Description'
      operationId: MlsAgeByApprovedMLSGet
      x-api-path-slug: mlsageapprovedmls-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - Age
      - Approved
      - MLS
  /mls/cities/{approvedMLS}:
    get:
      summary: Get Mls Cities Approved MLS
      description: All cities represented in the current set of MLS data are available
        from this method.
      operationId: MlsCitiesByApprovedMLSGet
      x-api-path-slug: mlscitiesapprovedmls-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - Cities
      - Approved
      - MLS
  /mls/listcomponents:
    get:
      summary: Get Mls List Components
      description: This is a simple, access anywhere, method for getting a list of
        all API components available.
      operationId: MlsListcomponentsGet
      x-api-path-slug: mlslistcomponents-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - List
      - Components
  /mls/listmethods:
    get:
      summary: Get Mls Listmethods
      description: A simple method for listing all available methods in the current
        API component. This method will also list which request methods (GET, PUT,
        POST, or DELETE) are supported by each method in addition to each method status.
      operationId: MlsListmethodsGet
      x-api-path-slug: mlslistmethods-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - Listmethods
  /mls/postalcodes/{approvedMLS}:
    get:
      summary: Get Mls Addalcodes Approvedmls
      description: All postal codes represented in the current set of MLS data are
        available from this method.
      operationId: MlsPostalcodesByApprovedMLSGet
      x-api-path-slug: mlspostalcodesapprovedmls-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - Alcodes
      - Approvedmls
  /mls/prices/{approvedMLS}:
    get:
      summary: Get Mls Prices Approvedmls
      description: The sum total of properties listed in a given MLS as well as sums
        for each property type in the MLS.
      operationId: MlsPricesByApprovedMLSGet
      x-api-path-slug: mlspricesapprovedmls-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - Prices
      - Approvedmls
  /mls/propertycount/{approvedMLS}:
    get:
      summary: Get Mls Propertycount Approvedmls
      description: Gives a total number of listings available for a given city, county,
        or zipcode
      operationId: MlsPropertycountByApprovedMLSGet
      x-api-path-slug: mlspropertycountapprovedmls-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: query
        name: countSpecifier
      - in: query
        name: countType
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - Propertycount
      - Approvedmls
  /mls/propertytypes/{approvedMLS}:
    get:
      summary: Get Mls Propertytypes Approvedmls
      description: Gives the property type information for all types that are available
        on a given MLS.
      operationId: MlsPropertytypesByApprovedMLSGet
      x-api-path-slug: mlspropertytypesapprovedmls-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - Propertytypes
      - Approvedmls
  /mls/searchfields/{approvedMLS}:
    get:
      summary: Get Mls Searchfields Approvedmls
      description: All the fields in a given MLS that are currently allowed to be
        searched according to MLS guidelines.
      operationId: MlsSearchfieldsByApprovedMLSGet
      x-api-path-slug: mlssearchfieldsapprovedmls-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - Searchfields
      - Approvedmls
  /mls/searchfieldvalues/{approvedMLS}:
    get:
      summary: Get Mls Search Field Values Approved MLS
      description: Field values in a given MLS that are currently allowed to be searched
        according to MLS guidelines.
      operationId: MlsSearchfieldvaluesByApprovedMLSGet
      x-api-path-slug: mlssearchfieldvaluesapprovedmls-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: query
        name: mlsPtID
      - in: query
        name: name
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - Search
      - Field
      - Values
      - Approved
      - MLS
  /mls/zipcodes/{approvedMLS}:
    get:
      summary: Get Mls Zipcodes Approved MLS
      description: All zip codes represented in the current set of MLS data are available
        from this method.
      operationId: MlsZipcodesByApprovedMLSGet
      x-api-path-slug: mlszipcodesapprovedmls-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - Zipcodes
      - Approved
      - MLS
  /clients/agents:
    get:
      summary: Get Agents
      description: View agent information on a multi-user account.
      operationId: ClientsAgentsGet
      x-api-path-slug: clientsagents-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Agents
  /clients/apiversion:
    get:
      summary: Get Apiversion
      description: Get the default api version.
      operationId: ClientsApiversionGet
      x-api-path-slug: clientsapiversion-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Apiversion
  /clients/cities:
    get:
      summary: Get Cities
      description: Returns the cities available in each of a client's city lists.
      operationId: ClientsCitiesGet
      x-api-path-slug: clientscities-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Cities
  /clients/citieslistname:
    get:
      summary: Get Cities List Name
      description: Returns the IDs and names for each of a client's city lists including
        MLS city lists.
      operationId: ClientsCitieslistnameGet
      x-api-path-slug: clientscitieslistname-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Cities
      - List
      - Name
  /clients/counties:
    get:
      summary: Get Counties
      description: Returns the counties available in each of a client's county lists.
      operationId: ClientsCountiesGet
      x-api-path-slug: clientscounties-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Counties
  /clients/countieslistname:
    get:
      summary: Get Countieslistname
      description: Returns the IDs and names for each of a client's counties lists
        including MLS counties lists.
      operationId: ClientsCountieslistnameGet
      x-api-path-slug: clientscountieslistname-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Countieslistname
  /clients/dynamicwrapperurl:
    post:
      summary: Post Dynamicwrapperurl
      description: Set wrapper URL. This is the global url.
      operationId: ClientsDynamicwrapperurlPost
      x-api-path-slug: clientsdynamicwrapperurl-post
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: formData
        name: dynamicURL
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Dynamicwrapperurl
  /clients/featured:
    get:
      summary: Get Featured
      description: Returns a basic set of information for all of the client's featured
        (active) properties
      operationId: ClientsFeaturedGet
      x-api-path-slug: clientsfeatured-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Featured
  /clients/listallowedfields/{approvedMLS}/{featuredId}:
    get:
      summary: Get List Allowed Fields Approved MLS Featured
      description: Returns the allowed returnable fields for a given listingID.
      operationId: ClientsListallowedfieldsByApprovedMLSAndFeaturedIdGet
      x-api-path-slug: clientslistallowedfieldsapprovedmlsfeaturedid-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: path
        name: featuredId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - List
      - Owed
      - Fields
      - Approved
      - MLS
      - Featured
  /clients/listcomponents:
    get:
      summary: Get Listcomponents
      description: This is a simple, access anywhere, method for getting a list of
        all API components available.
      operationId: ClientsListcomponentsGet
      x-api-path-slug: clientslistcomponents-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Listcomponents
  /clients/listing/{approvedMLS}/{featuredId}:
    get:
      summary: Get Listing Approved MLS Featuredid
      description: Returns the detailed information for a given listingID.
      operationId: ClientsListingByApprovedMLSAndFeaturedIdGet
      x-api-path-slug: clientslistingapprovedmlsfeaturedid-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: path
        name: featuredId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Approved
      - MLS
      - Featuredid
  /clients/listmethods:
    get:
      summary: Get List Methods
      description: A simple method for listing all available methods in the current
        API component.
      operationId: ClientsListmethodsGet
      x-api-path-slug: clientslistmethods-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - List
      - Methods
  /clients/offices:
    get:
      summary: Get Offices
      description: View all offices on a mutli-user account.
      operationId: ClientsOfficesGet
      x-api-path-slug: clientsoffices-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Offices
  /clients/postalcodes:
    get:
      summary: Get Addalcodes
      description: Returns the postalcodes available in each of a client's postalcode
        lists.
      operationId: ClientsPostalcodesGet
      x-api-path-slug: clientspostalcodes-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Alcodes
  /clients/postalcodeslistname:
    get:
      summary: Get Addalcodeslistname
      description: Returns the IDs and names for each of a client's postalcode lists
        including MLS postalcode lists.
      operationId: ClientsPostalcodeslistnameGet
      x-api-path-slug: clientspostalcodeslistname-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Alcodeslistname
  /clients/savedlinks:
    get:
      summary: Get Saved Link
      description: Getclient saved links
      operationId: ClientsSavedlinksGet
      x-api-path-slug: clientssavedlinks-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Link
    put:
      summary: Put Saved Link
      description: Create a new client saved link
      operationId: ClientsSavedlinksPut
      x-api-path-slug: clientssavedlinks-put
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: formData
        name: linkName
      - in: formData
        name: linkTitle
      - in: header
        name: outputtype
      - in: formData
        name: pageTitle
      - in: formData
        name: queryString[hp]
      - in: formData
        name: queryString[idxID]
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Link
  /clients/properties/{savedLinkId}:
    get:
      summary: Get Properties Saved Link
      description: Get client saved links results
      operationId: ClientsPropertiesBySavedLinkIdGet
      x-api-path-slug: clientspropertiessavedlinkid-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      - in: path
        name: savedLinkId
      responses:
        200:
          description: OK
      tags:
      - Properties
      - Saved
      - Link
  /clients/savedlinks/{savedLinkId}:
    post:
      summary: Post Saved Link Saved Link
      description: Update a client saved link
      operationId: ClientsSavedlinksBySavedLinkIdPost
      x-api-path-slug: clientssavedlinkssavedlinkid-post
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: formData
        name: linkName
      - in: formData
        name: linkTitle
      - in: header
        name: outputtype
      - in: formData
        name: pageTitle
      - in: formData
        name: queryString[hp]
      - in: formData
        name: queryString[idxID]
      - in: path
        name: savedLinkId
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Link
      - Saved
      - Link
    delete:
      summary: Delete Saved Link Saved Link
      description: Delete a client saved link
      operationId: ClientsSavedlinksBySavedLinkIdDelete
      x-api-path-slug: clientssavedlinkssavedlinkid-delete
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: formData
        name: linkName
      - in: formData
        name: linkTitle
      - in: header
        name: outputtype
      - in: formData
        name: pageTitle
      - in: formData
        name: queryString[hp]
      - in: formData
        name: queryString[idxID]
      - in: path
        name: savedLinkId
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Link
      - Saved
      - Link
  /clients/searchquery:
    get:
      summary: Get Search Query
      description: Performs search and returns the results.
      operationId: ClientsSearchqueryGet
      x-api-path-slug: clientssearchquery-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Search
      - Query
  /clients/soldpending:
    get:
      summary: Get Sold Pending
      description: Returns a basic set of information for all of the client's sold
        and pending properties.
      operationId: ClientsSoldpendingGet
      x-api-path-slug: clientssoldpending-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Sold
      - Pending
  /clients/supplemental:
    get:
      summary: Get Supplemental
      description: Get supplemental listings.
      operationId: ClientsSupplementalGet
      x-api-path-slug: clientssupplemental-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Supplemental
    put:
      summary: Put Supplemental
      description: Create a new supplemental listing.
      operationId: ClientsSupplementalPut
      x-api-path-slug: clientssupplemental-put
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: formData
        name: images[hp]
      - in: formData
        name: likeIdxID
      - in: formData
        name: likeMlsPtID
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Supplemental
  /clients/supplemental/{suppId}:
    post:
      summary: Post Supplemental
      description: Update a supplemental listing.
      operationId: ClientsSupplementalBySuppIdPost
      x-api-path-slug: clientssupplementalsuppid-post
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: formData
        name: images[hp]
      - in: formData
        name: likeIdxID
      - in: formData
        name: likeMlsPtID
      - in: header
        name: outputtype
      - in: path
        name: suppId
      responses:
        200:
          description: OK
      tags:
      - Supplemental
    delete:
      summary: Delete Supplemental
      description: Delete a supplemental listing.
      operationId: ClientsSupplementalBySuppIdDelete
      x-api-path-slug: clientssupplementalsuppid-delete
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      - in: path
        name: suppId
      responses:
        200:
          description: OK
      tags:
      - Supplemental
  /clients/systemlinks:
    get:
      summary: Get System Links
      description: Gathers all the pages system pages (search, featured, contact,
        etc) that can be directly linked to without additional property information
        being included in the URL.
      operationId: ClientsSystemlinksGet
      x-api-path-slug: clientssystemlinks-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - System
      - Links
  /clients/widgetsrc:
    get:
      summary: Get Wgetsrc
      description: Gather all the URLs for javascript widgets on the user's account.
        These widgets can then be placed on the user's main site via the included
        URLs.
      operationId: ClientsWidgetsrcGet
      x-api-path-slug: clientswidgetsrc-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Wgetsrc
  /clients/wrappercache:
    delete:
      summary: Delete Wrapper Cache
      description: Delete wrapper cache.
      operationId: ClientsWrappercacheDelete
      x-api-path-slug: clientswrappercache-delete
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Wrapper
      - Cache
  /clients/zipcodes:
    get:
      summary: Get Zipcodes
      description: Returns the zipcodes available in each of a client's zipcode lists.
      operationId: ClientsZipcodesGet
      x-api-path-slug: clientszipcodes-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Zipcodes
  /leads/lead:
    get:
      summary: Get Leads Lead
      description: |-
        Get information for one or multiple leads.

        Example Request: https://api.idxbroker.com/leads/lead?interval=24&startDatetime=2016-01-01+23:59:59&dateType=subscribeDate

        For Data on a specific lead add/LEAD_ID_HERE

        Example: https://api.idxbroker.com/leads/lead/123
      operationId: LeadsLeadGet
      x-api-path-slug: leadslead-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Lead
    put:
      summary: Put Leads Lead
      description: |-
        Get information for one or multiple leads.

        Example Request: https://api.idxbroker.com/leads/lead?interval=24&startDatetime=2016-01-01+23:59:59&dateType=subscribeDate

        For Data on a specific lead add/LEAD_ID_HERE

        Example: https://api.idxbroker.com/leads/lead/123
      operationId: LeadsLeadPut
      x-api-path-slug: leadslead-put
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: formData
        name: email
      - in: formData
        name: firstName
      - in: formData
        name: lastName
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Lead
  /leads/lead/{leadId}:
    post:
      summary: Post Leads Lead Lead
      description: |-
        Post information for a lead.


        Example: https://api.idxbroker.com/leads/lead/123
      operationId: LeadsLeadByLeadIdPost
      x-api-path-slug: leadsleadleadid-post
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: formData
        name: email
      - in: formData
        name: firstName
      - in: formData
        name: lastName
      - in: path
        name: leadId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Lead
      - Lead
    delete:
      summary: Delete Leads Lead Lead
      description: |-
        Delete Lead

        Example: https://api.idxbroker.com/leads/lead/123
      operationId: LeadsLeadByLeadIdDelete
      x-api-path-slug: leadsleadleadid-delete
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Lead
      - Lead
  /leads/note/{leadId}:
    put:
      summary: Put Leads Note
      description: Add new note information for a lead.
      operationId: LeadsNoteByLeadIdPut
      x-api-path-slug: leadsnoteleadid-put
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: formData
        name: note
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Note
  /leads/note/{noteId}:
    get:
      summary: Get Leads Not
      description: Get note information for a lead.
      operationId: LeadsNoteByNoteIdGet
      x-api-path-slug: leadsnotenoteid-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: noteId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Not
  /leads/note/{leadId}/{noteId}:
    post:
      summary: Post Leads Note
      description: Post new note information for a lead.
      operationId: LeadsNoteByLeadIdAndNoteIdPost
      x-api-path-slug: leadsnoteleadidnoteid-post
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: formData
        name: note
      - in: path
        name: noteId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Note
    delete:
      summary: Delete Leads Note
      description: Delete note information for a lead.
      operationId: LeadsNoteByLeadIdAndNoteIdDelete
      x-api-path-slug: leadsnoteleadidnoteid-delete
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: formData
        name: note
      - in: path
        name: noteId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Note
  /leads/property/{leadId}:
    get:
      summary: Get Leads Property
      description: Get a property information for a lead.
      operationId: LeadsPropertyByLeadIdGet
      x-api-path-slug: leadspropertyleadid-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Property
    put:
      summary: Put Leads Property
      description: Add new property information for a lead.
      operationId: LeadsPropertyByLeadIdPut
      x-api-path-slug: leadspropertyleadid-put
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      - in: formData
        name: propertyName
      - in: formData
        name: property[idxID]
      - in: formData
        name: property[listingID]
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Property
  /leads/property/{leadId}/{propId}:
    post:
      summary: Post Leads Property
      description: Update a property information for a lead.
      operationId: LeadsPropertyByLeadIdAndPropIdPost
      x-api-path-slug: leadspropertyleadidpropid-post
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      - in: formData
        name: propertyName
      - in: formData
        name: property[idxID]
      - in: formData
        name: property[listingID]
      - in: path
        name: propId
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Property
    delete:
      summary: Delete Leads Property
      description: Delete a property information for a lead.
      operationId: LeadsPropertyByLeadIdAndPropIdDelete
      x-api-path-slug: leadspropertyleadidpropid-delete
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      - in: path
        name: propId
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Property
  /leads/search/{leadId}:
    get:
      summary: Get Leads Search
      description: Get saved search information for a lead.
      operationId: LeadsSearchByLeadIdGet
      x-api-path-slug: leadssearchleadid-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Search
    put:
      summary: Put Leads Search
      description: New search information for a lead.
      operationId: LeadsSearchByLeadIdPut
      x-api-path-slug: leadssearchleadid-put
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      - in: formData
        name: searchName
      - in: formData
        name: search[hp]
      - in: formData
        name: search[idxID]
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Search
  /leads/search/{leadId}/{searchId}:
    post:
      summary: Post Leads Search
      description: Update search information for a lead.
      operationId: LeadsSearchByLeadIdAndSearchIdPost
      x-api-path-slug: leadssearchleadidsearchid-post
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      - in: path
        name: searchId
      - in: formData
        name: searchName
      - in: formData
        name: search[hp]
      - in: formData
        name: search[idxID]
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Search
    delete:
      summary: Delete Leads Search
      description: Delete search information for a lead.
      operationId: LeadsSearchByLeadIdAndSearchIdDelete
      x-api-path-slug: leadssearchleadidsearchid-delete
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      - in: path
        name: searchId
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Search
  /leads/leadtraffic/{leadId}:
    get:
      summary: Get Leads Lead Traffic
      description: Get information on a lead's traffic history.
      operationId: LeadsLeadtrafficByLeadIdGet
      x-api-path-slug: leadsleadtrafficleadid-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: path
        name: leadId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Lead
      - Traffic
  /leads/listcomponents:
    get:
      summary: Get Leads List Components
      description: This is a simple, access anywhere, method for getting a list of
        all API components available.
      operationId: LeadsListcomponentsGet
      x-api-path-slug: leadslistcomponents-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - List
      - Components
  /leads/listmethods:
    get:
      summary: Get Leads List Methods
      description: A simple method for listing all available methods in the current
        API component.
      operationId: LeadsListmethodsGet
      x-api-path-slug: leadslistmethods-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - List
      - Methods
  /partners/aggregatedagents:
    get:
      summary: Get Partners Aggregated Agents
      description: Get a list of all agents for your clients.
      operationId: PartnersAggregatedagentsGet
      x-api-path-slug: partnersaggregatedagents-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Aggregated
      - Agents
  /partners/aggregatedfeatured:
    get:
      summary: Get Partners Aggregated Featured
      description: Get a list of featured MLS properties.
      operationId: PartnersAggregatedfeaturedGet
      x-api-path-slug: partnersaggregatedfeatured-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Aggregated
      - Featured
  /partners/aggregatedleads:
    get:
      summary: Get Partners Aggregated Leads
      description: Get a list of all leads.
      operationId: PartnersAggregatedleadsGet
      x-api-path-slug: partnersaggregatedleads-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Aggregated
      - Leads
  /partners/aggregatedleadtraffic:
    get:
      summary: Get Partners Aggregated Lead Traffic
      description: Get a list of all leads traffic history.
      operationId: PartnersAggregatedleadtrafficGet
      x-api-path-slug: partnersaggregatedleadtraffic-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Aggregated
      - Lead
      - Traffic
  /partners/aggregatedlistingstatus:
    get:
      summary: Get Partners Aggregated Listing Status
      description: This method gives the status for all MLS listings (not supplemental)
        broken down by client account ID. This includes sold/pending listings with
        an unknown status which are not usually returned by sold/pending api methods.
        This is helpful if you need to know when previously gathered featured properties
        have left the market.
      operationId: PartnersAggregatedlistingstatusGet
      x-api-path-slug: partnersaggregatedlistingstatus-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Aggregated
      - Listing
      - Status
  /partners/aggregatedproperties:
    get:
      summary: Get Partners Aggregated Properties
      description: Get a list of all lead saved properties.
      operationId: PartnersAggregatedpropertiesGet
      x-api-path-slug: partnersaggregatedproperties-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Aggregated
      - Properties
  /partners/aggregatedsearches:
    get:
      summary: Get Partners Aggregated Searches
      description: Get a list of all lead saved searches.
      operationId: PartnersAggregatedsearchesGet
      x-api-path-slug: partnersaggregatedsearches-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Aggregated
      - Searches
  /partners/aggregatedsoldpending:
    get:
      summary: Get Partners Aggregated Sold Pending
      description: Get a list of sold/pending MLS properties.
      operationId: PartnersAggregatedsoldpendingGet
      x-api-path-slug: partnersaggregatedsoldpending-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Aggregated
      - Sold
      - Pending
  /partners/aggregatedsupplemental:
    get:
      summary: Get Partners Aggregated Supplemental
      description: Get a list of supplemental (non-MLS) properties.
      operationId: PartnersAggregatedsupplementalGet
      x-api-path-slug: partnersaggregatedsupplemental-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Aggregated
      - Supplemental
  /partners/clients:
    get:
      summary: Get Partners Clients
      description: A list of clients available to a given partner. The list of clients
        can be filtered by GET values.
      operationId: PartnersClientsGet
      x-api-path-slug: partnersclients-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Clients
  /partners/listcomponents:
    get:
      summary: Get Partners List Components
      description: This is a simple, access anywhere, method for getting a list of
        all API components available.
      operationId: PartnersListcomponentsGet
      x-api-path-slug: partnerslistcomponents-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - List
      - Components
  /partners/listmethods:
    get:
      summary: Get Partners List Methods
      description: A simple method for listing all available methods in the current
        API component.
      operationId: PartnersListmethodsGet
      x-api-path-slug: partnerslistmethods-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - List
      - Methods
  /partners/propertytypes:
    get:
      summary: Get Partners Property Types
      description: Gives the names and IDs of all available property types. This method
        differs from the property type lookup method in the client API component in
        that it can look up property types for any active Platinum MLS, not just those
        for which the client is a member.
      operationId: PartnersPropertytypesGet
      x-api-path-slug: partnerspropertytypes-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - Property
      - Types