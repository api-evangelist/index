{
  "info": {
    "name": "Quandl Get Databases",
    "_postman_id": "f70a953d-5062-4d32-b756-fb1b49c23268",
    "description": "You can search for specific databases on Quandl by making the following API request.  The API will return databases related to your query. Databases are returned 100 results at a time. You can page through the results using these parameters:",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Market Data",
      "item": [
        {
          "id": "11e9fce2-7de0-4323-ba07-e7e8042677aa",
          "name": "datasets.database_code.dataset_code.metadata.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.quandl.com",
              "path": [
                "api",
                "v3",
                "datasets/:database_code/:dataset_code/metadata"
              ],
              "query": [
                {
                  "key": "column_names",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "frequency",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "newest_available_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "oldest_available_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "premium",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "refreshed_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "database_code",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "dataset_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To download the metadata associated with any dataset object, append /metadata to your API request. (You can replace .csv with .json or .xml in this request). The following metadata fields are available in the response:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "805205ee-8530-4251-a70d-9c57d567b495"
            }
          ]
        },
        {
          "id": "67ec068f-1f7c-4299-8d4a-f14bf58decaf",
          "name": "datasets.database_code.dataset_code.data.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.quandl.com",
              "path": [
                "api",
                "v3",
                "datasets/:database_code/:dataset_code/data"
              ],
              "query": [
                {
                  "key": "collapse",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "column_index",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Cumulative",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "end_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "order",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Row-on-row",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "rows",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Start",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "transform",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "database_code",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "dataset_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To download the data in a dataset, simply append /data to the Quandl code in your API request. (You can replace .csv with .json or .xml in this request). If you request CSV, only the data you requested will be returned.  If you request JSON or XML, both data and input parameters will be returned. You can customize the dataset object being returned by adding various optional parameters to your query. Available parameters are tabulated below: If a datapoint for time t is denoted as y[t] and the transformed data as y???[t], the available transformations are defined as below: y[0] in the above table refers to the starting date for the API call, i.e., the date specified by start_date= or rows=, NOT the starting date of the underlying dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28fedcb2-1308-4d49-9096-b39e8b1b775e"
            }
          ]
        },
        {
          "id": "b074af63-92fc-4a53-b9d9-c28b8b255037",
          "name": "datasets.database_code.dataset_code.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.quandl.com",
              "path": [
                "api",
                "v3",
                "datasets/:database_code/:dataset_code"
              ],
              "query": [
                {
                  "key": "collapse",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "column_index",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "end_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "exclude_column_names",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "order",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "rows",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "transform",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "database_code",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "dataset_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can download both data and metadata in a single call, using the following API request. (You can replace .json with .csv or .xml in this request.  If you use .csv, only data will be returned.). In this call, you can customize the dataset object being returned, exactly as in the /data request above."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ff259dd-9974-4a5d-a600-fc3b08d36f1c"
            }
          ]
        },
        {
          "id": "c53b6992-3047-407b-9dd4-1365b6582b8e",
          "name": "datasets.get",
          "request": {
            "url": "http://www.quandl.com/api/v3/datasets?database_code=%7B%7D&page=%7B%7D&per_page=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can search for individual datasets on Quandl by making the following API request.  The API will return datasets related to your query, as well as datasets that belong to databases related to your query.  Datasets are returned 100 results at a time. You can page through the results using these parameters:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7844225b-ef14-4ddd-b1ff-83797fb78e3a"
            }
          ]
        },
        {
          "id": "64b98da8-5f92-4568-b160-f48742e0fb1d",
          "name": "databases.database_code.data.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.quandl.com",
              "path": [
                "api",
                "v3",
                "databases/:database_code/data"
              ],
              "query": [
                {
                  "key": "download_type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "database_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can download all the data in a premium database in a single call, by appending /data to your database request. You can specify whether you want the entire history, or merely the last day???s worth of updates, by setting the correct query parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53d57042-b1f3-4203-861c-5666d4fd54b7"
            }
          ]
        },
        {
          "id": "4897239e-ac48-4cec-a107-31987109171c",
          "name": "databases.database_code.codes.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.quandl.com",
              "path": [
                "api",
                "v3",
                "databases/:database_code/codes"
              ],
              "variable": [
                {
                  "id": "database_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can download a list of all dataset codes in a database in a single call, by appending /codes to your database request. The call will return a ZIP file containing a CSV."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8b03a4f-5798-4927-9294-cb99ae1cd002"
            }
          ]
        },
        {
          "id": "e8182228-9db2-4b68-bfca-64f2dfbee853",
          "name": "databases.database_code.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.quandl.com",
              "path": [
                "api",
                "v3",
                "databases/:database_code"
              ],
              "variable": [
                {
                  "id": "database_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This call returns descriptive metadata for the specified database."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b1abc1b-4d8d-4966-bca9-a7f7d9d99637"
            }
          ]
        },
        {
          "id": "2c9a096e-b587-4fcb-9628-059109f21b90",
          "name": "databases.get",
          "request": {
            "url": "http://www.quandl.com/api/v3/databases?page=%7B%7D&per_page=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can search for specific databases on Quandl by making the following API request.  The API will return databases related to your query. Databases are returned 100 results at a time. You can page through the results using these parameters:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f654840-dccf-4583-8547-3a9f1c78e6ab"
            }
          ]
        }
      ]
    }
  ]
}