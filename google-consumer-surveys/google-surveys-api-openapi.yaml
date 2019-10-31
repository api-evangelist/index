swagger: "2.0"
x-collection-name: Google Consumer Surveys
x-complete: 1
info:
  title: Consumer Surveys
  description: creates-and-conducts-surveys-lists-the-surveys-that-an-authenticated-user-owns-and-retrieves-survey-results-and-information-about-specified-surveys-
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /consumersurveys/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /mobileAppPanels:
    get:
      summary: Get Mobile App Panels
      description: Lists the MobileAppPanels available to the authenticated user.
      operationId: consumersurveys.mobileapppanels.list
      x-api-path-slug: mobileapppanels-get
      parameters:
      - in: query
        name: maxResults
      - in: query
        name: startIndex
      - in: query
        name: token
      responses:
        200:
          description: OK
      tags:
      - Mobile Application
  /mobileAppPanels/{panelId}:
    get:
      summary: Get Mobile App Panel
      description: Retrieves a MobileAppPanel that is available to the authenticated
        user.
      operationId: consumersurveys.mobileapppanels.get
      x-api-path-slug: mobileapppanelspanelid-get
      parameters:
      - in: path
        name: panelId
        description: External URL ID for the panel
      responses:
        200:
          description: OK
      tags:
      - Mobile Application
    put:
      summary: Update Mobile App Panel
      description: Updates a MobileAppPanel. Currently the only property that can
        be updated is the owners property.
      operationId: consumersurveys.mobileapppanels.update
      x-api-path-slug: mobileapppanelspanelid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: panelId
        description: External URL ID for the panel
      responses:
        200:
          description: OK
      tags:
      - Mobile Application
  /surveys:
    get:
      summary: Get Surveys
      description: Lists the surveys owned by the authenticated user.
      operationId: consumersurveys.surveys.list
      x-api-path-slug: surveys-get
      parameters:
      - in: query
        name: maxResults
      - in: query
        name: startIndex
      - in: query
        name: token
      responses:
        200:
          description: OK
      tags:
      - Survey
    post:
      summary: Create Survey
      description: Creates a survey.
      operationId: consumersurveys.surveys.insert
      x-api-path-slug: surveys-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Survey
  /surveys/{resourceId}/start:
    post:
      summary: Begin Survey
      description: Begins running a survey.
      operationId: consumersurveys.surveys.start
      x-api-path-slug: surveysresourceidstart-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceId
      responses:
        200:
          description: OK
      tags:
      - Survey
  /surveys/{resourceId}/stop:
    post:
      summary: Stop Survey
      description: Stops a running survey.
      operationId: consumersurveys.surveys.stop
      x-api-path-slug: surveysresourceidstop-post
      parameters:
      - in: path
        name: resourceId
      responses:
        200:
          description: OK
      tags:
      - Survey
  /surveys/{surveyUrlId}:
    delete:
      summary: Remove Survey
      description: Removes a survey from view in all user GET requests.
      operationId: consumersurveys.surveys.delete
      x-api-path-slug: surveyssurveyurlid-delete
      parameters:
      - in: path
        name: surveyUrlId
        description: External URL ID for the survey
      responses:
        200:
          description: OK
      tags:
      - Survey
    get:
      summary: Get Survey
      description: Retrieves information about the specified survey.
      operationId: consumersurveys.surveys.get
      x-api-path-slug: surveyssurveyurlid-get
      parameters:
      - in: path
        name: surveyUrlId
        description: External URL ID for the survey
      responses:
        200:
          description: OK
      tags:
      - Survey
    put:
      summary: Update Survey
      description: Updates a survey. Currently the only property that can be updated
        is the owners property.
      operationId: consumersurveys.surveys.update
      x-api-path-slug: surveyssurveyurlid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: surveyUrlId
        description: External URL ID for the survey
      responses:
        200:
          description: OK
      tags:
      - Survey
  /surveys/{surveyUrlId}/results:
    get:
      summary: Get Survey Results
      description: Retrieves any survey results that have been produced so far. Results
        are formatted as an Excel file. You must add "?alt=media" to the URL as an
        argument to get results.
      operationId: consumersurveys.results.get
      x-api-path-slug: surveyssurveyurlidresults-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: surveyUrlId
        description: External URL ID for the survey
      responses:
        200:
          description: OK
      tags:
      - Survey