swagger: "2.0"
x-collection-name: Weatherbit.io
x-complete: 1
info:
  title: Weatherbit
  description: this-is-the-documentation-for-the-weatherbit-api---the-base-url-for-the-api-is-httpapi-weatherbit-iov2-0httpapi-weatherbit-iov2-0-or-httpsapi-weatherbit-iov2-0httpapi-weatherbit-iov2-0--below-is-the-swagger-ui-documentation-for-the-api--all-api-requests-require-the-key-parameter---------an-example-for-a-5-day-forecast-for-london-uk-would-be-httpapi-weatherbit-iov2-0forecast3hourlycitylondoncountryuk
  version: 2.0.0
host: api.weatherbit.io
basePath: /v2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /bulk/history/daily?city={city}&country={country}:
    get:
      summary: Get Bulk History Daily City Country
      description: Returns Historical Observations - Given a city in the format of
        City,ST or City. The state, and country parameters can be provided to make
        the search more accurate.
      operationId: returns-historical-observations--given-a-city-in-the-format-of-cityst-or-city-the-state-and-country-
      x-api-path-slug: bulkhistorydailycitycitycountrycountry-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city
        description: City search
      - in: path
        name: country
        description: Country Code (2 letter)
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: state
        description: Full name of state
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Bulk
      - History
      - Daily
      - City
      - City
      - '&country'
      - Country
  /bulk/history/daily?city_id={city_id}:
    get:
      summary: Get Bulk History Daily City
      description: Returns Historical Observations - Given a City ID.
      operationId: returns-historical-observations--given-a-city-id
      x-api-path-slug: bulkhistorydailycity-idcity-id-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city_id
        description: City ID
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Bulk
      - History
      - Daily
      - City
      - ""
      - City
  /bulk/history/daily?ip={ip}:
    get:
      summary: Get Bulk History Daily IP
      description: Returns Historical Observations - Given IP Address, or auto.
      operationId: returns-historical-observations--given-ip-address-or-auto
      x-api-path-slug: bulkhistorydailyipip-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: path
        name: ip
        description: IP Address, or auto
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Bulk
      - History
      - Daily
      - Ip
      - Ip
  /bulk/history/daily?lat={lat}&lon={lon}:
    get:
      summary: Get Bulk History Daily Lat Lon
      description: Returns Historical Observations - Given a lat, and lon.
      operationId: returns-historical-observations--given-a-lat-and-lon
      x-api-path-slug: bulkhistorydailylatlatlonlon-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: lat
        description: Latitude component of location
      - in: path
        name: lon
        description: Longitude component of location
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Bulk
      - History
      - Daily
      - Lat
      - Lat
      - '&lon'
      - Lon
  /bulk/history/daily?postal_code={postal_code}:
    get:
      summary: Get Bulk History Daily Postal Code
      description: Returns Historical Observations - Given a Postal Code.
      operationId: returns-historical-observations--given-a-postal-code
      x-api-path-slug: bulkhistorydailypostal-codepostal-code-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: country
        description: Country Code (2 letter)
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: postal_code
        description: Postal Code
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Bulk
      - History
      - Daily
      - Postal
      - Code
      - Postal
      - Code
  /bulk/history/daily?station={station}:
    get:
      summary: Get Bulk History Daily Station
      description: Returns Historical Observations - Given a station ID.
      operationId: returns-historical-observations--given-a-station-id
      x-api-path-slug: bulkhistorydailystationstation-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: path
        name: station
        description: Station ID
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Bulk
      - History
      - Daily
      - Station
      - Station
  /bulk/history/hourly?city={city}&country={country}:
    get:
      summary: Get Bulk History Hourly City & Country
      description: Returns Historical Observations - Given a city in the format of
        City,ST or City. The state, and country parameters can be provided to make
        the search more accurate.
      operationId: returns-historical-observations--given-a-city-in-the-format-of-cityst-or-city-the-state-and-country-
      x-api-path-slug: bulkhistoryhourlycitycitycountrycountry-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city
        description: City search
      - in: path
        name: country
        description: Country Code (2 letter)
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: state
        description: Full name of state
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Bulk
      - History
      - Hourly
      - City
      - City
      - '&country'
      - Country
  /bulk/history/hourly?city_id={city_id}:
    get:
      summary: Get Bulk History Hourly City
      description: Returns Historical Observations - Given a City ID.
      operationId: returns-historical-observations--given-a-city-id
      x-api-path-slug: bulkhistoryhourlycity-idcity-id-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city_id
        description: City ID
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Bulk
      - History
      - Hourly
      - City
      - ""
      - City
  /bulk/history/hourly?ip={ip}:
    get:
      summary: Get Bulk History Hourly IP
      description: Returns Historical Observations - Given IP Address, or auto.
      operationId: returns-historical-observations--given-ip-address-or-auto
      x-api-path-slug: bulkhistoryhourlyipip-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: path
        name: ip
        description: IP Address, or auto
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Bulk
      - History
      - Hourly
      - Ip
      - Ip
  /bulk/history/hourly?lat={lat}&lon={lon}:
    get:
      summary: Get Bulk History Hourly Lat & Lon
      description: Returns Historical Observations - Given a lat, and lon.
      operationId: returns-historical-observations--given-a-lat-and-lon
      x-api-path-slug: bulkhistoryhourlylatlatlonlon-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: lat
        description: Latitude component of location
      - in: path
        name: lon
        description: Longitude component of location
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Bulk
      - History
      - Hourly
      - Lat
      - Lat
      - '&lon'
      - Lon
  /bulk/history/hourly?postal_code={postal_code}:
    get:
      summary: Get Bulk History Hourly Postal Code
      description: Returns Historical Observations - Given a Postal Code.
      operationId: returns-historical-observations--given-a-postal-code-
      x-api-path-slug: bulkhistoryhourlypostal-codepostal-code-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: country
        description: Country Code (2 letter)
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: postal_code
        description: Postal Code
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Bulk
      - History
      - Hourly
      - Postal
      - Code
      - Postal
      - Code
  /bulk/history/hourly?station={station}:
    get:
      summary: Get Bulk History Hourly Station
      description: Returns Historical Observations - Given a station ID.
      operationId: returns-historical-observations--given-a-station-id
      x-api-path-slug: bulkhistoryhourlystationstation-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: path
        name: station
        description: Station ID
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Bulk
      - History
      - Hourly
      - Station
      - Station
  /bulk/{file}:
    get:
      summary: Get Bulk File
      description: '**(Advanced/Advanced+/Enterprise plans only)** Downloads bulk
        data files - OPTIONS: (forecast16d.json.gz - 16 day forecasts for cities >
        1000 population, current.json.gz - Current observations for cities > 1000
        population).'
      operationId: advancedadvancedenterprise-plans-only-downloads-bulk-data-files--options-forecast16djsongz--16-day-f
      x-api-path-slug: bulkfile-get
      parameters:
      - in: path
        name: file
        description: Filename (ie
      - in: query
        name: key
        description: Your registered API key
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Bulk
      - File
  /current?city={city}:
    get:
      summary: Get Current Cities
      description: '**(Advanced/Advanced+/Enterprise plans only)** Returns a group
        of Current Observations - Given a list of City IDs.'
      operationId: advancedadvancedenterprise-plans-only-returns-a-group-of-current-observations--given-a-list-of-city-
      x-api-path-slug: currentcitycity-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback - Example - callback=func
      - in: query
        name: cities
        description: Comma separated list of City IDs
      - in: query
        name: city
        description: A city name
        type: string
        format: string
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: marine
        description: Marine stations only (buoys, oil platforms, etc)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Current
      - Cities
      - Cities
  /current?ip={ip}:
    get:
      summary: Get Current IP
      description: Returns a Current Observation - Given an IP address, or auto.
      operationId: returns-a-current-observation--given-an-ip-address-or-auto
      x-api-path-slug: currentipip-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback - Example - callback=func
      - in: path
        name: ip
        description: IP Address, or auto
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: marine
        description: Marine stations only (buoys, oil platforms, etc)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Current
      - Ip
      - Ip
  /current?lat={lat}&lon={lon}:
    get:
      summary: Get Current Lat & Lon
      description: Returns a Current Observation - given a lat, and a lon.
      operationId: returns-a-current-observation--given-a-lat-and-a-lon
      x-api-path-slug: currentlatlatlonlon-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback - Example - callback=func
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: lat
        description: Latitude component of location
      - in: path
        name: lon
        description: Longitude component of location
      - in: query
        name: marine
        description: Marine stations only (buoys, oil platforms, etc)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Current
      - Lat
      - Lat
      - '&lon'
      - Lon
  /current?postal_code={postal_code}:
    get:
      summary: Get Current Postla Code Code
      description: Returns current weather observation - Given a Postal Code.
      operationId: returns-current-weather-observation--given-a-postal-code-
      x-api-path-slug: currentpostal-codepostal-code-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback - Example - callback=func
      - in: query
        name: country
        description: Country Code (2 letter)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: marine
        description: Marine stations only (buoys, oil platforms, etc)
      - in: path
        name: postal_code
        description: Postal Code
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Current
      - Postal
      - Code
      - Postal
      - Code
  /current?station={station}:
    get:
      summary: Get Current Station Station
      description: Returns a Current Observation - Given a station ID.
      operationId: returns-a-current-observation--given-a-station-id
      x-api-path-slug: currentstationstation-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: station
        description: Station Call ID
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Current
      - Station
      - Station
  /current?stations={stations}:
    get:
      summary: Get Current Stations Stations
      description: '**(Advanced/Advanced+/Enterprise plans only)** Returns a group
        of Current Observations - Given a list of Station Call IDs.'
      operationId: advancedadvancedenterprise-plans-only-returns-a-group-of-current-observations--given-a-list-of-stati
      x-api-path-slug: currentstationsstations-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: stations
        description: Comma separated list of Station Call IDs
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Current
      - Stations
      - Stations
  /forecast/3hourly?city={city}&country={country}:
    get:
      summary: Get Forecast 3hourly City & Country
      description: Returns a 3-hourly forecast, where each point represents a three
        hour   period. Every point has a datetime string in the format "YYYY-MM-DD:HH".
        Time is UTC.
      operationId: returns-a-3hourly-forecast-where-each-point-represents-a-three-hour---period-every-point-has-a-datet
      x-api-path-slug: forecast3hourlycitycitycountrycountry-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city
        description: City search
      - in: path
        name: country
        description: Country Code (2 letter)
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: state
        description: Full name of state
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - 3hourly
      - City
      - City
      - '&country'
      - Country
  /forecast/3hourly?city_id={city_id}:
    get:
      summary: Get Forecast 3hourly City
      description: Returns a 3-hourly forecast, where each point represents a three
        hour   period. Every point has a datetime string in the format "YYYY-MM-DD:HH".
        Time is UTC.
      operationId: returns-a-3hourly-forecast-where-each-point-represents-a-three-hour---period-every-point-has-a-datet
      x-api-path-slug: forecast3hourlycity-idcity-id-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city_id
        description: City ID
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - 3hourly
      - City
      - ""
      - City
  /forecast/3hourly?ip={ip}:
    get:
      summary: Get Forecast 3hourly IP
      description: Returns a 3-hourly forecast, where each point represents a three
        hour   period. Every point has a datetime string in the format "YYYY-MM-DD:HH".
        Time is UTC.
      operationId: returns-a-3hourly-forecast-where-each-point-represents-a-three-hour---period-every-point-has-a-datet
      x-api-path-slug: forecast3hourlyipip-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: days
        description: Number of days to return
      - in: path
        name: ip
        description: IP address, or auto
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - 3hourly
      - Ip
      - Ip
  /forecast/3hourly?lat={lat}&lon={lon}:
    get:
      summary: Get Forecast 3hourly Lat & Lon
      description: Returns a 3-hourly forecast, where each point represents a three
        hour   period. Every point has a datetime string in the format "YYYY-MM-DD:HH".
        Time is UTC.
      operationId: returns-a-3hourly-forecast-where-each-point-represents-a-three-hour---period-every-point-has-a-datet
      x-api-path-slug: forecast3hourlylatlatlonlon-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: lat
        description: Latitude component of location
      - in: path
        name: lon
        description: Longitude component of location
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - 3hourly
      - Lat
      - Lat
      - '&lon'
      - Lon
  /forecast/3hourly?postal_code={postal_code}:
    get:
      summary: Get Forecast 3hourly Postla Code Code
      description: Returns a 3-hourly forecast, where each point represents a three
        hour period. Every point has a datetime string in the format "YYYY-MM-DD:HH".
        Time is UTC.
      operationId: returns-a-3hourly-forecast-where-each-point-represents-a-three-hour-period-every-point-has-a-datetim
      x-api-path-slug: forecast3hourlypostal-codepostal-code-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: country
        description: Country Code (2 letter)
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: postal_code
        description: Postal Code
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - 3hourly
      - Postal
      - Code
      - Postal
      - Code
  /forecast/daily?city={city}&country={country}:
    get:
      summary: Get Forecast Daily City & Country
      description: '**(REQUIRED: Basic Plan or Higher)** Returns a daily forecast,
        where each point represents one day (24hr) period. Every point has a datetime
        string in the format "YYYY-MM-DD". One day begins at 00:00 UTC, and ends at
        23:59 UTC. Accepts a city in the format of City,ST or City. The state, and
        country parameters can be provided to make the search more accurate.'
      operationId: required-basic-plan-or-higher-returns-a-daily-forecast-where-each-point-represents-one-day-24hr-peri
      x-api-path-slug: forecastdailycitycitycountrycountry-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city
        description: City search
      - in: path
        name: country
        description: Country Code (2 letter)
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: state
        description: Full name of state
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Daily
      - City
      - City
      - '&country'
      - Country
  /forecast/daily?city_id={city_id}:
    get:
      summary: Get Forecast Daily City
      description: '**(REQUIRED: Basic Plan or Higher)** Returns a daily forecast,
        where each point represents one day (24hr) period. Every point has a datetime
        string in the format "YYYY-MM-DD". One day begins at 00:00 UTC, and ends at
        23:59 UTC.'
      operationId: required-basic-plan-or-higher-returns-a-daily-forecast-where-each-point-represents-one-day-24hr-peri
      x-api-path-slug: forecastdailycity-idcity-id-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city_id
        description: City ID
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Daily
      - City
      - ""
      - City
  /forecast/daily?ip={ip}:
    get:
      summary: Get Forecast Daily IP
      description: '**(REQUIRED: Basic Plan or Higher)** Returns a daily forecast,
        where each point represents one day (24hr) period. Every point has a datetime
        string in the format "YYYY-MM-DD". One day begins at 00:00 UTC, and ends at
        23:59 UTC.'
      operationId: required-basic-plan-or-higher-returns-a-daily-forecast-where-each-point-represents-one-day-24hr-peri
      x-api-path-slug: forecastdailyipip-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: days
        description: Number of days to return
      - in: path
        name: ip
        description: IP address, or auto
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Daily
      - Ip
      - Ip
  /forecast/daily?lat={lat}&lon={lon}:
    get:
      summary: Get Forecast Daily Lat & Lon
      description: '**(REQUIRED: Basic Plan or Higher)** Returns a daily forecast,
        where each point represents one day (24hr) period. Every point has a datetime
        string in the format "YYYY-MM-DD". One day begins at 00:00 UTC, and ends at
        23:59 UTC.'
      operationId: required-basic-plan-or-higher-returns-a-daily-forecast-where-each-point-represents-one-day-24hr-peri
      x-api-path-slug: forecastdailylatlatlonlon-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: lat
        description: Latitude component of location
      - in: path
        name: lon
        description: Longitude component of location
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Daily
      - Lat
      - Lat
      - '&lon'
      - Lon
  /forecast/daily?postal_code={postal_code}:
    get:
      summary: Get Forecast Daily Postla Code Code
      description: '**(REQUIRED: Basic Plan or Higher)** Returns a daily forecast,
        where each point represents one day (24hr) period. Every point has a datetime
        string in the format "YYYY-MM-DD". One day begins at 00:00 UTC, and ends at
        23:59 UTC.'
      operationId: required-basic-plan-or-higher-returns-a-daily-forecast-where-each-point-represents-one-day-24hr-peri
      x-api-path-slug: forecastdailypostal-codepostal-code-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: country
        description: Country Code (2 letter)
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: postal_code
        description: Postal Code
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Daily
      - Postal
      - Code
      - Postal
      - Code
  /forecast/hourly?city={city}&country={country}:
    get:
      summary: Get Forecast Hourly City & Country
      description: '**(REQUIRED: Developer Plan or Higher)** Returns an hourly forecast,
        where each point represents a one hour   period. Every point has a datetime
        string in the format "YYYY-MM-DD:HH". Time is UTC. Accepts a city in the format
        of City,ST or City. The state, and country parameters can be provided to make
        the search more accurate.'
      operationId: required-developer-plan-or-higher-returns-an-hourly-forecast-where-each-point-represents-a-one-hour-
      x-api-path-slug: forecasthourlycitycitycountrycountry-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city
        description: City search
      - in: path
        name: country
        description: Country Code (2 letter)
      - in: query
        name: hours
        description: Number of hours to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: state
        description: Full name of state
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Hourly
      - City
      - City
      - '&country'
      - Country
  /forecast/hourly?city_id={city_id}:
    get:
      summary: Get Forecast Hourly City
      description: '**(REQUIRED: Developer Plan or Higher)** Returns an hourly forecast,
        where each point represents a one hour   period. Every point has a datetime
        string in the format "YYYY-MM-DD:HH". Time is UTC.'
      operationId: required-developer-plan-or-higher-returns-an-hourly-forecast-where-each-point-represents-a-one-hour-
      x-api-path-slug: forecasthourlycity-idcity-id-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city_id
        description: City ID
      - in: query
        name: hours
        description: Number of hours to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Hourly
      - City
      - ""
      - City
  /forecast/hourly?ip={ip}:
    get:
      summary: Get Forecast Hourly IP
      description: '**(REQUIRED: Developer Plan or Higher)** Returns an hourly forecast,
        where each point represents a one hour period. Every point has a datetime
        string in the format "YYYY-MM-DD:HH". Time is UTC.'
      operationId: required-developer-plan-or-higher-returns-an-hourly-forecast-where-each-point-represents-a-one-hour-
      x-api-path-slug: forecasthourlyipip-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: hours
        description: Number of hours to return
      - in: path
        name: ip
        description: IP address, or auto
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Hourly
      - Ip
      - Ip
  /forecast/hourly?lat={lat}&lon={lon}:
    get:
      summary: Get Forecast Hourly Lat & Lon
      description: '**(REQUIRED: Developer Plan or Higher)** Returns an hourly forecast,
        where each point represents a one hour period. Every point has a datetime
        string in the format "YYYY-MM-DD:HH". Time is UTC.'
      operationId: required-developer-plan-or-higher-returns-an-hourly-forecast-where-each-point-represents-a-one-hour-
      x-api-path-slug: forecasthourlylatlatlonlon-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: hours
        description: Number of hours to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: lat
        description: Latitude component of location
      - in: path
        name: lon
        description: Longitude component of location
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Hourly
      - Lat
      - Lat
      - '&lon'
      - Lon
  /forecast/hourly?postal_code={postal_code}:
    get:
      summary: Get Forecast Hourly Postla Code Code
      description: '**(REQUIRED: Developer Plan or Higher)** Returns an hourly forecast,
        where each point represents a one hour   period. Every point has a datetime
        string in the format "YYYY-MM-DD:HH". Time is UTC.'
      operationId: required-developer-plan-or-higher-returns-an-hourly-forecast-where-each-point-represents-a-one-hour-
      x-api-path-slug: forecasthourlypostal-codepostal-code-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: country
        description: Country Code (2 letter)
      - in: query
        name: hours
        description: Number of hours to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: postal_code
        description: Postal Code
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Hourly
      - Postal
      - Code
      - Postal
      - Code
  /history/daily?city={city}&country={country}:
    get:
      summary: Get History Daily City & Country
      description: Returns Historical Observations - Given a city in the format of
        City,ST or City. The state, and country parameters can be provided to make
        the search more accurate. **(LIMIT 1 day for Low Volume plans. LIMIT 7 days
        for Basic/Developer. LIMIT 30 days for Advanced/Advanced+/Enterprise)**
      operationId: returns-historical-observations--given-a-city-in-the-format-of-cityst-or-city-the-state-and-country-
      x-api-path-slug: historydailycitycitycountrycountry-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city
        description: City search
      - in: path
        name: country
        description: Country Code (2 letter)
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: state
        description: Full name of state
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - History
      - Daily
      - City
      - City
      - '&country'
      - Country
  /history/daily?city_id={city_id}:
    get:
      summary: Get History Daily City
      description: Returns Historical Observations - Given a City ID. **(LIMIT 1 day
        for Low Volume plans. LIMIT 7 days for Basic/Developer. LIMIT 30 days for
        Advanced/Advanced+/Enterprise)**
      operationId: returns-historical-observations--given-a-city-id-limit-1-day-for-low-volume-plans-limit-7-days-for-b
      x-api-path-slug: historydailycity-idcity-id-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city_id
        description: City ID
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - History
      - Daily
      - City
      - ""
      - City
  /history/daily?ip={ip}:
    get:
      summary: Get History Daily IP
      description: Returns Historical Observations - Given IP Address, or auto. **(LIMIT
        1 day for Low Volume plans. LIMIT 7 days for Basic/Developer. LIMIT 30 days
        for Advanced/Advanced+/Enterprise)**
      operationId: returns-historical-observations--given-ip-address-or-auto-limit-1-day-for-low-volume-plans-limit-7-d
      x-api-path-slug: historydailyipip-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: path
        name: ip
        description: IP Address, or auto
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - History
      - Daily
      - Ip
      - Ip
  /history/daily?lat={lat}&lon={lon}:
    get:
      summary: Get History Daily Lat & Lon
      description: Returns Historical Observations - Given a lat, and lon. **(LIMIT
        1 day for Low Volume plans. LIMIT 7 days for Basic/Developer. LIMIT 30 days
        for Advanced/Advanced+/Enterprise)**
      operationId: returns-historical-observations--given-a-lat-and-lon-limit-1-day-for-low-volume-plans-limit-7-days-f
      x-api-path-slug: historydailylatlatlonlon-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: lat
        description: Latitude component of location
      - in: path
        name: lon
        description: Longitude component of location
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - History
      - Daily
      - Lat
      - Lat
      - '&lon'
      - Lon
  /history/daily?postal_code={postal_code}:
    get:
      summary: Get History Daily Postla Code Code
      description: Returns Historical Observations - Given a Postal Code. **(LIMIT
        1 day for Low Volume plans. LIMIT 7 days for Basic/Developer. LIMIT 30 days
        for Advanced/Advanced+/Enterprise)**
      operationId: returns-historical-observations--given-a-postal-code-limit-1-day-for-low-volume-plans-limit-7-days-f
      x-api-path-slug: historydailypostal-codepostal-code-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: country
        description: Country Code (2 letter)
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: postal_code
        description: Postal Code
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - History
      - Daily
      - Postal
      - Code
      - Postal
      - Code
  /history/daily?station={station}:
    get:
      summary: Get History Daily Station Station
      description: Returns Historical Observations - Given a station ID. **(LIMIT
        1 day for Low Volume plans. LIMIT 7 days for Basic/Developer. LIMIT 30 days
        for Advanced/Advanced+/Enterprise)**
      operationId: returns-historical-observations--given-a-station-id-limit-1-day-for-low-volume-plans-limit-7-days-fo
      x-api-path-slug: historydailystationstation-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: path
        name: station
        description: Station ID
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - History
      - Daily
      - Station
      - Station
  /history/energy/bbox?lat1={lat1}&lon1={lon1}&lat2={lat2}&lon2={lon2}:
    get:
      summary: Get History Energy Bbox Lat1 Lat1 &lon1 Lon1 &lat2 Lat2 &lon2 Lon2
      description: 'Returns aggregate energy specific historical weather fields, over
        a specified time period. Supply a bounding box ex: lat1=40&lon1=-78&lat2=38&lon2=-80.
        This API will return UP TO 150 stations, aggregated by the specified time
        period start_date to end_date.'
      operationId: returns-aggregate-energy-specific-historical-weather-fields-over-a-specified-time-period-supply-a-bo
      x-api-path-slug: historyenergybboxlat1lat1lon1lon1lat2lat2lon2lon2-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: path
        name: lat1
        description: Latitude of upper left corner
      - in: path
        name: lat2
        description: Latitude of lower right corner
      - in: path
        name: lon1
        description: Longitude of upper left corner
      - in: path
        name: lon2
        description: Longitude of lower right corner
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - History
      - Energy
      - Bbox
      - Lat1
      - Lat1
      - '&lon1'
      - Lon1
      - '&lat2'
      - Lat2
      - '&lon2'
      - Lon2
  /history/energy?lat={lat}&lon={lon}:
    get:
      summary: Get History Energy Lat & Lon
      description: Returns aggregate energy specific historical weather fields, over
        a specified time period.
      operationId: returns-aggregate-energy-specific-historical-weather-fields-over-a-specified-time-period
      x-api-path-slug: historyenergylatlatlonlon-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: path
        name: lat
        description: Latitude component of location
      - in: path
        name: lon
        description: Longitude component of location
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - History
      - Energy
      - Lat
      - Lat
      - '&lon'
      - Lon
  /history/hourly?city={city}&country={country}:
    get:
      summary: Get History Hourly City & Country
      description: Returns Historical Observations - Given a city in the format of
        City,ST or City. The state, and country parameters can be provided to make
        the search more accurate. **(LIMIT 1 day for Low Volume plans. LIMIT 7 days
        for Basic/Developer. LIMIT 30 days for Advanced/Advanced+/Enterprise)**
      operationId: returns-historical-observations--given-a-city-in-the-format-of-cityst-or-city-the-state-and-country-
      x-api-path-slug: historyhourlycitycitycountrycountry-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city
        description: City search
      - in: path
        name: country
        description: Country Code (2 letter)
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: state
        description: Full name of state
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - History
      - Hourly
      - City
      - City
      - '&country'
      - Country
  /history/hourly?city_id={city_id}:
    get:
      summary: Get History Hourly City
      description: Returns Historical Observations - Given a City ID. **(LIMIT 1 day
        for Low Volume plans. LIMIT 7 days for Basic/Developer. LIMIT 30 days for
        Advanced/Advanced+/Enterprise)**
      operationId: returns-historical-observations--given-a-city-id-limit-1-day-for-low-volume-plans-limit-7-days-for-b
      x-api-path-slug: historyhourlycity-idcity-id-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city_id
        description: City ID
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - History
      - Hourly
      - City
      - ""
      - City
  /history/hourly?ip={ip}:
    get:
      summary: Get History Hourly IP
      description: Returns Historical Observations - Given IP Address, or auto. **(LIMIT
        1 day for Low Volume plans. LIMIT 7 days for Basic/Developer. LIMIT 30 days
        for Advanced/Advanced+/Enterprise)**
      operationId: returns-historical-observations--given-ip-address-or-auto-limit-1-day-for-low-volume-plans-limit-7-d
      x-api-path-slug: historyhourlyipip-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: path
        name: ip
        description: IP Address, or auto
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - History
      - Hourly
      - Ip
      - Ip
  /history/hourly?lat={lat}&lon={lon}:
    get:
      summary: Get History Hourly Lat & Lon
      description: Returns Historical Observations - Given a lat, and lon. **(LIMIT
        1 day for Low Volume plans. LIMIT 7 days for Basic/Developer. LIMIT 30 days
        for Advanced/Advanced+/Enterprise)**
      operationId: returns-historical-observations--given-a-lat-and-lon-limit-1-day-for-low-volume-plans-limit-7-days-f
      x-api-path-slug: historyhourlylatlatlonlon-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: lat
        description: Latitude component of location
      - in: path
        name: lon
        description: Longitude component of location
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - History
      - Hourly
      - Lat
      - Lat
      - '&lon'
      - Lon
  /history/hourly?postal_code={postal_code}:
    get:
      summary: Get History Hourly Postal Code
      description: Returns Historical Observations - Given a Postal Code. **(LIMIT
        1 day for Low Volume plans. LIMIT 7 days for Basic/Developer. LIMIT 30 days
        for Advanced/Advanced+/Enterprise)**
      operationId: returns-historical-observations--given-a-postal-code-limit-1-day-for-low-volume-plans-limit-7-days-f
      x-api-path-slug: historyhourlypostal-codepostal-code-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: country
        description: Country Code (2 letter)
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: postal_code
        description: Postal Code
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - History
      - Hourly
      - Postal
      - Code
      - Postal
      - Code
  /history/hourly?station={station}:
    get:
      summary: Get History Hourly Station Station
      description: Returns Historical Observations - Given a station ID. **(LIMIT
        1 day for Low Volume plans. LIMIT 7 days for Basic/Developer. LIMIT 30 days
        for Advanced/Advanced+/Enterprise)**
      operationId: returns-historical-observations--given-a-station-id-limit-1-day-for-low-volume-plans-limit-7-days-fo
      x-api-path-slug: historyhourlystationstation-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: path
        name: station
        description: Station ID
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - History
      - Hourly
      - Station
      - Station
  /ip?ip={ip}:
    get:
      summary: Get IP
      description: Returns a geolocation object. Given an IP address. If no IP supplied,
        will use request IP address.
      operationId: returns-a-geolocation-object-given-an-ip-address-if-no-ip-supplied-will-use-request-ip-address
      x-api-path-slug: ipipip-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: exclude
        description: exclude=all => return IP address only
      - in: query
        name: format
        description: '&format=none => return IP address as string'
      - in: path
        name: ip
        description: IP address
      - in: query
        name: key
        description: Your registered API key
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Ip
      - Ip
      - Ip