swagger: "2.0"
x-collection-name: International Trade Administration
x-complete: 1
info:
  title: ITA Offices And Centers
  description: this-api-provides-contact-and-address-information-for-all-of-itau2019s-domestic-and-international-export-assistance-centers--incorporating-these-listings-into-directories-of-business-counseling-services-is-one-example-of-how-developers-can-use-this-api-to-assist-exporters-
  termsOfService: http://developer.trade.gov/tos.html
  version: "1.0"
host: api.trade.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ita_office_locations/search:
    get:
      summary: ITA Offices and Centers Search
      description: This API provides contact and address information for all of ITAs
        domestic and international export assistance centers.
      operationId: office
      x-api-path-slug: ita-office-locationssearch-get
      parameters:
      - in: query
        name: city
        description: Returns office locations based on city name
      - in: query
        name: countries
        description: Returns office locations based on ISO alpha-2 country codes
      - in: query
        name: keyword
        description: Returns office locations for a match within the post or office
          name fields
      - in: query
        name: offset
        description: The offset parameter defines the offset from the first result
          you want to fetch
      - in: query
        name: size
        description: The size parameter allows you to configure the maximum amount
          of hits to be returned
      - in: query
        name: state
        description: Returns locations for export assistance centers located in a
          specific U
      responses:
        200:
          description: OK
      tags:
      - Offices