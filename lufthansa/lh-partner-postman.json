{
  "info": {
    "name": "LH Partner Seat Details",
    "_postman_id": "12e653dd-8538-49ae-882b-e98ab926021d",
    "description": "A description of all available seat details by aircraft type. You can retrieve the full set or details for a particular aircraft type.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Baggage",
      "item": [
        {
          "id": "ce4a9cc0-487c-4295-8510-e0968dd20f72",
          "name": "baggage.baggagetripandcontact.searchID.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "baggage/baggagetripandcontact/:searchID"
              ],
              "variable": [
                {
                  "id": "searchID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve passenger trip, contact and baggage details. This service is only accessible for LH privileged partners"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a60d146-93cf-41bf-8fde-b75f6e5e7d0a"
            }
          ]
        }
      ]
    },
    {
      "name": "All",
      "item": [
        {
          "id": "ee6ed9fe-9613-4426-b7bd-d62681cf1e1f",
          "name": "offers.fares.allfares.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/allfares?cabin-class=%7B%7D&catalogues=%7B%7D&destination=%7B%7D&fare-family=%7B%7D&origin=%7B%7D&return-date=%7B%7D&trackingid=%7B%7D&travel-date=%7B%7D&travelers=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "Mandatory http header:  application/xml or application/json",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves all available fares for a specific Origin & Destination pair on a given date. Available fares are: One-way and Return for 4U. Return only for OS"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5455d951-0daf-4f8b-9c47-b90ded3b6f07"
            }
          ]
        }
      ]
    },
    {
      "name": "Best",
      "item": [
        {
          "id": "aefc9997-3ef1-4f87-b002-dee108efbc1d",
          "name": "offers.fares.bestfares.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/bestfares?cabin-class=%7B%7D&catalogues=%7B%7D&country=%7B%7D&destination=%7B%7D&fare-family=%7B%7D&origin=%7B%7D&range=%7B%7D&trackingid=%7B%7D&travel-date=%7B%7D&trip-duration=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve best fares for the requested journey across multiple days or multiple months."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0bcebff-4360-4bfc-b455-2c4f23301f30"
            }
          ]
        }
      ]
    },
    {
      "name": "Deep",
      "item": [
        {
          "id": "7b295f17-4aee-4668-bbb2-62285639c32f",
          "name": "offers.fares.deeplink.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/deeplink?cabin-class=%7B%7D&catalogues=%7B%7D&country=%7B%7D&destination=%7B%7D&destination-name=%7B%7D&encryption-key=%7B%7D&fare=%7B%7D&fare-currency=%7B%7D&lang=%7B%7D&net-fare=%7B%7D&origin=%7B%7D&origin-name=%7B%7D&outbound-segments=%7B%7D&partnerid=%7B%7D&return-date=%7B%7D&return-segments=%7B%7D&trackingid=%7B%7D&travel-date=%7B%7D&travelers=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns valid deep links for the provided input parameters"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "863d2085-0ff7-49de-8d01-dc8fbf0e3b7a"
            }
          ]
        }
      ]
    },
    {
      "name": "LH",
      "item": [
        {
          "id": "11869eeb-63fa-4fa5-ab71-5c52bd773cbf",
          "name": "offers.fares.deeplink.ffp.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/deeplink/ffp?cabin-class=%7B%7D&catalogues=%7B%7D&country=%7B%7D&destination=%7B%7D&encryption-key=%7B%7D&lang=%7B%7D&origin=%7B%7D&partnerid=%7B%7D&return-date=%7B%7D&trackingid=%7B%7D&travel-date=%7B%7D&travelers=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns valid LH deep links (FFP - links to flight selection screen on LH.COM)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6a5638c-ddf4-4b15-ae35-d6aac2664f5d"
            }
          ]
        },
        {
          "id": "668616e8-bf60-4891-aa75-66ee3acc3648",
          "name": "offers.fares.deeplink.itco.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/deeplink/itco?cabin-class=%7B%7D&catalogues=%7B%7D&country=%7B%7D&destination=%7B%7D&encryption-key=%7B%7D&fare=%7B%7D&fare-currency=%7B%7D&lang=%7B%7D&net-fare=%7B%7D&origin=%7B%7D&outbound-segments=%7B%7D&partnerid=%7B%7D&return-date=%7B%7D&return-segments=%7B%7D&trackingid=%7B%7D&travel-date=%7B%7D&travelers=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns valid LH deep links (ITCO - links to shopping cart on LH.COM)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0871d9c7-c7d2-43ea-bc16-77149af3668b"
            }
          ]
        }
      ]
    },
    {
      "name": "Fares",
      "item": [
        {
          "id": "49297da7-84fd-4810-bcf5-3463cef0a5ce",
          "name": "Fares",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/fares?carriers=%7B%7D&catalogues=%7B%7D&fare-types=%7B%7D&segments=%7B%7D&travelers=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve all available fares per fare family for a specific Origin & Destination on a given date"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8161e37-ddac-49d8-9715-a9e2cc216701"
            }
          ]
        },
        {
          "id": "f13379c2-f407-41b3-9cdc-699966892f17",
          "name": "offers.fares.subscriptions.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/subscriptions?cabin-class=%7B%7D&country=%7B%7D&destination=%7B%7D&email=%7B%7D&lang=%7B%7D&origin=%7B%7D&trackingid=%7B%7D&trip-duration=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Create a subscription for best price O&D. Receive regular updates on lowest fares"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7ecfd9a-348e-4b1a-bb9c-5ab8f73b2244"
            }
          ]
        }
      ]
    },
    {
      "name": "Lowest",
      "item": [
        {
          "id": "e91558ce-fe83-47a5-baf0-0c228714c2fb",
          "name": "offers.fares.lowestfares.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/fares/lowestfares?cabin-class=%7B%7D&catalogues=%7B%7D&country=%7B%7D&destination=%7B%7D&fare-family=%7B%7D&origin=%7B%7D&return-date=%7B%7D&travel-date=%7B%7D&travelers=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve lowest fare for a specific Origin & Destination pair on a given date. Available fares are: One-way and Return for 4U. Return only for OS & LH"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e332871-9050-4005-b77f-fcbe8de5d331"
            }
          ]
        }
      ]
    },
    {
      "name": "OND",
      "item": [
        {
          "id": "4a2759e1-94ac-4d18-9ea6-6da40ea45e42",
          "name": "offers.ond.route.origin.destination.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "offers/ond/route/:origin/:destination"
              ],
              "query": [
                {
                  "key": "catalogues",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "destination",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "origin",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "Mandatory http header:  application/xml or application/json",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns LH route origin & destination information"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "250da01f-ca5c-4e43-9e67-f0320a7c55e1"
            }
          ]
        },
        {
          "id": "34ff76ed-cc9b-4e47-95a3-5e4981d4e083",
          "name": "offers.ond.status.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/ond/status?catalogues=%7B%7D&new-routes=%7B%7D&old-routes=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "Mandatory http header:  application/xml or application/json",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns LH network route status information. Search for recently added or retired routes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e10cc96-8098-4a13-8aed-589b8cdc05de"
            }
          ]
        }
      ]
    },
    {
      "name": "Top",
      "item": [
        {
          "id": "3940fed5-2dc3-4e35-a03f-6e927d33d5e3",
          "name": "offers.ond.top.get",
          "request": {
            "url": "http://api.lufthansa.com/v1/offers/ond/top?catalogues=%7B%7D&origin=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "Mandatory http header:  application/xml or application/json",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns LH Top routes per country or across all countries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59366fd2-812f-431c-9811-bd634eb785ba"
            }
          ]
        }
      ]
    },
    {
      "name": "Orders",
      "item": [
        {
          "id": "75697ac0-83de-48e9-811e-832c4a32e0ae",
          "name": "Orders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "orders/orders/:orderID/:name"
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "orderID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve order by ID and optionally name. This service is only accessible for LH privileged partners"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a8c3463-0600-4b78-82e6-b5f15d4da417"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto",
      "item": [
        {
          "id": "0ec32410-45a8-49c3-9b31-7db71165db47",
          "name": "preflight.autocheckin.ticketnumber.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "preflight/autocheckin/:ticketnumber"
              ],
              "query": [
                {
                  "key": "emailAddress",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ticketnumber",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Trigger an automatic check-in given a ticket number. This service is only accessible for LH privileged partners"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77511ffa-73a9-402e-b355-8b82e2adb051"
            }
          ]
        }
      ]
    },
    {
      "name": "Price",
      "item": [
        {
          "id": "be47912e-0dc6-4463-b3fb-28d01a71dae7",
          "name": "promotions.priceoffers.flights.ond.origin.destination.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "promotions/priceoffers/flights/ond/:origin/:destination"
              ],
              "query": [
                {
                  "key": "departureDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "returnDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "service",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "destination",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "origin",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a best price offer given an origin and destination."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db24778d-45ca-4964-bd6c-9778786023f3"
            }
          ]
        }
      ]
    },
    {
      "name": "Seat",
      "item": [
        {
          "id": "c930323a-ceba-43f9-a0bd-3ff529757da5",
          "name": "references.seatdetails.aircraftCode.cabinCode.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.lufthansa.com",
              "path": [
                "v1",
                "references/seatdetails/:aircraftCode/:cabinCode"
              ],
              "query": [
                {
                  "key": "lang",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "aircraftCode",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "cabinCode",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "http header: application/json or application/xml (Acceptable values are: application/json, application/xml)",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "A description of all available seat details by aircraft type. You can retrieve the full set or details for a particular aircraft type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d791757-5c9e-4185-bd20-9462ea4b9f03"
            }
          ]
        }
      ]
    }
  ]
}