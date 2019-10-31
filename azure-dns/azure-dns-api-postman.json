{
  "info": {
    "name": "Azure DNS API Zones List",
    "_postman_id": "0ae7b23f-15d2-452e-a0ba-427ca07666e5",
    "description": "Lists the DNS zones in all resource groups in a subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "zones",
      "item": [
        {
          "id": "d0128c5e-e743-46da-a8aa-a754a16d4b28",
          "name": "Zones_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Network/dnszones"
              ],
              "query": [
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
            "description": "Lists the DNS zones in all resource groups in a subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc5669e2-efc1-4ad7-84cb-484d4e8cb55c"
            }
          ]
        }
      ]
    }
  ]
}