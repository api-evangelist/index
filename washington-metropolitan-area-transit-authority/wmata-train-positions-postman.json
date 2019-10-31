{
  "info": {
    "name": "WMATA Train Positions Track Circuits",
    "_postman_id": "184a6377-7011-4096-bfa7-1025fc5cea6a",
    "description": "Description\r\n\r\nReturns a list of all track circuits including those on pocket tracks and crossovers.  Each track circuit may include references to its right and left neighbors.\r\nPlease refer to this page for additional details.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nTrackCircuits\r\n\r\n\r\nArray containing track circuit information (TrackCircuit).\r\n\r\n\r\n\r\n\r\n\r\n\r\nTrackCircuit Elements\r\n\r\n\r\n\r\n\r\n\r\nCircuitId\r\n\r\nAn internal system-wide uniquely identifiable circuit number.\r\n\r\n\r\n\r\nNeighbors\r\n\r\n\r\nArray containing track circuit neighbor information (TrackCircuitNeighbor).  Note that some track circuits have no neighbors in one direction.  All track circuits have at least one neighbor.\r\n\r\n\r\n\r\n\r\nTrack\r\n\r\nTrack number.  1 and 2 denote \"main\" lines, while 0 and 3 are connectors (between different types of tracks) and pocket tracks, respectively.\r\n\r\n\r\n\r\n\r\n\r\nTrackCircuitNeighbor Elements\r\n\r\n\r\n\r\n\r\n\r\nCircuitIds\r\n\r\n\r\nArray containing neighboring circuit ids.\r\n\r\n\r\n\r\n\r\nNeighborType\r\n\r\nLeft or Right neighbor group.  Generally speaking, left neighbors are to the west and south, while right neighbors are to the east/north.\r\n\r\n\r\n\r\n\r\nNeighbor Notes\r\n\r\nGiven the hypothetical example below, note that CircuitId 8 has two right neighbors - 4 and 3.  Similarly, CircuitId 6 has two left neighbors - 5 and 7.\r\n\r\n\r\n\r\n\r\n\r\nbackground\r\n\r\n\r\n\r\nLayer 1\r\nTrack 2\r\n\r\n8\r\n\r\n4\r\nTrack 1\r\n\r\nCircuitId 1\r\n\r\n2\r\n\r\nCircuitId 4\r\n\r\n9\r\n\r\n\r\n100\r\n\r\n3\r\n\r\nTrack 0\r\nTrack 0\r\nTrack 3\r\n7\r\n5\r\n\r\n6\r\n\r\n\r\n\r\nThe JSON representation of the image above would be as follows:\r\n\r\n\r\n{\r\n\"TrackCircuits\": [{\r\n\"Track\": 2,\r\n\"CircuitId\": 8,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [4, 3]\r\n}]\r\n}, {\r\n\"Track\": 2,\r\n\"CircuitId\": 4,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [8]\r\n}, {\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [9]\r\n}]\r\n}, {\r\n\"Track\": 2,\r\n\"CircuitId\": 9,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [4]\r\n}]\r\n}, {\r\n\"Track\": 0,\r\n\"CircuitId\": 3,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [8]\r\n}, {\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [100]\r\n}]\r\n}, {\r\n\"Track\": 3,\r\n\"CircuitId\": 100,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [3]\r\n}, {\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [7]\r\n}]\r\n}, {\r\n\"Track\": 0,\r\n\"CircuitId\": 7,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [100]\r\n}, {\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [6]\r\n}]\r\n}, {\r\n\"Track\": 1,\r\n\"CircuitId\": 1,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [2]\r\n}]\r\n}, {\r\n\"Track\": 1,\r\n\"CircuitId\": 2,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [1]\r\n}, {\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [5]\r\n}]\r\n}, {\r\n\"Track\": 1,\r\n\"CircuitId\": 5,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [2]\r\n}, {\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [6]\r\n}]\r\n}, {\r\n\"Track\": 1,\r\n\"CircuitId\": 6,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [5, 7]\r\n}]\r\n}]\r\n}",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Transit",
      "item": [
        {
          "id": "6d507512-327c-4c54-8883-535f02c093eb",
          "name": "getTrainpositions",
          "request": {
            "url": "http://api.wmata.com/TrainPositions/TrainPositions?contentType=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Description\n\nReturns uniquely identifiable trains in service and what track circuits they currently occupy. Will return an empty set of results when no positions are available.\n\nData is refreshed once every 7-10 seconds.\nPlease refer to this page for additional details.\n\nResponse Elements\n\n\n\n\nElement\n\nDescription\n\n\n\n\n\nTrainPositions\n\n\nArray containing train position information (TrainPosition).\n\n\n\n\n\n\nTrainPosition Elements\n\n\n\n\n\nCarCount\n\nNumber of cars.  Can sometimes be 0 when there is no data available.\n\n\n\nCircuitId\n\nThe circuit identifier the train is currently on.  This identifier can be referenced from the Standard Routes method.\n\n\n\nDestinationStationCode\n\nDestination station code. Can be NULL. Use this value in other rail-related APIs to retrieve data about a station.  Note that this value may sometimes differ from the destination station code returned by our Next Trains methods.\n\n\n\nDirectionNum\n\nThe direction of movement regardless of which track the train is on.  Valid values are 1 or 2.  Generally speaking, trains with direction 1 are northbound/eastbound, while trains with direction 2 are southbound/westbound.\n\n\n\nLineCode\n\nTwo-letter abbreviation for the line (e.g.: RD, BL, YL, OR, GR, or SV). May also be NULL in certain cases.\n\n\n\nSecondsAtLocation\n\nApproximate \"dwell time\".  This is not an exact value, but can be used to determine how long a train has been reported at the same track circuit.\n\n\n\nServiceType\n\nService Type of a train, can be any of the following Service Types\n\n\n\nTrainId\n\nUniquely identifiable internal train identifier.\n\n\n\n\n\nService Types\n\n\n\n\n\nNoPassengers\n\nThis is a non-revenue train with no passengers on board.  Note that this designation of NoPassengers does not necessarily correlate with PIDS \"No Passengers\".  As of 08/22/2016, this functionality has been reinstated to include all non-revenue vehicles, with minor exceptions.\n\n\n\nNormal\n\nThis is a normal revenue service train.\n\n\n\nSpecial\n\nThis is a special revenue service train with an unspecified line and destination.  This is more prevalent during scheduled track work.\n\n\n\nUnknown\n\nThis often denotes cases with unknown data or work vehicles."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ecdaabc-a2c7-43fb-a0e3-63d740d324ac"
            }
          ]
        },
        {
          "id": "ff9a858a-3ca7-476a-afbb-4bc6b5380475",
          "name": "getStandardroutes",
          "request": {
            "url": "http://api.wmata.com/TrainPositions/StandardRoutes?contentType=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Description\r\n\r\nReturns an ordered list of mostly revenue (and some lead) track circuits, arranged by line and track number.  This data does not change frequently and should be cached for a reasonable amount of time.\r\nPlease refer to this page for additional details.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nStandardRoutes\r\n\r\n\r\nArray containing revenue line information (StandardRoute).\r\n\r\n\r\n\r\n\r\n\r\n\r\nStandardRoute Elements\r\n\r\n\r\n\r\n\r\n\r\nLineCode\r\n\r\nAbbreviation for the revenue line.  Note that this also includes YLRP (Yellow Line Rush Plus).\r\n\r\n\r\n\r\nTrackCircuits\r\n\r\n\r\nArray containing ordered track circuit information (TrackCircuit).\r\n\r\n\r\n\r\n\r\nTrackNum\r\n\r\nTrack number (1 or 2).\r\n\r\n\r\n\r\n\r\n\r\nTrackCircuit Elements\r\n\r\n\r\n        \r\n\r\n\r\nCircuitId\r\n\r\nAn internal system-wide uniquely identifiable circuit number.\r\n\r\n\r\n\r\nSeqNum\r\n\r\nOrder in which the circuit appears for the given line and track.  Sequences go from West to East and South to North.\r\n        \r\n\r\n\r\nStationCode\r\n\r\nIf the circuit is at a station, this value will represent the station code.  Otherwise, it will be be NULL. Use this value in other rail-related APIs to retrieve data about a station."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07616e14-a3f0-4a97-a460-62e40e4ca4f2"
            }
          ]
        },
        {
          "id": "fa9f8da4-4111-40cb-b0f3-e19715b6bdc0",
          "name": "getTrackcircuits",
          "request": {
            "url": "http://api.wmata.com/TrainPositions/TrackCircuits?contentType=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Description\r\n\r\nReturns a list of all track circuits including those on pocket tracks and crossovers.  Each track circuit may include references to its right and left neighbors.\r\nPlease refer to this page for additional details.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nTrackCircuits\r\n\r\n\r\nArray containing track circuit information (TrackCircuit).\r\n\r\n\r\n\r\n\r\n\r\n\r\nTrackCircuit Elements\r\n\r\n\r\n\r\n\r\n\r\nCircuitId\r\n\r\nAn internal system-wide uniquely identifiable circuit number.\r\n\r\n\r\n\r\nNeighbors\r\n\r\n\r\nArray containing track circuit neighbor information (TrackCircuitNeighbor).  Note that some track circuits have no neighbors in one direction.  All track circuits have at least one neighbor.\r\n\r\n\r\n\r\n\r\nTrack\r\n\r\nTrack number.  1 and 2 denote \"main\" lines, while 0 and 3 are connectors (between different types of tracks) and pocket tracks, respectively.\r\n\r\n\r\n\r\n\r\n\r\nTrackCircuitNeighbor Elements\r\n\r\n\r\n\r\n\r\n\r\nCircuitIds\r\n\r\n\r\nArray containing neighboring circuit ids.\r\n\r\n\r\n\r\n\r\nNeighborType\r\n\r\nLeft or Right neighbor group.  Generally speaking, left neighbors are to the west and south, while right neighbors are to the east/north.\r\n\r\n\r\n\r\n\r\nNeighbor Notes\r\n\r\nGiven the hypothetical example below, note that CircuitId 8 has two right neighbors - 4 and 3.  Similarly, CircuitId 6 has two left neighbors - 5 and 7.\r\n\r\n\r\n\r\n\r\n\r\nbackground\r\n\r\n\r\n\r\nLayer 1\r\nTrack 2\r\n\r\n8\r\n\r\n4\r\nTrack 1\r\n\r\nCircuitId 1\r\n\r\n2\r\n\r\nCircuitId 4\r\n\r\n9\r\n\r\n\r\n100\r\n\r\n3\r\n\r\nTrack 0\r\nTrack 0\r\nTrack 3\r\n7\r\n5\r\n\r\n6\r\n\r\n\r\n\r\nThe JSON representation of the image above would be as follows:\r\n\r\n\r\n{\r\n\"TrackCircuits\": [{\r\n\"Track\": 2,\r\n\"CircuitId\": 8,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [4, 3]\r\n}]\r\n}, {\r\n\"Track\": 2,\r\n\"CircuitId\": 4,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [8]\r\n}, {\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [9]\r\n}]\r\n}, {\r\n\"Track\": 2,\r\n\"CircuitId\": 9,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [4]\r\n}]\r\n}, {\r\n\"Track\": 0,\r\n\"CircuitId\": 3,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [8]\r\n}, {\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [100]\r\n}]\r\n}, {\r\n\"Track\": 3,\r\n\"CircuitId\": 100,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [3]\r\n}, {\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [7]\r\n}]\r\n}, {\r\n\"Track\": 0,\r\n\"CircuitId\": 7,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [100]\r\n}, {\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [6]\r\n}]\r\n}, {\r\n\"Track\": 1,\r\n\"CircuitId\": 1,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [2]\r\n}]\r\n}, {\r\n\"Track\": 1,\r\n\"CircuitId\": 2,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [1]\r\n}, {\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [5]\r\n}]\r\n}, {\r\n\"Track\": 1,\r\n\"CircuitId\": 5,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [2]\r\n}, {\r\n\"NeighborType\": \"Right\",\r\n\"CircuitIds\": [6]\r\n}]\r\n}, {\r\n\"Track\": 1,\r\n\"CircuitId\": 6,\r\n\"Neighbors\": [{\r\n\"NeighborType\": \"Left\",\r\n\"CircuitIds\": [5, 7]\r\n}]\r\n}]\r\n}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6d9f8f1-afda-4a0f-a756-9fe1a1a62bdb"
            }
          ]
        }
      ]
    }
  ]
}