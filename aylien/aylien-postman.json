{
  "info": {
    "name": "Aylien List histograms",
    "_postman_id": "2b098c3b-dd15-4c91-8b34-e50bfffbb346",
    "description": "For the numerical metadata that the News API gathers (such as word counts or social shares for example), you can use the histograms endpoint to access and display this information. As this endpoint does not return actual stories, the results you are given will not count towards your story allowance provided by your subscription, so you can effectively query this endpoint free of charge.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "News",
      "item": [
        {
          "id": "efc41a91-de22-403d-82e5-ff513250293c",
          "name": "listStories",
          "request": {
            "url": "http://api.newsapi.aylien.com/api/v1/stories?No Name=%7B%7D",
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
            "description": "The stories endpoint is used to return stories based on parameters you set in your query. The News API crawler gathers articles in near real-time and stores information about them, or metadata. Below you can see all of the query parameters, which you can use to narrow down your query."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cb3e23b-bab8-4292-a8ee-bdd21643f31e"
            }
          ]
        },
        {
          "id": "1aac2f59-bee2-4c0d-a68f-d5b2e20b86cb",
          "name": "listRelatedStories",
          "request": {
            "url": "http://api.newsapi.aylien.com/api/v1/related_stories?No Name=%7B%7D",
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
            "description": "This endpoint is used for finding semantically similar stories based on the parameters you provide as inputs. For example, if you want to find stories similar to a Tweet or any text extract you input, the related stories endpoint will analyze the entities present and the meaning of the text, and find stories with a similar meaning. The maximum number of related stories returned is 100."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7467dc0-4239-4890-9d64-d0dfb56134be"
            }
          ]
        },
        {
          "id": "cdef0fe1-b759-4a77-9914-ff3df22cad23",
          "name": "listRelatedStoriesAsPost",
          "request": {
            "url": "http://api.newsapi.aylien.com/api/v1/related_stories?No Name=%7B%7D",
            "method": "POST",
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
            "description": "This endpoint is used for finding semantically similar stories based on the parameters you provide as inputs. For example, if you want to find stories similar to a Tweet or any text extract you input, the related stories endpoint will analyze the entities present and the meaning of the text, and find stories with a similar meaning. The maximum number of related stories returned is 100."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc74ee88-7ad8-4b37-a1d5-eb9747dd1ac1"
            }
          ]
        },
        {
          "id": "bbc7ea7d-9a42-4d4c-b1af-d80c6af587cc",
          "name": "listCoverages",
          "request": {
            "url": "http://api.newsapi.aylien.com/api/v1/coverages?No Name=%7B%7D",
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
            "description": "The coverages endpoint allows you to understand the reach a document has had. For example, you can track the coverage of a press release or a Tweet based on how many times it has been mentioned in stories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0791402c-52e8-4122-ae60-1c02d4b65037"
            }
          ]
        },
        {
          "id": "9af7a765-4136-4248-8bb2-11fff0f4e46a",
          "name": "listCoveragesAsPost",
          "request": {
            "url": "http://api.newsapi.aylien.com/api/v1/coverages?No Name=%7B%7D",
            "method": "POST",
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
            "description": "The coverages endpoint allows you to understand the reach a document has had. For example, you can track the coverage of a press release or a Tweet based on how many times it has been mentioned in stories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11855332-28a5-42ee-9b4e-be843d5ad541"
            }
          ]
        },
        {
          "id": "f0c84015-55ec-4a3d-82fe-f790d932412f",
          "name": "listAutocompletes",
          "request": {
            "url": "http://api.newsapi.aylien.com/api/v1/autocompletes?No Name=%7B%7D",
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
            "description": "The autocompletes endpoint a string of characters provided to it, and then returns suggested terms that are the most likely full words or strings. The terms returned by the News API are based on parameters the type parameters you can see below. For example, if you provide the autocompletes endpoint with the term `New York C` and select the type `dbpedia_resources`, the API will return links to the DBpedia resources `New_York_City`, `New_York_City_Subway`, `New_York_City_Police_Department`, and so on."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c6cac94-c953-4ad8-8013-2ede93f8668d"
            }
          ]
        },
        {
          "id": "ad426e17-3c60-41c4-b429-ca11c5f847c5",
          "name": "listTimeSeries",
          "request": {
            "url": "http://api.newsapi.aylien.com/api/v1/time_series?No Name=%7B%7D",
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
            "description": "The time series endpoint allows you to track information contained in stories over time. This information can be anything from mentions of a topic or entities, sentiment about a topic, or the volume of stories published by a source, to name but a few. The full list of parameters is given below. Using the [Date Math Syntax](https://newsapi.aylien.com/docs/working-with-dates), you can easily set your query to return information from any time period, from the current point in time to when the News API started collecting stories. The returned information can be rounded to a time also specified by you, for example by setting the results into hourly, daily, or weekly data points."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "523bd849-acfc-4a5a-b880-5ee35751a220"
            }
          ]
        },
        {
          "id": "d1be84ab-160d-4171-91a6-b2599235d6a0",
          "name": "listTrends",
          "request": {
            "url": "http://api.newsapi.aylien.com/api/v1/trends?No Name=%7B%7D",
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
            "description": "The trends endpoint allows you to identify the most-mentioned entities, concepts and keywords relevant to your query. For example, this endpoint allows you to set parameters like a time period, a subject category, or an entity, and your request will return the most mentioned entities or keywords that are mentioned in relation to your query."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ffe0b71c-0137-4896-b0e7-5e9d57ef3269"
            }
          ]
        },
        {
          "id": "bd3d0542-2912-4fc6-8b92-4e4e3da11034",
          "name": "listHistograms",
          "request": {
            "url": "http://api.newsapi.aylien.com/api/v1/histograms?No Name=%7B%7D",
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
            "description": "For the numerical metadata that the News API gathers (such as word counts or social shares for example), you can use the histograms endpoint to access and display this information. As this endpoint does not return actual stories, the results you are given will not count towards your story allowance provided by your subscription, so you can effectively query this endpoint free of charge."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c0fed6b-5011-4961-bb54-b93eb4750c6e"
            }
          ]
        }
      ]
    }
  ]
}