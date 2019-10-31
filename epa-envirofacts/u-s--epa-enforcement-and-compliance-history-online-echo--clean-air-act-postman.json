{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Clean Air Act Clean Air Act Metadata Service",
    "_postman_id": "62dfff26-d908-49d9-9553-5036ec668540",
    "description": "Returns the JSON Object Name and ColumnId for usage with the qcolumns parameter for get_qid, get_facility_info and other service endpoints.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "95779203-03e8-4751-88ee-7ae2ec07e5f0",
      "name": "based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-a-comma-sepated-va",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/air_rest_services.get_download?No Name=%7B%7D&output=%7B%7D",
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
          "id": "c3be5da3-7db3-4a55-987c-63d9e0e650e2"
        }
      ]
    },
    {
      "id": "07924bd0-340a-4c17-902c-972abcaa04e9",
      "name": "validates-query-search-parameters-and-returns-query-identifier---use-the-responseset-parameter-to-se",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/air_rest_services.get_facilities?No Name=%7B%7D&output=%7B%7D",
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
          "id": "b6947447-f2b8-4418-be12-36fb754018e7"
        }
      ]
    },
    {
      "id": "f69c3768-de69-4274-b8e1-8949cc58cd93",
      "name": "returns-either-an-array-of-facilities-or-an-array-of-clusters-that-meet-the-specified-search-criteri",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/air_rest_services.get_facility_info?No Name=%7B%7D&output=%7B%7D",
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
          "id": "467e9f76-fa43-4b13-ab20-ec6128ae4fa4"
        }
      ]
    },
    {
      "id": "258caa7b-c198-4d7d-97c7-7e96af6651b7",
      "name": "based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-geojson-of-the-fac",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/air_rest_services.get_geojson?No Name=%7B%7D&output=%7B%7D",
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
          "id": "b78c5642-f794-4893-8f7c-c3247d0d2bca"
        }
      ]
    },
    {
      "id": "6c4a7dd2-f27b-4f84-ba32-0f01e5ac0301",
      "name": "based-on-the-qid-obtained-from-a-clustered-get-facility-info-query-download-cluster-facility-informa",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/air_rest_services.get_info_clusters?No Name=%7B%7D&output=%7B%7D",
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
          "id": "b6b6baa9-fa30-4f55-92d5-3b396f9a7d63"
        }
      ]
    },
    {
      "id": "2380bbc5-0ed6-402c-83d1-f52334b62ff0",
      "name": "the-purpose-of-the-get-map-service-is-to-display-facility-coordinates-and-facility-clusters-related-",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/air_rest_services.get_map?No Name=%7B%7D&output=%7B%7D",
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
          "id": "7b301359-a317-46b0-bd5e-9621ac685ca8"
        }
      ]
    },
    {
      "id": "c258192b-4302-44d5-bf6e-95bb970b2b70",
      "name": "get-qid-is-passed-with-a-query-id-corresponding-to-a-previously-run-get-facilities-query--it-then-re",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/air_rest_services.get_qid?No Name=%7B%7D&output=%7B%7D",
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
          "id": "21e86e94-173f-43e9-b2aa-1816872ab59f"
        }
      ]
    },
    {
      "id": "f0f9d8c7-7653-47db-945b-2fd744989261",
      "name": "returns-the-json-object-name-and-columnid-for-usage-with-the-qcolumns-parameter-for-get-qid-get-faci",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/air_rest_services.metadata?No Name=%7B%7D&output=%7B%7D",
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
          "id": "573f9f4b-1eda-424b-a8b1-aae583bfeec5"
        }
      ]
    }
  ]
}