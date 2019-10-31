swagger: "2.0"
x-collection-name: MotaWord
x-complete: 1
info:
  title: Mota Word
  description: use-motaword-api-to-post-and-track-your-translation-projects-
  version: alpha-0.1.0
host: api.motaword.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    get:
      summary: Available endpoints
      description: The root endpoint will provide you a JSON Swagger definition.
      operationId: getEndpoints
      x-api-path-slug: get
      responses:
        200:
          description: OK
      tags:
      - ""
  /formats:
    get:
      summary: Get a list of supported formats
      description: Get a list of supported formats for documents, style guides and
        extensions.
      operationId: getFormats
      x-api-path-slug: formats-get
      responses:
        200:
          description: OK
      tags:
      - Formats
  /glossary:
    get:
      summary: Download the global glossary.
      description: Download your corporate account's global glossary. This endpoint
        is available only for corporate account customers.
      operationId: downloadGlobalGlossary
      x-api-path-slug: glossary-get
      responses:
        200:
          description: OK
      tags:
      - Glossary
    post:
      summary: Create or update the global glossary.
      description: Update your corporate account's global glossary. This endpoint
        is available only for corporate account customers.
      operationId: updateGlobalGlossary
      x-api-path-slug: glossary-post
      parameters:
      - in: formData
        name: glossary
        description: Glossary file
      responses:
        200:
          description: OK
      tags:
      - Glossary
  /languages:
    get:
      summary: Get a list of supported languages
      description: Get a list of supported languages.
      operationId: getLanguages
      x-api-path-slug: languages-get
      responses:
        200:
          description: OK
      tags:
      - Languages
  /me:
    get:
      summary: Get your account information and summary.
      description: Get your account information and summary..
      operationId: getAccount
      x-api-path-slug: me-get
      responses:
        200:
          description: OK
      tags:
      - Me
  /projects:
    get:
      summary: Get a list of your projects
      description: Get a list of your projects.
      operationId: getProjects
      x-api-path-slug: projects-get
      parameters:
      - in: query
        name: page
      - in: query
        name: per_page
      responses:
        200:
          description: OK
      tags:
      - Projects
    post:
      summary: Get a new quote
      description: Create a new project
      operationId: createProject
      x-api-path-slug: projects-post
      parameters:
      - in: formData
        name: callback_url
        description: Optional
      - in: formData
        name: custom
        description: Optional
      - in: formData
        name: documents[]
        description: Optional
      - in: formData
        name: glossaries[]
        description: Optional
      - in: formData
        name: source_language
      - in: formData
        name: styleguides[]
        description: Optional
      - in: formData
        name: target_languages[]
      responses:
        200:
          description: OK
      tags:
      - Projects
  /projects/{id}:
    delete:
      summary: Delete a project
      description: Delete(cancel) a project.
      operationId: deleteProject
      x-api-path-slug: projectsid-delete
      parameters:
      - in: path
        name: id
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
    get:
      summary: Get single project
      description: Get single project.
      operationId: getProject
      x-api-path-slug: projectsid-get
      parameters:
      - in: path
        name: id
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
    put:
      summary: Update project language pairs
      description: Update project language pairs.
      operationId: updateProject
      x-api-path-slug: projectsid-put
      parameters:
      - in: formData
        name: callback_url
        description: Optional
      - in: formData
        name: custom
        description: Optional
      - in: path
        name: id
        description: Project ID
      - in: formData
        name: source_language
      - in: formData
        name: target_languages[]
      responses:
        200:
          description: OK
      tags:
      - Projects
  /projects/{id}/callback/{actionType}:
    get:
      summary: Trigger a call to your callback URL related to this project.
      description: Trigger a call to your callback url related to this project..
      operationId: triggerCallback
      x-api-path-slug: projectsidcallbackactiontype-get
      parameters:
      - in: path
        name: actionType
        description: Callback type
      - in: path
        name: id
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Callback
      - ActionType
  /projects/{id}/cancel:
    post:
      summary: Cancel your translation project
      description: Cancel your translation project.
      operationId: cancelProject
      x-api-path-slug: projectsidcancel-post
      parameters:
      - in: path
        name: id
        description: Project ID
      - in: formData
        name: reason
        description: Cancellation reason
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Cancel
  /projects/{id}/download:
    post:
      summary: Download the latest translation package.
      description: Download the latest translation package. You must have given a
        /package call beforehand and wait until the packaging status is 'completed'.
      operationId: download
      x-api-path-slug: projectsiddownload-post
      parameters:
      - in: path
        name: id
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Download
  /projects/{id}/download/{language}:
    post:
      summary: Download the latest translation package.
      description: Download only the translation package of this language. You must
        have given a /package call beforehand and wait until the packaging status
        is 'completed'.
      operationId: downloadLanguage
      x-api-path-slug: projectsiddownloadlanguage-post
      parameters:
      - in: path
        name: id
        description: Project ID
      - in: path
        name: language
        description: Language code
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Download
      - Language
  /projects/{id}/launch:
    post:
      summary: Launch your translation project
      description: Launch your translation project.
      operationId: launchProject
      x-api-path-slug: projectsidlaunch-post
      parameters:
      - in: formData
        name: budget_code
        description: Optional with corporate accounts
      - in: path
        name: id
        description: Project ID
      - in: formData
        name: payment_code
        description: Optional
      - in: formData
        name: payment_method
        description: Optional
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Launch
  /projects/{id}/package:
    post:
      summary: Package the translation of all languages to be downloaded.
      description: Package the translation project, make it ready to be downloaded.
      operationId: package
      x-api-path-slug: projectsidpackage-post
      parameters:
      - in: query
        name: async
        description: If you want to package and download the translation synchronously,
          mark this parameter as 0
      - in: path
        name: id
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Package
  /projects/{id}/package/check:
    get:
      summary: Track the status of translation packaging.
      description: This request will tell you the current progress of the translation
        packaging. You will use the 'key' provided by the /package call.
      operationId: trackPackage
      x-api-path-slug: projectsidpackagecheck-get
      parameters:
      - in: path
        name: id
        description: Project ID
      - in: query
        name: key
        description: This is the package tracking key provided in the response of
          a /package call
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Package
      - Check
  /projects/{id}/package/{language}:
    post:
      summary: Package the translation of a specific target language to be downloaded.
      description: Package the translation of a specific target language to be downloaded..
      operationId: packageLanguage
      x-api-path-slug: projectsidpackagelanguage-post
      parameters:
      - in: query
        name: async
        description: If you want to package and download the translation synchronously,
          mark this parameter as 0
      - in: path
        name: id
        description: Project ID
      - in: path
        name: language
        description: Language code
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Package
      - Language
  /projects/{id}/progress:
    get:
      summary: Get project progress
      description: Get the progress of an already launched project.
      operationId: getProgress
      x-api-path-slug: projectsidprogress-get
      parameters:
      - in: path
        name: id
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Progress
  /projects/{id}/reports:
    post:
      summary: Submit reports for a project
      description: Submit reports for a project.
      operationId: submitProjectReports
      x-api-path-slug: projectsidreports-post
      parameters:
      - in: formData
        name: activity_type
        description: Activity Type
      - in: path
        name: id
        description: Project ID
      - in: formData
        name: message
        description: Report Message
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Reports
  /projects/{projectId}/activities:
    get:
      summary: Get a list of realtime activities.
      description: Get a list of realtime activities on the project, such as translation
        suggestion and translation approval.
      operationId: getActivities
      x-api-path-slug: projectsprojectidactivities-get
      parameters:
      - in: query
        name: page
      - in: query
        name: per_page
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Activities
  /projects/{projectId}/activities/{activityId}:
    get:
      summary: Get a single realtime activity.
      description: Get a single realtime activity..
      operationId: getActivity
      x-api-path-slug: projectsprojectidactivitiesactivityid-get
      parameters:
      - in: path
        name: activityId
        description: Activity ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Activities
      - ActivityId
    post:
      summary: Submit a comment to an activity.
      description: Submit a comment to an activity..
      operationId: submitComment
      x-api-path-slug: projectsprojectidactivitiesactivityid-post
      parameters:
      - in: path
        name: activityId
        description: Activity ID
      - in: formData
        name: comment
        description: Comment text
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Activities
      - ActivityId
  /projects/{projectId}/activities/{activityId}/comments:
    get:
      summary: Get a list of comments belonging to this activity.
      description: Get a list of comments belonging to this activity..
      operationId: getActivityComments
      x-api-path-slug: projectsprojectidactivitiesactivityidcomments-get
      parameters:
      - in: path
        name: activityId
        description: Activity ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Activities
      - ActivityId
      - Comments
  /projects/{projectId}/comments:
    get:
      summary: Get a list of activity comments throughout the whole project.
      description: Get a list of activity comments throughout the whole project..
      operationId: getComments
      x-api-path-slug: projectsprojectidcomments-get
      parameters:
      - in: query
        name: page
      - in: query
        name: per_page
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Comments
  /projects/{projectId}/documents:
    get:
      summary: Get a list of documents
      description: Get a list of documents.
      operationId: getDocuments
      x-api-path-slug: projectsprojectiddocuments-get
      parameters:
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Documents
    post:
      summary: Upload a new document
      description: Upload a new document.
      operationId: createDocument
      x-api-path-slug: projectsprojectiddocuments-post
      parameters:
      - in: formData
        name: documents[]
        description: You can add as many files as you want in documents[] parameter
      - in: path
        name: projectId
        description: Project ID
      - in: formData
        name: schemes[]
        description: JSON string
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Documents
  /projects/{projectId}/documents/{documentId}:
    delete:
      summary: Delete the document
      description: Delete the document.
      operationId: deleteDocument
      x-api-path-slug: projectsprojectiddocumentsdocumentid-delete
      parameters:
      - in: path
        name: documentId
        description: Document ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Documents
      - DocumentId
    get:
      summary: Get single document
      description: Get single document.
      operationId: getDocument
      x-api-path-slug: projectsprojectiddocumentsdocumentid-get
      parameters:
      - in: path
        name: documentId
        description: Document ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Documents
      - DocumentId
    put:
      summary: Update the document.
      description: Update the document. File name and contents will replaced with
        the new one.
      operationId: updateDocument
      x-api-path-slug: projectsprojectiddocumentsdocumentid-put
      parameters:
      - in: path
        name: documentId
        description: Document ID
      - in: formData
        name: documents
        description: Single file data
      - in: path
        name: projectId
        description: Project ID
      - in: formData
        name: schemes
        description: JSON string
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Documents
      - DocumentId
  /projects/{projectId}/documents/{documentId}/download:
    get:
      summary: Download a document
      description: Download a document.
      operationId: downloadDocument
      x-api-path-slug: projectsprojectiddocumentsdocumentiddownload-get
      parameters:
      - in: path
        name: documentId
        description: Document ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Documents
      - DocumentId
      - Download
  /projects/{projectId}/glossaries:
    get:
      summary: Get a list of glossaries
      description: Get a list of glossaries.
      operationId: getGlossaries
      x-api-path-slug: projectsprojectidglossaries-get
      parameters:
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Glossaries
    post:
      summary: Upload a new glossary
      description: Upload a new glossary.
      operationId: createGlossary
      x-api-path-slug: projectsprojectidglossaries-post
      parameters:
      - in: formData
        name: glossaries
        description: You can only add one glossary, even though the name suggests
          multiple glossaries
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Glossaries
  /projects/{projectId}/glossaries/{glossaryId}:
    delete:
      summary: Delete the glossary
      description: Delete the glossary.
      operationId: deleteGlossary
      x-api-path-slug: projectsprojectidglossariesglossaryid-delete
      parameters:
      - in: path
        name: glossaryId
        description: Glossary ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Glossaries
      - GlossaryId
    get:
      summary: Get single glossary
      description: Get single glossary.
      operationId: getGlossary
      x-api-path-slug: projectsprojectidglossariesglossaryid-get
      parameters:
      - in: path
        name: glossaryId
        description: Glossary ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Glossaries
      - GlossaryId
    put:
      summary: Update the glossary.
      description: Update the glossary. File name and contents will replaced with
        the new one.
      operationId: updateGlossary
      x-api-path-slug: projectsprojectidglossariesglossaryid-put
      parameters:
      - in: formData
        name: glossaries
        description: Single file data
      - in: path
        name: glossaryId
        description: Glossary ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Glossaries
      - GlossaryId
  /projects/{projectId}/glossaries/{glossaryId}/download:
    get:
      summary: Download a glossary
      description: Download a glossary.
      operationId: downloadGlossary
      x-api-path-slug: projectsprojectidglossariesglossaryiddownload-get
      parameters:
      - in: path
        name: glossaryId
        description: Glossary ID
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Glossaries
      - GlossaryId
      - Download
  /projects/{projectId}/styleguides:
    get:
      summary: Get a list of style guides
      description: Get a list of style guides.
      operationId: getStyleGuides
      x-api-path-slug: projectsprojectidstyleguides-get
      parameters:
      - in: path
        name: projectId
        description: Project ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Styleguides
    post:
      summary: Upload a new style guide
      description: Upload a new style guide.
      operationId: createStyleGuide
      x-api-path-slug: projectsprojectidstyleguides-post
      parameters:
      - in: path
        name: projectId
        description: Project ID
      - in: formData
        name: styleguides[]
        description: You can add as many files as you want in styleguides[] parameter
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Styleguides
  /projects/{projectId}/styleguides/{styleGuideId}:
    delete:
      summary: Delete the style guide
      description: Delete the style guide.
      operationId: deleteStyleGuide
      x-api-path-slug: projectsprojectidstyleguidesstyleguideid-delete
      parameters:
      - in: path
        name: projectId
        description: Project ID
      - in: path
        name: styleGuideId
        description: Style Guide ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Styleguides
      - StyleGuideId
    get:
      summary: Get single style guide
      description: Get single style guide.
      operationId: getStyleGuide
      x-api-path-slug: projectsprojectidstyleguidesstyleguideid-get
      parameters:
      - in: path
        name: projectId
        description: Project ID
      - in: path
        name: styleGuideId
        description: Style Guide ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Styleguides
      - StyleGuideId
    put:
      summary: Update the style guide.
      description: Update the style guide. File name and contents will replaced with
        the new one.
      operationId: updateStyleGuide
      x-api-path-slug: projectsprojectidstyleguidesstyleguideid-put
      parameters:
      - in: path
        name: projectId
        description: Project ID
      - in: path
        name: styleGuideId
        description: Style guide ID
      - in: formData
        name: styleguides
        description: Single file data
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Styleguides
      - StyleGuideId
  /projects/{projectId}/styleguides/{styleGuideId}/download:
    get:
      summary: Download a style guide
      description: Download a style guide.
      operationId: downloadStyleGuide
      x-api-path-slug: projectsprojectidstyleguidesstyleguideiddownload-get
      parameters:
      - in: path
        name: projectId
        description: Project ID
      - in: path
        name: styleGuideId
        description: Style Guide ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - ProjectId
      - Styleguides
      - StyleGuideId
      - Download
  /styleguide:
    get:
      summary: Download the global style guide.
      description: Download your corporate account's global style guide. This endpoint
        is available only for corporate account customers.
      operationId: downloadGlobalStyleGuide
      x-api-path-slug: styleguide-get
      responses:
        200:
          description: OK
      tags:
      - Styleguide
    post:
      summary: Create or update the global style guide.
      description: Update your corporate account's global style guide. This endpoint
        is available only for corporate account customers.
      operationId: updateGlobalStyleGuide
      x-api-path-slug: styleguide-post
      parameters:
      - in: formData
        name: styleguide
        description: Style guide file
      responses:
        200:
          description: OK
      tags:
      - Styleguide
  /token:
    post:
      summary: Retrieve an access token to interact with the API.
      description: MotaWord API is using OAuth2 procedures when authenticating or
        authorizing your API call. Currently, we only allow Client Credential type
        flow.
      operationId: getAccessToken
      x-api-path-slug: token-post
      parameters:
      - in: header
        name: Authorization
        description: HTTP Basic Authorization header
      - in: formData
        name: grant_type
        description: OAuth2 grant type
      responses:
        200:
          description: OK
      tags:
      - Token