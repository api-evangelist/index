swagger: "2.0"
x-collection-name: Google Manufacturer Center
x-complete: 1
info:
  title: Manufacturer Center
  description: public-api-for-managing-manufacturer-center-related-data-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: manufacturers.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{parent}/products:
    get:
      summary: Get Products
      description: Lists all the products in a Manufacturer Center account.
      operationId: manufacturers.accounts.products.list
      x-api-path-slug: v1parentproducts-get
      parameters:
      - in: query
        name: pageSize
        description: Maximum number of product statuses to return in the response,
          used forpaging
      - in: query
        name: pageToken
        description: The token returned by the previous request
      - in: path
        name: parent
        description: Parent ID in the format `accounts/{account_id}`
      responses:
        200:
          description: OK
      tags:
      - Product
  /v1/{parent}/products/{name}:
    get:
      summary: Get Product
      description: |-
        Gets the product from a Manufacturer Center account, including product
        issues.
      operationId: manufacturers.accounts.products.get
      x-api-path-slug: v1parentproductsname-get
      parameters:
      - in: path
        name: name
        description: Name in the format `{target_country}:{content_language}:{product_id}`
      - in: path
        name: parent
        description: Parent ID in the format `accounts/{account_id}`
      responses:
        200:
          description: OK
      tags:
      - Product