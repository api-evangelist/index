swagger: "2.0"
x-collection-name: Zencoder
x-complete: 1
info:
  title: Zencoder
  version: v2
host: app.zencoder.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account:
    get:
      summary: Get Account Details
      description: Get Account Details
      operationId: getAccount
      x-api-path-slug: account-get
      parameters:
      - in: query
        name: api_key
        description: The API key
      responses:
        200:
          description: OK
      tags:
      - Account
    post:
      summary: Create an Account
      description: Create an Account
      operationId: postAccount
      x-api-path-slug: account-post
      parameters:
      - in: query
        name: email
      - in: query
        name: password
      - in: query
        name: password_confirmation
      - in: query
        name: terms_of_service
      responses:
        200:
          description: OK
      tags:
      - Account
  /account/integration:
    put:
      summary: Integration Mode
      description: Integration Mode
      operationId: putAccountIntegration
      x-api-path-slug: accountintegration-put
      parameters:
      - in: query
        name: api_key
        description: The API key
      responses:
        200:
          description: OK
      tags:
      - Account
      - Integration
  /account/live:
    put:
      summary: Integration Mode - Live
      description: Integration Mode - Live
      operationId: putAccountLive
      x-api-path-slug: accountlive-put
      responses:
        200:
          description: OK
      tags:
      - Account
      - Live
  /inputs/{input_id}:
    get:
      summary: Get Input Details
      description: Get Input Details
      operationId: getInupdatesInupdate
      x-api-path-slug: inputsinput-id-get
      parameters:
      - in: query
        name: api_key
        description: The API key
      - in: query
        name: callback
        description: JSONP Callback
      - in: query
        name: input_id
        description: The input id
      responses:
        200:
          description: OK
      tags:
      - Inputs
      - Input
      - Id
  /inputs/{input_id}/progress:
    get:
      summary: Input Progress
      description: 'The return will contain one or more of the following keys: state,
        current_event, current_event_progress and progress.'
      operationId: getInupdatesInupdateProgress
      x-api-path-slug: inputsinput-idprogress-get
      responses:
        200:
          description: OK
      tags:
      - Inputs
      - Input
      - Id
      - Progress
  /jobs:
    get:
      summary: List Jobs
      description: A list of jobs can be obtained by sending an HTTP GET request.
      operationId: getJobs
      x-api-path-slug: jobs-get
      parameters:
      - in: query
        name: api_key
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Jobs
    post:
      summary: Create a Job
      description: Encoding jobs are created by sending an HTTP POST request.
      operationId: postJobs
      x-api-path-slug: jobs-post
      parameters:
      - in: query
        name: api_key
        description: The API key
      - in: query
        name: Encoding Settings
        description: '(see: https://app'
      - in: query
        name: input
        description: A valid URL to a media file (HTTP/HTTPS, FTP/FTPS, SFTP, GCS,
          CF or S3), with or without authentication
      responses:
        200:
          description: OK
      tags:
      - Jobs
  /jobs/{job_id}:
    get:
      summary: Get Job Details
      description: Get Job Details
      operationId: getJobsJob
      x-api-path-slug: jobsjob-id-get
      parameters:
      - in: query
        name: api_key
        description: The API Key
      - in: query
        name: Get Job Details
        description: The Job id
      responses:
        200:
          description: OK
      tags:
      - Jobs
      - Job
      - Id
  /jobs/{job_id}/cancel:
    put:
      summary: Cancel a Job
      description: If you wish to cancel a job that has not yet finished processing
        you may send a request.
      operationId: putJobsJobCancel
      x-api-path-slug: jobsjob-idcancel-put
      parameters:
      - in: query
        name: api_key
        description: The API Key
      - in: query
        name: job_id
        description: The job id
      responses:
        200:
          description: OK
      tags:
      - Jobs
      - Job
      - Id
      - Cancel
  /jobs/{job_id}/finish:
    put:
      summary: Finish a LIve Job
      description: Finishes the input on a Live streaming job.
      operationId: putJobsJobFinish
      x-api-path-slug: jobsjob-idfinish-put
      responses:
        200:
          description: OK
      tags:
      - Jobs
      - Job
      - Id
      - Finish
  /jobs/{job_id}/progress:
    get:
      summary: Job Progress
      description: 'The return will contain one or more of the following keys: state,
        input, outputs, and progress.'
      operationId: getJobsJobProgress
      x-api-path-slug: jobsjob-idprogress-get
      responses:
        200:
          description: OK
      tags:
      - Jobs
      - Job
      - Id
      - Progress
  /jobs/{job_id}/resubmit:
    put:
      summary: Resubmit a Job
      description: If a job has failed processing you may request that it be attempted
        again.
      operationId: putJobsJobResubmit
      x-api-path-slug: jobsjob-idresubmit-put
      parameters:
      - in: query
        name: api_key
        description: The API Key
      - in: query
        name: job_id
        description: The job id
      responses:
        200:
          description: OK
      tags:
      - Jobs
      - Job
      - Id
      - Resubmit
  /outputs/{output_id}/progress:
    get:
      summary: Output Progress
      description: 'The return will contain one or more of the following keys: state,
        current_event, current_event_progress and progress.'
      operationId: getOutupdatesOutupdateProgress
      x-api-path-slug: outputsoutput-idprogress-get
      parameters:
      - in: query
        name: api_key
        description: The API key
      - in: query
        name: callback
        description: JSONP Callback
      - in: query
        name: output_id
        description: The output id
      responses:
        200:
          description: OK
      tags:
      - Outputs
      - Output
      - Id
      - Progress
  /reports/all:
    get:
      summary: Get Usage for VOD & Live
      description: Get Usage for VOD & Live
      operationId: getReportsAll
      x-api-path-slug: reportsall-get
      parameters:
      - in: query
        name: api_key
        description: The API key
      - in: query
        name: from
        description: 'Start date in the format YYYY-MM-DD (default: 30 days ago)'
      - in: query
        name: grouping
        description: 'Hour usage for only one report grouping (default: none)'
      - in: query
        name: to
        description: 'End date in the format YYYY-MM-DD (default: yesterday)'
      responses:
        200:
          description: OK
      tags:
      - Reports
  /reports/live:
    get:
      summary: Get Usage for Live
      description: Get Usage for Live
      operationId: getReportsLive
      x-api-path-slug: reportslive-get
      parameters:
      - in: query
        name: api_key
        description: The API key
      - in: query
        name: from
        description: 'Start date in the format YYYY-MM-DD (default: 30 days ago)'
      - in: query
        name: grouping
        description: 'Hour usage for only one report grouping (default: none)'
      - in: query
        name: to
        description: 'End date in the format YYYY-MM-DD (default: yesterday)'
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Live
  /reports/minutes:
    get:
      summary: Get Minutes Used
      description: Get Minutes Used
      operationId: getReportsMinutes
      x-api-path-slug: reportsminutes-get
      parameters:
      - in: query
        name: api_key
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Minutes
  /reports/vod:
    get:
      summary: Get Usage for VOD
      description: Get Usage for VOD
      operationId: getReportsVod
      x-api-path-slug: reportsvod-get
      parameters:
      - in: query
        name: api_key
        description: The API key
      - in: query
        name: from
        description: 'Start date in the format YYYY-MM-DD (default: 30 days ago)'
      - in: query
        name: grouping
        description: 'Minute usage for only one report grouping (default: none)'
      - in: query
        name: to
        description: 'End date in the format YYYY-MM-DD (default: yesterday)'
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Vod
  /v2/outputs/{output_id}:
    get:
      summary: Get Output Details
      description: Get Output Details
      operationId: getV2OutupdatesOutupdate
      x-api-path-slug: v2outputsoutput-id-get
      parameters:
      - in: query
        name: api_key
        description: The API key
      - in: query
        name: output_id
        description: The output id
      responses:
        200:
          description: OK
      tags:
      - V2
      - Outputs
      - Output
      - Id