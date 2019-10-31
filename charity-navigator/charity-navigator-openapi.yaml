swagger: "2.0"
x-collection-name: Charity Navigator
x-complete: 1
info:
  title: CharityNavigatorDataAPI
  description: the-charity-navigator-data-api-provides-access-to-charity-navigatorsratings-research-content-and-charitable-organization-profiles-
  version: 1.0.0
host: api.data.charitynavigator.org
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Organizations:
    get:
      summary: Get Organizations
      description: |-
        Retrieve a list of the organizations available in the Charity Navigator Data
        Store. Allows paged retrieval, simple and advanced searching.
      operationId: searchOrganizations
      x-api-path-slug: organizations-get
      parameters:
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      - in: query
        name: categoryID
        description: ID of a Category
      - in: query
        name: causeID
        description: ID of a Cause
      - in: query
        name: cfcCharities
        description: Specifies whether to include or exclude organizations that are
          included inthe Combined Federal Campaign, the largest workplace giving campaign
          in USA
      - in: query
        name: city
        description: Filters search results to include only organizations in cities
          whose namesmatch the specified string
      - in: query
        name: donorPrivacy
        description: Specifies whether to include or exclude organizations that have
          a donorprivacy policy
      - in: query
        name: fundraisingOrgs
        description: Specifies whether to include or exclude organizations flagged
          by CharityNavigator as fundraising organizations
      - in: query
        name: maxRating
        description: Filters search results to include only organizations with a rating
          less thanor equal to the specified value
      - in: query
        name: minRating
        description: Filters search results to include only organizations with a rating
          greaterthan or equal to the specified value
      - in: query
        name: noGovSupport
        description: Specifies whether to include or exclude organizations that do
          not receivegovernment support
      - in: query
        name: pageNum
        description: Page number to return, in case the number of available objects
          in the resultset is greater than the specified or default `pageSize`
      - in: query
        name: pageSize
        description: Number of organizations to return in a single response message
      - in: query
        name: rated
        description: Specifies whether to include only rated charities or unrated
          charities
      - in: query
        name: scopeOfWork
        description: Filters search results to include only organizations with a given
          scope ofwork
      - in: query
        name: search
        description: A simple search string that narrows the results to organizations
          matchingthe specified search terms
      - in: query
        name: searchType
        description: Used in combination with the `search` parameter, specifies the
          type ofsearch to be performed
      - in: query
        name: sizeRange
        description: Filters search results to include only organizations within a
          given sizebracket, as measured in annual Total Expenses
      - in: query
        name: sort
        description: Specifies how results should be sorted
      - in: query
        name: state
        description: If set to a valid 2-letter state code (not case-sensitive), filters
          searchresults to include only organizations in the specified state
      - in: query
        name: zip
        description: Filters search results to include only organizations in the specified
          zipcode
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /Organizations/{ein}:
    get:
      summary: Get Organizations Ein
      description: |-
        Retrieve full detail of a single Organization. This is a composite set of
        information describing an organization that may engage in charitable work.
        Normally the Organization data structure includes a single legal entity, though
        legal entity information may be excluded in exceptional cases.
      operationId: getOrganization
      x-api-path-slug: organizationsein-get
      parameters:
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      - in: path
        name: ein
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Ein
  /Organizations/{ein}/Ratings:
    get:
      summary: Get Organizations Ein Ratings
      description: |-
        Retrieve all Charity Navigator ratings for a single organization. <br/>
        ![Content
        Subscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png
        "Included with the paid Content Subscription.")
      operationId: getRatings
      x-api-path-slug: organizationseinratings-get
      parameters:
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      - in: path
        name: ein
      - in: query
        name: pageNum
        description: Page number to return, in case the number of available objects
          in the resultset is greater than the specified or default `pageSize`
      - in: query
        name: pageSize
        description: Number of objects to return in a single response message
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Ein
      - Ratings
  /Organizations/{ein}/Ratings/{RatingID}:
    get:
      summary: Get Organizations Ein Ratings Rating
      description: |-
        Retrieve a single Rating object for an Organization. Each rating is listed
        once, under its primary `referenceOrganization`. Note that the rating may apply
        to other organizations, and this is represented by `includedOrganizations`,
        which is a collection of hyperlinks to all of the organizations to which the
        rating applies.
        The rating is a point-in-time assessment provided by Charity Navigator, along
        with related metrics and ratios taken from financial statements for a fiscal
        year, on which the rating is based. <br/> ![Content
        Subscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png
        "Included with the paid Content Subscription.")
      operationId: getRating
      x-api-path-slug: organizationseinratingsratingid-get
      parameters:
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      - in: path
        name: ein
      - in: path
        name: RatingID
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Ein
      - Ratings
      - Rating
  /Organizations/{ein}/Advisories:
    get:
      summary: Get Organizations Ein Advisories
      description: |-
        Retrieve the full set of Charity Navigator advisories for a specified
        organization. An advisory is a cautionary communication from Charity Navigator,
        advising of unusual events or behavior related to a known organization.
      operationId: getAdvisories
      x-api-path-slug: organizationseinadvisories-get
      parameters:
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      - in: path
        name: ein
      - in: query
        name: pageNum
        description: Page number to return, in case the number of available objects
          in the resultset is greater than the specified or default `pageSize`
      - in: query
        name: pageSize
        description: Number of objects to return in a single response message
      - in: query
        name: status
        description: An optional filter parameter to limit the Advisories returned,
          based onstatus:| Status Value | Advisories Included                                 ||
          ------------ | --------------------------------------------------- || ALL
          | All advisories included, regardless of status
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Ein
      - Advisories
  /Organizations/{ein}/Advisories/{AdvisoryID}:
    get:
      summary: Get Organizations Ein Advisories Advisory
      description: |-
        Retrieve full details of a single Advisory, under a given organization. An
        advisory is a cautionary communication from Charity Navigator, advising of
        unusual events or behavior related to a known organization.
      operationId: getAdvisory
      x-api-path-slug: organizationseinadvisoriesadvisoryid-get
      parameters:
      - in: path
        name: AdvisoryID
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      - in: path
        name: ein
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Ein
      - Advisories
      - Advisory
  /Lists:
    get:
      summary: Get Lists
      description: |-
        Retrieve a set of Lists defined in Charity Navigator. Each entry in this
        collection is a curated or generated list of organizations, published by Charity
        Navigator. <br/> ![Content
        Subscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png
        "Included with the paid Content Subscription.")
      operationId: getLists
      x-api-path-slug: lists-get
      parameters:
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      - in: query
        name: pageNum
        description: Page number to return, in case the number of available objects
          in the resultset is greater than the specified or default `pageSize`
      - in: query
        name: pageSize
        description: Number of objects to return in a single response message
      responses:
        200:
          description: OK
      tags:
      - Lists
  /Lists/{ListID}:
    get:
      summary: Get Lists List
      description: |-
        Retrieve a curated or generated list of organizations, published by Charity
        Navigator. <br/> ![Content
        Subscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png
        "Included with the paid Content Subscription.")
      operationId: getList
      x-api-path-slug: listslistid-get
      parameters:
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      - in: path
        name: ListID
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
  /Categories:
    get:
      summary: Get Categories
      description: |-
        Returns metadata for Charity Navigator's classification hierarchy for
        charitable Organizations. Category is the top-level classifier, and each
        category may contain a number of Causes. <br/> ![Content
        Subscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png
        "Included with the paid Content Subscription.")
      operationId: getCategories
      x-api-path-slug: categories-get
      parameters:
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      responses:
        200:
          description: OK
      tags:
      - Categories
  /Advisory:
    get:
      summary: Get Advisory
      description: |-
        Retrieve the full set of Charity Navigator advisories for a specified
        organization. An advisory is a cautionary communication from Charity Navigator,
        advising of unusual events or behavior related to a known organization.
      operationId: getAllActiveAdvisories
      x-api-path-slug: advisory-get
      parameters:
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      - in: query
        name: pageNum
        description: Page number to return, in case the number of available objects
          in the resultset is greater than the specified or default `pageSize`
      - in: query
        name: pageSize
        description: Number of organizations to return in a single response message
      responses:
        200:
          description: OK
      tags:
      - Advisory