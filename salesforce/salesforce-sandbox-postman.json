{
  "info": {
    "name": "Salesforce Sandbox Get Version Search",
    "_postman_id": "170a5f82-050e-441c-9141-17961557eaeb",
    "description": "Executes the specified SOSL search. The search string must be URL-encoded.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Folder",
      "item": [
        {
          "id": "aace0d23-ef0e-4daa-8109-a64f0aecfd49",
          "name": "get",
          "request": {
            "url": "http://na14.salesforce.com/services/data/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists summary information about each Salesforce version currently available, including the version, label, and a link to each version's root."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b73e1aa-4415-44d9-b7eb-8072653793e2"
            }
          ]
        }
      ]
    },
    {
      "name": "Version",
      "item": [
        {
          "id": "8e6fef85-15a6-4490-978e-154496bd47e6",
          "name": "getVersion",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version"
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
            "body": {
              "mode": "raw"
            },
            "description": "Lists available resources for the specified API version, including resource name and URI."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aaa1a26a-fed0-4902-9f25-bc92c9919378"
            }
          ]
        },
        {
          "id": "b648ad96-afb3-4048-a25c-1e250913c301",
          "name": "getVersionSobjects",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects"
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
            "body": {
              "mode": "raw"
            },
            "description": "Lists the available objects and their metadata for your organization's data. In addition, it provides the organization encoding, as well as maximum batch size permitted in queries. For more information, see Internationalization and Character Sets (http://www.salesforce.com/us/developer/docs/api/Content/implementation_considerations.htm#sforce_api_other_internationalization)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85cf29a1-2d16-4443-9386-8a8ca92cc601"
            }
          ]
        },
        {
          "id": "102b0399-0f83-4f83-bbc3-fee9624e0085",
          "name": "getVersionSobjectsSobject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/:sobject"
              ],
              "variable": [
                {
                  "id": "sobject",
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
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the metadata for an object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b503ff88-7ed4-4df6-bcb5-c1be2116619a"
            }
          ]
        },
        {
          "id": "098b0f72-5cf5-48d9-8220-01c9e4f4802d",
          "name": "postVersionSobjectsSobject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/:sobject"
              ],
              "variable": [
                {
                  "id": "sobject",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3dbc4ccf-e28f-4410-a68d-676c82ea2fae"
            }
          ]
        },
        {
          "id": "39b0ca52-ae15-4799-a5d9-cd9b1b38c2f5",
          "name": "getVersionSobjectsSobjectDescribe",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/:sobject/describe"
              ],
              "variable": [
                {
                  "id": "sobject",
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
            "body": {
              "mode": "raw"
            },
            "description": "Completely describes the individual metadata at all levels for the specified object. For example, this can be used to retrieve the fields, URLs, and child relationships for the Account object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8c55415-10ed-470c-bd2a-e78d8a0da3a8"
            }
          ]
        },
        {
          "id": "95e5d781-a29b-4720-aaa5-2c1df261e696",
          "name": "getVersionSobjectsSobject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/:sobject/:id"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sobject",
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
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves individual records for an object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cc7691c-4d84-4e6a-85cf-a76531f69f6a"
            }
          ]
        },
        {
          "id": "b92a8dd9-972c-4837-a37b-01ff6c6ef416",
          "name": "deleteVersionSobjectsSobject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/:sobject/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sobject",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a record."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b42b427-ccac-4238-9739-def27cbd735c"
            }
          ]
        },
        {
          "id": "29d53683-7d32-4cc6-b4b3-6a052d410ff2",
          "name": "getVersionSobjectsSobjectBlobfield",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/:sobject/:id/:blobField"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "blobField",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sobject",
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
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the specified blob field from an individual record. Because blob fields contain binary data, you can't use JSON or XML to retrieve this data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42805d34-b922-473a-a8a6-5d701c121554"
            }
          ]
        },
        {
          "id": "35e193ff-a029-4248-b6b2-c3f9f6feaa40",
          "name": "getVersionSobjectsUserPassword",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/User/:id/password"
              ],
              "variable": [
                {
                  "id": "id",
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
            "body": {
              "mode": "raw"
            },
            "description": "Gets password expiration status for a given user. The session must have permission to access the given user password information, otherwise an error response is returned."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4adda65-1714-442d-a6f0-d3c032c61178"
            }
          ]
        },
        {
          "id": "beef6d60-52f1-4814-ae32-da228579b95b",
          "name": "postVersionSobjectsUserPassword",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/User/:id/password"
              ],
              "variable": [
                {
                  "id": "id",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Changes the password for a given user ID. The new password must conform to the password policies for the organization, otherwise you will get an error response. You can only change one password per request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d75674ca-a2d3-462b-b2b3-293270ea663b"
            }
          ]
        },
        {
          "id": "cfc0f05d-95c5-4dd7-8aca-2fb106b0179e",
          "name": "deleteVersionSobjectsUserPassword",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/sobjects/User/:id/password"
              ],
              "variable": [
                {
                  "id": "id",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Resets an user password. Salesforce will reset the user password to an auto-generated password, which will be returned in the response."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07fe4d39-a313-4534-af9e-3a5ffa734de1"
            }
          ]
        },
        {
          "id": "9af0c210-0829-4c7b-8581-aa55670c5c84",
          "name": "getVersionQuery",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/query"
              ],
              "query": [
                {
                  "key": "q",
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
            "body": {
              "mode": "raw"
            },
            "description": "Executes the specified SOQL query. If the initial query returns only part of the results, the end of the response will contain a field called nextRecordsUrl. In such cases, use the resource {version}/query/{id} to request the next batch of records and repeat until all records have been retrieved."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83b2ba62-5f85-4b96-9068-7c5008b21cba"
            }
          ]
        },
        {
          "id": "83c15462-8b13-49c0-a89c-79e086f1ca8e",
          "name": "getVersionQuery",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/query/:id"
              ],
              "variable": [
                {
                  "id": "id",
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
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the remaining SOQL query results using the identifier within the field \"nextRecordsUrl\" value (i.e. \"nextRecordsUrl\" : \"/services/data/v24.0/query/01gD0000002HU6KIAW-2000\") located at the end of the initial query results. Requests the next batch of records and you could repeat (using the corresponding identifier) until all records have been retrieved."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "edaafa09-c4d9-48ac-a2bc-6420d0822f95"
            }
          ]
        },
        {
          "id": "e1da87af-3b92-4d69-abcc-9ccc7b388bf8",
          "name": "getVersionSearch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "na14.salesforce.com",
              "path": [
                "services",
                "data",
                ":version/search"
              ],
              "query": [
                {
                  "key": "q",
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
            "body": {
              "mode": "raw"
            },
            "description": "Executes the specified SOSL search. The search string must be URL-encoded."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96b36613-4e80-4e31-b723-8e2b3f55d7da"
            }
          ]
        }
      ]
    }
  ]
}