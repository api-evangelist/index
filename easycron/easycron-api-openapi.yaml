swagger: "2.0"
x-collection-name: EasyCron
x-complete: 1
info:
  title: Easycron API
  description: all-registered-users-of-easycron-can-utilize-our-api-to-manage-their-cron-jobs-without-logging-in-easycron-com-
  termsOfService: https://www.easycron.com/terms
  contact:
    name: EasyCron
    url: https://www.easycron.com/contact
  version: 1.0.0
host: www.easycron.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /add:
    get:
      summary: Add a cron job.
      description: Add a cron job.
      operationId: addCronJob
      x-api-path-slug: add-get
      parameters:
      - in: query
        name: cookies
        description: Cookie variable-value pairs
      - in: query
        name: cron_expression
        description: Cron expression that following the syntax defined at our Cron
          Expression page
      - in: query
        name: cron_job_name
        description: The name of your cron job
      - in: query
        name: email_me
        description: Email notification setting of the cron job
      - in: query
        name: log_output_length
        description: Length of execution log of the cron job
      - in: query
        name: posts
        description: POST variable-value pairs
      - in: query
        name: testfirst
        description: If to test the cron job URL first before adding
      - in: query
        name: token
        description: You API token
      - in: query
        name: url
        description: URL of the cron job
      responses:
        200:
          description: OK
      tags:
      - Cron
      - Job
  /delete:
    get:
      summary: Delete a cron job.
      description: Delete a cron job.
      operationId: deleteCronJob
      x-api-path-slug: delete-get
      parameters:
      - in: query
        name: id
        description: ID of the cron job you want to delete
      - in: query
        name: token
        description: You API token
      responses:
        200:
          description: OK
      tags:
      - Cron
      - Job
  /detail:
    get:
      summary: Get detail of a cron job.
      description: Get detail of a cron job.
      operationId: getDetailCronJob
      x-api-path-slug: detail-get
      parameters:
      - in: query
        name: id
        description: ID of the cron job you want to get detail of
      - in: query
        name: token
        description: You API token
      responses:
        200:
          description: OK
      tags:
      - Detail
      - Of
      - Cron
      - Job
  /disable:
    get:
      summary: Disable a cron job
      description: Disable a cron job
      operationId: disableCronJbo
      x-api-path-slug: disable-get
      parameters:
      - in: query
        name: id
        description: ID of the cron job you want to disable
      - in: query
        name: token
        description: You API token
      responses:
        200:
          description: OK
      tags:
      - Disable
      - Cron
      - Job
  /edit:
    get:
      summary: Edit a cron job.
      description: Edit a cron job.
      operationId: editCronJob
      x-api-path-slug: edit-get
      parameters:
      - in: query
        name: cookies
        description: Cookie variable-value pairs
      - in: query
        name: cron_expression
        description: Cron expression that following the syntax defined at our Cron
          Expression page
      - in: query
        name: cron_job_name
        description: The name of your cron job
      - in: query
        name: email_me
        description: Email notification setting of the cron job
      - in: query
        name: id
        description: ID of the cron job you want to edit
      - in: query
        name: log_output_length
        description: Length of execution log of the cron job
      - in: query
        name: posts
        description: POST variable-value pairs
      - in: query
        name: testfirst
        description: If to test the cron job URL first before updating
      - in: query
        name: token
        description: You API token
      - in: query
        name: url
        description: URL of the cron job
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Cron
      - Job
  /enable:
    get:
      summary: Enable a cron job.
      description: Enable a cron job.
      operationId: enableCronJob
      x-api-path-slug: enable-get
      parameters:
      - in: query
        name: id
        description: ID of the cron job you want to enable
      - in: query
        name: token
        description: You API token
      responses:
        200:
          description: OK
      tags:
      - Enable
      - Cron
      - Job
  /logs:
    get:
      summary: View the latest 10 execution logs of a cron job.
      description: View the latest 10 execution logs of a cron job.
      operationId: viewLast10Logs
      x-api-path-slug: logs-get
      parameters:
      - in: query
        name: id
        description: ID of the cron job you want to delete
      - in: query
        name: token
        description: You API token
      responses:
        200:
          description: OK
      tags:
      - View
      - Latest
      - "10"
      - Execution
      - Logs
      - Of
      - Cron
      - Job
  /timezone:
    get:
      summary: Get the timezone of a user account.
      description: Get the timezone of a user account.
      operationId: getTimzone
      x-api-path-slug: timezone-get
      parameters:
      - in: query
        name: token
        description: You API token
      responses:
        200:
          description: OK
      tags:
      - Timezone
      - Of
      - User
      - Account