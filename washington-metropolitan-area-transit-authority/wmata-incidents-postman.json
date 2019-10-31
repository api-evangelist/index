{
  "info": {
    "name": "WMATA Incidents XML - Rail Incidents",
    "_postman_id": "5a1d5d5d-2975-4a3e-8bf8-7b60ba06edb3",
    "description": "Description\r\n\r\nReturns reported rail incidents (significant disruptions and delays to\r\nnormal service). The data is identical to WMATA's Metrorail Service Status\r\nfeed.\r\n\r\nRail incidents are refreshed once every 20 to 30 seconds approximately.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nIncidents\r\n\r\n\r\nArray containing rail disruption information (Incident).\r\n\r\n\r\n\r\n\r\n\r\n\r\nIncident Elements\r\n\r\n\r\n\r\n\r\n\r\nDateUpdated\r\n\r\nDate and time (Eastern Standard Time) of last update. Will be\r\nin YYYY-MM-DDTHH:mm:SS format (e.g.: 2010-07-29T14:21:28).\r\n\r\n\r\n\r\nDelaySeverity\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nDescription\r\n\r\nFree-text description of the incident.\r\n\r\n\r\n\r\nEmergencyText\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nEndLocationFullName\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nIncidentID\r\n\r\nUnique identifier for an incident.\r\n\r\n\r\n\r\nIncidentType\r\n\r\nFree-text description of the incident type. Usually Delay or\r\nAlert but is subject to change at any time.\r\n\r\n\r\n\r\nLinesAffected\r\n\r\nSemi-colon and space separated list of line codes (e.g.:\r\nRD; or BL;\r\nOR; or BL; OR; RD;). We do\r\nplan to update this to return something more reasonable like an\r\narray, but until then, use code similar to the following:\r\n\r\n\"RD; GR; BL;\".split(/;[\\s]?/).filter(function(fn) { return fn\r\n!== ''; })\r\n\r\n\r\n\r\nPassengerDelay\r\n\r\nDeprecated.\r\n\r\n\r\n\r\n\r\nStartLocationFullName\r\n\r\nDeprecated.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Transit",
      "item": [
        {
          "id": "ef5dde73-9b1f-4d24-b02d-edcc1db64d30",
          "name": "54763641281d830c946a3d75",
          "request": {
            "url": "http://api.wmata.com/Incidents.svc/json/BusIncidents?Route=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Description\r\n\r\nReturns a set of reported bus incidents/delays for a given Route. Omit the\r\nRoute to return all reported items.\r\n\r\nNote that the Route parameter accepts only base route names and no\r\nvariations, i.e.: use 10A instead of 10Av1 and 10Av2.\r\n\r\nBus incidents/delays are refreshed once every 20 to 30 seconds approximately.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nBusIncidents\r\n\r\n\r\nArray containing bus incident information (BusIncident).\r\n\r\n\r\n\r\n\r\n\r\n\r\nBusIncident\r\nElements\r\n\r\n\r\n\r\n\r\n\r\nDateUpdated\r\n\r\nDate and time (Eastern Standard Time) of last update. Will be\r\nin YYYY-MM-DDTHH:mm:ss format (e.g.: 2014-10-28T08:13:03).\r\n\r\n\r\n\r\nDescription\r\n\r\nFree-text description of the delay or incident.\r\n\r\n\r\n\r\nIncidentID\r\n\r\nUnique identifier for an incident.\r\n\r\n\r\n\r\nIncidentType\r\n\r\nFree-text description of the incident type. Usually\r\nDelay or Alert but is subject to change at any time.\r\n\r\n\r\n\r\nRoutesAffected\r\n\r\nArray containing routes affected. Routes listed are usually\r\nidentical to base route names (i.e.: not 10Av1 or 10Av2, but 10A),\r\nbut may differ from what our bus methods return."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0ae3e7b-901c-427f-ab78-8f7ec65e95e1"
            }
          ]
        },
        {
          "id": "a365bc57-d28d-4362-9fb1-f3617c896510",
          "name": "54763641281d830c946a3d76",
          "request": {
            "url": "http://api.wmata.com/Incidents.svc/json/ElevatorIncidents?StationCode=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Description\r\n\r\nReturns a list of reported elevator and escalator outages at a\r\ngiven station. Omit the StationCode parameter to return all reported\r\noutages.\r\n\r\nNote that for stations with multiple platforms and therefore StationCodes\r\n(e.g.: Metro Center, L'Enfant Plaza, etc.), a distinct call is required for\r\neach StationCode.\r\n\r\nElevator and escalator outages are refreshed once every 20 to 30 seconds approximately.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nElevatorIncidents\r\n\r\n\r\nArray containing elevator/escalator outage information\r\n(ElevatorIncident).\r\n\r\n\r\n\r\n\r\n\r\n\r\nElevatorIncident Elements\r\n\r\n\r\n\r\n\r\n\r\nDateOutOfServ\r\n\r\nDate and time (Eastern Standard Time) unit was reported out of\r\nservice. Will be in YYYY-MM-DDTHH:mm:ss format (e.g.:\r\n2014-10-27T15:17:00).\r\n\r\n\r\n\r\nDateUpdated\r\n\r\nDate and time (Eastern Standard Time) outage details was last\r\nupdated. Will be in YYYY-MM-DDTHH:mm:ss format (e.g.:\r\n2014-10-27T15:17:00).\r\n\r\n\r\n\r\nDisplayOrder\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nLocationDescription\r\n\r\nFree-text description of the unit location within a station\r\n(e.g.: Escalator between mezzanine and\r\nplatform).\r\n\r\n\r\n\r\nStationCode\r\n\r\nUnit's station code. Use this value in other rail-related APIs\r\nto retrieve data about a station.\r\n\r\n\r\n\r\nStationName\r\n\r\nFull station name, may include entrance information (e.g.:\r\nMetro Center, G and 11th St\r\nEntrance).\r\n\r\n\r\n\r\nSymptomCode\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nSymptomDescription\r\n\r\nDescription for why the unit is out of service or otherwise in\r\nreduced operation.\r\n\r\n\r\n\r\nTimeOutOfService\r\n\r\nDeprecated. Use the time\r\nportion of the DateOutOfServ element.\r\n\r\n\r\n\r\nUnitName\r\n\r\nUnique identifier for unit, by type (a single elevator and\r\nescalator may have the same UnitName, but no two elevators or two\r\nescalators will have the same UnitName).\r\n\r\n\r\n\r\nUnitStatus\r\n\r\nDeprecated. If listed here,\r\nthe unit is inoperational or otherwise impaired.\r\n\r\n\r\n\r\nUnitType\r\n\r\nType of unit. Will be ELEVATOR\r\nor ESCALATOR."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3db0025-e157-4d15-9826-1802b6f4c4d1"
            }
          ]
        },
        {
          "id": "4acfce30-7005-4805-9e62-12b234adccdb",
          "name": "54763641281d830c946a3d77",
          "request": {
            "url": "http://api.wmata.com/Incidents.svc/json/Incidents",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Description\r\n\r\nReturns reported rail incidents (significant disruptions and delays to\r\nnormal service). The data is identical to WMATA's Metrorail Service Status\r\nfeed.\r\n\r\nRail incidents are refreshed once every 20 to 30 seconds approximately.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nIncidents\r\n\r\n\r\nArray containing rail disruption information (Incident).\r\n\r\n\r\n\r\n\r\n\r\n\r\nIncident Elements\r\n\r\n\r\n\r\n\r\n\r\nDateUpdated\r\n\r\nDate and time (Eastern Standard Time) of last update. Will be\r\nin YYYY-MM-DDTHH:mm:SS format (e.g.: 2010-07-29T14:21:28).\r\n\r\n\r\n\r\nDelaySeverity\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nDescription\r\n\r\nFree-text description of the incident.\r\n\r\n\r\n\r\nEmergencyText\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nEndLocationFullName\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nIncidentID\r\n\r\nUnique identifier for an incident.\r\n\r\n\r\n\r\nIncidentType\r\n\r\nFree-text description of the incident type. Usually Delay or\r\nAlert but is subject to change at any time.\r\n\r\n\r\n\r\nLinesAffected\r\n\r\nSemi-colon and space separated list of line codes (e.g.:\r\nRD; or BL;\r\nOR; or BL; OR; RD;). We do\r\nplan to update this to return something more reasonable like an\r\narray, but until then, use code similar to the following:\r\n\r\n\"RD; GR; BL;\".split(/;[\\s]?/).filter(function(fn) { return fn\r\n!== ''; })\r\n\r\n\r\n\r\nPassengerDelay\r\n\r\nDeprecated.\r\n\r\n\r\n\r\n\r\nStartLocationFullName\r\n\r\nDeprecated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bda9d33c-9d53-4256-a88e-28b1c916e82b"
            }
          ]
        },
        {
          "id": "dd0d0587-ac85-461f-87c7-9eb7483fc01f",
          "name": "54763641281d830c946a3d78",
          "request": {
            "url": "http://api.wmata.com/Incidents.svc/BusIncidents?Route=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Description\r\n\r\nReturns a set of reported bus incidents/delays for a given Route. Omit the\r\nRoute to return all reported items.\r\n\r\nNote that the Route parameter accepts only base route names and no\r\nvariations, i.e.: use 10A instead of 10Av1 and 10Av2.\r\n\r\nBus incidents/delays are refreshed once every 20 to 30 seconds approximately.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nBusIncidents\r\n\r\n\r\nArray containing bus incident information (BusIncident).\r\n\r\n\r\n\r\n\r\n\r\n\r\nBusIncident\r\nElements\r\n\r\n\r\n\r\n\r\n\r\nDateUpdated\r\n\r\nDate and time (Eastern Standard Time) of last update. Will be\r\nin YYYY-MM-DDTHH:mm:ss format (e.g.: 2014-10-28T08:13:03).\r\n\r\n\r\n\r\nDescription\r\n\r\nFree-text description of the delay or incident.\r\n\r\n\r\n\r\nIncidentID\r\n\r\nUnique identifier for an incident.\r\n\r\n\r\n\r\nIncidentType\r\n\r\nFree-text description of the incident type. Usually\r\nDelay or Alert but is subject to change at any time.\r\n\r\n\r\n\r\nRoutesAffected\r\n\r\nArray containing routes affected. Routes listed are usually\r\nidentical to base route names (i.e.: not 10Av1 or 10Av2, but 10A),\r\nbut may differ from what our bus methods return."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea657979-a758-49df-97ad-31986aa6d496"
            }
          ]
        },
        {
          "id": "857313a8-1be8-4a6a-b811-00ba88a9f26b",
          "name": "54763641281d830c946a3d79",
          "request": {
            "url": "http://api.wmata.com/Incidents.svc/ElevatorIncidents?StationCode=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Description\r\n\r\nReturns a list of reported elevator and escalator outages at a\r\ngiven station. Omit the StationCode parameter to return all reported\r\noutages.\r\n\r\nNote that for stations with multiple platforms and therefore StationCodes\r\n(e.g.: Metro Center, L'Enfant Plaza, etc.), a distinct call is required for\r\neach StationCode.\r\n\r\nElevator and escalator outages are refreshed once every 20 to 30 seconds approximately.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nElevatorIncidents\r\n\r\n\r\nArray containing elevator/escalator outage information\r\n(ElevatorIncident).\r\n\r\n\r\n\r\n\r\n\r\n\r\nElevatorIncident Elements\r\n\r\n\r\n\r\n\r\n\r\nDateOutOfServ\r\n\r\nDate and time (Eastern Standard Time) unit was reported out of\r\nservice. Will be in YYYY-MM-DDTHH:mm:ss format (e.g.:\r\n2014-10-27T15:17:00).\r\n\r\n\r\n\r\nDateUpdated\r\n\r\nDate and time (Eastern Standard Time) outage details was last\r\nupdated. Will be in YYYY-MM-DDTHH:mm:ss format (e.g.:\r\n2014-10-27T15:17:00).\r\n\r\n\r\n\r\nDisplayOrder\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nLocationDescription\r\n\r\nFree-text description of the unit location within a station\r\n(e.g.: Escalator between mezzanine and\r\nplatform).\r\n\r\n\r\n\r\nStationCode\r\n\r\nUnit's station code. Use this value in other rail-related APIs\r\nto retrieve data about a station.\r\n\r\n\r\n\r\nStationName\r\n\r\nFull station name, may include entrance information (e.g.:\r\nMetro Center, G and 11th St\r\nEntrance).\r\n\r\n\r\n\r\nSymptomCode\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nSymptomDescription\r\n\r\nDescription for why the unit is out of service or otherwise in\r\nreduced operation.\r\n\r\n\r\n\r\nTimeOutOfService\r\n\r\nDeprecated. Use the time\r\nportion of the DateOutOfServ element.\r\n\r\n\r\n\r\nUnitName\r\n\r\nUnique identifier for unit, by type (a single elevator and\r\nescalator may have the same UnitName, but no two elevators or two\r\nescalators will have the same UnitName).\r\n\r\n\r\n\r\nUnitStatus\r\n\r\nDeprecated. If listed here,\r\nthe unit is inoperational or otherwise impaired.\r\n\r\n\r\n\r\nUnitType\r\n\r\nType of unit. Will be ELEVATOR\r\nor ESCALATOR."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48f9a832-35f9-49cc-a732-7058dbc5f653"
            }
          ]
        },
        {
          "id": "95123d57-3ed7-445e-af5c-e0a4d835fc4f",
          "name": "54763641281d830c946a3d7a",
          "request": {
            "url": "http://api.wmata.com/Incidents.svc/Incidents",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Description\r\n\r\nReturns reported rail incidents (significant disruptions and delays to\r\nnormal service). The data is identical to WMATA's Metrorail Service Status\r\nfeed.\r\n\r\nRail incidents are refreshed once every 20 to 30 seconds approximately.\r\n\r\nResponse Elements\r\n\r\n\r\n\r\n\r\nElement\r\n\r\nDescription\r\n\r\n\r\n\r\n\r\n\r\nIncidents\r\n\r\n\r\nArray containing rail disruption information (Incident).\r\n\r\n\r\n\r\n\r\n\r\n\r\nIncident Elements\r\n\r\n\r\n\r\n\r\n\r\nDateUpdated\r\n\r\nDate and time (Eastern Standard Time) of last update. Will be\r\nin YYYY-MM-DDTHH:mm:SS format (e.g.: 2010-07-29T14:21:28).\r\n\r\n\r\n\r\nDelaySeverity\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nDescription\r\n\r\nFree-text description of the incident.\r\n\r\n\r\n\r\nEmergencyText\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nEndLocationFullName\r\n\r\nDeprecated.\r\n\r\n\r\n\r\nIncidentID\r\n\r\nUnique identifier for an incident.\r\n\r\n\r\n\r\nIncidentType\r\n\r\nFree-text description of the incident type. Usually Delay or\r\nAlert but is subject to change at any time.\r\n\r\n\r\n\r\nLinesAffected\r\n\r\nSemi-colon and space separated list of line codes (e.g.:\r\nRD; or BL;\r\nOR; or BL; OR; RD;). We do\r\nplan to update this to return something more reasonable like an\r\narray, but until then, use code similar to the following:\r\n\r\n\"RD; GR; BL;\".split(/;[\\s]?/).filter(function(fn) { return fn\r\n!== ''; })\r\n\r\n\r\n\r\nPassengerDelay\r\n\r\nDeprecated.\r\n\r\n\r\n\r\n\r\nStartLocationFullName\r\n\r\nDeprecated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6727481-a907-4b13-9d7d-e4ddce4ae8fd"
            }
          ]
        }
      ]
    }
  ]
}