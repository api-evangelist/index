swagger: "2.0"
x-collection-name: Google PageSpeed Insights
x-complete: 1
info:
  title: PageSpeed Insights
  description: analyzes-the-performance-of-a-web-page-and-provides-tailored-suggestions-to-make-that-page-faster-
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /pagespeedonline/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /runPagespeed:
    get:
      summary: Run PageSpeed Analysis
      description: Runs PageSpeed analysis on the page at the specified URL, and returns
        PageSpeed scores, a list of suggestions to make that page faster, and other
        information.
      operationId: pagespeedonline.pagespeedapi.runpagespeed
      x-api-path-slug: runpagespeed-get
      parameters:
      - in: query
        name: filter_third_party_resources
        description: Indicates if third party resources should be filtered out before
          PageSpeed analysis
      - in: query
        name: locale
        description: The locale used to localize formatted results
      - in: query
        name: rule
        description: A PageSpeed rule to run; if none are given, all rules are run
      - in: query
        name: screenshot
        description: Indicates if binary data containing a screenshot should be included
      - in: query
        name: strategy
        description: The analysis strategy to use
      - in: query
        name: url
        description: The URL to fetch and analyze
      responses:
        200:
          description: OK
      tags:
      - Pages
      - Speed
      - Analysis