swagger: "2.0"
x-collection-name: AWS AppStream
x-complete: 1
info:
  title: AWS AppStream 2.0 API
  description: amazon-appstream-2-0-is-a-fully-managed-secure-application-streaming-service-that-allows-you-to-stream-desktop-applications-from-aws-to-any-device-running-a-web-browser-without-rewriting-them--amazon-appstream-2-0-provides-users-instanton-access-to-the-applications-they-need-and-a-responsive-fluid-user-experience-on-the-device-of-their-choice-
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AssociateFleet:
    get:
      summary: Associate Fleet
      description: Associate a fleet to a stack.
      operationId: AssociateFleet
      x-api-path-slug: actionassociatefleet-get
      parameters:
      - in: query
        name: FleetName
        description: The name of the fleet to associate
        type: string
      - in: query
        name: StackName
        description: The name of the stack to which the fleet is associated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Fleet
  /?Action=CreateFleet:
    get:
      summary: Create Fleet
      description: Creates a new fleet.
      operationId: CreateFleet
      x-api-path-slug: actioncreatefleet-get
      parameters:
      - in: query
        name: ComputeCapacity
        description: The parameters for the capacity allocated to the fleet
        type: string
      - in: query
        name: Description
        description: The description of the fleet
        type: string
      - in: query
        name: DisconnectTimeoutInSeconds
        description: The time after disconnection when a session is considered to
          have ended
        type: string
      - in: query
        name: DisplayName
        description: The display name of the fleet
        type: string
      - in: query
        name: ImageName
        description: Unique name of the image used by the fleet
        type: string
      - in: query
        name: InstanceType
        description: The instance type of compute resources for the fleet
        type: string
      - in: query
        name: MaxUserDurationInSeconds
        description: The maximum time up to which a streaming session can run
        type: string
      - in: query
        name: Name
        description: A unique identifier for the fleet
        type: string
      - in: query
        name: VpcConfig
        description: The VPC configuration for the fleet
        type: string
      responses:
        200:
          description: OK
      tags:
      - Fleet
  /?Action=CreateStack:
    get:
      summary: Create Stack
      description: Create a new stack.
      operationId: CreateStack
      x-api-path-slug: actioncreatestack-get
      parameters:
      - in: query
        name: Description
        description: The description displayed to end users on the AppStream 2
        type: string
      - in: query
        name: DisplayName
        description: The name displayed to end users on the AppStream 2
        type: string
      - in: query
        name: Name
        description: The unique identifier for this stack
        type: string
      responses:
        200:
          description: OK
      tags:
      - Fleet
  /?Action=CreateStreamingURL:
    get:
      summary: Create Streaming URL
      description: Creates a URL to start an AppStream 2.
      operationId: CreateStreamingURL
      x-api-path-slug: actioncreatestreamingurl-get
      parameters:
      - in: query
        name: ApplicationId
        description: The ID of the application that must be launched after the session
          starts
        type: string
      - in: query
        name: FleetName
        description: The fleet for which the URL is generated
        type: string
      - in: query
        name: SessionContext
        description: The sessionContext of the streaming URL
        type: string
      - in: query
        name: StackName
        description: The stack for which the URL is generated
        type: string
      - in: query
        name: UserId
        description: A unique user ID for whom the URL is generated
        type: string
      - in: query
        name: Validity
        description: The validity duration of the URL in seconds
        type: string
      responses:
        200:
          description: OK
      tags:
      - URL
  /?Action=DeleteFleet:
    get:
      summary: Delete Fleet
      description: Deletes a fleet.
      operationId: DeleteFleet
      x-api-path-slug: actiondeletefleet-get
      parameters:
      - in: query
        name: Name
        description: The name of the fleet to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Fleet
  /?Action=DeleteStack:
    get:
      summary: Delete Stack
      description: Deletes the stack.
      operationId: DeleteStack
      x-api-path-slug: actiondeletestack-get
      parameters:
      - in: query
        name: Name
        description: The name of the stack to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack
  /?Action=DescribeFleets:
    get:
      summary: Describe Fleets
      description: |-
        If fleet names are provided, this operation describes the specified fleets;
                    otherwise, all the fleets in the account are described.
      operationId: DescribeFleets
      x-api-path-slug: actiondescribefleets-get
      parameters:
      - in: query
        name: Names
        description: The fleet names to describe
        type: string
      - in: query
        name: NextToken
        description: The pagination token to use to retrieve the next page of results
          for this operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Fleet
  /?Action=DescribeImages:
    get:
      summary: Describe Images
      description: Describes the images.
      operationId: DescribeImages
      x-api-path-slug: actiondescribeimages-get
      parameters:
      - in: query
        name: Names
        description: A specific list of images to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Images
  /?Action=DescribeSessions:
    get:
      summary: Describe Sessions
      description: Describes the streaming sessions for a stack and a fleet.
      operationId: DescribeSessions
      x-api-path-slug: actiondescribesessions-get
      parameters:
      - in: query
        name: FleetName
        description: The name of the fleet for which to list sessions
        type: string
      - in: query
        name: Limit
        description: The size of each page of results
        type: string
      - in: query
        name: NextToken
        description: The pagination token to use to retrieve the next page of results
          for this operation
        type: string
      - in: query
        name: StackName
        description: The name of the stack for which to list sessions
        type: string
      - in: query
        name: UserId
        description: The user for whom to list sessions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Sessions
  /?Action=DescribeStacks:
    get:
      summary: Describe Stacks
      description: |-
        If stack names are not provided, this operation describes the specified stacks;
                    otherwise, all stacks in the account are described.
      operationId: DescribeStacks
      x-api-path-slug: actiondescribestacks-get
      parameters:
      - in: query
        name: Names
        description: The stack names to describe
        type: string
      - in: query
        name: NextToken
        description: The pagination token to use to retrieve the next page of results
          for this operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stacks
  /?Action=DisassociateFleet:
    get:
      summary: Disassociate Fleet
      description: Disassociates a fleet from a stack.
      operationId: DisassociateFleet
      x-api-path-slug: actiondisassociatefleet-get
      parameters:
      - in: query
        name: FleetName
        description: The name of the fleet to disassociate
        type: string
      - in: query
        name: StackName
        description: The name of the stack with which the fleet is associated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Fleet
  /?Action=ExpireSession:
    get:
      summary: Expire Session
      description: This operation immediately stops a streaming session.
      operationId: ExpireSession
      x-api-path-slug: actionexpiresession-get
      parameters:
      - in: query
        name: SessionId
        description: The unique identifier of the streaming session to be stopped
        type: string
      responses:
        200:
          description: OK
      tags:
      - Session
  /?Action=ListAssociatedFleets:
    get:
      summary: List Associated Fleets
      description: Lists all fleets associated with the stack.
      operationId: ListAssociatedFleets
      x-api-path-slug: actionlistassociatedfleets-get
      parameters:
      - in: query
        name: NextToken
        description: The pagination token to use to retrieve the next page of results
          for this operation
        type: string
      - in: query
        name: StackName
        description: The name of the stack whose associated fleets are listed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Fleet
  /?Action=ListAssociatedStacks:
    get:
      summary: List Associated Stacks
      description: Lists all stacks to which the specified fleet is associated.
      operationId: ListAssociatedStacks
      x-api-path-slug: actionlistassociatedstacks-get
      parameters:
      - in: query
        name: FleetName
        description: The name of the fleet whose associated stacks are listed
        type: string
      - in: query
        name: NextToken
        description: The pagination token to use to retrieve the next page of results
          for this operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack
  /?Action=StartFleet:
    get:
      summary: Start Fleet
      description: Starts a fleet.
      operationId: StartFleet
      x-api-path-slug: actionstartfleet-get
      parameters:
      - in: query
        name: Name
        description: The name of the fleet to start
        type: string
      responses:
        200:
          description: OK
      tags:
      - Fleet
  /?Action=StopFleet:
    get:
      summary: Stop Fleet
      description: Stops a fleet.
      operationId: StopFleet
      x-api-path-slug: actionstopfleet-get
      parameters:
      - in: query
        name: Name
        description: The name of the fleet to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Fleet
  /?Action=UpdateFleet:
    get:
      summary: Update Fleet
      description: Updates an existing fleet.
      operationId: UpdateFleet
      x-api-path-slug: actionupdatefleet-get
      parameters:
      - in: query
        name: ComputeCapacity
        description: The parameters for the capacity allocated to the fleet
        type: string
      - in: query
        name: DeleteVpcConfig
        description: Delete the VPC association for the specified fleet
        type: string
      - in: query
        name: Description
        description: The description displayed to end users on the AppStream 2
        type: string
      - in: query
        name: DisconnectTimeoutInSeconds
        description: The time after disconnection when a session is considered to
          have ended
        type: string
      - in: query
        name: DisplayName
        description: The name displayed to end users on the AppStream 2
        type: string
      - in: query
        name: ImageName
        description: The image name from which a fleet is created
        type: string
      - in: query
        name: InstanceType
        description: The instance type of compute resources for the fleet
        type: string
      - in: query
        name: MaxUserDurationInSeconds
        description: The maximum time during which a streaming session can run
        type: string
      - in: query
        name: Name
        description: The name of the fleet
        type: string
      - in: query
        name: VpcConfig
        description: The VPC configuration for the fleet
        type: string
      responses:
        200:
          description: OK
      tags:
      - Fleet
  /?Action=UpdateStack:
    get:
      summary: Update Stack
      description: Updates the specified fields in the stack with the specified name.
      operationId: UpdateStack
      x-api-path-slug: actionupdatestack-get
      parameters:
      - in: query
        name: Description
        description: The description displayed to end users on the AppStream 2
        type: string
      - in: query
        name: DisplayName
        description: The name displayed to end users on the AppStream 2
        type: string
      - in: query
        name: Name
        description: The name of the stack to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stack