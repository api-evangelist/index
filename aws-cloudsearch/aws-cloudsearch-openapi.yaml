swagger: "2.0"
x-collection-name: AWS CloudSearch
x-complete: 1
info:
  title: AWS CloudSearch
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddTags:
    get:
      summary: Add Tags
      description: |-
        Attaches resource tags to an
         Amazon CloudSearch domain.
      operationId: AddTags
      x-api-path-slug: actionaddtags-get
      parameters:
      - in: query
        name: Base
        description: An                  error occurred while processing the request
        type: string
      - in: query
        name: InternalException
        description: The processing of the request failed because of an internal service
          error
        type: string
      - in: query
        name: LimitExceededException
        description: The request contains more than the allowed number and type of
          Amazon CloudSearch domain                  resources
        type: string
      - in: query
        name: ValidationException
        description: The request contains invalid input or is missing required input
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=BuildSuggesters:
    get:
      summary: Build Suggesters
      description: Indexes the search suggestions.
      operationId: BuildSuggesters
      x-api-path-slug: actionbuildsuggesters-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Suggesters
  /?Action=CreateDomain:
    get:
      summary: Create Domain
      description: Creates a new search domain.
      operationId: CreateDomain
      x-api-path-slug: actioncreatedomain-get
      parameters:
      - in: query
        name: DomainName
        description: A name for the domain you are creating
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=DefineAnalysisScheme:
    get:
      summary: Define Analysis Scheme
      description: Configures an analysis scheme that can be applied to a text or
        text-array field to define language-specific text processing options.
      operationId: DefineAnalysisScheme
      x-api-path-slug: actiondefineanalysisscheme-get
      parameters:
      - in: query
        name: AnalysisScheme
        description: Configuration information for an analysis scheme
        type: string
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Analysis Scheme
  /?Action=DefineExpression:
    get:
      summary: Define Expression
      description: Configures an Expression  for the search domain.
      operationId: DefineExpression
      x-api-path-slug: actiondefineexpression-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: Expression
        description: A named expression that can be evaluated at search time
        type: string
      responses:
        200:
          description: OK
      tags:
      - Expressions
  /?Action=DefineIndexField:
    get:
      summary: Define Index Field
      description: Configures an ndexField  for the search domain.
      operationId: DefineIndexField
      x-api-path-slug: actiondefineindexfield-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: IndexField
        description: The index field and field options you want to configure
        type: string
      responses:
        200:
          description: OK
      tags:
      - Index Fields
  /?Action=DefineSuggester:
    get:
      summary: Define Suggester
      description: Configures a suggester for a domain.
      operationId: DefineSuggester
      x-api-path-slug: actiondefinesuggester-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: Suggester
        description: Configuration information for a search suggester
        type: string
      responses:
        200:
          description: OK
      tags:
      - Suggesters
  /?Action=DeleteAnalysisScheme:
    get:
      summary: Delete Analysis Scheme
      description: Deletes an analysis scheme.
      operationId: DeleteAnalysisScheme
      x-api-path-slug: actiondeleteanalysisscheme-get
      parameters:
      - in: query
        name: AnalysisSchemeName
        description: The name of the analysis scheme you want to delete
        type: string
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Analysis Scheme
  /?Action=DeleteDomain:
    get:
      summary: Delete Domain
      description: Permanently deletes a search domain and all of its data.
      operationId: DeleteDomain
      x-api-path-slug: actiondeletedomain-get
      parameters:
      - in: query
        name: DomainName
        description: The name of the domain you want to permanently delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=DeleteExpression:
    get:
      summary: Delete Expression
      description: "Removes an \n  Expression\n  from the search domain."
      operationId: DeleteExpression
      x-api-path-slug: actiondeleteexpression-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: ExpressionName
        description: The name of the                         Expression                      to
          delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Expressions
  /?Action=DeleteIndexField:
    get:
      summary: Delete Index Field
      description: "Removes an \n  IndexField\n  from the search domain."
      operationId: DeleteIndexField
      x-api-path-slug: actiondeleteindexfield-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: IndexFieldName
        description: The name of the index field your want to remove from the domains
          indexing options
        type: string
      responses:
        200:
          description: OK
      tags:
      - Index Fields
  /?Action=DeleteSuggester:
    get:
      summary: Delete Suggester
      description: Deletes a suggester.
      operationId: DeleteSuggester
      x-api-path-slug: actiondeletesuggester-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: SuggesterName
        description: Specifies the name of the suggester you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Suggesters
  /?Action=DescribeAnalysisSchemes:
    get:
      summary: Describe Analysis Schemes
      description: Gets the analysis schemes configured for a domain.
      operationId: DescribeAnalysisSchemes
      x-api-path-slug: actiondescribeanalysisschemes-get
      parameters:
      - in: query
        name: AnalysisSchemeNames.member.N
        description: The analysis schemes you want to describe
        type: string
      - in: query
        name: Deployed
        description: Whether to display the deployed configuration (true) or include
          any pending changes (false)
        type: string
      - in: query
        name: DomainName
        description: The name of the domain you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Analysis Scheme
  /?Action=DescribeAvailabilityOptions:
    get:
      summary: Describe Availability Options
      description: Gets the availability options configured for a domain.
      operationId: DescribeAvailabilityOptions
      x-api-path-slug: actiondescribeavailabilityoptions-get
      parameters:
      - in: query
        name: Deployed
        description: Whether to display the deployed configuration (true) or include
          any pending changes (false)
        type: string
      - in: query
        name: DomainName
        description: The name of the domain you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Availability Options
  /?Action=DescribeDomains:
    get:
      summary: Describe Domains
      description: Gets information about the search domains owned by this account.
      operationId: DescribeDomains
      x-api-path-slug: actiondescribedomains-get
      parameters:
      - in: query
        name: DomainNames.member.N
        description: The names of the domains you want to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=DescribeExpressions:
    get:
      summary: Describe Expressions
      description: Gets the expressions configured for the search domain.
      operationId: DescribeExpressions
      x-api-path-slug: actiondescribeexpressions-get
      parameters:
      - in: query
        name: Deployed
        description: Whether to display the deployed configuration (true) or include
          any pending changes (false)
        type: string
      - in: query
        name: DomainName
        description: The name of the domain you want to describe
        type: string
      - in: query
        name: ExpressionNames.member.N
        description: Limits the                         DescribeExpressions                      response
          to the specified expressions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Expressions
  /?Action=DescribeIndexFields:
    get:
      summary: Describe Index Fields
      description: Gets information about the index fields configured for the search
        domain.
      operationId: DescribeIndexFields
      x-api-path-slug: actiondescribeindexfields-get
      parameters:
      - in: query
        name: Deployed
        description: Whether to display the deployed configuration (true) or include
          any pending changes (false)
        type: string
      - in: query
        name: DomainName
        description: The name of the domain you want to describe
        type: string
      - in: query
        name: FieldNames.member.N
        description: A list of the index fields you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Index Fields
  /?Action=DescribeScalingParameters:
    get:
      summary: Describe Scaling Parameters
      description: Gets the scaling parameters configured for a domain.
      operationId: DescribeScalingParameters
      x-api-path-slug: actiondescribescalingparameters-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scaling Parameters
  /?Action=DescribeServiceAccessPolicies:
    get:
      summary: Describe Service Access Policies
      description: Gets information about the access policies that control access
        to the domain's document and search endpoints.
      operationId: DescribeServiceAccessPolicies
      x-api-path-slug: actiondescribeserviceaccesspolicies-get
      parameters:
      - in: query
        name: Deployed
        description: Whether to display the deployed configuration (true) or include
          any pending changes (false)
        type: string
      - in: query
        name: DomainName
        description: The name of the domain you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Service Access Policies
  /?Action=DescribeSuggesters:
    get:
      summary: Describe Suggesters
      description: Gets the suggesters configured for a domain.
      operationId: DescribeSuggesters
      x-api-path-slug: actiondescribesuggesters-get
      parameters:
      - in: query
        name: Deployed
        description: Whether to display the deployed configuration (true) or include
          any pending changes (false)
        type: string
      - in: query
        name: DomainName
        description: The name of the domain you want to describe
        type: string
      - in: query
        name: SuggesterNames.member.N
        description: The suggesters you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Suggesters
  /?Action=IndexDocuments:
    get:
      summary: Index Documents
      description: Tells the search domain to start indexing its documents using the
        latest indexing options.
      operationId: IndexDocuments
      x-api-path-slug: actionindexdocuments-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Index Documents
  /?Action=ListDomainNames:
    get:
      summary: List Domain Names
      description: Lists all search domains owned by an account.
      operationId: ListDomainNames
      x-api-path-slug: actionlistdomainnames-get
      parameters:
      - in: query
        name: DomainNames
        description: The names of the search domains owned by an account
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=ListTags:
    get:
      summary: List Tags
      description: |-
        Displays all of the resource
         tags for an Amazon CloudSearch domain.
      operationId: ListTags
      x-api-path-slug: actionlisttags-get
      parameters:
      - in: query
        name: Base
        description: An error occurred while                  processing the request
        type: string
      - in: query
        name: InternalException
        description: The                  processing of the request failed because
          of an internal service error
        type: string
      - in: query
        name: LimitExceededException
        description: The                  request contains more than the allowed number
          and type of Amazon CloudSearch domain resources
        type: string
      - in: query
        name: ValidationException
        description: The                  request contains invalid input or is missing
          required input
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=RemoveTags:
    get:
      summary: Remove Tags
      description: |-
        Removes the specified resource tags
         from an Amazon ES domain.
      operationId: RemoveTags
      x-api-path-slug: actionremovetags-get
      parameters:
      - in: query
        name: Base
        description: An error occurred while                  processing the request
        type: string
      - in: query
        name: InternalException
        description: The                  processing of the request failed because
          of an internal service error
        type: string
      - in: query
        name: ValidationException
        description: The                  request contains invalid input or is missing
          required input
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=UpdateAvailabilityOptions:
    get:
      summary: Update Availability Options
      description: Configures the availability options for a domain.
      operationId: UpdateAvailabilityOptions
      x-api-path-slug: actionupdateavailabilityoptions-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: MultiAZ
        description: You expand an existing search domain to a second Availability
          Zone by setting the Multi-AZ option to true
        type: string
      responses:
        200:
          description: OK
      tags:
      - Availability Options
  /?Action=UpdateScalingParameters:
    get:
      summary: Update Scaling Parameters
      description: Configures scaling parameters for a domain.
      operationId: UpdateScalingParameters
      x-api-path-slug: actionupdatescalingparameters-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: ScalingParameters
        description: The desired instance type and desired number of replicas of each
          index partition
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scaling Parameters
  /?Action=UpdateServiceAccessPolicies:
    get:
      summary: Update Service Access Policies
      description: Configures the access rules that control access to the domain's
        document and search endpoints.
      operationId: UpdateServiceAccessPolicies
      x-api-path-slug: actionupdateserviceaccesspolicies-get
      parameters:
      - in: query
        name: AccessPolicies
        description: The access rules you want to configure
        type: string
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Service Access Policies
  /2013-01-01/documents/batch:
    get:
      summary: Search Documents
      description: You use the document service API to add, replace, or delete documents
        in your Amazon CloudSearch domain. For more information managing the documents
        in your search domain, see Uploading Data to an Amazon CloudSearch Domain.
      operationId: search
      x-api-path-slug: 20130101documentsbatch-get
      parameters:
      - in: body
        name: fields
        description: A collection of one or more field_name properties that define
          the fields the document contains
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: field_name
        description: Specifies a field within the document being added
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: id
        description: An alphanumeric string
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: type
        description: The operation type, add or delete
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Search