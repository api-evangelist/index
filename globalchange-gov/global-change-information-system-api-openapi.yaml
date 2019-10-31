swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 1
info:
  title: Global Change Information System API
  description: who-we-are-what-the-gcis-is-and-how-we-use-identifiers-and-semantic-information-to-provide-points-of-reference-and-traceability--examples-and-tutorials-for-using-this-system-as-a-researcher-citizen-scientist-application-developer-or-information-theorist--a-description-of-how-the-information-is-structured-including-the-overlaps-between-relational-and-semantic-representations-of-the-information--complete-documentation-for-the-api-including-methods-for-browsing-and-finding-resources-
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activity:
    get:
      summary: List activities.
      description: List the activities, 20 per page.
      operationId: list-the-activities-20-per-page
      x-api-path-slug: activity-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the activities
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Activities
  /activity/{activity_identifier}:
    get:
      summary: Get a representation of an activity.
      description: Get JSON which represents the structure of an activity.
      operationId: get-json-which-represents-the-structure-of-an-activity
      x-api-path-slug: activityactivity-identifier-get
      parameters:
      - in: path
        name: activity_identifier
        description: activity_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Activity
  /array:
    get:
      summary: List arrays.
      description: List the arrays, 20 per page.
      operationId: list-the-arrays-20-per-page
      x-api-path-slug: array-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the arrays
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Arrays
  /array/{array_identifier}:
    get:
      summary: Get a representation of an array.
      description: Get JSON which represents the structure of an array.
      operationId: get-json-which-represents-the-structure-of-an-array
      x-api-path-slug: arrayarray-identifier-get
      parameters:
      - in: path
        name: array_identifier
        description: array_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the array
      - in: query
        name: with_regions
        description: Include regions associated with the array
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Array
  /article:
    get:
      summary: List articles.
      description: List the articles, 20 per page.
      operationId: list-the-articles-20-per-page
      x-api-path-slug: article-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the articles
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Articles
  /article/{article_identifier}:
    get:
      summary: Get a representation of an article.
      description: Get JSON which represents the structure of an article.
      operationId: get-json-which-represents-the-structure-of-an-article
      x-api-path-slug: articlearticle-identifier-get
      parameters:
      - in: path
        name: article_identifier
        description: article_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the article
      - in: query
        name: with_regions
        description: Include regions associated with the article
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Article
  /book:
    get:
      summary: List books.
      description: List the books, 20 per page.
      operationId: list-the-books-20-per-page
      x-api-path-slug: book-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the books
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Books
  /book/{book_identifier}:
    get:
      summary: Get a representation of a book.
      description: Get JSON which represents the structure of a book.
      operationId: get-json-which-represents-the-structure-of-a-book
      x-api-path-slug: bookbook-identifier-get
      parameters:
      - in: path
        name: book_identifier
        description: book_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the book
      - in: query
        name: with_regions
        description: Include regions associated with the book
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Book
  /contributor/{contributor_identifier}:
    get:
      summary: Redirect to a particular contributor.
      description: Given a numeric ID, redirect to the full URI of a contributor.
      operationId: given-a-numeric-id-redirect-to-the-full-uri-of-a-contributor
      x-api-path-slug: contributorcontributor-identifier-get
      parameters:
      - in: path
        name: contributor_identifier
        description: contributor_identifier description
      responses:
        200:
          description: OK
      tags:
      - Redirect
      - To
      - Particular
      - Contributor
  /dataset:
    get:
      summary: List datasets.
      description: List the datasets, 20 per page.
      operationId: list-the-datasets-20-per-page
      x-api-path-slug: dataset-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the datasets
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Datasets
  /dataset/lookup/{doi}:
    get:
      summary: Look up a dataset by DOI.
      description: Given a DOI, return a redirect to the GCIS dataset.
      operationId: given-a-doi-return-a-redirect-to-the-gcis-dataset
      x-api-path-slug: datasetlookupdoi-get
      parameters:
      - in: path
        name: doi
        description: doi description
      responses:
        200:
          description: OK
      tags:
      - Look
      - Up
      - Dataset
      - By
      - DOI
  /dataset/{dataset_identifier}:
    get:
      summary: Get a representation of a dataset.
      description: Get JSON which represents the structure of a dataset.
      operationId: get-json-which-represents-the-structure-of-a-dataset
      x-api-path-slug: datasetdataset-identifier-get
      parameters:
      - in: path
        name: dataset_identifier
        description: dataset_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Dataset
  /figure:
    get:
      summary: List all figures
      description: List all the figures in GCIS.
      operationId: list-all-the-figures-in-gcis
      x-api-path-slug: figure-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the figures
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - ""
      - Figures
  /file/{file_identifier}:
    get:
      summary: Get a representation of a file.
      description: Get JSON which represents the structure of a file.
      operationId: get-json-which-represents-the-structure-of-a-file
      x-api-path-slug: filefile-identifier-get
      parameters:
      - in: path
        name: file_identifier
        description: file_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - File
  /gcmd_keyword:
    get:
      summary: List GCMD keywords in the GCIS.
      description: List the GCMD keywords in the GCIS, 20 per page.
      operationId: list-the-gcmd-keywords-in-the-gcis-20-per-page
      x-api-path-slug: gcmd-keyword-get
      parameters:
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - GCMD
      - Keywords
      - GCIS
  /gcmd_keyword/{gcmd_keyword_identifier}:
    get:
      summary: Get a representation of a GCMD keyword.
      description: Get JSON which represents the structure of a GCMD keyword.
      operationId: get-json-which-represents-the-structure-of-a-gcmd-keyword
      x-api-path-slug: gcmd-keywordgcmd-keyword-identifier-get
      parameters:
      - in: path
        name: gcmd_keyword_identifier
        description: gcmd_keyword_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - GCMD
      - Keyword
  /generic:
    get:
      summary: List generic publications.
      description: List the generic publications, 20 per page.
      operationId: list-the-generic-publications-20-per-page
      x-api-path-slug: generic-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the generic publications
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Generic
      - Publications
  /generic/{generic_identifier}:
    get:
      summary: Get a representation of a generic publication.
      description: Get JSON which represents the structure of a generic publication.
      operationId: get-json-which-represents-the-structure-of-a-generic-publication
      x-api-path-slug: genericgeneric-identifier-get
      parameters:
      - in: path
        name: generic_identifier
        description: generic_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Generic
      - Publication
  /image:
    get:
      summary: List images.
      description: List the images, 20 per page.
      operationId: list-the-images-20-per-page
      x-api-path-slug: image-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the images
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Images
  /image/{image_identifier}:
    get:
      summary: Get a representation of an image.
      description: Get JSON which represents the structure of an image.
      operationId: get-json-which-represents-the-structure-of-an-image
      x-api-path-slug: imageimage-identifier-get
      parameters:
      - in: path
        name: image_identifier
        description: image_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the image
      - in: query
        name: with_regions
        description: Include regions associated with the image
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Image
  /instrument:
    get:
      summary: List instruments.
      description: List the instruments, 20 per page.
      operationId: list-the-instruments-20-per-page
      x-api-path-slug: instrument-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the instruments
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Instruments
  /instrument/{instrument_identifier}:
    get:
      summary: Get a representation of an instrument.
      description: Get JSON which represents the structure of an instrument.
      operationId: get-json-which-represents-the-structure-of-an-instrument
      x-api-path-slug: instrumentinstrument-identifier-get
      parameters:
      - in: path
        name: instrument_identifier
        description: instrument_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Instrument
  /journal:
    get:
      summary: List journals.
      description: List the journals, 20 per page.
      operationId: list-the-journals-20-per-page
      x-api-path-slug: journal-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the journals
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Journals
  /journal/{journal_identifier}:
    get:
      summary: Get a representation of a journal.
      description: Get JSON which represents the structure of a journal.
      operationId: get-json-which-represents-the-structure-of-a-journal
      x-api-path-slug: journaljournal-identifier-get
      parameters:
      - in: path
        name: journal_identifier
        description: journal_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Journal
  /lexicon:
    get:
      summary: List lexicons.
      description: List the lexicons, 20 per page.
      operationId: list-the-lexicons-20-per-page
      x-api-path-slug: lexicon-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the lexicons
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Lexicons
  /lexicon/{lexicon_identifier}:
    get:
      summary: Get a representation of a lexicon.
      description: Get JSON which represents the structure of a lexicon.
      operationId: get-json-which-represents-the-structure-of-a-lexicon
      x-api-path-slug: lexiconlexicon-identifier-get
      parameters:
      - in: path
        name: lexicon_identifier
        description: lexicon_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Lexicon
  /lexicon/{lexicon_identifier}/find/{context}/{term}:
    get:
      summary: Lookup a GCID from a term
      description: Given a lexicon, term, and context, return a 303 redirect to a
        GCID
      operationId: given-a-lexicon-term-and-context-return-a-303-redirect-to-a-gcid
      x-api-path-slug: lexiconlexicon-identifierfindcontextterm-get
      parameters:
      - in: path
        name: context
        description: context description
      - in: path
        name: lexicon_identifier
        description: lexicon_identifier description
      - in: path
        name: term
        description: term description
      responses:
        200:
          description: OK
      tags:
      - Lookup
      - GCID
      - From
      - Term
  /lexicon/{lexicon_identifier}/list/{context}:
    get:
      summary: List the terms within a context of a lexicon
      description: List the terms within a context of a lexicon
      operationId: list-the-terms-within-a-context-of-a-lexicon
      x-api-path-slug: lexiconlexicon-identifierlistcontext-get
      parameters:
      - in: path
        name: context
        description: context description
      - in: path
        name: lexicon_identifier
        description: lexicon_identifier description
      responses:
        200:
          description: OK
      tags:
      - Terms
      - Within
      - Context
      - Lexicon
  /lexicon/{lexicon_identifier}/{context}/{term}:
    get:
      summary: Lookup a GCID from a term
      description: Given a lexicon, term, and context, return a 303 redirect to a
        GCID
      operationId: given-a-lexicon-term-and-context-return-a-303-redirect-to-a-gcid
      x-api-path-slug: lexiconlexicon-identifiercontextterm-get
      parameters:
      - in: path
        name: context
        description: context description
      - in: path
        name: lexicon_identifier
        description: lexicon_identifier description
      - in: path
        name: term
        description: term description
      responses:
        200:
          description: OK
      tags:
      - Lookup
      - GCID
      - From
      - Term
  /metrics:
    get:
      summary: Get overall metrics about GCIS data
      description: Get overall metrics about GCIS data
      operationId: get-overall-metrics-about-gcis-data
      x-api-path-slug: metrics-get
      responses:
        200:
          description: OK
      tags:
      - Overall
      - Metrics
      - About
      - GCIS
      - Data
  /model:
    get:
      summary: List models.
      description: List the models, 20 per page.
      operationId: list-the-models-20-per-page
      x-api-path-slug: model-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the models
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Models
  /model/{model_identifier}:
    get:
      summary: Get a representation of a model.
      description: Get JSON which represents the structure of a model.
      operationId: get-json-which-represents-the-structure-of-a-model
      x-api-path-slug: modelmodel-identifier-get
      parameters:
      - in: path
        name: model_identifier
        description: model_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Model
  /model/{model_identifier}/run:
    get:
      summary: List model runs for a particular model.
      description: List the model runs for a particular model, 20 per page.
      operationId: list-the-model-runs-for-a-particular-model-20-per-page
      x-api-path-slug: modelmodel-identifierrun-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the model runs
      - in: path
        name: model_identifier
        description: model_identifier description
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Model
      - Runsa
      - Particular
      - Model
  /model_run:
    get:
      summary: List model runs.
      description: List the model runs, 20 per page.
      operationId: list-the-model-runs-20-per-page
      x-api-path-slug: model-run-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the model runs
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Model
      - Runs
  /model_run/{model_identifier}/{scenario_identifier}/{range_start}/{range_end}/{spatial_resolution}/{time_resolution}/{sequence}:
    get:
      summary: Get a representation of a model run.
      description: Get JSON which represents the structure of a model run.
      operationId: get-json-which-represents-the-structure-of-a-model-run
      x-api-path-slug: model-runmodel-identifierscenario-identifierrange-startrange-endspatial-resolutiontime-resolutionsequence-get
      parameters:
      - in: path
        name: model_identifier
        description: model_identifier description
      - in: path
        name: range_end
        description: range_end description
      - in: path
        name: range_start
        description: range_start description
      - in: path
        name: scenario_identifier
        description: scenario_identifier description
      - in: path
        name: sequence
        description: sequence description
      - in: path
        name: spatial_resolution
        description: spatial_resolution description
      - in: path
        name: time_resolution
        description: time_resolution description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Model
      - Run
  /model_run/{model_run_identifier}:
    get:
      summary: Get a representation of a model run.
      description: Get JSON which represents the structure of a model run.
      operationId: get-json-which-represents-the-structure-of-a-model-run
      x-api-path-slug: model-runmodel-run-identifier-get
      parameters:
      - in: path
        name: model_run_identifier
        description: model_run_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Model
      - Run
  /organization:
    get:
      summary: List organizations.
      description: List the organizations, 20 per page.
      operationId: list-the-organizations-20-per-page
      x-api-path-slug: organization-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the organizations
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /organization/{organization_identifier}:
    get:
      summary: Get a representation of an organization.
      description: Get JSON which represents the structure of an organization.
      operationId: get-json-which-represents-the-structure-of-an-organization
      x-api-path-slug: organizationorganization-identifier-get
      parameters:
      - in: path
        name: organization_identifier
        description: organization_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Organization
  /organization/{organization_identifier}/contributions/{role_type_identifier}/{resource}:
    get:
      summary: Show contributions of a certain type by an organization
      description: Given a resource (dataset, report, etc.) and a role (editor, etc),
        and an identifier for an organization, show the resources to which the organization
        has contributed in that role.
      operationId: given-a-resource-dataset-report-etc-and-a-role-editor-etc-and-an-identifier-for-an-organization-show
      x-api-path-slug: organizationorganization-identifiercontributionsrole-type-identifierresource-get
      parameters:
      - in: path
        name: organization_identifier
        description: organization_identifier description
      - in: path
        name: resource
        description: resource description
      - in: path
        name: role_type_identifier
        description: role_type_identifier description
      responses:
        200:
          description: OK
      tags:
      - Show
      - Contributions
      - Certain
      - Type
      - By
      - Organization
  /person:
    get:
      summary: List people.
      description: List the people, 20 per page.
      operationId: list-the-people-20-per-page
      x-api-path-slug: person-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the people
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - People
  /person/{name}:
    get:
      summary: Redirect to a person based on a name
      description: Given a name (case sensitive, concatenated by dashes), redirect
        if there is a single match.  The first and last names can be in either order.
      operationId: given-a-name-case-sensitive-concatenated-by-dashes-redirect-if-there-is-a-single-match--the-first-an
      x-api-path-slug: personname-get
      parameters:
      - in: path
        name: name
        description: name description
      responses:
        200:
          description: OK
      tags:
      - Redirect
      - To
      - Person
      - Based
      - "On"
      - Name
  /person/{orcid}:
    get:
      summary: Redirect to a person based on an ORCID.
      description: Given an ORCID, if there is a match, redirect to the persons URI.
      operationId: given-an-orcid-if-there-is-a-match-redirect-to-the-persons-uri
      x-api-path-slug: personorcid-get
      parameters:
      - in: path
        name: orcid
        description: orcid description
      responses:
        200:
          description: OK
      tags:
      - Redirect
      - To
      - Person
      - Based
      - "On"
      - ORCID
  /person/{person_identifier}:
    get:
      summary: Get a representation of a person.
      description: Get JSON which represents the structure of a person.
      operationId: get-json-which-represents-the-structure-of-a-person
      x-api-path-slug: personperson-identifier-get
      parameters:
      - in: path
        name: person_identifier
        description: person_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Person
  /person/{person_identifier}/contributions/{role_type_identifier}/{resource}:
    get:
      summary: Show contributions of a certain type by a person
      description: Given a resource (dataset, report, etc.) and a role (editor, etc),
        and an identifier for a person, show the resources to which the person has
        contributed in that role.
      operationId: given-a-resource-dataset-report-etc-and-a-role-editor-etc-and-an-identifier-for-a-person-show-the-re
      x-api-path-slug: personperson-identifiercontributionsrole-type-identifierresource-get
      parameters:
      - in: path
        name: person_identifier
        description: person_identifier description
      - in: path
        name: resource
        description: resource description
      - in: path
        name: role_type_identifier
        description: role_type_identifier description
      responses:
        200:
          description: OK
      tags:
      - Show
      - Contributions
      - Certain
      - Type
      - By
      - Person
  /platform:
    get:
      summary: List platforms.
      description: List the platforms, 20 per page.
      operationId: list-the-platforms-20-per-page
      x-api-path-slug: platform-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the platforms
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Platforms
  /platform/{platform_identifier}:
    get:
      summary: Get a representation of a platform.
      description: Get JSON which represents the structure of a platform.
      operationId: get-json-which-represents-the-structure-of-a-platform
      x-api-path-slug: platformplatform-identifier-get
      parameters:
      - in: path
        name: platform_identifier
        description: platform_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Platform
  /platform/{platform_identifier}/instrument:
    get:
      summary: List instruments on a platform.
      description: List the instruments on a platform, 20 per page.
      operationId: list-the-instruments-on-a-platform-20-per-page
      x-api-path-slug: platformplatform-identifierinstrument-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the instruments
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: platform_identifier
        description: platform_identifier description
      responses:
        200:
          description: OK
      tags:
      - Instruments
      - "On"
      - Platform
  /platform/{platform_identifier}/instrument/{instrument_identifier}:
    get:
      summary: Get a representation of an instrument on a platform.
      description: Get JSON which represents the structure of an instrument on a platform.
      operationId: get-json-which-represents-the-structure-of-an-instrument-on-a-platform
      x-api-path-slug: platformplatform-identifierinstrumentinstrument-identifier-get
      parameters:
      - in: path
        name: instrument_identifier
        description: instrument_identifier description
      - in: path
        name: platform_identifier
        description: platform_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Instrument
      - "On"
      - Platform
  /project:
    get:
      summary: List projects.
      description: List the projects, 20 per page.
      operationId: list-the-projects-20-per-page
      x-api-path-slug: project-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the projects
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Projects
  /project/{project_identifier}:
    get:
      summary: Get a representation of a project.
      description: Get JSON which represents the structure of a project.
      operationId: get-json-which-represents-the-structure-of-a-project
      x-api-path-slug: projectproject-identifier-get
      parameters:
      - in: path
        name: project_identifier
        description: project_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Project
  /publication/{publication_identifier}:
    get:
      summary: Redirect to a particular publication.
      description: Given a numeric ID, redirect to the full URI of a publication.
      operationId: given-a-numeric-id-redirect-to-the-full-uri-of-a-publication
      x-api-path-slug: publicationpublication-identifier-get
      parameters:
      - in: path
        name: publication_identifier
        description: publication_identifier description
      responses:
        200:
          description: OK
      tags:
      - Redirect
      - To
      - Particular
      - Publication
  /reference:
    get:
      summary: List references.
      description: List the references, 20 per page.
      operationId: list-the-references-20-per-page
      x-api-path-slug: reference-get
      parameters:
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - References
  /reference/{reference_identifier}:
    get:
      summary: Get a representation of a reference.
      description: Get JSON which represents the structure of a reference.
      operationId: get-json-which-represents-the-structure-of-a-reference
      x-api-path-slug: referencereference-identifier-get
      parameters:
      - in: path
        name: reference_identifier
        description: reference_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Reference
  /region:
    get:
      summary: List regions.
      description: List the regions, 20 per page.
      operationId: list-the-regions-20-per-page
      x-api-path-slug: region-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the regions
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Regions
  /region/{region_identifier}:
    get:
      summary: Get a representation of a region.
      description: Get JSON which represents the structure of a region.
      operationId: get-json-which-represents-the-structure-of-a-region
      x-api-path-slug: regionregion-identifier-get
      parameters:
      - in: path
        name: region_identifier
        description: region_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Region
  /report:
    get:
      summary: Get a list of reports.
      description: List the reports, 20 per page.
      operationId: list-the-reports-20-per-page
      x-api-path-slug: report-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the reports
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: query
        name: report_type
        description: The type of report
      responses:
        200:
          description: OK
      tags:
      - Reports
  /report/{report_identifier}:
    get:
      summary: Get a representation of a report.
      description: Get JSON which represents the structure of a report.
      operationId: get-json-which-represents-the-structure-of-a-report
      x-api-path-slug: reportreport-identifier-get
      parameters:
      - in: path
        name: report_identifier
        description: report_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the report
      - in: query
        name: with_regions
        description: Include regions associated with the report
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Report
  /report/{report_identifier}/array:
    get:
      summary: List arrays associated with a report.
      description: List the arrays associated with a report, 20 per page.
      operationId: list-the-arrays-associated-with-a-report-20-per-page
      x-api-path-slug: reportreport-identifierarray-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the arrays
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Arrays
      - Associated
      - Report
  /report/{report_identifier}/book:
    get:
      summary: List books associated with a report.
      description: List the books associated with a report, 20 per page.
      operationId: list-the-books-associated-with-a-report-20-per-page
      x-api-path-slug: reportreport-identifierbook-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the books
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Books
      - Associated
      - Report
  /report/{report_identifier}/chapter:
    get:
      summary: List chapters in a report
      description: Get a list of chapters in a report.
      operationId: get-a-list-of-chapters-in-a-report
      x-api-path-slug: reportreport-identifierchapter-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the chapters
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Chapters
      - Report
  /report/{report_identifier}/chapter/{chapter_identifier}:
    get:
      summary: Get a representation of a chapter.
      description: Get JSON which represents the structure of a chapter.
      operationId: get-json-which-represents-the-structure-of-a-chapter
      x-api-path-slug: reportreport-identifierchapterchapter-identifier-get
      parameters:
      - in: path
        name: chapter_identifier
        description: chapter_identifier description
      - in: path
        name: ids
        description: '{ids} can contain up to 100 semicolon delimited ids, to find
          ids programatically look for answer_id on answer objects'
      - in: path
        name: report_identifier
        description: report_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the chapter
      - in: query
        name: with_regions
        description: Include regions associated with the chapter
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Chapter
  /report/{report_identifier}/chapter/{chapter_identifier}/figure:
    get:
      summary: List figures in a chapter
      description: Get a list of figures in a chapter.
      operationId: get-a-list-of-figures-in-a-chapter
      x-api-path-slug: reportreport-identifierchapterchapter-identifierfigure-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the figures
      - in: path
        name: chapter_identifier
        description: chapter_identifier description
      - in: path
        name: ids
        description: '{ids} can contain up to 100 semicolon delimited ids, to find
          ids programatically look for answer_id on answer objects'
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Figures
      - Chapter
  /report/{report_identifier}/chapter/{chapter_identifier}/figure/{figure_identifier}:
    get:
      summary: Get a representation of a figure in a chapter.
      description: Get JSON which represents the structure of a figure in a chapter.
      operationId: get-json-which-represents-the-structure-of-a-figure-in-a-chapter
      x-api-path-slug: reportreport-identifierchapterchapter-identifierfigurefigure-identifier-get
      parameters:
      - in: path
        name: chapter_identifier
        description: chapter_identifier description
      - in: path
        name: figure_identifier
        description: figure_identifier description
      - in: path
        name: ids
        description: '{ids} can contain up to 100 semicolon delimited ids, to find
          ids programatically look for answer_id on answer objects'
      - in: path
        name: report_identifier
        description: report_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the figure
      - in: query
        name: with_regions
        description: Include regions associated with the figure
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Figure
      - Chapter
  /report/{report_identifier}/chapter/{chapter_identifier}/finding:
    get:
      summary: List findings in a chapter
      description: Get a list of findings in a chapter.
      operationId: get-a-list-of-findings-in-a-chapter
      x-api-path-slug: reportreport-identifierchapterchapter-identifierfinding-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the findings
      - in: path
        name: chapter_identifier
        description: chapter_identifier description
      - in: path
        name: ids
        description: '{ids} can contain up to 100 semicolon delimited ids, to find
          ids programatically look for answer_id on answer objects'
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Findings
      - Chapter
  /report/{report_identifier}/chapter/{chapter_identifier}/finding/{finding_identifier}:
    get:
      summary: Get a representation of a finding in a chapter.
      description: Get JSON which represents the structure of a finding in a chapter.
      operationId: get-json-which-represents-the-structure-of-a-finding-in-a-chapter
      x-api-path-slug: reportreport-identifierchapterchapter-identifierfindingfinding-identifier-get
      parameters:
      - in: path
        name: chapter_identifier
        description: chapter_identifier description
      - in: path
        name: finding_identifier
        description: finding_identifier description
      - in: path
        name: report_identifier
        description: report_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the finding
      - in: query
        name: with_regions
        description: Include regions associated with the finding
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Finding
      - Chapter
  /report/{report_identifier}/chapter/{chapter_identifier}/reference:
    get:
      summary: List references in a chapter
      description: Get a list of references in a chapter.
      operationId: get-a-list-of-references-in-a-chapter
      x-api-path-slug: reportreport-identifierchapterchapter-identifierreference-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the references
      - in: path
        name: chapter_identifier
        description: chapter_identifier description
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - References
      - Chapter
  /report/{report_identifier}/chapter/{chapter_identifier}/table:
    get:
      summary: List tables in a chapter
      description: Get a list of tables in a chapter.
      operationId: get-a-list-of-tables-in-a-chapter
      x-api-path-slug: reportreport-identifierchapterchapter-identifiertable-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the tables
      - in: path
        name: chapter_identifier
        description: chapter_identifier description
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Tables
      - Chapter
  /report/{report_identifier}/chapter/{chapter_identifier}/table/{table_identifier}:
    get:
      summary: Get a representation of a table in a chapter.
      description: Get JSON which represents the structure of a table in a chapter.
      operationId: get-json-which-represents-the-structure-of-a-table-in-a-chapter
      x-api-path-slug: reportreport-identifierchapterchapter-identifiertabletable-identifier-get
      parameters:
      - in: path
        name: chapter_identifier
        description: chapter_identifier description
      - in: path
        name: report_identifier
        description: report_identifier description
      - in: path
        name: table_identifier
        description: table_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the table
      - in: query
        name: with_regions
        description: Include regions associated with the table
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Table
      - Chapter
  /report/{report_identifier}/figure:
    get:
      summary: List figures in a report.
      description: List the figures in a report, 20 per page.
      operationId: list-the-figures-in-a-report-20-per-page
      x-api-path-slug: reportreport-identifierfigure-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the figures
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Figures
      - Report
  /report/{report_identifier}/figure/{figure_identifier}:
    get:
      summary: Get a representation of a figure.
      description: Get JSON which represents the structure of a figure.
      operationId: get-json-which-represents-the-structure-of-a-figure
      x-api-path-slug: reportreport-identifierfigurefigure-identifier-get
      parameters:
      - in: path
        name: figure_identifier
        description: figure_identifier description
      - in: path
        name: report_identifier
        description: report_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the figure
      - in: query
        name: with_regions
        description: Include regions associated with the figure
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Figure
  /report/{report_identifier}/finding:
    get:
      summary: List findings in a report.
      description: List the findings in a report, 20 per page.
      operationId: list-the-findings-in-a-report-20-per-page
      x-api-path-slug: reportreport-identifierfinding-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the findings
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Findings
      - Report
  /report/{report_identifier}/finding/{finding_identifier}:
    get:
      summary: Get a representation of a finding.
      description: Get JSON which represents the structure of a finding.
      operationId: get-json-which-represents-the-structure-of-a-finding
      x-api-path-slug: reportreport-identifierfindingfinding-identifier-get
      parameters:
      - in: path
        name: finding_identifier
        description: finding_identifier description
      - in: path
        name: report_identifier
        description: report_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the finding
      - in: query
        name: with_regions
        description: Include regions associated with the finding
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Finding
  /report/{report_identifier}/image:
    get:
      summary: List images associated with a report.
      description: List the images associated with a report, 20 per page.
      operationId: list-the-images-associated-with-a-report-20-per-page
      x-api-path-slug: reportreport-identifierimage-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the images
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Images
      - Associated
      - Report
  /report/{report_identifier}/reference:
    get:
      summary: List references in a report.
      description: List the references in a report, 20 per page.
      operationId: list-the-references-in-a-report-20-per-page
      x-api-path-slug: reportreport-identifierreference-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the references
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - References
      - Report
  /report/{report_identifier}/table:
    get:
      summary: List tables in a report.
      description: List the tables in a report, 20 per page.
      operationId: list-the-tables-in-a-report-20-per-page
      x-api-path-slug: reportreport-identifiertable-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the tables
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Tables
      - Report
  /report/{report_identifier}/table/{table_identifier}:
    get:
      summary: Get a representation of a table.
      description: Get JSON which represents the structure of a table.
      operationId: get-json-which-represents-the-structure-of-a-table
      x-api-path-slug: reportreport-identifiertabletable-identifier-get
      parameters:
      - in: path
        name: report_identifier
        description: report_identifier description
      - in: path
        name: table_identifier
        description: table_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the table
      - in: query
        name: with_regions
        description: Include regions associated with the table
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Table
  /report/{report_identifier}/webpage:
    get:
      summary: List webpages associated with a report.
      description: List the webpages associated with a report, 20 per page.
      operationId: list-the-webpages-associated-with-a-report-20-per-page
      x-api-path-slug: reportreport-identifierwebpage-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the webpages
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: report_identifier
        description: report_identifier description
      responses:
        200:
          description: OK
      tags:
      - Webpages
      - Associated
      - Report
  /role_type:
    get:
      summary: List roles
      description: Get a list of the types of roles for contributors.
      operationId: get-a-list-of-the-types-of-roles-for-contributors
      x-api-path-slug: role-type-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the contributors
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Roles
  /scenario:
    get:
      summary: List scenarios.
      description: List the scenarios, 20 per page.
      operationId: list-the-scenarios-20-per-page
      x-api-path-slug: scenario-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the scenarios
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Scenarios
  /scenario/{scenario_identifier}:
    get:
      summary: Get a representation of a scenario.
      description: Get JSON which represents the structure of a scenario.
      operationId: get-json-which-represents-the-structure-of-a-scenario
      x-api-path-slug: scenarioscenario-identifier-get
      parameters:
      - in: path
        name: scenario_identifier
        description: scenario_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Scenario
  /scenario/{scenario_identifier}/run:
    get:
      summary: List model runs for a particular scenario.
      description: List the model runs for a particular scenario, 20 per page.
      operationId: list-the-model-runs-for-a-particular-scenario-20-per-page
      x-api-path-slug: scenarioscenario-identifierrun-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the model runs
      - in: query
        name: page
        description: The page number (starting at 1)
      - in: path
        name: scenario_identifier
        description: scenario_identifier description
      responses:
        200:
          description: OK
      tags:
      - Model
      - Runsa
      - Particular
      - Scenario
  /uuid:
    get:
      summary: Generate a UUID.
      description: <p>Generate version 4 Universally Unique Identifiers.  The algorithm
        used for thisn    is described <a target=_blank href=https://en.wikipedia.org/wiki/UUID#Version_4_.28random.29>here</a>.n    </p>
      operationId: pgenerate-version-4-universally-unique-identifiers--the-algorithm-used-for-this----is-described-a-ta
      x-api-path-slug: uuid-get
      parameters:
      - in: query
        name: count
        description: Number of UUIDs to generate (max 1000)
      responses:
        200:
          description: OK
      tags:
      - Generate
      - UUID
  /webpage:
    get:
      summary: List web pages.
      description: List the web pages, 20 per page.
      operationId: list-the-web-pages-20-per-page
      x-api-path-slug: webpage-get
      parameters:
      - in: query
        name: all
        description: Set to 1 to get all of the web pages
      - in: query
        name: page
        description: The page number (starting at 1)
      responses:
        200:
          description: OK
      tags:
      - Web
      - Pages
  /webpage/{webpage_identifier}:
    get:
      summary: Get a representation of a web page.
      description: Get JSON which represents the structure of a web page.
      operationId: get-json-which-represents-the-structure-of-a-web-page
      x-api-path-slug: webpagewebpage-identifier-get
      parameters:
      - in: path
        name: webpage_identifier
        description: webpage_identifier description
      - in: query
        name: with_gcmd
        description: Include GCMD keywords associated with the web page
      - in: query
        name: with_regions
        description: Include regions associated with the web page
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Web
      - Page