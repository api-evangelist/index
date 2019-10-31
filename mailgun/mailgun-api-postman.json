{
  "info": {
    "name": "Mailgun API Unsubscribe",
    "_postman_id": "f94c7b1d-5bf5-41a3-8334-8a4e18794732",
    "description": "Retreives a single unsubscribe record. Can be used to check if a given address is present in the list of unsubscribed users.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bounces",
      "item": [
        {
          "id": "01b71f2a-52c7-417b-9bab-cf527ff111f0",
          "name": "getBounces",
          "request": {
            "url": "http://api.mailgun.net/v2/bounces/?limit=%7B%7D&skip=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches the list of bounces."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bbc67cdd-4ea0-4c79-a605-0a828c037619"
            }
          ]
        }
      ]
    },
    {
      "name": "Bounce",
      "item": [
        {
          "id": "fc0cbbbb-3aee-4f72-95cb-1c329f98ae6f",
          "name": "postBounces",
          "request": {
            "url": "http://api.mailgun.net/v2/bounces/?address=%7B%7D&code=%7B%7D&error=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a permanent bounce to the bounces table. Updates the existing record if already here."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "efee6cf0-15a8-4d7e-90f4-bd7c73cda880"
            }
          ]
        },
        {
          "id": "fff0ba79-5598-44b6-b0b3-0eeae216cdca",
          "name": "getBouncesAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "bounces/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a single bounce event by a given email address. This is useful to check if a given email address has bounced before."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3e4377b-1286-4255-a0b5-6f7cd07e413d"
            }
          ]
        },
        {
          "id": "fef015db-f2be-4a8f-ab33-ee4c8d48f925",
          "name": "deleteBouncesAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "bounces/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "address",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Clears a bounce event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d5ed4e7-f54d-4d35-bdb6-3954bba6ae5f"
            }
          ]
        }
      ]
    },
    {
      "name": "Complaints",
      "item": [
        {
          "id": "21fe2496-0b9e-44c8-8515-b2aa8a9914c4",
          "name": "getComplaints",
          "request": {
            "url": "http://api.mailgun.net/v2/complaints/?limit=%7B%7D&skip=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches the list of complaints."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e88c555e-a34f-4ce2-a4c1-10e4c6b17f90"
            }
          ]
        }
      ]
    },
    {
      "name": "Complaint",
      "item": [
        {
          "id": "683928d7-ce53-4426-8964-30a42368de48",
          "name": "postComplaints",
          "request": {
            "url": "http://api.mailgun.net/v2/complaints/?address=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds an address to the complaints table."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59c2a9bf-bea7-4873-90ea-14c56167d29e"
            }
          ]
        },
        {
          "id": "44116d03-5507-41b2-afc8-472d152fd9b6",
          "name": "getComplaintsAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "complaints/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches a single spam complaint by a given email address. This is useful to check if a particular user has complained."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8f26399-2b83-42f3-9ff6-75f9d5e08014"
            }
          ]
        },
        {
          "id": "33b193b6-27f1-4c0c-bb56-d641aa64cc1a",
          "name": "deleteComplaintsAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "complaints/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a given spam complaint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8103ba1-75a8-41f9-9b77-116bf1e60bb2"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "cbdfbfb4-2eac-41f2-b2c1-d3fa2d2e5c52",
          "name": "postLists",
          "request": {
            "url": "http://api.mailgun.net/v2/lists?access_level=%7B%7D&address=%7B%7D&description=%7B%7D&name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new mailing list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b536d69a-7ff5-4171-ad11-5b7529d8016a"
            }
          ]
        },
        {
          "id": "8ee46902-d86e-40d9-b59d-d25f480bc177",
          "name": "getListsAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "lists/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a single mailing list by a given address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78265b6d-2cbd-46ce-b66f-1d997c7755a7"
            }
          ]
        },
        {
          "id": "197c48df-401a-4011-9ea6-f8b793fc9db9",
          "name": "putListsAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "lists/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "address",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update mailing list properties, such as address, description or name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "514cd094-7787-47e0-8a31-c0a8c2a6fbfc"
            }
          ]
        },
        {
          "id": "c2a86e52-a804-40d3-8730-7ecabc52333f",
          "name": "deleteListsAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "lists/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a mailing list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59e56f3b-3c25-4a29-b93c-44648c9b6020"
            }
          ]
        },
        {
          "id": "484cf1c7-49d9-41b4-bca4-201adb214b45",
          "name": "getListsAddressMembers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "lists/:address/members"
              ],
              "query": [
                {
                  "key": "Name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "subscribed",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "upsert",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "vars",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a member to the mailing list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e91080a1-10f9-4a43-80cc-0c5a7899da79"
            }
          ]
        },
        {
          "id": "ab817139-c4c9-4fa1-b679-15bf16c85693",
          "name": "getListsAddressMembers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "lists/:address/members/"
              ],
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "skip",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "subscribed",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "address",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches the list of mailing list members."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b724f8c-e7e9-450d-9e57-f82b4af60dd2"
            }
          ]
        },
        {
          "id": "42c228a6-8c23-41e0-be02-8ff12d3cd271",
          "name": "getListsAddressMembersMemberAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "lists/:address/members/:member_address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "member_address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a mailing list member."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be9fd490-2023-495c-a96c-b3f8f261daca"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "79601c59-bd84-40ed-8002-ce7f8fc1d42b",
          "name": "getLists",
          "request": {
            "url": "http://api.mailgun.net/v2/lists/?access_level=%7B%7D&address=%7B%7D&description=%7B%7D&limit=%7B%7D&namespace_id=%7B%7D&skip=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of mailing lists under your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d63e9c7-9df0-471a-866a-8dba66c82d6a"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "decaef92-cf72-4cc8-9111-5ab4b6be32c1",
          "name": "postMessages.mime",
          "request": {
            "url": "http://api.mailgun.net/v2/messages.mime?h:X-My-Header=%7B%7D&message=%7B%7D&o:campaign=%7B%7D&o:deliverytime=%7B%7D&o:dkim=%7B%7D&o:tag=%7B%7D&o:testmode=%7B%7D&o:tracking=%7B%7D&o:tracking-clicks=%7B%7D&o:tracking-opens=%7B%7D&to=%7B%7D&v:my-var=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a message in MIME format. Note: you will need to build a MIME string yourself. Use a MIME library for your programming language to do this. Pass the resulting MIME string as message parameter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a06c5b0a-56a9-49c6-985d-898a8fc587be"
            }
          ]
        },
        {
          "id": "f6e41cad-8c4c-460d-9790-20df1c644572",
          "name": "putRoutes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "routes/:id"
              ],
              "query": [
                {
                  "key": "action",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "expression",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "priority",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a given route by ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca8a4a46-b9de-43ef-af02-66221a2e5175"
            }
          ]
        }
      ]
    },
    {
      "name": "Send",
      "item": [
        {
          "id": "f0c59e77-b396-4e3e-9daf-f0583ebfd152",
          "name": "postMessages",
          "request": {
            "url": "http://api.mailgun.net/v2/messages/?attachment=%7B%7D&bcc=%7B%7D&cc=%7B%7D&from=%7B%7D&h:X-My-Header=%7B%7D&html=%7B%7D&inline=%7B%7D&o:campaign=%7B%7D&o:deliverytime=%7B%7D&o:dkim=%7B%7D&o:tag=%7B%7D&o:testmode=%7B%7D&o:tracking=%7B%7D&o:tracking-clicks=%7B%7D&o:tracking-opens=%7B%7D&subject=%7B%7D&text=%7B%7D&to=%7B%7D&v:my-var=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sends a message by assembling it from the components. Note that you can specify most parameters multiple times, HTTP supports this out of the box. This makes sense for parameters like cc, to or attachment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1bf2760-64bd-4851-9600-b2d69afc174f"
            }
          ]
        }
      ]
    },
    {
      "name": "Message",
      "item": [
        {
          "id": "fdcb0ca7-b007-4e2e-821f-6d649c091d83",
          "name": "getMessages",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "messages/:id"
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
            "body": {
              "mode": "raw"
            },
            "description": "Gets a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "537b40bf-1e8f-478b-ae9d-7095364b2f21"
            }
          ]
        }
      ]
    },
    {
      "name": "Routes",
      "item": [
        {
          "id": "dc55df2c-f757-4c45-b269-73b6c975784c",
          "name": "getRoutes",
          "request": {
            "url": "http://api.mailgun.net/v2/routes/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetches the list of routes. Note that routes are defined globally, per account, not per domain as most of other API calls."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b335827f-8bc1-45f8-a823-2a6535b27525"
            }
          ]
        }
      ]
    },
    {
      "name": "Route",
      "item": [
        {
          "id": "d8c6f490-fd48-4422-8803-394df11fbedc",
          "name": "postRoutes",
          "request": {
            "url": "http://api.mailgun.net/v2/routes/?action=%7B%7D&description=%7B%7D&expression=%7B%7D&priority=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new route."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b2ee8e6-4c57-42c2-8b06-802edcd64bbd"
            }
          ]
        },
        {
          "id": "3f1c2a6a-e73d-4bf2-b600-aa2731cde4c7",
          "name": "getRoutes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "routes/:id"
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
            "description": "Returns a single route object based on its ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9bb5d07d-4812-4005-8f8e-b355c9f52c8f"
            }
          ]
        },
        {
          "id": "57317d38-6031-4c26-bdcb-2a4229696371",
          "name": "deleteRoutes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "routes/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a route based on the id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b2c5cab-10a4-41e7-a4e6-2ee30244b822"
            }
          ]
        }
      ]
    },
    {
      "name": "Stats",
      "item": [
        {
          "id": "ab012e71-b8d1-4a10-85d4-7a93fcbf6343",
          "name": "getStats",
          "request": {
            "url": "http://api.mailgun.net/v2/stats/?event=%7B%7D&limit=%7B%7D&skip=%7B%7D&start-date=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of event stat items. Each record represents counts for one event per one day."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "149244a4-d7cd-4fd5-b50c-9a89ff808de4"
            }
          ]
        }
      ]
    },
    {
      "name": "Tag",
      "item": [
        {
          "id": "ad06ba46-1648-4271-9eea-809cbd1b7f83",
          "name": "deleteTagsTag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "tags/:tag"
              ],
              "variable": [
                {
                  "id": "tag",
                  "value": "tag",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes all counters for particular tag and the tag itself."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3791212-3cca-44e7-a57f-2b227ca2d411"
            }
          ]
        }
      ]
    },
    {
      "name": "Unsubscribes",
      "item": [
        {
          "id": "0b7ff47f-3235-43f2-8dce-1c9a42820a42",
          "name": "getUnsubscribes",
          "request": {
            "url": "http://api.mailgun.net/v2/unsubscribes/?limit=%7B%7D&skip=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API allows you to programmatically download the list of recipients who have unsubscribed from your emails."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7af894a-9800-49da-aa43-4830aa1ddfa4"
            }
          ]
        }
      ]
    },
    {
      "name": "To",
      "item": [
        {
          "id": "525a4733-5456-4ee1-b84f-2b4f1b17cc34",
          "name": "postUnsubscribes",
          "request": {
            "url": "http://api.mailgun.net/v2/unsubscribes/?address=%7B%7D&tag=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adds address to unsubscribed table."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b72706c3-dfcd-40c2-b4c6-f453bf1b2b68"
            }
          ]
        }
      ]
    },
    {
      "name": "Unsubscribe",
      "item": [
        {
          "id": "28477cbf-f719-4df4-a03b-b8b06127e185",
          "name": "getUnsubscribesAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "unsubscribes/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retreives a single unsubscribe record. Can be used to check if a given address is present in the list of unsubscribed users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94937bd7-7286-4481-a6df-cb402f285608"
            }
          ]
        },
        {
          "id": "34dfb529-80ae-49f4-8155-3ef253682368",
          "name": "deleteUnsubscribesAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.mailgun.net",
              "path": [
                "v2",
                "unsubscribes/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an address from the unsubscribes table. Address defines which events to delete."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a354fa8-eba2-4438-831a-cc2af384c9dc"
            }
          ]
        }
      ]
    }
  ]
}