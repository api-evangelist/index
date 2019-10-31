swagger: "2.0"
x-collection-name: Uber
x-complete: 1
info:
  title: Uber
  description: using-the-uber-api-developers-can-integrate-the-power-of-uber-into-3rd-party-applications--calls-to-the-api-can-be-made-to-request-information-on-available-car-types-driver-location-expressed-in-geocoordinates-time-estimates-estimated-prices-including-currency-conversion-when-applicable-as-well-as-user-account-history-and-activity--the-uber-api-documentation-describes-deep-linking-techniques-to-programmatically-launch-the-native-app-from-ios-or-android-or-the-uber-mobile-site-from-mobile-web--the-api-comes-with-a-detailed-style-guide-and-asset-package-for-implementing-licensed-brandings--the-uber-api-affiliate-program-grants-cash-and-issues-uber-credits-for-new-user-onboarding-through-a-3rd-party-app-
  version: 1.0.0
host: api.uber.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /products:
    get:
      summary: Product Types
      description: The Products endpoint returns information about the Uber products
        offered at a given location. The response includes the display name and other
        details about each product, and lists the products in the proper display order.
      operationId: the-products-endpoint-returns-information-about-the-uber-products-offered-at-a-given-location-the-re
      x-api-path-slug: products-get
      parameters:
      - in: query
        name: latitude
        description: Latitude component of location
      - in: query
        name: longitude
        description: Longitude component of location
      responses:
        200:
          description: OK
      tags:
      - Transportation
  /estimates/price:
    get:
      summary: Price Estimates
      description: The Price Estimates endpoint returns an estimated price range for
        each product offered at a given location. The price estimate is provided as
        a formatted string with the full price range and the localized currency symbol.<br><br>The
        response also includes low and high estimates, and the [ISO 4217](http://en.wikipedia.org/wiki/ISO_4217)
        currency code for situations requiring currency conversion. When surge is
        active for a particular product, its surge_multiplier will be greater than
        1, but the price estimate already factors in this multiplier.
      operationId: the-price-estimates-endpoint-returns-an-estimated-price-range-for-each-product-offered-at-a-given-lo
      x-api-path-slug: estimatesprice-get
      parameters:
      - in: query
        name: end_latitude
        description: Latitude component of end location
      - in: query
        name: end_longitude
        description: Longitude component of end location
      - in: query
        name: start_latitude
        description: Latitude component of start location
      - in: query
        name: start_longitude
        description: Longitude component of start location
      responses:
        200:
          description: OK
      tags:
      - Transportation
  /estimates/time:
    get:
      summary: Time Estimates
      description: The Time Estimates endpoint returns ETAs for all products offered
        at a given location, with the responses expressed as integers in seconds.
        We recommend that this endpoint be called every minute to provide the most
        accurate, up-to-date ETAs.
      operationId: the-time-estimates-endpoint-returns-etas-for-all-products-offered-at-a-given-location-with-the-respo
      x-api-path-slug: estimatestime-get
      parameters:
      - in: query
        name: customer_uuid
        description: Unique customer identifier to be used for experience customization
      - in: query
        name: product_id
        description: Unique identifier representing a specific product for a given
          latitude & longitude
      - in: query
        name: start_latitude
        description: Latitude component of start location
      - in: query
        name: start_longitude
        description: Longitude component of start location
      responses:
        200:
          description: OK
      tags:
      - Transportation
  /me:
    get:
      summary: User Profile
      description: The User Profile endpoint returns information about the Uber user
        that has authorized with the application.
      operationId: the-user-profile-endpoint-returns-information-about-the-uber-user-that-has-authorized-with-the-appli
      x-api-path-slug: me-get
      responses:
        200:
          description: OK
      tags:
      - Transportation
  /history:
    get:
      summary: User Activity
      description: The User Activity endpoint returns data about a user's lifetime
        activity with Uber. The response will include pickup locations and times,
        dropoff locations and times, the distance of past requests, and information
        about which products were requested.<br><br>The history array in the response
        will have a maximum length based on the limit parameter. The response value
        count may exceed limit, therefore subsequent API requests may be necessary.
      operationId: the-user-activity-endpoint-returns-data-about-a-users-lifetime-activity-with-uber-the-response-will-
      x-api-path-slug: history-get
      parameters:
      - in: query
        name: limit
        description: Number of items to retrieve
      - in: query
        name: offset
        description: Offset the list of returned results by this amount
      responses:
        200:
          description: OK
      tags:
      - Transportation