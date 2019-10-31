swagger: "2.0"
x-collection-name: AWS Service Catalog
x-complete: 1
info:
  title: AWS Service Catalog API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AcceptPortfolioShare:
    get:
      summary: Accept Portfolio Share
      description: Accepts an offer to share a portfolio.
      operationId: acceptPortfolioShare
      x-api-path-slug: actionacceptportfolioshare-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=AssociatePrincipalWithPortfolio:
    get:
      summary: Associate Principal With Portfolio
      description: Associates the specified principal ARN with the specified portfolio.
      operationId: associatePrincipalWithPortfolio
      x-api-path-slug: actionassociateprincipalwithportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: PrincipalARN
        description: The ARN representing the principal (IAM user, role, or group)
        type: string
      - in: query
        name: PrincipalType
        description: The principal type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=AssociateProductWithPortfolio:
    get:
      summary: Associate Product With Portfolio
      description: Associates a product with a portfolio.
      operationId: associateProductWithPortfolio
      x-api-path-slug: actionassociateproductwithportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      - in: query
        name: SourcePortfolioId
        description: The identifier of the source portfolio to use with this association
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=CreateConstraint:
    get:
      summary: Create Constraint
      description: Creates a new constraint.
      operationId: createConstraint
      x-api-path-slug: actioncreateconstraint-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Description
        description: The text description of the constraint
        type: string
      - in: query
        name: IdempotencyToken
        description: A token to disambiguate duplicate requests
        type: string
      - in: query
        name: Parameters
        description: The constraint parameters
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      - in: query
        name: Type
        description: The type of the constraint
        type: string
      responses:
        200:
          description: OK
      tags:
      - Constraints
  /?Action=CreatePortfolio:
    get:
      summary: Create Portfolio
      description: Creates a new portfolio.
      operationId: createPortfolio
      x-api-path-slug: actioncreateportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Description
        description: The text description of the portfolio
        type: string
      - in: query
        name: DisplayName
        description: The name to use for display purposes
        type: string
      - in: query
        name: IdempotencyToken
        description: A token to disambiguate duplicate requests
        type: string
      - in: query
        name: ProviderName
        description: The name of the portfolio provider
        type: string
      - in: query
        name: Tags
        description: Tags to associate with the new portfolio
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=CreatePortfolioShare:
    get:
      summary: Create Portfolio Share
      description: Creates a new portfolio share.
      operationId: createPortfolioShare
      x-api-path-slug: actioncreateportfolioshare-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: AccountId
        description: The account ID with which to share the portfolio
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=CreateProduct:
    get:
      summary: Create Product
      description: Creates a new product.
      operationId: createProduct
      x-api-path-slug: actioncreateproduct-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Description
        description: The text description of the product
        type: string
      - in: query
        name: Distributor
        description: The distributor of the product
        type: string
      - in: query
        name: IdempotencyToken
        description: A token to disambiguate duplicate requests
        type: string
      - in: query
        name: Name
        description: The name of the product
        type: string
      - in: query
        name: Owner
        description: The owner of the product
        type: string
      - in: query
        name: ProductType
        description: The type of the product to create
        type: string
      - in: query
        name: ProvisioningArtifactParameters
        description: Parameters for the provisioning artifact
        type: string
      - in: query
        name: SupportDescription
        description: Support information about the product
        type: string
      - in: query
        name: SupportEmail
        description: Contact email for product support
        type: string
      - in: query
        name: SupportUrl
        description: Contact URL for product support
        type: string
      - in: query
        name: Tags
        description: Tags to associate with the new product
        type: string
      responses:
        200:
          description: OK
      tags:
      - Products
  /?Action=CreateProvisioningArtifact:
    get:
      summary: Create Provisioning Artifact
      description: Create a new provisioning artifact for the specified product.
      operationId: createProvisioningArtifact
      x-api-path-slug: actioncreateprovisioningartifact-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: IdempotencyToken
        description: A token to disambiguate duplicate requests
        type: string
      - in: query
        name: Parameters
        description: The parameters to use when creating the new provisioning artifact
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Provisioning Artifacts
  /?Action=DeleteConstraint:
    get:
      summary: Delete Constraint
      description: Deletes the specified constraint.
      operationId: deleteConstraint
      x-api-path-slug: actiondeleteconstraint-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Id
        description: The identifier of the constraint to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Constraints
  /?Action=DeletePortfolio:
    get:
      summary: Delete Portfolio
      description: Deletes the specified portfolio.
      operationId: deletePortfolio
      x-api-path-slug: actiondeleteportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Id
        description: The identifier of the portfolio for the delete request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=DeletePortfolioShare:
    get:
      summary: Delete Portfolio Share
      description: Deletes the specified portfolio share.
      operationId: deletePortfolioShare
      x-api-path-slug: actiondeleteportfolioshare-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: AccountId
        description: The account ID associated with the share to delete
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=DeleteProduct:
    get:
      summary: Delete Product
      description: Deletes the specified product.
      operationId: deleteProduct
      x-api-path-slug: actiondeleteproduct-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Id
        description: The identifier of the product for the delete request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Products
  /?Action=DeleteProvisioningArtifact:
    get:
      summary: Delete Provisioning Artifact
      description: Deletes the specified provisioning artifact.
      operationId: deleteProvisioningArtifact
      x-api-path-slug: actiondeleteprovisioningartifact-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      - in: query
        name: ProvisioningArtifactId
        description: The identifier of the provisioning artifact for the delete request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Provisioning Artifacts
  /?Action=DescribeConstraint:
    get:
      summary: Describe Constraint
      description: Retrieves detailed information for a specified constraint.
      operationId: describeConstraint
      x-api-path-slug: actiondescribeconstraint-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Id
        description: The identifier of the constraint
        type: string
      responses:
        200:
          description: OK
      tags:
      - Constraints
  /?Action=DescribePortfolio:
    get:
      summary: Describe Portfolio
      description: |-
        Retrieves detailed information and any tags associated with the specified
                 portfolio.
      operationId: describePortfolio
      x-api-path-slug: actiondescribeportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Id
        description: The identifier of the portfolio for which to retrieve information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=DescribeProduct:
    get:
      summary: Describe Product
      description: Retrieves information about a specified product.
      operationId: describeProduct
      x-api-path-slug: actiondescribeproduct-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Id
        description: The ProductId of the product to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Products
  /?Action=DescribeProductAsAdmin:
    get:
      summary: Describe Product As Admin
      description: |-
        Retrieves information about a specified product, run with administrator
                 access.
      operationId: describeProductAsAdmin
      x-api-path-slug: actiondescribeproductasadmin-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Id
        description: The identifier of the product for which to retrieve information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Products
  /?Action=DescribeProductView:
    get:
      summary: Describe Product View
      description: Retrieves information about a specified product.
      operationId: describeProductView
      x-api-path-slug: actiondescribeproductview-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Id
        description: The ProductViewId of the product to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Products
  /?Action=DescribeProvisioningArtifact:
    get:
      summary: Describe Provisioning Artifact
      description: Retrieves detailed information about the specified provisioning
        artifact.
      operationId: describeProvisioningArtifact
      x-api-path-slug: actiondescribeprovisioningartifact-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      - in: query
        name: ProvisioningArtifactId
        description: The identifier of the provisioning artifact
        type: string
      responses:
        200:
          description: OK
      tags:
      - Provisioning Artifacts
  /?Action=DescribeProvisioningParameters:
    get:
      summary: Describe Provisioning Parameters
      description: |-
        Provides information about parameters required to provision a specified product in a
                 specified manner.
      operationId: describeProvisioningParameters
      x-api-path-slug: actiondescribeprovisioningparameters-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PathId
        description: The identifier of the path for this products provisioning
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      - in: query
        name: ProvisioningArtifactId
        description: The provisioning artifact identifier for this product
        type: string
      responses:
        200:
          description: OK
      tags:
      - Provisioning Parameters
  /?Action=DescribeRecord:
    get:
      summary: Describe Record
      description: Retrieves a paginated list of the full details of a specific request.
      operationId: describeRecord
      x-api-path-slug: actiondescriberecord-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Id
        description: The record identifier of the ProvisionedProduct object for which
          to retrieve output         information
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Records
  /?Action=DisassociatePrincipalFromPortfolio:
    get:
      summary: Disassociate Principal From Portfolio
      description: |-
        Disassociates a previously associated principal ARN from a specified
                 portfolio.
      operationId: disassociatePrincipalFromPortfolio
      x-api-path-slug: actiondisassociateprincipalfromportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: PrincipalARN
        description: The ARN representing the principal (IAM user, role, or group)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=DisassociateProductFromPortfolio:
    get:
      summary: Disassociate Product From Portfolio
      description: Disassociates the specified product from the specified portfolio.
      operationId: disassociateProductFromPortfolio
      x-api-path-slug: actiondisassociateproductfromportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=ListAcceptedPortfolioShares:
    get:
      summary: List Accepted Portfolio Shares
      description: |-
        Lists details of all portfolios for which sharing was accepted by this
                 account.
      operationId: listAcceptedPortfolioShares
      x-api-path-slug: actionlistacceptedportfolioshares-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=ListConstraintsForPortfolio:
    get:
      summary: List Constraints For Portfolio
      description: |-
        Retrieves detailed constraint information for the specified portfolio and
                 product.
      operationId: listConstraintsForPortfolio
      x-api-path-slug: actionlistconstraintsforportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=ListLaunchPaths:
    get:
      summary: List Launch Paths
      description: Returns a paginated list of all paths to a specified product.
      operationId: listLaunchPaths
      x-api-path-slug: actionlistlaunchpaths-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Launch Paths
  /?Action=ListPortfolioAccess:
    get:
      summary: List Portfolio Access
      description: |-
        Lists the account IDs that have been authorized sharing of the specified
                 portfolio.
      operationId: listPortfolioAccess
      x-api-path-slug: actionlistportfolioaccess-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=ListPortfolios:
    get:
      summary: List Portfolios
      description: Lists all portfolios in the catalog.
      operationId: listPortfolios
      x-api-path-slug: actionlistportfolios-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=ListPortfoliosForProduct:
    get:
      summary: List Portfolios For Product
      description: Lists all portfolios that the specified product is associated with.
      operationId: listPortfoliosForProduct
      x-api-path-slug: actionlistportfoliosforproduct-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=ListPrincipalsForPortfolio:
    get:
      summary: List Principals For Portfolio
      description: Lists all principal ARNs associated with the specified portfolio.
      operationId: listPrincipalsForPortfolio
      x-api-path-slug: actionlistprincipalsforportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=ListProvisioningArtifacts:
    get:
      summary: List Provisioning Artifacts
      description: Lists all provisioning artifacts associated with the specified
        product.
      operationId: listProvisioningArtifacts
      x-api-path-slug: actionlistprovisioningartifacts-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Provisioning Artifacts
  /?Action=ListRecordHistory:
    get:
      summary: List Record History
      description: |-
        Returns a paginated list of all performed requests, in the form of RecordDetails
                 objects that are filtered as specified.
      operationId: listRecordHistory
      x-api-path-slug: actionlistrecordhistory-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: AccessLevelFilter
        description: The access level for obtaining results
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      - in: query
        name: SearchFilter
        description: The filter to limit search results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Record History
  /?Action=ProvisionProduct:
    get:
      summary: Provision Product
      description: Requests a Provision of a specified product.
      operationId: provisionProduct
      x-api-path-slug: actionprovisionproduct-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: NotificationArns
        description: Passed to CloudFormation
        type: string
      - in: query
        name: PathId
        description: The identifier of the path for this products provisioning
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      - in: query
        name: ProvisionedProductName
        description: A user-friendly name to identify the ProvisionedProduct object
        type: string
      - in: query
        name: ProvisioningArtifactId
        description: The provisioning artifact identifier for this product
        type: string
      - in: query
        name: ProvisioningParameters
        description: Parameters specified by the administrator that are required for
          provisioning the         product
        type: string
      - in: query
        name: ProvisionToken
        description: An idempotency token that uniquely identifies the provisioning
          request
        type: string
      - in: query
        name: Tags
        description: A list of tags to use as provisioning options
        type: string
      responses:
        200:
          description: OK
      tags:
      - Products
  /?Action=RejectPortfolioShare:
    get:
      summary: Reject Portfolio Share
      description: Rejects an offer to share a portfolio.
      operationId: rejectPortfolioShare
      x-api-path-slug: actionrejectportfolioshare-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=ScanProvisionedProducts:
    get:
      summary: Scan Provisioned Products
      description: |-
        Returns a paginated list of all the ProvisionedProduct objects that are currently
                 available (not terminated).
      operationId: scanProvisionedProducts
      x-api-path-slug: actionscanprovisionedproducts-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: AccessLevelFilter
        description: The access level for obtaining results
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Provisioned Products
  /?Action=SearchProducts:
    get:
      summary: Search Products
      description: |-
        Returns a paginated list all of the Products objects to which the caller
                 has access.
      operationId: searchProducts
      x-api-path-slug: actionsearchproducts-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Filters
        description: The list of filters with which to limit search results
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      - in: query
        name: SortBy
        description: The sort field specifier
        type: string
      - in: query
        name: SortOrder
        description: The sort order specifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Products
  /?Action=SearchProductsAsAdmin:
    get:
      summary: Search Products As Admin
      description: |-
        Retrieves summary and status information about all products created within the
                 caller's account.
      operationId: searchProductsAsAdmin
      x-api-path-slug: actionsearchproductsasadmin-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Filters
        description: The list of filters with which to limit search results
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: ProductSource
        description: Access level of the source of the product
        type: string
      - in: query
        name: SortBy
        description: The sort field specifier
        type: string
      - in: query
        name: SortOrder
        description: The sort order specifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Products
  /?Action=TerminateProvisionedProduct:
    get:
      summary: Terminate Provisioned Product
      description: Requests termination of an existing ProvisionedProduct object.
      operationId: terminateProvisionedProduct
      x-api-path-slug: actionterminateprovisionedproduct-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: IgnoreErrors
        description: If set to true, AWS Service Catalog stops managing the specified
          ProvisionedProduct object even         if it cannot delete the underlying
          resources
        type: string
      - in: query
        name: ProvisionedProductId
        description: The identifier of the ProvisionedProduct object to terminate
        type: string
      - in: query
        name: ProvisionedProductName
        description: The name of the ProvisionedProduct object to terminate
        type: string
      - in: query
        name: TerminateToken
        description: An idempotency token that uniquely identifies the termination
          request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Provisioned Products
  /?Action=UpdateConstraint:
    get:
      summary: Update Constraint
      description: Updates an existing constraint.
      operationId: updateConstraint
      x-api-path-slug: actionupdateconstraint-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Description
        description: The updated text description of the constraint
        type: string
      - in: query
        name: Id
        description: The identifier of the constraint to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Constraints
  /?Action=UpdatePortfolio:
    get:
      summary: Update Portfolio
      description: Updates the specified portfolio's details.
      operationId: updatePortfolio
      x-api-path-slug: actionupdateportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: AddTags
        description: Tags to add to the existing list of tags associated with the
          portfolio
        type: string
      - in: query
        name: Description
        description: The updated text description of the portfolio
        type: string
      - in: query
        name: DisplayName
        description: The name to use for display purposes
        type: string
      - in: query
        name: Id
        description: The identifier of the portfolio for the update request
        type: string
      - in: query
        name: ProviderName
        description: The updated name of the portfolio provider
        type: string
      - in: query
        name: RemoveTags
        description: Tags to remove from the existing list of tags associated with
          the         portfolio
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=UpdateProduct:
    get:
      summary: Update Product
      description: Updates an existing product.
      operationId: updateProduct
      x-api-path-slug: actionupdateproduct-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: AddTags
        description: Tags to add to the existing list of tags associated with the
          product
        type: string
      - in: query
        name: Description
        description: The updated text description of the product
        type: string
      - in: query
        name: Distributor
        description: The updated distributor of the product
        type: string
      - in: query
        name: Id
        description: The identifier of the product for the update request
        type: string
      - in: query
        name: Name
        description: The updated product name
        type: string
      - in: query
        name: Owner
        description: The updated owner of the product
        type: string
      - in: query
        name: RemoveTags
        description: Tags to remove from the existing list of tags associated with
          the product
        type: string
      - in: query
        name: SupportDescription
        description: The updated support description for the product
        type: string
      - in: query
        name: SupportEmail
        description: The updated support email for the product
        type: string
      - in: query
        name: SupportUrl
        description: The updated support URL for the product
        type: string
      responses:
        200:
          description: OK
      tags:
      - Products
  /?Action=UpdateProvisionedProduct:
    get:
      summary: Update Provisioned Product
      description: Requests updates to the configuration of an existing ProvisionedProduct
        object.
      operationId: updateProvisionedProduct
      x-api-path-slug: actionupdateprovisionedproduct-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PathId
        description: The identifier of the path to use in the updated ProvisionedProduct
          object
        type: string
      - in: query
        name: ProductId
        description: The identifier of the ProvisionedProduct object
        type: string
      - in: query
        name: ProvisionedProductId
        description: The identifier of the ProvisionedProduct object to update
        type: string
      - in: query
        name: ProvisionedProductName
        description: 'The updated name of the ProvisionedProduct object '
        type: string
      - in: query
        name: ProvisioningArtifactId
        description: The provisioning artifact identifier for this product
        type: string
      - in: query
        name: ProvisioningParameters
        description: A list of ProvisioningParameter objects used to update the         ProvisionedProduct
          object
        type: string
      - in: query
        name: UpdateToken
        description: The idempotency token that uniquely identifies the provisioning
          update         request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Provisioned Products
  /?Action=UpdateProvisioningArtifact:
    get:
      summary: Update Provisioning Artifact
      description: Updates an existing provisioning artifact's information.
      operationId: updateProvisioningArtifact
      x-api-path-slug: actionupdateprovisioningartifact-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Description
        description: The updated text description of the provisioning artifact
        type: string
      - in: query
        name: Name
        description: The updated name of the provisioning artifact
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      - in: query
        name: ProvisioningArtifactId
        description: The identifier of the provisioning artifact for the update request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Provisioning Artifacts