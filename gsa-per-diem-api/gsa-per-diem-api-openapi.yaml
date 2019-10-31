swagger: "2.0"
x-collection-name: GSA Per Diem API
x-complete: 1
info:
  title: GSA Per Diem API
  description: per-diem-rates-are-the-allowed-reimbursement-rates-for-hotel-stays-and-meals-for-federal-travelers--rates-are-set-for-each-of-the-federal-governments-fiscal-years-fy-2014-is-october-1-2013-to-september-30-2014--gsa-is-responsible-for-setting-the-rates-in-the-continental-united-states---many-businesses-and-other-organizations-adopt-these-rates-as-well--gsa-is-making-the-rates-available-using-the-ckans-action-api-via-data-gov-to-allow-software-developers-programmatic-access-the-data-and-create-innovative-uses-for-it-
  version: 1.0.0
host: inventory.data.gov
basePath: /api/action/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /datastore_search?resource_id=8ea44bc4-22ba-4386-b84c-1494ab28964b:
    get:
      summary: Per Diem Rates
      description: GSA sets rates for geographic areas it determines called primary
        destinations. Areas outside the primary destinations are covered by the same,
        nation-wide standard rate.
      operationId: getPerDiemRates
      x-api-path-slug: datastore-searchresource-id8ea44bc422ba4386b84c1494ab28964b-get
      parameters:
      - in: query
        name: filters
        description: FiscalYear, Zip, State, DestinationID, City, County, Month, Meals
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Per Diem Rates