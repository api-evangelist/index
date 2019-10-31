{
  "info": {
    "name": "Instructure Canvas Polls API List opened poll sessions",
    "_postman_id": "33948b40-0bf8-427b-a3e9-a14e6c28a405",
    "description": "List opened poll sessions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Polls",
      "item": [
        {
          "id": "946529eb-531f-4554-bc6b-649316946df9",
          "name": "list-polls",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/polls",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List polls."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "932f5c5a-527f-4ef8-8aa6-a77a6dc99266"
            }
          ]
        },
        {
          "id": "88d9e621-d9a0-4e6c-8432-4dfd882c3e6d",
          "name": "create-a-single-poll",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/polls?polls[][description]=%7B%7D&polls[][question]=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a single poll."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96fef135-784a-455c-afa6-f43a1e468128"
            }
          ]
        },
        {
          "id": "3a1821e9-4af2-478e-9bab-f02f726da5a4",
          "name": "get-a-single-poll",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:id"
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
            "description": "Get a single poll."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30a79728-ca92-4670-a11b-1f055d6e0d59"
            }
          ]
        },
        {
          "id": "056d0eec-045d-4b12-a02d-342f7383087d",
          "name": "update-a-single-poll",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:id"
              ],
              "query": [
                {
                  "key": "polls[][description]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "polls[][question]",
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
            "description": "Update a single poll."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2abec21-907a-49af-9578-cb791da6ac4e"
            }
          ]
        },
        {
          "id": "1809c507-dc86-4ae0-98d8-0ae78c5cf729",
          "name": "delete-a-poll",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:id"
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
            "description": "Delete a poll."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8dd0e455-1ac3-434b-ad85-d5913346db00"
            }
          ]
        },
        {
          "id": "daa19783-c6fb-41ad-a7ef-447d003c2efd",
          "name": "list-poll-choices-in-a-poll",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:poll_id/poll_choices"
              ],
              "variable": [
                {
                  "id": "poll_id",
                  "value": "poll_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List poll choices in a poll."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6272699a-64c0-4758-bee0-8be207984632"
            }
          ]
        },
        {
          "id": "a0ff1b17-7b20-4949-a049-7a49cc772d89",
          "name": "create-a-single-poll-choice",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:poll_id/poll_choices"
              ],
              "query": [
                {
                  "key": "poll_choices[][is_correct]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "poll_choices[][position]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "poll_choices[][text]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "poll_id",
                  "value": "poll_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a single poll choice."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f64bb4c7-3950-4097-b2ec-cf64e88a8999"
            }
          ]
        },
        {
          "id": "5f30e693-777d-457f-a05a-20952c6115d1",
          "name": "get-a-single-poll-choice",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:poll_id/poll_choices/id"
              ],
              "variable": [
                {
                  "id": "poll_id",
                  "value": "poll_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single poll choice."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a38a27fe-2534-45e1-a5b8-28e037612cf9"
            }
          ]
        },
        {
          "id": "66a5a54d-72c7-4145-8df6-8d36f023fb2b",
          "name": "update-a-single-poll-choice",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:poll_id/poll_choices/id"
              ],
              "query": [
                {
                  "key": "poll_choices[][is_correct]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "poll_choices[][position]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "poll_choices[][text]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "poll_id",
                  "value": "poll_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a single poll choice."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64a77959-6e81-4a9a-b360-fc75d30dd943"
            }
          ]
        },
        {
          "id": "3b869840-6008-42f3-a656-a53ce09dcc41",
          "name": "delete-a-poll-choice",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:poll_id/poll_choices/id"
              ],
              "variable": [
                {
                  "id": "poll_id",
                  "value": "poll_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a poll choice."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e17e88a1-0064-473e-9740-50e501d272d0"
            }
          ]
        },
        {
          "id": "fe436764-4436-4c88-8f25-0fc8e6eed76f",
          "name": "list-poll-sessions-for-a-poll",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:poll_id/poll_sessions"
              ],
              "variable": [
                {
                  "id": "poll_id",
                  "value": "poll_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List poll sessions for a poll."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a641a28-de30-40cb-88c4-a00c0959eee9"
            }
          ]
        },
        {
          "id": "c452028c-f1dd-47ab-a32b-53098832e63a",
          "name": "create-a-single-poll-session",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:poll_id/poll_sessions"
              ],
              "query": [
                {
                  "key": "poll_sessions[][course_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "poll_sessions[][course_section_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "poll_sessions[][has_public_results]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "poll_id",
                  "value": "poll_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a single poll session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ab24764-7ffd-4727-877d-4d09bda722bd"
            }
          ]
        },
        {
          "id": "5e59e03e-6ea5-4c7f-9522-e6334e4ec8a7",
          "name": "get-the-results-for-a-single-poll-session",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:poll_id/poll_sessions/id"
              ],
              "variable": [
                {
                  "id": "poll_id",
                  "value": "poll_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the results for a single poll session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1079ce58-07f0-486b-85bd-33444f9a58e7"
            }
          ]
        },
        {
          "id": "fca70480-a44b-4bf1-8fd3-5e9595e37d38",
          "name": "update-a-single-poll-session",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:poll_id/poll_sessions/id"
              ],
              "query": [
                {
                  "key": "poll_sessions[][course_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "poll_sessions[][course_section_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "poll_sessions[][has_public_results]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "poll_id",
                  "value": "poll_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a single poll session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "864d8283-ea72-45ae-9b1c-1b6e293f360f"
            }
          ]
        },
        {
          "id": "e374bfbd-f130-490d-8afd-1f50b8ef3ed4",
          "name": "delete-a-poll-session",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:poll_id/poll_sessions/id"
              ],
              "variable": [
                {
                  "id": "poll_id",
                  "value": "poll_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a poll session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "030c2d3e-fccb-4879-8bc5-189f52527a6f"
            }
          ]
        },
        {
          "id": "68637475-fd62-4708-9c59-e5d8f06165a1",
          "name": "close-an-opened-poll-session",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:poll_id/poll_sessions/id/close"
              ],
              "variable": [
                {
                  "id": "poll_id",
                  "value": "poll_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Close an opened poll session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "591607b1-5650-44c3-86e9-8beae39b2681"
            }
          ]
        },
        {
          "id": "3fe86c67-c61f-4368-95e4-278e37138260",
          "name": "open-a-poll-session",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:poll_id/poll_sessions/id/open"
              ],
              "variable": [
                {
                  "id": "poll_id",
                  "value": "poll_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Open a poll session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84d8dbfd-7772-4500-bf3b-4dfe1e53ff65"
            }
          ]
        },
        {
          "id": "ea15b915-22e4-42d6-adb4-43fbd7c3f9d6",
          "name": "create-a-single-poll-submission",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:poll_id/poll_sessions/poll_session_id/poll_submissions"
              ],
              "query": [
                {
                  "key": "poll_submissions[][poll_choice_id]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "poll_id",
                  "value": "poll_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a single poll submission."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a49dab9-9faf-4205-8eb7-7c0f82ea1373"
            }
          ]
        },
        {
          "id": "7d39e150-65bd-4e3b-b41d-825f3e6061c7",
          "name": "get-a-single-poll-submission",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "polls/:poll_id/poll_sessions/poll_session_id/poll_submissions/:id"
              ],
              "variable": [
                {
                  "id": "poll_id",
                  "value": "poll_id",
                  "type": "string"
                },
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
            "description": "Get a single poll submission."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e6561d9-6390-49e2-8148-cf92f3083436"
            }
          ]
        }
      ]
    },
    {
      "name": "Poll",
      "item": [
        {
          "id": "c8eb0aac-9a2f-4225-a3c9-4ce05079cd4d",
          "name": "list-closed-poll-sessions",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/poll_sessions/closed",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List closed poll sessions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80d81e55-6286-4c35-89e8-86bcbf8d1842"
            }
          ]
        },
        {
          "id": "696742e1-0a51-4ac5-a109-03c1f4ed99e7",
          "name": "list-opened-poll-sessions",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/poll_sessions/opened",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List opened poll sessions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d748ab8-499a-4968-9701-326800cb9c47"
            }
          ]
        }
      ]
    }
  ]
}