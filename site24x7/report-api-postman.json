{
  "info": {
    "name": "Report API Response SLA",
    "_postman_id": "8df3af09-2a29-4bad-9411-5b85f84f090c",
    "description": "Request Example",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "0e5a1eb1-a455-4e7e-aeaf-24e2cdf042a0",
          "name": "get-custom-report-settings",
          "request": {
            "url": "http://www.site24x7.com./customize_report",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Custom Report Settings."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "91eac40f-0ced-43fd-97c5-3fad93187bc7"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "34a8f1c2-fa40-4116-9c7a-89f0ab117909"
            }
          ]
        },
        {
          "id": "497e5e93-f1af-4de1-bcdb-4c445f160b82",
          "name": "busy-hours-report",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/busy_hours/:monitor_id?period=:report_period_constants&segment_type=:segment_types"
              ],
              "variable": [
                {
                  "id": "monitor_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "report_period_constants",
                  "value": "report_period_constants",
                  "type": "string"
                },
                {
                  "id": "segment_types",
                  "value": "segment_types",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Request Example"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "24ebc75b-c666-4771-ac20-a1c1439bef04"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "8d602e79-a645-48f4-854d-8887d874c232"
            }
          ]
        },
        {
          "id": "f83d62ce-d316-47a0-a5d3-1ddaeabc0165",
          "name": "get-outage-details",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/outage?period=:report_period_constants"
              ],
              "query": [
                {
                  "key": "period",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "report_period_constants",
                  "value": "report_period_constants",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtain the actual down period and the total down duration of your monitors for a specified duration of time."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "2a701a46-9863-4482-a138-57d4609adb08"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "19627231-6b4d-46fe-a945-7fe015d8fa32"
            }
          ]
        },
        {
          "id": "fdd044b1-876f-4234-a840-dd9d90ec51dd",
          "name": "get-outage-details-of-monitor-groups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/outage/group/:monitor_group_id?period=:report_period_constants"
              ],
              "variable": [
                {
                  "id": "monitor_group_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "report_period_constants",
                  "value": "report_period_constants",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtain the actual down period and the total down duration of your chosen monitor group during a selected duration of time."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "e2e89eeb-8080-492c-be9e-f38a3b90d979"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "b58c02f1-9ef2-48e5-87cd-12746f2b2a97"
            }
          ]
        },
        {
          "id": "6dcffbfd-2ec0-4dc6-8cf2-0f975f594ae9",
          "name": "delete-outage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/outage/:monitor_id/:outage_id"
              ],
              "variable": [
                {
                  "id": "monitor_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "outage_id",
                  "value": "outage_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete the faulty downtime alerts to reflect the actual available state of the monitor."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "80e24313-46d1-4450-8c49-ccb637987956"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "fb84fc87-ec09-40bd-b109-2666f60b2b9c"
            }
          ]
        },
        {
          "id": "50b15db1-8808-4a75-9110-ec9697306308",
          "name": "get-alarms-of-monitor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/alarm/:monitor_id?period=:report_period_constants"
              ],
              "variable": [
                {
                  "id": "monitor_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "report_period_constants",
                  "value": "report_period_constants",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtain the actual down, trouble and maintenance status of your configured monitors. Alert types"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "8fec9825-1099-468e-bdcc-c4d6c74929be"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "a3a5b40e-2376-4d20-8a5c-598a7c625ddc"
            }
          ]
        },
        {
          "id": "952fb243-081c-4bc4-8ec0-8f3646aa89c1",
          "name": "get-comments-for-a-monitor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/comments/:monitor_id?period=:report_period_constants"
              ],
              "variable": [
                {
                  "id": "monitor_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "report_period_constants",
                  "value": "report_period_constants",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all the comments for a monitor for the given duration."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "a10e2f40-f486-484f-9c51-71618df6159c"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "b50375be-94bc-4e77-aaa2-3e023ecda0fd"
            }
          ]
        },
        {
          "id": "f945be7f-b603-410c-9abd-7f47009a0de8",
          "name": "update-outage-comments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/comments/:monitor_id/:outage_id"
              ],
              "variable": [
                {
                  "id": "monitor_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "outage_id",
                  "value": "outage_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update the comment for a given monitor."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "d465bfd7-9564-4d7e-a353-f2c9be690974"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "35cda9e7-d709-4c27-ad57-85dd3063d70f"
            }
          ]
        },
        {
          "id": "247494ac-9711-4d72-a8a8-5ccff25e3812",
          "name": "delete-comment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/comments/:monitor_id/:outage_id?comment_time=:comment_id"
              ],
              "variable": [
                {
                  "id": "monitor_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "outage_id",
                  "value": "outage_id",
                  "type": "string"
                },
                {
                  "id": "comment_id",
                  "value": "comment_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an outage comment."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "ee5091bc-7a1a-4428-8794-a271bd6b69ac"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "e23e6ad5-32a0-4d9b-97fe-47e843d36297"
            }
          ]
        },
        {
          "id": "d3267ff8-e1cf-4ed5-a365-2f53dec0e80d",
          "name": "availability-summary-by-monitor-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/availability_summary/group/:group_id?period="
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Request Example"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "c8e4d448-7780-41cf-b793-083e81ce8f15"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "b6f755a9-c4b5-47e4-8ca5-6ecc75a51f63"
            }
          ]
        },
        {
          "id": "ba395f5b-0abf-4489-92fe-4a29db5233ea",
          "name": "availability-summary-for-all-monitors",
          "request": {
            "url": "http://www.site24x7.com./reports/availability_summary?period=?period=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Request Example"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "1d3e19ba-efee-4829-98ad-a76b257bcef4"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "788a6586-8fb5-4773-b5c0-73aad38511f0"
            }
          ]
        },
        {
          "id": "d5403dd8-6208-488d-883f-c792932d0cb0",
          "name": "summary-by-monitor-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/summary/group/:group_id?period="
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Request Example"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "36d325c5-57bb-4abd-8b7b-6a1ffcb2fa6a"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "356c49ac-d24c-41ac-a5ce-d54d4588f4f2"
            }
          ]
        },
        {
          "id": "b353aa5b-4a69-4f1d-a37b-96a0b645c2bb",
          "name": "summary-for-all-monitors",
          "request": {
            "url": "http://www.site24x7.com./reports/summary?period=?availability_percentage=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Request Example"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "acf25dae-b9a8-4e0b-ae86-f614875a8c7a"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "4fd3d777-f899-41d2-bc5d-b54530f866e1"
            }
          ]
        },
        {
          "id": "5e11b20f-c173-44b0-936e-c048e1ce14ae",
          "name": "health-trend-report-by-monitor-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/trend/group/:group_id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Request Example"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "82b42f2d-0d5c-486c-8e6a-57f058439767"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "702c5ef6-b4fd-4ca4-ada2-763f44a02c0b"
            }
          ]
        },
        {
          "id": "bd77dfea-49b4-4393-89af-c7de2343018e",
          "name": "health-trend-report-for-all-monitors",
          "request": {
            "url": "http://www.site24x7.com./reports/trend?period=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Request Example"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "a3b626c0-2548-450d-bfb6-92b17983942f"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "b5a622f4-0fe4-46e9-b122-cc87f5125c57"
            }
          ]
        },
        {
          "id": "0838ba2c-e183-422e-b04a-d4fd969734b0",
          "name": "top-n-report-by-monitor-and-attribute-type",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/top_n/:monitor_type/:attribute_name?limit=:N&period=:report_period_constants"
              ],
              "query": [
                {
                  "key": "period",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "monitor_type",
                  "value": "monitor_type",
                  "type": "string"
                },
                {
                  "id": "attribute_name",
                  "value": "attribute_name",
                  "type": "string"
                },
                {
                  "id": "N",
                  "value": "N",
                  "type": "string"
                },
                {
                  "id": "report_period_constants",
                  "value": "report_period_constants",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Request Example"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "c6f159f9-1c1f-4ff5-8e61-66695981bebe"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "16e4d596-86bc-4875-b7fb-da30f345e547"
            }
          ]
        },
        {
          "id": "76270770-bb6e-4570-98c4-6a3801e301b6",
          "name": "performance-report-by-monitor-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/performance/group/:group_id?period=3"
              ],
              "query": [
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Request Example"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "75d97c73-58e0-4316-a52d-1e4e1107898a"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "d405d2f7-b511-43ef-95ef-0cce78eff2c5"
            }
          ]
        },
        {
          "id": "7d4425af-009d-4ee6-aac7-4a5a0f533613",
          "name": "performance-report-of-all-monitors",
          "request": {
            "url": "http://www.site24x7.com./reports/performance?period=3?period=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Request Example"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "6df3ad3d-75b3-4be9-8b24-fcd3f00f1a4d"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "b55b91dc-9d63-4a6d-8b1f-a390efa0a29e"
            }
          ]
        },
        {
          "id": "fde4e5b4-0189-4742-90b3-74011b6416c6",
          "name": "response-sla",
          "request": {
            "url": "http://www.site24x7.com./reports/sla_reports/response?period=3",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Request Example"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "42b90019-b253-402e-8a57-e08b85655690"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "57604dfe-dcda-46c6-b574-4dc01f2f3148"
            }
          ]
        }
      ]
    }
  ]
}