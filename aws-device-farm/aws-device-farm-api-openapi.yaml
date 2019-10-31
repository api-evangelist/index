swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 1
info:
  title: AWS Device Farm API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateDevicePool:
    get:
      summary: Create Device Pool
      description: Creates a device pool.
      operationId: createDevicePool
      x-api-path-slug: actioncreatedevicepool-get
      parameters:
      - in: query
        name: description
        description: The device pools description
        type: string
      - in: query
        name: name
        description: The device pools name
        type: string
      - in: query
        name: projectArn
        description: The ARN of the project for the device pool
        type: string
      - in: query
        name: rules
        description: The device pools rules
        type: string
      responses:
        200:
          description: OK
      tags:
      - Device Pool
  /?Action=CreateProject:
    get:
      summary: Create Project
      description: Creates a new project.
      operationId: createProject
      x-api-path-slug: actioncreateproject-get
      parameters:
      - in: query
        name: name
        description: The projects name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Project
  /?Action=CreateRemoteAccessSession:
    get:
      summary: Create Remote Access Session
      description: Specifies and starts a remote access session.
      operationId: createRemoteAccessSession
      x-api-path-slug: actioncreateremoteaccesssession-get
      parameters:
      - in: query
        name: configuration
        description: The configuration information for the remote access session request
        type: string
      - in: query
        name: deviceArn
        description: The Amazon Resource Name (ARN) of the device for which you want
          to create a remote access session
        type: string
      - in: query
        name: name
        description: The name of the remote access session that you wish to create
        type: string
      - in: query
        name: projectArn
        description: The Amazon Resource Name (ARN) of the project for which you want
          to create a remote access session
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remote Access Sessions
  /?Action=CreateUpload:
    get:
      summary: Create Upload
      description: Uploads an app or test scripts.
      operationId: createUpload
      x-api-path-slug: actioncreateupload-get
      parameters:
      - in: query
        name: contentType
        description: The uploads content type (for example, application/octet-stream)
        type: string
      - in: query
        name: name
        description: The uploads file name
        type: string
      - in: query
        name: projectArn
        description: The ARN of the project for the upload
        type: string
      - in: query
        name: type
        description: The uploads upload type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload
  /?Action=DeleteDevicePool:
    get:
      summary: Delete Device Pool
      description: Deletes a device pool given the pool ARN.
      operationId: deleteDevicePool
      x-api-path-slug: actiondeletedevicepool-get
      parameters:
      - in: query
        name: arn
        description: Represents the Amazon Resource Name (ARN) of the Device Farm
          device pool you wish to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Device Pool
  /?Action=DeleteProject:
    get:
      summary: Delete Project
      description: Deletes an AWS Device Farm project, given the project ARN.
      operationId: deleteProject
      x-api-path-slug: actiondeleteproject-get
      parameters:
      - in: query
        name: arn
        description: Represents the Amazon Resource Name (ARN) of the Device Farm
          project you wish to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Projects
  /?Action=DeleteRemoteAccessSession:
    get:
      summary: Delete Remote Access Session
      description: Deletes a completed remote access session and its results.
      operationId: deleteRemoteAccessSession
      x-api-path-slug: actiondeleteremoteaccesssession-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the sesssion for which you
          want to delete remote access
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remote Access Sessions
  /?Action=DeleteRun:
    get:
      summary: Delete Run
      description: Deletes the run, given the run ARN.
      operationId: deleteRun
      x-api-path-slug: actiondeleterun-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) for the run you wish to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Runs
  /?Action=DeleteUpload:
    get:
      summary: Delete Upload
      description: Deletes an upload given the upload ARN.
      operationId: deleteUpload
      x-api-path-slug: actiondeleteupload-get
      parameters:
      - in: query
        name: arn
        description: Represents the Amazon Resource Name (ARN) of the Device Farm
          upload you wish to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Uploads
  /?Action=GetAccountSettings:
    get:
      summary: Get Account Settings
      description: Returns the number of unmetered iOS and/or unmetered Android devices
        that have been purchased by the account.
      operationId: getAccountSettings
      x-api-path-slug: actiongetaccountsettings-get
      parameters:
      - in: query
        name: accountSettings
        description: A container for account-level settings within AWS Device Farm
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Settings
  /?Action=GetDevice:
    get:
      summary: Get Device
      description: Gets information about a unique device type.
      operationId: getDevice
      x-api-path-slug: actiongetdevice-get
      parameters:
      - in: query
        name: arn
        description: The device types ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Devices
  /?Action=GetDevicePool:
    get:
      summary: Get Device Pool
      description: Gets information about a device pool.
      operationId: getDevicePool
      x-api-path-slug: actiongetdevicepool-get
      parameters:
      - in: query
        name: arn
        description: The device pools ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Device Pool
  /?Action=GetDevicePoolCompatibility:
    get:
      summary: Get Device Pool Compatibility
      description: Gets information about compatibility with a device pool.
      operationId: getDevicePoolCompatibility
      x-api-path-slug: actiongetdevicepoolcompatibility-get
      parameters:
      - in: query
        name: appArn
        description: The ARN of the app that is associated with the specified device
          pool
        type: string
      - in: query
        name: devicePoolArn
        description: The device pools ARN
        type: string
      - in: query
        name: testType
        description: The test type for the specified device pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Device Pool
  /?Action=GetJob:
    get:
      summary: Get Job
      description: Gets information about a job.
      operationId: getJob
      x-api-path-slug: actiongetjob-get
      parameters:
      - in: query
        name: arn
        description: The jobs ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs
  /?Action=GetOfferingStatus:
    get:
      summary: Get Offering Status
      description: Gets the current status and future status of all offerings purchased
        by an AWS account.
      operationId: getOfferingStatus
      x-api-path-slug: actiongetofferingstatus-get
      parameters:
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Offering Status
  /?Action=GetProject:
    get:
      summary: Get Project
      description: Gets information about a project.
      operationId: getProject
      x-api-path-slug: actiongetproject-get
      parameters:
      - in: query
        name: arn
        description: The projects ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Projects
  /?Action=GetRemoteAccessSession:
    get:
      summary: Get Remote Access Session
      description: Returns a link to a currently running remote access session.
      operationId: getRemoteAccessSession
      x-api-path-slug: actiongetremoteaccesssession-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the remote access session about
          which you want to get session information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remote Access Sessions
  /?Action=GetRun:
    get:
      summary: Get Run
      description: Gets information about a run.
      operationId: getRun
      x-api-path-slug: actiongetrun-get
      parameters:
      - in: query
        name: arn
        description: The runs ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Runs
  /?Action=GetSuite:
    get:
      summary: Get Suite
      description: Gets information about a suite.
      operationId: getSuite
      x-api-path-slug: actiongetsuite-get
      parameters:
      - in: query
        name: arn
        description: The suites ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Suites
  /?Action=GetTest:
    get:
      summary: Get Test
      description: Gets information about a test.
      operationId: getTest
      x-api-path-slug: actiongettest-get
      parameters:
      - in: query
        name: arn
        description: The tests ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tests
  /?Action=GetUpload:
    get:
      summary: Get Upload
      description: Gets information about an upload.
      operationId: getUpload
      x-api-path-slug: actiongetupload-get
      parameters:
      - in: query
        name: arn
        description: The uploads ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Upload
  /?Action=InstallToRemoteAccessSession:
    get:
      summary: Install To Remote Access Session
      description: Installs an application to the device in a remote access session.
      operationId: installToRemoteAccessSession
      x-api-path-slug: actioninstalltoremoteaccesssession-get
      parameters:
      - in: query
        name: appArn
        description: The Amazon Resource Name (ARN) of the app about which you are
          requesting information
        type: string
      - in: query
        name: remoteAccessSessionArn
        description: The Amazon Resource Name (ARN) of the remote access session about
          which you are requesting information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remote Access Sessions
  /?Action=ListArtifacts:
    get:
      summary: List Artifacts
      description: Gets information about artifacts.
      operationId: listArtifacts
      x-api-path-slug: actionlistartifacts-get
      parameters:
      - in: query
        name: arn
        description: The Run, Job, Suite, or Test ARN
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      - in: query
        name: type
        description: The artifacts type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Artifacts
  /?Action=ListDevicePools:
    get:
      summary: List Device Pools
      description: Gets information about device pools.
      operationId: listDevicePools
      x-api-path-slug: actionlistdevicepools-get
      parameters:
      - in: query
        name: arn
        description: The project ARN
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      - in: query
        name: type
        description: The device pools type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Device Pool
  /?Action=ListDevices:
    get:
      summary: List Devices
      description: Gets information about unique device types.
      operationId: listDevices
      x-api-path-slug: actionlistdevices-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the project
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Devices
  /?Action=ListJobs:
    get:
      summary: List Jobs
      description: Gets information about jobs.
      operationId: listJobs
      x-api-path-slug: actionlistjobs-get
      parameters:
      - in: query
        name: arn
        description: The jobs ARNs
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Jobs
  /?Action=ListOfferings:
    get:
      summary: List Offerings
      description: Returns a list of products or offerings that the user can manage
        through the API.
      operationId: listOfferings
      x-api-path-slug: actionlistofferings-get
      parameters:
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Offerings
  /?Action=ListOfferingTransactions:
    get:
      summary: List Offering Transactions
      description: |-
        Returns a list of all historical purchases, renewals, and system renewal transactions for an
              AWS account.
      operationId: listOfferingTransactions
      x-api-path-slug: actionlistofferingtransactions-get
      parameters:
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Offering Transactions
  /?Action=ListProjects:
    get:
      summary: List Projects
      description: Gets information about projects.
      operationId: listProjects
      x-api-path-slug: actionlistprojects-get
      parameters:
      - in: query
        name: arn
        description: Optional
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Projects
  /?Action=ListRemoteAccessSessions:
    get:
      summary: List Remote Access Sessions
      description: Returns a list of all currently running remote access sessions.
      operationId: listRemoteAccessSessions
      x-api-path-slug: actionlistremoteaccesssessions-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the remote access session about
          which you are requesting information
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remote Access Sessions
  /?Action=ListRuns:
    get:
      summary: List Runs
      description: Gets information about runs, given an AWS Device Farm project ARN.
      operationId: listRuns
      x-api-path-slug: actionlistruns-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the project for which you want
          to list runs
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Runs
  /?Action=ListSamples:
    get:
      summary: List Samples
      description: Gets information about samples, given an AWS Device Farm project
        ARN.
      operationId: listSamples
      x-api-path-slug: actionlistsamples-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the project for which you want
          to list samples
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Samples
  /?Action=ListSuites:
    get:
      summary: List Suites
      description: Gets information about suites.
      operationId: listSuites
      x-api-path-slug: actionlistsuites-get
      parameters:
      - in: query
        name: arn
        description: The suites ARNs
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Suites
  /?Action=ListTests:
    get:
      summary: List Tests
      description: Gets information about tests.
      operationId: listTests
      x-api-path-slug: actionlisttests-get
      parameters:
      - in: query
        name: arn
        description: The tests ARNs
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tests
  /?Action=ListUniqueProblems:
    get:
      summary: List Unique Problems
      description: Gets information about unique problems.
      operationId: listUniqueProblems
      x-api-path-slug: actionlistuniqueproblems-get
      parameters:
      - in: query
        name: arn
        description: The unique problems ARNs
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Unique Problems
  /?Action=ListUploads:
    get:
      summary: List Uploads
      description: Gets information about uploads, given an AWS Device Farm project
        ARN.
      operationId: listUploads
      x-api-path-slug: actionlistuploads-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the project for which you want
          to list uploads
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Uploads
  /?Action=PurchaseOffering:
    get:
      summary: Purchase Offering
      description: Immediately purchases offerings for an AWS account.
      operationId: purchaseOffering
      x-api-path-slug: actionpurchaseoffering-get
      parameters:
      - in: query
        name: offeringId
        description: The ID of the offering
        type: string
      - in: query
        name: quantity
        description: The number of device slots you wish to purchase in an offering
          request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Offerings
  /?Action=RenewOffering:
    get:
      summary: Renew Offering
      description: |-
        Explicitly sets the quantity of devices to renew for an offering, starting from the
              effectiveDate of the next period.
      operationId: renewOffering
      x-api-path-slug: actionrenewoffering-get
      parameters:
      - in: query
        name: offeringId
        description: The ID of a request to renew an offering
        type: string
      - in: query
        name: quantity
        description: The quantity requested in an offering renewal
        type: string
      responses:
        200:
          description: OK
      tags:
      - Offerings
  /?Action=ScheduleRun:
    get:
      summary: Schedule Run
      description: Schedules a run.
      operationId: scheduleRun
      x-api-path-slug: actionschedulerun-get
      parameters:
      - in: query
        name: appArn
        description: The ARN of the app to schedule a run
        type: string
      - in: query
        name: configuration
        description: Information about the settings for the run to be scheduled
        type: string
      - in: query
        name: devicePoolArn
        description: The ARN of the device pool for the run to be scheduled
        type: string
      - in: query
        name: name
        description: The name for the run to be scheduled
        type: string
      - in: query
        name: projectArn
        description: The ARN of the project for the run to be scheduled
        type: string
      - in: query
        name: test
        description: Information about the test for the run to be scheduled
        type: string
      responses:
        200:
          description: OK
      tags:
      - Runs
  /?Action=StopRemoteAccessSession:
    get:
      summary: Stop Remote Access Session
      description: Ends a specified remote access session.
      operationId: stopRemoteAccessSession
      x-api-path-slug: actionstopremoteaccesssession-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the remote access session you
          wish to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Remote Access Sessions
  /?Action=StopRun:
    get:
      summary: Stop Run
      description: Initiates a stop request for the current test run.
      operationId: stopRun
      x-api-path-slug: actionstoprun-get
      parameters:
      - in: query
        name: arn
        description: Represents the Amazon Resource Name (ARN) of the Device Farm
          run you wish to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Runs
  /?Action=UpdateDevicePool:
    get:
      summary: Update Device Pool
      description: Modifies the name, description, and rules in a device pool given
        the attributes and the pool ARN.
      operationId: updateDevicePool
      x-api-path-slug: actionupdatedevicepool-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resourc Name (ARN) of the Device Farm device pool
          you wish to update
        type: string
      - in: query
        name: description
        description: A description of the device pool you wish to update
        type: string
      - in: query
        name: name
        description: A string representing the name of the device pool you wish to
          update
        type: string
      - in: query
        name: rules
        description: Represents the rules you wish to modify for the device pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Device Pool
  /?Action=UpdateProject:
    get:
      summary: Update Project
      description: Modifies the specified project name, given the project ARN and
        a new name.
      operationId: updateProject
      x-api-path-slug: actionupdateproject-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the project whose name you
          wish to update
        type: string
      - in: query
        name: name
        description: A string representing the new name of the project that you are
          updating
        type: string
      responses:
        200:
          description: OK
      tags:
      - Projects