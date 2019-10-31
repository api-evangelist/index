{
  "info": {
    "name": "NSIDC Web Service Documentation Index Suggest search terms based on a partial query",
    "_postman_id": "9a520737-984d-4b94-8062-90f5f0be3842",
    "description": "In NSIDC Search and the Arctic Data Explorer, this endpoint is queried whenever the user types into the search terms box, and the returned suggestions are displayed in a dropdown beneath the search terms box. The q parameter and returned JSON follow the specifications of the OpenSearch Suggestions 1.0 extension.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Environment",
      "item": [
        {
          "id": "85aa6d2b-0e76-4960-bb74-1080924368a7",
          "name": "facets",
          "request": {
            "url": "http://nsidc.org/api/dataset/2/Facets?count=%7B%7D&endDate=%7B%7D&facetFilters=%7B%7D&searchTerms=%7B%7D&sortKeys=%7B%7D&source=%7B%7D&spatial=%7B%7D&startDate=%7B%7D&startIndex=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "In the NSIDC Search and Arctic Data Explorer interfaces, this endpoint is used in conjunction with /OpenSearch whenever a user submits a new search. Consequently, it has the same parameters as /OpenSearch."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2075b3d1-c37c-403a-a559-05d19d36a4a5"
            }
          ]
        },
        {
          "id": "288c4d95-ad80-4650-af3a-b03ffd4e5884",
          "name": "OpenSearch.get",
          "request": {
            "url": "http://nsidc.org/api/dataset/2/OpenSearch?count=%7B%7D&endDate=%7B%7D&facetFilters=%7B%7D&searchTerms=%7B%7D&sortKeys=%7B%7D&source=%7B%7D&spatial=%7B%7D&startDate=%7B%7D&startIndex=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint uses parameters from the OpenSearch 1.1 specification, as well as parameters from the OpenSearch Geo (1.0) and SRU (1.0) extensions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ddd8bc7-5a0d-4456-b208-eb79a7139478"
            }
          ]
        },
        {
          "id": "e74a708d-5551-4ae6-b9b3-537b1b4b790f",
          "name": "OpenSearchDescription.get",
          "request": {
            "url": "http://nsidc.org/api/dataset/2/OpenSearchDescription",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the web interface of NSIDC's data search engine"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76136cd3-c359-4fac-be2f-e049f76d5fc8"
            }
          ]
        },
        {
          "id": "8fa3f0d8-151b-4826-a001-7e708fb219e1",
          "name": "getSuggest",
          "request": {
            "url": "http://nsidc.org/api/dataset/2/suggest?q=%7B%7D&source=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "In NSIDC Search and the Arctic Data Explorer, this endpoint is queried whenever the user types into the search terms box, and the returned suggestions are displayed in a dropdown beneath the search terms box. The q parameter and returned JSON follow the specifications of the OpenSearch Suggestions 1.0 extension."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "741e6360-ad84-47d0-a6f6-bccd07fa9d70"
            }
          ]
        }
      ]
    }
  ]
}