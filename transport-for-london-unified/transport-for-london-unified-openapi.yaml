swagger: "2.0"
x-collection-name: Transport for London Unified
x-complete: 1
info:
  title: Transport for London Unified
  description: our-unified-api-brings-together-data-across-all-modes-of-transport-into-a-single-restful-api--this-api-provides-access-to-the-most-highly-requested-realtime-and-status-infomation-across-all-the-modes-of-transport-in-a-single-and-consistent-way--access-to-the-developer-documentation-is-available-at-httpsapi-tfl-gov-uk
  version: v1
host: api.tfl.gov.uk
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /AccidentStats/{year}:
    get:
      summary: Accent Stats year
      description: Gets all accident details for accidents occuring in the specified
        year.
      operationId: AccidentStats_Get
      x-api-path-slug: accidentstatsyear-get
      parameters:
      - in: path
        name: year
        description: The year for which to filter the accidents on
      responses:
        200:
          description: OK
      tags:
      - Accent
      - Stats
      - Year
  /AirQuality:
    get:
      summary: Air Quality
      description: Gets air quality data feed.
      operationId: AirQuality_Get
      x-api-path-slug: airquality-get
      responses:
        200:
          description: OK
      tags:
      - Air
      - Quality
  /BikePoint:
    get:
      summary: Bike Point
      description: "Gets all bike point locations. the place object has an addtionalproperties
        array which contains the nbbikes, nbdocks and nbspaces\r\n            numbers
        which give the status of the bikepoint. a mismatch in these numbers i.e. nbdocks
        - (nbbikes + nbspa."
      operationId: BikePoint_GetAll
      x-api-path-slug: bikepoint-get
      responses:
        200:
          description: OK
      tags:
      - Bike
      - Point
  /BikePoint/Search:
    get:
      summary: Bike Point  Search
      description: "Search for bike stations by their name, a bike point's name often
        contains information about the name of the street\r\n            or nearby
        landmarks, for example. note that the search result does not contain the placeproperties
        i.e. the status\r\n     ."
      operationId: BikePoint_Search
      x-api-path-slug: bikepointsearch-get
      parameters:
      - in: query
        name: query
        description: The search term e
      responses:
        200:
          description: OK
      tags:
      - Bike
      - Point
      - ""
      - Search
  /BikePoint/{id}:
    get:
      summary: Bike Point
      description: Gets the bike point with the given id..
      operationId: BikePoint_Get
      x-api-path-slug: bikepointid-get
      parameters:
      - in: path
        name: id
        description: A bike point id (a list of ids can be obtained from the above
          BikePoint call)
      responses:
        200:
          description: OK
      tags:
      - Bike
      - Point
  /Cabwise/search:
    get:
      summary: Cabwise search
      description: Gets taxis and minicabs contact information.
      operationId: Cabwise_Get
      x-api-path-slug: cabwisesearch-get
      parameters:
      - in: query
        name: forceXml
        description: Force Xml
      - in: query
        name: lat
        description: Latitude
      - in: query
        name: legacyFormat
        description: Legacy Format
      - in: query
        name: lon
        description: Longitude
      - in: query
        name: maxResults
        description: An optional parameter to limit the number of results return
      - in: query
        name: name
        description: Trading name of operating company
      - in: query
        name: optype
        description: Operator Type e
      - in: query
        name: radius
        description: The radius of the bounding circle in metres
      - in: query
        name: twentyFourSevenOnly
        description: Twenty Four Seven Only
      - in: query
        name: wc
        description: Wheelchair accessible
      responses:
        200:
          description: OK
      tags:
      - Cabwise
      - Search
  /Journey/JourneyResults/{from}/to/{to}:
    get:
      summary: Journey  Journey Results from to to
      description: Perform a journey planner search from the parameters specified
        in simple types.
      operationId: Journey_JourneyResults
      x-api-path-slug: journeyjourneyresultsfromtoto-get
      parameters:
      - in: query
        name: accessibilityPreference
        description: The accessibility preference must be a comma separated list eg
      - in: query
        name: adjustment
        description: Time adjustment command
      - in: query
        name: alternativeCycle
        description: Option to determine whether to return alternative cycling journey
      - in: query
        name: alternativeWalking
        description: Option to determine whether to return alternative walking journey
      - in: query
        name: applyHtmlMarkup
        description: Flag to determine whether certain text (e
      - in: query
        name: bikeProficiency
        description: A comma separated list of cycling proficiency levels
      - in: query
        name: cyclePreference
        description: The cycle preference
      - in: query
        name: date
        description: The date must be in yyyyMMdd format
      - in: path
        name: from
        description: Origin of the journey
      - in: query
        name: fromName
        description: An optional name to associate with the origin of the journey
          in the results
      - in: query
        name: journeyPreference
        description: 'The journey preference eg possible options: leastinterchange
          | leasttime | leastwalking'
      - in: query
        name: maxTransferMinutes
        description: The max walking time in minutes for transfer eg
      - in: query
        name: maxWalkingMinutes
        description: The max walking time in minutes for journeys eg
      - in: query
        name: mode
        description: The mode must be a comma separated list of modes
      - in: query
        name: nationalSearch
        description: Does the journey cover stops outside London? eg
      - in: query
        name: taxiOnlyTrip
        description: A boolean to indicate whether to return one or more taxi journeys
      - in: query
        name: time
        description: The time must be in HHmm format
      - in: query
        name: timeIs
        description: 'Does the time given relate to arrival or leaving time? Possible
          options: departing | arriving'
      - in: path
        name: to
        description: Destination of the journey
      - in: query
        name: toName
        description: An optional name to associate with the destination of the journey
          in the results
      - in: query
        name: useMultiModalCall
        description: A boolean to indicate whether or not to return 3 public transport
          journeys, a bus journey, a cycle hire journey, a personal cycle journey
          and a walking journey
      - in: query
        name: via
        description: Travel through point on the journey
      - in: query
        name: viaName
        description: An optional name to associate with the via point of the journey
          in the results
      - in: query
        name: walkingOptimization
        description: A boolean to indicate whether to optimize journeys using walking
      - in: query
        name: walkingSpeed
        description: The walking speed
      responses:
        200:
          description: OK
      tags:
      - Journey
      - ""
      - Journey
      - Results
      - From
      - To
      - To
  /Journey/Meta/Modes:
    get:
      summary: Journey  Meta  Modes
      description: Gets a list of all of the available journey planner modes.
      operationId: Journey_Meta
      x-api-path-slug: journeymetamodes-get
      responses:
        200:
          description: OK
      tags:
      - Journey
      - ""
      - Meta
      - ""
      - Modes
  /Line/Meta/DisruptionCategories:
    get:
      summary: Line  Meta  Disruption Categories
      description: Gets a list of valid disruption categories.
      operationId: Line_MetaDisruptionCategories
      x-api-path-slug: linemetadisruptioncategories-get
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Meta
      - ""
      - Disruption
      - Categories
  /Line/Meta/Modes:
    get:
      summary: Line  Meta  Modes
      description: Gets a list of valid modes.
      operationId: Line_MetaModes
      x-api-path-slug: linemetamodes-get
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Meta
      - ""
      - Modes
  /Line/Meta/ServiceTypes:
    get:
      summary: Line  Meta  Service Types
      description: Gets a list of valid servicetypes to filter on.
      operationId: Line_MetaServiceTypes
      x-api-path-slug: linemetaservicetypes-get
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Meta
      - ""
      - Service
      - Types
  /Line/Meta/Severity:
    get:
      summary: Line  Meta  Severity
      description: Gets a list of valid severity codes.
      operationId: Line_MetaSeverity
      x-api-path-slug: linemetaseverity-get
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Meta
      - ""
      - Severity
  /Line/Mode/{modes}:
    get:
      summary: Line  Mode modes
      description: Gets lines that serve the given modes..
      operationId: Line_GetByMode
      x-api-path-slug: linemodemodes-get
      parameters:
      - in: path
        name: modes
        description: A comma-separated list of modes e
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Mode
      - Modes
  /Line/Mode/{modes}/Disruption:
    get:
      summary: Line  Mode modes  Disruption
      description: Get disruptions for all lines of the given modes..
      operationId: Line_DisruptionByMode
      x-api-path-slug: linemodemodesdisruption-get
      parameters:
      - in: path
        name: modes
        description: A comma-separated list of modes e
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Mode
      - Modes
      - ""
      - Disruption
  /Line/Mode/{modes}/Route:
    get:
      summary: Line  Mode modes  Route
      description: Gets all lines and their valid routes for given modes, including
        the name and id of the originating and terminating stops for each route.
      operationId: Line_RouteByMode
      x-api-path-slug: linemodemodesroute-get
      parameters:
      - in: path
        name: modes
        description: A comma-separated list of modes e
      - in: query
        name: serviceTypes
        description: A comma seperated list of service types to filter on
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Mode
      - Modes
      - ""
      - Route
  /Line/Mode/{modes}/Status:
    get:
      summary: Line  Mode modes  Status
      description: Gets the line status of for all lines for the given modes.
      operationId: Line_StatusByMode
      x-api-path-slug: linemodemodesstatus-get
      parameters:
      - in: query
        name: detail
        description: Include details of the disruptions that are causing the line
          status including the affected stops and routes
      - in: path
        name: modes
        description: A comma-separated list of modes to filter by
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Mode
      - Modes
      - ""
      - Status
  /Line/Route:
    get:
      summary: Line  Route
      description: Get all valid routes for all lines, including the name and id of
        the originating and terminating stops for each route..
      operationId: Line_Route
      x-api-path-slug: lineroute-get
      parameters:
      - in: query
        name: serviceTypes
        description: A comma seperated list of service types to filter on
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Route
  /Line/Search/{query}:
    get:
      summary: Line  Search query
      description: Search for lines or routes matching the query string.
      operationId: Line_Search
      x-api-path-slug: linesearchquery-get
      parameters:
      - in: query
        name: modes
        description: Optionally filter by the specified modes
      - in: path
        name: query
        description: Search term e
      - in: query
        name: serviceTypes
        description: A comma seperated list of service types to filter on
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Search
      - Query
  /Line/Status/{severity}:
    get:
      summary: Line  Status severity
      description: "Gets the line status for all lines with a given severity\r\n            a
        list of valid severity codes can be obtained from a call to line/meta/severity."
      operationId: Line_StatusBySeverity
      x-api-path-slug: linestatusseverity-get
      parameters:
      - in: path
        name: severity
        description: 'The level of severity (eg: a number from 0 to 14)'
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Status
      - Severity
  /Line/{ids}:
    get:
      summary: Line s
      description: Gets lines that match the specified line ids..
      operationId: Line_Get
      x-api-path-slug: lineids-get
      parameters:
      - in: path
        name: ids
        description: A comma-separated list of line ids e
      responses:
        200:
          description: OK
      tags:
      - Line
      - S
  /Line/{ids}/Arrivals/{stopPointId}:
    get:
      summary: Line s  Arrivals stop Point Id
      description: Get the list of arrival predictions for given line ids based at
        the given stop.
      operationId: Line_Arrivals
      x-api-path-slug: lineidsarrivalsstoppointid-get
      parameters:
      - in: query
        name: destinationStationId
        description: Optional
      - in: query
        name: direction
        description: Optional
      - in: path
        name: ids
        description: A comma-separated list of line ids e
      - in: path
        name: stopPointId
        description: Optional
      responses:
        200:
          description: OK
      tags:
      - Line
      - S
      - ""
      - Arrivals
      - Stop
      - Point
      - Id
  /Line/{ids}/Disruption:
    get:
      summary: Line s  Disruption
      description: Get disruptions for the given line ids.
      operationId: Line_Disruption
      x-api-path-slug: lineidsdisruption-get
      parameters:
      - in: path
        name: ids
        description: A comma-separated list of line ids e
      responses:
        200:
          description: OK
      tags:
      - Line
      - S
      - ""
      - Disruption
  /Line/{ids}/Route:
    get:
      summary: Line s  Route
      description: Get all valid routes for given line ids, including the name and
        id of the originating and terminating stops for each route..
      operationId: Line_LineRoutesByIds
      x-api-path-slug: lineidsroute-get
      parameters:
      - in: path
        name: ids
        description: A comma-separated list of line ids e
      - in: query
        name: serviceTypes
        description: A comma seperated list of service types to filter on
      responses:
        200:
          description: OK
      tags:
      - Line
      - S
      - ""
      - Route
  /Line/{ids}/Status:
    get:
      summary: Line s  Status
      description: Gets the line status of for given line ids e.g minor delays.
      operationId: Line_StatusByIds
      x-api-path-slug: lineidsstatus-get
      parameters:
      - in: query
        name: detail
        description: Include details of the disruptions that are causing the line
          status including the affected stops and routes
      - in: path
        name: ids
        description: A comma-separated list of line ids e
      responses:
        200:
          description: OK
      tags:
      - Line
      - S
      - ""
      - Status
  /Line/{ids}/Status/{StartDate}/to/{EndDate}:
    get:
      summary: Line s  Status  Start Date to  End Date
      description: Gets the line status for given line ids during the provided dates
        e.g minor delays.
      operationId: Line_Status
      x-api-path-slug: lineidsstatusstartdatetoenddate-get
      parameters:
      - in: query
        name: dateRange.endDate
      - in: query
        name: dateRange.startDate
      - in: query
        name: detail
        description: Include details of the disruptions that are causing the line
          status including the affected stops and routes
      - in: query
        name: endDate
      - in: path
        name: EndDate
      - in: path
        name: ids
        description: A comma-separated list of line ids e
      - in: query
        name: startDate
      - in: path
        name: StartDate
      responses:
        200:
          description: OK
      tags:
      - Line
      - S
      - ""
      - Status
      - ""
      - Start
      - Date
      - To
      - ""
      - End
      - Date
  /Line/{id}/Route/Sequence/{direction}:
    get:
      summary: Line  Route  Sequence direction
      description: Gets all valid routes for given line id, including the sequence
        of stops on each route..
      operationId: Line_RouteSequence
      x-api-path-slug: lineidroutesequencedirection-get
      parameters:
      - in: path
        name: direction
        description: The direction of travel
      - in: query
        name: excludeCrowding
        description: That excludes crowding from line disruptions
      - in: path
        name: id
        description: A single line id e
      - in: query
        name: serviceTypes
        description: A comma seperated list of service types to filter on
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Route
      - ""
      - Sequence
      - Direction
  /Line/{id}/StopPoints:
    get:
      summary: Line  Stop Points
      description: Gets a list of the stations that serve the given line id.
      operationId: Line_StopPoints
      x-api-path-slug: lineidstoppoints-get
      parameters:
      - in: path
        name: id
        description: A single line id e
      - in: query
        name: tflOperatedNationalRailStationsOnly
        description: If the national-rail line is requested, this flag will filter
          the national rail stations so that only those operated by TfL are returned
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Stop
      - Points
  /Line/{id}/Timetable/{fromStopPointId}:
    get:
      summary: Line  Timetable from Stop Point Id
      description: Gets the timetable for a specified station on the give line.
      operationId: Line_Timetable
      x-api-path-slug: lineidtimetablefromstoppointid-get
      parameters:
      - in: path
        name: fromStopPointId
        description: The originating stations stop point id (station naptan code e
      - in: path
        name: id
        description: A single line id e
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Timetable
      - From
      - Stop
      - Point
      - Id
  /Line/{id}/Timetable/{fromStopPointId}/to/{toStopPointId}:
    get:
      summary: Line  Timetable from Stop Point Id to to Stop Point Id
      description: Gets the timetable for a specified station on the give line with
        specified destination.
      operationId: Line_TimetableTo
      x-api-path-slug: lineidtimetablefromstoppointidtotostoppointid-get
      parameters:
      - in: path
        name: fromStopPointId
        description: The originating stations stop point id (station naptan code e
      - in: path
        name: id
        description: A single line id e
      - in: path
        name: toStopPointId
        description: The destination stationss Naptan code
      responses:
        200:
          description: OK
      tags:
      - Line
      - ""
      - Timetable
      - From
      - Stop
      - Point
      - Id
      - To
      - To
      - Stop
      - Point
      - Id
  /Mode/ActiveServiceTypes:
    get:
      summary: Mode  Active Service Types
      description: "Returns the service type active for a mode.\r\n            currently
        only supports tube."
      operationId: Mode_GetActiveServiceTypes
      x-api-path-slug: modeactiveservicetypes-get
      responses:
        200:
          description: OK
      tags:
      - Mode
      - ""
      - Active
      - Service
      - Types
  /Mode/{mode}/Arrivals:
    get:
      summary: Mode mode  Arrivals
      description: Gets the next arrival predictions for all stops of a given mode.
      operationId: Mode_Arrivals
      x-api-path-slug: modemodearrivals-get
      parameters:
      - in: query
        name: count
        description: A number of arrivals to return for each stop, -1 to return all
          available
      - in: path
        name: mode
        description: A mode name e
      responses:
        200:
          description: OK
      tags:
      - Mode
      - Mode
      - ""
      - Arrivals
  /Occupancy/BikePoints/{ids}:
    get:
      summary: Occupancy  Bike Points s
      description: Get the occupancy for bike points..
      operationId: Occupancy_GetBikePointsOccupancies
      x-api-path-slug: occupancybikepointsids-get
      parameters:
      - in: path
        name: ids
      responses:
        200:
          description: OK
      tags:
      - Occupancy
      - ""
      - Bike
      - Points
      - S
  /Occupancy/CarPark:
    get:
      summary: Occupancy  Car Park
      description: Gets the occupancy for all car parks that have occupancy data.
      operationId: Occupancy.CarPark.get
      x-api-path-slug: occupancycarpark-get
      responses:
        200:
          description: OK
      tags:
      - Occupancy
      - ""
      - Car
      - Park
  /Occupancy/CarPark/{id}:
    get:
      summary: Occupancy  Car Park
      description: Gets the occupancy for a car park with a given id.
      operationId: Occupancy.CarPark.id.get
      x-api-path-slug: occupancycarparkid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Occupancy
      - ""
      - Car
      - Park
  /Occupancy/ChargeConnector:
    get:
      summary: Occupancy  Charge Connector
      description: Gets the occupancy for all charge connectors.
      operationId: Occupancy_GetAllChargeConnectorStatus
      x-api-path-slug: occupancychargeconnector-get
      responses:
        200:
          description: OK
      tags:
      - Occupancy
      - ""
      - Charge
      - Connector
  /Occupancy/ChargeConnector/{ids}:
    get:
      summary: Occupancy  Charge Connector s
      description: Gets the occupancy for a charge connectors with a given id (sourcesystemplaceid).
      operationId: Occupancy_GetChargeConnectorStatus
      x-api-path-slug: occupancychargeconnectorids-get
      parameters:
      - in: path
        name: ids
      responses:
        200:
          description: OK
      tags:
      - Occupancy
      - ""
      - Charge
      - Connector
      - S
  /Place:
    get:
      summary: Place
      description: "Gets the places that lie within the bounding box defined by the
        lat/lon of its north-west and south-east corners. optionally filters\r\n            on
        type and can strip properties for a smaller payload.."
      operationId: Place_GetByGeoBox
      x-api-path-slug: place-get
      parameters:
      - in: query
        name: activeOnly
        description: An optional parameter to limit the results to active records
          only (Currently only the VariableMessageSign place type is supported)
      - in: query
        name: bbBoxpoints.neLat
      - in: query
        name: bbBoxpoints.neLon
      - in: query
        name: bbBoxpoints.swLat
      - in: query
        name: bbBoxpoints.swLon
      - in: query
        name: categories
        description: an optional list of comma separated property categories to return
          in the Places property bag
      - in: query
        name: includeChildren
        description: Defaults to false
      - in: query
        name: type
        description: place types to filter on, or null to return all types
      responses:
        200:
          description: OK
      tags:
      - Place
  /Place/Address/Streets/{Postcode}:
    get:
      summary: Place  Address  Streets  Postcode
      description: Gets the set of streets associated with a post code..
      operationId: Place_GetStreetsByPostCode
      x-api-path-slug: placeaddressstreetspostcode-get
      parameters:
      - in: query
        name: postcode
      - in: path
        name: Postcode
      - in: query
        name: postcodeInput.postcode
      responses:
        200:
          description: OK
      tags:
      - Place
      - ""
      - Ress
      - ""
      - Streets
      - ""
      - Code
  /Place/Meta/Categories:
    get:
      summary: Place  Meta  Categories
      description: Gets a list of all of the available place property categories and
        keys..
      operationId: Place_MetaCategories
      x-api-path-slug: placemetacategories-get
      responses:
        200:
          description: OK
      tags:
      - Place
      - ""
      - Meta
      - ""
      - Categories
  /Place/Meta/PlaceTypes:
    get:
      summary: Place  Meta  Place Types
      description: Gets a list of the available types of place..
      operationId: Place_MetaPlaceTypes
      x-api-path-slug: placemetaplacetypes-get
      responses:
        200:
          description: OK
      tags:
      - Place
      - ""
      - Meta
      - ""
      - Place
      - Types
  /Place/Search:
    get:
      summary: Place  Search
      description: Gets all places that matches the given query.
      operationId: Place_Search
      x-api-path-slug: placesearch-get
      parameters:
      - in: query
        name: name
        description: The name of the place, you can use the /Place/Types/{types} endpoint
          to get a list of places for a given type including their names
      - in: query
        name: types
        description: A comma-separated list of the types to return
      responses:
        200:
          description: OK
      tags:
      - Place
      - ""
      - Search
  /Place/Type/{types}:
    get:
      summary: Place  Type types
      description: Gets all places of a given type.
      operationId: Place_GetByType
      x-api-path-slug: placetypetypes-get
      parameters:
      - in: query
        name: activeOnly
        description: An optional parameter to limit the results to active records
          only (Currently only the VariableMessageSign place type is supported)
      - in: path
        name: types
        description: A comma-separated list of the types to return
      responses:
        200:
          description: OK
      tags:
      - Place
      - ""
      - Type
      - Types
  /Place/{id}:
    get:
      summary: Place
      description: Gets the place with the given id..
      operationId: Place_Get
      x-api-path-slug: placeid-get
      parameters:
      - in: path
        name: id
        description: The id of the place, you can use the /Place/Types/{types} endpoint
          to get a list of places for a given type including their ids
      - in: query
        name: includeChildren
        description: Defaults to false
      responses:
        200:
          description: OK
      tags:
      - Place
  /Place/{type}/At/{Lat}/{Lon}:
    get:
      summary: Place type  At  Lat  Lon
      description: "Gets any places of the given type whose geography intersects the
        given latitude and longitude. in practice this means the place\r\n            must
        be polygonal e.g. a boroughboundary.."
      operationId: Place_GetAt
      x-api-path-slug: placetypeatlatlon-get
      parameters:
      - in: query
        name: lat
      - in: path
        name: Lat
      - in: query
        name: location.lat
      - in: query
        name: location.lon
      - in: query
        name: lon
      - in: path
        name: Lon
      - in: path
        name: type
        description: The place type (a valid list of place types can be obtained from
          the /Place/Meta/placeTypes endpoint)
      responses:
        200:
          description: OK
      tags:
      - Place
      - Type
      - ""
      - At
      - ""
      - Lat
      - ""
      - Lon
  /Place/{type}/overlay/{z}/{Lat}/{Lon}/{width}/{height}:
    get:
      summary: Place type overlay z  Lat  Lon wth height
      description: Gets the place overlay for a given set of co-ordinates and a given
        width/height..
      operationId: Place_GetOverlay
      x-api-path-slug: placetypeoverlayzlatlonwidthheight-get
      parameters:
      - in: path
        name: height
        description: The height of the requested overlay
      - in: query
        name: lat
      - in: path
        name: Lat
      - in: query
        name: location.lat
      - in: query
        name: location.lon
      - in: query
        name: lon
      - in: path
        name: Lon
      - in: path
        name: type
        description: The place type (a valid list of place types can be obtained from
          the /Place/Meta/placeTypes endpoint)
      - in: path
        name: width
        description: The width of the requested overlay
      - in: path
        name: z
        description: The zoom level
      responses:
        200:
          description: OK
      tags:
      - Place
      - Type
      - Overlay
      - Z
      - ""
      - Lat
      - ""
      - Lon
      - Wth
      - Height
  /Road:
    get:
      summary: Road
      description: Gets all roads managed by tfl.
      operationId: Road.get
      x-api-path-slug: road-get
      responses:
        200:
          description: OK
      tags:
      - Road
  /Road/Meta/Categories:
    get:
      summary: Road  Meta  Categories
      description: Gets a list of valid roaddisruption categories.
      operationId: Road_MetaCategories
      x-api-path-slug: roadmetacategories-get
      responses:
        200:
          description: OK
      tags:
      - Road
      - ""
      - Meta
      - ""
      - Categories
  /Road/Meta/Severities:
    get:
      summary: Road  Meta  Severities
      description: Gets a list of valid roaddisruption severity codes.
      operationId: Road_MetaSeverities
      x-api-path-slug: roadmetaseverities-get
      responses:
        200:
          description: OK
      tags:
      - Road
      - ""
      - Meta
      - ""
      - Severities
  /Road/all/Disruption/{disruptionIds}:
    get:
      summary: Road all  Disruption disruption Ids
      description: Gets a list of active disruptions filtered by disruption ids..
      operationId: Road_DisruptionById
      x-api-path-slug: roadalldisruptiondisruptionids-get
      parameters:
      - in: path
        name: disruptionIds
        description: Comma-separated list of disruption identifiers to filter by
      - in: query
        name: stripContent
        description: Optional, defaults to false
      responses:
        200:
          description: OK
      tags:
      - Road
      - ""
      - ""
      - Disruption
      - Disruption
      - Ids
  /Road/all/Street/Disruption:
    get:
      summary: Road all  Street  Disruption
      description: Gets a list of disrupted streets. if no date filters are provided,
        current disruptions are returned..
      operationId: Road_DisruptedStreets
      x-api-path-slug: roadallstreetdisruption-get
      parameters:
      - in: query
        name: endDate
        description: Optional, The end time to filter on
      - in: query
        name: startDate
        description: Optional, the start time to filter on
      responses:
        200:
          description: OK
      tags:
      - Road
      - ""
      - ""
      - Street
      - ""
      - Disruption
  /Road/{ids}:
    get:
      summary: Road s
      description: Gets the road with the specified id (e.g. a1).
      operationId: Road.ids.get
      x-api-path-slug: roadids-get
      parameters:
      - in: path
        name: ids
        description: Comma-separated list of road identifiers e
      responses:
        200:
          description: OK
      tags:
      - Road
      - S
  /Road/{ids}/Disruption:
    get:
      summary: Road s  Disruption
      description: Get active disruptions, filtered by road ids.
      operationId: Road_Disruption
      x-api-path-slug: roadidsdisruption-get
      parameters:
      - in: query
        name: categories
        description: an optional list of category names to filter on (a valid list
          of categories can be obtained from the /Road/Meta/categories endpoint)
      - in: query
        name: closures
        description: Optional, defaults to true
      - in: path
        name: ids
        description: Comma-separated list of road identifiers e
      - in: query
        name: severities
        description: an optional list of Severity names to filter on (a valid list
          of severities can be obtained from the /Road/Meta/severities endpoint)
      - in: query
        name: stripContent
        description: Optional, defaults to false
      responses:
        200:
          description: OK
      tags:
      - Road
      - S
      - ""
      - Disruption
  /Road/{ids}/Status:
    get:
      summary: Road s  Status
      description: Gets the specified roads with the status aggregated over the date
        range specified, or now until the end of today if no dates are passed..
      operationId: Road_Status
      x-api-path-slug: roadidsstatus-get
      parameters:
      - in: query
        name: dateRangeNullable.endDate
      - in: query
        name: dateRangeNullable.startDate
      - in: path
        name: ids
        description: Comma-separated list of road identifiers e
      responses:
        200:
          description: OK
      tags:
      - Road
      - S
      - ""
      - Status
  /Search:
    get:
      summary: Search
      description: "Search the site for occurrences of the query string. the maximum
        number of results returned is equal to the maximum page size\r\n            of
        100. to return subsequent pages, use the paginated overload.."
      operationId: Search_Get
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: query
        description: The search query
      responses:
        200:
          description: OK
      tags:
      - Search
  /Search/BusSchedules:
    get:
      summary: Search  Bus Schedules
      description: Searches the bus schedules folder on s3 for a given bus number..
      operationId: Search_BusSchedules
      x-api-path-slug: searchbusschedules-get
      parameters:
      - in: query
        name: query
        description: The search query
      responses:
        200:
          description: OK
      tags:
      - Search
      - ""
      - Bus
      - Schedules
  /Search/Meta/Categories:
    get:
      summary: Search  Meta  Categories
      description: Gets the available search categories..
      operationId: Search_MetaCategories
      x-api-path-slug: searchmetacategories-get
      responses:
        200:
          description: OK
      tags:
      - Search
      - ""
      - Meta
      - ""
      - Categories
  /Search/Meta/SearchProviders:
    get:
      summary: Search  Meta  Search Provers
      description: Gets the available searchprovider names..
      operationId: Search_MetaSearchProviders
      x-api-path-slug: searchmetasearchproviders-get
      responses:
        200:
          description: OK
      tags:
      - Search
      - ""
      - Meta
      - ""
      - Search
      - Provers
  /Search/Meta/Sorts:
    get:
      summary: Search  Meta  Sorts
      description: Gets the available sorting options..
      operationId: Search_MetaSorts
      x-api-path-slug: searchmetasorts-get
      responses:
        200:
          description: OK
      tags:
      - Search
      - ""
      - Meta
      - ""
      - Sorts
  /StopPoint:
    get:
      summary: Stop Point
      description: Gets a list of stoppoints within {radius} by the specified criteria.
      operationId: StopPoint_GetByGeoPoint
      x-api-path-slug: stoppoint-get
      parameters:
      - in: query
        name: categories
        description: an optional list of comma separated property categories to return
          in the StopPoints property bag
      - in: query
        name: location.lat
      - in: query
        name: location.lon
      - in: query
        name: modes
        description: the list of modes to search (comma separated mode names e
      - in: query
        name: radius
        description: 'the radius of the bounding circle in metres (default : 200)'
      - in: query
        name: returnLines
        description: true to return the lines that each stop point serves as a nested
          resource
      - in: query
        name: stopTypes
        description: a list of stopTypes that should be returned (a list of valid
          stop types can be obtained from the StopPoint/meta/stoptypes endpoint)
      - in: query
        name: useStopPointHierarchy
        description: Re-arrange the output into a parent/child hierarchy
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
  /StopPoint/Meta/Categories:
    get:
      summary: Stop Point  Meta  Categories
      description: Gets the list of available stoppoint additional information categories.
      operationId: StopPoint_MetaCategories
      x-api-path-slug: stoppointmetacategories-get
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Meta
      - ""
      - Categories
  /StopPoint/Meta/Modes:
    get:
      summary: Stop Point  Meta  Modes
      description: Gets the list of available stoppoint modes.
      operationId: StopPoint_MetaModes
      x-api-path-slug: stoppointmetamodes-get
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Meta
      - ""
      - Modes
  /StopPoint/Meta/StopTypes:
    get:
      summary: Stop Point  Meta  Stop Types
      description: Gets the list of available stoppoint types.
      operationId: StopPoint_MetaStopTypes
      x-api-path-slug: stoppointmetastoptypes-get
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Meta
      - ""
      - Stop
      - Types
  /StopPoint/Mode/{modes}:
    get:
      summary: Stop Point  Mode modes
      description: Gets a list of stoppoints filtered by the modes available at that
        stoppoint..
      operationId: StopPoint_GetByMode
      x-api-path-slug: stoppointmodemodes-get
      parameters:
      - in: path
        name: modes
        description: A comma-seperated list of modes e
      - in: query
        name: page
        description: The data set page to return
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Mode
      - Modes
  /StopPoint/Mode/{modes}/Disruption:
    get:
      summary: Stop Point  Mode modes  Disruption
      description: Gets a distinct list of disrupted stop points for the given modes.
      operationId: StopPoint_DisruptionByMode
      x-api-path-slug: stoppointmodemodesdisruption-get
      parameters:
      - in: query
        name: includeRouteBlockedStops
      - in: path
        name: modes
        description: A comma-seperated list of modes e
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Mode
      - Modes
      - ""
      - Disruption
  /StopPoint/Search:
    get:
      summary: Stop Point  Search
      description: Search stoppoints by their common name, or their 5-digit countdown
        bus stop code..
      operationId: StopPoint.Search.get
      x-api-path-slug: stoppointsearch-get
      parameters:
      - in: query
        name: faresOnly
        description: True to only return stations in that have Fares data available
          for single fares to another station
      - in: query
        name: includeHubs
        description: If true, returns results including HUBs
      - in: query
        name: lines
        description: An optional, parameter separated list of the lines to filter
          by
      - in: query
        name: maxResults
        description: An optional result limit, defaulting to and with a maximum of
          50
      - in: query
        name: modes
        description: An optional, parameter separated list of the modes to filter
          by
      - in: query
        name: query
        description: The query string, case-insensitive
      - in: query
        name: tflOperatedNationalRailStationsOnly
        description: If the national-rail mode is included, this flag will filter
          the national rail stations so that only those operated by TfL are returned
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Search
  /StopPoint/Search/{query}:
    get:
      summary: Stop Point  Search query
      description: Search stoppoints by their common name, or their 5-digit countdown
        bus stop code..
      operationId: StopPoint.Search.query.get
      x-api-path-slug: stoppointsearchquery-get
      parameters:
      - in: query
        name: faresOnly
        description: True to only return stations in that have Fares data available
          for single fares to another station
      - in: query
        name: includeHubs
        description: If true, returns results including HUBs
      - in: query
        name: lines
        description: An optional, parameter separated list of the lines to filter
          by
      - in: query
        name: maxResults
        description: An optional result limit, defaulting to and with a maximum of
          50
      - in: query
        name: modes
        description: An optional, parameter separated list of the modes to filter
          by
      - in: path
        name: query
        description: The query string, case-insensitive
      - in: query
        name: tflOperatedNationalRailStationsOnly
        description: If the national-rail mode is included, this flag will filter
          the national rail stations so that only those operated by TfL are returned
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Search
      - Query
  /StopPoint/ServiceTypes:
    get:
      summary: Stop Point  Service Types
      description: Gets the service types for a given stoppoint.
      operationId: StopPoint_GetServiceTypes
      x-api-path-slug: stoppointservicetypes-get
      parameters:
      - in: query
        name: id
        description: The Naptan id of the stop
      - in: query
        name: lineIds
        description: The lines which contain the given Naptan id (all lines relevant
          to the given stoppoint if empty)
      - in: query
        name: modes
        description: The modes which the lines are relevant to (all if empty)
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Service
      - Types
  /StopPoint/Sms/{id}:
    get:
      summary: Stop Point  Sms
      description: Gets a stoppoint for a given sms code..
      operationId: StopPoint_GetBySms
      x-api-path-slug: stoppointsmsid-get
      parameters:
      - in: path
        name: id
        description: A 5-digit Countdown Bus Stop Code e
      - in: query
        name: output
        description: If set to web, a 302 redirect to relevant website bus stop page
          is returned
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Sms
  /StopPoint/Type/{types}:
    get:
      summary: Stop Point  Type types
      description: Gets all stop points of a given type.
      operationId: StopPoint_GetByType
      x-api-path-slug: stoppointtypetypes-get
      parameters:
      - in: path
        name: types
        description: A comma-separated list of the types to return
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Type
      - Types
  /StopPoint/{ids}:
    get:
      summary: Stop Point s
      description: Gets a list of stoppoints corresponding to the given list of stop
        ids..
      operationId: StopPoint.ids.get
      x-api-path-slug: stoppointids-get
      parameters:
      - in: path
        name: ids
        description: A comma-separated list of stop point ids (station naptan code
          e
      - in: query
        name: includeCrowdingData
        description: Include the crowding data (static)
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - S
  /StopPoint/{ids}/Disruption:
    get:
      summary: Stop Point s  Disruption
      description: Gets all disruptions for the specified stoppointid, plus disruptions
        for any child naptan records it may have..
      operationId: StopPoint_Disruption
      x-api-path-slug: stoppointidsdisruption-get
      parameters:
      - in: query
        name: flattenResponse
        description: Specify true to associate all disruptions with parent stop point
      - in: query
        name: getFamily
        description: Specify true to return disruptions for entire family, or false
          to return disruptions for just this stop point
      - in: path
        name: ids
        description: A comma-seperated list of stop point ids
      - in: query
        name: includeRouteBlockedStops
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - S
      - ""
      - Disruption
  /StopPoint/{id}/Arrivals:
    get:
      summary: Stop Point  Arrivals
      description: Gets the list of arrival predictions for the given stop point id.
      operationId: StopPoint_Arrivals
      x-api-path-slug: stoppointidarrivals-get
      parameters:
      - in: path
        name: id
        description: A StopPoint id (station naptan code e
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Arrivals
  /StopPoint/{id}/CanReachOnLine/{lineId}:
    get:
      summary: Stop Point  Can Reach On Line line Id
      description: Gets stopoints that are reachable from a station/line combination..
      operationId: StopPoint_ReachableFrom
      x-api-path-slug: stoppointidcanreachonlinelineid-get
      parameters:
      - in: path
        name: id
        description: The id (station naptan code e
      - in: path
        name: lineId
        description: Line id of the line to filter by (e
      - in: query
        name: serviceTypes
        description: A comma-separated list of service types to filter on
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Can
      - Reach
      - "On"
      - Line
      - Line
      - Id
  /StopPoint/{id}/Crowding/{line}:
    get:
      summary: Stop Point  Crowding line
      description: Gets all the crowding data (static) for the stoppointid, plus crowding
        data for a given line and optionally a particular direction..
      operationId: StopPoint_Crowding
      x-api-path-slug: stoppointidcrowdingline-get
      parameters:
      - in: query
        name: direction
        description: The direction of travel
      - in: path
        name: id
        description: The Naptan id of the stop
      - in: path
        name: line
        description: A particular line e
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Crowding
      - Line
  /StopPoint/{id}/DirectionTo/{toStopPointId}:
    get:
      summary: Stop Point  Direction To to Stop Point Id
      description: Returns the canonical direction, "inbound" or "outbound", for a
        given pair of stop point ids in the direction from -&gt; to..
      operationId: StopPoint_Direction
      x-api-path-slug: stoppointiddirectiontotostoppointid-get
      parameters:
      - in: path
        name: id
        description: Originating stop id (station naptan code e
      - in: query
        name: lineId
        description: Optional line id filter e
      - in: path
        name: toStopPointId
        description: Destination stop id (station naptan code e
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Direction
      - To
      - Stop
      - Point
      - Id
  /StopPoint/{id}/Route:
    get:
      summary: Stop Point  Route
      description: Returns the route sections for all the lines that service the given
        stop point ids.
      operationId: StopPoint_Route
      x-api-path-slug: stoppointidroute-get
      parameters:
      - in: path
        name: id
        description: A stop point id (station naptan codes e
      - in: query
        name: serviceTypes
        description: A comma-separated list of service types to filter on
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - ""
      - Route
  /StopPoint/{id}/placeTypes:
    get:
      summary: Stop Point place Types
      description: Get a list of places corresponding to a given id and place types..
      operationId: StopPoint.id.placeTypes.get
      x-api-path-slug: stoppointidplacetypes-get
      parameters:
      - in: path
        name: id
        description: A naptan id for a stop point (station naptan code e
      - in: query
        name: placeTypes
        description: A comcomma-separated value representing the place types
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - Place
      - Types
  /StopPoint/{stopPointId}/CarParks:
    get:
      summary: Stop Point stop Point Id  Car Parks
      description: Get car parks corresponding to the given stop point id..
      operationId: StopPoint_GetCarParksById
      x-api-path-slug: stoppointstoppointidcarparks-get
      parameters:
      - in: path
        name: stopPointId
        description: stopPointId is required to get the car parks
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - Stop
      - Point
      - Id
      - ""
      - Car
      - Parks
  /StopPoint/{stopPointId}/TaxiRanks:
    get:
      summary: Stop Point stop Point Id  Taxi Ranks
      description: Gets a list of taxi ranks corresponding to the given stop point
        id..
      operationId: StopPoint_GetTaxiRanksByIds
      x-api-path-slug: stoppointstoppointidtaxiranks-get
      parameters:
      - in: path
        name: stopPointId
        description: stopPointId is required to get the taxi ranks
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Point
      - Stop
      - Point
      - Id
      - ""
      - Taxi
      - Ranks
  ? /TravelTimes/compareOverlay/{z}/mapcenter/{mapCenterLat}/{mapCenterLon}/pinlocation/{pinLat}/{pinLon}/dimensions/{width}/{height}
  : get:
      summary: Travel Times compare Overlay z mapcenter map Center Lat map Center
        Lon pinlocation pin Lat pin Lon dimensions wth height
      description: Gets the traveltime overlay..
      operationId: TravelTime_GetCompareOverlay
      x-api-path-slug: traveltimescompareoverlayzmapcentermapcenterlatmapcenterlonpinlocationpinlatpinlondimensionswidthheight-get
      parameters:
      - in: query
        name: compareType
      - in: query
        name: compareValue
      - in: query
        name: direction
        description: The direction of travel
      - in: path
        name: height
        description: The height of the requested overlay
      - in: path
        name: mapCenterLat
        description: The map center latitude
      - in: path
        name: mapCenterLon
        description: The map center longitude
      - in: query
        name: modeId
        description: The id of the mode
      - in: path
        name: pinLat
        description: The latitude of the pin
      - in: path
        name: pinLon
        description: The longitude of the pin
      - in: query
        name: scenarioTitle
        description: The title of the scenario
      - in: query
        name: timeOfDayId
        description: The id for the time of day (AM/INTER/PM)
      - in: query
        name: travelTimeInterval
        description: The total minutes between the travel time bands
      - in: path
        name: width
        description: The width of the requested overlay
      - in: path
        name: z
        description: The zoom level
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Times
      - Compare
      - Overlay
      - Z
      - Mapcenter
      - Map
      - Center
      - Lat
      - Map
      - Center
      - Lon
      - Pinlocation
      - Pin
      - Lat
      - Pin
      - Lon
      - Dimensions
      - Wth
      - Height
  /TravelTimes/overlay/{z}/mapcenter/{mapCenterLat}/{mapCenterLon}/pinlocation/{pinLat}/{pinLon}/dimensions/{width}/{height}:
    get:
      summary: Travel Times overlay z mapcenter map Center Lat map Center Lon pinlocation
        pin Lat pin Lon dimensions wth height
      description: Gets the traveltime overlay..
      operationId: TravelTime_GetOverlay
      x-api-path-slug: traveltimesoverlayzmapcentermapcenterlatmapcenterlonpinlocationpinlatpinlondimensionswidthheight-get
      parameters:
      - in: query
        name: direction
        description: The direction of travel
      - in: path
        name: height
        description: The height of the requested overlay
      - in: path
        name: mapCenterLat
        description: The map center latitude
      - in: path
        name: mapCenterLon
        description: The map center longitude
      - in: query
        name: modeId
        description: The id of the mode
      - in: path
        name: pinLat
        description: The latitude of the pin
      - in: path
        name: pinLon
        description: The longitude of the pin
      - in: query
        name: scenarioTitle
        description: The title of the scenario
      - in: query
        name: timeOfDayId
        description: The id for the time of day (AM/INTER/PM)
      - in: query
        name: travelTimeInterval
        description: The total minutes between the travel time bands
      - in: path
        name: width
        description: The width of the requested overlay
      - in: path
        name: z
        description: The zoom level
      responses:
        200:
          description: OK
      tags:
      - Travel
      - Times
      - Overlay
      - Z
      - Mapcenter
      - Map
      - Center
      - Lat
      - Map
      - Center
      - Lon
      - Pinlocation
      - Pin
      - Lat
      - Pin
      - Lon
      - Dimensions
      - Wth
      - Height
  /Vehicle/EmissionSurcharge:
    get:
      summary: Vehicle  Emission Surcharge
      description: Gets the emissions surcharge compliance for the vehicle.
      operationId: Vehicle_GetEmissionsSurchargeCompliance
      x-api-path-slug: vehicleemissionsurcharge-get
      parameters:
      - in: query
        name: vrm
        description: The Vehicle Registration Mark
      responses:
        200:
          description: OK
      tags:
      - Vehicle
      - ""
      - Emission
      - Surcharge
  /Vehicle/UlezCompliance:
    get:
      summary: Vehicle  Ulez Compliance
      description: Gets the ulez surcharge compliance for the vehicle.
      operationId: Vehicle_GetUlezCompliance
      x-api-path-slug: vehicleulezcompliance-get
      parameters:
      - in: query
        name: vrm
        description: The Vehicle Registration Mark
      responses:
        200:
          description: OK
      tags:
      - Vehicle
      - ""
      - Ulez
      - Compliance
  /Vehicle/{ids}/Arrivals:
    get:
      summary: Vehicle s  Arrivals
      description: Gets the predictions for a given list of vehicle id's..
      operationId: Vehicle_Get
      x-api-path-slug: vehicleidsarrivals-get
      parameters:
      - in: path
        name: ids
        description: A comma-separated list of vehicle ids e
      responses:
        200:
          description: OK
      tags:
      - Vehicle
      - S
      - ""
      - Arrivals
  /Line/{ids}/Arrivals:
    get:
      summary: Line s  Arrivals
      description: Get the list of arrival predictions for given line ids based at
        the given stop.
      operationId: ""
      x-api-path-slug: lineidsarrivals-get
      parameters:
      - in: path
        name: ids
        description: A comma-separated list of line ids e
      - in: query
        name: stopPointId
        description: Id of stop to get arrival predictions for (station naptan code
          e
      responses:
        200:
          description: OK
      tags:
      - Line
      - S
      - ""
      - Arrivals