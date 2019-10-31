{
  "info": {
    "name": "123FormBuilder Update account",
    "_postman_id": "d52a1fa7-bbf7-47fe-b14b-0c0cd83ca08f",
    "description": "Updates an account. You can only update the users that you have created using your account token.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Ping",
      "item": [
        {
          "id": "82d31587-0ae1-4d09-a363-ec3881742363",
          "name": "this-indicates-if-our-servers-are-up-and-running",
          "request": {
            "url": "http://api.123contactform.com/v2/ping",
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
            "description": "This indicates if our servers are up and running."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d895deae-51ca-42d1-8fdf-c27d2f4af555"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "861e6b93-3be0-44b9-bcba-7b20ee8f307e",
          "name": "allows-you-to-authenticate-users-required-parameters-username-or-email-password-or-passhash",
          "request": {
            "url": "http://api.123contactform.com/v2/token?email=%7B%7D&passhash=%7B%7D&password=%7B%7D&username=%7B%7D",
            "method": "POST",
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
            "description": "Allows you to authenticate users. \n\nRequired parameters:\n- username OR email\n- password OR passhash"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7fa4de0f-5608-4745-b86a-b692212e56f0"
            }
          ]
        },
        {
          "id": "d02a6a9d-f980-4e6b-8ff4-8116edbffbe1",
          "name": "get-all-user-groups",
          "request": {
            "url": "http://api.123contactform.com/v2/groups?JWT=%7B%7D&page=%7B%7D&per_page=%7B%7D",
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
            "description": "Get all user groups"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e70da808-97f6-4ab6-b92c-db3a2fe55b8e"
            }
          ]
        },
        {
          "id": "ea169d8a-957e-4d3d-b3a9-e50389695ed3",
          "name": "update-user-information",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "users/:identifier"
              ],
              "variable": [
                {
                  "id": "identifier",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "admin",
                  "value": "{}",
                  "disabled": false,
                  "description": "Indicates if the subuser is admin or not"
                },
                {
                  "key": "allow_create_form",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow or restrict subuser access to creating new forms"
                },
                {
                  "key": "allow_delete_form",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow subusers to delete forms"
                },
                {
                  "key": "allow_duplicate_form",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow subusers to duplicate forms"
                },
                {
                  "key": "can_manage_groups",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow admin subusers to manage groups"
                },
                {
                  "key": "can_manage_users",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow admin subusers to manage users"
                },
                {
                  "key": "company_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the company to which the subuser belongs"
                },
                {
                  "key": "email",
                  "value": "{}",
                  "disabled": false,
                  "description": "Email address of the account"
                },
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                },
                {
                  "key": "passhash",
                  "value": "{}",
                  "disabled": false,
                  "description": "MD5 password"
                },
                {
                  "key": "password",
                  "value": "{}",
                  "disabled": false,
                  "description": "Plain text password"
                }
              ]
            },
            "description": "Update user information"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb5f3174-cbb0-4d46-bf85-2593dbc3a87c"
            }
          ]
        }
      ]
    },
    {
      "name": "Refresh",
      "item": [
        {
          "id": "9fee5b1e-6653-4d20-b499-6332f336ac3e",
          "name": "refresh-token",
          "request": {
            "url": "http://api.123contactform.com/v2/token/refresh",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                }
              ]
            },
            "description": "Refresh token"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "daf699b2-0559-4fa9-8993-6c742049a5a2"
            }
          ]
        }
      ]
    },
    {
      "name": "Invalidate",
      "item": [
        {
          "id": "c25ef33f-bdeb-4042-952b-2ac89aeeb83d",
          "name": "invalidate-token",
          "request": {
            "url": "http://api.123contactform.com/v2/token/invalidate",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                }
              ]
            },
            "description": "Invalidate token"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "795cced9-37ad-498d-abeb-03b98c519da5"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "fd2f435d-84e5-4d96-a128-4911dc92b43b",
          "name": "the-forms-endpoint-returns-information-about-the-forms-the-response-includes-submissions-and-other-d",
          "request": {
            "url": "http://api.123contactform.com/v2/forms?JWT=%7B%7D&page=%7B%7D&per_page=%7B%7D&search=%7B%7D",
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
            "description": "The forms endpoint returns information about the forms. The response includes submissions and other details about each form."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26c67e6a-87ed-4284-91e8-1322cbe0620e"
            }
          ]
        }
      ]
    },
    {
      "name": "New",
      "item": [
        {
          "id": "d4267f4a-8da7-48db-aa5d-ae3f62dbf8e4",
          "name": "create-a-new-form",
          "request": {
            "url": "http://api.123contactform.com/v2/forms",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "active",
                  "value": "{}",
                  "disabled": false,
                  "description": "Form activity status"
                },
                {
                  "key": "active_date_from",
                  "value": "{}",
                  "disabled": false,
                  "description": "If activity status is 1, this field is required"
                },
                {
                  "key": "active_date_to",
                  "value": "{}",
                  "disabled": false,
                  "description": "If activity status is 1, this field is required"
                },
                {
                  "key": "active_days",
                  "value": "{}",
                  "disabled": false,
                  "description": "If activity status is 4, this field is required"
                },
                {
                  "key": "group_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of the group in which you want to create the form"
                },
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the new form"
                }
              ]
            },
            "description": "Create a new form"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84be86b0-b1cc-4d21-8b7a-27230572eaa4"
            }
          ]
        },
        {
          "id": "9c877198-e049-4837-b59c-bc8d3231cc3c",
          "name": "create-a-new-group",
          "request": {
            "url": "http://api.123contactform.com/v2/groups",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Form name"
                },
                {
                  "key": "parent_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "Indicates the ID of the parent group"
                },
                {
                  "key": "webhook_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The URL of the WebHook"
                }
              ]
            },
            "description": "Create a new group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4151430-241e-42cc-acf2-abf11a0d2967"
            }
          ]
        },
        {
          "id": "e12bc1ce-4a95-4b46-b72e-ed891a8eea7a",
          "name": "create-a-new-subuser",
          "request": {
            "url": "http://api.123contactform.com/v2/users",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "admin",
                  "value": "{}",
                  "disabled": false,
                  "description": "Indicates if the subuser is admin or not"
                },
                {
                  "key": "allow_create_form",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow or restrict subuser access to creating new forms"
                },
                {
                  "key": "allow_delete_form",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow subusers to delete forms"
                },
                {
                  "key": "allow_duplicate_form",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow subusers to duplicate forms"
                },
                {
                  "key": "can_manage_groups",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow admin subusers to manage groups"
                },
                {
                  "key": "can_manage_users",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow admin subusers to manage users"
                },
                {
                  "key": "company_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the company to which the subuser belongs"
                },
                {
                  "key": "email",
                  "value": "{}",
                  "disabled": false,
                  "description": "Email address of the account"
                },
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Username of the account"
                },
                {
                  "key": "passhash",
                  "value": "{}",
                  "disabled": false,
                  "description": "MD5 password"
                },
                {
                  "key": "password",
                  "value": "{}",
                  "disabled": false,
                  "description": "Plain text password"
                }
              ]
            },
            "description": "Create a new subuser"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7dd11ad7-27a3-4b8b-88d7-f1980340aa88"
            }
          ]
        },
        {
          "id": "247e1716-efbd-4da2-b8b1-6962752b4f72",
          "name": "creates-a-new-account-standalone-user-this-is-available-only-upon-request",
          "request": {
            "url": "http://api.123contactform.com/v2/accounts",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "company_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The company name associated with the account"
                },
                {
                  "key": "email",
                  "value": "{}",
                  "disabled": false,
                  "description": "The email address associated with the account"
                },
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The username associated with the account"
                },
                {
                  "key": "password",
                  "value": "{}",
                  "disabled": false,
                  "description": "The password associated with the account"
                },
                {
                  "key": "password_repeat",
                  "value": "{}",
                  "disabled": false,
                  "description": "Password repeat"
                },
                {
                  "key": "plan",
                  "value": "{}",
                  "disabled": false,
                  "description": "The service plan of the account: 0 - Free (default value), 1 - Gold, 2 - Platinum, 3 - Diamond"
                }
              ]
            },
            "description": "Creates a new account (standalone user). This is available only upon request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "811ee3aa-0e82-48d4-95b7-ecb1c7382063"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "4ff84709-033a-4c34-8360-d5344b5ea297",
          "name": "delete-multiple-forms",
          "request": {
            "url": "http://api.123contactform.com/v2/forms/bulk",
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "form_ids",
                  "value": "{}",
                  "disabled": false,
                  "description": "The IDs of the forms separated by comma"
                },
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                }
              ]
            },
            "description": "Delete multiple forms"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51c6e004-23b8-4a49-8fff-d2d8e6ea839c"
            }
          ]
        }
      ]
    },
    {
      "name": "Form",
      "item": [
        {
          "id": "c336abcc-3150-4ca2-802d-110e4b4f30e1",
          "name": "get-the-details-of-a-single-form",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "forms/:form_id"
              ],
              "query": [
                {
                  "key": "JWT",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "form_id",
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
            "description": "Get the details of a single form"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "941fc798-3be5-436b-b2a3-419a4a932c4a"
            }
          ]
        },
        {
          "id": "1c5e7184-902a-4bd9-963b-f504e08ad602",
          "name": "update-form-details",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "forms/:form_id"
              ],
              "query": [
                {
                  "key": "JWT",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "form_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "active",
                  "value": "{}",
                  "disabled": false,
                  "description": "Form activity status"
                },
                {
                  "key": "active_date_from",
                  "value": "{}",
                  "disabled": false,
                  "description": "If activity status is 1, this field is required"
                },
                {
                  "key": "active_date_to",
                  "value": "{}",
                  "disabled": false,
                  "description": "If activity status is 1, this field is required"
                },
                {
                  "key": "active_days",
                  "value": "{}",
                  "disabled": false,
                  "description": "If activity status is 4, this field is required"
                },
                {
                  "key": "group_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of the group in which you want to create the form"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Change the name of the form"
                }
              ]
            },
            "description": "Update form details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "615e0e44-4a31-4ddc-98e1-7dcc230ac23c"
            }
          ]
        },
        {
          "id": "16f8a26f-13ec-4b7e-b6de-359bf24d32a3",
          "name": "delete-a-form",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "forms/:form_id"
              ],
              "variable": [
                {
                  "id": "form_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                }
              ]
            },
            "description": "Delete a form"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b25f0ee5-4244-43b4-9ec6-a3fa7bd4a141"
            }
          ]
        },
        {
          "id": "33175e20-4e08-4a4e-87a9-32f56813c3b7",
          "name": "get-the-details-of-a-single-form-and-its-fields",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "forms/:form_id/fields"
              ],
              "query": [
                {
                  "key": "JWT",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "form_id",
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
            "description": "Get the details of a single form and its fields"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ac1fe81-8d6e-4a23-8cec-e989910a35a5"
            }
          ]
        },
        {
          "id": "e248d071-0c4c-4811-895f-8b5853d68a40",
          "name": "delete-one-form-submission",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "forms/:form_id/submissions/:submission_id"
              ],
              "query": [
                {
                  "key": "JWT",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "form_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "submission_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Delete one form submission"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0101da35-d52c-49fc-824f-48eedefb164c"
            }
          ]
        }
      ]
    },
    {
      "name": "Submissions",
      "item": [
        {
          "id": "b6e2125c-73a3-4904-9984-7a235f3e3e69",
          "name": "get-all-submissions-received-through-a-form",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "forms/:form_id/submissions"
              ],
              "query": [
                {
                  "key": "include_recipients",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "JWT",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "per_page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_submission_id",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "form_id",
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
            "description": "Get all submissions received through a form"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a065e08-0f52-4200-832e-429250cde991"
            }
          ]
        }
      ]
    },
    {
      "name": "Submission",
      "item": [
        {
          "id": "2f3dc566-c14f-4ffb-bcd1-4527a907f747",
          "name": "get-the-details-of-a-single-submission",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "forms/:form_id/submissions/:submission_id"
              ],
              "query": [
                {
                  "key": "include_recipients",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "JWT",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "form_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "submission_id",
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
            "description": "Get the details of a single submission"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "648e8df4-4a4e-4587-8bfe-da760dc594a5"
            }
          ]
        },
        {
          "id": "9d547b53-a81e-4e43-a88f-d385e39827af",
          "name": "update-submission",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "forms/:form_id/submissions/:submission_id"
              ],
              "query": [
                {
                  "key": "approved",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "JWT",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "payed",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "form_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "submission_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
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
            "description": "Update Submission"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b2cc703-002f-411c-a257-7994871c8edb"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "881a6235-b36b-4493-b4ca-2ab71f1964e4",
          "name": "get-information-about-a-specific-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "groups/:group_id"
              ],
              "query": [
                {
                  "key": "JWT",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
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
            "description": "Get information about a specific group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd07c29c-2cdd-423b-9d36-ba7a0f18c622"
            }
          ]
        },
        {
          "id": "1877339a-41ac-432b-b331-115c9244acb9",
          "name": "updates-the-details-of-a-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "groups/:group_id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "This is required when the webhook_url or parent_id is missing"
                },
                {
                  "key": "parent_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "Indicates the ID of the parent group"
                },
                {
                  "key": "webhook_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "This is required when the name or parent_id is missing"
                }
              ]
            },
            "description": "Updates the details of a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27675abe-b9e7-403b-a588-0ab8b38a3bca"
            }
          ]
        }
      ]
    },
    {
      "name": "Forms",
      "item": [
        {
          "id": "99155865-9c08-4c35-ab35-f2207aebee2e",
          "name": "displays-a-list-of-all-of-the-forms-within-a-specific-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "groups/:group_id/forms"
              ],
              "query": [
                {
                  "key": "JWT",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
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
            "description": "Displays a list of all of the forms within a specific group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23722f08-2c06-4a99-a3dc-cf4bde615d7d"
            }
          ]
        }
      ]
    },
    {
      "name": "Share",
      "item": [
        {
          "id": "8a7e9240-02d7-440d-8785-c24022d72ac4",
          "name": "this-may-not-be-available-for-your-account-it-is-specific-to-certain-users",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "groups/:group_id/share"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                },
                {
                  "key": "subuser_email",
                  "value": "{}",
                  "disabled": false,
                  "description": "The username with whom you want to share this group"
                },
                {
                  "key": "subuser_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of the user with whom you want to share this group"
                }
              ]
            },
            "description": "This may not be available for your account. It is specific to certain users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e4dc14c-67ec-42d1-a897-b6ee31486be2"
            }
          ]
        }
      ]
    },
    {
      "name": "Unshare",
      "item": [
        {
          "id": "5cd1187d-ba5a-4207-9dfc-ad3a1850cc2e",
          "name": "this-may-not-be-available-for-your-account-it-is-specific-to-certain-users",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "groups/:group_id/unshare"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                },
                {
                  "key": "subuser_email",
                  "value": "{}",
                  "disabled": false,
                  "description": "The username from whom you want to unshare the group"
                },
                {
                  "key": "subuser_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of the subuser from whom you want to unshare the group"
                }
              ]
            },
            "description": "This may not be available for your account. It is specific to certain users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "361d12f6-f025-4c4e-b5b6-88e826a070c0"
            }
          ]
        }
      ]
    },
    {
      "name": "Info",
      "item": [
        {
          "id": "85efec5f-7207-4981-9be5-633d47b8d819",
          "name": "get-info-about-master-user-and-subusers",
          "request": {
            "url": "http://api.123contactform.com/v2/users?JWT=%7B%7D&page=%7B%7D&per_page=%7B%7D",
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
            "description": "Get info about master user and subusers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6abfde35-9259-4093-9cd1-17b748988fd0"
            }
          ]
        }
      ]
    },
    {
      "name": "Account",
      "item": [
        {
          "id": "c96430e9-da43-45c7-9d68-6545473230b2",
          "name": "updates-an-account-you-can-only-update-the-users-that-you-have-created-using-your-account-token",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "accounts/:user_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "company_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The company name associated with the account"
                },
                {
                  "key": "email",
                  "value": "{}",
                  "disabled": false,
                  "description": "The email address associated with the account"
                },
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                },
                {
                  "key": "password",
                  "value": "{}",
                  "disabled": false,
                  "description": "The password associated with the account"
                },
                {
                  "key": "password_repeat",
                  "value": "{}",
                  "disabled": false,
                  "description": "Password repeat"
                },
                {
                  "key": "plan",
                  "value": "{}",
                  "disabled": false,
                  "description": "The service plan of the account: 0 - Free (default value), 1 - Gold, 2 - Platinum, 3 - Diamond"
                }
              ]
            },
            "description": "Updates an account. You can only update the users that you have created using your account token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a0e2fc9-0611-48ca-a0fc-329bcb846ed7"
            }
          ]
        }
      ]
    }
  ]
}