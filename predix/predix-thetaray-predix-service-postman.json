{
  "info": {
    "name": "Predix ThetaRay Predix Service Upload a file",
    "_postman_id": "49479a55-7c44-45b5-adea-53f238dd03c9",
    "description": "Upload a data file",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Proxy",
      "item": [
        {
          "id": "5bf3e4ea-e43c-401d-8c33-de700781249e",
          "name": "retrieveNewUsingGET",
          "request": {
            "url": "http://thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io/v1/proxy/analyses",
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
            "description": "Get list of Analyses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c4de5bf-6d8f-452a-a93f-21b57f6d5849"
            }
          ]
        },
        {
          "id": "3761a6f6-dbf0-476b-bcec-c2755f22c9d1",
          "name": "retrieveReportUsingGET",
          "request": {
            "url": "http://thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io/v1/proxy/anomalies/report?analysisId=%7B%7D&dataSourceName=%7B%7D&fromAnomaly=%7B%7D&numOfTopFeatures=%7B%7D&toAnomaly=%7B%7D",
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
            "description": "Retrieves Anomalies Report"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "414c09f8-889e-4aa8-b414-ddc23aee1a91"
            }
          ]
        },
        {
          "id": "f9265fdf-212c-48e6-9503-507ada82eae5",
          "name": "getClustersReportUsingGET",
          "request": {
            "url": "http://thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io/v1/proxy/clusters/report?analysisId=%7B%7D&dataSourceName=%7B%7D&filterOnlyUsedToCluster=%7B%7D&fromAnomaly=%7B%7D&toAnomaly=%7B%7D&withMinClusterSize=%7B%7D",
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
            "description": "Get Clusters report"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92024252-5d09-4d53-81e4-c6ddb79d5776"
            }
          ]
        },
        {
          "id": "2440a0bd-1ec4-42ff-9c77-baf4ace9a8a4",
          "name": "getDataSourcesUsingGET",
          "request": {
            "url": "http://thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io/v1/proxy/datasources/datasources",
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
            "description": "Get list of all Data Sources"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1619ffef-6438-48f0-8254-5d0d8087547b"
            }
          ]
        },
        {
          "id": "a69431ba-19d6-456d-b650-62cbc5d1a4af",
          "name": "processUsingPOST",
          "request": {
            "url": "http://thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io/v1/proxy/datasources/process?dataSourceName=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "file",
                  "value": "{}",
                  "disabled": false,
                  "description": "The file"
                }
              ]
            },
            "description": "Upload a data file"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "527cf37b-3fef-4da4-a572-d79c6ec13f35"
            }
          ]
        }
      ]
    }
  ]
}