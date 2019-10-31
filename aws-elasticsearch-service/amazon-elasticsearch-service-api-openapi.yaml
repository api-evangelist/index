swagger: "2.0"
x-collection-name: AWS Elasticsearch Service
x-complete: 1
info:
  title: AWS Elasticsearch Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2015-01-01/tags:
    post:
      summary: Add Tags
      description: |-
        Attaches resource tags to an Amazon ES domain. Use the POST HTTP method
                        with this operation. For more information, see Tagging Amazon ES
                        Domains.
      operationId: addTags
      x-api-path-slug: 20150101tags-post
      responses:
        200:
          description: OK
      tags:
      - Tags
  /2015-01-01/es/domain:
    post:
      summary: Create Elasticsearch Domain
      description: |-
        Creates a new Amazon ES domain. Use the HTTP POST method with this
                        operation. For more information, see Creating Amazon ES Domains.
      operationId: createElasticsearchDomain
      x-api-path-slug: 20150101esdomain-post
      responses:
        200:
          description: OK
      tags:
      - Domains
  /2015-01-01/es/domain/{domain_name}:
    delete:
      summary: Delete Elasticsearch Domain
      description: |-
        Deletes an Amazon ES domain and all of its data. A domain cannot be recovered after it
                        is deleted. Use the DELETE HTTP method with this operation.
      operationId: deleteElasticsearchDomain
      x-api-path-slug: 20150101esdomaindomain-name-delete
      responses:
        200:
          description: OK
      tags:
      - Domains
    get:
      summary: Describe Elasticsearch Domain
      description: |-
        Describes the domain configuration for the specified Amazon ES domain, including the
                        domain ID, domain service endpoint, and domain ARN. Use the HTTP GET
                        method with this operation.
      operationId: describeElasticsearchDomain
      x-api-path-slug: 20150101esdomaindomain-name-get
      parameters:
      - in: query
        name: DomainName
        description: Name of the Amazon ES domain that you want to                                        describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /2015-01-01/es/domain-info:
    post:
      summary: Describe Elasticsearch Domains
      description: |-
        Describes the domain configuration for up to five specified Amazon ES domains.
                        Information includes the domain ID, domain service endpoint, and domain ARN. Use the
                        HTTP POST method with this operation.
      operationId: describeElasticsearchDomains
      x-api-path-slug: 20150101esdomaininfo-post
      parameters:
      - in: body
        name: DomainNames
        description: Array of Amazon ES domains in the following                                            format:{DomainNames:[&lt;Domain_Name&gt;,&lt;Domain_Name&gt;
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Domains
  /2015-01-01/domain:
    get:
      summary: List Domain Names
      description: Displays the names of all Amazon ES domains owned by the current
        user.
      operationId: listDomainNames
      x-api-path-slug: 20150101domain-get
      responses:
        200:
          description: OK
      tags:
      - Domains
  /2015-01-01/es/domain/{domain_name}/config:
    get:
      summary: Describe Elasticsearch Domain Config
      description: |-
        Displays the configuration of an Amazon ES domain. Use the HTTP GET method
                        with this operation.
      operationId: describeElasticsearchDomainConfig
      x-api-path-slug: 20150101esdomaindomain-nameconfig-get
      parameters:
      - in: query
        name: DomainName
        description: Name of the Amazon ES domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
    post:
      summary: Update Elasticsearch Domain Config
      description: |-
        Modifies the configuration of an Amazon ES domain, such as the instance type and the
                        number of instances. Use the POST HTTP method with this
                        operation.
      operationId: updateElasticsearchDomainConfig
      x-api-path-slug: 20150101esdomaindomain-nameconfig-post
      responses:
        200:
          description: OK
      tags:
      - Domains
  /2015-01-01/tags?arn={domain_arn}:
    get:
      summary: List Tags
      description: |-
        Displays all of the tags for an Amazon ES domain. Use the GET HTTP method
                        with this operation.
      operationId: listTags
      x-api-path-slug: 20150101tagsarndomain-arn-get
      responses:
        200:
          description: OK
      tags:
      - Tags
  es.{aws_region}.amazonaws.com/2015-01-01/tags-removal:
    post:
      summary: Remove Tags
      description: |-
        Removes the specified resource tags from an Amazon ES domain. Use the POST
                        HTTP method with this operation.
      operationId: removeTags
      x-api-path-slug: es-aws-region-amazonaws-com20150101tagsremoval-post
      responses:
        200:
          description: OK
      tags:
      - Tags