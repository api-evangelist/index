{
  "info": {
    "name": "Azure Scheduler API Jobs List Job History",
    "_postman_id": "e167491f-7aa8-433c-8ed3-af599e46bb04",
    "description": "Lists job history.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "jobs",
      "item": [
        {
          "id": "f27913a3-b322-48d2-b957-43512dd3ab9e",
          "name": "Jobs_ListJobHistory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Scheduler/jobCollections/:jobCollectionName/jobs/:jobName/history"
              ],
              "query": [
                {
                  "key": "$filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$skip",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$top",
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
                  "id": "jobCollectionName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "jobName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists job history"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39f139ad-83d6-4e5e-a3e6-df3d4704bad6"
            }
          ]
        }
      ]
    }
  ]
}