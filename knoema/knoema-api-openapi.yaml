swagger: "2.0"
x-collection-name: Knoema
x-complete: 1
info:
  title: Knoema
  description: you-dont-need-to-be-a-developer-to-get-started--we-made-a-number-of-useful-platform-features-available-as-ready-to-use-widgets--you-can-put-a-dashboard-or-presentation-with-any-visualizationcontent-you-like-and-then-embed-it-in-your-site-or-blog-in-a-few-minutes---such-an-approach-requires-no-programming-skills-at-all-just-basic-understanding-of-html--refer-to-widgets-sections-for-more-information-on-this-topic--knoema-is-a-truly-open-platform---in-addition-to-our-own-apis-we-support-several-formats-widely-acknowledged-by-industry-such-as-odata-and-sdmx---if-you-already-have-toolsclients-utilizing-data-in-these-formats-you-can-add-knoema-support-very-easily--more-information-can-be-found-in-open-data-section--for-enthusiasts-and-hardcore-developers-knoema-offers-extensive-knoema-api-providing-access-to-all-platform-capabilities--start-with-getting-familiar-with-core-knoema-concepts--then-proceed-to-applications-section-to-find-stepbystep-tutorials-detailed-documentation-and-sample-apps-
  version: 1.0.0
host: knoema.com
basePath: /api/1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /meta/dataset:
    get:
      summary: List of datasets
      description: Returns the list of datasets
      operationId: listOfDatasets
      x-api-path-slug: metadataset-get
      responses:
        200:
          description: OK
      tags:
      - Datasets
  /meta/dataset/{dataset id}:
    get:
      summary: Dataset details
      description: Lists out details of a particular dataset.
      operationId: datasetDetails
      x-api-path-slug: metadatasetdataset-id-get
      responses:
        200:
          description: OK
      tags:
      - Datasets
  /meta/dataset/{datasetId}/dimension/{dimensionId}:
    get:
      summary: Dimension
      description: Lists out the given dataset's dimension details.
      operationId: datasetDimensions
      x-api-path-slug: metadatasetdatasetiddimensiondimensionid-get
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dimensions
  /meta/group/{groupKey}:
    get:
      summary: Dimension Group
      description: 'This endpoint used to list/add/edit/delete groups in dimensions.
        The functionality of endpoint depends on HTTP method: GET, POST, PUT or DELETE.'
      operationId: dimensionGroup
      x-api-path-slug: metagroupgroupkey-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Dimensions
  /frontend/tags:
    get:
      summary: List of tags
      description: Lists out all the public tags present in the system
      operationId: getTags
      x-api-path-slug: frontendtags-get
      responses:
        200:
          description: OK
      tags:
      - Tags
  /data/dataset/{dataset id}:
    get:
      summary: Get timeseries list
      description: For the given dataset, this endpoint returns time series list for
        all the available frequencies with the combination of all the dimension members.
      operationId: getTimeseriesList
      x-api-path-slug: datadatasetdataset-id-get
      parameters:
      - in: path
        name: dataset id
        description: Unique dataset identifier
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Time Series
  /data/get:
    get:
      summary: Get data
      description: This endpoint returns observation data for the given filter.
      operationId: getData
      x-api-path-slug: dataget-get
      parameters:
      - in: query
        name: DatasetId
        description: Unique dataset identifier
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Datasets
  /search:
    get:
      summary: Search by keyword
      description: This namespace provides search details for data accessible by that
        user.
      operationId: search
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: correct
        description: correct (default true) - correct mistakes in the query or not
        type: string
        format: string
      - in: query
        name: count
        description: count (default 100) - number results count [0
        type: string
        format: string
      - in: query
        name: query
        description: search query for which data is required
        type: string
        format: string
      - in: query
        name: scope
        description: String to specify the type of search results
        type: string
        format: string
      - in: query
        name: start
        description: start (default 0) - number of the first result [0
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Search