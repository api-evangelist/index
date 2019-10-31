swagger: "2.0"
x-collection-name: AWS Machine Learning
x-complete: 1
info:
  title: AWS Machine Learning API
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
      description: Adds one or more tags to an object, up to a limit of 10.
      operationId: addTags
      x-api-path-slug: actionaddtags-get
      parameters:
      - in: query
        name: ResourceId
        description: The ID of the ML object to tag
        type: string
      - in: query
        name: ResourceType
        description: The type of the ML object to tag
        type: string
      - in: query
        name: Tags
        description: The key-value pairs to use to create tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Tags
  /?Action=CreateBatchPrediction:
    get:
      summary: Create Batch Prediction
      description: Generates predictions for a group of observations.
      operationId: createBatchPrediction
      x-api-path-slug: actioncreatebatchprediction-get
      parameters:
      - in: query
        name: BatchPredictionDataSourceId
        description: The ID of the DataSource that points to the group of observations
          to predict
        type: string
      - in: query
        name: BatchPredictionId
        description: A user-supplied ID that uniquely identifies the                BatchPrediction
        type: string
      - in: query
        name: BatchPredictionName
        description: A user-supplied name or description of the BatchPrediction
        type: string
      - in: query
        name: MLModelId
        description: The ID of the MLModel that will generate predictions for the
          group of observations
        type: string
      - in: query
        name: OutputUri
        description: The location of an Amazon Simple Storage Service (Amazon S3)
          bucket or directory to store the batch prediction results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Batches
  /?Action=CreateDataSourceFromRDS:
    get:
      summary: Create Data Source From R D S
      description: Creates a DataSource object from an.
      operationId: createDataSourceFromRDS
      x-api-path-slug: actioncreatedatasourcefromrds-get
      parameters:
      - in: query
        name: ComputeStatistics
        description: The compute statistics for a DataSource
        type: string
      - in: query
        name: DataSourceId
        description: A user-supplied ID that uniquely identifies the DataSource
        type: string
      - in: query
        name: DataSourceName
        description: A user-supplied name or description of the DataSource
        type: string
      - in: query
        name: RDSData
        description: 'The data specification of an Amazon RDS DataSource:'
        type: string
      - in: query
        name: RoleARN
        description: The role that Amazon ML assumes on behalf of the user to create
          and activate a data          pipeline in the users account and copy data
          using the SelectSqlQuery query from Amazon RDS to Amazon S3
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=CreateDataSourceFromRedshift:
    get:
      summary: Create Data Source From Redshift
      description: Creates a DataSource from a database hosted on an Amazon Redshift
        cluster.
      operationId: createDataSourceFromRedshift
      x-api-path-slug: actioncreatedatasourcefromredshift-get
      parameters:
      - in: query
        name: ComputeStatistics
        description: The compute statistics for a DataSource
        type: string
      - in: query
        name: DataSourceId
        description: A user-supplied ID that uniquely identifies the DataSource
        type: string
      - in: query
        name: DataSourceName
        description: A user-supplied name or description of the DataSource
        type: string
      - in: query
        name: DataSpec
        description: 'The data specification of an Amazon Redshift DataSource:'
        type: string
      - in: query
        name: RoleARN
        description: A fully specified role Amazon Resource Name (ARN)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=CreateDataSourceFromS3:
    get:
      summary: Create Data Source From S3
      description: Creates a DataSource object.
      operationId: createDataSourceFromS3
      x-api-path-slug: actioncreatedatasourcefroms3-get
      parameters:
      - in: query
        name: ComputeStatistics
        description: The compute statistics for a DataSource
        type: string
      - in: query
        name: DataSourceId
        description: A user-supplied identifier that uniquely identifies the DataSource
        type: string
      - in: query
        name: DataSourceName
        description: A user-supplied name or description of the DataSource
        type: string
      - in: query
        name: DataSpec
        description: 'The data specification of a DataSource:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=CreateEvaluation:
    get:
      summary: Create Evaluation
      description: Creates a new Evaluation of an MLModel.
      operationId: createEvaluation
      x-api-path-slug: actioncreateevaluation-get
      parameters:
      - in: query
        name: EvaluationDataSourceId
        description: The ID of the DataSource for the evaluation
        type: string
      - in: query
        name: EvaluationId
        description: A user-supplied ID that uniquely identifies the Evaluation
        type: string
      - in: query
        name: EvaluationName
        description: A user-supplied name or description of the Evaluation
        type: string
      - in: query
        name: MLModelId
        description: The ID of the MLModel to evaluate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Evaluations
  /?Action=CreateMLModel:
    get:
      summary: Create M L Model
      description: |-
        Creates a new MLModel using the DataSource and the recipe as
                    information sources.
      operationId: createMLModel
      x-api-path-slug: actioncreatemlmodel-get
      parameters:
      - in: query
        name: MLModelId
        description: A user-supplied ID that uniquely identifies the MLModel
        type: string
      - in: query
        name: MLModelName
        description: A user-supplied name or description of the MLModel
        type: string
      - in: query
        name: MLModelType
        description: The category of supervised learning that this MLModel will address
        type: string
      - in: query
        name: Parameters
        description: A list of the training parameters in the MLModel
        type: string
      - in: query
        name: Recipe
        description: The data recipe for creating the MLModel
        type: string
      - in: query
        name: RecipeUri
        description: The Amazon Simple Storage Service (Amazon S3) location and file
          name that contains the MLModel recipe
        type: string
      - in: query
        name: TrainingDataSourceId
        description: The DataSource that points to the training data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Models
  /?Action=CreateRealtimeEndpoint:
    get:
      summary: Create Realtime Endpoint
      description: Creates a real-time endpoint for the MLModel.
      operationId: createRealtimeEndpoint
      x-api-path-slug: actioncreaterealtimeendpoint-get
      parameters:
      - in: query
        name: MLModelId
        description: The ID assigned to the MLModel during creation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Real Time
  /?Action=DeleteBatchPrediction:
    get:
      summary: Delete Batch Prediction
      description: Assigns the DELETED status to a BatchPrediction, rendering it unusable.
      operationId: deleteBatchPrediction
      x-api-path-slug: actiondeletebatchprediction-get
      parameters:
      - in: query
        name: BatchPredictionId
        description: A user-supplied ID that uniquely identifies the BatchPrediction
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Batches
  /?Action=DeleteDataSource:
    get:
      summary: Delete Data Source
      description: Assigns the DELETED status to a DataSource, rendering it unusable.
      operationId: deleteDataSource
      x-api-path-slug: actiondeletedatasource-get
      parameters:
      - in: query
        name: DataSourceId
        description: A user-supplied ID that uniquely identifies the DataSource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=DeleteEvaluation:
    get:
      summary: Delete Evaluation
      description: Assigns the DELETED status to an Evaluation, rendering it unusable.
      operationId: deleteEvaluation
      x-api-path-slug: actiondeleteevaluation-get
      parameters:
      - in: query
        name: EvaluationId
        description: A user-supplied ID that uniquely identifies the Evaluation to
          delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Evaluations
  /?Action=DeleteMLModel:
    get:
      summary: Delete M L Model
      description: Assigns the DELETED status to an MLModel, rendering it unusable.
      operationId: deleteMLModel
      x-api-path-slug: actiondeletemlmodel-get
      parameters:
      - in: query
        name: MLModelId
        description: A user-supplied ID that uniquely identifies the MLModel
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Models
  /?Action=DeleteRealtimeEndpoint:
    get:
      summary: Delete Realtime Endpoint
      description: Deletes a real time endpoint of an MLModel.
      operationId: deleteRealtimeEndpoint
      x-api-path-slug: actiondeleterealtimeendpoint-get
      parameters:
      - in: query
        name: MLModelId
        description: The ID assigned to the MLModel during creation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Real Time
  /?Action=DeleteTags:
    get:
      summary: Delete Tags
      description: Deletes the specified tags associated with an ML object.
      operationId: deleteTags
      x-api-path-slug: actiondeletetags-get
      parameters:
      - in: query
        name: ResourceId
        description: The ID of the tagged ML object
        type: string
      - in: query
        name: ResourceType
        description: The type of the tagged ML object
        type: string
      - in: query
        name: TagKeys
        description: One or more tags to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Tags
  /?Action=DescribeBatchPredictions:
    get:
      summary: Describe Batch Predictions
      description: Returns a list of BatchPrediction operations that match the search
        criteria in the request.
      operationId: describeBatchPredictions
      x-api-path-slug: actiondescribebatchpredictions-get
      parameters:
      - in: query
        name: EQ
        description: The equal to operator
        type: string
      - in: query
        name: FilterVariable
        description: 'Use one of the following variables to filter a list of BatchPrediction:'
        type: string
      - in: query
        name: GE
        description: The greater than or equal to operator
        type: string
      - in: query
        name: GT
        description: The greater than operator
        type: string
      - in: query
        name: LE
        description: The less than or equal to operator
        type: string
      - in: query
        name: Limit
        description: The number of pages of information to include in the result
        type: string
      - in: query
        name: LT
        description: The less than operator
        type: string
      - in: query
        name: NE
        description: The not equal to operator
        type: string
      - in: query
        name: NextToken
        description: An ID of the page in the paginated results
        type: string
      - in: query
        name: Prefix
        description: A string that is found at the beginning of a variable, such as
          Name or Id
        type: string
      - in: query
        name: SortOrder
        description: A two-value parameter that determines the sequence of the resulting
          list of MLModels
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Batches
  /?Action=DescribeDataSources:
    get:
      summary: Describe Data Sources
      description: Returns a list of DataSource that match the search criteria in
        the request.
      operationId: describeDataSources
      x-api-path-slug: actiondescribedatasources-get
      parameters:
      - in: query
        name: EQ
        description: The equal to operator
        type: string
      - in: query
        name: FilterVariable
        description: 'Use one of the following variables to filter a list of DataSource:'
        type: string
      - in: query
        name: GE
        description: The greater than or equal to operator
        type: string
      - in: query
        name: GT
        description: The greater than operator
        type: string
      - in: query
        name: LE
        description: The less than or equal to operator
        type: string
      - in: query
        name: Limit
        description: The maximum number of DataSource to include in the result
        type: string
      - in: query
        name: LT
        description: The less than operator
        type: string
      - in: query
        name: NE
        description: The not equal to operator
        type: string
      - in: query
        name: NextToken
        description: The ID of the page in the paginated results
        type: string
      - in: query
        name: Prefix
        description: A string that is found at the beginning of a variable, such as
          Name or Id
        type: string
      - in: query
        name: SortOrder
        description: A two-value parameter that determines the sequence of the resulting
          list of DataSource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=DescribeEvaluations:
    get:
      summary: Describe Evaluations
      description: Returns a list of DescribeEvaluations that match the search criteria
        in the request.
      operationId: describeEvaluations
      x-api-path-slug: actiondescribeevaluations-get
      parameters:
      - in: query
        name: EQ
        description: The equal to operator
        type: string
      - in: query
        name: FilterVariable
        description: 'Use one of the following variable to filter a list of Evaluation
          objects:'
        type: string
      - in: query
        name: GE
        description: The greater than or equal to operator
        type: string
      - in: query
        name: GT
        description: The greater than operator
        type: string
      - in: query
        name: LE
        description: The less than or equal to operator
        type: string
      - in: query
        name: Limit
        description: The maximum number of Evaluation to include in the result
        type: string
      - in: query
        name: LT
        description: The less than operator
        type: string
      - in: query
        name: NE
        description: The not equal to operator
        type: string
      - in: query
        name: NextToken
        description: The ID of the page in the paginated results
        type: string
      - in: query
        name: Prefix
        description: A string that is found at the beginning of a variable, such as
          Name or Id
        type: string
      - in: query
        name: SortOrder
        description: A two-value parameter that determines the sequence of the resulting
          list of Evaluation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Evaluations
  /?Action=DescribeMLModels:
    get:
      summary: Describe M L Models
      description: Returns a list of MLModel that match the search criteria in the
        request.
      operationId: describeMLModels
      x-api-path-slug: actiondescribemlmodels-get
      parameters:
      - in: query
        name: EQ
        description: The equal to operator
        type: string
      - in: query
        name: FilterVariable
        description: 'Use one of the following variables to filter a list of MLModel:'
        type: string
      - in: query
        name: GE
        description: The greater than or equal to operator
        type: string
      - in: query
        name: GT
        description: The greater than operator
        type: string
      - in: query
        name: LE
        description: The less than or equal to operator
        type: string
      - in: query
        name: Limit
        description: The number of pages of information to include in the result
        type: string
      - in: query
        name: LT
        description: The less than operator
        type: string
      - in: query
        name: NE
        description: The not equal to operator
        type: string
      - in: query
        name: NextToken
        description: The ID of the page in the paginated results
        type: string
      - in: query
        name: Prefix
        description: A string that is found at the beginning of a variable, such as
          Name or Id
        type: string
      - in: query
        name: SortOrder
        description: A two-value parameter that determines the sequence of the resulting
          list of MLModel
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Models
  /?Action=DescribeTags:
    get:
      summary: Describe Tags
      description: Describes one or more of the tags for your Amazon ML object.
      operationId: describeTags
      x-api-path-slug: actiondescribetags-get
      parameters:
      - in: query
        name: ResourceId
        description: The ID of the ML object
        type: string
      - in: query
        name: ResourceType
        description: The type of the ML object
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Real Time
  /?Action=GetBatchPrediction:
    get:
      summary: Get Batch Prediction
      description: |-
        Returns a BatchPrediction that includes detailed metadata, status, and data file information for a
                    Batch Prediction request.
      operationId: getBatchPrediction
      x-api-path-slug: actiongetbatchprediction-get
      parameters:
      - in: query
        name: BatchPredictionId
        description: An ID assigned to the BatchPrediction at creation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Batches
  /?Action=GetDataSource:
    get:
      summary: Get Data Source
      description: Returns a DataSource that includes metadata and data file information,
        as well as the current status of the DataSource.
      operationId: getDataSource
      x-api-path-slug: actiongetdatasource-get
      parameters:
      - in: query
        name: DataSourceId
        description: The ID assigned to the DataSource at creation
        type: string
      - in: query
        name: Verbose
        description: Specifies whether the GetDataSource operation should return DataSourceSchema
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=GetEvaluation:
    get:
      summary: Get Evaluation
      description: Returns an Evaluation that includes metadata as well as the current
        status of the Evaluation.
      operationId: getEvaluation
      x-api-path-slug: actiongetevaluation-get
      parameters:
      - in: query
        name: EvaluationId
        description: The ID of the Evaluation to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Evaluations
  /?Action=GetMLModel:
    get:
      summary: Get M L Model
      description: Returns an MLModel that includes detailed metadata, data source
        information, and the current status of the MLModel.
      operationId: getMLModel
      x-api-path-slug: actiongetmlmodel-get
      parameters:
      - in: query
        name: MLModelId
        description: The ID assigned to the MLModel at creation
        type: string
      - in: query
        name: Verbose
        description: Specifies whether the GetMLModel operation should return Recipe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Models
  /?Action=Predict:
    get:
      summary: Predict
      description: Generates a prediction for the observation using the specified
        ML Model.
      operationId: predict
      x-api-path-slug: actionpredict-get
      parameters:
      - in: query
        name: MLModelId
        description: A unique identifier of the MLModel
        type: string
      - in: query
        name: PredictEndpoint
        description: 'Type: String'
        type: string
      - in: query
        name: Record
        description: A map of variable name-value pairs that represent an observation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Predict
  /?Action=UpdateBatchPrediction:
    get:
      summary: Update Batch Prediction
      description: Updates the BatchPredictionName of a BatchPrediction.
      operationId: updateBatchPrediction
      x-api-path-slug: actionupdatebatchprediction-get
      parameters:
      - in: query
        name: BatchPredictionId
        description: The ID assigned to the BatchPrediction during creation
        type: string
      - in: query
        name: BatchPredictionName
        description: A new user-supplied name or description of the BatchPrediction
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Batches
  /?Action=UpdateDataSource:
    get:
      summary: Update Data Source
      description: Updates the DataSourceName of a DataSource.
      operationId: updateDataSource
      x-api-path-slug: actionupdatedatasource-get
      parameters:
      - in: query
        name: DataSourceId
        description: The ID assigned to the DataSource during creation
        type: string
      - in: query
        name: DataSourceName
        description: A new user-supplied name or description of the DataSource that
          will replace the current description
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=UpdateEvaluation:
    get:
      summary: Update Evaluation
      description: Updates the EvaluationName of an Evaluation.
      operationId: updateEvaluation
      x-api-path-slug: actionupdateevaluation-get
      parameters:
      - in: query
        name: EvaluationId
        description: The ID assigned to the Evaluation during creation
        type: string
      - in: query
        name: EvaluationName
        description: A new user-supplied name or description of the Evaluation that
          will replace the current content
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Evaluations
  /?Action=UpdateMLModel:
    get:
      summary: Update M L Model
      description: Updates the MLModelName and the ScoreThreshold of an MLModel.
      operationId: updateMLModel
      x-api-path-slug: actionupdatemlmodel-get
      parameters:
      - in: query
        name: MLModelId
        description: The ID assigned to the MLModel during creation
        type: string
      - in: query
        name: MLModelName
        description: A user-supplied name or description of the MLModel
        type: string
      - in: query
        name: ScoreThreshold
        description: The ScoreThreshold used in binary classification MLModel that
          marks the boundary between a positive prediction and a negative prediction
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Models