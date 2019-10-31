swagger: "2.0"
x-collection-name: Code.gov
x-complete: 1
info:
  title: Code.gov API
  description: code-gov-api-documentation--while-using-this-documentation-locally-please-choose-to-
  version: 1.0.0
host: api.code.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repos:
    get:
      summary: Get a list of repos
      description: Get list of repositories indexed by Code.gov.
      operationId: getRepos
      x-api-path-slug: repos-get
      parameters:
      - in: query
        name: agency.acronym
        description: Filters search by the Agencys acronym
      - in: query
        name: agency.name
        description: Filters search by the Agencys name
      - in: query
        name: agency.website
        description: Filters search by the Agencys website URL
      - in: query
        name: contact.email
        description: Filters search by the repositorys contact email
      - in: query
        name: contact.name
        description: Filters search by the repositorys contact name
      - in: query
        name: date.created
        description: Filters search by the repositorys created date
      - in: query
        name: date.lastModified
        description: Filters search by the last date the repository was modified
      - in: query
        name: from
        description: Sets the offset from where to paginate
      - in: query
        name: laborHours
        description: Filters search by the amount of labor hours dedicated to the
          project
      - in: query
        name: languages
        description: Filters search by programming languages
      - in: query
        name: name
        description: Filters search by the repositorys name
      - in: query
        name: organization
        description: Filters search by the repositorys organization
      - in: query
        name: permissions.licenses.name
        description: Filters search by the repositorys license name
      - in: query
        name: permissions.usageType
        description: Filters search by the repositorys usage type
      - in: query
        name: q
        description: Text to search for
      - in: query
        name: size
        description: Sets the size of the results returned
      - in: query
        name: status
        description: Filters search by the repositorys status
      - in: query
        name: tags
        description: Filters search by the repositorys tags
      - in: query
        name: vcs
        description: Filters search by the version control system for the repository
      responses:
        200:
          description: OK
      tags:
      - Code
      - Repositories
  /repos/{repoId}:
    get:
      summary: Get information for specified repoId
      description: Gets the information of a specific repository index with the passed
        repoId.
      operationId: getReposRepo
      x-api-path-slug: reposrepoid-get
      parameters:
      - in: path
        name: repoId
        description: ID of repo to return
      responses:
        200:
          description: OK
      tags:
      - Code
      - Repositories
  /terms:
    get:
      summary: Get a list of terms
      description: Get a list of terms that were extracted from the repositories indexed.
      operationId: getTerms
      x-api-path-slug: terms-get
      parameters:
      - in: query
        name: from
        description: Sets the offset from where to paginate
      - in: query
        name: size
        description: Sets the size of the results returned
      - in: query
        name: term
        description: Filters the result set by the term value
      - in: query
        name: term_type
        description: Filters the result set by the term type
      responses:
        200:
          description: OK
      tags:
      - Code
      - Terms of Service
  /agencies:
    get:
      summary: Get a list of agencies
      description: Get a list of agencies.
      operationId: getAgencies
      x-api-path-slug: agencies-get
      parameters:
      - in: query
        name: from
        description: Specify an offset to return
      - in: query
        name: size
        description: Number of agencies to return
      responses:
        200:
          description: OK
      tags:
      - Agencies
  /languages:
    get:
      summary: Get a list of programming languages found in our code inventory.
      description: This returns a list of the programming languages that are used
        in the indexed code inventory. When a repo is index the programming language
        is extracted written to a file.
      operationId: getLanguages
      x-api-path-slug: languages-get
      parameters:
      - in: query
        name: from
        description: Specify an offset to return
      - in: query
        name: size
        description: Number of programming languages to return
      responses:
        200:
          description: OK
      tags:
      - Languages
  /repo.json:
    get:
      summary: Get the JSON schema for a repo
      description: Get the json schema for a repo.
      operationId: getRepo
      x-api-path-slug: repo-json-get
      responses:
        200:
          description: OK
      tags:
      - Code
      - Repositories
  /status.json:
    get:
      summary: Get a list of agencies with their compliance status
      description: Get a list of agencies with their Federal Source Code Policy compliance
        status
      operationId: getStatus.json
      x-api-path-slug: status-json-get
      responses:
        200:
          description: OK
      tags:
      - Code
      - Status
  /status:
    get:
      summary: Get an HTML page rendering the agencies status from status.json
      description: Get an html page rendering the agencies status from status.json.
      operationId: getStatus
      x-api-path-slug: status-get
      responses:
        200:
          description: OK
      tags:
      - Code
      - Status
  /status/{agencyName}/issues:
    get:
      summary: Get a list of issues for a particular agency
      description: Get a list of issues for a particular agency. These issues are
        grouped by software repository.
      operationId: getStatusAgencynameIssues
      x-api-path-slug: statusagencynameissues-get
      parameters:
      - in: path
        name: agencyName
        description: Agency name
      responses:
        200:
          description: OK
      tags:
      - Code
      - Status
  /status/{agencyName}/fetched:
    get:
      summary: Get a list of repos by agency
      description: Lists out all repositories that have been indexed for a given agency.
      operationId: getStatusAgencynameFetched
      x-api-path-slug: statusagencynamefetched-get
      parameters:
      - in: path
        name: agencyName
        description: Agency name
      responses:
        200:
          description: OK
      tags:
      - Code
      - Status
  /status/{agencyName}/discovered:
    get:
      summary: Get a list of repos by agency
      description: Get a list of repos by agency.
      operationId: getStatusAgencynameDiscovered
      x-api-path-slug: statusagencynamediscovered-get
      parameters:
      - in: path
        name: agencyName
        description: Agency name
      responses:
        200:
          description: OK
      tags:
      - Code
      - Status
  /version:
    get:
      summary: Get the version of this API
      description: Get the version of this api.
      operationId: getVersion
      x-api-path-slug: version-get
      responses:
        200:
          description: OK
      tags:
      - Code
      - Version