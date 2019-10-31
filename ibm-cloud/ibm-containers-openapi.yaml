swagger: "2.0"
x-collection-name: IBM Cloud
x-complete: 1
info:
  title: IBM Containers
  description: containers-are-virtual-software-objects-that-include-all-the-elements-that-an-app-needs-to-run--a-container-has-the-benefits-of-resource-isolation-and-allocation-but-is-more-portable-and-efficient-than-for-example-a-virtual-machine--this-documentation-describes-the-ibm-containers-api-which-is-based-on-the-docker-remote-api--the-api-provides-endpoints-that-you-can-use-to-create-and-manage-your-single-containers-and-container-groups-in-bluemix--endpoints-are-summarized-under-the-following-tags--authentication-retrieve-and-refresh-your-tls-certificates---private-docker-images-registry-create-your-own-private-docker-images-registry-in-bluemix-by-setting-a-namespace-for-your-organization---images-view-build-and-push-your-images-to-your-private-bluemix-registry-so-you-can-use-them-with-ibm-containers--you-can-also-scan-your-container-images-with-the-vulnerability-advisor-against-standard-policies-set-by-the-organization-manager-and-a-database-of-known-ubuntu-issues---single-containers-create-and-manage-single-containers-in-bluemix--use-a-single-container-to-implement-shortlived-processes-or-to-run-simple-tests-as-you-develop-an-app-or-service--to-make-your-single-container-available-from-the-internet-review-the-public-ip-addresses-endpoints---container-groups-create-and-manage-your-container-groups-in-bluemix--a-container-group-consists-of-multiple-single-containers-that-are-all-created-from-the-same-container-image-and-as-a-consequence-are-configured-in-the-same-way--container-groups-offer-further-options-at-no-cost-to-make-your-app-highly-available--these-options-include-inbuilt-load-balancing-autorecovery-of-unhealthy-container-instances-and-autoscaling-of-container-instances-based-on-cpu-and-memory-usage--map-a-public-route-to-your-container-group-to-make-your-app-accessible-from-the-internet----public-ip-addresses-use-these-endpoints-to-request-public-ip-addresses-for-your-space--you-can-bind-this-ip-address-to-your-container-to-make-your-container-accessible-from-the-internet---file-shares-create-list-and-delete-file-shares-in-a-space--a-file-share-is-a-nfs-storage-system-that-hosts-docker-volumes----volumes-create-and-manage-container-volumes-in-your-space-to-persist-the-data-of-your-containers----each-api-request-requires-an-http-header-that-includes-the-xauthtoken-and-xauthprojectid-parameter---xauthtoken-the-json-web-token-jwt-that-you-receive-when-logging-into-the-bluemix-platform--it-allows-you-to-use-the-ibm-containers-rest-api-access-services-and-resources--run-cf-oauthtoken-to-retrieve-your-access-token-information--xauthprojectid-the-unique-id-of-your-organization-space-where-you-want-to-create-or-work-with-your-containers--run-cf-space-space-name-guid-where-space-name-is-the-name-of-your-space-to-retrieve-your-space-id--for-further-information-about-how-containers-work-in-the-ibm-containers-service-review-the-documentation-under-httpsnewconsole-ng-bluemix-netdocscontainerscontainer-index-html--
  version: 3.0.0
host: containers-api.ng.bluemix.net
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /build:
    post:
      summary: Build a Docker image from a Dockerfile
      description: |-
        This API builds a new container image from a Dockerfile that is stored on your local machine and pushes the image to the private Bluemix registry (corresponding IBM Containers command: `cf ic build`).

         To push an image to your Bluemix registry, a namespace must be set for the organization. Run `cf ic namespace get` or call the `GET /registry/namespaces` API to check if a namespace is already set. If not, run `cf ic namespace set NAMESPACE` or call the `PUT /registry/namespaces/{namespace}` API to set a namespace for your organization.
      operationId: this-api-builds-a-new-container-image-from-a-dockerfile-that-is-stored-on-your-local-machine-and-pus
      x-api-path-slug: build-post
      parameters:
      - in: body
        name: file
        description: Must be the content of a tar archive compressed with gzip
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: nocache
        description: If you set the query parameter to `nocache=true`, `nocache=True`,
          or `nocache=1`, the cache will not be used to build your image
      - in: query
        name: pull
        description: If set to pull=true, pull=True, or pull=1, then a newer version
          of the image is always attempted to be pulled even though an older version
          of the image exists locally
      - in: query
        name: q
        description: You can choose whether or not to show the verbose build output
          to review every step during the container image build
      - in: query
        name: t
        description: 'Tag the image with the full path to your private Bluemix registry
          in the following format: `t=registry'
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Build
  /containers/create:
    post:
      summary: Create and start a single container
      description: "This endpoint creates and starts a single container in your space
        based on the Docker image that is specified in the Image field of the request
        json. A single container in IBM Containers is similar to a container that
        you create in your local Docker environment. Single containers are a good
        way to start with IBM Containers and to learn about how containers work in
        the IBM Cloud and the features that IBM Containers provides. They are also
        recommended when you want to run simple app tests or during the development
        process of an app. \n\n In the Docker API there are two separate APIs to create
        and start a container. However in IBM Containers a container is created and
        started in a single API call. Therefore, this API merges parameters from the
        Docker API to create and start container. \n\n To create a container with
        IBM Containers, you must at least define the image that the container is based
        on.\n\n- Image: You must include the full path to the image in your private
        Bluemix registry in the format: `registry.ng.bluemix.net/<namespace>/<image>`."
      operationId: this-endpoint-creates-and-starts-a-single-container-in-your-space-based-on-the-docker-image-that-is-
      x-api-path-slug: containerscreate-post
      parameters:
      - in: query
        name: name
        description: Choose a name for your container
      - in: body
        name: Param
        description: Summary of input parameter to create a container in IBM Containers
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Create
  /containers/floating-ips:
    get:
      summary: List available public IP addresses in a space
      description: 'This endpoint returns a list of all public IP addresses that are
        allocated to a space and not bound to a container. If you want to list all
        public IP addresses that are allocated to a space, even those that are already
        bound to a container, use the `all` query parameter (corrsponding IBM Containers
        command: `cf ic ip list`).'
      operationId: this-endpoint-returns-a-list-of-all-public-ip-addresses-that-are-allocated-to-a-space-and-not-bound-
      x-api-path-slug: containersfloatingips-get
      parameters:
      - in: query
        name: all
        description: If this option is set to `all=1`, `all=True`, or `all=true`,
          all public IP addresses that are allocated to a space are returned
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Floating-ips
  /containers/floating-ips/request:
    post:
      summary: Request a public IP address for a space
      description: 'This endpoint requests a new public IP address for a space (corresponding
        IBM Containers command: `cf ic ip request`). The number of public IP addresses
        depends on the quota that is assigned to the space. If there is not enough
        quota left to request a new public IP address, you can either contact your
        organization manager to increase the quota, or unbind an existing IP address
        from a container by running `cf ic ip unbind <ip_adress> <container>` command,
        or  calling the `POST /container/{name_or_id}/floating-ips/{ip}/unbind` endpoint.'
      operationId: this-endpoint-requests-a-new-public-ip-address-for-a-space-corresponding-ibm-containers-command-cf-i
      x-api-path-slug: containersfloatingipsrequest-post
      parameters:
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Floating-ips
      - Request
  /containers/floating-ips/{ip}/release:
    post:
      summary: Release public IP address
      description: 'This endpoint releases a public IP address from a space (corresponding
        IBM Containers command: `cf ic ip release <ip_adress>`). The public IP address
        is no longer allocated to the space. If a container was bound to the IP address,
        it is automatically unbound.'
      operationId: this-endpoint-releases-a-public-ip-address-from-a-space-corresponding-ibm-containers-command-cf-ic-i
      x-api-path-slug: containersfloatingipsiprelease-post
      parameters:
      - in: path
        name: ip
        description: The public IP address that you want to release
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Floating-ips
      - Ip
      - Release
  /containers/groups:
    get:
      summary: List all container groups in a space
      description: 'This endpoint returns a list of all container groups in a space
        independent of their current state. (corresponding IBM Containers command:
        `cf ic group list`).'
      operationId: this-endpoint-returns-a-list-of-all-container-groups-in-a-space-independent-of-their-current-state--
      x-api-path-slug: containersgroups-get
      parameters:
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Groups
    post:
      summary: Create and start a container group.
      description: "This endpoint creates and starts a new container group in your
        space. A container group consists of two or more single containers that are
        all created from the same container image and as a consequence are configured
        in the same way. Container groups offer different options at no cost to make
        your app highly available, such as in-built load balancing, auto-recovery
        of unhealthy container instances, and auto-scaling of container instances
        based on CPU and memory usage.\n\nTo create a container group with IBM Containers,
        you must at least define a container group name and the image that the container
        group is based on. Required attributes:\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n-
        Name: The container group name must start with a letter and then can include
        uppercase letters, lowercase letters, numbers, periods (.), underscores (_),
        or hyphens (-). \n- Image: You must include the full path to the image in
        your private Bluemix registry in the format:`registry.ng.bluemix.net/<namespace>/<image>`."
      operationId: this-endpoint-creates-and-starts-a-new-container-group-in-your-space--a-container-group-consists-of-
      x-api-path-slug: containersgroups-post
      parameters:
      - in: body
        name: RequiredAttributes
        description: Attributes that are required to create a container group in your
          space
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Groups
  /containers/groups/{name_or_id}:
    delete:
      summary: Stop and delete all container instances in a container group.
      description: 'Stops and deletes the container instances that run in a container
        group (corresponding IBM Containers command: `cf ic group rm <group_name>`).
        When you delete a container group, all floating private IP addresses are released.'
      operationId: stops-and-deletes-the-container-instances-that-run-in-a-container-group-corresponding-ibm-containers
      x-api-path-slug: containersgroupsname-or-id-delete
      parameters:
      - in: query
        name: force
        description: If you want to force the deletion of a container group that has
          running container instances, use the force option
      - in: path
        name: name_or_id
        description: The name or unique ID of the container group that you want to
          delete
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Groups
      - Name
    get:
      summary: Inspect a container group.
      description: 'This endpoint retrieves detailed information about a container
        group with a given name (corresponding IBM Containers command: `cf ic group
        inspect GROUP`).'
      operationId: this-endpoint-retrieves-detailed-information-about-a-container-group-with-a-given-name-corresponding
      x-api-path-slug: containersgroupsname-or-id-get
      parameters:
      - in: path
        name: name_or_id
        description: The name or unique ID of the container group that you want to
          inspect
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Groups
      - Name
    patch:
      summary: Update a container group.
      description: "Update the number of container instances that run in a container
        group (corresponding IBM Containers command: `cf ic group update <option>
        <group>`). \n\nNote: You can run only one update at a time.  \n\n The desired
        number is the number of container instances that you require. It must be within
        the current limits of Max and Min. To increase the number of desired container
        instances above the Max value, you must first execute an update on the Max
        value. Once this update is completed, you can increase the desired number
        of container instances."
      operationId: update-the-number-of-container-instances-that-run-in-a-container-group-corresponding-ibm-containers-
      x-api-path-slug: containersgroupsname-or-id-patch
      parameters:
      - in: path
        name: name_or_id
        description: The name or unique ID of the container group that you want to
          update
      - in: body
        name: Updates
        description: The container group parameter that you want to update
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Groups
      - Name
  /containers/groups/{name_or_id}/maproute:
    post:
      summary: Map a public route to a container group.
      description: 'If you want your container group to be accessible from the Internet,
        you need to expose a public port and map a public route to it (corresponding
        IBM Containers command: `cf ic route map -n <host> -d <domain> <group>`).
        Every route consists of the host name and domain.'
      operationId: if-you-want-your-container-group-to-be-accessible-from-the-internet-you-need-to-expose-a-public-port
      x-api-path-slug: containersgroupsname-or-idmaproute-post
      parameters:
      - in: path
        name: name_or_id
        description: The name or unique ID of the container group to which you want
          to map a public route
      - in: body
        name: Route
        description: The public route that is mapped to the container group
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Groups
      - Name
      - Maproute
  /containers/groups/{name_or_id}/unmaproute:
    post:
      summary: Unmap a public route from a container group
      description: "This endpoint unmaps a public route from a container group (corresponding
        IBM Containers command: `cf ic route unmap -n <host> -d <domain> <group>`).
        If no other public route is mapped to the container group, then the container
        group is no longer available from the internet. \n\n When you unmap a route
        from a container group, the route is not deleted and can be mapped to other
        container groups."
      operationId: this-endpoint-unmaps-a-public-route-from-a-container-group-corresponding-ibm-containers-command-cf-i
      x-api-path-slug: containersgroupsname-or-idunmaproute-post
      parameters:
      - in: path
        name: name_or_id
        description: The name or unique ID (UUID) of the container group that you
          want to inspect
      - in: body
        name: Route
        description: The public route that is unmapped from the container group
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Groups
      - Name
      - Unmaproute
  /containers/json:
    get:
      summary: List single containers in a space.
      description: 'This endpoint returns a list of all single containers in a space
        that are currently in a running state (corresponding IBM Containers command:
        `cf ic ps`). To list all single containers independent of their current state,
        set the `all` query parameter to true.'
      operationId: this-endpoint-returns-a-list-of-all-single-containers-in-a-space-that-are-currently-in-a-running-sta
      x-api-path-slug: containersjson-get
      parameters:
      - in: query
        name: all
        description: By default, the `GET /containers/json` endpoint returns a list
          of all single containers in a space that are in a running state
      - in: query
        name: filters
        description: You can filter your containers by any environment variable key
          or value that is listed in the `Env` section of your CLI/ API response when
          you run the `cf ic inspect ` command, or call the `GET /containers/{id}/json`
          endpoint
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Json
  /containers/messages:
    get:
      summary: List messages for the user
      description: This endpoint retrieves all IBM Containers system messages for
        the user.
      operationId: this-endpoint-retrieves-all-ibm-containers-system-messages-for-the-user-
      x-api-path-slug: containersmessages-get
      parameters:
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Messages
  /containers/quota:
    get:
      summary: Retrieve organization and space specific quota
      description: Retrieve the quota that is assigned to the organization and space.
      operationId: retrieve-the-quota-that-is-assigned-to-the-organization-and-space-
      x-api-path-slug: containersquota-get
      parameters:
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Quota
    put:
      summary: Update space quota
      description: "This endpoint updates the quota that is allocated to a Bluemix
        space. \n\n **Note**: Only paid accounts are eligbile to update the space
        quota. If you are using a free-trial account, upgrade to a paid account first."
      operationId: this-endpoint-updates-the-quota-that-is-allocated-to-a-bluemix-space---note-only-paid-accounts-are-e
      x-api-path-slug: containersquota-put
      parameters:
      - in: body
        name: ContainersQuotaList
        description: The space quota details that you want to update
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Quota
  /containers/usage:
    get:
      summary: List container sizes and quota limits
      description: "This endpoint returns a list of available container sizes and
        the quota limit and usage for the space. \n\n- Container sizes: A list of
        available container sizes indicating the amount of container memory, disk
        space and virtual CPUs that can be assigned to the container.\n- Quota limit:
        Lists the number of containers, public IP addresses, available container memory,
        and virtual CPUS that are allocated to a space. \n- Quota usage: Lists the
        current number of containers, images, and public IP addresses in a space that
        is counted towards your quota limit."
      operationId: this-endpoint-returns-a-list-of-available-container-sizes-and-the-quota-limit-and-usage-for-the-spac
      x-api-path-slug: containersusage-get
      parameters:
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Usage
  /containers/version:
    get:
      summary: List latest API version
      description: This endpoint retrieves a list of all microservices that are used
        in the IBM Containers service with their current build version. This method
        does not require authentication.
      operationId: this-endpoint-retrieves-a-list-of-all-microservices-that-are-used-in-the-ibm-containers-service-with
      x-api-path-slug: containersversion-get
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Version
  /containers/{id}/status:
    get:
      summary: List the current state of a container.
      description: This endpoint returns the current state of a container. This state
        can either be a transient state, such as BUILDING and NETWORKING, or a non-transient
        state, such as RUNNING, SHUTDOWN, CRASHED, or SUSPENDED.
      operationId: this-endpoint-returns-the-current-state-of-a-container--this-state-can-either-be-a-transient-state-s
      x-api-path-slug: containersidstatus-get
      parameters:
      - in: path
        name: id
        description: The unique identifier that represents the container
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Status
  /containers/{name_or_id}:
    delete:
      summary: Remove a single container
      description: 'Remove a single container that is identified by container ID or
        name from a space (corresponding IBM Containers command: `cf ic delete <container>`).
        The container must be stopped before it can be deleted, unless the `force`
        query parameter is set to true.'
      operationId: remove-a-single-container-that-is-identified-by-container-id-or-name-from-a-space-corresponding-ibm-
      x-api-path-slug: containersname-or-id-delete
      parameters:
      - in: query
        name: force
        description: Use the `force` query parameter if you want to delete the container
          independent of their current state
      - in: path
        name: name_or_id
        description: The unique identifier or name of the container that you want
          to delete
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Name
  /containers/{name_or_id}/floating-ips/{ip}/bind:
    post:
      summary: Bind a public IP address to a single container
      description: 'This endpoint binds an available public IP address to a single
        container (corresponding IBM Containers command: `cf ic ip bind <ip_adress>
        <container>`). After a container is bound to a public IP address, it can be
        accessed at `https://<public_ip_adress>:<public_port>`.'
      operationId: this-endpoint-binds-an-available-public-ip-address-to-a-single-container-corresponding-ibm-container
      x-api-path-slug: containersname-or-idfloatingipsipbind-post
      parameters:
      - in: path
        name: ip
        description: The public IP address that you want to bind to your container
      - in: path
        name: name_or_id
        description: The name or ID of the container that you want to bind to the
          public IP address
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Name
      - Floating-ips
      - Ip
      - Bind
  /containers/{name_or_id}/floating-ips/{ip}/unbind:
    post:
      summary: Unbind a public IP address from a container
      description: 'This endpoint unbinds a public IP address from a container (corresponding
        IBM Containers command: `cf ic ip unbind <ip_adress> <container>`). The container
        that is unbound from the IP address will not be accessible from the internet
        anymore. The public IP address will be further allocated to the space and
        can be used to be bound to other containers.'
      operationId: this-endpoint-unbinds-a-public-ip-address-from-a-container-corresponding-ibm-containers-command-cf-i
      x-api-path-slug: containersname-or-idfloatingipsipunbind-post
      parameters:
      - in: path
        name: ip
        description: The public IP address that you want to unbind from your container
      - in: path
        name: name_or_id
        description: The name or ID of the container that you want to bind to the
          public IP address
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Name
      - Floating-ips
      - Ip
      - Unbind
  /containers/{name_or_id}/json:
    get:
      summary: Inspect a single container
      description: 'This endpoint retrieves detailed information about a single container
        (corresponding IBM Containers command: `cf ic inspect <container>`).'
      operationId: this-endpoint-retrieves-detailed-information-about-a-single-container-corresponding-ibm-containers-c
      x-api-path-slug: containersname-or-idjson-get
      parameters:
      - in: path
        name: name_or_id
        description: The name or ID of the container that you want to inspect
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Name
      - Json
  /containers/{name_or_id}/pause:
    post:
      summary: Pause a single container
      description: 'Pause all processes in a running single container with a given
        container ID or name (corresponding IBM Containers command: `cf ic pause <container>`).'
      operationId: pause-all-processes-in-a-running-single-container-with-a-given-container-id-or-name-corresponding-ib
      x-api-path-slug: containersname-or-idpause-post
      parameters:
      - in: path
        name: name_or_id
        description: The unique identifier or name of the container that you want
          to pause
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Name
      - Pause
  /containers/{name_or_id}/rename:
    post:
      summary: Rename a single container
      description: 'Change the current name of an existing single container that is
        identified by the container ID or name (corresponding IBM Containers command:
        `cf ic rename <old_name> <new_name>`).'
      operationId: change-the-current-name-of-an-existing-single-container-that-is-identified-by-the-container-id-or-na
      x-api-path-slug: containersname-or-idrename-post
      parameters:
      - in: query
        name: name
        description: The new name for the container
      - in: path
        name: name_or_id
        description: The unique identifier or name of the container that you want
          to rename
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Name
      - Rename
  /containers/{name_or_id}/restart:
    post:
      summary: Restart a single container
      description: 'Restart a container with a given container ID or name (corresponding
        IBM Containers command: `cf ic restart <container>`).'
      operationId: restart-a-container-with-a-given-container-id-or-name-corresponding-ibm-containers-command-cf-ic-res
      x-api-path-slug: containersname-or-idrestart-post
      parameters:
      - in: path
        name: name_or_id
        description: The unique identifier or name of the container that you want
          to restart
      - in: query
        name: t
        description: The number of seconds to wait before the container is restarted
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Name
      - Restart
  /containers/{name_or_id}/start:
    post:
      summary: Start a single container
      description: 'Start a single container with a given container name or ID (corresponding
        IBM Containers command: `cf ic start <container>`).'
      operationId: start-a-single-container-with-a-given-container-name-or-id-corresponding-ibm-containers-command-cf-i
      x-api-path-slug: containersname-or-idstart-post
      parameters:
      - in: path
        name: name_or_id
        description: The unique identifier or name of the container that you want
          to start
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Name
      - Start
  /containers/{name_or_id}/stop:
    post:
      summary: Stop a single container
      description: 'Stop a single container with a given container name or ID (corresponding
        IBM Containers command: `cf ic stop <container>`).'
      operationId: stop-a-single-container-with-a-given-container-name-or-id-corresponding-ibm-containers-command-cf-ic
      x-api-path-slug: containersname-or-idstop-post
      parameters:
      - in: path
        name: name_or_id
        description: The unique identifier or name of the container that you want
          to stop
      - in: query
        name: t
        description: The number of seconds to wait before the container is stopped
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Name
      - Stop
  /containers/{name_or_id}/unpause:
    post:
      summary: Unpause a single container
      description: 'Unpause all processes that are currently stopped inside a single
        containers with a given container ID or name (corresponding IBM Containers
        command: `cf ic unpause <container>`).'
      operationId: unpause-all-processes-that-are-currently-stopped-inside-a-single-containers-with-a-given-container-i
      x-api-path-slug: containersname-or-idunpause-post
      parameters:
      - in: path
        name: name_or_id
        description: The unique identifier or name of the container that you want
          to unpause
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Name
      - Unpause
  /images/json:
    get:
      summary: List all Docker images that are available in your private Bluemix registry.
      description: 'This endpoint returns a list of all available Docker images in
        a private Bluemix registry (corresponding IBM Containers command: `cf ic images`.'
      operationId: this-endpoint-returns-a-list-of-all-available-docker-images-in-a-private-bluemix-registry-correspond
      x-api-path-slug: imagesjson-get
      parameters:
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Images
      - Json
  /images/{id}:
    delete:
      summary: Remove a Docker image.
      description: 'Remove a Docker image from the private Bluemix registry that is
        identified by the image ID (corresponding IBM Containers command: `cf ic rmi
        <image>`).'
      operationId: remove-a-docker-image-from-the-private-bluemix-registry-that-is-identified-by-the-image-id-correspon
      x-api-path-slug: imagesid-delete
      parameters:
      - in: path
        name: id
        description: The unique identifier representing a Docker image
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Images
  /images/{name_or_id}/json:
    get:
      summary: Inspect a Docker image in private Bluemix registry
      description: 'This endpoint returns detailed information about a Docker image
        that is stored in the private Bluemix registry of an organization (corresponding
        IBM Containers command: `cf ic inspect <image_name_or_id>`).'
      operationId: this-endpoint-returns-detailed-information-about-a-docker-image-that-is-stored-in-the-private-bluemi
      x-api-path-slug: imagesname-or-idjson-get
      parameters:
      - in: path
        name: name_or_id
        description: The full private Bluemix registry path to your image or the unique
          ID of the image that you want to inspect
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Images
      - Name
      - Json
  /registry/namespaces:
    get:
      summary: Retrieve the namespace of an organization.
      description: 'This endpoint retrieves the namespace that was set for the organization
        that owns the current space (corresponding IBM Containers command: `cf ic
        namespace get`).'
      operationId: this-endpoint-retrieves-the-namespace-that-was-set-for-the-organization-that-owns-the-current-space-
      x-api-path-slug: registrynamespaces-get
      parameters:
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Registry
      - Namespaces
  /registry/namespaces/{namespace}:
    get:
      summary: Check the availability of a namespace
      description: "This endpoint checks whether a namespace is available in Bluemix
        and can be used to set up the private Docker images registry for an organization.
        When a HTTP code `201 Ok` is returned, the namespace is already assigned to
        another organization in Bluemix and cannot be used. When a HTTP code `404
        Not found` is returned, the namespace can be used for your organization. \n\n
        Consider the following rules when choosing a namespace for your organization:
        \n\n- Every organization can have one namespace at a time only \n- The namespace
        must be unique in Bluemix. \n- The namespace can be 4-30 characters long.
        \n- The namespace must start with at least one letter or number. \n- The namespace
        can only contain lowercase letters, numbers or underscores (_)."
      operationId: this-endpoint-checks-whether-a-namespace-is-available-in-bluemix-and-can-be-used-to-set-up-the-priva
      x-api-path-slug: registrynamespacesnamespace-get
      parameters:
      - in: path
        name: namespace
        description: The name of the namespace that you would like to use for your
          organization and for which you would like to check availability in Bluemix
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Registry
      - Namespaces
      - Namespace
    put:
      summary: Set a namespace for your private Bluemix registry.
      description: "Set up your own Docker images registry in Bluemix by defining
        a namespace for your organization (corresponding IBM Containers command: `cf
        ic namespace set <namespace>`). The namespace is used to generate a unique
        URL to your private Bluemix registry. In your private registry you store all
        Docker images that you want to share across your organization. To create a
        container from an image, you must first push the image to your registry. \n\n
        The namespace cannot be changed after is has been set. Consider the following
        rules to choose a namespace for your organization: \n\n- Every organization
        can have one namespace at a time only \n- The namespace must be unique in
        Bluemix. \n- The namespace can be 4-30 characters long. \n- The namespace
        must start with at least one letter or number. \n- The namespace can only
        contain lowercase letters, numbers or underscores (_)."
      operationId: set-up-your-own-docker-images-registry-in-bluemix-by-defining-a-namespace-for-your-organization-corr
      x-api-path-slug: registrynamespacesnamespace-put
      parameters:
      - in: path
        name: namespace
        description: The name for your namespace to create your private Docker images
          registry in Bluemix
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Registry
      - Namespaces
      - Namespace
  /tlskey:
    get:
      summary: Retrieve the TLS Certificate
      description: 'This endpoint returns the TLS (Transport Layer Security) certificate
        to the user (corresponding IBM Containers command: `cf ic login`). The TLS
        certificate is a SSL certificate that is used to authenticate the user''s
        CLI with the IBM Containers service and to establish a secure communication
        between the user''s local machine and the container in Bluemix.'
      operationId: this-endpoint-returns-the-tls-transport-layer-security-certificate-to-the-user-corresponding-ibm-con
      x-api-path-slug: tlskey-get
      parameters:
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Tlskey
  /tlskey/refresh:
    put:
      summary: Refresh the TLS Certificate
      description: 'This endpoint requests to generate a new TLS (Transport Layer
        Security) certificate on the server and to update the existing user TLS certificate
        (corresponding IBM Containers command: `cf ic init`).'
      operationId: this-endpoint-requests-to-generate-a-new-tls-transport-layer-security-certificate-on-the-server-and-
      x-api-path-slug: tlskeyrefresh-put
      parameters:
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Tlskey
      - Refresh
  /volumes/create:
    post:
      summary: Create a volume in a space
      description: "This endpoints creates a new volume in your space (corresponding
        IBM Containers command: `cf ic volume create VOLNAME`). A volume is used to
        persist and access app data between container restarts. Volumes are hosted
        on file shares that define the available actual storage in Bluemix and the
        number of input and output transactions per second (IOPS). \n\n After you
        have created a volume, you must mount it to a container by using the `--volume`
        option in the `cf ic run` (single containers) or `cf ic group create` (container
        groups) command. You can also define the volume as part of the HTTP body and
        send a request to the `POST /containers/create` (single containers) or `POST
        /containers/groups` (container groups) endpoints. \n\n Note: If you mount
        multiple containers in a space to the same volume, they share the data in
        the volume and can access them anytime. When a container is deleted, the associated
        volume is not removed."
      operationId: this-endpoints-creates-a-new-volume-in-your-space-corresponding-ibm-containers-command-cf-ic-volume-
      x-api-path-slug: volumescreate-post
      parameters:
      - in: query
        name: fsName
        description: The name of the file share that the volume is hosted on
      - in: query
        name: name
        description: The name of the volume
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Volumes
      - Create
  /volumes/fs/create:
    post:
      summary: Create a file share in a space
      description: "This endpoint creates a new file share in a space (corresponding
        IBM Containers command: `cf ic volume fs-create FSNAME FSSIZE FSIOPS`). \n\n
        A file share is a persistent NFS-based (Network File System) storage system
        that hosts Docker volumes in a Bluemix space and allows a user to store and
        access container and app-related files. To store files in a file share, you
        must create a container volume and save the data into this volume.\n\n As
        soon as you create your first volume in a space with the `cf ic volume create
        VOLNAME` command or the `POST /volumes/create` API endpoint, a default file
        share with 20 GB at 4 IOPS (Input Output operations Per Second) is created
        at no cost. \n\nThe organization manager can create file shares with specific
        storage size and IOPS to meet the storage needs of the space. File shares
        can be provisioned in sizes from 20 GB to 12 TB and at IOPS per GB of 0.25,
        2 or 4. Run `cf ic volume fs-flavor-list` or call the `GET /volumes/fs/flavors/json`
        API endpoint to retrieve a list of available file share sizes. The file share
        size in relation to the number of IOPS impacts the speed that data can be
        read and written from and to the container volume."
      operationId: this-endpoint-creates-a-new-file-share-in-a-space-corresponding-ibm-containers-command-cf-ic-volume-
      x-api-path-slug: volumesfscreate-post
      parameters:
      - in: body
        name: FileshareParam
        description: The input parameter to create a new file share in a space
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Volumes
      - Create
  /volumes/fs/flavors/json:
    get:
      summary: List available file share sizes
      description: 'This endpoint returns a list of available file shares in gigabyte
        (corresponding IBM Containers command: `cf ic volume fs-flavor-list`).'
      operationId: this-endpoint-returns-a-list-of-available-file-shares-in-gigabyte-corresponding-ibm-containers-comma
      x-api-path-slug: volumesfsflavorsjson-get
      parameters:
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Volumes
      - Flavors
      - Json
  /volumes/fs/json:
    get:
      summary: List available file shares in a space
      description: 'This endpoint returns a list of all file shares that are availble
        in a space (corresponding IBM Containers command: `cf ic volume fs-list`).'
      operationId: this-endpoint-returns-a-list-of-all-file-shares-that-are-availble-in-a-space-corresponding-ibm-conta
      x-api-path-slug: volumesfsjson-get
      parameters:
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Volumes
      - Json
  /volumes/fs/{name}:
    delete:
      summary: Delete a file share
      description: "This endpoint deletes a file share from a space (corresponding
        IBM Containers command: `cf ic volume fs-rm FSNAME`).\n\n Before you can delete
        a file share, all mounted volumes must be deleted first. To delete a volume,
        run `cf ic volume rm VOLNAME` or call the `DELETE /volumes/{name}` API endpoint.
        \n\n **Note:** To delete a file share you must have been granted organization
        developer rights."
      operationId: this-endpoint-deletes-a-file-share-from-a-space-corresponding-ibm-containers-command-cf-ic-volume-fs
      x-api-path-slug: volumesfsname-delete
      parameters:
      - in: path
        name: name
        description: The name of the file share that you want to delete
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Volumes
      - Name
  /volumes/fs/{name}/json:
    get:
      summary: Inspect a file share
      description: 'This endpoint returns detailed information about a file share
        (corresponding IBM Containers command: `cf ic volume fs-inspect FSNAME`).'
      operationId: this-endpoint-returns-detailed-information-about-a-file-share-corresponding-ibm-containers-command-c
      x-api-path-slug: volumesfsnamejson-get
      parameters:
      - in: path
        name: name
        description: The name of the file share that you want to inspect
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Volumes
      - Name
      - Json
  /volumes/json:
    get:
      summary: List all volumes for a space
      description: 'This endpoint returns a list of all volumes that are available
        in the given space (corresponding IBM Containers command: `cf ic volume list`).'
      operationId: this-endpoint-returns-a-list-of-all-volumes-that-are-available-in-the-given-space-corresponding-ibm-
      x-api-path-slug: volumesjson-get
      parameters:
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Volumes
      - Json
  /volumes/{name}:
    delete:
      summary: Delete a volume
      description: 'Delete a volume with a given name from a space (corresponding
        IBM Containers command: `cf ic volume rm VOLNAME`). To delete a volume, all
        mounted containers must be unmounted first. After the volume is deleted, the
        data that are stored in the volume are lost.'
      operationId: delete-a-volume-with-a-given-name-from-a-space-corresponding-ibm-containers-command-cf-ic-volume-rm-
      x-api-path-slug: volumesname-delete
      parameters:
      - in: path
        name: name
        description: The name of the volume that you want to delete
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Volumes
      - Name
    post:
      summary: Share a volume with another space
      description: This endpoint provisions an existing volume that was created in
        one space to another space within the same organization. Single containers
        and container groups in each space can read and write to the shared volume.
        The volume remains owned by the original space it was created in, including
        management and billing. For example, the volume can be deleted from the original
        space only.
      operationId: this-endpoint-provisions-an-existing-volume-that-was-created-in-one-space-to-another-space-within-th
      x-api-path-slug: volumesname-post
      parameters:
      - in: path
        name: name
        description: The name of the volume that you want to share with another space
          in your organization
      - in: body
        name: volumeParam
        description: Input parameter that are required to provision an existing volume
          to a new space and to unprovision it from a space
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Volumes
      - Name
  /volumes/{name}/json:
    get:
      summary: Retrieve detailed information about a volume.
      description: 'Retrieve a detailed list of information about a volume that is
        identified by the volume name (corresponding IBM Containers command: `cf ic
        volume inspect VOLNAME`).'
      operationId: retrieve-a-detailed-list-of-information-about-a-volume-that-is-identified-by-the-volume-name-corresp
      x-api-path-slug: volumesnamejson-get
      parameters:
      - in: path
        name: name
        description: The name of the volume, for which you want to retrieve detailed
          information
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Volumes
      - Name
      - Json