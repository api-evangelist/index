{
  "info": {
    "name": "Azure Virtual Network API Network Interfaces Get Virtual Machine Scale Set Network Interface",
    "_postman_id": "8713aeab-c72a-4e90-a678-2ca0e29338fe",
    "description": "Get the specified network interface in a virtual machine scale set.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "network interfaces",
      "item": [
        {
          "id": "139e3ad9-9824-4fc1-937f-5d4f54b57e36",
          "name": "NetworkInterfaces_GetVirtualMachineScaleSetNetworkInterface",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/microsoft.Compute/virtualMachineScaleSets/:virtualMachineScaleSetName/virtualMachines/:virtualmachineIndex/networkInterfaces/:networkInterfaceName"
              ],
              "query": [
                {
                  "key": "$expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "api-version",
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
                  "id": "networkInterfaceName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "virtualmachineIndex",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "virtualMachineScaleSetName",
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
            "description": "Get the specified network interface in a virtual machine scale set"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5addd62-b96b-4bea-93b3-fba16ff36ef7"
            }
          ]
        }
      ]
    }
  ]
}