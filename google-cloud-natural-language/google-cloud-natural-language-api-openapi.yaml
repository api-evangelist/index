swagger: "2.0"
x-collection-name: Google Cloud Natural Language
x-complete: 1
info:
  title: Google Cloud Natural Language
  description: google-cloud-natural-language-api-provides-natural-language-understanding-technologies-to-developers--examples-include-sentiment-analysis-entity-recognition-and-text-annotations-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: language.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/documents:analyzeEntities:
    post:
      summary: Find Named Entities
      description: |-
        Finds named entities (currently proper names and common nouns) in the text
        along with entity types, salience, mentions for each entity, and
        other properties.
      operationId: language.documents.analyzeEntities
      x-api-path-slug: v1documentsanalyzeentities-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Entities
  /v1/documents:analyzeSentiment:
    post:
      summary: Analyze SEntiment
      description: Analyzes the sentiment of the provided text.
      operationId: language.documents.analyzeSentiment
      x-api-path-slug: v1documentsanalyzesentiment-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Sentiment
  /v1/documents:analyzeSyntax:
    post:
      summary: Analyze Syntax
      description: |-
        Analyzes the syntax of the text and provides sentence boundaries and
        tokenization along with part of speech tags, dependency trees, and other
        properties.
      operationId: language.documents.analyzeSyntax
      x-api-path-slug: v1documentsanalyzesyntax-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Syntax
  /v1/documents:annotateText:
    post:
      summary: Annotate Text
      description: |-
        A convenience method that provides all the features that analyzeSentiment,
        analyzeEntities, and analyzeSyntax provide in one call.
      operationId: language.documents.annotateText
      x-api-path-slug: v1documentsannotatetext-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Annotation