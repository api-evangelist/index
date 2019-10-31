swagger: "2.0"
x-collection-name: Hacker News
x-complete: 1
info:
  title: Hacker News
  description: phacker-news-apip
  version: 1.0.0
host: hacker-news.firebaseio.com
basePath: /v0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /updates.json:
    get:
      summary: Get the changed items and profiles
      description: Get the changed items and profiles
      operationId: get
      x-api-path-slug: updates-json-get
      responses:
        200:
          description: Successful response
      tags:
      - Links
      - Stories
      - Updates
  /topstories.json:
    get:
      summary: Returns the current top 100 stories.
      description: Returns the current top 100 stories.
      operationId: get_top_stories
      x-api-path-slug: topstories-json-get
      responses:
        200:
          description: Successful response
      tags:
      - Links
      - Stories
      - Top
  /user/{id}.json:
    get:
      summary: Users are identified by case-sensitive ids
      description: Users are identified by case-sensitive ids
      operationId: get_user
      x-api-path-slug: userid-json-get
      parameters:
      - in: path
        name: id
        description: User ID
      responses:
        200:
          description: Successful response
      tags:
      - Links
      - Stories
  /maxitem.json:
    get:
      summary: Get the current largest item id
      description: Get the current largest item id
      operationId: get_max_item
      x-api-path-slug: maxitem-json-get
      responses:
        200:
          description: Successful response
      tags:
      - Links
      - Stories
  /item/{id}.json:
    get:
      summary: Get the Item (story, comment, jobs, Ask HN, etc)
      description: Stories, comments, jobs, Ask HNs and even polls are just items.
        They're identified by their ids, which are unique integers.
      operationId: get_item
      x-api-path-slug: itemid-json-get
      parameters:
      - in: path
        name: id
        description: Item ID
      responses:
        200:
          description: Successful response
      tags:
      - Links
      - Stories