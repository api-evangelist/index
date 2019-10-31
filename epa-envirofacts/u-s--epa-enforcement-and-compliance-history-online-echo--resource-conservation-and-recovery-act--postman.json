{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Resource Conservation and Recovery Act  Resource Conservation and Recovery Act (RCRA) Metadata Service",
    "_postman_id": "c0cbc73b-6215-4652-a1ec-2bc867129808",
    "description": "Returns the JSON Object Name and ColumnId for usage with the qcolumns parameter for get_qid, get_facility_info and other service endpoints.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "77e87945-5378-441e-91df-bb1769d3a4b8",
      "name": "based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-a-comma-sepated-va",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rcra_rest_services.get_download?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Based on the QID obtained from a get_facilities or get_facility_info query, return a comma sepated vaule (CSV) file of the facilities found."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "81177159-a50f-4924-b294-d69b0733ce3c"
        }
      ]
    },
    {
      "id": "98cd5ada-00b4-49f9-a27f-7ca5ddbc0594",
      "name": "validates-query-search-parameters-and-returns-query-identifier---use-the-responseset-parameter-to-se",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rcra_rest_services.get_facilities?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Validates query search parameters and returns query identifier.  Use the responseset parameter to set the page size"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "5aa13e35-584e-4b3d-a98e-b587f8f3f0a1"
        }
      ]
    },
    {
      "id": "bf30b6a3-cd6e-4c0d-ad0b-83a1aeb7ea73",
      "name": "returns-either-an-array-of-facilities-or-an-array-of-clusters-that-meet-the-specified-search-criteri",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rcra_rest_services.get_facility_info?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns either an array of Facilities or an array of Clusters that meet the specified search criteria."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "b5e2d535-faf7-490d-8072-5124545f5851"
        }
      ]
    },
    {
      "id": "28e51bd9-4945-4107-b531-827576fc883d",
      "name": "based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-geojson-of-the-fac",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rcra_rest_services.get_geojson?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Based on the QID obtained from a get_facilities or get_facility_info query, return GeoJSON of the facilities found."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "e0d02468-aa29-469a-a685-e7fbebb23e0a"
        }
      ]
    },
    {
      "id": "6afa5cef-84c4-41ac-81e4-16a47c9d604e",
      "name": "based-on-the-qid-obtained-from-a-clustered-get-facility-info-query-download-cluster-facility-informa",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rcra_rest_services.get_info_clusters?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Based on the QID obtained from a clustered get_facility_info query, download cluster facility information as either a CSV or GEOJSON file."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "fe76f51f-9996-4c49-96ce-a5a2aa0f2e74"
        }
      ]
    },
    {
      "id": "737ea544-3f2f-4d83-a9ba-51b8c76394a9",
      "name": "the-purpose-of-the-get-map-service-is-to-display-facility-coordinates-and-facility-clusters-related-",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rcra_rest_services.get_map?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "The purpose of the GET_MAP service is to display facility coordinates and facility clusters related to a get_facilities facility query. Currently, the maximum number of coordinates returned is 500. GET_MAP performs automatic clustering at the state, county, and zip code levels to maximize the number of coordinates returned."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "557984f7-eb92-4309-8e49-6a3c332224ea"
        }
      ]
    },
    {
      "id": "5613142e-4289-4769-af4b-1ae146fe6097",
      "name": "get-qid-is-passed-with-a-query-id-corresponding-to-a-previously-run-get-facilities-query--it-then-re",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rcra_rest_services.get_qid?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "GET_QID is passed with a query ID corresponding to a previously run get_facilities query. It then returns a Facility object containing all matching facilities. The main purpose of GET_QID is for large querysets that contain multiple pages (responsesets) of output. GET_QID allows for pagination and for the selection and sorting of columns."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "6b4a111f-70bb-4819-90b8-f772d7fd8768"
        }
      ]
    },
    {
      "id": "1b87bd5c-2a9d-4be7-88b7-be5db846c28a",
      "name": "returns-the-json-object-name-and-columnid-for-usage-with-the-qcolumns-parameter-for-get-qid-get-faci",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rcra_rest_services.metadata?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns the JSON Object Name and ColumnId for usage with the qcolumns parameter for get_qid, get_facility_info and other service endpoints."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "2b738f28-879d-4f31-b3ca-af66a8364b7b"
        }
      ]
    }
  ]
}