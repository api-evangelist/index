swagger: "2.0"
x-collection-name: Nexmo
x-complete: 1
info:
  title: Nexmo SMS API
  description: nexmo-makes-it-simple-to-send-and-receive-a-high-volume-of-sms-anywhere-in-the-world-within-minutes-
  termsOfService: https://www.nexmo.com/terms
  version: v1
host: rest.nexmo.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  sms/{format}:
    get:
      summary: Send Message
      description: Nexmo makes it simple to send and receive a high volume of SMS
        anywhere in the world within minutes.
      operationId: sendMessage
      x-api-path-slug: smsformat-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: api_secret
        description: Your API Secret
      - in: query
        name: client-ref
        description: Include any reference string for your reference
      - in: path
        name: format
        description: XML or JSON
      - in: query
        name: from
        description: 'Sender address may be alphanumeric (Ex: from=MyCompany20)'
      - in: query
        name: message-class
        description: Set to 0 for Flash SMS
      - in: query
        name: network-code
        description: Force the recipient network operator MCCMNC, make sure to supply
          the correct information otherwise the message wont be delivered
      - in: query
        name: status-report-req
        description: Set to 1 if you want to receive a delivery report (DLR) for this
          request
      - in: query
        name: text
        description: Body of the text message (with a maximum length of 3200 characters),
          UTF-8 and URL encoded value
      - in: query
        name: to
        description: Mobile number in international format, and one recipient per
          request
      - in: query
        name: ttl
        description: Message life span in milliseconds
      - in: query
        name: type_of_media
        description: This can be omitted for text (default), but is required when
          sending a Binary (binary), WAP Push (wappush), Unicode message (unicode),
          vcal (vcal) or vcard (vcard)
      - in: query
        name: vcard
        description: vcard text body correctly formatted
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - SMS