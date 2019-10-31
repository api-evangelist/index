swagger: "2.0"
x-collection-name: USA.Gov Corporate Consumer Contact Information
x-complete: 1
info:
  title: USA.Gov Corporate Consumer Contact Information API
  description: we-make-the-corporate-consumer-contact-listing-found-in-the-consumer-action-handbook-pdf-available-via-a-rest-api--the-api-programmatically-returns-all-of-the-information-contained-in-the-directory-or-you-can-query-the-api-to-return-just-a-subset-of-the-available-information-
  termsOfService: https://github.com/usagov/Corporate-Consumer-Contact-API-Documentation#terms-of-service
  contact:
    name: USA.Gov Developers
    email: usagov-developers@gsa.gov
  version: 1.0.0
host: www.usa.gov
basePath: api/USAGovAPI/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /contacts.{format}/contacts:
    get:
      summary: Get Contacts
      description: Contacts is a general purpose call that, by default, will return
        all of the corporate directory records. However, you can pass parameters into
        the contacts call that allow you to filter the records returned by the API
        in powerful ways.
      operationId: getContacts
      x-api-path-slug: contacts-formatcontacts-get
      parameters:
      - in: query
        name: query_filter
        description: Return only corporate directory records that meet the criteria
          you enter into this parameter
        type: string
        format: string
      - in: query
        name: result_filter
        description: Return only the fields listed here (separated by |) as opposed
          to every field in each directory record
        type: string
        format: string
      - in: query
        name: sort
        description: Allows you to specify the sort order of the returned agency directory
          records
        type: string
        format: string
      - in: header
        name: X-Range
        description: You can limit the results returned by the API by including an
          X-Range HTTP header in your GET request, with a value of items=x to y, where
          x is the lower limit and y is the upper limit of the results to be returned
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Contacts
  /contacts.{format}/contacts/{id}:
    get:
      summary: Get Contact
      description: The Contact call will let you access an individual corporation's
        information by including its unique identifier in the call.
      operationId: getContact
      x-api-path-slug: contacts-formatcontactsid-get
      responses:
        200:
          description: OK
      tags:
      - Contacts