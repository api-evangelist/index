swagger: "2.0"
x-collection-name: Kubernetes
x-complete: 1
info:
  title: Kubernetes
  version: 1.0.0
host: /api/v1beta3
basePath: 127.0.0.1:6443
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1beta3/endpoints:
    get:
      summary: Get Endpoints
      description: List objects of kind endpoints.
      operationId: listEndpoints
      x-api-path-slug: apiv1beta3endpoints-get
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /api/v1beta3/events:
    get:
      summary: Get Events
      description: List objects of kind event.
      operationId: listEvent
      x-api-path-slug: apiv1beta3events-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /api/v1beta3/limitranges:
    get:
      summary: Get Limitranges
      description: List objects of kind limitrange.
      operationId: listLimitRange
      x-api-path-slug: apiv1beta3limitranges-get
      responses:
        200:
          description: OK
      tags:
      - Limitranges
  /api/v1beta3/namespaces:
    get:
      summary: Get Namespaces
      description: List objects of kind namespace.
      operationId: listNamespace
      x-api-path-slug: apiv1beta3namespaces-get
      responses:
        200:
          description: OK
      tags:
      - Namespaces
    post:
      summary: Post Namespaces
      description: Create a namespace.
      operationId: createNamespace
      x-api-path-slug: apiv1beta3namespaces-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Namespaces
  /api/v1beta3/namespaces/{namespaces}/bindings:
    post:
      summary: Post Namespaces Bindings
      description: Create a binding.
      operationId: createBinding
      x-api-path-slug: apiv1beta3namespacesnamespacesbindings-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Bindings
  /api/v1beta3/namespaces/{namespaces}/endpoints:
    get:
      summary: Get Namespaces Endpoints
      description: List objects of kind endpoints.
      operationId: listEndpoints
      x-api-path-slug: apiv1beta3namespacesnamespacesendpoints-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Endpoints
    post:
      summary: Post Namespaces Endpoints
      description: Create a endpoints.
      operationId: createEndpoints
      x-api-path-slug: apiv1beta3namespacesnamespacesendpoints-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Endpoints
  /api/v1beta3/namespaces/{namespaces}/endpoints/{name}:
    get:
      summary: Get Namespaces Endpoints Name
      description: Read the specified endpoints.
      operationId: readEndpoints
      x-api-path-slug: apiv1beta3namespacesnamespacesendpointsname-get
      parameters:
      - in: path
        name: name
        description: name of the Endpoints
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Endpoints
      - Name
    put:
      summary: Put Namespaces Endpoints Name
      description: Update the specified endpoints.
      operationId: updateEndpoints
      x-api-path-slug: apiv1beta3namespacesnamespacesendpointsname-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: name of the Endpoints
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Endpoints
      - Name
  /api/v1beta3/namespaces/{namespaces}/events:
    get:
      summary: Get Namespaces Events
      description: List objects of kind event.
      operationId: listEvent
      x-api-path-slug: apiv1beta3namespacesnamespacesevents-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Events
    post:
      summary: Post Namespaces Events
      description: Create a event.
      operationId: createEvent
      x-api-path-slug: apiv1beta3namespacesnamespacesevents-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Events
  /api/v1beta3/namespaces/{namespaces}/events/{name}:
    delete:
      summary: Delete Namespaces Events Name
      description: Delete a event.
      operationId: deleteEvent
      x-api-path-slug: apiv1beta3namespacesnamespaceseventsname-delete
      parameters:
      - in: path
        name: name
        description: name of the Event
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Events
      - Name
    get:
      summary: Get Namespaces Events Name
      description: Read the specified event.
      operationId: readEvent
      x-api-path-slug: apiv1beta3namespacesnamespaceseventsname-get
      parameters:
      - in: path
        name: name
        description: name of the Event
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Events
      - Name
    put:
      summary: Put Namespaces Events Name
      description: Update the specified event.
      operationId: updateEvent
      x-api-path-slug: apiv1beta3namespacesnamespaceseventsname-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: name of the Event
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Events
      - Name
  /api/v1beta3/namespaces/{namespaces}/limitranges:
    get:
      summary: Get Namespaces Limitranges
      description: List objects of kind limitrange.
      operationId: listLimitRange
      x-api-path-slug: apiv1beta3namespacesnamespaceslimitranges-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Limitranges
    post:
      summary: Post Namespaces Limitranges
      description: Create a limitrange.
      operationId: createLimitRange
      x-api-path-slug: apiv1beta3namespacesnamespaceslimitranges-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Limitranges
  /api/v1beta3/namespaces/{namespaces}/limitranges/{name}:
    delete:
      summary: Delete Namespaces Limitranges Name
      description: Delete a limitrange.
      operationId: deleteLimitRange
      x-api-path-slug: apiv1beta3namespacesnamespaceslimitrangesname-delete
      parameters:
      - in: path
        name: name
        description: name of the LimitRange
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Limitranges
      - Name
    get:
      summary: Get Namespaces Limitranges Name
      description: Read the specified limitrange.
      operationId: readLimitRange
      x-api-path-slug: apiv1beta3namespacesnamespaceslimitrangesname-get
      parameters:
      - in: path
        name: name
        description: name of the LimitRange
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Limitranges
      - Name
    put:
      summary: Put Namespaces Limitranges Name
      description: Update the specified limitrange.
      operationId: updateLimitRange
      x-api-path-slug: apiv1beta3namespacesnamespaceslimitrangesname-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: name of the LimitRange
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Limitranges
      - Name
  /api/v1beta3/namespaces/{namespaces}/pods:
    get:
      summary: Get Namespaces Pods
      description: List objects of kind pod.
      operationId: listPod
      x-api-path-slug: apiv1beta3namespacesnamespacespods-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Pods
    post:
      summary: Post Namespaces Pods
      description: Create a pod.
      operationId: createPod
      x-api-path-slug: apiv1beta3namespacesnamespacespods-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Pods
  /api/v1beta3/namespaces/{namespaces}/pods/{name}:
    delete:
      summary: Delete Namespaces Pods Name
      description: Delete a pod.
      operationId: deletePod
      x-api-path-slug: apiv1beta3namespacesnamespacespodsname-delete
      parameters:
      - in: path
        name: name
        description: name of the Pod
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Pods
      - Name
    get:
      summary: Get Namespaces Pods Name
      description: Read the specified pod.
      operationId: readPod
      x-api-path-slug: apiv1beta3namespacesnamespacespodsname-get
      parameters:
      - in: path
        name: name
        description: name of the Pod
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Pods
      - Name
    put:
      summary: Put Namespaces Pods Name
      description: Update the specified pod.
      operationId: updatePod
      x-api-path-slug: apiv1beta3namespacesnamespacespodsname-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: name of the Pod
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Pods
      - Name
  /api/v1beta3/namespaces/{namespaces}/replicationcontrollers:
    get:
      summary: Get Namespaces Replicationcontrollers
      description: List objects of kind replicationcontroller.
      operationId: listReplicationController
      x-api-path-slug: apiv1beta3namespacesnamespacesreplicationcontrollers-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Replicationcontrollers
    post:
      summary: Post Namespaces Replicationcontrollers
      description: Create a replicationcontroller.
      operationId: createReplicationController
      x-api-path-slug: apiv1beta3namespacesnamespacesreplicationcontrollers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Replicationcontrollers
  /api/v1beta3/namespaces/{namespaces}/replicationcontrollers/{name}:
    delete:
      summary: Delete Namespaces Replicationcontrollers Name
      description: Delete a replicationcontroller.
      operationId: deleteReplicationController
      x-api-path-slug: apiv1beta3namespacesnamespacesreplicationcontrollersname-delete
      parameters:
      - in: path
        name: name
        description: name of the ReplicationController
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Replicationcontrollers
      - Name
    get:
      summary: Get Namespaces Replicationcontrollers Name
      description: Read the specified replicationcontroller.
      operationId: readReplicationController
      x-api-path-slug: apiv1beta3namespacesnamespacesreplicationcontrollersname-get
      parameters:
      - in: path
        name: name
        description: name of the ReplicationController
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Replicationcontrollers
      - Name
    put:
      summary: Put Namespaces Replicationcontrollers Name
      description: Update the specified replicationcontroller.
      operationId: updateReplicationController
      x-api-path-slug: apiv1beta3namespacesnamespacesreplicationcontrollersname-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: name of the ReplicationController
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Replicationcontrollers
      - Name
  /api/v1beta3/namespaces/{namespaces}/resourcequotas:
    get:
      summary: Get Namespaces Resourcequotas
      description: List objects of kind resourcequota.
      operationId: listResourceQuota
      x-api-path-slug: apiv1beta3namespacesnamespacesresourcequotas-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Resourcequotas
    post:
      summary: Post Namespaces Resourcequotas
      description: Create a resourcequota.
      operationId: createResourceQuota
      x-api-path-slug: apiv1beta3namespacesnamespacesresourcequotas-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Resourcequotas
  /api/v1beta3/namespaces/{namespaces}/resourcequotas/{name}:
    delete:
      summary: Delete Namespaces Resourcequotas Name
      description: Delete a resourcequota.
      operationId: deleteResourceQuota
      x-api-path-slug: apiv1beta3namespacesnamespacesresourcequotasname-delete
      parameters:
      - in: path
        name: name
        description: name of the ResourceQuota
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Resourcequotas
      - Name
    get:
      summary: Get Namespaces Resourcequotas Name
      description: Read the specified resourcequota.
      operationId: readResourceQuota
      x-api-path-slug: apiv1beta3namespacesnamespacesresourcequotasname-get
      parameters:
      - in: path
        name: name
        description: name of the ResourceQuota
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Resourcequotas
      - Name
    put:
      summary: Put Namespaces Resourcequotas Name
      description: Update the specified resourcequota.
      operationId: updateResourceQuota
      x-api-path-slug: apiv1beta3namespacesnamespacesresourcequotasname-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: name of the ResourceQuota
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Resourcequotas
      - Name
  /api/v1beta3/namespaces/{namespaces}/resourcequotausages:
    post:
      summary: Post Namespaces Resourcequotausages
      description: Create a resourcequotausage.
      operationId: createResourceQuotaUsage
      x-api-path-slug: apiv1beta3namespacesnamespacesresourcequotausages-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Resourcequotausages
  /api/v1beta3/namespaces/{namespaces}/secrets:
    get:
      summary: Get Namespaces Secrets
      description: List objects of kind secret.
      operationId: listSecret
      x-api-path-slug: apiv1beta3namespacesnamespacessecrets-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Secrets
    post:
      summary: Post Namespaces Secrets
      description: Create a secret.
      operationId: createSecret
      x-api-path-slug: apiv1beta3namespacesnamespacessecrets-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Secrets
  /api/v1beta3/namespaces/{namespaces}/secrets/{name}:
    delete:
      summary: Delete Namespaces Secrets Name
      description: Delete a secret.
      operationId: deleteSecret
      x-api-path-slug: apiv1beta3namespacesnamespacessecretsname-delete
      parameters:
      - in: path
        name: name
        description: name of the Secret
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Secrets
      - Name
    get:
      summary: Get Namespaces Secrets Name
      description: Read the specified secret.
      operationId: readSecret
      x-api-path-slug: apiv1beta3namespacesnamespacessecretsname-get
      parameters:
      - in: path
        name: name
        description: name of the Secret
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Secrets
      - Name
    put:
      summary: Put Namespaces Secrets Name
      description: Update the specified secret.
      operationId: updateSecret
      x-api-path-slug: apiv1beta3namespacesnamespacessecretsname-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: name of the Secret
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Secrets
      - Name
  /api/v1beta3/namespaces/{namespaces}/services:
    get:
      summary: Get Namespaces Services
      description: List objects of kind service.
      operationId: listService
      x-api-path-slug: apiv1beta3namespacesnamespacesservices-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Services
    post:
      summary: Post Namespaces Services
      description: Create a service.
      operationId: createService
      x-api-path-slug: apiv1beta3namespacesnamespacesservices-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Services
  /api/v1beta3/namespaces/{namespaces}/services/{name}:
    delete:
      summary: Delete Namespaces Services Name
      description: Delete a service.
      operationId: deleteService
      x-api-path-slug: apiv1beta3namespacesnamespacesservicesname-delete
      parameters:
      - in: path
        name: name
        description: name of the Service
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Services
      - Name
    get:
      summary: Get Namespaces Services Name
      description: Read the specified service.
      operationId: readService
      x-api-path-slug: apiv1beta3namespacesnamespacesservicesname-get
      parameters:
      - in: path
        name: name
        description: name of the Service
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Services
      - Name
    put:
      summary: Put Namespaces Services Name
      description: Update the specified service.
      operationId: updateService
      x-api-path-slug: apiv1beta3namespacesnamespacesservicesname-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: name of the Service
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Services
      - Name
  /api/v1beta3/namespaces/{name}:
    delete:
      summary: Delete Namespaces Name
      description: Delete a namespace.
      operationId: deleteNamespace
      x-api-path-slug: apiv1beta3namespacesname-delete
      parameters:
      - in: path
        name: name
        description: name of the Namespace
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Name
    get:
      summary: Get Namespaces Name
      description: Read the specified namespace.
      operationId: readNamespace
      x-api-path-slug: apiv1beta3namespacesname-get
      parameters:
      - in: path
        name: name
        description: name of the Namespace
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Name
    put:
      summary: Put Namespaces Name
      description: Update the specified namespace.
      operationId: updateNamespace
      x-api-path-slug: apiv1beta3namespacesname-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: name of the Namespace
      responses:
        200:
          description: OK
      tags:
      - Namespaces
      - Name
  /api/v1beta3/nodes:
    get:
      summary: Get Nodes
      description: List objects of kind node.
      operationId: listNode
      x-api-path-slug: apiv1beta3nodes-get
      responses:
        200:
          description: OK
      tags:
      - Nodes
    post:
      summary: Post Nodes
      description: Create a node.
      operationId: createNode
      x-api-path-slug: apiv1beta3nodes-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Nodes
  /api/v1beta3/nodes/{name}:
    delete:
      summary: Delete Nodes Name
      description: Delete a node.
      operationId: deleteNode
      x-api-path-slug: apiv1beta3nodesname-delete
      parameters:
      - in: path
        name: name
        description: name of the Node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Name
    get:
      summary: Get Nodes Name
      description: Read the specified node.
      operationId: readNode
      x-api-path-slug: apiv1beta3nodesname-get
      parameters:
      - in: path
        name: name
        description: name of the Node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Name
    put:
      summary: Put Nodes Name
      description: Update the specified node.
      operationId: updateNode
      x-api-path-slug: apiv1beta3nodesname-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: name of the Node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Name
  /api/v1beta3/pods:
    get:
      summary: Get Pods
      description: List objects of kind pod.
      operationId: listPod
      x-api-path-slug: apiv1beta3pods-get
      responses:
        200:
          description: OK
      tags:
      - Pods
  /api/v1beta3/proxy/namespaces/{namespaces}/pods/{name}:
    delete:
      summary: Delete Proxy Namespaces Pods Name
      description: Proxy delete requests to pod.
      operationId: proxyDELETEPod
      x-api-path-slug: apiv1beta3proxynamespacesnamespacespodsname-delete
      parameters:
      - in: path
        name: name
        description: name of the Pod
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Namespaces
      - Pods
      - Name
    get:
      summary: Get Proxy Namespaces Pods Name
      description: Proxy get requests to pod.
      operationId: proxyGETPod
      x-api-path-slug: apiv1beta3proxynamespacesnamespacespodsname-get
      parameters:
      - in: path
        name: name
        description: name of the Pod
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Namespaces
      - Pods
      - Name
    post:
      summary: Post Proxy Namespaces Pods Name
      description: Proxy post requests to pod.
      operationId: proxyPOSTPod
      x-api-path-slug: apiv1beta3proxynamespacesnamespacespodsname-post
      parameters:
      - in: path
        name: name
        description: name of the Pod
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Namespaces
      - Pods
      - Name
    put:
      summary: Put Proxy Namespaces Pods Name
      description: Proxy put requests to pod.
      operationId: proxyPUTPod
      x-api-path-slug: apiv1beta3proxynamespacesnamespacespodsname-put
      parameters:
      - in: path
        name: name
        description: name of the Pod
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Namespaces
      - Pods
      - Name
  /api/v1beta3/proxy/namespaces/{namespaces}/pods/{name}/{path:*}:
    delete:
      summary: Delete Proxy Namespaces Pods Name Path *
      description: Proxy delete requests to pod.
      operationId: proxyDELETEPod
      x-api-path-slug: apiv1beta3proxynamespacesnamespacespodsnamepath-delete
      parameters:
      - in: path
        name: name
        description: name of the Pod
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Namespaces
      - Pods
      - Name
      - Path
      - '*'
    get:
      summary: Get Proxy Namespaces Pods Name Path *
      description: Proxy get requests to pod.
      operationId: proxyGETPod
      x-api-path-slug: apiv1beta3proxynamespacesnamespacespodsnamepath-get
      parameters:
      - in: path
        name: name
        description: name of the Pod
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Namespaces
      - Pods
      - Name
      - Path
      - '*'
    post:
      summary: Post Proxy Namespaces Pods Name Path *
      description: Proxy post requests to pod.
      operationId: proxyPOSTPod
      x-api-path-slug: apiv1beta3proxynamespacesnamespacespodsnamepath-post
      parameters:
      - in: path
        name: name
        description: name of the Pod
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Namespaces
      - Pods
      - Name
      - Path
      - '*'
    put:
      summary: Put Proxy Namespaces Pods Name Path *
      description: Proxy put requests to pod.
      operationId: proxyPUTPod
      x-api-path-slug: apiv1beta3proxynamespacesnamespacespodsnamepath-put
      parameters:
      - in: path
        name: name
        description: name of the Pod
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Namespaces
      - Pods
      - Name
      - Path
      - '*'
  /api/v1beta3/proxy/namespaces/{namespaces}/services/{name}:
    delete:
      summary: Delete Proxy Namespaces Services Name
      description: Proxy delete requests to service.
      operationId: proxyDELETEService
      x-api-path-slug: apiv1beta3proxynamespacesnamespacesservicesname-delete
      parameters:
      - in: path
        name: name
        description: name of the Service
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Namespaces
      - Services
      - Name
    get:
      summary: Get Proxy Namespaces Services Name
      description: Proxy get requests to service.
      operationId: proxyGETService
      x-api-path-slug: apiv1beta3proxynamespacesnamespacesservicesname-get
      parameters:
      - in: path
        name: name
        description: name of the Service
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Namespaces
      - Services
      - Name
    post:
      summary: Post Proxy Namespaces Services Name
      description: Proxy post requests to service.
      operationId: proxyPOSTService
      x-api-path-slug: apiv1beta3proxynamespacesnamespacesservicesname-post
      parameters:
      - in: path
        name: name
        description: name of the Service
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Namespaces
      - Services
      - Name
    put:
      summary: Put Proxy Namespaces Services Name
      description: Proxy put requests to service.
      operationId: proxyPUTService
      x-api-path-slug: apiv1beta3proxynamespacesnamespacesservicesname-put
      parameters:
      - in: path
        name: name
        description: name of the Service
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Namespaces
      - Services
      - Name
  /api/v1beta3/proxy/namespaces/{namespaces}/services/{name}/{path:*}:
    delete:
      summary: Delete Proxy Namespaces Services Name Path *
      description: Proxy delete requests to service.
      operationId: proxyDELETEService
      x-api-path-slug: apiv1beta3proxynamespacesnamespacesservicesnamepath-delete
      parameters:
      - in: path
        name: name
        description: name of the Service
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Namespaces
      - Services
      - Name
      - Path
      - '*'
    get:
      summary: Get Proxy Namespaces Services Name Path *
      description: Proxy get requests to service.
      operationId: proxyGETService
      x-api-path-slug: apiv1beta3proxynamespacesnamespacesservicesnamepath-get
      parameters:
      - in: path
        name: name
        description: name of the Service
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Namespaces
      - Services
      - Name
      - Path
      - '*'
    post:
      summary: Post Proxy Namespaces Services Name Path *
      description: Proxy post requests to service.
      operationId: proxyPOSTService
      x-api-path-slug: apiv1beta3proxynamespacesnamespacesservicesnamepath-post
      parameters:
      - in: path
        name: name
        description: name of the Service
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Namespaces
      - Services
      - Name
      - Path
      - '*'
    put:
      summary: Put Proxy Namespaces Services Name Path *
      description: Proxy put requests to service.
      operationId: proxyPUTService
      x-api-path-slug: apiv1beta3proxynamespacesnamespacesservicesnamepath-put
      parameters:
      - in: path
        name: name
        description: name of the Service
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Namespaces
      - Services
      - Name
      - Path
      - '*'
  /api/v1beta3/proxy/nodes/{name}:
    delete:
      summary: Delete Proxy Nodes Name
      description: Proxy delete requests to node.
      operationId: proxyDELETENode
      x-api-path-slug: apiv1beta3proxynodesname-delete
      parameters:
      - in: path
        name: name
        description: name of the Node
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Nodes
      - Name
    get:
      summary: Get Proxy Nodes Name
      description: Proxy get requests to node.
      operationId: proxyGETNode
      x-api-path-slug: apiv1beta3proxynodesname-get
      parameters:
      - in: path
        name: name
        description: name of the Node
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Nodes
      - Name
    post:
      summary: Post Proxy Nodes Name
      description: Proxy post requests to node.
      operationId: proxyPOSTNode
      x-api-path-slug: apiv1beta3proxynodesname-post
      parameters:
      - in: path
        name: name
        description: name of the Node
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Nodes
      - Name
    put:
      summary: Put Proxy Nodes Name
      description: Proxy put requests to node.
      operationId: proxyPUTNode
      x-api-path-slug: apiv1beta3proxynodesname-put
      parameters:
      - in: path
        name: name
        description: name of the Node
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Nodes
      - Name
  /api/v1beta3/proxy/nodes/{name}/{path:*}:
    delete:
      summary: Delete Proxy Nodes Name Path *
      description: Proxy delete requests to node.
      operationId: proxyDELETENode
      x-api-path-slug: apiv1beta3proxynodesnamepath-delete
      parameters:
      - in: path
        name: name
        description: name of the Node
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Nodes
      - Name
      - Path
      - '*'
    get:
      summary: Get Proxy Nodes Name Path *
      description: Proxy get requests to node.
      operationId: proxyGETNode
      x-api-path-slug: apiv1beta3proxynodesnamepath-get
      parameters:
      - in: path
        name: name
        description: name of the Node
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Nodes
      - Name
      - Path
      - '*'
    post:
      summary: Post Proxy Nodes Name Path *
      description: Proxy post requests to node.
      operationId: proxyPOSTNode
      x-api-path-slug: apiv1beta3proxynodesnamepath-post
      parameters:
      - in: path
        name: name
        description: name of the Node
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Nodes
      - Name
      - Path
      - '*'
    put:
      summary: Put Proxy Nodes Name Path *
      description: Proxy put requests to node.
      operationId: proxyPUTNode
      x-api-path-slug: apiv1beta3proxynodesnamepath-put
      parameters:
      - in: path
        name: name
        description: name of the Node
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Nodes
      - Name
      - Path
      - '*'
  /api/v1beta3/redirect/namespaces/{namespaces}/pods/{name}:
    get:
      summary: Get Redirect Namespaces Pods Name
      description: Redirect get request to pod.
      operationId: redirectPod
      x-api-path-slug: apiv1beta3redirectnamespacesnamespacespodsname-get
      parameters:
      - in: path
        name: name
        description: name of the Pod
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Redirect
      - Namespaces
      - Pods
      - Name
  /api/v1beta3/redirect/namespaces/{namespaces}/services/{name}:
    get:
      summary: Get Redirect Namespaces Services Name
      description: Redirect get request to service.
      operationId: redirectService
      x-api-path-slug: apiv1beta3redirectnamespacesnamespacesservicesname-get
      parameters:
      - in: path
        name: name
        description: name of the Service
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Redirect
      - Namespaces
      - Services
      - Name
  /api/v1beta3/redirect/nodes/{name}:
    get:
      summary: Get Redirect Nodes Name
      description: Redirect get request to node.
      operationId: redirectNode
      x-api-path-slug: apiv1beta3redirectnodesname-get
      parameters:
      - in: path
        name: name
        description: name of the Node
      responses:
        200:
          description: OK
      tags:
      - Redirect
      - Nodes
      - Name
  /api/v1beta3/replicationcontrollers:
    get:
      summary: Get Replicationcontrollers
      description: List objects of kind replicationcontroller.
      operationId: listReplicationController
      x-api-path-slug: apiv1beta3replicationcontrollers-get
      responses:
        200:
          description: OK
      tags:
      - Replicationcontrollers
  /api/v1beta3/resourcequotas:
    get:
      summary: Get Resourcequotas
      description: List objects of kind resourcequota.
      operationId: listResourceQuota
      x-api-path-slug: apiv1beta3resourcequotas-get
      responses:
        200:
          description: OK
      tags:
      - Resourcequotas
  /api/v1beta3/secrets:
    get:
      summary: Get Secrets
      description: List objects of kind secret.
      operationId: listSecret
      x-api-path-slug: apiv1beta3secrets-get
      responses:
        200:
          description: OK
      tags:
      - Secrets
  /api/v1beta3/services:
    get:
      summary: Get Services
      description: List objects of kind service.
      operationId: listService
      x-api-path-slug: apiv1beta3services-get
      responses:
        200:
          description: OK
      tags:
      - Services
  /api/v1beta3/watch/endpoints:
    get:
      summary: Get Watch Endpoints
      description: Watch a list of endpoints.
      operationId: watchEndpointslist
      x-api-path-slug: apiv1beta3watchendpoints-get
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Endpoints
  /api/v1beta3/watch/events:
    get:
      summary: Get Watch Events
      description: Watch a list of event.
      operationId: watchEventlist
      x-api-path-slug: apiv1beta3watchevents-get
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Events
  /api/v1beta3/watch/limitranges:
    get:
      summary: Get Watch Limitranges
      description: Watch a list of limitrange.
      operationId: watchLimitRangelist
      x-api-path-slug: apiv1beta3watchlimitranges-get
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Limitranges
  /api/v1beta3/watch/namespaces:
    get:
      summary: Get Watch Namespaces
      description: Watch a list of namespace.
      operationId: watchNamespacelist
      x-api-path-slug: apiv1beta3watchnamespaces-get
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
  /api/v1beta3/watch/namespaces/{namespaces}/endpoints:
    get:
      summary: Get Watch Namespaces Endpoints
      description: Watch a list of endpoints.
      operationId: watchEndpointslist
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesendpoints-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Endpoints
  /api/v1beta3/watch/namespaces/{namespaces}/endpoints/{name}:
    get:
      summary: Get Watch Namespaces Endpoints Name
      description: Watch a particular endpoints.
      operationId: watchEndpoints
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesendpointsname-get
      parameters:
      - in: path
        name: name
        description: name of the Endpoints
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Endpoints
      - Name
  /api/v1beta3/watch/namespaces/{namespaces}/events:
    get:
      summary: Get Watch Namespaces Events
      description: Watch a list of event.
      operationId: watchEventlist
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesevents-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Events
  /api/v1beta3/watch/namespaces/{namespaces}/events/{name}:
    get:
      summary: Get Watch Namespaces Events Name
      description: Watch a particular event.
      operationId: watchEvent
      x-api-path-slug: apiv1beta3watchnamespacesnamespaceseventsname-get
      parameters:
      - in: path
        name: name
        description: name of the Event
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Events
      - Name
  /api/v1beta3/watch/namespaces/{namespaces}/limitranges:
    get:
      summary: Get Watch Namespaces Limitranges
      description: Watch a list of limitrange.
      operationId: watchLimitRangelist
      x-api-path-slug: apiv1beta3watchnamespacesnamespaceslimitranges-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Limitranges
  /api/v1beta3/watch/namespaces/{namespaces}/limitranges/{name}:
    get:
      summary: Get Watch Namespaces Limitranges Name
      description: Watch a particular limitrange.
      operationId: watchLimitRange
      x-api-path-slug: apiv1beta3watchnamespacesnamespaceslimitrangesname-get
      parameters:
      - in: path
        name: name
        description: name of the LimitRange
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Limitranges
      - Name
  /api/v1beta3/watch/namespaces/{namespaces}/pods:
    get:
      summary: Get Watch Namespaces Pods
      description: Watch a list of pod.
      operationId: watchPodlist
      x-api-path-slug: apiv1beta3watchnamespacesnamespacespods-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Pods
  /api/v1beta3/watch/namespaces/{namespaces}/pods/{name}:
    get:
      summary: Get Watch Namespaces Pods Name
      description: Watch a particular pod.
      operationId: watchPod
      x-api-path-slug: apiv1beta3watchnamespacesnamespacespodsname-get
      parameters:
      - in: path
        name: name
        description: name of the Pod
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Pods
      - Name
  /api/v1beta3/watch/namespaces/{namespaces}/replicationcontrollers:
    get:
      summary: Get Watch Namespaces Replicationcontrollers
      description: Watch a list of replicationcontroller.
      operationId: watchReplicationControllerlist
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesreplicationcontrollers-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Replicationcontrollers
  /api/v1beta3/watch/namespaces/{namespaces}/replicationcontrollers/{name}:
    get:
      summary: Get Watch Namespaces Replicationcontrollers Name
      description: Watch a particular replicationcontroller.
      operationId: watchReplicationController
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesreplicationcontrollersname-get
      parameters:
      - in: path
        name: name
        description: name of the ReplicationController
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Replicationcontrollers
      - Name
  /api/v1beta3/watch/namespaces/{namespaces}/resourcequotas:
    get:
      summary: Get Watch Namespaces Resourcequotas
      description: Watch a list of resourcequota.
      operationId: watchResourceQuotalist
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesresourcequotas-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Resourcequotas
  /api/v1beta3/watch/namespaces/{namespaces}/resourcequotas/{name}:
    get:
      summary: Get Watch Namespaces Resourcequotas Name
      description: Watch a particular resourcequota.
      operationId: watchResourceQuota
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesresourcequotasname-get
      parameters:
      - in: path
        name: name
        description: name of the ResourceQuota
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Resourcequotas
      - Name
  /api/v1beta3/watch/namespaces/{namespaces}/secrets:
    get:
      summary: Get Watch Namespaces Secrets
      description: Watch a list of secret.
      operationId: watchSecretlist
      x-api-path-slug: apiv1beta3watchnamespacesnamespacessecrets-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Secrets
  /api/v1beta3/watch/namespaces/{namespaces}/secrets/{name}:
    get:
      summary: Get Watch Namespaces Secrets Name
      description: Watch a particular secret.
      operationId: watchSecret
      x-api-path-slug: apiv1beta3watchnamespacesnamespacessecretsname-get
      parameters:
      - in: path
        name: name
        description: name of the Secret
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Secrets
      - Name
  /api/v1beta3/watch/namespaces/{namespaces}/services:
    get:
      summary: Get Watch Namespaces Services
      description: Watch a list of service.
      operationId: watchServicelist
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesservices-get
      parameters:
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Services
  /api/v1beta3/watch/namespaces/{namespaces}/services/{name}:
    get:
      summary: Get Watch Namespaces Services Name
      description: Watch a particular service.
      operationId: watchService
      x-api-path-slug: apiv1beta3watchnamespacesnamespacesservicesname-get
      parameters:
      - in: path
        name: name
        description: name of the Service
      - in: path
        name: namespaces
        description: object name and auth scope, such as for teams and projects
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Services
      - Name
  /api/v1beta3/watch/namespaces/{name}:
    get:
      summary: Get Watch Namespaces Name
      description: Watch a particular namespace.
      operationId: watchNamespace
      x-api-path-slug: apiv1beta3watchnamespacesname-get
      parameters:
      - in: path
        name: name
        description: name of the Namespace
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Namespaces
      - Name
  /api/v1beta3/watch/nodes:
    get:
      summary: Get Watch Nodes
      description: Watch a list of node.
      operationId: watchNodelist
      x-api-path-slug: apiv1beta3watchnodes-get
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Nodes
  /api/v1beta3/watch/nodes/{name}:
    get:
      summary: Get Watch Nodes Name
      description: Watch a particular node.
      operationId: watchNode
      x-api-path-slug: apiv1beta3watchnodesname-get
      parameters:
      - in: path
        name: name
        description: name of the Node
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Nodes
      - Name
  /api/v1beta3/watch/pods:
    get:
      summary: Get Watch Pods
      description: Watch a list of pod.
      operationId: watchPodlist
      x-api-path-slug: apiv1beta3watchpods-get
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Pods
  /api/v1beta3/watch/replicationcontrollers:
    get:
      summary: Get Watch Replicationcontrollers
      description: Watch a list of replicationcontroller.
      operationId: watchReplicationControllerlist
      x-api-path-slug: apiv1beta3watchreplicationcontrollers-get
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Replicationcontrollers
  /api/v1beta3/watch/resourcequotas:
    get:
      summary: Get Watch Resourcequotas
      description: Watch a list of resourcequota.
      operationId: watchResourceQuotalist
      x-api-path-slug: apiv1beta3watchresourcequotas-get
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Resourcequotas
  /api/v1beta3/watch/secrets:
    get:
      summary: Get Watch Secrets
      description: Watch a list of secret.
      operationId: watchSecretlist
      x-api-path-slug: apiv1beta3watchsecrets-get
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Secrets
  /api/v1beta3/watch/services:
    get:
      summary: Get Watch Services
      description: Watch a list of service.
      operationId: watchServicelist
      x-api-path-slug: apiv1beta3watchservices-get
      responses:
        200:
          description: OK
      tags:
      - Watch
      - Services