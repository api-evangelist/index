swagger: "2.0"
x-collection-name: Zendesk
x-complete: 1
info:
  title: Swagger API
  version: 1.0.0
host: '{host}.zendesk.com'
basePath: /api/v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tickets.json:
    post:
      summary: createTicket
      description: Create Ticket
      operationId: TicketsJsonPost
      x-api-path-slug: tickets-json-post
      parameters:
      - in: body
        name: ticket
        description: Ticket
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Support
      - Tickets