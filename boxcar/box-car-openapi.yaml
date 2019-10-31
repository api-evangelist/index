swagger: "2.0"
x-collection-name: Boxcar
x-complete: 1
info:
  title: Box Car
  description: add-boxcar-services-to-your-app-so-users-can-get-messages-and-update-all-their-favorite-social-services-
  version: 1.0.0
host: boxcar.io
basePath: /devices/providers/%7Bprovider_key%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /notifications/subscribe:
    post:
      summary: Subscribe to Provider
      description: This sends the user with the matching e-mail address a push notification
        which requests that they add your service. This will ease integration with
        your website, as you will have already registered them on your system and
        can identify whom they are based on their Boxcar e-mail address. Please note,
        this API call is an exception and will return an HTTP status code of 404 if
        we are unable to find the registered user by e-mail in our system. If the
        email address is not found in our system, we'll send an email to it letting
        the user know where they can download Boxcar. If the user has already added
        your service, we'll return an HTTP status code of 401.
      operationId: Create_subscribeToProvider_
      x-api-path-slug: notificationssubscribe-post
      parameters:
      - in: query
        name: email
        description: The users e-mail address
      - in: query
        name: provider_key
        description: The API key
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Subscriptions