{
  "info": {
    "name": "Pinboard Get User Secret",
    "_postman_id": "7568259b-b2d3-415d-914c-499a2c9068ba",
    "description": "Get the secret RSS token (allows viewing user's private RSS feeds).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Posts",
      "item": [
        {
          "id": "f9f3aeec-74a0-48cb-a611-edb4ae0cfe55",
          "name": "posts.update.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/update",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the most recent time a bookmark was added, updated or deleted. Use this before calling posts/all to see if the data has changed since the last fetch."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c03754fc-0cc2-4ce8-a665-fab4ae332e80"
            }
          ]
        },
        {
          "id": "ff331f65-6a4f-4b52-b5d1-637646ac1d46",
          "name": "posts.add.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/add",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Add a new bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "796d460d-a5eb-4bfc-908c-c23597b750a0"
            }
          ]
        },
        {
          "id": "885152be-0706-4824-bf35-b4e5d9079645",
          "name": "posts.delete.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/delete",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12408d24-4cd3-4393-a5cf-aac253febdec"
            }
          ]
        },
        {
          "id": "357ac55b-e148-4b0c-afdb-2f294f73e8d0",
          "name": "posts.get.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/get",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns one or more posts on a single day matching the arguments. If no date or url is given, date of most recent bookmark will be used."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6132c8e3-5510-4789-bd12-56a6a551937f"
            }
          ]
        },
        {
          "id": "ba1a09da-1e3e-4d13-935e-c8471c9d3577",
          "name": "posts.dates.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/dates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of dates with the number of posts at each date."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3bdaad1-c11c-4cf2-99e8-21e59bf76026"
            }
          ]
        },
        {
          "id": "636e9f45-f5a2-4407-b9c2-70ef50928a3f",
          "name": "posts.recent.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/recent?count=count&tag=tag",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the user's most recent posts, filtered by tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d49d5acc-b216-4944-90d4-95cd1e2a3a65"
            }
          ]
        },
        {
          "id": "e9294a38-b708-4178-a5c8-053a9d153507",
          "name": "posts.all.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/all?fromdt=fromdt&meta=meta&results=results&start=start&tag=tag&todt=todt",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all bookmarks in the user's account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "446a0422-38d0-48f3-92d1-cbbd20c6bb45"
            }
          ]
        },
        {
          "id": "1d7a06aa-b3fb-4d45-852a-dd4bac36f228",
          "name": "posts.suggest.get",
          "request": {
            "url": "http://api.pinboard.in/v1/posts/suggest?format=format&url=url",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of popular tags and recommended tags for a given URL. Popular tags are tags used site-wide for the url; recommended tags are drawn from the user's own tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f90bcc2-dec3-474a-b27e-911b321c1f6c"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "65f91438-f82a-4fa6-be59-7a316e23a901",
          "name": "tags.get.get",
          "request": {
            "url": "http://api.pinboard.in/v1/tags/get?format=format",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a full list of the user's tags along with the number of times they were used."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94877135-db74-4bbf-bf80-13942dc909af"
            }
          ]
        },
        {
          "id": "8dcf25fb-20e2-46ea-9e32-2b31c0aea56a",
          "name": "tags.delete.get",
          "request": {
            "url": "http://api.pinboard.in/v1/tags/delete",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an existing tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "969fdbaf-2414-431f-b823-28a04d0fc024"
            }
          ]
        },
        {
          "id": "3022b80b-1eb2-4a4c-a975-fb3328f558c1",
          "name": "tags.rename.get",
          "request": {
            "url": "http://api.pinboard.in/v1/tags/rename",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Rename an tag, or fold it in to an existing tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72adb979-04f2-4f43-9967-c0137ab7b881"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "97bb9cd3-8f0d-414e-9104-f3e00c8d41f1",
          "name": "user.secret.get",
          "request": {
            "url": "http://api.pinboard.in/v1/user/secret",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the secret RSS token (allows viewing user's private RSS feeds)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98fc95e5-789d-49f5-8d1f-003900273afb"
            }
          ]
        }
      ]
    }
  ]
}