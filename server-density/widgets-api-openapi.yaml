swagger: "2.0"
x-collection-name: Server Density
x-complete: 1
info:
  title: Widgets API
  description: the-widgets-api-
  version: 1.0.0
host: api.serverdensity.io.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/widgets/widgetId:
    "":
      summary: Deleting a widget
      description: Deleting a widget.
      operationId: deleting-a-widget
      x-api-path-slug: userswidgetswidgetid-
      parameters:
      - in: path
        name: token
        description: Your API token
        type: string
      - in: body
        name: token
        description: Your API token
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: widgetId
        description: The ID of the widget to delete
        type: string
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
      - Widgets
  /users/widgets/duplicate/widgetId:
    "":
      summary: Duplicating a widget
      description: Duplicating a widget.
      operationId: duplicating-a-widget
      x-api-path-slug: userswidgetsduplicatewidgetid-
      parameters:
      - in: path
        name: token
        description: Your API token
        type: string
      - in: body
        name: token
        description: Your API token
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: widgetId
        description: ID of the widget to duplicate
        type: string
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
      - Widgets