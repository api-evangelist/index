swagger: "2.0"
x-collection-name: Sustainable Facilities Tool API
x-complete: 1
info:
  title: Sustainable Facilities Tool API
  description: our-core-api-allows-developers-to-interact-with-the-sustainable-facilities-tool-programmatically--its-designed-for-public-use-and-to-be-easily-integrated-into-other-applications-
  termsOfService: https://sftool.gov/developer/terms-of-use
  version: 1.0.0
host: api.data.gov
basePath: /sftool/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /building-systems:
    get:
      summary: Returns all building systems.
      description: Returns all building systems.
      operationId: returnBuildingSystems
      x-api-path-slug: buildingsystems-get
      responses:
        200:
          description: OK
      tags:
      - Building Systems
  /building-systems/{parameter}:
    get:
      summary: Returns a building system by parameter.
      description: Returns a building system by parameter.
      operationId: returnBuildingSystem
      x-api-path-slug: buildingsystemsparameter-get
      responses:
        200:
          description: OK
      tags:
      - Building Systems
  /building-systems/{parameter}/resources:
    get:
      summary: Returns Building System Resources
      description: Returns informational resources for the building system selected
        by parameter.
      operationId: returnBuildingSystemResources
      x-api-path-slug: buildingsystemsparameterresources-get
      responses:
        200:
          description: OK
      tags:
      - Building System Resources
  /building-systems/case-studies:
    get:
      summary: Building System Case Studies
      description: Returns all building systems case studies
      operationId: returnBuildingSystemCaseStudies
      x-api-path-slug: buildingsystemscasestudies-get
      responses:
        200:
          description: OK
      tags:
      - Case Studies
  /building-systems/{parameter}/case-studies:
    get:
      summary: Building System Case Study
      description: Returns a building system case study by parameter.
      operationId: returnBuildingSystemCaseStudies
      x-api-path-slug: buildingsystemsparametercasestudies-get
      responses:
        200:
          description: OK
      tags:
      - Case Studies
  /building-systems/mandates:
    get:
      summary: Building System Mandates
      description: Returns all building systems mandates
      operationId: returnBuildingSystemMandates
      x-api-path-slug: buildingsystemsmandates-get
      responses:
        200:
          description: OK
      tags:
      - Mandates
  /building-systems/{parameter}/mandates:
    get:
      summary: Building System Mandate
      description: Returns a building system mandate by parameter.
      operationId: returnBuildingSystemMandate
      x-api-path-slug: buildingsystemsparametermandates-get
      responses:
        200:
          description: OK
      tags:
      - Mandates
  /building-systems/rating-systems:
    get:
      summary: Building System Rating Systems
      description: Returns all building system rating systems
      operationId: returnBuildingSystemRating
      x-api-path-slug: buildingsystemsratingsystems-get
      responses:
        200:
          description: OK
      tags:
      - Rating Systems
  /building-systems/{parameter}/rating-systems:
    get:
      summary: Building System Rating System
      description: Returns a building system rating system by parameter.
      operationId: returnBuildingSystemRating
      x-api-path-slug: buildingsystemsparameterratingsystems-get
      responses:
        200:
          description: OK
      tags:
      - Rating Systems
  /building-systems/system-bundles:
    get:
      summary: Building System Bundles
      description: Returns all building system bundles.
      operationId: returnsBuildingSystemBundles
      x-api-path-slug: buildingsystemssystembundles-get
      responses:
        200:
          description: OK
      tags:
      - Bundles
  /building-systems/{parameter}/system-bundles:
    get:
      summary: Building System Bundle
      description: Returns a building system bundle by parameter.
      operationId: returnsBuildingSystemBundle
      x-api-path-slug: buildingsystemsparametersystembundles-get
      responses:
        200:
          description: OK
      tags:
      - Bundles
  /building-systems/integrative-teams:
    get:
      summary: Building System Integrative Teams
      description: Returns all building system integrative teams.
      operationId: returnBuildingSystemIntegrativeTeams
      x-api-path-slug: buildingsystemsintegrativeteams-get
      responses:
        200:
          description: OK
      tags:
      - Teams
  /building-systems/{parameter}/integrative-teams:
    get:
      summary: Building System Integrative Team
      description: Returns a building system integrative team by parameter.
      operationId: returnBuildingSystemIntegrativeTeams
      x-api-path-slug: buildingsystemsparameterintegrativeteams-get
      responses:
        200:
          description: OK
      tags:
      - Teams
  /contentpages:
    get:
      summary: Content Pages
      description: Returns all content pages
      operationId: returnContentPages
      x-api-path-slug: contentpages-get
      responses:
        200:
          description: OK
      tags:
      - Content
  /contentpages/{parameter}:
    get:
      summary: Content Page
      description: Returns a content page by parameter.
      operationId: returnContentPage
      x-api-path-slug: contentpagesparameter-get
      responses:
        200:
          description: OK
      tags:
      - Content
  /procurementclauses:
    get:
      summary: Federal Acquisition Regulation (FAR) Clause
      description: Returns Federal Acquisition Regulation (FAR) clause numbers and
        environmental programs for all NAICS and PSC codes with federal sustainable
        procurement requirements in GPC.
      operationId: returnFederalAcquisitionRegulationClause
      x-api-path-slug: procurementclauses-get
      responses:
        200:
          description: OK
      tags:
      - Regulation Clause
  /procurementclauses/naics/{parameter}:
    get:
      summary: Federal Acquisition Regulation (FAR) Clause
      description: Returns any FAR clause number(s) and sample procurement language
        associated with the given NAICS parameter.
      operationId: returnFederalAcquisitionRegulationClause
      x-api-path-slug: procurementclausesnaicsparameter-get
      responses:
        200:
          description: OK
      tags:
      - Regulation Clause
  /procurementclauses/psc/{parameter}:
    get:
      summary: Procurement Clause
      description: Returns any FAR clause number(s) and sample procurement language
        associated with the given PSC parameter.
      operationId: returnFederalAcquisitionRegulationClause
      x-api-path-slug: procurementclausespscparameter-get
      responses:
        200:
          description: OK
      tags:
      - Procurement Clause
  /procurementclauses/allcontractlanguage:
    get:
      summary: Contract Language
      description: Returns all sample contract language for environmental programs
      operationId: contractLanguage
      x-api-path-slug: procurementclausesallcontractlanguage-get
      responses:
        200:
          description: OK
      tags:
      - Contract Language
  /materials:
    get:
      summary: Return Materials
      description: Returns all materials.
      operationId: returnMaterials
      x-api-path-slug: materials-get
      responses:
        200:
          description: OK
      tags:
      - Materials
  /materials/{parameter}:
    get:
      summary: Return Material
      description: Returns a material by parameter.
      operationId: returnMaterial
      x-api-path-slug: materialsparameter-get
      responses:
        200:
          description: OK
      tags:
      - Materials
  /materials/{parameter}/alternatives:
    get:
      summary: Alternative Materials
      description: Returns alternatives for the material selected by parameter.
      operationId: getAlternativeMaterials
      x-api-path-slug: materialsparameteralternatives-get
      responses:
        200:
          description: OK
      tags:
      - Alternative Materials
  /materials/{parameter}/comparisons:
    get:
      summary: Compairson Materials
      description: Returns comparisons for the material selected by parameter.
      operationId: returnCompairsonMaterials
      x-api-path-slug: materialsparametercomparisons-get
      responses:
        200:
          description: OK
      tags:
      - Comparison Materials
  /products:
    get:
      summary: Products
      description: Returns all products.
      operationId: getProducts
      x-api-path-slug: products-get
      responses:
        200:
          description: OK
      tags:
      - Products
  /products/{parameter}/details:
    get:
      summary: Product Details
      description: Returns details for the product selected by parameter.
      operationId: getProductDetails
      x-api-path-slug: productsparameterdetails-get
      responses:
        200:
          description: OK
      tags:
      - Products
  /services:
    get:
      summary: Services
      description: Returns all services
      operationId: getServices
      x-api-path-slug: services-get
      responses:
        200:
          description: OK
      tags:
      - Services
  /services/{parameter}:
    get:
      summary: Services
      description: Returns a service by parameter.
      operationId: getService
      x-api-path-slug: servicesparameter-get
      responses:
        200:
          description: OK
      tags:
      - Services
  /services/{parameter}/related-products:
    get:
      summary: Related Products
      description: Returns products related to a service by parameter.
      operationId: getRelatedProducts
      x-api-path-slug: servicesparameterrelatedproducts-get
      responses:
        200:
          description: OK
      tags:
      - Products
  /tags:
    get:
      summary: Tags
      description: Returns all search tags.
      operationId: getTags
      x-api-path-slug: tags-get
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/{parameter}:
    get:
      summary: Tag
      description: Returns a tag by parameter.
      operationId: getTag
      x-api-path-slug: tagsparameter-get
      responses:
        200:
          description: OK
      tags:
      - Tags
  /workspaces:
    get:
      summary: Workspaces
      description: Returns all workspaces.
      operationId: getWorkspaces
      x-api-path-slug: workspaces-get
      responses:
        200:
          description: OK
      tags:
      - Workspaces
  /workspaces/{parameter}:
    get:
      summary: Workspace
      description: Returns a workspace by parameter.
      operationId: getWorkspace
      x-api-path-slug: workspacesparameter-get
      responses:
        200:
          description: OK
      tags:
      - Workspaces
  /workspaces/{parameter}/material-groups:
    get:
      summary: Workspaces
      description: Returns material groups for the workspace selected by parameter.
      operationId: getWorkspaceMaterialGroups
      x-api-path-slug: workspacesparametermaterialgroups-get
      responses:
        200:
          description: OK
      tags:
      - Workspaces
  /workspaces/{parameter}/materials:
    get:
      summary: Workspace Materials
      description: Returns materials for the workspace selected by parameter.
      operationId: getWorkspaceMaterials
      x-api-path-slug: workspacesparametermaterials-get
      responses:
        200:
          description: OK
      tags:
      - Workspaces