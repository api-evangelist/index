swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 1
info:
  title: AWS Elastic Beanstalk API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AbortEnvironmentUpdate:
    get:
      summary: Abort Environment Update
      description: |-
        Cancels in-progress environment configuration update or application version
              deployment.
      operationId: abortEnvironmentUpdate
      x-api-path-slug: actionabortenvironmentupdate-get
      parameters:
      - in: query
        name: EnvironmentId
        description: This specifies the ID of the environment with the in-progress
          update that you want to      cancel
        type: string
      - in: query
        name: EnvironmentName
        description: This specifies the name of the environment with the in-progress
          update that you want to      cancel
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=ApplyEnvironmentManagedAction:
    get:
      summary: Apply Environment Managed Action
      description: Applies a scheduled managed action immediately.
      operationId: applyEnvironmentManagedAction
      x-api-path-slug: actionapplyenvironmentmanagedaction-get
      parameters:
      - in: query
        name: ActionId
        description: The action ID of the scheduled managed action to execute
        type: string
      - in: query
        name: EnvironmentId
        description: The environment ID of the target environment
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the target environment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=CheckDNSAvailability:
    get:
      summary: Check D N S Availability
      description: Checks if the specified CNAME is available.
      operationId: checkDNSAvailability
      x-api-path-slug: actioncheckdnsavailability-get
      parameters:
      - in: query
        name: CNAMEPrefix
        description: The prefix used when this CNAME is reserved
        type: string
      responses:
        200:
          description: OK
      tags:
      - DNS
  /?Action=ComposeEnvironments:
    get:
      summary: Compose Environments
      description: |-
        Create or update a group of environments that each run a separate component of a single
              application.
      operationId: composeEnvironments
      x-api-path-slug: actioncomposeenvironments-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application to which the specified source bundles
          belong
        type: string
      - in: query
        name: GroupName
        description: The name of the group to which the target environments belong
        type: string
      - in: query
        name: VersionLabels.member.N
        description: A list of version labels, specifying one or more application
          source bundles that belong      to the target application
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=CreateApplication:
    get:
      summary: Create Application
      description: |-
        Creates an application that has one configuration template named default
              and no application versions.
      operationId: createApplication
      x-api-path-slug: actioncreateapplication-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application
        type: string
      - in: query
        name: Description
        description: Describes the application
        type: string
      - in: query
        name: ResourceLifecycleConfig
        description: Specify an application resource lifecycle configuration to prevent
          your application      from accumulating too many versions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=CreateApplicationVersion:
    get:
      summary: Create Application Version
      description: Creates an application version for the specified application.
      operationId: createApplicationVersion
      x-api-path-slug: actioncreateapplicationversion-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application
        type: string
      - in: query
        name: AutoCreateApplication
        description: Set to true to create an application with the specified name
          if it doesnt      already exist
        type: string
      - in: query
        name: BuildConfiguration
        description: Settings for an AWS CodeBuild build
        type: string
      - in: query
        name: Description
        description: Describes this version
        type: string
      - in: query
        name: Process
        description: Preprocesses and validates the environment manifest and configuration
          files in the      source bundle
        type: string
      - in: query
        name: SourceBuildInformation
        description: Specify a commit in an AWS CodeCommit Git repository to use as
          the source code for the      application version
        type: string
      - in: query
        name: SourceBundle
        description: The Amazon S3 bucket and key that identify the location of the
          source bundle for this      version
        type: string
      - in: query
        name: VersionLabel
        description: A label identifying this version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=CreateConfigurationTemplate:
    get:
      summary: Create Configuration Template
      description: Creates a configuration template.
      operationId: createConfigurationTemplate
      x-api-path-slug: actioncreateconfigurationtemplate-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application to associate with this configuration
          template
        type: string
      - in: query
        name: Description
        description: Describes this configuration
        type: string
      - in: query
        name: EnvironmentId
        description: The ID of the environment used with this configuration template
        type: string
      - in: query
        name: OptionSettings.member.N
        description: If specified, AWS Elastic Beanstalk sets the specified configuration
          option to the      requested value
        type: string
      - in: query
        name: SolutionStackName
        description: The name of the solution stack used by this configuration
        type: string
      - in: query
        name: SourceConfiguration
        description: If specified, AWS Elastic Beanstalk uses the configuration values
          from the specified      configuration template to create a new configuration
        type: string
      - in: query
        name: TemplateName
        description: The name of the configuration template
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Templates
  /?Action=CreateEnvironment:
    get:
      summary: Create Environment
      description: |-
        Launches an environment for the specified application using the specified
              configuration.
      operationId: createEnvironment
      x-api-path-slug: actioncreateenvironment-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application that contains the version to be deployed
        type: string
      - in: query
        name: CNAMEPrefix
        description: If specified, the environment attempts to use this value as the
          prefix for the CNAME
        type: string
      - in: query
        name: Description
        description: Describes this environment
        type: string
      - in: query
        name: EnvironmentName
        description: A unique name for the deployment environment
        type: string
      - in: query
        name: GroupName
        description: The name of the group to which the target environment belongs
        type: string
      - in: query
        name: OptionSettings.member.N
        description: If specified, AWS Elastic Beanstalk sets the specified configuration
          options to the      requested value in the configuration set for the new
          environment
        type: string
      - in: query
        name: OptionsToRemove.member.N
        description: A list of custom user-defined configuration options to remove
          from the configuration      set for this new environment
        type: string
      - in: query
        name: SolutionStackName
        description: This is an alternative to specifying a template name
        type: string
      - in: query
        name: Tags.member.N
        description: This specifies the tags applied to resources in the environment
        type: string
      - in: query
        name: TemplateName
        description: The name of the configuration template to use in deployment
        type: string
      - in: query
        name: Tier
        description: This specifies the tier to use for creating this environment
        type: string
      - in: query
        name: VersionLabel
        description: The name of the application version to deploy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=CreateStorageLocation:
    get:
      summary: Create Storage Location
      description: Creates the Amazon S3 storage location for the account.
      operationId: createStorageLocation
      x-api-path-slug: actioncreatestoragelocation-get
      parameters:
      - in: query
        name: S3Bucket
        description: The name of the Amazon S3 bucket created
        type: string
      responses:
        200:
          description: OK
      tags:
      - Storage Location
  /?Action=DeleteApplication:
    get:
      summary: Delete Application
      description: |-
        Deletes the specified application along with all associated versions and
              configurations.
      operationId: deleteApplication
      x-api-path-slug: actiondeleteapplication-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application to delete
        type: string
      - in: query
        name: TerminateEnvByForce
        description: When set to true, running environments will be terminated before
          deleting the      application
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=DeleteApplicationVersion:
    get:
      summary: Delete Application Version
      description: Deletes the specified version from the specified application.
      operationId: deleteApplicationVersion
      x-api-path-slug: actiondeleteapplicationversion-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application to which the version belongs
        type: string
      - in: query
        name: DeleteSourceBundle
        description: Set to true to delete the source bundle from your storage bucket
        type: string
      - in: query
        name: VersionLabel
        description: The label of the version to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Application Version
  /?Action=DeleteConfigurationTemplate:
    get:
      summary: Delete Configuration Template
      description: Deletes the specified configuration template.
      operationId: deleteConfigurationTemplate
      x-api-path-slug: actiondeleteconfigurationtemplate-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application to delete the configuration template
          from
        type: string
      - in: query
        name: TemplateName
        description: The name of the configuration template to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Templates
  /?Action=DeleteEnvironmentConfiguration:
    get:
      summary: Delete Environment Configuration
      description: Deletes the draft configuration associated with the running environment.
      operationId: deleteEnvironmentConfiguration
      x-api-path-slug: actiondeleteenvironmentconfiguration-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application the environment is associated with
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment to delete the draft configuration
          from
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=DescribeApplications:
    get:
      summary: Describe Applications
      description: Returns the descriptions of existing applications.
      operationId: describeApplications
      x-api-path-slug: actiondescribeapplications-get
      parameters:
      - in: query
        name: ApplicationNames.member.N
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to only include      those with the specified names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=DescribeApplicationVersions:
    get:
      summary: Describe Application Versions
      description: Retrieve a list of application versions.
      operationId: describeApplicationVersions
      x-api-path-slug: actiondescribeapplicationversions-get
      parameters:
      - in: query
        name: ApplicationName
        description: Specify an application name to show only application versions
          for that      application
        type: string
      - in: query
        name: MaxRecords
        description: Specify a maximum number of application versions to paginate
          in the request
        type: string
      - in: query
        name: NextToken
        description: Specify a next token to retrieve the next page in a paginated
          request
        type: string
      - in: query
        name: VersionLabels.member.N
        description: Specify a version label to show a specific application version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Application Version
  /?Action=DescribeConfigurationOptions:
    get:
      summary: Describe Configuration Options
      description: |-
        Describes the configuration options that are used in a particular configuration
              template or environment, or that a specified solution stack defines.
      operationId: describeConfigurationOptions
      x-api-path-slug: actiondescribeconfigurationoptions-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application associated with the configuration
          template or environment
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment whose configuration options you want
          to describe
        type: string
      - in: query
        name: Options.member.N
        description: If specified, restricts the descriptions to only the specified
          options
        type: string
      - in: query
        name: SolutionStackName
        description: The name of the solution stack whose configuration options you
          want to      describe
        type: string
      - in: query
        name: TemplateName
        description: The name of the configuration template whose configuration options
          you want to      describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - ConfigurationOptions
  /?Action=DescribeConfigurationSettings:
    get:
      summary: Describe Configuration Settings
      description: |-
        Returns a description of the settings for the specified configuration set, that is,
              either a configuration template or the configuration set associated with a running
              environment.
      operationId: describeConfigurationSettings
      x-api-path-slug: actiondescribeconfigurationsettings-get
      parameters:
      - in: query
        name: ApplicationName
        description: The application for the environment or configuration template
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment to describe
        type: string
      - in: query
        name: TemplateName
        description: The name of the configuration template to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Settings
  /?Action=DescribeEnvironmentHealth:
    get:
      summary: Describe Environment Health
      description: Returns information about the overall health of the specified environment.
      operationId: describeEnvironmentHealth
      x-api-path-slug: actiondescribeenvironmenthealth-get
      parameters:
      - in: query
        name: AttributeNames.member.N
        description: Specify the response elements to return
        type: string
      - in: query
        name: EnvironmentId
        description: Specify the environment by ID
        type: string
      - in: query
        name: EnvironmentName
        description: Specify the environment by name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=DescribeEnvironmentManagedActionHistory:
    get:
      summary: Describe Environment Managed Action History
      description: Lists an environment's completed and failed managed actions.
      operationId: describeEnvironmentManagedActionHistory
      x-api-path-slug: actiondescribeenvironmentmanagedactionhistory-get
      parameters:
      - in: query
        name: EnvironmentId
        description: The environment ID of the target environment
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the target environment
        type: string
      - in: query
        name: MaxItems
        description: The maximum number of items to return for a single request
        type: string
      - in: query
        name: NextToken
        description: The pagination token returned by a previous request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=DescribeEnvironmentManagedActions:
    get:
      summary: Describe Environment Managed Actions
      description: Lists an environment's upcoming and in-progress managed actions.
      operationId: describeEnvironmentManagedActions
      x-api-path-slug: actiondescribeenvironmentmanagedactions-get
      parameters:
      - in: query
        name: EnvironmentId
        description: The environment ID of the target environment
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the target environment
        type: string
      - in: query
        name: Status
        description: To show only actions with a particular status, specify a status
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=DescribeEnvironmentResources:
    get:
      summary: Describe Environment Resources
      description: Returns AWS resources for this environment.
      operationId: describeEnvironmentResources
      x-api-path-slug: actiondescribeenvironmentresources-get
      parameters:
      - in: query
        name: EnvironmentId
        description: The ID of the environment to retrieve AWS resource usage data
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment to retrieve AWS resource usage data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=DescribeEnvironments:
    get:
      summary: Describe Environments
      description: Returns descriptions for existing environments.
      operationId: describeEnvironments
      x-api-path-slug: actiondescribeenvironments-get
      parameters:
      - in: query
        name: ApplicationName
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to include only      those that are associated with this application
        type: string
      - in: query
        name: EnvironmentIds.member.N
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to include only      those that have the specified IDs
        type: string
      - in: query
        name: EnvironmentNames.member.N
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to include only      those that have the specified names
        type: string
      - in: query
        name: IncludedDeletedBackTo
        description: If specified when IncludeDeleted is set to true, then      environments
          deleted after this date are displayed
        type: string
      - in: query
        name: IncludeDeleted
        description: 'Indicates whether to include deleted environments:'
        type: string
      - in: query
        name: VersionLabel
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to include only      those that are associated with this application version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=DescribeEvents:
    get:
      summary: Describe Events
      description: Returns list of event descriptions matching criteria up to the
        last 6 weeks.
      operationId: describeEvents
      x-api-path-slug: actiondescribeevents-get
      parameters:
      - in: query
        name: ApplicationName
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to include only      those associated with this application
        type: string
      - in: query
        name: EndTime
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those that      occur up to, but not including, the EndTime
        type: string
      - in: query
        name: EnvironmentId
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those      associated with this environment
        type: string
      - in: query
        name: EnvironmentName
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those      associated with this environment
        type: string
      - in: query
        name: MaxRecords
        description: Specifies the maximum number of events that can be returned,
          beginning with the most      recent event
        type: string
      - in: query
        name: NextToken
        description: Pagination token
        type: string
      - in: query
        name: RequestId
        description: If specified, AWS Elastic Beanstalk restricts the described events
          to include only      those associated with this request ID
        type: string
      - in: query
        name: Severity
        description: If specified, limits the events returned from this call to include
          only those with the      specified severity or higher
        type: string
      - in: query
        name: StartTime
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those that      occur on or after this time
        type: string
      - in: query
        name: TemplateName
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those that      are associated with this environment configuration
        type: string
      - in: query
        name: VersionLabel
        description: If specified, AWS Elastic Beanstalk restricts the returned descriptions
          to those      associated with this application version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
  /?Action=DescribeInstancesHealth:
    get:
      summary: Describe Instances Health
      description: |-
        Retrives detailed information about the health of instances in your AWS Elastic
              Beanstalk.
      operationId: describeInstancesHealth
      x-api-path-slug: actiondescribeinstanceshealth-get
      parameters:
      - in: query
        name: AttributeNames.member.N
        description: Specifies the response elements you wish to receive
        type: string
      - in: query
        name: EnvironmentId
        description: Specify the AWS Elastic Beanstalk environment by ID
        type: string
      - in: query
        name: EnvironmentName
        description: Specify the AWS Elastic Beanstalk environment by name
        type: string
      - in: query
        name: NextToken
        description: Specify the pagination token returned by a previous call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances Health
  /?Action=ListAvailableSolutionStacks:
    get:
      summary: List Available Solution Stacks
      description: Returns a list of the available solution stack names.
      operationId: listAvailableSolutionStacks
      x-api-path-slug: actionlistavailablesolutionstacks-get
      parameters:
      - in: query
        name: SolutionStackDetails.member.N
        description: A list of available solution stacks and their SolutionStackDescription
        type: string
      - in: query
        name: SolutionStacks.member.N
        description: A list of available solution stacks
        type: string
      responses:
        200:
          description: OK
      tags:
      - Solution Stacks
  /?Action=RebuildEnvironment:
    get:
      summary: Rebuild Environment
      description: |-
        Deletes and recreates all of the AWS resources (for example: the Auto Scaling group,
              load balancer, etc.
      operationId: rebuildEnvironment
      x-api-path-slug: actionrebuildenvironment-get
      parameters:
      - in: query
        name: EnvironmentId
        description: The ID of the environment to rebuild
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment to rebuild
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=RequestEnvironmentInfo:
    get:
      summary: Request Environment Info
      description: |-
        Initiates a request to compile the specified type of information of the deployed
              environment.
      operationId: requestEnvironmentInfo
      x-api-path-slug: actionrequestenvironmentinfo-get
      parameters:
      - in: query
        name: EnvironmentId
        description: The ID of the environment of the requested data
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment of the requested data
        type: string
      - in: query
        name: InfoType
        description: The type of information to request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=RestartAppServer:
    get:
      summary: Restart App Server
      description: |-
        Causes the environment to restart the application container server running on each
              Amazon EC2 instance.
      operationId: restartAppServer
      x-api-path-slug: actionrestartappserver-get
      parameters:
      - in: query
        name: EnvironmentId
        description: The ID of the environment to restart the server for
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment to restart the server for
        type: string
      responses:
        200:
          description: OK
      tags:
      - App Servers
  /?Action=RetrieveEnvironmentInfo:
    get:
      summary: Retrieve Environment Info
      description: Retrieves the compiled information from a.
      operationId: retrieveEnvironmentInfo
      x-api-path-slug: actionretrieveenvironmentinfo-get
      parameters:
      - in: query
        name: EnvironmentId
        description: The ID of the datas environment
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the datas environment
        type: string
      - in: query
        name: InfoType
        description: The type of information to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=SwapEnvironmentCNAMEs:
    get:
      summary: Swap Environment C N A M Es
      description: Swaps the CNAMEs of two environments.
      operationId: swapEnvironmentCNAMEs
      x-api-path-slug: actionswapenvironmentcnames-get
      parameters:
      - in: query
        name: DestinationEnvironmentId
        description: The ID of the destination environment
        type: string
      - in: query
        name: DestinationEnvironmentName
        description: The name of the destination environment
        type: string
      - in: query
        name: SourceEnvironmentId
        description: The ID of the source environment
        type: string
      - in: query
        name: SourceEnvironmentName
        description: The name of the source environment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=TerminateEnvironment:
    get:
      summary: Terminate Environment
      description: Terminates the specified environment.
      operationId: terminateEnvironment
      x-api-path-slug: actionterminateenvironment-get
      parameters:
      - in: query
        name: EnvironmentId
        description: The ID of the environment to terminate
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment to terminate
        type: string
      - in: query
        name: ForceTerminate
        description: Terminates the target environment even if another environment
          in the same group is      dependent on it
        type: string
      - in: query
        name: TerminateResources
        description: 'Indicates whether the associated AWS resources should shut down
          when the environment is      terminated:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=UpdateApplication:
    get:
      summary: Update Application
      description: Updates the specified application to have the specified properties.
      operationId: updateApplication
      x-api-path-slug: actionupdateapplication-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application to update
        type: string
      - in: query
        name: Description
        description: A new description for the application
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=UpdateApplicationResourceLifecycle:
    get:
      summary: Update Application Resource Lifecycle
      description: Modifies lifecycle settings for an application.
      operationId: updateApplicationResourceLifecycle
      x-api-path-slug: actionupdateapplicationresourcelifecycle-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application
        type: string
      - in: query
        name: ResourceLifecycleConfig
        description: The lifecycle configuration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Application Resource Lifecycle
  /?Action=UpdateApplicationVersion:
    get:
      summary: Update Application Version
      description: Updates the specified application version to have the specified
        properties.
      operationId: updateApplicationVersion
      x-api-path-slug: actionupdateapplicationversion-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application associated with this version
        type: string
      - in: query
        name: Description
        description: A new description for this version
        type: string
      - in: query
        name: VersionLabel
        description: The name of the version to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=UpdateConfigurationTemplate:
    get:
      summary: Update Configuration Template
      description: |-
        Updates the specified configuration template to have the specified properties or
              configuration option values.
      operationId: updateConfigurationTemplate
      x-api-path-slug: actionupdateconfigurationtemplate-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application associated with the configuration
          template to      update
        type: string
      - in: query
        name: Description
        description: A new description for the configuration
        type: string
      - in: query
        name: OptionSettings.member.N
        description: A list of configuration option settings to update with the new
          specified option      value
        type: string
      - in: query
        name: OptionsToRemove.member.N
        description: A list of configuration options to remove from the configuration
          set
        type: string
      - in: query
        name: TemplateName
        description: The name of the configuration template to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Templates
  /?Action=UpdateEnvironment:
    get:
      summary: Update Environment
      description: |-
        Updates the environment description, deploys a new application version, updates the
              configuration settings to an entirely new configuration template, or updates select
              configuration option values in the running environment.
      operationId: updateEnvironment
      x-api-path-slug: actionupdateenvironment-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application with which the environment is associated
        type: string
      - in: query
        name: Description
        description: If this parameter is specified, AWS Elastic Beanstalk updates
          the description of this      environment
        type: string
      - in: query
        name: EnvironmentId
        description: The ID of the environment to update
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment to update
        type: string
      - in: query
        name: GroupName
        description: The name of the group to which the target environment belongs
        type: string
      - in: query
        name: OptionSettings.member.N
        description: If specified, AWS Elastic Beanstalk updates the configuration
          set associated with the      running environment and sets the specified
          configuration options to the requested      value
        type: string
      - in: query
        name: OptionsToRemove.member.N
        description: A list of custom user-defined configuration options to remove
          from the configuration      set for this environment
        type: string
      - in: query
        name: SolutionStackName
        description: This specifies the platform version that the environment will
          run after the environment      is updated
        type: string
      - in: query
        name: TemplateName
        description: If this parameter is specified, AWS Elastic Beanstalk deploys
          this configuration      template to the environment
        type: string
      - in: query
        name: Tier
        description: This specifies the tier to use to update the environment
        type: string
      - in: query
        name: VersionLabel
        description: If this parameter is specified, AWS Elastic Beanstalk deploys
          the named application      version to the environment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments
  /?Action=ValidateConfigurationSettings:
    get:
      summary: Validate Configuration Settings
      description: |-
        Takes a set of configuration settings and either a configuration template or
              environment, and determines whether those values are valid.
      operationId: validateConfigurationSettings
      x-api-path-slug: actionvalidateconfigurationsettings-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application that the configuration template or
          environment belongs      to
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment to validate the settings against
        type: string
      - in: query
        name: OptionSettings.member.N
        description: A list of the options and desired values to evaluate
        type: string
      - in: query
        name: TemplateName
        description: The name of the configuration template to validate the settings
          against
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Settings