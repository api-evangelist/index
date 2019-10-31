{
  "info": {
    "name": "Coord Bike Share API Get detailed information on a bike system, as a GeoJSON feature.",
    "_postman_id": "603dc530-0d12-4190-ae1c-77014957d6a6",
    "description": "Bike systems are individual bike share systems, often per-region.\n\nInformation is returned as a GeoJSON Feature. The geometry of the GeoJSON Feature is\na MultiPolygon that defines the system's operational area. All bike systems have an\noperational area, in which bikes may be found and parked.\nFor systems that require bikes be docked, this area is somewhat arbitrary, as bikes are\nonly found at stations. In this case, the operational area is roughly the city or\njurisdiction that the system covers.\nFor semi-dockless and dockless systems that allow bikes to be parked anywhere, the\noperational area is very important and strictly defined. Often there are extra fees for\nparking outside of the operational area (also known as a \"catchment area\"), and almost all\nbikes should be within the area.\n\nThese bike system types are reflected in the `station_type` property.\n* `dock` - All bikes must be taken from and returned to a dock.\n* `dockless` - All bikes are only dockless.\n* `dockless_with_hub` - Bikes may be dockless, or taken from or returned to a hub.\nA hub can be an area rather than a discrete station, where a bike can be returned and\nlocked but not explicitly docked. The total price of a rental may change based on whether\na bike is returned to a hub or not.\n\nAreas are returned as a GeoJSON MultiPolygon since areas may be discontiguous or have\nholes.\n\n### Example\n\n#### Request:\n`curl -G \"https://api.coord.co/v1/bike/system/CitiBike?access_key=\"`\n\n#### Response:\n```\n{\n  \"type\": \"Feature\",\n  \"geometry\": {\n      \"type\": \"MultiPolygon\",\n      \"coordinates\": [\n        [\n          [ [-74.00, 40.70], [-74.00, 40.80], [-73.90, 40.80], ..., [-74.00, 40.70] ]\n        ],\n        ...,\n        [\n          [ [-73.00, 41.70], [-73.00, 41.80], [-72.90, 41.80], ..., [-73.00, 41.70] ],\n          [ [-72.98, 41.75], [-72.98, 41.78], [-72.95, 41.78], ..., [-72.98, 41.75] ]\n        ]\n      ]\n    },\n  \"id\": \"CitiBike\",\n  \"properties\": {\n    \"email\": \"support@coord.co\",\n    \"phone_number\": \"+6789998212\",\n    \"station_type\": \"dock\",\n    \"is_transactable\": \"false\"\n  }\n}\n```",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bike",
      "item": [
        {
          "id": "74a78bcc-6a1a-4918-8b90-e8c4f83a8e66",
          "name": "search_locations",
          "request": {
            "url": "http://api.coord.co/v1/bike/location?access_key=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&radius_km=%7B%7D&system_ids=%7B%7D",
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
            "description": "Get a list of locations given the input parameters. Specify a search area by radius around\na latitude and longitude, as well as any filter for specific systems. Each location will\nbe a GeoJSON Feature, and aggregated into a GeoJSON FeatureCollection.\n\n### Example\n\n#### Request:\n`curl -G \"https://api.coord.co/v1/bike/location?latitude=40.742868&longitude=-73.989186&radius_km=0.25&access_key=\"`\n\n#### Response:\n```\n{\n  \"features\": [\n    {\n      \"geometry\": {\n        \"coordinates\": [\n          -73.98918628692627,\n          40.74286877312112\n        ],\n        \"type\": \"Point\"\n      },\n      \"id\": \"CitiBike-3641\",\n      \"properties\": {\n        \"is_renting\": true,\n        \"is_returning\": true,\n        \"last_reported\": \"2018-05-17T15:39:24.000Z\",\n        \"lat\": 40.74286877312112,\n        \"location_id\": \"3641\",\n        \"location_type\": \"bike_station_dock\",\n        \"lon\": -73.98918628692627,\n        \"name\": \"Broadway & W 25 St\",\n        \"num_bikes_available\": 53,\n        \"num_docks_available\": 1,\n        \"region_id\": \"71\",\n        \"system_id\": \"CitiBike\"\n      },\n      \"type\": \"Feature\"\n    },\n    {\n      \"geometry\": {\n        \"coordinates\": [\n          -73.99144871,\n          40.74395411\n        ],\n        \"type\": \"Point\"\n      },\n      \"id\": \"CitiBike-466\",\n      \"properties\": {\n        \"is_renting\": true,\n        \"is_returning\": true,\n        \"last_reported\": \"2018-05-17T15:32:40.000Z\",\n        \"lat\": 40.74395411,\n        \"location_id\": \"466\",\n        \"location_type\": \"bike_station_dock\",\n        \"lon\": -73.99144871,\n        \"name\": \"W 25 St & 6 Ave\",\n        \"num_bikes_available\": 35,\n        \"region_id\": \"71\",\n        \"system_id\": \"CitiBike\"\n      },\n      \"type\": \"Feature\"\n    }\n  ],\n  \"type\": \"FeatureCollection\"\n}\n```"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "721a964a-92dc-4148-9269-906492dd9654"
            }
          ]
        }
      ]
    },
    {
      "name": "Detailed",
      "item": [
        {
          "id": "876fb8c1-9e35-4ad9-9f74-3b9e70c25093",
          "name": "get_bike_location",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.coord.co",
              "path": [
                "v1",
                "bike",
                "location/:system_id/:location_id"
              ],
              "query": [
                {
                  "key": "access_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "system_id",
                  "value": "system_id",
                  "type": "string"
                },
                {
                  "id": "location_id",
                  "value": "location_id",
                  "type": "string"
                }
              ]
            },
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
            "description": "A bike location may be a single bike station (which can have multiple docked bikes) or a\nsingle dockless bike itself. All working docks are returned, but only free and rentable\ndockless bikes are returned.\n\n### Example\n\n#### Request:\n`curl -G \"https://api.coord.co/v1/bike/location/CitiBike/482?access_key=\"`\n\n#### Response:\n```\n{\n  \"geometry\": {\n    \"coordinates\": [\n      -73.99931783,\n      40.73935542\n    ],\n    \"type\": \"Point\"\n  },\n  \"id\": \"CitiBike-482\",\n  \"properties\": {\n    \"is_renting\": true,\n    \"is_returning\": true,\n    \"last_reported\": \"2018-05-17T15:41:06.000Z\",\n    \"lat\": 40.73935542,\n    \"location_id\": \"482\",\n    \"location_type\": \"bike_station_dock\",\n    \"lon\": -73.99931783,\n    \"name\": \"W 15 St & 7 Ave\",\n    \"num_bikes_available\": 19,\n    \"num_docks_available\": 19,\n    \"region_id\": \"71\",\n    \"system_id\": \"CitiBike\"\n  },\n  \"type\": \"Feature\"\n}\n```"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0e75ffc-d322-4c93-8c62-8f7f3d7f2d05"
            }
          ]
        },
        {
          "id": "2231fa16-ec8a-4288-a118-c42c97135792",
          "name": "get_bike_system",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.coord.co",
              "path": [
                "v1",
                "bike",
                "system/:system_id"
              ],
              "query": [
                {
                  "key": "access_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "system_id",
                  "value": "system_id",
                  "type": "string"
                }
              ]
            },
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
            "description": "Bike systems are individual bike share systems, often per-region.\n\nInformation is returned as a GeoJSON Feature. The geometry of the GeoJSON Feature is\na MultiPolygon that defines the system's operational area. All bike systems have an\noperational area, in which bikes may be found and parked.\nFor systems that require bikes be docked, this area is somewhat arbitrary, as bikes are\nonly found at stations. In this case, the operational area is roughly the city or\njurisdiction that the system covers.\nFor semi-dockless and dockless systems that allow bikes to be parked anywhere, the\noperational area is very important and strictly defined. Often there are extra fees for\nparking outside of the operational area (also known as a \"catchment area\"), and almost all\nbikes should be within the area.\n\nThese bike system types are reflected in the `station_type` property.\n* `dock` - All bikes must be taken from and returned to a dock.\n* `dockless` - All bikes are only dockless.\n* `dockless_with_hub` - Bikes may be dockless, or taken from or returned to a hub.\nA hub can be an area rather than a discrete station, where a bike can be returned and\nlocked but not explicitly docked. The total price of a rental may change based on whether\na bike is returned to a hub or not.\n\nAreas are returned as a GeoJSON MultiPolygon since areas may be discontiguous or have\nholes.\n\n### Example\n\n#### Request:\n`curl -G \"https://api.coord.co/v1/bike/system/CitiBike?access_key=\"`\n\n#### Response:\n```\n{\n  \"type\": \"Feature\",\n  \"geometry\": {\n      \"type\": \"MultiPolygon\",\n      \"coordinates\": [\n        [\n          [ [-74.00, 40.70], [-74.00, 40.80], [-73.90, 40.80], ..., [-74.00, 40.70] ]\n        ],\n        ...,\n        [\n          [ [-73.00, 41.70], [-73.00, 41.80], [-72.90, 41.80], ..., [-73.00, 41.70] ],\n          [ [-72.98, 41.75], [-72.98, 41.78], [-72.95, 41.78], ..., [-72.98, 41.75] ]\n        ]\n      ]\n    },\n  \"id\": \"CitiBike\",\n  \"properties\": {\n    \"email\": \"support@coord.co\",\n    \"phone_number\": \"+6789998212\",\n    \"station_type\": \"dock\",\n    \"is_transactable\": \"false\"\n  }\n}\n```"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61c2b53a-09cc-4f09-b360-3ec1b0f0d652"
            }
          ]
        }
      ]
    },
    {
      "name": "Cost",
      "item": [
        {
          "id": "5613ac0b-bda0-45fb-89ed-2b3a4d1ec554",
          "name": "get_quote",
          "request": {
            "url": "http://api.coord.co/v1/bike/quote?access_key=%7B%7D&system_ids=%7B%7D",
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
            "description": "Provide price quotes for renting a bike. There can be multiple quotes per system, reflecting\ndifferent options for buying membership such as single-ride, single-day, and multi-day\npasses. Please keep in mind that quotes are estimates.\n\n### Example\n\n#### Request:\n`curl -G \"https://api.coord.co/v1/bike/quote?access_key=\"`\n\n#### Response:\n```\n[\n  {\n    \"cost\": {\n      \"amount\": 108,\n      \"currency\": \"USD\"\n    },\n    \"id\": 2,\n    \"max_days\": 1,\n    \"system_id\": \"CitiBike\",\n    \"tax_regions\": [{\n      \"name\": \"New York City\",\n      \"tax_rate\": 0.08875\n    }, {\n      \"name\": \"Jersey City\",\n      \"tax_rate\": 0.07\n    }],\n    \"usage_fees\": [\n      {\n        \"cost\": {\n          \"amount\": 200,\n          \"currency\": \"USD\"\n        },\n        \"id\": 1,\n        \"pass_type_id\": 2,\n        \"prorated\": false,\n        \"start_time_seconds\": 1800\n      },\n      {\n        \"cost\": 1.5,\n        \"fee_increment_seconds\": 900,\n        \"prorated\": false,\n        \"start_time_seconds\": 3600\n      }\n    ]\n  },\n  {\n    \"cost\": {\n      \"amount\": 272,\n      \"currency\": \"USD\"\n    },\n    \"id\": 3,\n    \"max_days\": 3,\n    \"system_id\": \"CitiBike\",\n    \"tax_regions\": [{\n      \"name\": \"New York City\",\n      \"tax_rate\": 0.08875\n    }, {\n      \"name\": \"Jersey City\",\n      \"tax_rate\": 0.07\n    }],\n    \"usage_fees\": [\n      {\n        \"cost\": {\n          \"amount\": 100,\n          \"currency\": \"USD\"\n        },\n        \"fee_increment_seconds\": 900,\n        \"prorated\": false,\n        \"start_time_seconds\": 1800\n      }\n    ]\n  }\n]\n```"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94fad6ad-36db-4e05-b867-aa420a4a7078"
            }
          ]
        }
      ]
    },
    {
      "name": "Information",
      "item": [
        {
          "id": "17324d39-faf8-4dd4-a455-6d1187bb2041",
          "name": "search_bike_systems",
          "request": {
            "url": "http://api.coord.co/v1/bike/system?access_key=%7B%7D&latitude=%7B%7D&longitude=%7B%7D&radius_km=%7B%7D",
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
            "description": "Bike systems are individual bike share systems, often per-region.\n\nInformation about each system is returned as a GeoJSON Feature, within a single GeoJSON\nFeatureCollection.\n\nSee the [/system/{system_id}](#reference/0/get-information-for-a-bike-system) call for more\ndetails on the individual system Features.\n\n### Example\n\n#### Request:\n`curl -G \"https://api.coord.co/v1/bike/system?latitude=40.74286877312112&longitude=-73.98918628692627&radius_km=0.5&access_key=\"`\n\n#### Response:\n```\n{\n  \"features\": [\n    {\n      \"geometry\": {\n        \"coordinates\": [\n          [\n            [\n              [\n                -74.055701,\n                40.707838\n              ],\n              [\n                -74.083639,\n                40.714807\n              ],\n              ...,\n              [\n                -74.055701,\n                40.707838\n              ]\n            ]\n          ]\n        ],\n        \"type\": \"MultiPolygon\"\n      },\n      \"id\": \"CitiBike\",\n      \"properties\": {\n        \"is_transactable\": true,\n        \"station_type\": \"dock\"\n      },\n      \"type\": \"Feature\"\n    }\n  ],\n  \"type\": \"FeatureCollection\"\n}\n```"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f720a22f-b98f-43e8-9d82-85c2396fffdb"
            }
          ]
        }
      ]
    }
  ]
}