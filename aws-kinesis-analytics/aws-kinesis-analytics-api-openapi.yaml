swagger: "2.0"
x-collection-name: AWS Kinesis Analytics
x-complete: 1
info:
  title: AWS Kinesis Analytics API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddApplicationInput:
    get:
      summary: Add Application Input
      description: Adds a streaming source to your Amazon Kinesis application.
      operationId: addApplicationInput
      x-api-path-slug: actionaddapplicationinput-get
      parameters:
      - in: query
        name: ApplicationName
        description: Name of your existing Amazon Kinesis Analytics application to
          which you want to add the streaming source
        type: string
      - in: query
        name: CurrentApplicationVersionId
        description: Current version of your Amazon Kinesis Analytics application
        type: string
      - in: query
        name: Input
        description: When you configure the application input, you specify the streaming
          source,  the         in-application stream name that is created, and the
          mapping between the two
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=AddApplicationOutput:
    get:
      summary: Add Application Output
      description: Adds an external destination to your Amazon Kinesis Analytics application.
      operationId: addApplicationOutput
      x-api-path-slug: actionaddapplicationoutput-get
      parameters:
      - in: query
        name: ApplicationName
        description: Name of the application to which you want to add the output configuration
        type: string
      - in: query
        name: CurrentApplicationVersionId
        description: Version of the application to which you want add the             output
          configuration
        type: string
      - in: query
        name: Output
        description: An array of objects, each describing one output configuration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=AddApplicationReferenceDataSource:
    get:
      summary: Add Application Reference Data Source
      description: Adds a reference data source to an existing application.
      operationId: addApplicationReferenceDataSource
      x-api-path-slug: actionaddapplicationreferencedatasource-get
      parameters:
      - in: query
        name: ApplicationName
        description: Name of an existing application
        type: string
      - in: query
        name: CurrentApplicationVersionId
        description: Version of the application for which you are adding the reference
          data source
        type: string
      - in: query
        name: ReferenceDataSource
        description: The reference data source can be an object in your Amazon S3
          bucket
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=CreateApplication:
    get:
      summary: Create Application
      description: Creates an Amazon Kinesis Analytics application.
      operationId: createApplication
      x-api-path-slug: actioncreateapplication-get
      parameters:
      - in: query
        name: ApplicationCode
        description: One or more SQL statements that read input data, transform it,             and
          generate output
        type: string
      - in: query
        name: ApplicationDescription
        description: Summary description of the application
        type: string
      - in: query
        name: ApplicationName
        description: Name of your Amazon Kinesis Analytics application (for example,
          sample-app)
        type: string
      - in: query
        name: Inputs
        description: Use this parameter to configure the application input
        type: string
      - in: query
        name: Outputs
        description: You can configure application output to write data from any of
          the in-application streams to up to five destinations
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=DeleteApplication:
    get:
      summary: Delete Application
      description: Deletes the specified application.
      operationId: deleteApplication
      x-api-path-slug: actiondeleteapplication-get
      parameters:
      - in: query
        name: ApplicationName
        description: Name of the Amazon Kinesis Analytics application to delete
        type: string
      - in: query
        name: CreateTimestamp
        description: You can use the DescribeApplication operation to get this value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=DeleteApplicationOutput:
    get:
      summary: Delete Application Output
      description: Deletes output destination configuration from your application
        configuration.
      operationId: deleteApplicationOutput
      x-api-path-slug: actiondeleteapplicationoutput-get
      parameters:
      - in: query
        name: ApplicationName
        description: Amazon Kinesis Analytics application name
        type: string
      - in: query
        name: CurrentApplicationVersionId
        description: Amazon Kinesis Analytics application version
        type: string
      - in: query
        name: OutputId
        description: The ID of the configuration to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=DeleteApplicationReferenceDataSource:
    get:
      summary: Delete Application Reference Data Source
      description: Deletes a reference data source configuration from the specified
        application configuration.
      operationId: deleteApplicationReferenceDataSource
      x-api-path-slug: actiondeleteapplicationreferencedatasource-get
      parameters:
      - in: query
        name: ApplicationName
        description: Name of an existing application
        type: string
      - in: query
        name: CurrentApplicationVersionId
        description: Version of the application
        type: string
      - in: query
        name: ReferenceId
        description: ID of the reference data source
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=DescribeApplication:
    get:
      summary: Describe Application
      description: Returns information about a specific Amazon Kinesis Analytics application.
      operationId: describeApplication
      x-api-path-slug: actiondescribeapplication-get
      parameters:
      - in: query
        name: ApplicationName
        description: Name of the application
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=DiscoverInputSchema:
    get:
      summary: Discover Input Schema
      description: Infers a schema by evaluating sample records on the specified streaming
        source (Amazon Kinesis stream or Amazon Kinesis Firehose delivery stream).
      operationId: discoverInputSchema
      x-api-path-slug: actiondiscoverinputschema-get
      parameters:
      - in: query
        name: InputStartingPositionConfiguration
        description: Point at which you want Amazon Kinesis Analytics to start reading
          records from the specified streaming source discovery purposes
        type: string
      - in: query
        name: ResourceARN
        description: Amazon Resource Name (ARN) of the streaming source
        type: string
      - in: query
        name: RoleARN
        description: ARN of the IAM role that Amazon Kinesis Analytics can assume
          to access the stream on your behalf
        type: string
      responses:
        200:
          description: OK
      tags:
      - Schema
  /?Action=ListApplications:
    get:
      summary: List Applications
      description: Returns a list of Amazon Kinesis Analytics applications in your
        account.
      operationId: listApplications
      x-api-path-slug: actionlistapplications-get
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=StartApplication:
    get:
      summary: Start Application
      description: Starts the specified Amazon Kinesis Analytics application.
      operationId: startApplication
      x-api-path-slug: actionstartapplication-get
      parameters:
      - in: query
        name: ApplicationName
        description: Name of the application
        type: string
      - in: query
        name: InputConfigurations
        description: Identifies the specific input, by ID, that the application starts
          consuming
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=StopApplication:
    get:
      summary: Stop Application
      description: Stops the application from processing input data.
      operationId: stopApplication
      x-api-path-slug: actionstopapplication-get
      parameters:
      - in: query
        name: ApplicationName
        description: Name of the running application to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=UpdateApplication:
    get:
      summary: Update Application
      description: Updates an existing Amazon Kinesis Analytics application.
      operationId: updateApplication
      x-api-path-slug: actionupdateapplication-get
      parameters:
      - in: query
        name: ApplicationName
        description: Name of the Amazon Kinesis Analytics application to update
        type: string
      - in: query
        name: ApplicationUpdate
        description: Describes application updates
        type: string
      - in: query
        name: CurrentApplicationVersionId
        description: The current application version ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications