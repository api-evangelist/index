{
  "info": {
    "name": "Instructure Canvas Appointment Groups API List user participants",
    "_postman_id": "d2bd58eb-f21f-4f4d-a7f9-24e203680399",
    "description": "List user participants.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Appointment",
      "item": [
        {
          "id": "560d745f-d08e-41c9-8f5b-b110428f1bec",
          "name": "list-appointment-groups",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/appointment_groups?context_codes=%5B%7B%7D%5D&include=%5B%7B%7D%5D&include_past_appointments=%7B%7D&scope=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List appointment groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b79d113e-1ea8-4d60-b0c6-49bd3af8cd8f"
            }
          ]
        },
        {
          "id": "4d0403f8-f1aa-4d70-8cba-e43e4ce45408",
          "name": "create-an-appointment-group",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/appointment_groups?appointment_group[context_codes=%5B%7B%7D%5D&appointment_group[description]=%7B%7D&appointment_group[location_address]=%7B%7D&appointment_group[location_name]=%7B%7D&appointment_group[max_appointments_per_participant]=%7B%7D&appointment_group[min_appointments_per_participant]=%7B%7D&appointment_group[new_appointments][X=%5B%7B%7D%5D&appointment_group[participants_per_appointment]=%7B%7D&appointment_group[participant_visibility]=%7B%7D&appointment_group[publish]=%7B%7D&appointment_group[sub_context_codes=%5B%7B%7D%5D&appointment_group[title]=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an appointment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9829a91-09b9-4306-8b20-9c11a25629b0"
            }
          ]
        },
        {
          "id": "ea9269e5-fe67-47f2-89bf-7237d3998000",
          "name": "get-a-single-appointment-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "appointment_groups/:id"
              ],
              "query": [
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single appointment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b073803e-71c8-4090-b13e-4a558d4cb0ee"
            }
          ]
        },
        {
          "id": "ac080b9a-0d42-41d5-a18e-85cc1b9014c2",
          "name": "update-an-appointment-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "appointment_groups/:id"
              ],
              "query": [
                {
                  "key": "appointment_group[context_codes",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[description]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[location_address]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[location_name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[max_appointments_per_participant]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[min_appointments_per_participant]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[new_appointments][X",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[participants_per_appointment]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[participant_visibility]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[publish]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[sub_context_codes",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[title]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update an appointment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "911e9481-444b-45c2-9db1-835d7e999f8c"
            }
          ]
        },
        {
          "id": "57570899-3854-41b3-8d13-f93bc7136d4d",
          "name": "delete-an-appointment-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "appointment_groups/:id"
              ],
              "query": [
                {
                  "key": "cancel_reason",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an appointment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37cc7f3a-9863-4a26-ad05-923b6d093d7d"
            }
          ]
        },
        {
          "id": "44d0e07e-7b82-42e7-ba40-332366937cfd",
          "name": "list-student-group-participants",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "appointment_groups/:id/groups"
              ],
              "query": [
                {
                  "key": "registration_status",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List student group participants."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49cea4e8-b5b3-4e69-997d-a8f8c53921c0"
            }
          ]
        },
        {
          "id": "6c39de7c-ae3f-4840-a0f5-a3fb31a19859",
          "name": "list-user-participants",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "appointment_groups/:id/users"
              ],
              "query": [
                {
                  "key": "registration_status",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List user participants."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8372723-805c-4e93-9fc4-a695e6c2dd16"
            }
          ]
        }
      ]
    }
  ]
}