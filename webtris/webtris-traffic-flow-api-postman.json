{
  "info": {
    "name": "WebTRIS Traffic Flow API Returns the layer metadata for the LayerId specified.",
    "_postman_id": "ab1a4228-e486-4b73-b84d-31f60a65f7fb",
    "description": "Returns the layer metadata for the layerid specified..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Returns",
      "item": [
        {
          "id": "a0471432-a700-490d-b7a2-f21614fbb546",
          "name": "Areas_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "webtris.highwaysengland.co.uk",
              "path": [
                "api",
                "v:version/areas"
              ],
              "variable": [
                {
                  "id": "version",
                  "value": "{}",
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
            "description": "Returns list of areas."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c1a65f1-b3ff-4460-86d3-133f66e14548"
            }
          ]
        },
        {
          "id": "06a80a86-bba3-492d-a259-516f471f6738",
          "name": "Areas_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "webtris.highwaysengland.co.uk",
              "path": [
                "api",
                "v:version/areas/:area_Ids"
              ],
              "variable": [
                {
                  "id": "area_Ids",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "version",
                  "value": "{}",
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
            "description": "Returns details of selected area."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2e7570a-dd18-4b3a-bda6-5dd923ba23a9"
            }
          ]
        },
        {
          "id": "58573955-a0bc-428c-8a1e-6d75e89437b6",
          "name": "SiteTypes_GetSitesForPublicFacingAPI",
          "request": {
            "url": {
              "protocol": "http",
              "host": "webtris.highwaysengland.co.uk",
              "path": [
                "api",
                "v:version/sitetypes/:siteType_Id/sites"
              ],
              "variable": [
                {
                  "id": "siteType_Id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "version",
                  "value": "{}",
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
            "description": "Returns the layer metadata for the layerid specified.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6633bc15-50a1-44ea-81ba-e3c12fb52e21"
            }
          ]
        }
      ]
    },
    {
      "name": "Site",
      "item": [
        {
          "id": "4e298215-cb9d-417d-aff5-3d28c219bd73",
          "name": "Quality_GetOverallDataQualityForSites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "webtris.highwaysengland.co.uk",
              "path": [
                "api",
                "v:version/quality/overall"
              ],
              "query": [
                {
                  "key": "end_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sites",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_date",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "version",
                  "value": "{}",
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
            "description": "Get site overallquality."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4d3cf6b-3892-44d6-a3e3-38ebffe3e390"
            }
          ]
        },
        {
          "id": "f79ae1e6-cdb5-4066-9081-2afdc9bdc038",
          "name": "Quality_GetDailyDataQualityForSite",
          "request": {
            "url": {
              "protocol": "http",
              "host": "webtris.highwaysengland.co.uk",
              "path": [
                "api",
                "v:version/quality/daily"
              ],
              "query": [
                {
                  "key": "end_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "siteId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_date",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "version",
                  "value": "{}",
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
            "description": "Get site dailyquality."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cba2c91-1fbc-48d5-93d1-4f27ce26bf72"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "5bc1380c-f494-4a75-94d7-e1f5c0a51ded",
          "name": "Reports_Index",
          "request": {
            "url": {
              "protocol": "http",
              "host": "webtris.highwaysengland.co.uk",
              "path": [
                "api",
                "v:version/reports/:report_type"
              ],
              "query": [
                {
                  "key": "end_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page_size",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "reportSubTypeId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sites",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_date",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "report_type",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "version",
                  "value": "{}",
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
            "description": "Gets the daily report.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c91f9e6e-d6c4-4819-bb0c-f0332c0c5b57"
            }
          ]
        },
        {
          "id": "f4e4acb7-05e1-40f3-ba44-1bceb728ab3a",
          "name": "Reports_Index1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "webtris.highwaysengland.co.uk",
              "path": [
                "api",
                "v:version/reports/:start_date/to/:end_date/:report_type"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page_size",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "reportSubTypeId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sites",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "end_date",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "report_type",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "start_date",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "version",
                  "value": "{}",
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
            "description": "Gets the daily report.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6912c5b-c70c-404b-afd3-c61d2733e276"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "b38ae3b8-fcd6-4a34-a724-41d95936d569",
          "name": "Sites_Index",
          "request": {
            "url": {
              "protocol": "http",
              "host": "webtris.highwaysengland.co.uk",
              "path": [
                "api",
                "v:version/sites"
              ],
              "variable": [
                {
                  "id": "version",
                  "value": "{}",
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
            "description": "Get a list of sites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a36390f-d025-4bb1-a2e3-083673de1d3e"
            }
          ]
        }
      ]
    },
    {
      "name": "Selected",
      "item": [
        {
          "id": "e9eb6b2f-4bb0-4741-8387-4fba5ae50fcf",
          "name": "Sites_Index",
          "request": {
            "url": {
              "protocol": "http",
              "host": "webtris.highwaysengland.co.uk",
              "path": [
                "api",
                "v:version/sites/:site_Ids"
              ],
              "variable": [
                {
                  "id": "site_Ids",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "version",
                  "value": "{}",
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
            "description": "Get selected sites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a85ff0a1-b5b6-48ec-bb31-dccf4511a429"
            }
          ]
        }
      ]
    },
    {
      "name": "Return",
      "item": [
        {
          "id": "166238da-95df-4514-9ad5-7c3d27ec23b7",
          "name": "SiteTypes_Index",
          "request": {
            "url": {
              "protocol": "http",
              "host": "webtris.highwaysengland.co.uk",
              "path": [
                "api",
                "v:version/sitetypes"
              ],
              "variable": [
                {
                  "id": "version",
                  "value": "{}",
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
            "description": "Return list of site types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1afda79-1d4d-4844-8505-9298b9c74617"
            }
          ]
        }
      ]
    }
  ]
}