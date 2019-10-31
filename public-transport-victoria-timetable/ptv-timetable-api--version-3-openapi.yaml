swagger: "2.0"
x-collection-name: Public Transport Victoria Timetable
x-complete: 1
info:
  title: Public Transport Victoria Timetable
  description: the-ptv-timetable-api-provides-direct-access-to-public-transport-victorias-public-transport-timetable-data--the-api-returns-scheduled-timetable-route-and-stop-data-for-all-metropolitan-and-regional-train-tram-and-bus-services-in-victoria-including-night-networknight-train-and-night-tram-data-are-included-in-metropolitan-train-and-tram-services-data-respectively-whereas-night-bus-is-a-separate-route-type--the-api-also-returns-realtime-data-for-metropolitan-train-tram-and-bus-services-where-this-data-is-made-available-to-ptv-as-well-as-disruption-information-stop-facility-information-and-access-to-myki-ticket-outlet-data-
  termsOfService: http://ptv.vic.gov.au/ptv-timetable-api/
  contact:
    name: Public Transport Victoria
    url: http://ptv.vic.gov.au/digital
  version: v3
host: timetableapi.ptv.vic.gov.au
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/departures/route_type/{route_type}/stop/{stop_id}:
    get:
      summary: Get V3 Departures Route Type Route Type Stop Stop
      description: View departures for all routes from a stop.
      operationId: Departures_GetForStop
      x-api-path-slug: v3departuresroute-typeroute-typestopstop-id-get
      parameters:
      - in: query
        name: date_utc
        description: Filter by the date and time of the request (ISO 8601 UTC format)
      - in: query
        name: devid
        description: Your developer id
      - in: query
        name: direction_id
        description: Filter by identifier of direction of travel; values returned
          by Directions API - /v3/directions/route/{route_id}
      - in: query
        name: expand
        description: List objects to be returned in full (i
      - in: query
        name: gtfs
        description: Indicates that stop_id parameter will accept GTFS stop_id data
      - in: query
        name: include_cancelled
        description: Indicates if cancelled services (if they exist) are returned
          (default = false) - metropolitan train only
      - in: query
        name: max_results
        description: Maximum number of results returned
      - in: query
        name: platform_numbers
        description: Filter by platform number at stop
      - in: path
        name: route_type
        description: Number identifying transport mode; values returned via RouteTypes
          API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: path
        name: stop_id
        description: Identifier of stop; values returned by Stops API
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Departures
      - Route
      - Type
      - Route
      - Type
      - Stop
      - Stop
      - Id
  /v3/departures/route_type/{route_type}/stop/{stop_id}/route/{route_id}:
    get:
      summary: Get V3 Departures Route Type Route Type Stop Stop Route Route
      description: View departures for a specific route from a stop.
      operationId: Departures_GetForStopAndRoute
      x-api-path-slug: v3departuresroute-typeroute-typestopstop-idrouteroute-id-get
      parameters:
      - in: query
        name: date_utc
        description: Filter by the date and time of the request (ISO 8601 UTC format)
      - in: query
        name: devid
        description: Your developer id
      - in: query
        name: direction_id
        description: Filter by identifier of direction of travel; values returned
          by Directions API - /v3/directions/route/{route_id}
      - in: query
        name: expand
        description: List objects to be returned in full (i
      - in: query
        name: gtfs
        description: Indicates that stop_id parameter will accept GTFS stop_id data
      - in: query
        name: include_cancelled
        description: Indicates if cancelled services (if they exist) are returned
          (default = false) - metropolitan train only
      - in: query
        name: max_results
        description: Maximum number of results returned
      - in: path
        name: route_id
        description: Identifier of route; values returned by Routes API - v3/routes
      - in: path
        name: route_type
        description: Number identifying transport mode; values returned via RouteTypes
          API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: path
        name: stop_id
        description: Identifier of stop; values returned by Stops API
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Departures
      - Route
      - Type
      - Route
      - Type
      - Stop
      - Stop
      - Id
      - Route
      - Route
      - Id
  /v3/directions/route/{route_id}:
    get:
      summary: Get V3 Directions Route Route
      description: View directions that a route travels in.
      operationId: Directions_ForRoute
      x-api-path-slug: v3directionsrouteroute-id-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: route_id
        description: Identifier of route; values returned by Routes API - v3/routes
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Directions
      - Route
      - Route
      - Id
  /v3/directions/{direction_id}:
    get:
      summary: Get V3 Directions Direction
      description: View all routes for a direction of travel.
      operationId: Directions_ForDirection
      x-api-path-slug: v3directionsdirection-id-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: direction_id
        description: Identifier of direction of travel; values returned by Directions
          API - /v3/directions/route/{route_id}
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Directions
      - Direction
      - Id
  /v3/directions/{direction_id}/route_type/{route_type}:
    get:
      summary: Get V3 Directions Direction Route Type Route Type
      description: View all routes of a particular type for a direction of travel.
      operationId: Directions_ForDirectionAndType
      x-api-path-slug: v3directionsdirection-idroute-typeroute-type-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: direction_id
        description: Identifier of direction of travel; values returned by Directions
          API - /v3/directions/route/{route_id}
      - in: path
        name: route_type
        description: Number identifying transport mode; values returned via RouteTypes
          API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Directions
      - Direction
      - Id
      - Route
      - Type
      - Route
      - Type
  /v3/disruptions:
    get:
      summary: Get V3 Disruptions
      description: View all disruptions for all route types.
      operationId: Disruptions_GetAllDisruptions
      x-api-path-slug: v3disruptions-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: query
        name: disruption_status
        description: Filter by status of disruption
      - in: query
        name: route_types
        description: Filter by route_type; values returned via RouteTypes API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Disruptions
  /v3/disruptions/route/{route_id}:
    get:
      summary: Get V3 Disruptions Route Route
      description: View all disruptions for a particular route.
      operationId: Disruptions_GetDisruptionsByRoute
      x-api-path-slug: v3disruptionsrouteroute-id-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: query
        name: disruption_status
        description: Filter by status of disruption
      - in: path
        name: route_id
        description: Identifier of route; values returned by Routes API - v3/routes
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Disruptions
      - Route
      - Route
      - Id
  /v3/disruptions/{disruption_id}:
    get:
      summary: Get V3 Disruptions Disruption
      description: View a specific disruption.
      operationId: Disruptions_GetDisruptionById
      x-api-path-slug: v3disruptionsdisruption-id-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: disruption_id
        description: Identifier of disruption; values returned by Disruptions API
          - /v3/disruptions OR /v3/disruptions/route/{route_id}
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Disruptions
      - Disruption
      - Id
  /v3/pattern/run/{run_id}/route_type/{route_type}:
    get:
      summary: Get V3 Pattern Run Run Route Type Route Type
      description: View the stopping pattern for a specific trip/service run.
      operationId: Patterns_GetPatternByRun
      x-api-path-slug: v3patternrunrun-idroute-typeroute-type-get
      parameters:
      - in: query
        name: date_utc
        description: Filter by the date and time of the request (ISO 8601 UTC format)
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: route_type
        description: Number identifying transport mode; values returned via RouteTypes
          API
      - in: path
        name: run_id
        description: Identifier of a trip/service run; values returned by Runs API
          - /v3/route/{route_id} and Departures API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: stop_id
        description: Filter by stop_id; values returned by Stops API
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Pattern
      - Run
      - Run
      - Id
      - Route
      - Type
      - Route
      - Type
  /v3/route_types:
    get:
      summary: Get V3 Route Types
      description: View all route types and their names.
      operationId: RouteTypes_GetRouteTypes
      x-api-path-slug: v3route-types-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Route
      - Types
  /v3/routes:
    get:
      summary: Get V3 Routes
      description: View route names and numbers for all routes.
      operationId: Routes_OneOrMoreRoutes
      x-api-path-slug: v3routes-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: query
        name: route_name
        description: Filter by name  of route (accepts partial route name matches)
      - in: query
        name: route_types
        description: Filter by route_type; values returned via RouteTypes API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Routes
  /v3/routes/{route_id}:
    get:
      summary: Get V3 Routes Route
      description: View route name and number for specific route id.
      operationId: Routes_RouteFromId
      x-api-path-slug: v3routesroute-id-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: route_id
        description: Identifier of route; values returned by Departures, Directions
          and Disruptions APIs
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Routes
      - Route
      - Id
  /v3/runs/route/{route_id}:
    get:
      summary: Get V3 Runs Route Route
      description: View all trip/service runs for a specific route id.
      operationId: Runs_ForRoute
      x-api-path-slug: v3runsrouteroute-id-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: route_id
        description: Identifier of route; values returned by Routes API - v3/routes
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Route
      - Route
      - Id
  /v3/runs/route/{route_id}/route_type/{route_type}:
    get:
      summary: Get V3 Runs Route Route Route Type Route Type
      description: View all trip/service runs for a specific route id and route type.
      operationId: Runs_ForRouteAndRouteType
      x-api-path-slug: v3runsrouteroute-idroute-typeroute-type-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: route_id
        description: Identifier of route; values returned by Routes API - v3/routes
      - in: path
        name: route_type
        description: Number identifying transport mode; values returned via RouteTypes
          API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Route
      - Route
      - Id
      - Route
      - Type
      - Route
      - Type
  /v3/runs/{run_id}:
    get:
      summary: Get V3 Runs Run
      description: View all trip/service runs for a specific run id.
      operationId: Runs_ForRun
      x-api-path-slug: v3runsrun-id-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: run_id
        description: Identifier of a trip/service run; values returned by Runs API
          - /v3/route/{route_id} and Departures API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Run
      - Id
  /v3/runs/{run_id}/route_type/{route_type}:
    get:
      summary: Get V3 Runs Run Route Type Route Type
      description: View the trip/service run for a specific run id and route type.
      operationId: Runs_ForRunAndRouteType
      x-api-path-slug: v3runsrun-idroute-typeroute-type-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: route_type
        description: Number identifying transport mode; values returned via RouteTypes
          API
      - in: path
        name: run_id
        description: Identifier of a trip/service run; values returned by Runs API
          - /v3/route/{route_id} and Departures API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Run
      - Id
      - Route
      - Type
      - Route
      - Type
  /v3/search/{search_term}:
    get:
      summary: Get V3 Search Search Term
      description: View stops, routes and myki ticket outlets that match the search
        term.
      operationId: Search_Search
      x-api-path-slug: v3searchsearch-term-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: query
        name: include_addresses
        description: Placeholder for future development; currently unavailable
      - in: query
        name: include_outlets
        description: Indicates if outlets will be returned in response (default =
          true)
      - in: query
        name: latitude
        description: Filter by geographic coordinate of latitude
      - in: query
        name: longitude
        description: Filter by geographic coordinate of longitude
      - in: query
        name: max_distance
        description: Filter by maximum distance (in metres) from location specified
          via latitude and longitude parameters
      - in: query
        name: route_types
        description: 'Filter by route_type; values returned via RouteTypes API (note:
          stops and routes are ordered by route_types specified)'
      - in: path
        name: search_term
        description: 'Search text (note: if search text is numeric and/or less than
          3 characters, the API will only return routes)'
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Search
      - Search
      - Term
  /v3/stops/location/{latitude},{longitude}:
    get:
      summary: Get V3 Stops Location Latitude , Longitude
      description: View all stops near a specific location.
      operationId: Stops_StopsByGeolocation
      x-api-path-slug: v3stopslocationlatitudelongitude-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: latitude
        description: Geographic coordinate of latitude
      - in: path
        name: longitude
        description: Geographic coordinate of longitude
      - in: query
        name: max_distance
        description: Filter by maximum distance (in metres) from location specified
          via latitude and longitude parameters (default = 300)
      - in: query
        name: max_results
        description: Maximum number of results returned (default = 30)
      - in: query
        name: route_types
        description: Filter by route_type; values returned via RouteTypes API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Stops
      - Location
      - Latitude
      - Longitude
  /v3/stops/route/{route_id}/route_type/{route_type}:
    get:
      summary: Get V3 Stops Route Route Route Type Route Type
      description: View all stops on a specific route.
      operationId: Stops_StopsForRoute
      x-api-path-slug: v3stopsrouteroute-idroute-typeroute-type-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: route_id
        description: Identifier of route; values returned by Routes API - v3/routes
      - in: path
        name: route_type
        description: Number identifying transport mode; values returned via RouteTypes
          API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Stops
      - Route
      - Route
      - Id
      - Route
      - Type
      - Route
      - Type
  /v3/stops/{stop_id}/route_type/{route_type}:
    get:
      summary: Get V3 Stops Stop Route Type Route Type
      description: View facilities at a specific stop (metro and v/line stations only).
      operationId: Stops_StopDetails
      x-api-path-slug: v3stopsstop-idroute-typeroute-type-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: query
        name: gtfs
        description: Incdicates whether the stop_id is a GTFS ID or not
      - in: path
        name: route_type
        description: Number identifying transport mode; values returned via RouteTypes
          API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: stop_accessibility
        description: Indicates if stop accessibility information will be returned
          (default = false)
      - in: query
        name: stop_amenities
        description: Indicates if stop amenity information will be returned (default
          = false)
      - in: query
        name: stop_contact
        description: Placeholder for future development; currently unavailable
      - in: path
        name: stop_id
        description: Identifier of stop; values returned by Stops API
      - in: query
        name: stop_location
        description: Indicates if stop location information will be returned (default
          = false)
      - in: query
        name: stop_ticket
        description: Placeholder for future development; currently unavailable
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Stops
      - Stop
      - Id
      - Route
      - Type
      - Route
      - Type