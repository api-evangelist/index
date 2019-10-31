swagger: "2.0"
x-collection-name: link.fish
x-complete: 1
info:
  title: link.fish
  description: api-to-easily-extract-data-from-websites--base-urlall-urls-referenced-in-the-documentation-have-the-following-basehttpsapi-link-fishthe-rest-api-is-only-served-over-https--to-ensure-data-privacy-unencrypted-http-is-not-supported--authenticationhttp-requests-to-the-rest-api-are-protected-with-http-basic-authenticationhttpsen-wikipedia-orgwikibasic-access-authentication--you-will-use-the-email-address-of-your-link-fish-account-as-the-username-and-your-api-access-token-as-the-password-for-http-basic-authentication-if-you-do-not-have-an-account-yet-go-to-httpslink-fishapihttpslink-fishapi-and-create-one-first-you-will-receive-the-api-access-token-automatically-via-email-after-you-signed-up--to-generate-a-new-token-and-invalidate-the-current-one-log-into-your-link-fish--account-at-httpsapp-link-fishhttpsapp-link-fish-and-go-to-plugins--api-dashboardthere-you-can-also-see-how-many-credits-you-used-already--errorsthe-api-uses-standard-http-status-codes-to-indicate-the-success-or-failure-of-the-api-call--the-body-of-the-response-will-be-json-in-the-following-format--status-http-status-code--message-error-messagelike-for-example-when-the-authorization-is-not-provided-or-wrong--status-401--message-unauthorized-request-idseach-api-request-has-an-associated-request-identifier--you-can-find-it-in-the-response-headers-under-xlfrequestid--in-case-you-have-problems-please-provide-this-identifier-that-we-can-help-you-as-good-and-fast-as-possible-examplexlfrequestid-f7f0036f5277421ab143f7a151571d18-item-formatthe-data-is-by-default-deeply-nested--so-if-it-should-be-checked-if-there-is-an-offer-with-a-price-the-whole-tree-has-to-be-checked--to-make-that-simpler-it-is-also-possible-to-return-the-data-flat--if-selected-it-will-flatten-the-tree-by-copying-all-the-data-to-the-main-level-under-a-property-with-the-name-of-its-type-and-link-the-data-internally-information-we-created-a-node-module-which-allows-converting-between-the-two-formats--it-did-not-get-open-sourced-yet--if-you-are-in-need-simply-contact-us-via-apilink-fish--response-content-typeby-default-all-data-gets-returned-as-json--if-the-data-should-be-returned-as-xml-add-the-following-headeraccept-applicationxml-creditsdepending-on-the-request-made-a-different-amount-of-credits-get-charged--how-many-which-request-costs-can-be-found-on-the-api-pricing-pagehttplink-fishapipricing--additionally-does-a--header-named-xlfcreditscharged-get-added-to-each-successful-response-with-the-amount-of-credits-charged-examplexlfcreditscharged-1you-can-check-anytime-how-many-credits-you-did-use-already-by-logging-into-your-link-fish--account-at-httpsapp-link-fishhttpsapp-link-fish-and-checking-under--plugins--api-dashboardif-you-have-problems-questions-or-improvement-advice-please-send-us-an-email-to-apilink-fish
  termsOfService: https://link.fish/terms-of-service/
  contact:
    name: link.fish
    url: https://link.fish/api
    email: api@link.fish
  version: "2017-12-01"
host: api.link.fish
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Urls/apps:
    get:
      summary: Get mobile apps
      description: |-
        Visits the URL and checks if there are mobile apps on them and returns the found ones.

        Will by default return the app identifiers and not the full URL to the apps. To return URLs instead set the parameter "return_urls" to true.

        The URLs can also be created manually like this:

        | Property | URL                                                |
        | -------- | -------------------------------------------------- |
        | android  | https://play.google.com/store/apps/details?id={ID} |
        | ios      | https://itunes.apple.com/us/app/app-name/id{ID}    |

        Properties only get set when a value for it has been found. That means that if no app has been found only the property "url" will be set.
      operationId: Urls.apps.get
      x-api-path-slug: urlsapps-get
      parameters:
      - in: query
        name: browser_render
        description: If the page should be fully rendered with a browser to extract
          data
      - in: query
        name: return_urls
        description: Returns app URLs instead of the identifiers
      - in: query
        name: url
        description: The URL of the website to query
      responses:
        200:
          description: OK
      tags:
      - Urls
      - Apps
  /Urls/browser-data:
    get:
      summary: Extract data (browser)
      description: Visits the URL with a full browser and extracts the data. This
        request costs 5 credits.
      operationId: Urls.browser_data.get
      x-api-path-slug: urlsbrowserdata-get
      parameters:
      - in: query
        name: item_format
        description: If the items should be return normal with multiple levels or
          flat with just one level and linked instead
      - in: query
        name: screenshot
        description: If and what kind of screenshot should be returned
      - in: query
        name: screenshot_file_format
        description: The file format of the screenshot
      - in: query
        name: screenshot_width
        description: The widh of the screenshot in pixel
      - in: query
        name: simplify_special_types
        description: Some types like PropertyValue do save key and value in separate
          properties which makes the data harder to process
      - in: query
        name: url
        description: The URL of the website to query
      responses:
        200:
          description: OK
      tags:
      - Urls
      - Browser
      - Data
  /Urls/browser-screenshot:
    get:
      summary: Generate screenshot (browser)
      description: Visits the URL with full browser and creates a screenshot. This
        request costs 5 credits.
      operationId: Urls.browser_screenshot.get
      x-api-path-slug: urlsbrowserscreenshot-get
      parameters:
      - in: query
        name: file_format
        description: The file format of the screenshot
      - in: query
        name: type
        description: What kind of screenshot should be returned
      - in: query
        name: url
        description: The URL of the website to create screenshot of
      - in: query
        name: width
        description: The widh of the screenshot in pixel
      responses:
        200:
          description: OK
      tags:
      - Urls
      - Browser
      - Screenshot
  /Urls/data:
    get:
      summary: Extract data
      description: Visits the URL and extracts the data.
      operationId: Urls.data.get
      x-api-path-slug: urlsdata-get
      parameters:
      - in: query
        name: browser_render
        description: If the page should be fully rendered with a browser to extract
          data
      - in: query
        name: item_format
        description: If the items should be return normal with multiple levels or
          flat with just one level and linked instead
      - in: query
        name: simplify_special_types
        description: Some types like PropertyValue do save key and value in separate
          properties which makes the data harder to process
      - in: query
        name: url
        description: The URL of the website to query
      responses:
        200:
          description: OK
      tags:
      - Urls
      - Data
  /Urls/geo-coordinates:
    get:
      summary: Get geo coordinates
      description: |-
        Visits the URL and checks if there are Geo Coordinates on them and returns the found ones.

        Properties only get set when a value for both latitude and longitude have been found. That means that if no geo coordinates have been found only the property "url" will be set.
      operationId: Urls.geo_coordinates.get
      x-api-path-slug: urlsgeocoordinates-get
      parameters:
      - in: query
        name: browser_render
        description: If the page should be fully rendered with a browser to extract
          data
      - in: query
        name: url
        description: The URL of the website to query
      responses:
        200:
          description: OK
      tags:
      - Urls
      - Geo
      - Coordinates
  /Urls/social-media:
    get:
      summary: Get social media accounts
      description: |-
        Visits the URL and checks if there are any social media accounts and returns the found ones.

        Will by default return the account identifiers and not the full URL to the profiles. To return URLs instead set the parameter "return_urls" to true.

        The URLs can also be created manually like this:

        | Property        | URL                                    |
        | --------------- | -------------------------------------- |
        | facebookPage    | https://facebook.com/{ID}              |
        | githubUser      | https://github.com/{ID}                |
        | googlePlus      | https://plus.google.com/+{ID}          |
        | instagram       | https://instagram.com/{ID}             |
        | linkedInCompany | https://linkedin.com/company/{ID}      |
        | pinterest       | https://pinterest.com/{ID}             |
        | twitter         | https://twitter.com/{ID}               |
        | youTubeUser     | https://youtube.com/user/{ID}          |

        Properties only get set when a value for it has been found. That means that if no social media account has been found only the property "url" will be set.
      operationId: Urls.social_media.get
      x-api-path-slug: urlssocialmedia-get
      parameters:
      - in: query
        name: browser_render
        description: If the page should be fully rendered with a browser to extract
          data
      - in: query
        name: return_urls
        description: Returns profile URLs instead of the profile names/ids
      - in: query
        name: url
        description: The URL of the website to query
      responses:
        200:
          description: OK
      tags:
      - Urls
      - Social
      - Media