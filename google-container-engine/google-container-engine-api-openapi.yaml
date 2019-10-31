swagger: "2.0"
x-collection-name: Google Container Engine
x-complete: 1
info:
  title: Google Container Engine
  description: builds-and-manages-clusters-that-run-containerbased-applications-powered-by-open-source-kubernetes-technology-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: container.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/projects/{projectId}/zones/{zone}/clusters:
    get:
      summary: Get Clusters
      description: Lists all clusters owned by a project in either the specified zone
        or all zones.
      operationId: container.projects.zones.clusters.list
      x-api-path-slug: v1projectsprojectidzoneszoneclusters-get
      parameters:
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides, or - for all zones
      responses:
        200:
          description: OK
      tags:
      - Cluster
    post:
      summary: Create Cluster
      description: Creates a cluster, consisting of the specified number and type
        of Google Compute Engine instances. By default, the cluster is created in
        the project's [default network](/compute/docs/networks-and-firewalls#networks).
        One firewall is added for the cluster. After cluster creation, the cluster
        creates routes for each node to allow the containers on that node to communicate
        with all other instances in the cluster. Finally, an entry is added to the
        project's global metadata indicating which CIDR range is being used by the
        cluster.
      operationId: container.projects.zones.clusters.create
      x-api-path-slug: v1projectsprojectidzoneszoneclusters-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides
      responses:
        200:
          description: OK
      tags:
      - Cluster
  /v1/projects/{projectId}/zones/{zone}/clusters/{clusterId}:
    delete:
      summary: Delete Cluster
      description: Deletes the cluster, including the Kubernetes endpoint and all
        worker nodes. Firewalls and routes that were configured during cluster creation
        are also deleted. Other Google Compute Engine resources that might be in use
        by the cluster (e.g. load balancer resources) will not be deleted if they
        weren't present at the initial create time.
      operationId: container.projects.zones.clusters.delete
      x-api-path-slug: v1projectsprojectidzoneszoneclustersclusterid-delete
      parameters:
      - in: path
        name: clusterId
        description: The name of the cluster to delete
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides
      responses:
        200:
          description: OK
      tags:
      - Cluster
    get:
      summary: Get Cluster
      description: Gets the details of a specific cluster.
      operationId: container.projects.zones.clusters.get
      x-api-path-slug: v1projectsprojectidzoneszoneclustersclusterid-get
      parameters:
      - in: path
        name: clusterId
        description: The name of the cluster to retrieve
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides
      responses:
        200:
          description: OK
      tags:
      - Cluster
    put:
      summary: Update Cluster
      description: Updates the settings of a specific cluster.
      operationId: container.projects.zones.clusters.update
      x-api-path-slug: v1projectsprojectidzoneszoneclustersclusterid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: clusterId
        description: The name of the cluster to upgrade
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides
      responses:
        200:
          description: OK
      tags:
      - Cluster
  /v1/projects/{projectId}/zones/{zone}/clusters/{clusterId}/nodePools:
    get:
      summary: Get Cluster Node Pools
      description: Lists the node pools for a cluster.
      operationId: container.projects.zones.clusters.nodePools.list
      x-api-path-slug: v1projectsprojectidzoneszoneclustersclusteridnodepools-get
      parameters:
      - in: path
        name: clusterId
        description: The name of the cluster
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://developers
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides
      responses:
        200:
          description: OK
      tags:
      - Node Pool
    post:
      summary: Create Cluster Node Pool
      description: Creates a node pool for a cluster.
      operationId: container.projects.zones.clusters.nodePools.create
      x-api-path-slug: v1projectsprojectidzoneszoneclustersclusteridnodepools-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: clusterId
        description: The name of the cluster
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://developers
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides
      responses:
        200:
          description: OK
      tags:
      - Node Pool
  /v1/projects/{projectId}/zones/{zone}/clusters/{clusterId}/nodePools/{nodePoolId}:
    delete:
      summary: Delete Cluster Node Pool
      description: Deletes a node pool from a cluster.
      operationId: container.projects.zones.clusters.nodePools.delete
      x-api-path-slug: v1projectsprojectidzoneszoneclustersclusteridnodepoolsnodepoolid-delete
      parameters:
      - in: path
        name: clusterId
        description: The name of the cluster
      - in: path
        name: nodePoolId
        description: The name of the node pool to delete
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://developers
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides
      responses:
        200:
          description: OK
      tags:
      - Node Pool
    get:
      summary: Get Cluster Node Pool
      description: Retrieves the node pool requested.
      operationId: container.projects.zones.clusters.nodePools.get
      x-api-path-slug: v1projectsprojectidzoneszoneclustersclusteridnodepoolsnodepoolid-get
      parameters:
      - in: path
        name: clusterId
        description: The name of the cluster
      - in: path
        name: nodePoolId
        description: The name of the node pool
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://developers
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides
      responses:
        200:
          description: OK
      tags:
      - Node Pool
  /v1/projects/{projectId}/zones/{zone}/clusters/{clusterId}/nodePools/{nodePoolId}/setManagement:
    post:
      summary: Set Cluster Node Management
      description: Sets the NodeManagement options for a node pool.
      operationId: container.projects.zones.clusters.nodePools.setManagement
      x-api-path-slug: v1projectsprojectidzoneszoneclustersclusteridnodepoolsnodepoolidsetmanagement-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: clusterId
        description: The name of the cluster to update
      - in: path
        name: nodePoolId
        description: The name of the node pool to update
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides
      responses:
        200:
          description: OK
      tags:
      - Node Pool
  /v1/projects/{projectId}/zones/{zone}/clusters/{clusterId}/nodePools/{nodePoolId}:rollback:
    post:
      summary: Rollback Node
      description: Roll back the previously Aborted or Failed NodePool upgrade. This
        will be an no-op if the last upgrade successfully completed.
      operationId: container.projects.zones.clusters.nodePools.rollback
      x-api-path-slug: v1projectsprojectidzoneszoneclustersclusteridnodepoolsnodepoolidrollback-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: clusterId
        description: The name of the cluster to rollback
      - in: path
        name: nodePoolId
        description: The name of the node pool to rollback
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides
      responses:
        200:
          description: OK
      tags:
      - Node Pool
  /v1/projects/{projectId}/zones/{zone}/operations:
    get:
      summary: Get Operations
      description: Lists all operations in a project in a specific zone or all zones.
      operationId: container.projects.zones.operations.list
      x-api-path-slug: v1projectsprojectidzoneszoneoperations-get
      parameters:
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          to return operations for, or `-` for all zones
      responses:
        200:
          description: OK
      tags:
      - Operation
  /v1/projects/{projectId}/zones/{zone}/operations/{operationId}:
    get:
      summary: Get Operations
      description: Gets the specified operation.
      operationId: container.projects.zones.operations.get
      x-api-path-slug: v1projectsprojectidzoneszoneoperationsoperationid-get
      parameters:
      - in: path
        name: operationId
        description: The server-assigned `name` of the operation
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides
      responses:
        200:
          description: OK
      tags:
      - Operation
  /v1/projects/{projectId}/zones/{zone}/operations/{operationId}:cancel:
    post:
      summary: Create Operation
      description: Cancels the specified operation.
      operationId: container.projects.zones.operations.cancel
      x-api-path-slug: v1projectsprojectidzoneszoneoperationsoperationidcancel-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: operationId
        description: The server-assigned `name` of the operation
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the operation resides
      responses:
        200:
          description: OK
      tags:
      - Operation
  /v1/projects/{projectId}/zones/{zone}/serverconfig:
    get:
      summary: Get Server Configuration
      description: Returns configuration info about the Container Engine service.
      operationId: container.projects.zones.getServerconfig
      x-api-path-slug: v1projectsprojectidzoneszoneserverconfig-get
      parameters:
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          to return operations for
      responses:
        200:
          description: OK
      tags:
      - Server