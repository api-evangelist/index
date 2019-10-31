swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 1
info:
  title: AWS Lightsale API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AllocateStaticIp:
    get:
      summary: Allocate Static Ip
      description: Allocates a static IP address.
      operationId: allocateStaticIp
      x-api-path-slug: actionallocatestaticip-get
      parameters:
      - in: query
        name: staticIpName
        description: The name of the static IP address
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Addresses
  /?Action=AttachStaticIp:
    get:
      summary: Attach Static Ip
      description: Attaches a static IP address to a specific Amazon Lightsail instance.
      operationId: attachStaticIp
      x-api-path-slug: actionattachstaticip-get
      parameters:
      - in: query
        name: instanceName
        description: The instance name to which you want to attach the static IP address
        type: string
      - in: query
        name: staticIpName
        description: The name of the static IP
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Addresses
  /?Action=CloseInstancePublicPorts:
    get:
      summary: Close Instance Public Ports
      description: Closes the public ports on a specific Amazon Lightsail instance.
      operationId: closeInstancePublicPorts
      x-api-path-slug: actioncloseinstancepublicports-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance on which youre attempting to close the
          public      ports
        type: string
      - in: query
        name: portInfo
        description: Information about the public port you are trying to close
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=CreateDomain:
    get:
      summary: Create Domain
      description: Creates a domain resource for the specified domain (e.
      operationId: createDomain
      x-api-path-slug: actioncreatedomain-get
      parameters:
      - in: query
        name: domainName
        description: The domain name to manage (e
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=CreateDomainEntry:
    get:
      summary: Create Domain Entry
      description: |-
        Creates one of the following entry records associated with the domain: A record, CNAME
              record, TXT record, or MX record.
      operationId: createDomainEntry
      x-api-path-slug: actioncreatedomainentry-get
      parameters:
      - in: query
        name: domainEntry
        description: An array of key-value pairs containing information about the
          domain entry      request
        type: string
      - in: query
        name: domainName
        description: The domain name (e
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=CreateInstances:
    get:
      summary: Create Instances
      description: |-
        Creates one or more Amazon Lightsail virtual private servers, or
                instances.
      operationId: createInstances
      x-api-path-slug: actioncreateinstances-get
      parameters:
      - in: query
        name: availabilityZone
        description: The Availability Zone in which to create your instance
        type: string
      - in: query
        name: blueprintId
        description: The ID for a virtual private server image (e
        type: string
      - in: query
        name: bundleId
        description: The bundle of specification information for your virtual private
          server (or        instance), including the pricing plan (e
        type: string
      - in: query
        name: customImageName
        description: The name for your custom image
        type: string
      - in: query
        name: instanceNames
        description: The names to use for your new Lightsail instances
        type: string
      - in: query
        name: keyPairName
        description: The name of your key pair
        type: string
      - in: query
        name: userData
        description: A launch script you can create that configures a server with
          additional user data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=CreateInstancesFromSnapshot:
    get:
      summary: Create Instances From Snapshot
      description: |-
        Uses a specific snapshot as a blueprint for creating one or more new instances that are
              based on that identical configuration.
      operationId: createInstancesFromSnapshot
      x-api-path-slug: actioncreateinstancesfromsnapshot-get
      parameters:
      - in: query
        name: availabilityZone
        description: The Availability Zone where you want to create your instances
        type: string
      - in: query
        name: bundleId
        description: The bundle of specification information for your virtual private
          server (or        instance), including the pricing plan (e
        type: string
      - in: query
        name: instanceNames
        description: The names for your new instances
        type: string
      - in: query
        name: instanceSnapshotName
        description: The name of the instance snapshot on which you are basing your
          new instances
        type: string
      - in: query
        name: keyPairName
        description: The name for your key pair
        type: string
      - in: query
        name: userData
        description: You can create a launch script that configures a server with
          additional user data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=CreateInstanceSnapshot:
    get:
      summary: Create Instance Snapshot
      description: |-
        Creates a snapshot of a specific virtual private server, or
                instance.
      operationId: createInstanceSnapshot
      x-api-path-slug: actioncreateinstancesnapshot-get
      parameters:
      - in: query
        name: instanceName
        description: The Lightsail instance on which to base your snapshot
        type: string
      - in: query
        name: instanceSnapshotName
        description: The name for your new snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=CreateKeyPair:
    get:
      summary: Create Key Pair
      description: Creates sn SSH key pair.
      operationId: createKeyPair
      x-api-path-slug: actioncreatekeypair-get
      parameters:
      - in: query
        name: keyPairName
        description: The name for your new key pair
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pairs
  /?Action=DeleteDomain:
    get:
      summary: Delete Domain
      description: Deletes the specified domain recordset and all of its domain records.
      operationId: deleteDomain
      x-api-path-slug: actiondeletedomain-get
      parameters:
      - in: query
        name: domainName
        description: The specific domain name to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=DeleteDomainEntry:
    get:
      summary: Delete Domain Entry
      description: Deletes a specific domain entry.
      operationId: deleteDomainEntry
      x-api-path-slug: actiondeletedomainentry-get
      parameters:
      - in: query
        name: domainEntry
        description: An array of key-value pairs containing information about your
          domain entries
        type: string
      - in: query
        name: domainName
        description: The name of the domain entry to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=DeleteInstance:
    get:
      summary: Delete Instance
      description: |-
        Deletes a specific Amazon Lightsail virtual private server, or
                instance.
      operationId: deleteInstance
      x-api-path-slug: actiondeleteinstance-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=DeleteInstanceSnapshot:
    get:
      summary: Delete Instance Snapshot
      description: |-
        Deletes a specific snapshot of a virtual private server (or
                instance).
      operationId: deleteInstanceSnapshot
      x-api-path-slug: actiondeleteinstancesnapshot-get
      parameters:
      - in: query
        name: instanceSnapshotName
        description: The name of the snapshot to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=DeleteKeyPair:
    get:
      summary: Delete Key Pair
      description: Deletes a specific SSH key pair.
      operationId: deleteKeyPair
      x-api-path-slug: actiondeletekeypair-get
      parameters:
      - in: query
        name: keyPairName
        description: The name of the key pair to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pairs
  /?Action=DetachStaticIp:
    get:
      summary: Detach Static Ip
      description: |-
        Detaches a static IP from the Amazon Lightsail instance to which it is
              attached.
      operationId: detachStaticIp
      x-api-path-slug: actiondetachstaticip-get
      parameters:
      - in: query
        name: staticIpName
        description: The name of the static IP to detach from the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Addresses
  /?Action=DownloadDefaultKeyPair:
    get:
      summary: Download Default Key Pair
      description: Downloads the default SSH key pair from the user's account.
      operationId: downloadDefaultKeyPair
      x-api-path-slug: actiondownloaddefaultkeypair-get
      parameters:
      - in: query
        name: privateKeyBase64
        description: A base64-encoded RSA private key
        type: string
      - in: query
        name: publicKeyBase64
        description: A base64-encoded public key of the ssh-rsa type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pairs
  /?Action=GetActiveNames:
    get:
      summary: Get Active Names
      description: Returns the names of all active (not deleted) resources.
      operationId: getActiveNames
      x-api-path-slug: actiongetactivenames-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for paginating results from your get active names
          request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Names
  /?Action=GetBlueprints:
    get:
      summary: Get Blueprints
      description: Returns the list of available instance images, or blueprints.
      operationId: getBlueprints
      x-api-path-slug: actiongetblueprints-get
      parameters:
      - in: query
        name: includeInactive
        description: A Boolean value indicating whether to include inactive results
          in your      request
        type: string
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get blueprints      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetBundles:
    get:
      summary: Get Bundles
      description: Returns the list of bundles that are available for purchase.
      operationId: getBundles
      x-api-path-slug: actiongetbundles-get
      parameters:
      - in: query
        name: includeInactive
        description: A Boolean value that indicates whether to include inactive bundle
          results in your      request
        type: string
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get bundles      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bundles
  /?Action=GetDomain:
    get:
      summary: Get Domain
      description: Returns information about a specific domain recordset.
      operationId: getDomain
      x-api-path-slug: actiongetdomain-get
      parameters:
      - in: query
        name: domainName
        description: The domain name for which your want to return information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=GetDomains:
    get:
      summary: Get Domains
      description: Returns a list of all domains in the user's account.
      operationId: getDomains
      x-api-path-slug: actiongetdomains-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get domains      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains
  /?Action=GetInstance:
    get:
      summary: Get Instance
      description: |-
        Returns information about a specific Amazon Lightsail instance, which is a virtual
              private server.
      operationId: getInstance
      x-api-path-slug: actiongetinstance-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstanceAccessDetails:
    get:
      summary: Get Instance Access Details
      description: |-
        Returns temporary SSH keys you can use to connect to a specific virtual private server,
              or instance.
      operationId: getInstanceAccessDetails
      x-api-path-slug: actiongetinstanceaccessdetails-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance to access
        type: string
      - in: query
        name: protocol
        description: The protocol to use to connect to your instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstanceMetricData:
    get:
      summary: Get Instance Metric Data
      description: |-
        Returns the data points for the specified Amazon Lightsail instance metric, given an
              instance name.
      operationId: getInstanceMetricData
      x-api-path-slug: actiongetinstancemetricdata-get
      parameters:
      - in: query
        name: endTime
        description: The end time of the time period
        type: string
      - in: query
        name: instanceName
        description: The name of the instance for which you want to get metrics data
        type: string
      - in: query
        name: metricName
        description: The metric name to get data about
        type: string
      - in: query
        name: period
        description: The time period for which you are requesting data
        type: string
      - in: query
        name: startTime
        description: The start time of the time period
        type: string
      - in: query
        name: statistics
        description: The instance statistics
        type: string
      - in: query
        name: unit
        description: The unit
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstancePortStates:
    get:
      summary: Get Instance Port States
      description: |-
        Returns the port states for a specific virtual private server, or
                instance.
      operationId: getInstancePortStates
      x-api-path-slug: actiongetinstanceportstates-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstances:
    get:
      summary: Get Instances
      description: |-
        Returns information about all Amazon Lightsail virtual private servers, or
                instances.
      operationId: getInstances
      x-api-path-slug: actiongetinstances-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get instances      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstanceSnapshot:
    get:
      summary: Get Instance Snapshot
      description: Returns information about a specific instance snapshot.
      operationId: getInstanceSnapshot
      x-api-path-slug: actiongetinstancesnapshot-get
      parameters:
      - in: query
        name: instanceSnapshotName
        description: The name of the snapshot for which you are requesting information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstanceSnapshots:
    get:
      summary: Get Instance Snapshots
      description: Returns all instance snapshots for the user's account.
      operationId: getInstanceSnapshots
      x-api-path-slug: actiongetinstancesnapshots-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get instance snapshots      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstanceState:
    get:
      summary: Get Instance State
      description: Returns the state of a specific instance.
      operationId: getInstanceState
      x-api-path-slug: actiongetinstancestate-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance to get state information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetKeyPair:
    get:
      summary: Get Key Pair
      description: Returns information about a specific key pair.
      operationId: getKeyPair
      x-api-path-slug: actiongetkeypair-get
      parameters:
      - in: query
        name: keyPairName
        description: The name of the key pair for which you are requesting information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pairs
  /?Action=GetKeyPairs:
    get:
      summary: Get Key Pairs
      description: Returns information about all key pairs in the user's account.
      operationId: getKeyPairs
      x-api-path-slug: actiongetkeypairs-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get key pairs      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pairs
  /?Action=GetOperation:
    get:
      summary: Get Operation
      description: Returns information about a specific operation.
      operationId: getOperation
      x-api-path-slug: actiongetoperation-get
      parameters:
      - in: query
        name: operationId
        description: A GUID used to identify the operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Operations
  /?Action=GetOperations:
    get:
      summary: Get Operations
      description: Returns information about all operations.
      operationId: getOperations
      x-api-path-slug: actiongetoperations-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get operations      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Operations
  /?Action=GetOperationsForResource:
    get:
      summary: Get Operations For Resource
      description: Gets operations for a specific resource (e.
      operationId: getOperationsForResource
      x-api-path-slug: actiongetoperationsforresource-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get operations for      resource request
        type: string
      - in: query
        name: resourceName
        description: The name of the resource for which you are requesting information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Operations
  /?Action=GetRegions:
    get:
      summary: Get Regions
      description: Returns a list of all valid regions for Amazon Lightsail.
      operationId: getRegions
      x-api-path-slug: actiongetregions-get
      parameters:
      - in: query
        name: includeAvailabilityZones
        description: A Boolean value indicating whether to also include Availability
          Zones in your get      regions request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Regions
  /?Action=GetStaticIp:
    get:
      summary: Get Static Ip
      description: Returns information about a specific static IP.
      operationId: getStaticIp
      x-api-path-slug: actiongetstaticip-get
      parameters:
      - in: query
        name: staticIpName
        description: The name of the static IP in Lightsail
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Addresses
  /?Action=GetStaticIps:
    get:
      summary: Get Static Ips
      description: Returns information about all static IPs in the user's account.
      operationId: getStaticIps
      x-api-path-slug: actiongetstaticips-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get static IPs      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Addresses
  /?Action=ImportKeyPair:
    get:
      summary: Import Key Pair
      description: Imports a public SSH key from a specific key pair.
      operationId: importKeyPair
      x-api-path-slug: actionimportkeypair-get
      parameters:
      - in: query
        name: keyPairName
        description: The name of the key pair for which you want to import the public
          key
        type: string
      - in: query
        name: publicKeyBase64
        description: A base64-encoded public key of the ssh-rsa type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Key Pairs
  /?Action=IsVpcPeered:
    get:
      summary: Is Vpc Peered
      description: Returns a Boolean value indicating whether your Lightsail VPC is
        peered.
      operationId: isVpcPeered
      x-api-path-slug: actionisvpcpeered-get
      parameters:
      - in: query
        name: isPeered
        description: Returns true if the Lightsail VPC is peered; otherwise,      false
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC
  /?Action=OpenInstancePublicPorts:
    get:
      summary: Open Instance Public Ports
      description: Adds public ports to an Amazon Lightsail instance.
      operationId: openInstancePublicPorts
      x-api-path-slug: actionopeninstancepublicports-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance for which you want to open the public
          ports
        type: string
      - in: query
        name: portInfo
        description: An array of key-value pairs containing information about the
          port mappings
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=PeerVpc:
    get:
      summary: Peer Vpc
      description: Tries to peer the Lightsail VPC with the user's default VPC.
      operationId: peerVpc
      x-api-path-slug: actionpeervpc-get
      parameters:
      - in: query
        name: operation
        description: An array of key-value pairs containing information about the
          request      operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC
  /?Action=RebootInstance:
    get:
      summary: Reboot Instance
      description: Restarts a specific instance.
      operationId: rebootInstance
      x-api-path-slug: actionrebootinstance-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance to reboot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=ReleaseStaticIp:
    get:
      summary: Release Static Ip
      description: Deletes a specific static IP from your account.
      operationId: releaseStaticIp
      x-api-path-slug: actionreleasestaticip-get
      parameters:
      - in: query
        name: staticIpName
        description: The name of the static IP to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Addresses
  /?Action=StartInstance:
    get:
      summary: Start Instance
      description: Starts a specific Amazon Lightsail instance from a stopped state.
      operationId: startInstance
      x-api-path-slug: actionstartinstance-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance (a virtual private server) to start
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=StopInstance:
    get:
      summary: Stop Instance
      description: Stops a specific Amazon Lightsail instance that is currently running.
      operationId: stopInstance
      x-api-path-slug: actionstopinstance-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance (a virtual private server) to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=UnpeerVpc:
    get:
      summary: Unpeer Vpc
      description: Attempts to unpeer the Lightsail VPC from the user's default VPC.
      operationId: unpeerVpc
      x-api-path-slug: actionunpeervpc-get
      parameters:
      - in: query
        name: operation
        description: An array of key-value pairs containing information about the
          request      operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC
  /?Action=UpdateDomainEntry:
    get:
      summary: Update Domain Entry
      description: Updates a domain recordset after it is created.
      operationId: updateDomainEntry
      x-api-path-slug: actionupdatedomainentry-get
      parameters:
      - in: query
        name: domainEntry
        description: An array of key-value pairs containing information about the
          domain entry
        type: string
      - in: query
        name: domainName
        description: The name of the domain recordset to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Domains