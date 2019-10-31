swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 1
info:
  title: Data.gov API
  description: the-data-gov-catalog-is-powered-by-ckan-a-powerful-open-source-data-platform-that-includes-a-robust-api--please-be-aware-that-data-gov-and-the-data-gov-ckan-api-only-contain-metadata-about-datasets--this-metadata-includes-urls-and-descriptions-of-datasets-but-it-does-not-include-the-actual-data-within-each-dataset-
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activity:
    get:
      summary: Get Activity
      description: Fetch site activity, optionally filterd by user of org
      operationId: getActivity
      x-api-path-slug: activity-get
      parameters:
      - in: query
        name: organization
        description: Filter activities for that particular organization
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      - in: query
        name: user
        description: Filter activities for that particular user
      responses:
        200:
          description: OK
      tags:
      - Activity
  /datasets/:
    get:
      summary: Get Datasets
      description: List or search all datasets
      operationId: getDatasets
      x-api-path-slug: datasets-get
      parameters:
      - in: query
        name: badge
      - in: query
        name: extra
      - in: query
        name: facets
        description: Selected facets to fetch
      - in: query
        name: featured
      - in: query
        name: format
      - in: query
        name: geozone
      - in: query
        name: granularity
      - in: query
        name: license
      - in: query
        name: organization
      - in: query
        name: owner
      - in: query
        name: page
        description: The page to display
      - in: query
        name: page_size
        description: The page size
      - in: query
        name: q
        description: The search query
      - in: query
        name: reuses
      - in: query
        name: sort
        description: The field (and direction) on which sorting apply
      - in: query
        name: tag
      - in: query
        name: temporal_coverage
      responses:
        200:
          description: OK
      tags:
      - Datasets
    post:
      summary: Add Datasets
      description: Create a new dataset
      operationId: postDatasets
      x-api-path-slug: datasets-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datasets
  /datasets/badges/:
    get:
      summary: Get Datasets Badges
      description: List all available dataset badges and their labels
      operationId: getDatasetsBadges
      x-api-path-slug: datasetsbadges-get
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Badges
  /datasets/checkurl/:
    get:
      summary: Get Datasets Checkurl
      description: Checks that a URL exists and returns metadata
      operationId: getDatasetsCheckurl
      x-api-path-slug: datasetscheckurl-get
      parameters:
      - in: query
        name: group
        description: The dataset related to the URL
      - in: query
        name: url
        description: The URL to check
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Checkurl
  /datasets/community_resources/:
    get:
      summary: Get Datasets Community Resources
      description: List all community resources
      operationId: getDatasetsCommunityResources
      x-api-path-slug: datasetscommunity-resources-get
      parameters:
      - in: query
        name: dataset
        description: Filter activities for that particular dataset
      - in: query
        name: organization
        description: Filter activities for that particular organization
      - in: query
        name: owner
        description: Filter activities for that particular user
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      - in: query
        name: sort
        description: The sorting attribute
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Community
      - Resources
    post:
      summary: Add Datasets Community Resources
      description: Create a new community resource
      operationId: postDatasetsCommunityResources
      x-api-path-slug: datasetscommunity-resources-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Community
      - Resources
  /datasets/community_resources/{community}/:
    delete:
      summary: Delete Datasets Community Resources Community
      description: Delete a given community resource
      operationId: deleteDatasetsCommunityResourcesCommunity
      x-api-path-slug: datasetscommunity-resourcescommunity-delete
      parameters:
      - in: path
        name: community
        description: The community resource unique identifier
      - in: query
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Community
      - Resources
      - Community
    get:
      summary: Get Datasets Community Resources Community
      description: Retrieve a community resource given its identifier
      operationId: getDatasetsCommunityResourcesCommunity
      x-api-path-slug: datasetscommunity-resourcescommunity-get
      parameters:
      - in: path
        name: community
        description: The community resource unique identifier
      - in: query
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Community
      - Resources
      - Community
    put:
      summary: Put Datasets Community Resources Community
      description: Update a given community resource
      operationId: putDatasetsCommunityResourcesCommunity
      x-api-path-slug: datasetscommunity-resourcescommunity-put
      parameters:
      - in: path
        name: community
        description: The community resource unique identifier
      - in: query
        name: dataset
        description: The dataset ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Community
      - Resources
      - Community
  /datasets/community_resources/{community}/upload/:
    post:
      summary: Add Datasets Community Resources Community Upload
      description: Update the file related to a given community resource
      operationId: postDatasetsCommunityResourcesCommunityUpload
      x-api-path-slug: datasetscommunity-resourcescommunityupload-post
      parameters:
      - in: path
        name: community
        description: The community resource unique identifier
      - in: query
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Community
      - Resources
      - Community
      - Upload
  /datasets/frequencies/:
    get:
      summary: Get Datasets Frequencies
      description: List all available frequencies
      operationId: getDatasetsFrequencies
      x-api-path-slug: datasetsfrequencies-get
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Frequencies
  /datasets/full/:
    get:
      summary: Get Datasets Full
      description: ""
      operationId: getDatasetsFull
      x-api-path-slug: datasetsfull-get
      parameters:
      - in: query
        name: badge
      - in: query
        name: extra
      - in: query
        name: facets
        description: Selected facets to fetch
      - in: query
        name: featured
      - in: query
        name: format
      - in: query
        name: geozone
      - in: query
        name: granularity
      - in: query
        name: license
      - in: query
        name: organization
      - in: query
        name: owner
      - in: query
        name: page
        description: The page to display
      - in: query
        name: page_size
        description: The page size
      - in: query
        name: q
        description: The search query
      - in: query
        name: reuses
      - in: query
        name: sort
        description: The field (and direction) on which sorting apply
      - in: query
        name: tag
      - in: query
        name: temporal_coverage
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Full
  /datasets/licenses/:
    get:
      summary: Get Datasets Licenses
      description: List all available licenses
      operationId: getDatasetsLicenses
      x-api-path-slug: datasetslicenses-get
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Licenses
  /datasets/suggest/:
    get:
      summary: Get Datasets Suggest
      description: Suggest datasets
      operationId: getDatasetsSuggest
      x-api-path-slug: datasetssuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Suggest
  /datasets/suggest/formats/:
    get:
      summary: Get Datasets Suggest Formats
      description: Suggest file formats
      operationId: getDatasetsSuggestFormats
      x-api-path-slug: datasetssuggestformats-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Suggest
      - Formats
  /datasets/{dataset}/:
    delete:
      summary: Delete Datasets Dataset
      description: Delete a dataset given its identifier
      operationId: deleteDatasetsDataset
      x-api-path-slug: datasetsdataset-delete
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
    get:
      summary: Get Datasets Dataset
      description: Get a dataset given its identifier
      operationId: getDatasetsDataset
      x-api-path-slug: datasetsdataset-get
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
    put:
      summary: Put Datasets Dataset
      description: Update a dataset given its identifier
      operationId: putDatasetsDataset
      x-api-path-slug: datasetsdataset-put
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
  /datasets/{dataset}/badges/:
    post:
      summary: Add Datasets Dataset Badges
      description: Create a new badge for a given dataset
      operationId: postDatasetsDatasetBadges
      x-api-path-slug: datasetsdatasetbadges-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Badges
  /datasets/{dataset}/badges/{badge_kind}/:
    delete:
      summary: Delete Datasets Dataset Badges Badge Kind
      description: Delete a badge for a given dataset
      operationId: deleteDatasetsDatasetBadgesBadgeKind
      x-api-path-slug: datasetsdatasetbadgesbadge-kind-delete
      parameters:
      - in: path
        name: badge_kind
      - in: path
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Badges
      - Badge
      - Kind
  /datasets/{dataset}/featured/:
    delete:
      summary: Delete Datasets Dataset Featured
      description: Unmark the dataset as featured
      operationId: deleteDatasetsDatasetFeatured
      x-api-path-slug: datasetsdatasetfeatured-delete
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Featured
    post:
      summary: Add Datasets Dataset Featured
      description: Mark the dataset as featured
      operationId: postDatasetsDatasetFeatured
      x-api-path-slug: datasetsdatasetfeatured-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Featured
  /datasets/{dataset}/full/:
    get:
      summary: Get Datasets Dataset Full
      description: Get a dataset given its identifier
      operationId: getDatasetsDatasetFull
      x-api-path-slug: datasetsdatasetfull-get
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Full
  /datasets/{dataset}/resources/:
    post:
      summary: Add Datasets Dataset Resources
      description: Create a new resource for a given dataset
      operationId: postDatasetsDatasetResources
      x-api-path-slug: datasetsdatasetresources-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Resources
    put:
      summary: Put Datasets Dataset Resources
      description: Reorder resources
      operationId: putDatasetsDatasetResources
      x-api-path-slug: datasetsdatasetresources-put
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Resources
  /datasets/{dataset}/resources/{rid}/:
    delete:
      summary: Delete Datasets Dataset Resources R
      description: Delete a given resource on a given dataset
      operationId: deleteDatasetsDatasetResourcesR
      x-api-path-slug: datasetsdatasetresourcesrid-delete
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: path
        name: rid
        description: The resource unique identifier
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Resources
      - R
    put:
      summary: Put Datasets Dataset Resources R
      description: Update a given resource on a given dataset
      operationId: putDatasetsDatasetResourcesR
      x-api-path-slug: datasetsdatasetresourcesrid-put
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: rid
        description: The resource unique identifier
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Resources
      - R
  /datasets/{dataset}/resources/{rid}/upload/:
    post:
      summary: Add Datasets Dataset Resources R Upload
      description: Upload a file related to a given resource on a given dataset
      operationId: postDatasetsDatasetResourcesRUpload
      x-api-path-slug: datasetsdatasetresourcesridupload-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: path
        name: rid
        description: The resource unique identifier
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Resources
      - R
      - Upload
  /datasets/{dataset}/upload/:
    post:
      summary: Add Datasets Dataset Upload
      description: Upload a new dataset resource
      operationId: postDatasetsDatasetUpload
      x-api-path-slug: datasetsdatasetupload-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: formData
        name: file
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Upload
  /datasets/{dataset}/upload/community/:
    post:
      summary: Add Datasets Dataset Upload Community
      description: Upload a new community resource
      operationId: postDatasetsDatasetUploadCommunity
      x-api-path-slug: datasetsdatasetuploadcommunity-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: formData
        name: file
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Upload
      - Community
  /datasets/{id}/followers/:
    delete:
      summary: Delete Datasets  Followers
      description: Unfollow an object given its ID
      operationId: deleteDatasetsFollowers
      x-api-path-slug: datasetsidfollowers-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - ""
      - Followers
    get:
      summary: Get Datasets  Followers
      description: List all followers for a given object
      operationId: getDatasetsFollowers
      x-api-path-slug: datasetsidfollowers-get
      parameters:
      - in: path
        name: id
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - ""
      - Followers
    post:
      summary: Add Datasets  Followers
      description: Follow an object given its ID
      operationId: postDatasetsFollowers
      x-api-path-slug: datasetsidfollowers-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - ""
      - Followers
  /discussions/:
    get:
      summary: Get Discussions
      description: List all Discussions
      operationId: getDiscussions
      x-api-path-slug: discussions-get
      parameters:
      - in: query
        name: closed
        description: Filters discussions on their closed status if specified
      - in: query
        name: for
        description: Filter discussions for a given subject
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      - in: query
        name: sort
        description: The sorting attribute
      responses:
        200:
          description: OK
      tags:
      - Discussions
    post:
      summary: Add Discussions
      description: Create a new Discussion
      operationId: postDiscussions
      x-api-path-slug: discussions-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Discussions
  /discussions/{id}/:
    delete:
      summary: Delete Discussions
      description: Delete a discussion given its ID
      operationId: deleteDiscussions
      x-api-path-slug: discussionsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Discussions
    get:
      summary: Get Discussions
      description: Get a discussion given its ID
      operationId: getDiscussions
      x-api-path-slug: discussionsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Discussions
    post:
      summary: Add Discussions
      description: Add comment and optionnaly close a discussion given its ID
      operationId: postDiscussions
      x-api-path-slug: discussionsid-post
      parameters:
      - in: path
        name: id
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Discussions
  /harvest/backends:
    get:
      summary: Get Harvest Backends
      description: List all available harvest backends
      operationId: getHarvestBackends
      x-api-path-slug: harvestbackends-get
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Backends
  /harvest/job/{ident}/:
    get:
      summary: Get Harvest Job
      description: List all jobs for a given source
      operationId: getHarvestJobEnt
      x-api-path-slug: harvestjobident-get
      parameters:
      - in: path
        name: ident
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Job
      - Ent
  /harvest/job_status:
    get:
      summary: Get Harvest Job Status
      description: List all available harvesters
      operationId: getHarvestJobStatus
      x-api-path-slug: harvestjob-status-get
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Job
      - Status
  /harvest/source/{ident}:
    delete:
      summary: Delete Harvest Source Ent
      description: ""
      operationId: deleteHarvestSourceEnt
      x-api-path-slug: harvestsourceident-delete
      parameters:
      - in: path
        name: ident
        description: A source ID or slug
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Source
      - Ent
    get:
      summary: Get Harvest Source Ent
      description: Get a single source given an ID or a slug
      operationId: getHarvestSourceEnt
      x-api-path-slug: harvestsourceident-get
      parameters:
      - in: path
        name: ident
        description: A source ID or slug
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Source
      - Ent
  /harvest/source/{ident}/jobs/:
    get:
      summary: Get Harvest Source Ent Jobs
      description: List all jobs for a given source
      operationId: getHarvestSourceEntJobs
      x-api-path-slug: harvestsourceidentjobs-get
      parameters:
      - in: path
        name: ident
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Source
      - Ent
      - Jobs
  /harvest/source/{ident}/preview:
    get:
      summary: Get Harvest Source Ent Preview
      description: Preview a single harvest source given an ID or a slug
      operationId: getHarvestSourceEntPreview
      x-api-path-slug: harvestsourceidentpreview-get
      parameters:
      - in: path
        name: ident
        description: A source ID or slug
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Source
      - Ent
      - Preview
  /harvest/source/{ident}/validate:
    post:
      summary: Add Harvest Source Ent Valate
      description: Validate or reject an harvest source
      operationId: postHarvestSourceEntValate
      x-api-path-slug: harvestsourceidentvalidate-post
      parameters:
      - in: path
        name: ident
        description: A source ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Source
      - Ent
      - Valate
  /harvest/sources/:
    get:
      summary: Get Harvest Sources
      description: List all harvest sources
      operationId: getHarvestSources
      x-api-path-slug: harvestsources-get
      parameters:
      - in: query
        name: owner
        description: The organization or user ID to filter on
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Sources
    post:
      summary: Add Harvest Sources
      description: Create a new harvests source
      operationId: postHarvestSources
      x-api-path-slug: harvestsources-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Sources
  /issues/:
    get:
      summary: Get Issues
      description: List all Issues
      operationId: getIssues
      x-api-path-slug: issues-get
      parameters:
      - in: query
        name: closed
        description: Filter closed issues
      - in: query
        name: for
        description: Filter issues for a given subject
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      - in: query
        name: sort
        description: The sorting attribute
      responses:
        200:
          description: OK
      tags:
      - Issues
    post:
      summary: Add Issues
      description: Create a new Issue
      operationId: postIssues
      x-api-path-slug: issues-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Issues
  /issues/{id}/:
    get:
      summary: Get Issues
      description: Get an issue given its ID
      operationId: getIssues
      x-api-path-slug: issuesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Issues
    post:
      summary: Add Issues
      description: Add comment and optionnaly close an issue given its ID
      operationId: postIssues
      x-api-path-slug: issuesid-post
      parameters:
      - in: path
        name: id
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Issues
  /me/:
    get:
      summary: Get Me
      description: Fetch the current user (me) identity
      operationId: getMe
      x-api-path-slug: me-get
      responses:
        200:
          description: OK
      tags:
      - Me
    put:
      summary: Put Me
      description: Update my profile
      operationId: putMe
      x-api-path-slug: me-put
      responses:
        200:
          description: OK
      tags:
      - Me
  /me/apikey:
    delete:
      summary: Delete Me Apikey
      description: Clear/destroy an apikey
      operationId: deleteMeApikey
      x-api-path-slug: meapikey-delete
      responses:
        200:
          description: OK
      tags:
      - Me
      - Apikey
    post:
      summary: Add Me Apikey
      description: (Re)Generate my API Key
      operationId: postMeApikey
      x-api-path-slug: meapikey-post
      responses:
        200:
          description: OK
      tags:
      - Me
      - Apikey
  /me/avatar:
    post:
      summary: Add Me Avatar
      description: Upload a new avatar
      operationId: postMeAvatar
      x-api-path-slug: meavatar-post
      parameters:
      - in: formData
        name: bbox
      - in: formData
        name: file
      responses:
        200:
          description: OK
      tags:
      - Me
      - Avatar
  /me/datasets/:
    get:
      summary: Get Me Datasets
      description: List all my datasets (including private ones)
      operationId: getMeDatasets
      x-api-path-slug: medatasets-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Datasets
  /me/metrics/:
    get:
      summary: Get Me Metrics
      description: Fetch the current user (me) metrics
      operationId: getMeMetrics
      x-api-path-slug: memetrics-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Metrics
  /me/org_community_resources/:
    get:
      summary: Get Me Org Community Resources
      description: List all community resources related to me and my organizations
      operationId: getMeOrgCommunityResources
      x-api-path-slug: meorg-community-resources-get
      parameters:
      - in: query
        name: q
        description: The string to filter items
      responses:
        200:
          description: OK
      tags:
      - Me
      - Org
      - Community
      - Resources
  /me/org_datasets/:
    get:
      summary: Get Me Org Datasets
      description: List all datasets related to me and my organizations
      operationId: getMeOrgDatasets
      x-api-path-slug: meorg-datasets-get
      parameters:
      - in: query
        name: q
        description: The string to filter items
      responses:
        200:
          description: OK
      tags:
      - Me
      - Org
      - Datasets
  /me/org_discussions/:
    get:
      summary: Get Me Org Discussions
      description: List all discussions related to my organizations
      operationId: getMeOrgDiscussions
      x-api-path-slug: meorg-discussions-get
      parameters:
      - in: query
        name: q
        description: The string to filter items
      responses:
        200:
          description: OK
      tags:
      - Me
      - Org
      - Discussions
  /me/org_issues/:
    get:
      summary: Get Me Org Issues
      description: List all issues related to my organizations
      operationId: getMeOrgIssues
      x-api-path-slug: meorg-issues-get
      parameters:
      - in: query
        name: q
        description: The string to filter items
      responses:
        200:
          description: OK
      tags:
      - Me
      - Org
      - Issues
  /me/org_reuses/:
    get:
      summary: Get Me Org Reuses
      description: List all reuses related to me and my organizations
      operationId: getMeOrgReuses
      x-api-path-slug: meorg-reuses-get
      parameters:
      - in: query
        name: q
        description: The string to filter items
      responses:
        200:
          description: OK
      tags:
      - Me
      - Org
      - Reuses
  /me/reuses/:
    get:
      summary: Get Me Reuses
      description: List all my reuses (including private ones)
      operationId: getMeReuses
      x-api-path-slug: mereuses-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Reuses
  /metrics/{id}:
    get:
      summary: Get Metrics
      description: Fetch metrics for an object given its ID
      operationId: getMetrics
      x-api-path-slug: metricsid-get
      parameters:
      - in: query
        name: cumulative
        description: Either cumulative metrics or not
      - in: query
        name: day
        description: Specific day date to fetch
      - in: query
        name: end
        description: End of the period to fetch
      - in: path
        name: id
        description: The object ID to fetch metric for
      - in: query
        name: start
        description: Start of the period to fetch
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /notifications/:
    get:
      summary: Get Notifications
      description: List all current user pending notifications
      operationId: getNotifications
      x-api-path-slug: notifications-get
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /oembeds/:
    get:
      summary: Get Oembeds
      description: The returned payload is a list of OEmbed formatted responses
      operationId: getOembeds
      x-api-path-slug: oembeds-get
      parameters:
      - in: query
        name: references
        description: References of the resources to embed
      responses:
        200:
          description: OK
      tags:
      - Oembeds
  /organizations/:
    get:
      summary: Get Organizations
      description: List or search all organizations
      operationId: getOrganizations
      x-api-path-slug: organizations-get
      parameters:
      - in: query
        name: badge
      - in: query
        name: datasets
      - in: query
        name: facets
        description: Selected facets to fetch
      - in: query
        name: followers
      - in: query
        name: page
        description: The page to display
      - in: query
        name: page_size
        description: The page size
      - in: query
        name: permitted_reuses
      - in: query
        name: q
        description: The search query
      - in: query
        name: reuses
      - in: query
        name: sort
        description: The field (and direction) on which sorting apply
      responses:
        200:
          description: OK
      tags:
      - Organizations
    post:
      summary: Add Organizations
      description: Create a new organization
      operationId: postOrganizations
      x-api-path-slug: organizations-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /organizations/badges/:
    get:
      summary: Get Organizations Badges
      description: List all available organization badges and their labels
      operationId: getOrganizationsBadges
      x-api-path-slug: organizationsbadges-get
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Badges
  /organizations/suggest/:
    get:
      summary: Get Organizations Suggest
      description: Suggest organizations
      operationId: getOrganizationsSuggest
      x-api-path-slug: organizationssuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Suggest
  /organizations/{id}/followers/:
    delete:
      summary: Delete Organizations  Followers
      description: Unfollow an object given its ID
      operationId: deleteOrganizationsFollowers
      x-api-path-slug: organizationsidfollowers-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - ""
      - Followers
    get:
      summary: Get Organizations  Followers
      description: List all followers for a given object
      operationId: getOrganizationsFollowers
      x-api-path-slug: organizationsidfollowers-get
      parameters:
      - in: path
        name: id
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - ""
      - Followers
    post:
      summary: Add Organizations  Followers
      description: Follow an object given its ID
      operationId: postOrganizationsFollowers
      x-api-path-slug: organizationsidfollowers-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - ""
      - Followers
  /organizations/{org}/:
    delete:
      summary: Delete Organizations Org
      description: Delete a organization given its identifier
      operationId: deleteOrganizationsOrg
      x-api-path-slug: organizationsorg-delete
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
    get:
      summary: Get Organizations Org
      description: Get a organization given its identifier
      operationId: getOrganizationsOrg
      x-api-path-slug: organizationsorg-get
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
    put:
      summary: Put Organizations Org
      description: Update a organization given its identifier
      operationId: putOrganizationsOrg
      x-api-path-slug: organizationsorg-put
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
  /organizations/{org}/badges/:
    post:
      summary: Add Organizations Org Badges
      description: Create a new badge for a given organization
      operationId: postOrganizationsOrgBadges
      x-api-path-slug: organizationsorgbadges-post
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Badges
  /organizations/{org}/badges/{badge_kind}/:
    delete:
      summary: Delete Organizations Org Badges Badge Kind
      description: Delete a badge for a given organization
      operationId: deleteOrganizationsOrgBadgesBadgeKind
      x-api-path-slug: organizationsorgbadgesbadge-kind-delete
      parameters:
      - in: path
        name: badge_kind
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Badges
      - Badge
      - Kind
  /organizations/{org}/datasets/:
    get:
      summary: Get Organizations Org Datasets
      description: List organization datasets (including private ones when member)
      operationId: getOrganizationsOrgDatasets
      x-api-path-slug: organizationsorgdatasets-get
      parameters:
      - in: path
        name: org
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Datasets
  /organizations/{org}/discussions/:
    get:
      summary: Get Organizations Org Discussions
      description: List organization discussions
      operationId: getOrganizationsOrgDiscussions
      x-api-path-slug: organizationsorgdiscussions-get
      parameters:
      - in: path
        name: org
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Discussions
  /organizations/{org}/issues/:
    get:
      summary: Get Organizations Org Issues
      description: List organization issues
      operationId: getOrganizationsOrgIssues
      x-api-path-slug: organizationsorgissues-get
      parameters:
      - in: path
        name: org
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Issues
  /organizations/{org}/logo:
    post:
      summary: Add Organizations Org Logo
      description: Upload a new logo
      operationId: postOrganizationsOrgLogo
      x-api-path-slug: organizationsorglogo-post
      parameters:
      - in: formData
        name: bbox
      - in: formData
        name: file
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Logo
    put:
      summary: Put Organizations Org Logo
      description: Set the logo BBox
      operationId: putOrganizationsOrgLogo
      x-api-path-slug: organizationsorglogo-put
      parameters:
      - in: formData
        name: bbox
      - in: formData
        name: file
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Logo
  /organizations/{org}/member/{user}:
    delete:
      summary: Delete Organizations Org Member User
      description: Delete member from an organization
      operationId: deleteOrganizationsOrgMemberUser
      x-api-path-slug: organizationsorgmemberuser-delete
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      - in: path
        name: user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Member
      - User
    post:
      summary: Add Organizations Org Member User
      description: Add a member into a given organization
      operationId: postOrganizationsOrgMemberUser
      x-api-path-slug: organizationsorgmemberuser-post
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Member
      - User
    put:
      summary: Put Organizations Org Member User
      description: Update member status into a given organization
      operationId: putOrganizationsOrgMemberUser
      x-api-path-slug: organizationsorgmemberuser-put
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Member
      - User
  /organizations/{org}/membership/:
    get:
      summary: Get Organizations Org Membership
      description: List membership requests for a given organization
      operationId: getOrganizationsOrgMembership
      x-api-path-slug: organizationsorgmembership-get
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      - in: query
        name: status
        description: If provided, only return requests ith a given status
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Membership
    post:
      summary: Add Organizations Org Membership
      description: Apply for membership to a given organization
      operationId: postOrganizationsOrgMembership
      x-api-path-slug: organizationsorgmembership-post
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Membership
  /organizations/{org}/membership/{id}/accept/:
    post:
      summary: Add Organizations Org Membership  Accept
      description: Accept user membership to a given organization
      operationId: postOrganizationsOrgMembershipAccept
      x-api-path-slug: organizationsorgmembershipidaccept-post
      parameters:
      - in: path
        name: id
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Membership
      - ""
      - Accept
  /organizations/{org}/membership/{id}/refuse/:
    post:
      summary: Add Organizations Org Membership  Refuse
      description: Refuse user membership to a given organization
      operationId: postOrganizationsOrgMembershipRefuse
      x-api-path-slug: organizationsorgmembershipidrefuse-post
      parameters:
      - in: body
        name: comment
        description: The refusal reason
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: org
        description: The organization ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Membership
      - ""
      - Refuse
  /organizations/{org}/reuses/:
    get:
      summary: Get Organizations Org Reuses
      description: List organization reuses (including private ones when member)
      operationId: getOrganizationsOrgReuses
      x-api-path-slug: organizationsorgreuses-get
      parameters:
      - in: path
        name: org
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Reuses
  /posts/:
    get:
      summary: Posts
      description: List all posts
      operationId: getPosts
      x-api-path-slug: posts-get
      parameters:
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Posts
    post:
      summary: Add Post
      description: Create a post
      operationId: postPosts
      x-api-path-slug: posts-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/{post}/:
    delete:
      summary: Delete Post
      description: Delete a given post
      operationId: deletePostsPost
      x-api-path-slug: postspost-delete
      parameters:
      - in: path
        name: post
        description: The post ID or slug
      responses:
        200:
          description: OK
      tags:
      - Posts
    get:
      summary: Get Post
      description: Get a given post
      operationId: getPostsPost
      x-api-path-slug: postspost-get
      parameters:
      - in: path
        name: post
        description: The post ID or slug
      responses:
        200:
          description: OK
      tags:
      - Posts
    put:
      summary: Update Post
      description: Update a given post
      operationId: putPostsPost
      x-api-path-slug: postspost-put
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: post
        description: The post ID or slug
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/{post}/image:
    post:
      summary: Add Post Image
      description: Upload a new image
      operationId: postPostsPostImage
      x-api-path-slug: postspostimage-post
      parameters:
      - in: formData
        name: bbox
      - in: formData
        name: file
      - in: path
        name: post
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Images
    put:
      summary: Update Post Image
      description: Set the image BBox
      operationId: putPostsPostImage
      x-api-path-slug: postspostimage-put
      parameters:
      - in: formData
        name: bbox
      - in: formData
        name: file
      - in: path
        name: post
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Images
  /reuses/:
    get:
      summary: Get Reuses
      description: Get Reuses
      operationId: getReuses
      x-api-path-slug: reuses-get
      parameters:
      - in: query
        name: badge
      - in: query
        name: dataset
      - in: query
        name: datasets
      - in: query
        name: extra
      - in: query
        name: facets
        description: Selected facets to fetch
      - in: query
        name: featured
      - in: query
        name: followers
      - in: query
        name: organization
      - in: query
        name: owner
      - in: query
        name: page
        description: The page to display
      - in: query
        name: page_size
        description: The page size
      - in: query
        name: q
        description: The search query
      - in: query
        name: sort
        description: The field (and direction) on which sorting apply
      - in: query
        name: tag
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - Reuses
    post:
      summary: Add Reuses
      description: Create a new object
      operationId: postReuses
      x-api-path-slug: reuses-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Reuses
  /reuses/badges/:
    get:
      summary: Get Reuses Badges
      description: List all available reuse badges and their labels
      operationId: getReusesBadges
      x-api-path-slug: reusesbadges-get
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Badges
  /reuses/suggest/:
    get:
      summary: Get Reuses Suggest
      description: Suggest reuses
      operationId: getReusesSuggest
      x-api-path-slug: reusessuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Suggest
  /reuses/types/:
    get:
      summary: Get Reuses Types
      description: List all reuse types
      operationId: getReusesTypes
      x-api-path-slug: reusestypes-get
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Types
  /reuses/{id}/followers/:
    delete:
      summary: Delete Reuses  Followers
      description: Unfollow an object given its ID
      operationId: deleteReusesFollowers
      x-api-path-slug: reusesidfollowers-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - ""
      - Followers
    get:
      summary: Get Reuses  Followers
      description: List all followers for a given object
      operationId: getReusesFollowers
      x-api-path-slug: reusesidfollowers-get
      parameters:
      - in: path
        name: id
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - ""
      - Followers
    post:
      summary: Add Reuses  Followers
      description: Follow an object given its ID
      operationId: postReusesFollowers
      x-api-path-slug: reusesidfollowers-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - ""
      - Followers
  /reuses/{reuse}/:
    delete:
      summary: Delete Reuses Reuse
      description: Delete a given reuse
      operationId: deleteReusesReuse
      x-api-path-slug: reusesreuse-delete
      parameters:
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
    get:
      summary: Get Reuses Reuse
      description: Fetch a given reuse
      operationId: getReusesReuse
      x-api-path-slug: reusesreuse-get
      parameters:
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
    put:
      summary: Put Reuses Reuse
      description: Update a given reuse
      operationId: putReusesReuse
      x-api-path-slug: reusesreuse-put
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
  /reuses/{reuse}/badges/:
    post:
      summary: Add Reuses Reuse Badges
      description: Create a new badge for a given reuse
      operationId: postReusesReuseBadges
      x-api-path-slug: reusesreusebadges-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Badges
  /reuses/{reuse}/badges/{badge_kind}/:
    delete:
      summary: Delete Reuses Reuse Badges Badge Kind
      description: Delete a badge for a given reuse
      operationId: deleteReusesReuseBadgesBadgeKind
      x-api-path-slug: reusesreusebadgesbadge-kind-delete
      parameters:
      - in: path
        name: badge_kind
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Badges
      - Badge
      - Kind
  /reuses/{reuse}/datasets/:
    post:
      summary: Add Reuses Reuse Datasets
      description: Add a dataset to a given reuse
      operationId: postReusesReuseDatasets
      x-api-path-slug: reusesreusedatasets-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Datasets
  /reuses/{reuse}/featured/:
    delete:
      summary: Delete Reuses Reuse Featured
      description: Unmark a reuse as featured
      operationId: deleteReusesReuseFeatured
      x-api-path-slug: reusesreusefeatured-delete
      parameters:
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Featured
    post:
      summary: Add Reuses Reuse Featured
      description: Mark a reuse as featured
      operationId: postReusesReuseFeatured
      x-api-path-slug: reusesreusefeatured-post
      parameters:
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Featured
  /reuses/{reuse}/image:
    post:
      summary: Add Reuses Reuse Image
      description: Upload a new reuse image
      operationId: postReusesReuseImage
      x-api-path-slug: reusesreuseimage-post
      parameters:
      - in: formData
        name: bbox
      - in: formData
        name: file
      - in: path
        name: reuse
        description: The reuse ID or slug
      responses:
        200:
          description: OK
      tags:
      - Reuses
      - Reuse
      - Image
  /site/:
    get:
      summary: Get Site
      description: Site-wide variables
      operationId: getSite
      x-api-path-slug: site-get
      responses:
        200:
          description: OK
      tags:
      - Site
  /site/home/datasets/:
    get:
      summary: Get Site Home Datasets
      description: List homepage datasets
      operationId: getSiteHomeDatasets
      x-api-path-slug: sitehomedatasets-get
      responses:
        200:
          description: OK
      tags:
      - Site
      - Home
      - Datasets
    put:
      summary: Put Site Home Datasets
      description: Set the homepage datasets editorial selection
      operationId: putSiteHomeDatasets
      x-api-path-slug: sitehomedatasets-put
      parameters:
      - in: body
        name: payload
        description: Dataset IDs to put in homepage
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Site
      - Home
      - Datasets
  /site/home/reuses/:
    get:
      summary: Get Site Home Reuses
      description: List homepage featured reuses
      operationId: getSiteHomeReuses
      x-api-path-slug: sitehomereuses-get
      responses:
        200:
          description: OK
      tags:
      - Site
      - Home
      - Reuses
    put:
      summary: Put Site Home Reuses
      description: Set the homepage reuses editorial selection
      operationId: putSiteHomeReuses
      x-api-path-slug: sitehomereuses-put
      parameters:
      - in: body
        name: payload
        description: Reuse IDs to put in homepage
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Site
      - Home
      - Reuses
  /spatial/coverage/{level}:
    get:
      summary: Get Spatial Coverage Level
      description: List each zone for a given level with their datasets count
      operationId: getSpatialCoverageLevel
      x-api-path-slug: spatialcoveragelevel-get
      parameters:
      - in: path
        name: level
      responses:
        200:
          description: OK
      tags:
      - Spatial
      - Coverage
      - Level
  /spatial/granularities:
    get:
      summary: Get Spatial Granularities
      description: List all known spatial granularities
      operationId: getSpatialGranularities
      x-api-path-slug: spatialgranularities-get
      responses:
        200:
          description: OK
      tags:
      - Spatial
      - Granularities
  /spatial/levels:
    get:
      summary: Get Spatial Levels
      description: List all known levels
      operationId: getSpatialLevels
      x-api-path-slug: spatiallevels-get
      responses:
        200:
          description: OK
      tags:
      - Spatial
      - Levels
  /spatial/zone/{id}:
    get:
      summary: Get Spatial Zone
      description: Fetch a zone
      operationId: getSpatialZone
      x-api-path-slug: spatialzoneid-get
      parameters:
      - in: path
        name: id
        description: A zone identifier
      responses:
        200:
          description: OK
      tags:
      - Spatial
      - Zone
  /spatial/zones/suggest:
    get:
      summary: Get Spatial Zones Suggest
      description: Suggest geospatial zones
      operationId: getSpatialZonesSuggest
      x-api-path-slug: spatialzonessuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Spatial
      - Zones
      - Suggest
  /spatial/zones/{ids}:
    get:
      summary: Get Spatial Zones S
      description: Fetch a zone list as GeoJSON
      operationId: getSpatialZonesS
      x-api-path-slug: spatialzonesids-get
      parameters:
      - in: path
        name: ids
        description: A zone identifiers list (comma separated)
      responses:
        200:
          description: OK
      tags:
      - Spatial
      - Zones
      - S
  /tags/suggest/:
    get:
      summary: Get Tags Suggest
      description: Suggest tags
      operationId: getTagsSuggest
      x-api-path-slug: tagssuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Suggest
  /territory/suggest/:
    get:
      summary: Get Territory Suggest
      description: ""
      operationId: getTerritorySuggest
      x-api-path-slug: territorysuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The maximum result size
      responses:
        200:
          description: OK
      tags:
      - Territory
      - Suggest
  /topics/:
    get:
      summary: Get Topics
      description: List all topics
      operationId: getTopics
      x-api-path-slug: topics-get
      parameters:
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Topics
    post:
      summary: Add Topics
      description: Create a topic
      operationId: postTopics
      x-api-path-slug: topics-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Topics
  /topics/{topic}/:
    delete:
      summary: Delete Topics Topic
      description: Delete a given topic
      operationId: deleteTopicsTopic
      x-api-path-slug: topicstopic-delete
      parameters:
      - in: path
        name: topic
        description: The topic ID or slug
      responses:
        200:
          description: OK
      tags:
      - Topics
      - Topic
    get:
      summary: Get Topics Topic
      description: Get a given topic
      operationId: getTopicsTopic
      x-api-path-slug: topicstopic-get
      parameters:
      - in: path
        name: topic
        description: The topic ID or slug
      responses:
        200:
          description: OK
      tags:
      - Topics
      - Topic
    put:
      summary: Put Topics Topic
      description: Update a given topic
      operationId: putTopicsTopic
      x-api-path-slug: topicstopic-put
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: topic
        description: The topic ID or slug
      responses:
        200:
          description: OK
      tags:
      - Topics
      - Topic
  /transfer/:
    get:
      summary: Get Transfer
      description: List all transfer requests
      operationId: getTransfer
      x-api-path-slug: transfer-get
      responses:
        200:
          description: OK
      tags:
      - Transfer
    post:
      summary: Add Transfer
      description: Initiate transfer request
      operationId: postTransfer
      x-api-path-slug: transfer-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Transfer
  /transfer/{id}/:
    get:
      summary: Get Transfer
      description: Fetch a transfer request given its identifier
      operationId: getTransfer
      x-api-path-slug: transferid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Transfer
    post:
      summary: Add Transfer
      description: Respond to a transfer request
      operationId: postTransfer
      x-api-path-slug: transferid-post
      parameters:
      - in: path
        name: id
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Transfer
  /users/:
    get:
      summary: Get Users
      description: List all objects
      operationId: getUsers
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: datasets
      - in: query
        name: facets
        description: Selected facets to fetch
      - in: query
        name: organization
      - in: query
        name: page
        description: The page to display
      - in: query
        name: page_size
        description: The page size
      - in: query
        name: q
        description: The search query
      - in: query
        name: reuses
      - in: query
        name: sort
        description: The field (and direction) on which sorting apply
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Add Users
      description: Create a new object
      operationId: postUsers
      x-api-path-slug: users-post
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/suggest/:
    get:
      summary: Get Users Suggest
      description: Suggest users
      operationId: getUsersSuggest
      x-api-path-slug: userssuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Users
      - Suggest
  /users/{id}/followers/:
    delete:
      summary: Delete Users  Followers
      description: Unfollow an object given its ID
      operationId: deleteUsersFollowers
      x-api-path-slug: usersidfollowers-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Users
      - ""
      - Followers
    get:
      summary: Get Users  Followers
      description: List all followers for a given object
      operationId: getUsersFollowers
      x-api-path-slug: usersidfollowers-get
      parameters:
      - in: path
        name: id
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Users
      - ""
      - Followers
    post:
      summary: Add Users  Followers
      description: Follow an user given its ID
      operationId: postUsersFollowers
      x-api-path-slug: usersidfollowers-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Users
      - ""
      - Followers
  /users/{user}/:
    delete:
      summary: Delete Users User
      description: Delete a given object
      operationId: deleteUsersUser
      x-api-path-slug: usersuser-delete
      parameters:
      - in: path
        name: user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
    get:
      summary: Get Users User
      description: Get a given object
      operationId: getUsersUser
      x-api-path-slug: usersuser-get
      parameters:
      - in: path
        name: user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
    put:
      summary: Put Users User
      description: Update a given object
      operationId: putUsersUser
      x-api-path-slug: usersuser-put
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
  /workers/jobs/:
    get:
      summary: Get Workers Jobs
      description: List all scheduled jobs
      operationId: getWorkersJobs
      x-api-path-slug: workersjobs-get
      responses:
        200:
          description: OK
      tags:
      - Workers
      - Jobs
    post:
      summary: Add Workers Jobs
      description: Create a new scheduled job
      operationId: postWorkersJobs
      x-api-path-slug: workersjobs-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Workers
      - Jobs
  /workers/jobs/schedulables:
    get:
      summary: Get Workers Jobs Schedulables
      description: List all schedulable jobs
      operationId: getWorkersJobsSchedulables
      x-api-path-slug: workersjobsschedulables-get
      responses:
        200:
          description: OK
      tags:
      - Workers
      - Jobs
      - Schedulables
  /workers/jobs/{id}:
    delete:
      summary: Delete Workers Jobs
      description: Delete a single scheduled job
      operationId: deleteWorkersJobs
      x-api-path-slug: workersjobsid-delete
      parameters:
      - in: path
        name: id
        description: A job ID
      responses:
        200:
          description: OK
      tags:
      - Workers
      - Jobs
    get:
      summary: Get Workers Jobs
      description: Fetch a single scheduled job
      operationId: getWorkersJobs
      x-api-path-slug: workersjobsid-get
      parameters:
      - in: path
        name: id
        description: A job ID
      responses:
        200:
          description: OK
      tags:
      - Workers
      - Jobs
    put:
      summary: Put Workers Jobs
      description: Update a single scheduled job
      operationId: putWorkersJobs
      x-api-path-slug: workersjobsid-put
      parameters:
      - in: path
        name: id
        description: A job ID
      responses:
        200:
          description: OK
      tags:
      - Workers
      - Jobs
  /workers/tasks/{id}:
    get:
      summary: Get Workers Tasks
      description: Get a tasks status given its ID
      operationId: getWorkersTasks
      x-api-path-slug: workerstasksid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Workers
      - Tasks