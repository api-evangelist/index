swagger: "2.0"
x-collection-name: OrgHunter
x-complete: 1
info:
  title: Org Hunter
  description: get-the-latest-irs-data-and-most-up-to-date-charity-information-for-your-website-or-application
  version: 1.0.0
host: data.orghunter.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/categories:
    post:
      summary: Get categories!
      description: This operation provides a list of categories.
      operationId: postV1Categories
      x-api-path-slug: v1categories-post
      responses:
        200:
          description: OK
      tags:
      - Charity
  /v1/charitybasic:
    post:
      summary: Get details!
      description: This operation detail data.
      operationId: postV1Charitybasic
      x-api-path-slug: v1charitybasic-post
      parameters:
      - in: query
        name: ein
        description: ein (Employer Identification Number)
      responses:
        200:
          description: OK
      tags:
      - Charity
  /v1/charityfinancial:
    post:
      summary: Get details!
      description: This operation detail data.
      operationId: postV1Charityfinancial
      x-api-path-slug: v1charityfinancial-post
      parameters:
      - in: query
        name: ein
        description: ein (Employer Identification Number)
      responses:
        200:
          description: OK
      tags:
      - Charity
      - Financial
  /v1/charitygeolocation:
    post:
      summary: Get details!
      description: This operation detail data.
      operationId: postV1Charitygeolocation
      x-api-path-slug: v1charitygeolocation-post
      parameters:
      - in: query
        name: ein
        description: ein (Employer Identification Number)
      responses:
        200:
          description: OK
      tags:
      - Charity
      - Geo
      - Location
  /v1/charitypremium:
    post:
      summary: Get details!
      description: This operation detail data.
      operationId: postV1Charitypremium
      x-api-path-slug: v1charitypremium-post
      parameters:
      - in: query
        name: ein
        description: ein (Employer Identification Number)
      responses:
        200:
          description: OK
      tags:
      - Charity
      - Premium
  /v1/charitysearch:
    post:
      summary: Get summary data!
      description: This operation provides summary data.
      operationId: postV1Charitysearch
      x-api-path-slug: v1charitysearch-post
      parameters:
      - in: query
        name: category
        description: Category Value Selected from Categories API
      - in: query
        name: city
        description: City Name
      - in: query
        name: ein
        description: Employer Identification Number (EIN)
      - in: query
        name: eligible
        description: eligible=1 will return only organizations that are tax deductible
          and in good standing with the IRS
      - in: query
        name: rows
        description: Records Per Page
      - in: query
        name: searchTerm
        description: Charity Name or Keyword
      - in: query
        name: start
        description: Record Set Start Position
      - in: query
        name: state
        description: State Name - Two letter state abbreviation
      - in: query
        name: zipCode
        description: Zipcode Value - 5 digit zipcode value
      responses:
        200:
          description: OK
      tags:
      - Charity
      - Search