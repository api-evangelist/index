swagger: "2.0"
x-collection-name: Washington Metropolitan Area Transit Authority
x-complete: 1
info:
  title: Train Positions
  description: realtime-train-positions-and-support-methods-
  version: 1.0.0
host: api.wmata.com
basePath: /TrainPositions
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /TrainPositions:
    get:
      summary: Live Train Positions
      description: |-
        Description

        Returns uniquely identifiable trains in service and what track circuits they currently occupy. Will return an empty set of results when no positions are available.

        Data is refreshed once every 7-10 seconds.
        Please refer to this page for additional details.

        Response Elements




        Element

        Description





        TrainPositions


        Array containing train position information (TrainPosition).






        TrainPosition Elements





        CarCount

        Number of cars.  Can sometimes be 0 when there is no data available.



        CircuitId

        The circuit identifier the train is currently on.  This identifier can be referenced from the Standard Routes method.



        DestinationStationCode

        Destination station code. Can be NULL. Use this value in other rail-related APIs to retrieve data about a station.  Note that this value may sometimes differ from the destination station code returned by our Next Trains methods.



        DirectionNum

        The direction of movement regardless of which track the train is on.  Valid values are 1 or 2.  Generally speaking, trains with direction 1 are northbound/eastbound, while trains with direction 2 are southbound/westbound.



        LineCode

        Two-letter abbreviation for the line (e.g.: RD, BL, YL, OR, GR, or SV). May also be NULL in certain cases.



        SecondsAtLocation

        Approximate "dwell time".  This is not an exact value, but can be used to determine how long a train has been reported at the same track circuit.



        ServiceType

        Service Type of a train, can be any of the following Service Types



        TrainId

        Uniquely identifiable internal train identifier.





        Service Types





        NoPassengers

        This is a non-revenue train with no passengers on board.  Note that this designation of NoPassengers does not necessarily correlate with PIDS "No Passengers".  As of 08/22/2016, this functionality has been reinstated to include all non-revenue vehicles, with minor exceptions.



        Normal

        This is a normal revenue service train.



        Special

        This is a special revenue service train with an unspecified line and destination.  This is more prevalent during scheduled track work.



        Unknown

        This often denotes cases with unknown data or work vehicles.
      operationId: getTrainpositions
      x-api-path-slug: trainpositions-get
      parameters:
      - in: query
        name: contentType
        description: Returns response in the specified format
      responses:
        200:
          description: OK
      tags:
      - Transit
      - Subway
      - Positions
  /StandardRoutes:
    get:
      summary: Standard Routes
      description: "Description\r\n\r\nReturns an ordered list of mostly revenue (and
        some lead) track circuits, arranged by line and track number.  This data does
        not change frequently and should be cached for a reasonable amount of time.\r\nPlease
        refer to this page for additional details.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nStandardRoutes\r\n\r\n\r\nArray
        containing revenue line information (StandardRoute).\r\n\r\n\r\n\r\n\r\n\r\n\r\nStandardRoute
        Elements\r\n\r\n\r\n\r\n\r\n\r\nLineCode\r\n\r\nAbbreviation for the revenue
        line.  Note that this also includes YLRP (Yellow Line Rush Plus).\r\n\r\n\r\n\r\nTrackCircuits\r\n\r\n\r\nArray
        containing ordered track circuit information (TrackCircuit).\r\n\r\n\r\n\r\n\r\nTrackNum\r\n\r\nTrack
        number (1 or 2).\r\n\r\n\r\n\r\n\r\n\r\nTrackCircuit Elements\r\n\r\n\r\n
        \       \r\n\r\n\r\nCircuitId\r\n\r\nAn internal system-wide uniquely identifiable
        circuit number.\r\n\r\n\r\n\r\nSeqNum\r\n\r\nOrder in which the circuit appears
        for the given line and track.  Sequences go from West to East and South to
        North.\r\n        \r\n\r\n\r\nStationCode\r\n\r\nIf the circuit is at a station,
        this value will represent the station code.  Otherwise, it will be be NULL.
        Use this value in other rail-related APIs to retrieve data about a station."
      operationId: getStandardroutes
      x-api-path-slug: standardroutes-get
      parameters:
      - in: query
        name: contentType
        description: Returns response in the specified format
      responses:
        200:
          description: OK
      tags:
      - Transit
      - Subway
      - Routes
  /TrackCircuits:
    get:
      summary: Track Circuits
      description: "Description\r\n\r\nReturns a list of all track circuits including
        those on pocket tracks and crossovers.  Each track circuit may include references
        to its right and left neighbors.\r\nPlease refer to this page for additional
        details.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nTrackCircuits\r\n\r\n\r\nArray
        containing track circuit information (TrackCircuit).\r\n\r\n\r\n\r\n\r\n\r\n\r\nTrackCircuit
        Elements\r\n\r\n\r\n\r\n\r\n\r\nCircuitId\r\n\r\nAn internal system-wide uniquely
        identifiable circuit number.\r\n\r\n\r\n\r\nNeighbors\r\n\r\n\r\nArray containing
        track circuit neighbor information (TrackCircuitNeighbor).  Note that some
        track circuits have no neighbors in one direction.  All track circuits have
        at least one neighbor.\r\n\r\n\r\n\r\n\r\nTrack\r\n\r\nTrack number.  1 and
        2 denote \"main\" lines, while 0 and 3 are connectors (between different types
        of tracks) and pocket tracks, respectively.\r\n\r\n\r\n\r\n\r\n\r\nTrackCircuitNeighbor
        Elements\r\n\r\n\r\n\r\n\r\n\r\nCircuitIds\r\n\r\n\r\nArray containing neighboring
        circuit ids.\r\n\r\n\r\n\r\n\r\nNeighborType\r\n\r\nLeft or Right neighbor
        group.  Generally speaking, left neighbors are to the west and south, while
        right neighbors are to the east/north.\r\n\r\n\r\n\r\n\r\nNeighbor Notes\r\n\r\nGiven
        the hypothetical example below, note that CircuitId 8 has two right neighbors
        - 4 and 3.  Similarly, CircuitId 6 has two left neighbors - 5 and 7.\r\n\r\n\r\n\r\n\r\n\r\nbackground\r\n\r\n\r\n\r\nLayer
        1\r\nTrack 2\r\n\r\n8\r\n\r\n4\r\nTrack 1\r\n\r\nCircuitId 1\r\n\r\n2\r\n\r\nCircuitId
        4\r\n\r\n9\r\n\r\n\r\n100\r\n\r\n3\r\n\r\nTrack 0\r\nTrack 0\r\nTrack 3\r\n7\r\n5\r\n\r\n6\r\n\r\n\r\n\r\nThe
        JSON representation of the image above would be as follows:\r\n\r\n\r\n{\r\n\"TrackCircuits\":
        [{\r\n\"Track\": 2,\r\n\"CircuitId\": 8,\r\n\"Neighbors\": [{\r\n\"NeighborType\":
        \"Right\",\r\n\"CircuitIds\": [4, 3]\r\n}]\r\n}, {\r\n\"Track\": 2,\r\n\"CircuitId\":
        4,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\":
        [8]\r\n}, {\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [9]\r\n}]\r\n},
        {\r\n\"Track\": 2,\r\n\"CircuitId\": 9,\r\n\"Neighbors\": [{\r\n\"NeighborType\":
        \"Left\",\r\n\"CircuitIds\": [4]\r\n}]\r\n}, {\r\n\"Track\": 0,\r\n\"CircuitId\":
        3,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\":
        [8]\r\n}, {\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [100]\r\n}]\r\n},
        {\r\n\"Track\": 3,\r\n\"CircuitId\": 100,\r\n\"Neighbors\": [{\r\n\"NeighborType\":
        \"Left\",\r\n\"CircuitIds\": [3]\r\n}, {\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\":
        [7]\r\n}]\r\n}, {\r\n\"Track\": 0,\r\n\"CircuitId\": 7,\r\n\"Neighbors\":
        [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [100]\r\n}, {\r\n\"NeighborType\":
        \"Right\",\r\n\"CircuitIds\": [6]\r\n}]\r\n}, {\r\n\"Track\": 1,\r\n\"CircuitId\":
        1,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\":
        [2]\r\n}]\r\n}, {\r\n\"Track\": 1,\r\n\"CircuitId\": 2,\r\n\"Neighbors\":
        [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [1]\r\n}, {\r\n\"NeighborType\":
        \"Right\",\r\n\"CircuitIds\": [5]\r\n}]\r\n}, {\r\n\"Track\": 1,\r\n\"CircuitId\":
        5,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\":
        [2]\r\n}, {\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [6]\r\n}]\r\n},
        {\r\n\"Track\": 1,\r\n\"CircuitId\": 6,\r\n\"Neighbors\": [{\r\n\"NeighborType\":
        \"Left\",\r\n\"CircuitIds\": [5, 7]\r\n}]\r\n}]\r\n}"
      operationId: getTrackcircuits
      x-api-path-slug: trackcircuits-get
      parameters:
      - in: query
        name: contentType
        description: Returns response in the specified format
      responses:
        200:
          description: OK
      tags:
      - Transit
      - Subway
      - Tracks
      - Circuits