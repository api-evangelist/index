{
  "info": {
    "name": "NxtPort Bel Air API Retrieve the city layer data for the specified layer, metric and date.",
    "_postman_id": "b6568eaf-7b96-430b-bfb8-905ae2a4f1d4",
    "description": "This operation retrieves city layer data for the specified layer, metric and date combination. The date is passed in the following format: YYYYMMDD. The values for the layerId and metricId can be fetched from the /layers and /metrics operations.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "MEtrics",
      "item": [
        {
          "id": "9aaf3cbd-98c0-4497-820c-7346fd28775b",
          "name": "getMetrics",
          "request": {
            "url": "http://api-stg.nxtport.eu/belair/v1/metrics",
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
            "description": "The platform allows you to retrieve supported metrics by sending a HTTP GET to /metrics. \nThe string-values for the attribute id can be used as a metricId path parameter in the City Layer operations. \nThe attribute granularity indicates how fine grained temporal pages should be split up when querying individual sources (and can be ignored here)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "acfcd5b4-360e-4108-9a6a-41889475ea3f"
            }
          ]
        }
      ]
    },
    {
      "name": "Layers",
      "item": [
        {
          "id": "54fe270c-e1cc-4e6c-8ee6-fe7ce8e4d3d6",
          "name": "getLayers",
          "request": {
            "url": "http://api-stg.nxtport.eu/belair/v1/layers",
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
            "description": "This operation lists the currently available city layers. \nThe returned strings can then be used as a layerId path parameter in the /layers operations included in this API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82d53934-01d6-4f3e-9f07-d03607dadbbd"
            }
          ]
        },
        {
          "id": "faf07f78-5745-4316-8de5-8b72698adbb8",
          "name": "getLayerDateByLayerMetricDate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api-stg.nxtport.eu",
              "path": [
                "belair",
                "v1",
                "layers/:layerId/:metricId/:date"
              ],
              "variable": [
                {
                  "id": "date",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "layerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "metricId",
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
            "description": "This operation retrieves city layer data for the specified layer, metric and date combination. The date is passed in the following format: YYYYMMDD. The values for the layerId and metricId can be fetched from the /layers and /metrics operations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e352b49-ed50-4c3f-a884-a063ca14c439"
            }
          ]
        },
        {
          "id": "d58a4df6-6105-4e6c-864f-4e2b44cadff8",
          "name": "getLayerDateByLayerMetricDateHour",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api-stg.nxtport.eu",
              "path": [
                "belair",
                "v1",
                "layers/:layerId/:metricId/:date/:hour"
              ],
              "variable": [
                {
                  "id": "date",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "hour",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "layerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "metricId",
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
            "description": "This operation retrieves city layer data for the specified layer, metric and date combination. The date is passed in the following format: YYYYMMDD. The values for the layerId and metricId can be fetched from the /layers and /metrics operations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26cc5695-d410-4637-97ec-76d39e652cfb"
            }
          ]
        }
      ]
    }
  ]
}