swagger: "2.0"
x-collection-name: Yahoo
x-complete: 1
info:
  title: Yahoo Weather
  description: access-uptodate-weather-information-for-your-location-including-condition-codes-
  version: 1.0.0
host: weather.yahooapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /forecastrss:
    get:
      summary: ""
      description: Retrieves weather information for a location.
      operationId: Get_weather.get_
      x-api-path-slug: forecastrss-get
      parameters:
      - in: query
        name: u
        description: Units for temperature (case sensitive)
      - in: query
        name: w
        description: The location for the weather forecast as a WOEID, example is
          Palo Alto, CA
      responses:
        200:
          description: OK
      tags:
      - ""