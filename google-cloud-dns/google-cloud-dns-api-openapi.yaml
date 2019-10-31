swagger: "2.0"
x-collection-name: Google Cloud DNS
x-complete: 1
info:
  title: Google Cloud DNS
  description: configures-and-serves-authoritative-dns-records-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /dns/v1/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}:
    get:
      summary: Get Project
      description: Fetch the representation of an existing Project.
      operationId: dns.projects.get
      x-api-path-slug: project-get
      parameters:
      - in: path
        name: project
        description: Identifies the project addressed by this request
      responses:
        200:
          description: OK
      tags:
      - Project
  /{project}/managedZones:
    get:
      summary: Get Managed Zones
      description: Enumerate ManagedZones that have been created but not yet deleted.
      operationId: dns.managedZones.list
      x-api-path-slug: projectmanagedzones-get
      parameters:
      - in: query
        name: dnsName
        description: Restricts the list to return only zones with this domain name
      - in: query
        name: maxResults
        description: Optional
      - in: query
        name: pageToken
        description: Optional
      - in: path
        name: project
        description: Identifies the project addressed by this request
      responses:
        200:
          description: OK
      tags:
      - Managed Zone
    post:
      summary: Create Managed Zone
      description: Create a new ManagedZone.
      operationId: dns.managedZones.create
      x-api-path-slug: projectmanagedzones-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Identifies the project addressed by this request
      responses:
        200:
          description: OK
      tags:
      - Managed Zone
  /{project}/managedZones/{managedZone}:
    delete:
      summary: Delete Managed Zone
      description: Delete a previously created ManagedZone.
      operationId: dns.managedZones.delete
      x-api-path-slug: projectmanagedzonesmanagedzone-delete
      parameters:
      - in: path
        name: managedZone
        description: Identifies the managed zone addressed by this request
      - in: path
        name: project
        description: Identifies the project addressed by this request
      responses:
        200:
          description: OK
      tags:
      - Managed Zone
    get:
      summary: Get Managed Zone
      description: Fetch the representation of an existing ManagedZone.
      operationId: dns.managedZones.get
      x-api-path-slug: projectmanagedzonesmanagedzone-get
      parameters:
      - in: path
        name: managedZone
        description: Identifies the managed zone addressed by this request
      - in: path
        name: project
        description: Identifies the project addressed by this request
      responses:
        200:
          description: OK
      tags:
      - Managed Zone
  /{project}/managedZones/{managedZone}/changes:
    get:
      summary: List Managed Zone Changes
      description: Enumerate Changes to a ResourceRecordSet collection.
      operationId: dns.changes.list
      x-api-path-slug: projectmanagedzonesmanagedzonechanges-get
      parameters:
      - in: path
        name: managedZone
        description: Identifies the managed zone addressed by this request
      - in: query
        name: maxResults
        description: Optional
      - in: query
        name: pageToken
        description: Optional
      - in: path
        name: project
        description: Identifies the project addressed by this request
      - in: query
        name: sortBy
        description: Sorting criterion
      - in: query
        name: sortOrder
        description: 'Sorting order direction: ascending or descending'
      responses:
        200:
          description: OK
      tags:
      - Managed Zone
    post:
      summary: Create Managed Zone Change
      description: Atomically update the ResourceRecordSet collection.
      operationId: dns.changes.create
      x-api-path-slug: projectmanagedzonesmanagedzonechanges-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: managedZone
        description: Identifies the managed zone addressed by this request
      - in: path
        name: project
        description: Identifies the project addressed by this request
      responses:
        200:
          description: OK
      tags:
      - Managed Zone
  /{project}/managedZones/{managedZone}/changes/{changeId}:
    get:
      summary: Get Managed Zone Change
      description: Fetch the representation of an existing Change.
      operationId: dns.changes.get
      x-api-path-slug: projectmanagedzonesmanagedzonechangeschangeid-get
      parameters:
      - in: path
        name: changeId
        description: The identifier of the requested change, from a previous ResourceRecordSetsChangeResponse
      - in: path
        name: managedZone
        description: Identifies the managed zone addressed by this request
      - in: path
        name: project
        description: Identifies the project addressed by this request
      responses:
        200:
          description: OK
      tags:
      - Managed Zone
  /{project}/managedZones/{managedZone}/rrsets:
    get:
      summary: Get Managed Zone Resources
      description: Enumerate ResourceRecordSets that have been created but not yet
        deleted.
      operationId: dns.resourceRecordSets.list
      x-api-path-slug: projectmanagedzonesmanagedzonerrsets-get
      parameters:
      - in: path
        name: managedZone
        description: Identifies the managed zone addressed by this request
      - in: query
        name: maxResults
        description: Optional
      - in: query
        name: name
        description: Restricts the list to return only records with this fully qualified
          domain name
      - in: query
        name: pageToken
        description: Optional
      - in: path
        name: project
        description: Identifies the project addressed by this request
      - in: query
        name: type
        description: Restricts the list to return only records of this type
      responses:
        200:
          description: OK
      tags:
      - Managed Zone