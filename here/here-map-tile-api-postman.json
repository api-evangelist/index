{
  "info": {
    "name": "HERE Map Tile API Transparent Truck Restrictions Map",
    "_postman_id": "94552c31-9f06-4c98-b7b6-544c2cb2d487",
    "description": "*Request a transparent tile showing restrictions for heavy vehicles only*\n\nTo obtain a transparent map tile displaying route restrictions for trucks, use the `truckonlytile` parameter in the path of the request URL.\n\n\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Terrain",
      "item": [
        {
          "id": "dedf2286-6717-469a-b74a-70c318a6046b",
          "name": "TerrainDay76645256Png8Get",
          "request": {
            "url": "http://1.aerial.maps.cit.api.here.com/maptile/2.1/maptile/newest/terrain.day/7/66/45/256/png8?app_code=%7B%7D&app_id=%7B%7D",
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
            "description": "*Request a terrain map tile*\n\nTerrain map tile are available by passing `terrain.day` in the path of the request URL.\n\n\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81916bf8-4b6f-4907-bc36-9b97dcb48e49"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "01d795ac-72b8-404e-b9df-db3a7e6c0c5e",
          "name": "MaptileNewestNormalDay63024256Png8Get",
          "request": {
            "url": "http://1.aerial.maps.cit.api.here.com/maptile/2.1/maptile/newest/maptile/newest/normal.day/6/30/24/256/png8?app_code=%7B%7D&app_id=%7B%7D&output=%7B%7D&range=%7B%7D",
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
            "description": "*Request multiple base64 encoded map tiles*\n\nA square consisting of multiple base64 encoded tiles is requested by adding the parameters `output=base64` and `range=NxN` to the request URL. The `column` and `row` in the path of the URL, defining the top left-hand corner of the tile group must be divisible by the value of the `range` parameter.\n  \n  Click on the response to decode the tiles returned.\n\n\n\n* **output**  `text`\n \\- Indicates whether to return the tile as base64 encoded text.\n\n* **range**  `enum`\n \\- Indicates the size of the array of tiles returned. Valid values are `2x2`, `3x3` or `4x4`\n\n Valid values are : `2x2`, `3x3`, `4x4`\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7eec457-da07-44c5-91f1-6c777f86af60"
            }
          ]
        }
      ]
    },
    {
      "name": "Color-reduced",
      "item": [
        {
          "id": "08d5cf9e-abdf-488e-925b-6849c55723de",
          "name": "MaptileNewestNormalDayTransit1220741409256Png8Get",
          "request": {
            "url": "http://1.aerial.maps.cit.api.here.com/maptile/2.1/maptile/newest/maptile/newest/normal.day.transit/12/2074/1409/256/png8?app_code=%7B%7D&app_id=%7B%7D",
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
            "description": "*Request a color-reduced map tile with public transport*\n\nColor-reduced street map tiles with full-color transit overlays are requested by passing `normal.day.transit` in the path of the request URL.\n\n\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e9df867-8969-4d69-8c34-ad52e71765ed"
            }
          ]
        },
        {
          "id": "0f4e87ab-bbcc-4f26-bb0e-728eb86cadbf",
          "name": "MaptileNewestNormalDayGrey11525761256Png8Get",
          "request": {
            "url": "http://1.aerial.maps.cit.api.here.com/maptile/2.1/maptile/newest/maptile/newest/normal.day.grey/11/525/761/256/png8?app_code=%7B%7D&app_id=%7B%7D",
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
            "description": "*Request a greyed out street map tile*\n\nMaps using a reduced color palette can be requested by passing `normal.day.grey` in the path of the request URL.\n\n\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e4c4847e-a4de-41b7-bcac-94823fc992c4"
            }
          ]
        }
      ]
    },
    {
      "name": "Hybrid",
      "item": [
        {
          "id": "00085e16-cd79-434c-aab5-4f90f4a610e7",
          "name": "HybridDay485256Png8Get",
          "request": {
            "url": "http://1.aerial.maps.cit.api.here.com/maptile/2.1/maptile/newest/hybrid.day/4/8/5/256/png8?app_code=%7B%7D&app_id=%7B%7D&lg=%7B%7D",
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
            "description": "*Request a hybrid map tile - satellite imagery with labels*\n\nHybrid map tile are available by passing `hybrid.day` in the path of the request URL. The map tiles will display using the default language of the server unless the `lg` query parameter is used to change the map tile language. Consult the  Map Tile API Reference for a full list of available languages.\n\n\n\n* **lg**  `enum`\n \\- Alters the language of the labels displayed on the map. Three letter MARC code, for example `rus` for Russian language.\n\n Valid values are : `ara` - Arabic, `chi` - Chinese, `cht` - Chinese (Trad), `dut` - Dutch, `eng` - English, `fre` - French, `ger` - German, `gle` - Gaelic, `gre` - Greek, `heb` - Hebrew, `hin` - Hindi, `ind` - Indonesian, `ita` - Italian, `per` - Persian, `pol` - Polish, `por` - Portuguese, `rus` - Russian, `sin` - Sinhalese, `spa` - Spanish, `tha` - Thai, `tur` - Turkish, `ukr` - Ukranian, `urd` - Urdu, `vie` - Vietnamese, `wel` - Welsh\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0cd243ca-cc9f-446f-9126-e1d6a8195b57"
            }
          ]
        }
      ]
    },
    {
      "name": "Truck",
      "item": [
        {
          "id": "6554fdce-4498-4ce5-8581-05993e8c31db",
          "name": "TrucktileNewestNormalDay1221991342256Png8Get",
          "request": {
            "url": "http://1.aerial.maps.cit.api.here.com/maptile/2.1/maptile/newest/trucktile/newest/normal.day/12/2199/1342/256/png8?app_code=%7B%7D&app_id=%7B%7D",
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
            "description": "*Request a street map tile showing restrictions for heavy vehicles*\n\nTo obtain a map tile displaying route restrictions for trucks, use the `trucktile` parameter in the path of the request URL.\n\n\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ab05256-ada6-44dd-b635-a9504d0210a1"
            }
          ]
        }
      ]
    },
    {
      "name": "Toll",
      "item": [
        {
          "id": "bcdc3a71-16d9-4530-bdf6-2436ab7959c2",
          "name": "MaptileNewestNormalDay9255170256Png8Get",
          "request": {
            "url": "http://1.aerial.maps.cit.api.here.com/maptile/2.1/maptile/newest/maptile/newest/normal.day/9/255/170/256/png8?app_code=%7B%7D&app_id=%7B%7D&congestion=%7B%7D",
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
            "description": "*Request a street map tile highlighting congestion and environmental toll zones*\n\nTo highlight such toll zones, add the `congestion` parameter to the request URL.\n\n\n\n* **congestion**  `null`\n \\- Flag to indicate if congestion zones are to be shown on the map.\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e599c8da-4ce7-45d5-8cfc-64de2ac70de9"
            }
          ]
        }
      ]
    },
    {
      "name": "Satellite",
      "item": [
        {
          "id": "fdd68a51-d996-453c-a11a-927d00a821fd",
          "name": "SatelliteDay51512256Png8Get",
          "request": {
            "url": "http://1.aerial.maps.cit.api.here.com/maptile/2.1/maptile/newest/satellite.day/5/15/12/256/png8?app_code=%7B%7D&app_id=%7B%7D",
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
            "description": "*Request a satellite map tile*\n\nSatellite map tiles do not display labels and are available by passing `satellite.day` in the path of the request URL.\n\n\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "598b0bd5-fb9b-4311-8dad-b8c124cc4a0d"
            }
          ]
        }
      ]
    },
    {
      "name": "Fleet",
      "item": [
        {
          "id": "fbc6c75c-03b4-4caa-8b93-c569c1a2cd19",
          "name": "MaptileNewestNormalDay1340932723256Png8Get",
          "request": {
            "url": "http://1.aerial.maps.cit.api.here.com/maptile/2.1/maptile/newest/maptile/newest/normal.day/13/4093/2723/256/png8?app_code=%7B%7D&app_id=%7B%7D&style=%7B%7D",
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
            "description": "*Request a street map tile using the fleet vehicle color scheme*\n\nFleet color scheme map tiles are available by passing `style=fleet` as a parameter of the request URL.\n\n\n\n* **style**  `enum`\n \\- If present, selects the style to use to render the tile.\n\n Valid values are : `default`, `alps`, `fleet`, `wings`, `dreamworks`, `flame`, `mini`\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a14246f4-dd1a-4ff1-a87a-58f01faa0c1f"
            }
          ]
        }
      ]
    },
    {
      "name": "Base64",
      "item": [
        {
          "id": "b0520c9c-7cb8-4165-9549-eaabb0e07fe1",
          "name": "MaptileNewestNormalDay11525761256Png8Get4",
          "request": {
            "url": "http://1.aerial.maps.cit.api.here.com/maptile/2.1/maptile/newest/maptile/newest/normal.day/11/525/761/256/png8?app_code=%7B%7D&app_id=%7B%7D&output=%7B%7D",
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
            "description": "*Request a base64 encoded map tile*\n\nBase64 encoded tiles are requested by adding the parameter `output=base64` to the request URL.\n  \n  Click on the response to decode the tile returned.\n\n\n\n* **output**  `text`\n \\- Indicates whether to return the tile as base64 encoded text.\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6cfc95e-2f93-4e29-a477-8d32b065ac57"
            }
          ]
        }
      ]
    },
    {
      "name": "Map",
      "item": [
        {
          "id": "a990ac36-14d8-4d49-a885-bf22e1c2b89b",
          "name": "InfoGet",
          "request": {
            "url": "http://1.aerial.maps.cit.api.here.com/maptile/2.1/maptile/newest/info?app_code=%7B%7D&app_id=%7B%7D&output=%7B%7D",
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
            "description": "*Request information about the types of map tiles available on a server*\n\nTo make a request for metadata information, use the `info` parameter in the path of the request URL.\n\n\n\n* **output**  `enum`\n \\- Indicates whether to return the information in XML format, JSON format or as an XML schema (XSD) of the API metadata\n\n Valid values are : `json`, `xml`, `xsd`\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9726d074-ea5e-44a9-a18c-26d4c6526ac0"
            }
          ]
        }
      ]
    },
    {
      "name": "Transparent",
      "item": [
        {
          "id": "f6bd30ef-ec9e-4726-b231-350364a20c89",
          "name": "TruckonlytileNewestNormalDay1221991342256Png8Get",
          "request": {
            "url": "http://1.aerial.maps.cit.api.here.com/maptile/2.1/maptile/newest/truckonlytile/newest/normal.day/12/2199/1342/256/png8?app_code=%7B%7D&app_id=%7B%7D",
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
            "description": "*Request a transparent tile showing restrictions for heavy vehicles only*\n\nTo obtain a transparent map tile displaying route restrictions for trucks, use the `truckonlytile` parameter in the path of the request URL.\n\n\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.\n\n* **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed9cedcd-2c01-4d51-8467-4892a8b7b0a7"
            }
          ]
        }
      ]
    }
  ]
}