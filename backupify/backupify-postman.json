{
  "info": {
    "name": "Backupify Provides information about the currently authenticated vendor user",
    "_postman_id": "04ea0dd6-7c2e-4b9b-8b6f-e9511ab271de",
    "description": "Provides information about the currently authenticated vendor user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "V1",
      "item": [
        {
          "id": "cb04a5f9-da4b-4ff6-806a-5ec0692d3bdb",
          "name": "getV1AuthenticateCustomer",
          "request": {
            "url": "http://api.backupify.com/v1/authenticate_customer",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer Access Token granted for customer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "A simple method to test authentication of a customer access token.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65c86198-3a21-4f2e-8a99-a99b134a2169"
            }
          ]
        },
        {
          "id": "368d1248-c6b6-45f5-a569-94d326326f34",
          "name": "getV1BackupInstancesBackupInstanceEndpointsEndpointName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.backupify.com",
              "path": [
                "v1/backup_instances/:backup_instance_id/endpoints/:endpoint_name"
              ],
              "variable": [
                {
                  "id": "backup_instance_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "endpoint_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer Access Token granted from client credentials authorizing vendor to perform action",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "You can only retrieve endpoints for backup_instances you have access to"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d649c3df-744e-4f6a-ac2e-a4b9dd761777"
            }
          ]
        },
        {
          "id": "872031c6-437c-4d8d-ad61-64540bdd610d",
          "name": "getV1BackupInstancesBackupInstanceEndpointsEndpointNameRecords",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.backupify.com",
              "path": [
                "v1/backup_instances/:backup_instance_id/endpoints/:endpoint_name/records"
              ],
              "variable": [
                {
                  "id": "backup_instance_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "endpoint_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer Access Token granted from client credentials authorizing vendor to perform action",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "You can only retrieve records for endpoints that belong to backup_instances you have access to. Records are returned in ascending order (by id), with a default of 20 per page. Links to the next, previous, first, and last pages can be found in the response headers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97839dd9-bcca-48c6-ba17-350c2fd94376"
            }
          ]
        },
        {
          "id": "7f0a7065-49b8-4161-8407-a46a93d4e169",
          "name": "getV1BackupInstancesBackupInstanceEndpointsEndpointNameRecordsRecord",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.backupify.com",
              "path": [
                "v1/backup_instances/:backup_instance_id/endpoints/:endpoint_name/records/:record_id"
              ],
              "variable": [
                {
                  "id": "backup_instance_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "endpoint_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "record_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer Access Token granted from client credentials authorizing vendor to perform action",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "You can only retrieve records for endpoints of backup_instances you have access to"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a2b7dfd-a735-4941-8a3c-7550d328df21"
            }
          ]
        },
        {
          "id": "f7ef9b19-256a-4754-90b5-99dfbf231761",
          "name": "getV1BackupInstancesBackupInstanceEndpointsEndpointNameRecordsRecordBlob",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.backupify.com",
              "path": [
                "v1/backup_instances/:backup_instance_id/endpoints/:endpoint_name/records/:record_id/blob"
              ],
              "variable": [
                {
                  "id": "backup_instance_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "endpoint_name",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "record_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Access-Token",
                "value": "{}",
                "description": "Access Token granted from client credentials authorizing vendor to perform action",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the blob associated with the specified record for the specified endpoint and backup_instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3782c67e-8b6a-43ba-83aa-75d76d0bb5a4"
            }
          ]
        },
        {
          "id": "bed853e5-9d76-4a0e-984b-3e635486cfe6",
          "name": "getV1Customers",
          "request": {
            "url": "http://api.backupify.com/v1/customers",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer Access Token granted from client credentials authorizing vendor to perform action",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Requires Access Token granted from client credentials. Records are returned in ascending order (by id), with a default of 20 per page. Links to the next, previous, first, and last pages can be found in the response headers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1abe11cf-9eff-48a0-a9ce-61469aa2e0f4"
            }
          ]
        },
        {
          "id": "13fd3af1-c005-4cd7-93ab-f3b08b7c7e50",
          "name": "postV1Customers",
          "request": {
            "url": "http://api.backupify.com/v1/customers",
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer Access Token granted from client credentials authorizing vendor to perform action",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "customer[email]",
                  "value": "{}",
                  "disabled": false,
                  "description": "Email address associated with the customer"
                },
                {
                  "key": "customer[name]",
                  "value": "{}",
                  "disabled": false,
                  "description": "Vendor provided ID uniquely identifying customer"
                }
              ]
            },
            "description": "Create a new customer instance identified by the given {name} identifier."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab0ac4a2-d0a7-439e-9310-68d52e720f8a"
            }
          ]
        },
        {
          "id": "b1f45a0b-a740-4bac-94d2-2f7ef006846e",
          "name": "getV1CustomersCustomer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.backupify.com",
              "path": [
                "v1/customers/:customer_id"
              ],
              "variable": [
                {
                  "id": "customer_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer Access Token granted from client credentials authorizing vendor to perform action",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Requires Access Token granted from client credentials."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97056941-ffe5-47d0-ab52-701b39f9887b"
            }
          ]
        },
        {
          "id": "b7cde162-b5ec-456e-9394-a6cc8c98bb8f",
          "name": "putV1CustomersCustomer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.backupify.com",
              "path": [
                "v1/customers/:customer_id"
              ],
              "variable": [
                {
                  "id": "customer_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer Access Token granted from client credentials authorizing vendor to perform action",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "customer[name]",
                  "value": "{}",
                  "disabled": false,
                  "description": "Vendor provided ID uniquely identifying customer"
                }
              ]
            },
            "description": "Update a customer instance identified by the given customer_id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c7018fc-acf6-4209-94f1-190e3159739f"
            }
          ]
        },
        {
          "id": "4d16d874-6c64-4985-8ba9-cbe96ed64709",
          "name": "getV1CustomersCustomerBackupInstances",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.backupify.com",
              "path": [
                "v1/customers/:customer_id/backup_instances"
              ],
              "variable": [
                {
                  "id": "customer_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer Access Token granted from client credentials authorizing vendor to perform action",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "It is only possible to retrieve backup_instances for customers you are authorized to access. Records are returned in ascending order (by id), with a default of 20 per page. Links to the next, previous, first, and last pages can be found in the response headers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0346a28e-6424-497e-8a12-78c745661365"
            }
          ]
        },
        {
          "id": "c1956209-39c3-453d-87ad-47e7b30010e9",
          "name": "getV1VendorsMe",
          "request": {
            "url": "http://api.backupify.com/v1/vendors/me",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer Access Token granted from client credentials authorizing vendor to perform action",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Provides information about the currently authenticated vendor user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4342afb-7563-49cf-b646-f71b112076bf"
            }
          ]
        }
      ]
    }
  ]
}