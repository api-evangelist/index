{
  "info": {
    "name": "Azure Container Service API Container Services List By Resource Group",
    "_postman_id": "1d7d921b-b38a-42d5-8262-7f42a4b5870d",
    "description": "Gets a list of container services in the specified subscription and resource group. The operation returns properties of each container service including state, orchestrator, number of masters and agents, and FQDNs of masters and agents.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "containers",
      "item": [
        {
          "id": "2802e0ae-33ad-46f5-b9b7-f0eede8ac605",
          "name": "ContainerServices_ListByResourceGroup",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ContainerService/containerServices"
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
            "description": "Gets a list of container services in the specified subscription and resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "094fd601-180f-4d4b-8803-2bb34abaff3d"
            }
          ]
        }
      ]
    }
  ]
}