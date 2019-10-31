{
  "info": {
    "name": "Zencoder API Get Output Details",
    "_postman_id": "e83bc72c-339e-439a-9b44-fdabcede70df",
    "description": "Get Output Details",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "ee28ec81-56e8-4ff4-a3d0-181f5e473fe5",
          "name": "getAccount",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account?api_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Account Details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1ae26d8-8444-4bf5-98a0-004b8177a5f8"
            }
          ]
        },
        {
          "id": "9978993c-2173-4c07-ad78-6102578914fd",
          "name": "postAccount",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account?email=%7B%7D&password=%7B%7D&password_confirmation=%7B%7D&terms_of_service=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an Account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1516acd-ce0b-478c-969e-c3d88c3dd998"
            }
          ]
        },
        {
          "id": "fb4ebbad-e31a-4c50-9dcb-49b8a0feae40",
          "name": "putAccountIntegration",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account/integration?api_key=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Integration Mode"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3bd98ed-a818-49c3-92f2-12d538a460a5"
            }
          ]
        },
        {
          "id": "c3877f79-8469-4933-9c8c-13c9bf3b39da",
          "name": "putAccountLive",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account/live",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Integration Mode - Live"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68094d0b-dc2e-4a68-ab11-7b99e352ee18"
            }
          ]
        }
      ]
    },
    {
      "name": "Inputs",
      "item": [
        {
          "id": "cbdf1517-0d75-482c-bfe4-d57aae1c93a8",
          "name": "getInupdatesInupdate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "inputs/:input_id"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "input_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Input Details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1627f445-b422-4a70-8d0d-d589097e5370"
            }
          ]
        },
        {
          "id": "34190d65-945f-4f84-bef2-9aa9f93b5836",
          "name": "getInupdatesInupdateProgress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "inputs/:input_id/progress"
              ],
              "variable": [
                {
                  "id": "input_id",
                  "value": "input_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The return will contain one or more of the following keys: state, current_event, current_event_progress and progress."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9ad6bc7-a3f3-4def-9df6-2f2500ebfc12"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "409d669b-960e-4ccf-8486-04c783f1308f",
          "name": "getJobs",
          "request": {
            "url": "http://app.zencoder.com/api/v2/jobs?api_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A list of jobs can be obtained by sending an HTTP GET request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f9a565d-0536-4c27-b18f-0671b62eb03b"
            }
          ]
        },
        {
          "id": "7ddd2b00-984b-4da9-9c0e-fa806e63c8e9",
          "name": "postJobs",
          "request": {
            "url": "http://app.zencoder.com/api/v2/jobs?api_key=%7B%7D&Encoding Settings=%7B%7D&input=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Encoding jobs are created by sending an HTTP POST request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "017e54cb-0e6a-4a4d-ad79-672c2e100c01"
            }
          ]
        },
        {
          "id": "2b0baefc-62a5-4a84-b4ec-4bbfc97906f3",
          "name": "getJobsJob",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "jobs/:job_id"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Get Job Details",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "job_id",
                  "value": "job_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Job Details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c28cd8fe-a671-4744-b50c-9541455ba953"
            }
          ]
        },
        {
          "id": "9f5912fc-9202-4bf4-b5e1-fe0393952e47",
          "name": "putJobsJobCancel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "jobs/:job_id/cancel"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "job_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "If you wish to cancel a job that has not yet finished processing you may send a request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "898b8e4a-11ed-4a28-990e-1b2a12a662af"
            }
          ]
        },
        {
          "id": "f47af5b1-84dd-4b4f-8084-e83dd09a84e0",
          "name": "putJobsJobFinish",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "jobs/:job_id/finish"
              ],
              "variable": [
                {
                  "id": "job_id",
                  "value": "job_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Finishes the input on a Live streaming job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b43a090c-79ab-4d95-8a01-6f083c1748dd"
            }
          ]
        },
        {
          "id": "ab79f7ef-2809-472f-bfb1-1e1f8daa86a7",
          "name": "getJobsJobProgress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "jobs/:job_id/progress"
              ],
              "variable": [
                {
                  "id": "job_id",
                  "value": "job_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The return will contain one or more of the following keys: state, input, outputs, and progress."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "917295c4-8387-4eb6-8265-3cf0c9f71fa8"
            }
          ]
        },
        {
          "id": "950eedfa-33eb-4f98-8486-b6e42e83d62d",
          "name": "putJobsJobResubmit",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "jobs/:job_id/resubmit"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "job_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "If a job has failed processing you may request that it be attempted again."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ecc2fdb4-ffed-4cd0-b988-04913dff873e"
            }
          ]
        }
      ]
    },
    {
      "name": "Outputs",
      "item": [
        {
          "id": "6d49b2e4-8a72-4f83-88bd-a86dcb9ca60d",
          "name": "getOutupdatesOutupdateProgress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "outputs/:output_id/progress"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "output_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The return will contain one or more of the following keys: state, current_event, current_event_progress and progress."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "423ec7f7-0ff3-4015-878e-f46b40aca372"
            }
          ]
        }
      ]
    },
    {
      "name": "Reports",
      "item": [
        {
          "id": "c7cb77b6-d399-462a-9d39-314df35451dc",
          "name": "getReportsAll",
          "request": {
            "url": "http://app.zencoder.com/api/v2/reports/all?api_key=%7B%7D&from=%7B%7D&grouping=%7B%7D&to=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Usage for VOD & Live"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ccc1f191-dd2b-46f9-8424-01383440da83"
            }
          ]
        },
        {
          "id": "b7043707-2bf1-4258-aaed-3b047542a829",
          "name": "getReportsLive",
          "request": {
            "url": "http://app.zencoder.com/api/v2/reports/live?api_key=%7B%7D&from=%7B%7D&grouping=%7B%7D&to=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Usage for Live"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a760587-27ed-4451-bb04-af76d4a21a5f"
            }
          ]
        },
        {
          "id": "ff9cc3a3-9b2e-4065-bdc1-c6b60d5c34a1",
          "name": "getReportsMinutes",
          "request": {
            "url": "http://app.zencoder.com/api/v2/reports/minutes?api_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Minutes Used"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11326da7-cc85-4252-afbd-bc02b1e9af57"
            }
          ]
        },
        {
          "id": "e01f15a1-4220-4186-9ab1-866601f125c0",
          "name": "getReportsVod",
          "request": {
            "url": "http://app.zencoder.com/api/v2/reports/vod?api_key=%7B%7D&from=%7B%7D&grouping=%7B%7D&to=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Usage for VOD"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3695641f-1e74-4005-b96e-2c899d4066c1"
            }
          ]
        }
      ]
    },
    {
      "name": "V2",
      "item": [
        {
          "id": "a80b53b2-3a14-4aa3-ac4d-552195615506",
          "name": "getV2OutupdatesOutupdate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "v2/outputs/:output_id"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "output_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Output Details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95516359-0e9d-4116-8a82-a13df97f2f8c"
            }
          ]
        }
      ]
    }
  ]
}