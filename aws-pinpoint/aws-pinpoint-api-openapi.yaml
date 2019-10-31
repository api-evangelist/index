swagger: "2.0"
x-collection-name: AWS Pinpoint
x-complete: 1
info:
  title: AWS Pinpoint API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apps/application-id/campaigns/campaign-id/activities:
    get:
      summary: Campaign Activities
      description: Returns information about the activity performed by a campaign,
        such as the time during which the campaign ran and the number of endpoints
        to which it delivered messages. You can use this resource to look up activity
        information by app ID and campaign ID.
      operationId: campaignActivities
      x-api-path-slug: appsapplicationidcampaignscampaignidactivities-get
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      - in: query
        name: page-size
        description: The number of entries you want on each page in the response
        type: string
        format: string
      - in: query
        name: token
        description: token
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign Activities
  /apps/application-id/campaigns/:
    get:
      summary: Get Campaigns
      description: Campaigns are messaging initiatives that engage specific segments
        of end users. The information represented by this resource includes the segment
        that the campaign reaches out to, the message that it delivers, and the schedule
        on which it runs. You can use this resource to look up, create, update, or
        delete campaigns.
      operationId: campaigns
      x-api-path-slug: appsapplicationidcampaigns-get
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      - in: query
        name: page-size
        description: The number of entries you want on each page in the response
        type: string
        format: string
      - in: query
        name: token
        description: An identifier used to retrieve the next page of results
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign
    put:
      summary: Add Campaign
      description: Use the POST method to create or update a campaign.
      operationId: addCampaign
      x-api-path-slug: appsapplicationidcampaigns-put
      parameters:
      - schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Campaign
  /apps/application-id/campaigns/campaign-id:
    get:
      summary: Campaign Instance
      description: Use the GET method to request information about a campaign.
      operationId: getCampaign
      x-api-path-slug: appsapplicationidcampaignscampaignid-get
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign
    put:
      summary: Update Campaign Instance
      description: Use the PUT method to update a campaign.
      operationId: updateCampaign
      x-api-path-slug: appsapplicationidcampaignscampaignid-put
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign
    delete:
      summary: Delete Campaign Instance
      description: Use the DELETE method to delete a campaign.
      operationId: deleteCampaign
      x-api-path-slug: appsapplicationidcampaignscampaignid-delete
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign
  /apps/application-id/campaigns/campaign-id/versions:
    get:
      summary: Campaign Versions List
      description: Use the GET method to request information about your campaign versions.
      operationId: getVersonsList
      x-api-path-slug: appsapplicationidcampaignscampaignidversions-get
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      - in: query
        name: page-size
        description: The number of entries you want on each page in the response
        type: string
        format: string
      - in: query
        name: token
        description: token
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign Versions
  /apps/application-id/campaigns/campaign-id/versions/version:
    get:
      summary: Campaign Version Instance
      description: Use the GET method to request information about a campaign version.
      operationId: campaignVersionInstance
      x-api-path-slug: appsapplicationidcampaignscampaignidversionsversion-get
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign Version
  /apps/application-id/endpoints:
    put:
      summary: Endpoints List
      description: Use the PUT method to update your endpoints.
      operationId: updateEndpointsList
      x-api-path-slug: appsapplicationidendpoints-put
      parameters:
      - in: query
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Endpoint
  /apps/application-id/endpoints/endpoint-id:
    get:
      summary: Endpoint Instance
      description: Use the GET method to request information about an endpoint.
      operationId: getEndpointInstance
      x-api-path-slug: appsapplicationidendpointsendpointid-get
      responses:
        200:
          description: OK
      tags:
      - Endpoint
    put:
      summary: Update Endpoint Instance
      description: Use the PUT method to update an endpoint.
      operationId: updateEndpointInstance
      x-api-path-slug: appsapplicationidendpointsendpointid-put
      responses:
        200:
          description: OK
      tags:
      - Endpoint
  /apps/application-id/jobs/import:
    get:
      summary: Import Job List
      description: Use the GET method to request information about your import jobs.
      operationId: importJobList
      x-api-path-slug: appsapplicationidjobsimport-get
      responses:
        200:
          description: OK
      tags:
      - Import Job
    post:
      summary: Update Import Job List
      description: Use the POST method to create or update an import job.
      operationId: updateImportJobList
      x-api-path-slug: appsapplicationidjobsimport-post
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Import Job
  /apps/application-id/segments/segment-id/jobs/import:
    get:
      summary: Import Job List by Segment
      description: Use the GET method to request information about the import jobs
        for a segment.
      operationId: importJobListbySegment
      x-api-path-slug: appsapplicationidsegmentssegmentidjobsimport-get
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Import Job
  /apps/application-id/jobs/import/{job-id}:
    get:
      summary: Import Job Instance
      description: Use the GET method to request information about an import job.
      operationId: importJobInstance
      x-api-path-slug: appsapplicationidjobsimportjobid-get
      parameters:
      - in: path
        name: job-id
        description: The job id
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Import Job
  /apps/application-id/segments:
    get:
      summary: Segments List
      description: Use the GET method to request information about your segments.
      operationId: segmentsList
      x-api-path-slug: appsapplicationidsegments-get
      responses:
        200:
          description: OK
      tags:
      - Segments
    post:
      summary: Segments List
      description: Use the POST method to create or update a segment.
      operationId: addSegmentsList
      x-api-path-slug: appsapplicationidsegments-post
      responses:
        200:
          description: OK
      tags:
      - Segments
  /apps/application-id/segments/segment-id:
    get:
      summary: Segment Instance
      description: Use the GET method to request information about a segment.
      operationId: getSegmentInstance
      x-api-path-slug: appsapplicationidsegmentssegmentid-get
      responses:
        200:
          description: OK
      tags:
      - Segments
    put:
      summary: Segment Instance
      description: Use the PUT method to update a segment.
      operationId: updateSegmentInstance
      x-api-path-slug: appsapplicationidsegmentssegmentid-put
      responses:
        200:
          description: OK
      tags:
      - Segments
    delete:
      summary: Segment Instance
      description: Use the DELETE method to delete a segment.
      operationId: deleteSegmentInstance
      x-api-path-slug: appsapplicationidsegmentssegmentid-delete
      responses:
        200:
          description: OK
      tags:
      - Segments
  /apps/application-id/segment/versions:
    get:
      summary: Segment Versions List
      description: Use the GET method to request information about your segment versions.
      operationId: getSegmentVersionsList
      x-api-path-slug: appsapplicationidsegmentversions-get
      responses:
        200:
          description: OK
      tags:
      - Segments
  /apps/application-id/segments/segment-id/versions/version:
    get:
      summary: Segment Version Instance
      description: Use the GET method to request information about a segment version.
      operationId: getSegmentVersionInstance
      x-api-path-slug: appsapplicationidsegmentssegmentidversionsversion-get
      responses:
        200:
          description: OK
      tags:
      - Segments
  /apps/application-id/settings:
    get:
      summary: Get URI
      description: Use the GET method to request the settings for an app.
      operationId: getURI
      x-api-path-slug: appsapplicationidsettings-get
      responses:
        200:
          description: OK
      tags:
      - URI
    put:
      summary: Update URI
      description: Use the PUT method to update the settings for an app.
      operationId: updateURI
      x-api-path-slug: appsapplicationidsettings-put
      responses:
        200:
          description: OK
      tags:
      - URI