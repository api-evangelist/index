{
  "info": {
    "name": "Spire All Messages from Date/Time Window",
    "_postman_id": "2f1e5b31-8f6f-4599-a850-957c20421f03",
    "description": "Returns all messages with a timestamp greater than `received_after` and timestamp less than `received_before`.\nQuery can also be used without the `received_before` parameter.\nTimestamp must be within the past 7 days.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Vessels",
      "item": [
        {
          "id": "4b37a95a-207f-455a-a798-ea0a2189790f",
          "name": "VesselsGet10",
          "request": {
            "url": "http://ais.spire.com/vessels?arriving_after=%7B%7D&arriving_before=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns all vessels with an ETA greater than the `arriving_after` and ETA less than the `arriving_before` parameter.\n\nQuery can also be used without the `arriving_before` parameter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bee0a863-14a7-4aa3-82fa-9da70d75b4b5"
            }
          ]
        },
        {
          "id": "02e63f7e-f829-4bb7-83bf-03d4685db772",
          "name": "VesselsA5b738b4Faf04a7e9a871c0ccfb123d2Get",
          "request": {
            "url": "http://ais.spire.com/vessels/a5b738b4-faf0-4a7e-9a87-1c0ccfb123d2",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns individual ship details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc3116e4-4868-400a-b89b-e3fe679ee157"
            }
          ]
        }
      ]
    },
    {
      "name": "Messages",
      "item": [
        {
          "id": "0e00266e-efd1-4ea0-bc18-a86973cd5e0c",
          "name": "MessagesGet4",
          "request": {
            "url": "http://ais.spire.com/messages?fields=%7B%7D&limit=%7B%7D&received_after=%7B%7D&received_before=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns all messages with a timestamp greater than `received_after` and timestamp less than `received_before`.\nQuery can also be used without the `received_before` parameter.\nTimestamp must be within the past 7 days."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77abc3e4-e162-49ae-9ebf-3a0f4c9aba00"
            }
          ]
        }
      ]
    }
  ]
}