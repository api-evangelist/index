{
  "info": {
    "name": "Hacker News Get the Item (story, comment, jobs, Ask HN, etc)",
    "_postman_id": "fa19075f-ef15-46c9-8bc9-cb9f2db39c88",
    "description": "Stories, comments, jobs, Ask HNs and even polls are just items. They're identified by their ids, which are unique integers.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Links",
      "item": [
        {
          "id": "64a06fcc-a1d4-43f6-98a0-b31dc6df2149",
          "name": "get",
          "request": {
            "url": "http://hacker-news.firebaseio.com/v0/updates.json",
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
            "description": "Get the changed items and profiles"
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "5b700efe-8762-43fb-9720-5ff4d47f6ac7"
            }
          ]
        },
        {
          "id": "76d00fdf-0aff-459a-9db6-cba6250245f3",
          "name": "get_top_stories",
          "request": {
            "url": "http://hacker-news.firebaseio.com/v0/topstories.json",
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
            "description": "Returns the current top 100 stories."
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "df6c7bce-421c-4d41-857a-8e7bcce49e24"
            }
          ]
        },
        {
          "id": "94c55060-5211-4ec4-a591-ae0b14e1c609",
          "name": "get_user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "hacker-news.firebaseio.com",
              "path": [
                "v0",
                "user/:id.json"
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
            "description": "Users are identified by case-sensitive ids"
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "51ad8056-9d3c-4b9c-b912-2c0611a70a91"
            }
          ]
        },
        {
          "id": "c3aa481e-1da6-4dc9-a773-174b9884a79c",
          "name": "get_max_item",
          "request": {
            "url": "http://hacker-news.firebaseio.com/v0/maxitem.json",
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
            "description": "Get the current largest item id"
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "b2d9e634-c0d3-40e3-9ac8-4130d45413de"
            }
          ]
        },
        {
          "id": "955d0415-a7cf-4046-90e3-e7f279410934",
          "name": "get_item",
          "request": {
            "url": {
              "protocol": "http",
              "host": "hacker-news.firebaseio.com",
              "path": [
                "v0",
                "item/:id.json"
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
            "description": "Stories, comments, jobs, Ask HNs and even polls are just items. They're identified by their ids, which are unique integers."
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "c33f136c-d9b1-493b-825b-f32f8b427e7c"
            }
          ]
        }
      ]
    }
  ]
}