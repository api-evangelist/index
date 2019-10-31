swagger: "2.0"
x-collection-name: Halifax Bank
x-complete: 1
info:
  title: Halifax Bank
  description: this-is-an-openapi-definition-for-the-standard-set-of-open-banking-httpopenbankingapis-io-apis-for-halifax-bank-
  termsOfService: https://www.openbanking.org.uk/open-licence/
  contact:
    name: API Evangelist
    url: https://apievangelist.com
    email: info@apievangelist.com
  version: 1.0.0
host: api.halifax.co.uk
basePath: open-banking/v2.1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  atms/:
    get:
      summary: Get ATMs
      description: This endpoint can contain multiple brands owned by a particular
        banking group. Each brand can provide multiple ATMs.
      operationId: getATMS
      x-api-path-slug: atms-get
      responses:
        200:
          description: OK
      tags:
      - Atms
  branches/:
    get:
      summary: Get Branches
      description: This endpoint can contain multiple brands owned by a particular
        banking group. Each brand can own multiple branches.
      operationId: getBranches
      x-api-path-slug: branches-get
      responses:
        200:
          description: OK
      tags:
      - Branches
  personal-current-accounts/:
    get:
      summary: Get Current Personal Accounts
      description: This endpoint can contain multiple brands owned by a particular
        banking group. Each brand can own multiple PCA products.
      operationId: getCurrentPersonalAccounts
      x-api-path-slug: personalcurrentaccounts-get
      responses:
        200:
          description: OK
      tags:
      - Personal
      - Current
      - Accounts