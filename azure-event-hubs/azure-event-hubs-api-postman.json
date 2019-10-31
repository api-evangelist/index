{
  "info": {
    "name": "Azure Event Hubs API Consumer Groups List All",
    "_postman_id": "69d06771-d0fa-4b87-b277-bce259700b6d",
    "description": "Gets all the consumer groups in a Namespace. An empty feed is returned if no consumer group exists in the Namespace.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "consumer groups all",
      "item": [
        {
          "id": "77093d28-6340-4878-9032-fc1659852f9a",
          "name": "ConsumerGroups_ListAll",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.EventHub/namespaces/:namespaceName/eventhubs/:eventHubName/consumergroups"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "namespaceName",
                  "value": "namespaceName",
                  "type": "string"
                },
                {
                  "id": "eventHubName",
                  "value": "eventHubName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the consumer groups in a Namespace"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07f99390-2ec0-4c40-b5c6-5a79146b4c9f"
            }
          ]
        }
      ]
    }
  ]
}