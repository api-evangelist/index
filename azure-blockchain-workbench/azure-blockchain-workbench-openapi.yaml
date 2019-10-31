swagger: "2.0"
x-collection-name: Azure Blockchain Workbench
x-complete: 1
info:
  title: Azure Blockchain Workbench REST API
  description: the-azure-blockchain-workbench-rest-api-is-a-workbench-extensibility-point-which-allows-developers-to-create-and-manage-blockchain-applications-manage-users-and-organizations-within-a-consortium-integrate-blockchain-applications-into-services-and-platforms-perform-transactions-on-a-blockchain-and-retrieve-transactional-and-contract-data-from-a-blockchain-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/applications:
    get:
      summary: Get Applications
      description: |-
        Lists all blockchain applications to which a user has access in Workbench. Users who are Workbench administrators get
                     all blockchain applications. Non-Workbench administrators get all blockchain applications for which they have at least one
                     associated application role or an associated smart contract instance role.
      operationId: ApplicationsGet
      x-api-path-slug: apiv1applications-get
      parameters:
      - in: query
        name: enabled
        description: A Boolean for whether to filter the result set to only enabled
          applications
      - in: query
        name: skip
        description: The number of entries to skip in the result set
      - in: query
        name: sortBy
        description: The field to sort
      - in: query
        name: top
        description: The maximum number of entries to return in the result set
      responses:
        200:
          description: OK
      tags:
      - Applications
    post:
      summary: Post Applications
      description: |-
        Creates a new blockchain application. This method can only be performed by users who are
                     Workbench administrators.
      operationId: ApplicationsPost
      x-api-path-slug: apiv1applications-post
      parameters:
      - in: formData
        name: appFile
        description: Upload Application File
      responses:
        200:
          description: OK
      tags:
      - Applications
  /api/v1/applications/{applicationId}:
    get:
      summary: Get Applications
      description: |-
        Gets the blockchain application matching a specific application ID. Users who are Workbench administrators get
                     the blockchain application. Non-Workbench administrators get the blockchain application if they have at least one associated
                     application role or is associated with a smart contract instance role.
      operationId: ApplicationGet
      x-api-path-slug: apiv1applicationsapplicationid-get
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      responses:
        200:
          description: OK
      tags:
      - Applications
    delete:
      summary: Delete Applications
      description: |-
        Deletes the specified blockchain application. This method can only be performed by users who are
                     Workbench administrators. NOTE: Currently not implemented.
      operationId: ApplicationDelete
      x-api-path-slug: apiv1applicationsapplicationid-delete
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      responses:
        200:
          description: OK
      tags:
      - Applications
  /api/v1/applications/{applicationId}/enable:
    patch:
      summary: Patch Applications Enable
      description: |-
        Enables the specified blockchain application. This method can only be performed by users who are
                     Workbench administrators.
      operationId: ApplicationEnable
      x-api-path-slug: apiv1applicationsapplicationidenable-patch
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Enable
  /api/v1/applications/{applicationId}/disable:
    patch:
      summary: Patch Applications Disable
      description: |-
        Disables the specified blockchain application. This method can only be performed by users who are
                     Workbench administrators.
      operationId: ApplicationDisable
      x-api-path-slug: apiv1applicationsapplicationiddisable-patch
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Disable
  /api/v1/applications/{applicationId}/roleAssignments:
    get:
      summary: Get Applications Roleassignments
      description: |-
        List all role assignments of the specified blockchain application. Users who are Workbench administrators
                     get all role assignments. Non-Workbench administrators get all their role assignments. Roles are specified
                     in the Workbench application configuration and can be retrieved from GET /applications/{applicationID}.
                     Also, user information can be retrieved from GET /users/{userID}.
      operationId: RoleAssignmentsGet
      x-api-path-slug: apiv1applicationsapplicationidroleassignments-get
      parameters:
      - in: path
        name: applicationId
        description: The id of the configuration
      - in: query
        name: applicationRoleId
        description: The id of the application role
      - in: query
        name: skip
        description: The number of entries to skip in the result set
      - in: query
        name: sortBy
        description: The field to sort
      - in: query
        name: top
        description: The maximum number of entries to return in the result set
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Roleassignments
    post:
      summary: Post Applications Roleassignments
      description: |-
        Creates a user-to-role mapping in the specified blockchain application. This method can only be performed by
                     users who are Workbench administrators.
      operationId: RoleAssignmentsPost
      x-api-path-slug: apiv1applicationsapplicationidroleassignments-post
      parameters:
      - in: path
        name: applicationId
        description: The id of the configuration
      - in: body
        name: roleAssignment
        description: New user-to-role mapping
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Roleassignments
  /api/v1/applications/{applicationId}/roleAssignments/{roleAssignmentId}:
    get:
      summary: Get Applications Roleassignments Roleassignmentid
      description: |-
        Get a role assignment of the specified blockchain application matching a specific user role assignment ID.
                     Users who are Workbench administrators get the role assignment. Non-Workbench administrators get the role assignment
                     if they are associated in the application.
      operationId: RoleAssignmentGet
      x-api-path-slug: apiv1applicationsapplicationidroleassignmentsroleassignmentid-get
      parameters:
      - in: path
        name: applicationId
        description: The id of the configuration
      - in: path
        name: roleAssignmentId
        description: The id of the role assignment
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Roleassignments
      - Roleassignmentid
    put:
      summary: Put Applications Roleassignments Roleassignmentid
      description: Updates the specified role assignment. This method can only be
        performed by users who are Workbench administrators.
      operationId: RoleAssignmentPut
      x-api-path-slug: apiv1applicationsapplicationidroleassignmentsroleassignmentid-put
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      - in: body
        name: roleAssignment
        description: New user-to-role mapping parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: roleAssignmentId
        description: The id of the user-to-role mapping
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Roleassignments
      - Roleassignmentid
    delete:
      summary: Delete Applications Roleassignments Roleassignmentid
      description: |-
        Deletes the specified role assignment. This method can only be performed by users who are
                     Workbench administrators.
      operationId: RoleAssignmentDelete
      x-api-path-slug: apiv1applicationsapplicationidroleassignmentsroleassignmentid-delete
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      - in: path
        name: roleAssignmentId
        description: The id of the role assignment
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Roleassignments
      - Roleassignmentid
  /api/v1/applications/{applicationId}/workflows:
    get:
      summary: Get Applications Workflows
      description: |-
        List all workflows of the specified blockchain application. Users who are Workbench administrators get all
                     workflows. Non-Workbench administrators get all workflows for which they have at least one associated application role
                     or are associated with a smart contract instance role.
      operationId: WorkflowsGet
      x-api-path-slug: apiv1applicationsapplicationidworkflows-get
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      - in: query
        name: skip
        description: The number of items to skip before returning
      - in: query
        name: top
        description: The maximum number of items to return
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Workflows
  /api/v1/applications/workflows/{workflowId}:
    get:
      summary: Get Applications Workflows
      description: |-
        Get a workflow matching a specific workflow ID.
                     Users who are Workbench administrators get the workflow. Non-Workbench administrators get the workflow if they
                     have at least one associated application role or is associated with a smart contract instance role.
      operationId: WorkflowGet
      x-api-path-slug: apiv1applicationsworkflowsworkflowid-get
      parameters:
      - in: path
        name: workflowId
        description: The id of the workflow
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Workflows
  /api/v1/applications/{applicationId}/contractCode:
    get:
      summary: Get Applications Contract Code
      description: |-
        List all blockchain smart contract implementations of the specified blockchain application.
                     Users who are Workbench administrators get all smart contract implementations. Non-Workbench administrators get all
                     smart contract implementations for which they have at least one associated application role or is associated with a
                     smart contract instance role.
      operationId: ContractCodesGet
      x-api-path-slug: apiv1applicationsapplicationidcontractcode-get
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      - in: query
        name: ledgerId
        description: The index of the chain type
      - in: query
        name: skip
        description: The number of items to skip before returning
      - in: query
        name: top
        description: The maximum number of items to return
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Contract
      - Code
    post:
      summary: Post Applications Contract Code
      description: |-
        Uploads one or more smart contracts (ex. .sol or .zip), representing the implementation of the specified blockchain
                     application. This method can only be performed by users who are Workbench administrators.
      operationId: ContractCodePost
      x-api-path-slug: apiv1applicationsapplicationidcontractcode-post
      parameters:
      - in: path
        name: applicationId
        description: The id of the application
      - in: formData
        name: contractFile
        description: Upload ContractCode File
      - in: query
        name: ledgerId
        description: The index of the ledger
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Contract
      - Code
  /api/v1/applications/contractCode/{contractCodeId}:
    get:
      summary: Get Applications Contract Code
      description: |-
        Get the blockchain smart contract implementation matching a specific
                     contract code id. Users who are Workbench administrators get the specified smart contract implementation.
                     Non-Workbench administrators get the smart contract implementation if they have at least one associated application
                     role or is associated with a smart contract instance role.
      operationId: ContractCodeGet
      x-api-path-slug: apiv1applicationscontractcodecontractcodeid-get
      parameters:
      - in: path
        name: contractCodeId
        description: The id of the contract code
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Contract
      - Code
    delete:
      summary: Delete Applications Contract Code
      description: |-
        Deletes the specified blockchain smart contract implementation of a specific blockchain application.
                     This method can only be performed by users who are Workbench administrators.
                     NOTE: not currently implemented
      operationId: ContractCodeDelete
      x-api-path-slug: apiv1applicationscontractcodecontractcodeid-delete
      parameters:
      - in: path
        name: contractCodeId
        description: The id of the contract code
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Contract
      - Code
  /api/v1/capabilities:
    get:
      summary: Get Capabilities
      description: |-
        List all capabilities the user can perform within Workbench.
                     Checked capabilities include ability to add blockchain applications, add smart contract implementations,
                     add or edit user role assignments, and add new users.
      operationId: CapabilitiesGet
      x-api-path-slug: apiv1capabilities-get
      responses:
        200:
          description: OK
      tags:
      - Capabilities
  /api/v1/capabilities/canCreateContract/{workflowId}:
    get:
      summary: Get Capabilities Can Create Contract
      description: Checks if user has capability to create new smart contract instance
        for a specific workflow ID.
      operationId: CanCreateContract
      x-api-path-slug: apiv1capabilitiescancreatecontractworkflowid-get
      parameters:
      - in: path
        name: workflowId
        description: The id of the workflow
      responses:
        200:
          description: OK
      tags:
      - Capabilities
      - Can
      - Contract
  /api/v1/checkers/checkApplication:
    post:
      summary: Post Checkers Check Application
      description: Checks if the supplied application configuration file is valid
        for Workbench.
      operationId: CheckApplicationPost
      x-api-path-slug: apiv1checkerscheckapplication-post
      parameters:
      - in: formData
        name: appFile
        description: Upload Application File
      responses:
        200:
          description: OK
      tags:
      - Checkers
      - Check
      - Application
  /api/v1/checkers/checkContractCode:
    post:
      summary: Post Checkers Check Contract Node
      description: Check if the application smart contract implementation file is
        valid for Workbench.
      operationId: CheckContractCodePost
      x-api-path-slug: apiv1checkerscheckcontractcode-post
      parameters:
      - in: formData
        name: appFile
        description: Upload Application File
      - in: formData
        name: contractFile
        description: Upload Contract Code File
      - in: query
        name: ledgerId
        description: The index of the chain type
      responses:
        200:
          description: OK
      tags:
      - Checkers
      - Check
      - Contract
      - Node
  /api/v1/ledgers/connections:
    get:
      summary: Get Ledgers Connections
      description: Lists the connected blockchain networks.
      operationId: ConnectionsGet
      x-api-path-slug: apiv1ledgersconnections-get
      parameters:
      - in: query
        name: skip
        description: The number of items to skip before returning
      - in: query
        name: top
        description: The maximum number of items to return
      responses:
        200:
          description: OK
      tags:
      - Ledgers
      - Connections
  /api/v1/ledgers/connections/{connectionId}:
    get:
      summary: Get Ledgers Connections
      description: Gets the connected blockchain network matching a specific connection
        ID.
      operationId: ConnectionGet
      x-api-path-slug: apiv1ledgersconnectionsconnectionid-get
      parameters:
      - in: path
        name: connectionId
        description: The id of the connection
      responses:
        200:
          description: OK
      tags:
      - Ledgers
      - Connections
  /api/v1/ledgers/connections/{connectionId}/blocks:
    get:
      summary: Get Ledgers Connections Blocks
      description: Lists the blocks for a connected blockchain network.
      operationId: BlocksGet
      x-api-path-slug: apiv1ledgersconnectionsconnectionidblocks-get
      parameters:
      - in: path
        name: connectionId
        description: The id of the connection
      - in: query
        name: skip
        description: The number of items to skip before returning
      - in: query
        name: top
        description: The maximum number of items to return
      responses:
        200:
          description: OK
      tags:
      - Ledgers
      - Connections
      - Blocks
  /api/v1/ledgers/connections/{connectionId}/blocks/{blockId}:
    get:
      summary: Get Ledgers Connections Blocks Blockid
      description: Gets the block matching a specific block ID.
      operationId: BlockGet
      x-api-path-slug: apiv1ledgersconnectionsconnectionidblocksblockid-get
      parameters:
      - in: path
        name: blockId
        description: The id of the block
      - in: path
        name: connectionId
        description: The connectionId of the block
      responses:
        200:
          description: OK
      tags:
      - Ledgers
      - Connections
      - Blocks
      - Blockid
  /api/v1/ledgers/connections/{connectionId}/transactions:
    get:
      summary: Get Ledgers Connections Transactions
      description: Lists the transactions for a connected blockchain network.
      operationId: TransactionsGet
      x-api-path-slug: apiv1ledgersconnectionsconnectionidtransactions-get
      parameters:
      - in: path
        name: connectionId
        description: The id of the connection
      - in: query
        name: skip
        description: The number of items to skip before returning
      - in: query
        name: top
        description: The maximum number of items to return
      responses:
        200:
          description: OK
      tags:
      - Ledgers
      - Connections
      - Transactions
  /api/v1/ledgers/connections/{connectionId}/transactions/{transactionId}:
    get:
      summary: Get Ledgers Connections Transactions Transactionid
      description: Gets the transaction matching a specific transaction ID.
      operationId: TransactionGet
      x-api-path-slug: apiv1ledgersconnectionsconnectionidtransactionstransactionid-get
      parameters:
      - in: path
        name: connectionId
        description: The connectionId of the transaction
      - in: path
        name: transactionId
        description: The id of the transaction
      responses:
        200:
          description: OK
      tags:
      - Ledgers
      - Connections
      - Transactions
      - Transactionid
  /api/v1/contracts:
    get:
      summary: Get Contracts
      description: |-
        Lists the smart contract instances of the specified workflow. Users who are Workbench administrators get all
                     smart contract instances. Non-Workbench administrators get all smart contract instances for which they have at least
                     one associated application role or is associated with a smart contract instance role.
      operationId: ContractsGet
      x-api-path-slug: apiv1contracts-get
      parameters:
      - in: query
        name: skip
        description: The number of items to skip before returning
      - in: query
        name: sortBy
        description: The field to sort
      - in: query
        name: top
        description: The maximum number of items to return
      - in: query
        name: workflowId
        description: The ID of the associated workflow
      responses:
        200:
          description: OK
      tags:
      - Contracts
    post:
      summary: Post Contracts
      description: |-
        Creates a new smart contract instance for the specified workflow ID.
                     Users are only able to create a new smart contract instance if the user is associated with an application role,
                     which can initiate a smart contract instance for the workflow.
      operationId: ContractPost
      x-api-path-slug: apiv1contracts-post
      parameters:
      - in: query
        name: connectionId
        description: The id of the blockchain connection
      - in: query
        name: contractCodeId
        description: The id of the smart contract implementation
      - in: body
        name: workflowActionInput
        description: The set of all contract action parameters
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: workflowId
        description: The id of the workflow
      responses:
        200:
          description: OK
      tags:
      - Contracts
  /api/v1/contracts/{contractId}:
    get:
      summary: Get Contracts
      description: |-
        Gets the smart contract instance matching a specific contract ID. Users who are Workbench
                     administrators get the smart contract instance. Non-Workbench administrators get the smart contract instance
                     if they have at least one associated application role or is associated with the smart contract instance.
      operationId: ContractGet
      x-api-path-slug: apiv1contractscontractid-get
      parameters:
      - in: path
        name: contractId
        description: The id of the contract
      responses:
        200:
          description: OK
      tags:
      - Contracts
  /api/v1/contracts/{contractId}/actions:
    get:
      summary: Get Contracts Actions
      description: |-
        Lists all actions, which can be taken by the given user and current state of the specified smart contract
                     instance. Users get all applicable actions if the user has an associated application role or is associated with a smart
                     contract instance role for the current state of the specified smart contract instance.
      operationId: ContractActionsGet
      x-api-path-slug: apiv1contractscontractidactions-get
      parameters:
      - in: path
        name: contractId
        description: The id of the contract
      - in: query
        name: skip
        description: The number of items to skip before returning
      - in: query
        name: top
        description: The maximum number of items to return
      responses:
        200:
          description: OK
      tags:
      - Contracts
      - Actions
    post:
      summary: Post Contracts Actions
      description: |-
        Executes an action for the specified smart contract instance and action ID. Users are only able to execute
                     the action given the current state of the specified smart contract instance and the user's associated application role
                     or smart contract instance role.
      operationId: ContractActionPost
      x-api-path-slug: apiv1contractscontractidactions-post
      parameters:
      - in: body
        name: actionInformation
        description: Parameters for a particular action
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contractId
        description: The id of the contract
      responses:
        200:
          description: OK
      tags:
      - Contracts
      - Actions
  /api/v1/contracts/{contractId}/actions/{actionId}:
    get:
      summary: Get Contracts Actions
      description: |-
        Gets the action matching the specified action ID. Users get the action if the user can take the action
                     given the current state of the specified smart contract instance and the user's associated application role or smart
                     contract instance role.
      operationId: ContractActionGet
      x-api-path-slug: apiv1contractscontractidactionsactionid-get
      parameters:
      - in: path
        name: actionId
        description: The id of the action
      - in: path
        name: contractId
        description: The id of the contract
      responses:
        200:
          description: OK
      tags:
      - Contracts
      - Actions
  /api/v1/graphProxy/{version}/users:
    get:
      summary: Get Graph Proxy Version Users
      description: |-
        Represents a proxy method to the Azure Active Directory Graph API for users.
                     See https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list for more details.
      operationId: GraphProxy-UsersGet
      x-api-path-slug: apiv1graphproxyversionusers-get
      parameters:
      - in: path
        name: version
        description: The version for the graph api endpoint
      responses:
        200:
          description: OK
      tags:
      - Graph
      - Proxy
      - Version
      - Users
  /api/health:
    get:
      summary: Get Api Health
      description: |-
        Returns the health of the system. See https://docs.microsoft.com/en-us/azure/architecture/patterns/health-endpoint-monitoring
                     for more details.
      operationId: Health
      x-api-path-slug: apihealth-get
      responses:
        200:
          description: OK
      tags:
      - Api
      - Health
  /api/v1/ledgers:
    get:
      summary: Get Ledgers
      description: Lists the supported blockchain types, such as Ethereum or Hyperledger
        Fabric.
      operationId: LedgersGet
      x-api-path-slug: apiv1ledgers-get
      parameters:
      - in: query
        name: skip
        description: The number of items to skip before returning
      - in: query
        name: top
        description: The maximum number of items to return
      responses:
        200:
          description: OK
      tags:
      - Ledgers
  /api/v1/users:
    get:
      summary: Get Users
      description: Lists all users within the connected blockchain consortium.
      operationId: UsersGet
      x-api-path-slug: apiv1users-get
      parameters:
      - in: query
        name: externalId
        description: The external ID of the user to query for
      - in: query
        name: skip
        description: The number of items to skip before returning
      - in: query
        name: sortBy
        description: The field to sort
      - in: query
        name: top
        description: The maximum number of items to return
      - in: query
        name: userChainIdentifier
        description: The on-chain address of the user to query for
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: Post Users
      description: |-
        Adds a user to the blockchain consortium. This method can only be performed by users who are
                     Workbench administrators.
      operationId: UsersPost
      x-api-path-slug: apiv1users-post
      parameters:
      - in: body
        name: userInput
        description: New user to add
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Users
  /api/v1/users/{userId}:
    get:
      summary: Get Users Userid
      description: Gets the user matching a specific user ID.
      operationId: UserGet
      x-api-path-slug: apiv1usersuserid-get
      parameters:
      - in: path
        name: userId
        description: The id of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Userid
    delete:
      summary: Delete Users Userid
      description: |-
        Deletes the specified user. This method can only be performed by users who are Workbench administrators.
                     NOTE: Not currently implemented.
      operationId: UserDelete
      x-api-path-slug: apiv1usersuserid-delete
      parameters:
      - in: path
        name: userId
        description: The id of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Userid
  /api/v1/users/me:
    get:
      summary: Get Users Me
      description: Returns the current user.
      operationId: MeGet
      x-api-path-slug: apiv1usersme-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Me