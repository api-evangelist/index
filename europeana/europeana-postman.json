{
  "info": {
    "name": "Europeana translate a term to different languages",
    "_postman_id": "27c93aa9-5a2d-4d83-ae3e-4e17873088da",
    "description": "Translate a term to different languages.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Dataset",
      "item": [
        {
          "id": "a3a7fe79-7ced-4181-8900-080b076502d2",
          "name": "getDataset",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.europeana.eu",
              "path": [
                "v2",
                "dataset/:id.json"
              ],
              "query": [
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "wskey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a specific dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a2b994e-75c6-46a1-a40c-e38ef3e56820"
            }
          ]
        }
      ]
    },
    {
      "name": "Datasets",
      "item": [
        {
          "id": "764feb70-b197-4d36-b868-d604777172f7",
          "name": "listDatasets",
          "request": {
            "url": "http://www.europeana.eu/v2/datasets.json?callback=%7B%7D&countryCode=%7B%7D&edmDatasetName=%7B%7D&offset=%7B%7D&pagesize=%7B%7D&status=%7B%7D&wskey=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of europeana datasets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "def8e425-74ab-4873-ab87-b5a876f48d7f"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "682c99fa-e3d6-4777-b59d-c81d2d68058f",
          "name": "openSearch",
          "request": {
            "url": "http://www.europeana.eu/v2/opensearch.rss?count=%7B%7D&searchTerms=%7B%7D&startIndex=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Basic search function following the opensearch specification."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3eee305-af9b-4a11-a856-4cbde091b596"
            }
          ]
        },
        {
          "id": "f71242d7-468a-4878-b563-51b3171984cf",
          "name": "searchRecords",
          "request": {
            "url": "http://www.europeana.eu/v2/search.json?callback=%7B%7D&colourpalette=%7B%7D&cursor=%7B%7D&facet=%7B%7D&landingpage=%7B%7D&media=%7B%7D&profile=%7B%7D&qf=%7B%7D&query=%7B%7D&reusability=%7B%7D&rows=%7B%7D&sort=%7B%7D&start=%7B%7D&text_fulltext=%7B%7D&thumbnail=%7B%7D&wskey=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search for records."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72e4f960-6fd3-4d04-9453-7a128d0fe2fd"
            }
          ]
        },
        {
          "id": "758615a4-f069-4afa-a71c-60e392afd455",
          "name": "fieldTrip",
          "request": {
            "url": "http://www.europeana.eu/v2/search.rss?language=%7B%7D&limit=%7B%7D&offset=%7B%7D&profile=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Google fieldtrip formatted rss of selected collections."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "594e78e5-973d-4170-b876-7b7eb38a7b4f"
            }
          ]
        }
      ]
    },
    {
      "name": "Provider",
      "item": [
        {
          "id": "b55cf59f-1a3e-4f52-8072-9615436881de",
          "name": "getProvider",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.europeana.eu",
              "path": [
                "v2",
                "provider/:id.json"
              ],
              "query": [
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "wskey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a specific europeana provider."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "975ac1c3-2e5f-4412-932a-08eb0fa0bec2"
            }
          ]
        }
      ]
    },
    {
      "name": "Providers",
      "item": [
        {
          "id": "35c4e3d9-cc93-4412-aae4-3805f8ede6eb",
          "name": "listProviderDatasets",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.europeana.eu",
              "path": [
                "v2",
                "provider/:id/datasets.json"
              ],
              "query": [
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "wskey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of datasets provided by a specific provider."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3055822-72fd-4673-8adb-bc6606cbda31"
            }
          ]
        },
        {
          "id": "b5f95691-8078-4de7-9b97-2cc855706140",
          "name": "listProviders",
          "request": {
            "url": "http://www.europeana.eu/v2/providers.json?callback=%7B%7D&countryCode=%7B%7D&offset=%7B%7D&pagesize=%7B%7D&wskey=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of europeana data providers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bdae90c0-7044-460f-ad1f-999c29df04b0"
            }
          ]
        }
      ]
    },
    {
      "name": "Collections",
      "item": [
        {
          "id": "29e3d68b-6c7e-416e-a6c1-fad90ee985f8",
          "name": "getSingleRecordJson",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.europeana.eu",
              "path": [
                "v2",
                "record/:collectionId/:recordId.json"
              ],
              "query": [
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "hierarchytimeout",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "profile",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "wskey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "collectionId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "recordId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single record in json format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1425842-0188-412b-b74e-57f0fae9151e"
            }
          ]
        },
        {
          "id": "1a2386a2-67ca-483a-a9c3-9d696f24f73d",
          "name": "getSingleRecordJsonLD",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.europeana.eu",
              "path": [
                "v2",
                "record/:collectionId/:recordId.jsonld"
              ],
              "query": [
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "wskey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "collectionId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "recordId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get single record in json ld format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4587fef-94a4-416e-a749-fad56faff7f6"
            }
          ]
        },
        {
          "id": "ac643788-cbda-42ba-9362-1519710d1432",
          "name": "getSingleRecordRDF",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.europeana.eu",
              "path": [
                "v2",
                "record/:collectionId/:recordId.rdf"
              ],
              "query": [
                {
                  "key": "wskey",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "collectionId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "recordId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get single record in rdf format)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6713c366-e4f2-43bb-ac85-b5f5ce892661"
            }
          ]
        }
      ]
    },
    {
      "name": "Suggestions",
      "item": [
        {
          "id": "ac4000c0-b160-4d9e-ac15-1dc38c50e4c3",
          "name": "suggestions",
          "request": {
            "url": "http://www.europeana.eu/v2/suggestions.json?callback=%7B%7D&phrases=%7B%7D&query=%7B%7D&rows=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get autocompletion recommendations for search queries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c76ed0d1-df47-42ef-9351-954b2360eb05"
            }
          ]
        }
      ]
    },
    {
      "name": "Translations",
      "item": [
        {
          "id": "0d2a53a0-afcb-4da0-b237-4def9249ce29",
          "name": "translateQueryUsingGET",
          "request": {
            "url": "http://www.europeana.eu/v2/translateQuery.json?callback=%7B%7D&languageCodes=%7B%7D&profile=%7B%7D&term=%7B%7D&wskey=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Translate a term to different languages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d53f357-b9ca-42c6-b1b1-ec0d371f0d1e"
            }
          ]
        }
      ]
    }
  ]
}