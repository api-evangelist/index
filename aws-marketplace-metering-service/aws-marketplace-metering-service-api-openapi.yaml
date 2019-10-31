swagger: "2.0"
x-collection-name: AWS Marketplace Metering Service
x-complete: 1
info:
  title: AWS Marketplace Metering Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=MeterUsage:
    get:
      summary: Meter Usage
      description: API to emit metering records.
      operationId: MeterUsage
      x-api-path-slug: actionmeterusage-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the permissions required for the action,
          but does not make the request
        type: string
      - in: query
        name: ProductCode
        description: Product code is used to uniquely identify a product in AWS Marketplace
        type: string
      - in: query
        name: Timestamp
        description: Timestamp of the hour, recorded in UTC
        type: string
      - in: query
        name: UsageDimension
        description: It will be one of the fcp dimension name provided during the
          publishing of the product
        type: string
      - in: query
        name: UsageQuantity
        description: Consumption value for the hour
        type: string
      responses:
        200:
          description: OK
      tags:
      - Meter Usage