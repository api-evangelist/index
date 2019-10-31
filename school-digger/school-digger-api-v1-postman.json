{
  "info": {
    "name": "School Digger API V1 Returns a detailed record for one school",
    "_postman_id": "f335559a-a0af-4d7a-ba70-7f42fe0cd80f",
    "description": "Retrieve a school record from the SchoolDigger database",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "5740b71f-8ba5-4e2b-8c1c-e951251ce0aa",
      "name": "Districts_GetAllDistricts",
      "request": {
        "url": "http://api.schooldigger.com/v1/districts?appID=%7B%7D&appKey=%7B%7D&boundaryAddress=%7B%7D&boxLatitudeNW=%7B%7D&boxLatitudeSE=%7B%7D&boxLongitudeNW=%7B%7D&boxLongitudeSE=%7B%7D&city=%7B%7D&distanceMiles=%7B%7D&isInBoundaryOnly=%7B%7D&nearLatitude=%7B%7D&nearLongitude=%7B%7D&page=%7B%7D&perPage=%7B%7D&q=%7B%7D&sortBy=%7B%7D&st=%7B%7D&zip=%7B%7D",
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
        "description": "Search the SchoolDigger database for districts. You may use any combination of criteria as query parameters."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "fcdd7ce5-790f-435b-a741-c132b7bc15a0"
        }
      ]
    },
    {
      "id": "eff0f8ca-3392-48bd-b97a-2d5d28f9f6e4",
      "name": "Districts_GetDistrict",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.schooldigger.com",
          "path": [
            "v1/districts/:id"
          ],
          "query": [
            {
              "key": "appID",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "appKey",
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
        "description": "Retrieve a single district record from the SchoolDigger database"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "ec6283c0-f66a-4e96-af22-efd6e21ada1f"
        }
      ]
    },
    {
      "id": "efd6f6b2-6c3b-448d-af8f-d92d43d07d90",
      "name": "v1.rankings.districts.st.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.schooldigger.com",
          "path": [
            "v1/rankings/districts/:st"
          ],
          "query": [
            {
              "key": "appID",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "appKey",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "page",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "perPage",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "year",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "st",
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
        "description": "Returns a SchoolDigger district ranking list"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "76761422-d063-4c65-8873-39b62a191d3f"
        }
      ]
    },
    {
      "id": "f55f8f55-75d2-499d-b887-5237cc46d58b",
      "name": "v1.rankings.schools.st.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.schooldigger.com",
          "path": [
            "v1/rankings/schools/:st"
          ],
          "query": [
            {
              "key": "appID",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "appKey",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "level",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "page",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "perPage",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "year",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "st",
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
        "description": "Returns a SchoolDigger school ranking list"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "169d318d-4e0a-4c7e-8617-dbb69846a8f8"
        }
      ]
    },
    {
      "id": "b15eaa25-9383-47b6-8c60-1a833274218c",
      "name": "Schools_GetAllSchools",
      "request": {
        "url": "http://api.schooldigger.com/v1/schools?appID=%7B%7D&appKey=%7B%7D&boundaryAddress=%7B%7D&boxLatitudeNW=%7B%7D&boxLatitudeSE=%7B%7D&boxLongitudeNW=%7B%7D&boxLongitudeSE=%7B%7D&city=%7B%7D&distanceMiles=%7B%7D&districtID=%7B%7D&isCharter=%7B%7D&isInBoundaryOnly=%7B%7D&isMagnet=%7B%7D&isTitleI=%7B%7D&isTitleISchoolwide=%7B%7D&isVirtual=%7B%7D&level=%7B%7D&nearLatitude=%7B%7D&nearLongitude=%7B%7D&page=%7B%7D&perPage=%7B%7D&q=%7B%7D&sortBy=%7B%7D&st=%7B%7D&zip=%7B%7D",
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
        "description": "Search the SchoolDigger database for schools. You may use any combination of criteria as query parameters."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "d3dcea3c-6993-4824-8d0a-27e192fa7424"
        }
      ]
    },
    {
      "id": "45ae8978-5c00-4e0f-aa0b-614af723395c",
      "name": "Schools_GetSchool",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.schooldigger.com",
          "path": [
            "v1/schools/:id"
          ],
          "query": [
            {
              "key": "appID",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "appKey",
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
        "description": "Retrieve a school record from the SchoolDigger database"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "1b30492a-9ecc-4890-a890-6daa82a90652"
        }
      ]
    }
  ]
}