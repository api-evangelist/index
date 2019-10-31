{
  "info": {
    "name": "Amadeus Get Travel Record Record Locator",
    "_postman_id": "613b1f93-b5c3-4a4f-8231-51cb2cbf529d",
    "description": "Note: This API requires the use of HTTPS\n\nThis service retrieves a travel record (also sometimes referred to as a PNR) for a given journey when provided with Record Locator to identify a travel record, along with the last name of any traveler who is marked as a passenger on this record.\n\nThe API provides detailed information on a given record, including any air, car, hotel or rail reservations, as well as passenger details, and contact frequent traveler information for each passenger when available. You can use this to provide a wide variety of pre-trip or in-trip services.\n\nNote that this API transmits sensitive personal data about a traveler's journey. We work hard to ensure that we comply with all the legal requirements this entails, and as an application owner, you need to do so too - we don't want you to get in trouble! This paragraph, or anything else in our documentation, does not constitute legal advice, it's just to give you an idea of some of the potential issues that you may encounter. Please check your legal obligations regarding the use of this data before implementing this API\n\nIn most countries, the data in the returned travel record is considered to be the property of the traveler. In order to ensure that you are acting on behalf of the traveler, we require you to provide the traveler's last name in addition to the record locator when you make a call to this API. You should ensure that you have consent from the traveler before retrieving this record, in some countries this is a legal requirement - please respect this appropriately.\n\nOur data center is based in Europe, so there is a legal requirement that you to access this API over a secure connection. If you plan to store the information returned by this API, ensure you comply with storage requirements for European data, in addition to those of your local country. For example, there are strict requirements on the caching of retrieved travel records, so please ensure the cache control HTTP headers in the response are respected.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "travel",
      "item": [
        {
          "id": "cb9a710c-bd3b-4fc4-84da-846d03765aa4",
          "name": "getTravelRecordRecordLocator",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.sandbox.amadeus.com",
              "path": [
                "v1.2",
                "travel-record/:record_locator"
              ],
              "query": [
                {
                  "key": "env",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "last_name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "record_locator",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Note: This API requires the use of HTTPS\n\nThis service retrieves a travel record (also sometimes referred to as a PNR) for a given journey when provided with Record Locator to identify a travel record, along with the last name of any traveler who is marked as a passenger on this record"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e4322e31-9691-4a20-b077-61fa4c6b1cbb"
            }
          ]
        }
      ]
    }
  ]
}