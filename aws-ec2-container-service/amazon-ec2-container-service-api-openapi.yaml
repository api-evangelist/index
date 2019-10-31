swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 1
info:
  title: AWS EC2 Container Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateCluster:
    get:
      summary: Create Cluster
      description: Creates a new Amazon ECS cluster.
      operationId: createCluster
      x-api-path-slug: actioncreatecluster-get
      parameters:
      - in: query
        name: clusterName
        description: The name of your cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=CreateService:
    get:
      summary: Create Service
      description: Runs and maintains a desired number of tasks from a specified task
        definition.
      operationId: createService
      x-api-path-slug: actioncreateservice-get
      parameters:
      - in: query
        name: clientToken
        description: Unique, case-sensitive identifier you provide to ensure the idempotency
          of the            request
        type: string
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          on which to run your service
        type: string
      - in: query
        name: deploymentConfiguration
        description: Optional deployment parameters that control how many tasks run
          during the            deployment and the ordering of stopping and starting
          tasks
        type: string
      - in: query
        name: desiredCount
        description: The number of instantiations of the specified task definition
          to place and keep            running on your cluster
        type: string
      - in: query
        name: loadBalancers
        description: A load balancer object representing the load balancer to use
          with your service
        type: string
      - in: query
        name: placementConstraints
        description: An array of placement constraint objects to use for tasks in
          your service
        type: string
      - in: query
        name: placementStrategy
        description: The placement strategy objects to use for tasks in your service
        type: string
      - in: query
        name: role
        description: The name or full Amazon Resource Name (ARN) of the IAM role that
          allows Amazon ECS to make calls to your            load balancer on your
          behalf
        type: string
      - in: query
        name: serviceName
        description: The name of your service
        type: string
      - in: query
        name: taskDefinition
        description: The family and revision (family:revision) or            full
          Amazon Resource Name (ARN) of the task definition to run in your service
        type: string
      responses:
        200:
          description: OK
      tags:
      - Services
  /?Action=DeleteAttributes:
    get:
      summary: Delete Attributes
      description: Deletes one or more custom attributes from an Amazon ECS resource.
      operationId: deleteAttributes
      x-api-path-slug: actiondeleteattributes-get
      parameters:
      - in: query
        name: attributes
        description: The attributes to delete from your resource
        type: string
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that contains the resource to apply            attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attributes
  /?Action=DeleteCluster:
    get:
      summary: Delete Cluster
      description: Deletes the specified cluster.
      operationId: deleteCluster
      x-api-path-slug: actiondeletecluster-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DeleteService:
    get:
      summary: Delete Service
      description: Deletes a specified service within a cluster.
      operationId: deleteService
      x-api-path-slug: actiondeleteservice-get
      parameters:
      - in: query
        name: cluster
        description: The name of the cluster that hosts the service to delete
        type: string
      - in: query
        name: service
        description: The name of the service to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Services
  /?Action=DeregisterContainerInstance:
    get:
      summary: Deregister Container Instance
      description: Deregisters an Amazon ECS container instance from the specified
        cluster.
      operationId: deregisterContainerInstance
      x-api-path-slug: actionderegistercontainerinstance-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the container instance            to deregister
        type: string
      - in: query
        name: containerInstance
        description: The container instance ID or full Amazon Resource Name (ARN)
          of the container instance to            deregister
        type: string
      - in: query
        name: force
        description: Forces the deregistration of the container instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Instances
  /?Action=DeregisterTaskDefinition:
    get:
      summary: Deregister Task Definition
      description: Deregisters the specified task definition by family and revision.
      operationId: deregisterTaskDefinition
      x-api-path-slug: actionderegistertaskdefinition-get
      parameters:
      - in: query
        name: taskDefinition
        description: The family and revision (family:revision) or            full
          Amazon Resource Name (ARN) of the task definition to deregister
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Definitions
  /?Action=DescribeClusters:
    get:
      summary: Describe Clusters
      description: Describes one or more of your clusters.
      operationId: describeClusters
      x-api-path-slug: actiondescribeclusters-get
      parameters:
      - in: query
        name: clusters
        description: A space-separated list of up to 100 cluster names or full cluster
          Amazon Resource Name (ARN)            entries
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DescribeContainerInstances:
    get:
      summary: Describe Container Instances
      description: Describes Amazon EC2 Container Service container instances.
      operationId: describeContainerInstances
      x-api-path-slug: actiondescribecontainerinstances-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the container instances            to describe
        type: string
      - in: query
        name: containerInstances
        description: A space-separated list of container instance IDs or full Amazon
          Resource Name (ARN)            entries
        type: string
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Instances
  /?Action=DescribeServices:
    get:
      summary: Describe Services
      description: Describes the specified services running in your cluster.
      operationId: describeServices
      x-api-path-slug: actiondescribeservices-get
      parameters:
      - in: query
        name: cluster
        description: The name of the cluster that hosts the service to describe
        type: string
      - in: query
        name: services
        description: A list of services to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Services
  /?Action=DescribeTaskDefinition:
    get:
      summary: Describe Task Definition
      description: Describes a task definition.
      operationId: describeTaskDefinition
      x-api-path-slug: actiondescribetaskdefinition-get
      parameters:
      - in: query
        name: taskDefinition
        description: The family for the latest ACTIVE revision,                family
          and revision (family:revision) for a            specific revision in the
          family, or full Amazon Resource Name (ARN) of the task definition to            describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Definitions
  /?Action=DescribeTasks:
    get:
      summary: Describe Tasks
      description: Describes a specified task or tasks.
      operationId: describeTasks
      x-api-path-slug: actiondescribetasks-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the task to describe
        type: string
      - in: query
        name: tasks
        description: A space-separated list of task IDs or full Amazon Resource Name
          (ARN) entries
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=DiscoverPollEndpoint:
    get:
      summary: Discover Poll Endpoint
      description: This action is only used by the Amazon EC2 Container Service agent,
        and it is not intended for use outside of the agent.
      operationId: discoverPollEndpoint
      x-api-path-slug: actiondiscoverpollendpoint-get
      responses:
        200:
          description: OK
      tags:
      - Poll Endpoints
  /?Action=ListAttributes:
    get:
      summary: List Attributes
      description: |-
        Lists the attributes for Amazon ECS resources within a specified target type and
                    cluster.
      operationId: listAttributes
      x-api-path-slug: actionlistattributes-get
      parameters:
      - in: query
        name: attributeName
        description: The name of the attribute with which to filter the results
        type: string
      - in: query
        name: attributeValue
        description: The value of the attribute with which to filter results
        type: string
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          to list attributes
        type: string
      - in: query
        name: maxResults
        description: The maximum number of cluster results returned by ListAttributes
          in            paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListAttributes
          request where maxResults was used and the            results exceeded the
          value of that parameter
        type: string
      - in: query
        name: targetType
        description: The type of the target with which to list attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attributes
  /?Action=ListClusters:
    get:
      summary: List Clusters
      description: Returns a list of existing clusters.
      operationId: listClusters
      x-api-path-slug: actionlistclusters-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of cluster results returned by ListClusters
          in            paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListClusters
          request where maxResults was used and the            results exceeded the
          value of that parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=ListContainerInstances:
    get:
      summary: List Container Instances
      description: Returns a list of container instances in a specified cluster.
      operationId: listContainerInstances
      x-api-path-slug: actionlistcontainerinstances-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the container instances            to list
        type: string
      - in: query
        name: filter
        description: You can filter the results of a ListContainerInstances operation
          with            cluster query language statements
        type: string
      - in: query
        name: maxResults
        description: The maximum number of container instance results returned by                ListContainerInstances
          in paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListContainerInstances
          request where maxResults was used            and the results exceeded the
          value of that parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Instances
  /?Action=ListServices:
    get:
      summary: List Services
      description: Lists the services that are running in a specified cluster.
      operationId: listServices
      x-api-path-slug: actionlistservices-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the services to list
        type: string
      - in: query
        name: maxResults
        description: The maximum number of container instance results returned by                ListServices
          in paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListServices
          request where maxResults was used and the            results exceeded the
          value of that parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Services
  /?Action=ListTaskDefinitionFamilies:
    get:
      summary: List Task Definition Families
      description: |-
        Returns a list of task definition families that are registered to your account
                    (which may include task definition families that no longer have any ACTIVE
                    task definition revisions).
      operationId: listTaskDefinitionFamilies
      x-api-path-slug: actionlisttaskdefinitionfamilies-get
      parameters:
      - in: query
        name: familyPrefix
        description: The familyPrefix is a string that is used to filter the results
          of                ListTaskDefinitionFamilies
        type: string
      - in: query
        name: maxResults
        description: The maximum number of task definition family results returned
          by                ListTaskDefinitionFamilies in paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListTaskDefinitionFamilies
          request where maxResults was            used and the results exceeded the
          value of that parameter
        type: string
      - in: query
        name: status
        description: The task definition family status with which to filter the                ListTaskDefinitionFamilies
          results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Definition Families
  /?Action=ListTaskDefinitions:
    get:
      summary: List Task Definitions
      description: Returns a list of task definitions that are registered to your
        account.
      operationId: listTaskDefinitions
      x-api-path-slug: actionlisttaskdefinitions-get
      parameters:
      - in: query
        name: familyPrefix
        description: The full family name with which to filter the ListTaskDefinitions            results
        type: string
      - in: query
        name: maxResults
        description: The maximum number of task definition results returned by                ListTaskDefinitions
          in paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListTaskDefinitions
          request where maxResults was used and            the results exceeded the
          value of that parameter
        type: string
      - in: query
        name: sort
        description: The order in which to sort the results
        type: string
      - in: query
        name: status
        description: The task definition status with which to filter the                ListTaskDefinitions
          results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Definitions
  /?Action=ListTasks:
    get:
      summary: List Tasks
      description: Returns a list of tasks for a specified cluster.
      operationId: listTasks
      x-api-path-slug: actionlisttasks-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the tasks to list
        type: string
      - in: query
        name: containerInstance
        description: The container instance ID or full Amazon Resource Name (ARN)
          of the container instance with which to            filter the ListTasks
          results
        type: string
      - in: query
        name: desiredStatus
        description: The task desired status with which to filter the ListTasks results
        type: string
      - in: query
        name: family
        description: The name of the family with which to filter the ListTasks results
        type: string
      - in: query
        name: maxResults
        description: The maximum number of task results returned by ListTasks in paginated            output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListTasks
          request where maxResults was used and the            results exceeded the
          value of that parameter
        type: string
      - in: query
        name: serviceName
        description: The name of the service with which to filter the ListTasks results
        type: string
      - in: query
        name: startedBy
        description: The startedBy value with which to filter the task results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=PutAttributes:
    get:
      summary: Put Attributes
      description: Create or update an attribute on an Amazon ECS resource.
      operationId: putAttributes
      x-api-path-slug: actionputattributes-get
      parameters:
      - in: query
        name: attributes
        description: The attributes to apply to your resource
        type: string
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that contains the resource to apply            attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attributes
  /?Action=RegisterContainerInstance:
    get:
      summary: Register Container Instance
      description: Deregisters an Amazon ECS container instance from the specified
        cluster.
      operationId: registerContainerInstance
      x-api-path-slug: actionregistercontainerinstance-get
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Instances
  /?Action=RegisterTaskDefinition:
    get:
      summary: Register Task Definition
      description: |-
        Registers a new task definition from the supplied family and
                        containerDefinitions.
      operationId: registerTaskDefinition
      x-api-path-slug: actionregistertaskdefinition-get
      parameters:
      - in: query
        name: containerDefinitions
        description: A list of container definitions in JSON format that describe
          the different            containers that make up your task
        type: string
      - in: query
        name: family
        description: You must specify a family for a task definition, which allows
          you to            track multiple versions of the same task definition
        type: string
      - in: query
        name: networkMode
        description: The Docker networking mode to use for the containers in the task
        type: string
      - in: query
        name: placementConstraints
        description: An array of placement constraint objects to use for the task
        type: string
      - in: query
        name: taskRoleArn
        description: The short name or full Amazon Resource Name (ARN) of the IAM
          role that containers in this task can            assume
        type: string
      - in: query
        name: volumes
        description: A list of volume definitions in JSON format that containers in
          your task may            use
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Definitions
  /?Action=RunTask:
    get:
      summary: Run Task
      description: Starts a new task using the specified task definition.
      operationId: runTask
      x-api-path-slug: actionruntask-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          on which to run your task
        type: string
      - in: query
        name: count
        description: The number of instantiations of the specified task to place on
          your            cluster
        type: string
      - in: query
        name: group
        description: The name of the task group to associate with the task
        type: string
      - in: query
        name: overrides
        description: A list of container overrides in JSON format that specify the
          name of a container            in the specified task definition and the
          overrides it should receive
        type: string
      - in: query
        name: placementConstraints
        description: An array of placement constraint objects to use for the task
        type: string
      - in: query
        name: placementStrategy
        description: The placement strategy objects to use for the task
        type: string
      - in: query
        name: startedBy
        description: An optional tag specified when a task is started
        type: string
      - in: query
        name: taskDefinition
        description: The family and revision (family:revision) or            full
          Amazon Resource Name (ARN) of the task definition to run
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=StartTask:
    get:
      summary: Start Task
      description: |-
        Starts a new task from the specified task definition on the specified container
                    instance or instances.
      operationId: startTask
      x-api-path-slug: actionstarttask-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          on which to start your task
        type: string
      - in: query
        name: containerInstances
        description: The container instance IDs or full Amazon Resource Name (ARN)
          entries for the container instances on            which you would like to
          place your task
        type: string
      - in: query
        name: group
        description: The name of the task group to associate with the task
        type: string
      - in: query
        name: overrides
        description: A list of container overrides in JSON format that specify the
          name of a container            in the specified task definition and the
          overrides it should receive
        type: string
      - in: query
        name: startedBy
        description: An optional tag specified when a task is started
        type: string
      - in: query
        name: taskDefinition
        description: The family and revision (family:revision) or            full
          Amazon Resource Name (ARN) of the task definition to start
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=StopTask:
    get:
      summary: Stop Task
      description: Stops a running task.
      operationId: stopTask
      x-api-path-slug: actionstoptask-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the task to stop
        type: string
      - in: query
        name: reason
        description: An optional message specified when a task is stopped
        type: string
      - in: query
        name: task
        description: The task ID or full Amazon Resource Name (ARN) entry of the task
          to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=SubmitContainerStateChange:
    get:
      summary: Submit Container State Change
      description: This action is only used by the Amazon EC2 Container Service agent,
        and it is not intended for use outside of the agent.
      operationId: submitContainerStateChange
      x-api-path-slug: actionsubmitcontainerstatechange-get
      responses:
        200:
          description: OK
      tags:
      - Container State Change
  /?Action=SubmitTaskStateChange:
    get:
      summary: Submit Task State Change
      description: This action is only used by the Amazon EC2 Container Service agent,
        and it is not intended for use outside of the agent.
      operationId: submitTaskStateChange
      x-api-path-slug: actionsubmittaskstatechange-get
      responses:
        200:
          description: OK
      tags:
      - Task State Change
  /?Action=UpdateContainerAgent:
    get:
      summary: Update Container Agent
      description: Updates the Amazon ECS container agent on a specified container
        instance.
      operationId: updateContainerAgent
      x-api-path-slug: actionupdatecontaineragent-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that your container instance is            running on
        type: string
      - in: query
        name: containerInstance
        description: The container instance ID or full Amazon Resource Name (ARN)
          entries for the container instance on            which you would like to
          update the Amazon ECS container agent
        type: string
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Agents
  /?Action=UpdateService:
    get:
      summary: Update Service
      description: |-
        Modifies the desired count, deployment configuration, or task definition used in a
                    service.
      operationId: updateService
      x-api-path-slug: actionupdateservice-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that your service is running on
        type: string
      - in: query
        name: deploymentConfiguration
        description: Optional deployment parameters that control how many tasks run
          during the            deployment and the ordering of stopping and starting
          tasks
        type: string
      - in: query
        name: desiredCount
        description: The number of instantiations of the task to place and keep running
          in your            service
        type: string
      - in: query
        name: service
        description: The name of the service to update
        type: string
      - in: query
        name: taskDefinition
        description: The family and revision (family:revision) or            full
          Amazon Resource Name (ARN) of the task definition to run in your service
        type: string
      responses:
        200:
          description: OK
      tags:
      - Services