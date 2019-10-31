{
  "info": {
    "name": "WMATA Real-Time Rail Predictions XML - Next Trains",
    "_postman_id": "62657ba6-95a2-458c-8bb6-5fa55692a90d",
    "description": "Description\r\n\r\nReturns next train arrival information for one or more stations. Will return\r\nan empty set of results when no predictions are available. Use All for the StationCodes parameter to return predictions for\r\nall stations.\r\n\r\nFor terminal stations (e.g.: Greenbelt, Shady Grove, etc.), predictions may\r\nbe displayed twice.\r\n\r\nSome stations have two platforms (e.g.: Gallery Place, Fort Totten, L'Enfant\r\nPlaza, and Metro Center). To retrieve complete predictions for these stations,\r\nbe sure to pass in both StationCodes.\r\n\r\nFor trains with no passengers, the DestinationName will be No Passenger.\r\n\r\nNext train arrival information is refreshed once every 20 to 30 seconds approximately.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nTrains\r\n\r\n\r\nArray containing train prediction information (AIMPredictionTrainInfo).\r\n\r\n\r\n\r\n\r\n\r\n\r\nAIMPredictionTrainInfo\r\nElements\r\n\r\n\r\n\r\n\r\n\r\nCar\r\n\r\nNumber of cars on a train, usually 6 or 8, but might also\r\nreturn - or NULL.\r\n\r\n\r\n\r\nDestination\r\n\r\nAbbreviated version of the final destination for a train. This\r\nis similar to what is displayed on the signs at stations.\r\n\r\n\r\n\r\nDestinationCode\r\n\r\nDestination station code. Can be NULL. Use this value in other\r\nrail-related APIs to retrieve data about a station.\r\n\r\n\r\n\r\nDestinationName\r\n\r\nWhen DestinationCode is populated, this is the full name of the\r\ndestination station, as shown on the WMATA website.\r\n\r\n\r\n\r\nGroup\r\n\r\nDenotes the track this train is on, but does not necessarily\r\nequate to Track 1 or Track 2. With the exception of terminal\r\nstations, predictions at the same station with different Group\r\nvalues refer to trains on different tracks.\r\n\r\n\r\n\r\nLine\r\n\r\nTwo-letter abbreviation for the line (e.g.: RD, BL, YL, OR, GR,\r\nor SV). May also be blank or No for\r\ntrains with no passengers.\r\n\r\n\r\n\r\nLocationCode\r\n\r\nStation code for where the train is arriving. Useful when\r\npassing in All as the StationCodes\r\nparameter. Use this value in other rail-related APIs to retrieve\r\ndata about a station.\r\n\r\n\r\n\r\nLocationName\r\n\r\nFull name of the station where the train is arriving. Useful\r\nwhen passing in All as the\r\nStationCodes parameter.\r\n\r\n\r\n\r\nMin\r\n\r\nMinutes until arrival. Can be a numeric value, ARR (arriving), BRD (boarding), ---, or empty.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Transit",
      "item": [
        {
          "id": "fa289bdb-3ec5-4541-a481-84859ebe0d82",
          "name": "getJsonGetpredictionStationcodes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wmata.com",
              "path": [
                "StationPrediction.svc",
                "json/GetPrediction/:StationCodes"
              ],
              "variable": [
                {
                  "id": "StationCodes",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Description\r\n\r\nReturns next train arrival information for one or more stations. Will return\r\nan empty set of results when no predictions are available. Use All for the StationCodes parameter to return predictions for\r\nall stations.\r\n\r\nFor terminal stations (e.g.: Greenbelt, Shady Grove, etc.), predictions may\r\nbe displayed twice.\r\n\r\nSome stations have two platforms (e.g.: Gallery Place, Fort Totten, L'Enfant\r\nPlaza, and Metro Center). To retrieve complete predictions for these stations,\r\nbe sure to pass in both StationCodes.\r\n\r\nFor trains with no passengers, the DestinationName will be No Passenger.\r\n\r\nNext train arrival information is refreshed once every 20 to 30 seconds approximately.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nTrains\r\n\r\n\r\nArray containing train prediction information (AIMPredictionTrainInfo).\r\n\r\n\r\n\r\n\r\n\r\n\r\nAIMPredictionTrainInfo\r\nElements\r\n\r\n\r\n\r\n\r\n\r\nCar\r\n\r\nNumber of cars on a train, usually 6 or 8, but might also\r\nreturn - or NULL.\r\n\r\n\r\n\r\nDestination\r\n\r\nAbbreviated version of the final destination for a train. This\r\nis similar to what is displayed on the signs at stations.\r\n\r\n\r\n\r\nDestinationCode\r\n\r\nDestination station code. Can be NULL. Use this value in other\r\nrail-related APIs to retrieve data about a station.\r\n\r\n\r\n\r\nDestinationName\r\n\r\nWhen DestinationCode is populated, this is the full name of the\r\ndestination station, as shown on the WMATA website.\r\n\r\n\r\n\r\nGroup\r\n\r\nDenotes the track this train is on, but does not necessarily\r\nequate to Track 1 or Track 2. With the exception of terminal\r\nstations, predictions at the same station with different Group\r\nvalues refer to trains on different tracks.\r\n\r\n\r\n\r\nLine\r\n\r\nTwo-letter abbreviation for the line (e.g.: RD, BL, YL, OR, GR,\r\nor SV). May also be blank or No for\r\ntrains with no passengers.\r\n\r\n\r\n\r\nLocationCode\r\n\r\nStation code for where the train is arriving. Useful when\r\npassing in All as the StationCodes\r\nparameter. Use this value in other rail-related APIs to retrieve\r\ndata about a station.\r\n\r\n\r\n\r\nLocationName\r\n\r\nFull name of the station where the train is arriving. Useful\r\nwhen passing in All as the\r\nStationCodes parameter.\r\n\r\n\r\n\r\nMin\r\n\r\nMinutes until arrival. Can be a numeric value, ARR (arriving), BRD (boarding), ---, or empty."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1355365-e268-4ecd-8037-60d88e0b8cfb"
            }
          ]
        },
        {
          "id": "de926f03-edf2-4931-aba0-a89a39bf4679",
          "name": "getGetpredictionStationcodes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wmata.com",
              "path": [
                "StationPrediction.svc",
                "GetPrediction/:StationCodes"
              ],
              "variable": [
                {
                  "id": "StationCodes",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Description\r\n\r\nReturns next train arrival information for one or more stations. Will return\r\nan empty set of results when no predictions are available. Use All for the StationCodes parameter to return predictions for\r\nall stations.\r\n\r\nFor terminal stations (e.g.: Greenbelt, Shady Grove, etc.), predictions may\r\nbe displayed twice.\r\n\r\nSome stations have two platforms (e.g.: Gallery Place, Fort Totten, L'Enfant\r\nPlaza, and Metro Center). To retrieve complete predictions for these stations,\r\nbe sure to pass in both StationCodes.\r\n\r\nFor trains with no passengers, the DestinationName will be No Passenger.\r\n\r\nNext train arrival information is refreshed once every 20 to 30 seconds approximately.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nTrains\r\n\r\n\r\nArray containing train prediction information (AIMPredictionTrainInfo).\r\n\r\n\r\n\r\n\r\n\r\n\r\nAIMPredictionTrainInfo\r\nElements\r\n\r\n\r\n\r\n\r\n\r\nCar\r\n\r\nNumber of cars on a train, usually 6 or 8, but might also\r\nreturn - or NULL.\r\n\r\n\r\n\r\nDestination\r\n\r\nAbbreviated version of the final destination for a train. This\r\nis similar to what is displayed on the signs at stations.\r\n\r\n\r\n\r\nDestinationCode\r\n\r\nDestination station code. Can be NULL. Use this value in other\r\nrail-related APIs to retrieve data about a station.\r\n\r\n\r\n\r\nDestinationName\r\n\r\nWhen DestinationCode is populated, this is the full name of the\r\ndestination station, as shown on the WMATA website.\r\n\r\n\r\n\r\nGroup\r\n\r\nDenotes the track this train is on, but does not necessarily\r\nequate to Track 1 or Track 2. With the exception of terminal\r\nstations, predictions at the same station with different Group\r\nvalues refer to trains on different tracks.\r\n\r\n\r\n\r\nLine\r\n\r\nTwo-letter abbreviation for the line (e.g.: RD, BL, YL, OR, GR,\r\nor SV). May also be blank or No for\r\ntrains with no passengers.\r\n\r\n\r\n\r\nLocationCode\r\n\r\nStation code for where the train is arriving. Useful when\r\npassing in All as the StationCodes\r\nparameter. Use this value in other rail-related APIs to retrieve\r\ndata about a station.\r\n\r\n\r\n\r\nLocationName\r\n\r\nFull name of the station where the train is arriving. Useful\r\nwhen passing in All as the\r\nStationCodes parameter.\r\n\r\n\r\n\r\nMin\r\n\r\nMinutes until arrival. Can be a numeric value, ARR (arriving), BRD (boarding), ---, or empty."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b65339ef-9993-418f-82a8-e4e01629893b"
            }
          ]
        }
      ]
    }
  ]
}