swagger: "2.0"
x-collection-name: System Award Management
x-complete: 1
info:
  title: System Award Management API
  description: sam-gov-is-the-system-for-award-management--it-is-the-site-on-which-all-vendors-grantees-receivers-of-federal-financial-assistance-and-other-entities-doing-business-with-the-government-must-register-prior-to-receiving-an-award---the-registrations-api-currently-provides-the-publicly-available-data-for-a-specific-entity-along-with-status-and-progress-information-for-that-registration-
  version: 1.0.0
host: api.data.gov
basePath: /sam/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /registrations/{registrationId}:
    get:
      summary: Find a registration by its DUN+4 number
      description: If the entity only has a 9-digit DUNS number, pad the end to include
        4 zeros
      operationId: getData
      x-api-path-slug: registrationsregistrationid-get
      parameters:
      - in: query
        name: api_key
        description: An API Key from api
        type: string
      - in: path
        name: registrationId
        description: DUNS+4 number (no - sign) of the registration to be fetched
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""