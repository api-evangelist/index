swagger: "2.0"
x-collection-name: Docsmore
x-complete: 1
info:
  title: Docsmore API 2.1
  description: alt-texthttpswww-docsmore-comwpcontentuploads201802docsmoreapi-png-titleh3create-a-developer-account-at-docsmore-io-and-start-unleashing-the-power-of-docsmore-into-your-own-applications--to-make-it-easier-we-have-provided-client-libraries-and-sdk-in-several-languages-for-you-to-get-started-and-hit-the-ground-running-in-no-time-h3brbrh4note-if-you-dont-see-api-setting-under-top-right-menu-that-means-you-will-need-to-be-a-developer-account--please-contact-supportdocsmore-com-and-a-customer-service-expert-will-switch-your-account-to-developer-account--h4brbrh5just-head-over-to-httpsdocsmore-io-and-sign-up-for-your-30-days-trial-h5
  version: "1.0"
host: api.docsmore.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/getwebhooks:
    get:
      summary: List all Webhooks
      description: List Webhooks that are both active and inactive. Inactive webhooks
        with webhook type of 'static' will be automatically removed during the nightly
        job process.
      operationId: ApiGetwebhooksGet
      x-api-path-slug: apigetwebhooks-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Webhooks
  /api/getwebhooks/{id}:
    get:
      summary: Get Details of Single Webhook
      description: Details of Single Webhook.
      operationId: ApiGetwebhooksByIdGet
      x-api-path-slug: apigetwebhooksid-get
      parameters:
      - in: header
        name: Content-Type
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Details
      - Of
      - Single
      - Webhook
  /api/webhook/subscribe:
    post:
      summary: Subscribe To Webhook
      description: |-
        Make sure you have a unique payload URL every time you use this api call to register your webhook. Unable to do so will result in webhook registration denial.


        For multiple events subscription, just use it comma separated values. Here are the available list of register events.



        documentUploadComplete
        workflowProgressEvent
        workflowCompleteEvent
        documentflowProgressEvent
        documentflowCompleteEvent
        documentSelfSigninCompleteEvent
      operationId: ApiWebhookSubscribePost
      x-api-path-slug: apiwebhooksubscribe-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Subscribe
      - Webhook
  /api/webhook/unsubscribe/{id}:
    delete:
      summary: Unsubscribe Webhook
      description: It is important that you call this event to unsubscribe otherwise
        it will automatically be removed in 10 minutes. If not unsubscribed manually,
        it can also lead to the problem of duplication and create further issues.
      operationId: ApiWebhookUnsubscribeByIdDelete
      x-api-path-slug: apiwebhookunsubscribeid-delete
      parameters:
      - in: header
        name: Content-Type
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Unsubscribe
      - Webhook
  /oauth/token:
    post:
      summary: Get OAuth TOKEN
      description: |-
        Obtaining an Auth Token is the first thing in the process. The lifetime of Auth token is configurable in the developer portal depending upon your need. Once auth token is obtained, all the follow up API calls will need to include auth token in the header. FaIlure to do so would result in response with 401 Unauthorized Access.

        Under Your Developer Account - Go to Api Setting and you will screen similar to below.


        Make sure you call this in server side code. Exposing apiKey and clientSecret is a not a good idea on front end and can lead up to security vulnerabilities.
      operationId: OauthTokenPost
      x-api-path-slug: oauthtoken-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - OAuth
      - TOKEN
  /api/dmcatalogue:
    post:
      summary: Fetch All Documents from Your Team Catalogue
      description: By design, the authenticated user can only view the files that
        are either created by them or shared with them. Make sure user has at least
        read permission to view the catalogue.
      operationId: ApiDmcataloguePost
      x-api-path-slug: apidmcatalogue-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: items
      - in: query
        name: page
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - ""
      - Documents
      - From
      - Your
      - Team
      - Catalogue
  /api/dmcatalogue/:id:
    post:
      summary: Fetch Single Document
      description: Fetch single document.
      operationId: ApiDmcatalogueIdPost
      x-api-path-slug: apidmcatalogueid-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: id
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Single
      - Document
  /api/docflow/getdocflows:
    get:
      summary: Get All Document Flows
      description: Get all document flows.
      operationId: ApiDocflowGetdocflowsGet
      x-api-path-slug: apidocflowgetdocflows-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Document
      - Flows
  /api/clientdocs/getrawdata/:authToken/:documentKey:
    get:
      summary: Get Raw Data For A Given Document
      description: |-
        This API call gets you underlying raw data of the document. All you need to do is supply Auth token and Document Key as part of the call.

        Document Key can be obtained from "Document Gallery" Page and Clicking on the sub-menu of the desired document.

        As a response object, jsondata and metadata information is passed. Jsondata is basically raw data and metadata is data columns information.
      operationId: ApiClientdocsGetrawdataAuthTokenDocumentKeyGet
      x-api-path-slug: apiclientdocsgetrawdataauthtokendocumentkey-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: authToken
      - in: header
        name: Content-Type
      - in: query
        name: documentKey
      responses:
        200:
          description: OK
      tags:
      - Raw
      - Data
      - Given
      - Document
  /api/getworkflowlink:
    post:
      summary: Get Workflow Link
      description: |-
        This is the most popular use of Docsmore API. From your connected app, you can launch workflow and obtain the unique link for immediate launch or later on. You can also supply data in flat json format that can be used inside the document for pre-fill purpose saving your customer time.

        Please make sure you pay close attention to the requirement for this API call as there are several aspects of it as required parameters.
      operationId: ApiGetworkflowlinkPost
      x-api-path-slug: apigetworkflowlink-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Link
  /api/docflowtracks/flowtrackviaapi:
    post:
      summary: Get Workflow Link For Flow Track
      description: |-
        In Docsmore space, Flow Track means all the client documents generated using one of the Document Flow. In other words, it is an instance of Document FLow. The other thing to notice here is payload information is remarkably similar to general "Workflow" of a Single Document.

        When you initiate this API call, you are basically setting up a new instance of Workflow and in turn getting workflow link of the starting document in the workflow.

        If "flowtrackid" value is "new", then new flowtrack will be created. If flowtrackid has a value of actual flowtrackid then link will be provided to access read-only view of document flowtrack
      operationId: ApiDocflowtracksFlowtrackviaapiPost
      x-api-path-slug: apidocflowtracksflowtrackviaapi-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Link
      - Flow
      - Track
  /rawdata:
    post:
      summary: Returns raw data response as json FOR SINGLE CLIENT DOC
      description: This API call gets you underlying raw data of the document. All
        you need to do is supply Auth token and Document Key as part of the call
      operationId: RawdataPost
      x-api-path-slug: rawdata-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Raw
      - Data
      - Response
      - As
      - Json
      - FOR
      - SINGLE
      - CLIENT
      - DOC
  /getclientdocs:
    post:
      summary: Get List of Client Documents By Document ID
      description: In order to export as PDf, you will need to have client document
        ID available for that specific document you are looking to download.
      operationId: GetclientdocsPost
      x-api-path-slug: getclientdocs-post
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Client
      - Documents
      - Document
      - ID
  /clientdocs/exportpdf/{id}:
    get:
      summary: Export As PDF
      description: In order to export as PDf, you will need to have client document
        ID available for that specific document you are looking to download.
      operationId: ClientdocsExportpdfByIdGet
      x-api-path-slug: clientdocsexportpdfid-get
      parameters:
      - in: header
        name: Content-Type
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Export
      - As
      - PDF