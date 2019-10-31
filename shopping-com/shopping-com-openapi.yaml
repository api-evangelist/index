swagger: "2.0"
x-collection-name: Shopping.com
x-complete: 1
info:
  title: Shopping.com
  description: shopping-com-offers-publishers-rich-content-via-the-shopping-coms-api-
  version: 1.0.0
host: sandbox.api.shopping.com
basePath: /publisher/3.0/rest/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GeneralSearch:
    parameters:
      summary: ""
      description: ""
      operationId: ""
      x-api-path-slug: generalsearch-parameters
      responses:
        200:
          description: OK
      tags:
      - ""
    get:
      summary: ""
      description: Searches for products by offer. See API docs for request parameters/format.
      operationId: GeneralSearch.get
      x-api-path-slug: generalsearch-get
      parameters:
      - in: query
        name: groupItemsByCategory
        description: Control whether or not items are separated into different categories
      - in: query
        name: numFeatured
        description: Set the maximum number of featured stores to include in a result
          containing a list of offers, when using the featured-store offer sort type
      - in: query
        name: offerSortOrder
        description: Control whether results containing only offers will be sorted
          in ascending or descending order
      - in: query
        name: offerSortType
        description: Set the method of sorting offers
      - in: query
        name: postalCode
        description: Set the postal code of the current user, for tax and shipping
          purposes
      - in: query
        name: productReviewSortType
        description: Control how to sort product reviews listings
      - in: query
        name: productReviewsSortOrder
        description: Control whether product reviews listings will be sorted in ascending
          or descending order
      - in: query
        name: showAllMatchingCategories
        description: Control whether or not this query will return all matching categories,
          regardless of relevance
      - in: query
        name: showSmartBuy
        description: Control whether or not the lowest-price offer from a trusted
          store will be flagged
      - in: query
        name: subTrackingId
        description: User generated ID used to further break down traffic sources
          beyond SDC campaign level tracking
      - in: query
        name: visitorIPAddress
        description: The IP address of the visitor to which this data is being presented
      - in: query
        name: visitorUserAgent
        description: The browser user-agent of the visitor to which this data is being
          presented
      responses:
        200:
          description: OK
      tags:
      - ""
  /CategoryTree:
    parameters:
      summary: ""
      description: ""
      operationId: ""
      x-api-path-slug: categorytree-parameters
      responses:
        200:
          description: OK
      tags:
      - ""
    get:
      summary: ""
      description: Returns information on a single category (e.g. name) or the relationship
        hierarchy between categories.
      operationId: CategoryTree.get
      x-api-path-slug: categorytree-get
      parameters:
      - in: query
        name: categoryId
        description: The ID of the category for to return information for, as well
          as the information for all its immediate children (if any)
      - in: query
        name: showAllDescendants
        description: Specifies that information for all descendants of the specified
          category should be returned
      responses:
        200:
          description: OK
      tags:
      - ""