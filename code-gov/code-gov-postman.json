{
  "info": {
    "name": "Code.gov Get the version of this API",
    "_postman_id": "3f6a997d-1e85-483a-b188-d6efd1ffa685",
    "description": "Get the version of this api.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Code",
      "item": [
        {
          "id": "bbb68633-b351-43aa-9ef0-dc0da8c71b47",
          "name": "getRepos",
          "request": {
            "url": "http://api.code.gov/repos?agency.acronym=%7B%7D&agency.name=%7B%7D&agency.website=%7B%7D&contact.email=%7B%7D&contact.name=%7B%7D&date.created=%7B%7D&date.lastModified=%7B%7D&from=%7B%7D&laborHours=%7B%7D&languages=%7B%7D&name=%7B%7D&organization=%7B%7D&permissions.licenses.name=%7B%7D&permissions.usageType=%7B%7D&q=%7B%7D&size=%7B%7D&status=%7B%7D&tags=%7B%7D&vcs=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get list of repositories indexed by Code.gov."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "577de0e1-f184-4422-8173-236099b6ad94"
            }
          ]
        },
        {
          "id": "f183980c-c362-4247-937f-7dd6f851b286",
          "name": "getReposRepo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.code.gov",
              "path": [
                "repos/:repoId"
              ],
              "variable": [
                {
                  "id": "repoId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the information of a specific repository index with the passed repoId."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "018dee64-0b44-4888-bca6-04128e34e6b9"
            }
          ]
        },
        {
          "id": "cd8300dc-659e-4ea2-b68e-91e364b03bf9",
          "name": "getTerms",
          "request": {
            "url": "http://api.code.gov/terms?from=%7B%7D&size=%7B%7D&term=%7B%7D&term_type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of terms that were extracted from the repositories indexed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3caa0f6-907f-48d7-8a20-fe29a711c31d"
            }
          ]
        },
        {
          "id": "61c5182f-44e3-4cce-a4b5-bb5720e16e4c",
          "name": "getRepo",
          "request": {
            "url": "http://api.code.gov/repo.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the json schema for a repo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ba7dd03-0d0d-46d6-8ff4-7a1e776910ba"
            }
          ]
        },
        {
          "id": "1ed91984-4951-47ef-ada4-85d058132182",
          "name": "getStatus.json",
          "request": {
            "url": "http://api.code.gov/status.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of agencies with their Federal Source Code Policy compliance status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98097445-5b4a-4383-82ca-f3aeddf17f9f"
            }
          ]
        },
        {
          "id": "d2685591-f7ef-4be4-992b-cf7a54b1afa9",
          "name": "getStatus",
          "request": {
            "url": "http://api.code.gov/status",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get an html page rendering the agencies status from status.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14d69008-1f46-464a-a64c-0dbf8a82201d"
            }
          ]
        },
        {
          "id": "bbed9346-5b5d-4aac-9a6c-448e7bed73fe",
          "name": "getStatusAgencynameIssues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.code.gov",
              "path": [
                "status/:agencyName/issues"
              ],
              "variable": [
                {
                  "id": "agencyName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of issues for a particular agency. These issues are grouped by software repository."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0dd0dfb3-5fe8-4118-9d34-efb271c6d1b3"
            }
          ]
        },
        {
          "id": "c240a5f6-4d6d-4e98-820c-8d6949d00df3",
          "name": "getStatusAgencynameFetched",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.code.gov",
              "path": [
                "status/:agencyName/fetched"
              ],
              "variable": [
                {
                  "id": "agencyName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists out all repositories that have been indexed for a given agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "634e891e-29c9-4647-b460-c2d14a3e8117"
            }
          ]
        },
        {
          "id": "4ffcca8d-5896-4cfe-ac32-081240bf1c9c",
          "name": "getStatusAgencynameDiscovered",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.code.gov",
              "path": [
                "status/:agencyName/discovered"
              ],
              "variable": [
                {
                  "id": "agencyName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of repos by agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d929fbe-e227-40c3-b016-6244738246d5"
            }
          ]
        },
        {
          "id": "48402ef9-da4b-4aa3-89b1-66105a633e35",
          "name": "getVersion",
          "request": {
            "url": "http://api.code.gov/version",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the version of this api."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24bb1848-8af8-46d8-810e-65b8860696d1"
            }
          ]
        }
      ]
    },
    {
      "name": "Agencies",
      "item": [
        {
          "id": "d3317b45-84e5-4021-b697-8e6dd12e5e38",
          "name": "getAgencies",
          "request": {
            "url": "http://api.code.gov/agencies?from=%7B%7D&size=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of agencies."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0bab0d27-9185-4718-b7f5-5da8e842fbd1"
            }
          ]
        }
      ]
    },
    {
      "name": "Languages",
      "item": [
        {
          "id": "715911ef-ba17-41eb-b36e-33581441da3d",
          "name": "getLanguages",
          "request": {
            "url": "http://api.code.gov/languages?from=%7B%7D&size=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This returns a list of the programming languages that are used in the indexed code inventory. When a repo is index the programming language is extracted written to a file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cc8579c-3abe-420a-b83b-36b95cfc7eec"
            }
          ]
        }
      ]
    }
  ]
}