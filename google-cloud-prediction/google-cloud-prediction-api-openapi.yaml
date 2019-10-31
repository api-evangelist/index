swagger: "2.0"
x-collection-name: Google Cloud Prediction
x-complete: 1
info:
  title: Prediction
  description: lets-you-access-a-cloud-hosted-machine-learning-service-that-makes-it-easy-to-build-smart-apps
  contact:
    name: Google
    url: https://google.com
  version: v1.6
host: www.googleapis.com
basePath: /prediction/v1.6/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/hostedmodels/{hostedModelName}/predict:
    post:
      summary: Predict Model
      description: Submit input and request an output against a hosted model.
      operationId: prediction.hostedmodels.predict
      x-api-path-slug: projecthostedmodelshostedmodelnamepredict-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: hostedModelName
        description: The name of a hosted model
      - in: path
        name: project
        description: The project associated with the model
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Model
  /{project}/trainedmodels:
    post:
      summary: Train Model
      description: Train a Prediction API model.
      operationId: prediction.trainedmodels.insert
      x-api-path-slug: projecttrainedmodels-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: The project associated with the model
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Model
  /{project}/trainedmodels/list:
    get:
      summary: List Models
      description: List available models.
      operationId: prediction.trainedmodels.list
      x-api-path-slug: projecttrainedmodelslist-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Pagination token
      - in: path
        name: project
        description: The project associated with the model
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Model
  /{project}/trainedmodels/{id}:
    delete:
      summary: Delete Model
      description: Delete a trained model.
      operationId: prediction.trainedmodels.delete
      x-api-path-slug: projecttrainedmodelsid-delete
      parameters:
      - in: path
        name: id
        description: The unique name for the predictive model
      - in: path
        name: project
        description: The project associated with the model
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Model
    get:
      summary: Model Status
      description: Check training status of your model.
      operationId: prediction.trainedmodels.get
      x-api-path-slug: projecttrainedmodelsid-get
      parameters:
      - in: path
        name: id
        description: The unique name for the predictive model
      - in: path
        name: project
        description: The project associated with the model
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Model
    put:
      summary: Add New Data
      description: Add new data to a trained model.
      operationId: prediction.trainedmodels.update
      x-api-path-slug: projecttrainedmodelsid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The unique name for the predictive model
      - in: path
        name: project
        description: The project associated with the model
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Model
  /{project}/trainedmodels/{id}/analyze:
    get:
      summary: Analyze
      description: Get analysis of the model and the data the model was trained on.
      operationId: prediction.trainedmodels.analyze
      x-api-path-slug: projecttrainedmodelsidanalyze-get
      parameters:
      - in: path
        name: id
        description: The unique name for the predictive model
      - in: path
        name: project
        description: The project associated with the model
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Model
      - Analysis
  /{project}/trainedmodels/{id}/predict:
    post:
      summary: Predict
      description: Submit model id and request a prediction.
      operationId: prediction.trainedmodels.predict
      x-api-path-slug: projecttrainedmodelsidpredict-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The unique name for the predictive model
      - in: path
        name: project
        description: The project associated with the model
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Model