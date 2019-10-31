{
  "info": {
    "name": "U.S. EPA Enforcement and Compliance History Online (ECHO) - Clean Water Act (CWA) Rest Services ECHO WBD Name Lookup Service",
    "_postman_id": "1b992373-6548-4a49-9b6c-d7af4ea57cd3",
    "description": "USGS Watershed Boundary Dataset (WBD) Code lookup based on a supplied WBD Name and Watershed Level",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "e04de3d2-2312-4fd4-b684-c3c40307d08a",
      "name": "based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-geojson-of-the-fac",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/cwa_rest_services.get_download?No Name=%7B%7D&output=%7B%7D&qcolumns=%7B%7D",
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
          "id": "be7b594a-d3ee-4e31-865b-580f82e4ff60"
        }
      ]
    },
    {
      "id": "57effa3f-b1f5-418d-8137-abddc0b8e58e",
      "name": "validates-query-search-parameters-and-returns-query-identifier---use-the-responseset-parameter-to-se",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/cwa_rest_services.get_facilities?No Name=%7B%7D&output=%7B%7D&qcolumns=%7B%7D",
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
          "id": "4a813c53-2f5e-4f3e-b3a4-6ced5c1d048e"
        }
      ]
    },
    {
      "id": "abecf8b0-a366-4bf0-b167-46a224c64422",
      "name": "returns-either-an-array-of-facilities-or-an-array-of-clusters-that-meet-the-specified-search-criteri",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/cwa_rest_services.get_facility_info?No Name=%7B%7D&output=%7B%7D&qcolumns=%7B%7D",
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
          "id": "71bd6d24-edc6-4dd1-a72b-1444d1212881"
        }
      ]
    },
    {
      "id": "4924162c-7170-441e-a420-d63bdec2afc0",
      "name": "based-on-the-qid-obtained-from-a-get-facilities-or-get-facility-info-query-return-a-comma-sepated-va",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/cwa_rest_services.get_geojson?No Name=%7B%7D&output=%7B%7D&qcolumns=%7B%7D",
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
          "id": "124e811c-6ceb-4109-94ac-392dbd1cf620"
        }
      ]
    },
    {
      "id": "09e73249-ca74-4cf5-b321-f28853c3546a",
      "name": "based-on-the-qid-obtained-from-a-clustered-get-facility-info-query-download-cluster-facility-informa",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/cwa_rest_services.get_info_clusters?No Name=%7B%7D&output=%7B%7D",
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
          "id": "dc2dbf9f-b2be-4dc9-969c-a1e661cb86bf"
        }
      ]
    },
    {
      "id": "e6856b35-ddc5-45ab-85c2-c7d64b363c26",
      "name": "the-purpose-of-the-get-map-service-is-to-display-facility-coordinates-and-facility-clusters-related-",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/cwa_rest_services.get_map?No Name=%7B%7D&output=%7B%7D",
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
          "id": "0ac599e1-b253-4980-b2ea-2ff8739bd285"
        }
      ]
    },
    {
      "id": "19819237-9f41-4cfe-aaf0-095527ed16c1",
      "name": "get-qid-is-passed-with-a-query-id-corresponding-to-a-previously-run-get-facilities-query--it-then-re",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/cwa_rest_services.get_qid?No Name=%7B%7D&output=%7B%7D&qcolumns=%7B%7D",
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
          "id": "04a17ef8-4014-4e4d-acba-a141bda5a1a2"
        }
      ]
    },
    {
      "id": "31b381ad-e964-4cbe-b535-c2b6300ec8f5",
      "name": "returns-the-json-object-name-and-columnid-for-usage-with-the-qcolumns-parameter-for-get-qid-get-faci",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/cwa_rest_services.metadata?No Name=%7B%7D&output=%7B%7D",
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
          "id": "be11fec4-d960-4819-92a2-b74298fec0ce"
        }
      ]
    },
    {
      "id": "8f255a36-dfc3-491f-9cd3-b0af4bf3483b",
      "name": "returns-the-epa-standard-indian-tribes-and-native-alaskan-villages-tribal-id-and-tribe-name-",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.bp_tribes?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns the EPA Standard Indian Tribes and Native Alaskan Villages tribal_id and tribe_name."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "eb588288-6bd4-4466-be33-416e6dd072c9"
        }
      ]
    },
    {
      "id": "d449a17a-763b-4785-8a97-b65535d22b06",
      "name": "look-up-clean-water-act-parameter-codes-and-descriptions-in-the-integrated-compliance-information-sy",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.cwa_parameters?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Look up Clean Water Act parameter codes and descriptions in the Integrated Compliance Information System - National Pollutant Discharge Elimination System (ICIS-NPDES) by code or term."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "2f668af4-e7aa-4535-b5e4-f6017bf91c4b"
        }
      ]
    },
    {
      "id": "d21ff79b-df86-46eb-9f5a-d681c9ec5534",
      "name": "ECHO CWA Pollutants Lookup Service",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.cwa_pollutants?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "ECHO CWA Pollutants Lookup Service"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "ba1d4531-6043-44ac-89c9-133d108c9e21"
        }
      ]
    },
    {
      "id": "ffb879b3-5bf3-4d77-885d-faf04f63f7bd",
      "name": "look-up-federal-agency-code",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.federal_agencies?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Look up Federal Agency Code"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "624cfe03-6b79-4eb5-9dad-43e0ef76f928"
        }
      ]
    },
    {
      "id": "29f55eeb-0d0f-4010-b90b-f8305d8eb112",
      "name": "returns-the-icis-npdes-compliance-monitoring-type-code-and-description-",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.icis_inspection_types?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns the ICIS NPDES Compliance Monitoring Type Code and Description."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "3916c05a-d143-4cd0-83d8-f6390ff10dae"
        }
      ]
    },
    {
      "id": "2f107caf-e135-47af-8895-c7de910090af",
      "name": "returns-the-icis-law-section-descriptions-",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.icis_law_sections?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns the ICIS Law Section Descriptions."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "89e3f639-984f-4748-a501-a5166b141c0e"
        }
      ]
    },
    {
      "id": "00a2ea12-eb40-4f84-8f7e-53d338c250e7",
      "name": "ECHO NAICS Codes Lookup Service",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.naics_codes?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "ECHO NAICS Codes Lookup Service"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "1c5e235a-c86f-4399-a191-3bc2b800aea4"
        }
      ]
    },
    {
      "id": "d4366a64-a09c-42bd-b436-2ac1746b3342",
      "name": "icis-limit-parameter-code-and-name-lookup-based-on-the-supply-of-a-partial-parameter-name--npdes--na",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.npdes_parameters?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "ICIS Limit Parameter Code and Name lookup based on the supply of a partial parameter name. (NPDES = National Pollutant Discharge Elimination System)"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "2f46284e-c0f7-4a83-bbe7-4b4c5677653e"
        }
      ]
    },
    {
      "id": "d079f6b0-86c4-413f-a7a7-21a178b1ee7a",
      "name": "usgs-watershed-boundary-dataset-wbd-name-lookup-based-on-a-supplied-wbd-code-and-watershed-level",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.wbd_code_lu?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "USGS Watershed Boundary Dataset (WBD) Name lookup based on a supplied WBD Code and Watershed Level"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "925ea8f1-c84b-47a0-ae76-09d1cfa1bc29"
        }
      ]
    },
    {
      "id": "37bf8e7b-df35-4c3f-a82f-ff318f277d92",
      "name": "usgs-watershed-boundary-dataset-wbd-code-lookup-based-on-a-supplied-wbd-name-and-watershed-level",
      "request": {
        "url": "http://ofmpub.epa.gov/echo/rest_lookups.wbd_name_lu?No Name=%7B%7D&output=%7B%7D",
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "USGS Watershed Boundary Dataset (WBD) Code lookup based on a supplied WBD Name and Watershed Level"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "76868f3c-5600-4423-abd4-899c35db0877"
        }
      ]
    }
  ]
}