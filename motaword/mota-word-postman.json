{
  "info": {
    "name": "Mota Word Retrieve an access token to interact with the API.",
    "_postman_id": "f062e843-7d7a-4f36-833a-64b19ad6b010",
    "description": "MotaWord API is using OAuth2 procedures when authenticating or authorizing your API call. Currently, we only allow Client Credential type flow.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Folder",
      "item": [
        {
          "id": "8789aa7d-753a-4dde-8097-1d2fdae13459",
          "name": "getEndpoints",
          "request": {
            "url": "http://api.motaword.com/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The root endpoint will provide you a JSON Swagger definition."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0538f6d8-cd75-46a2-acf8-7989fe6bd383"
            }
          ]
        }
      ]
    },
    {
      "name": "Formats",
      "item": [
        {
          "id": "83af4f5a-37b2-416b-a51a-6008e228f681",
          "name": "getFormats",
          "request": {
            "url": "http://api.motaword.com/formats",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of supported formats for documents, style guides and extensions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6282d2a1-1c26-40e6-9c71-1c7f196bea4c"
            }
          ]
        }
      ]
    },
    {
      "name": "Glossary",
      "item": [
        {
          "id": "4a4bf3e0-cac9-46de-904c-cae5bd7909a3",
          "name": "downloadGlobalGlossary",
          "request": {
            "url": "http://api.motaword.com/glossary",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Download your corporate account's global glossary. This endpoint is available only for corporate account customers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1247d7b3-205c-4016-b98b-1450abbb6e22"
            }
          ]
        },
        {
          "id": "cd27132d-ef53-4421-8e45-370e527a91e4",
          "name": "updateGlobalGlossary",
          "request": {
            "url": "http://api.motaword.com/glossary",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "glossary",
                  "value": "{}",
                  "disabled": false,
                  "description": "Glossary file"
                }
              ]
            },
            "description": "Update your corporate account's global glossary. This endpoint is available only for corporate account customers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68c57dca-e04d-4a82-9116-3b025986e4fe"
            }
          ]
        }
      ]
    },
    {
      "name": "Languages",
      "item": [
        {
          "id": "fa25d481-f436-41bc-8e57-5e78fab5c07a",
          "name": "getLanguages",
          "request": {
            "url": "http://api.motaword.com/languages",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of supported languages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "115b63a9-33ba-4ba0-be07-2fb33c6c4422"
            }
          ]
        }
      ]
    },
    {
      "name": "Me",
      "item": [
        {
          "id": "4273fdfd-2bfd-40d4-bdd0-20c428d33b35",
          "name": "getAccount",
          "request": {
            "url": "http://api.motaword.com/me",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get your account information and summary.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ecd818a-a4bf-49ef-b5b2-24a4234bd9e6"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "4adf5cb9-81a2-464b-a7b4-6f4be75083a4",
          "name": "getProjects",
          "request": {
            "url": "http://api.motaword.com/projects?page=%7B%7D&per_page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of your projects."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68f99702-57e3-40f5-b85f-61f66a8d35fe"
            }
          ]
        },
        {
          "id": "4b3225e9-e513-4d11-93de-ff5fa1059084",
          "name": "createProject",
          "request": {
            "url": "http://api.motaword.com/projects",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "callback_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "Optional"
                },
                {
                  "key": "custom",
                  "value": "{}",
                  "disabled": false,
                  "description": "Optional"
                },
                {
                  "key": "documents",
                  "value": "[{}]",
                  "disabled": false,
                  "description": "Optional"
                },
                {
                  "key": "glossaries",
                  "value": "[{}]",
                  "disabled": false,
                  "description": "Optional"
                },
                {
                  "key": "source_language",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "styleguides",
                  "value": "[{}]",
                  "disabled": false,
                  "description": "Optional"
                },
                {
                  "key": "target_languages",
                  "value": "[{}]",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Create a new project"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce7ba767-9b9b-4d07-8056-fb208e1411dc"
            }
          ]
        },
        {
          "id": "1f594db6-37a8-496c-a536-c911cf1f3844",
          "name": "getProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id"
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
            "description": "Get single project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "743834e4-5678-442a-a4f7-deecbc34dd00"
            }
          ]
        },
        {
          "id": "d65e2790-9ce7-433a-bffb-f19648e10c2b",
          "name": "updateProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id"
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
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "callback_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "Optional"
                },
                {
                  "key": "custom",
                  "value": "{}",
                  "disabled": false,
                  "description": "Optional"
                },
                {
                  "key": "source_language",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "target_languages",
                  "value": "[{}]",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Update project language pairs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5a87908-4508-4218-ae73-f1f0fd5d88f9"
            }
          ]
        },
        {
          "id": "ba7a3e07-1401-4f33-873a-174e463c8e16",
          "name": "deleteProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id"
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
            "description": "Delete(cancel) a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ac819fd-27c9-4495-9d79-194dc4b57467"
            }
          ]
        },
        {
          "id": "86b9b097-3c73-43ee-b551-9a02f46de492",
          "name": "triggerCallback",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/callback/:actionType"
              ],
              "variable": [
                {
                  "id": "actionType",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Trigger a call to your callback url related to this project.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "099d7a5a-0a07-4255-b0b1-00a709a54f02"
            }
          ]
        },
        {
          "id": "ffe345e3-d4ec-40e2-843a-4fd64b49ea12",
          "name": "cancelProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/cancel"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "reason",
                  "value": "{}",
                  "disabled": false,
                  "description": "Cancellation reason"
                }
              ]
            },
            "description": "Cancel your translation project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8c392d5-ba50-452a-8221-a3c8d28e3c5b"
            }
          ]
        },
        {
          "id": "656d73a8-3b3f-4b74-aa10-53f37e08e25b",
          "name": "download",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/download"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Download the latest translation package. You must have given a /package call beforehand and wait until the packaging status is 'completed'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "feda22f6-6c63-46a9-9ea1-297d2a9768f6"
            }
          ]
        },
        {
          "id": "c4990244-5de1-4e58-9979-57c862a086b4",
          "name": "downloadLanguage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/download/:language"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "language",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Download only the translation package of this language. You must have given a /package call beforehand and wait until the packaging status is 'completed'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01e3f009-aa2e-4015-bf72-6caa551aedbf"
            }
          ]
        },
        {
          "id": "1baa6915-7aef-4cc8-9b57-9dcded18507f",
          "name": "launchProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/launch"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "budget_code",
                  "value": "{}",
                  "disabled": false,
                  "description": "Optional with corporate accounts"
                },
                {
                  "key": "payment_code",
                  "value": "{}",
                  "disabled": false,
                  "description": "Optional"
                },
                {
                  "key": "payment_method",
                  "value": "{}",
                  "disabled": false,
                  "description": "Optional"
                }
              ]
            },
            "description": "Launch your translation project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "240f604d-a20c-4de2-994b-ff3bda963c55"
            }
          ]
        },
        {
          "id": "12835a2f-7240-4379-b933-5be127096f06",
          "name": "package",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/package"
              ],
              "query": [
                {
                  "key": "async",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Package the translation project, make it ready to be downloaded."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1a954c1-9a7a-41ae-a6cc-5875160af391"
            }
          ]
        },
        {
          "id": "3e0e5081-76c3-4d5f-9d8c-dbd2919c8c48",
          "name": "trackPackage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/package/check"
              ],
              "query": [
                {
                  "key": "key",
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
            "body": {
              "mode": "raw"
            },
            "description": "This request will tell you the current progress of the translation packaging. You will use the 'key' provided by the /package call."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6266737c-5e78-4e6a-ad89-eaa6105752c2"
            }
          ]
        },
        {
          "id": "15ed6b5e-f0b0-4c0f-9495-4239f5e61a8d",
          "name": "packageLanguage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/package/:language"
              ],
              "query": [
                {
                  "key": "async",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "language",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Package the translation of a specific target language to be downloaded.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eef97296-5107-4f16-8291-6b67e549beb0"
            }
          ]
        },
        {
          "id": "7de58947-05ad-44d7-80d8-21ebf8231096",
          "name": "getProgress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/progress"
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
            "description": "Get the progress of an already launched project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50f9378f-cd07-4a00-9017-5d68789d65e9"
            }
          ]
        },
        {
          "id": "4cf20486-8470-4e72-be55-0817f2f8492d",
          "name": "submitProjectReports",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:id/reports"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "activity_type",
                  "value": "{}",
                  "disabled": false,
                  "description": "Activity Type"
                },
                {
                  "key": "message",
                  "value": "{}",
                  "disabled": false,
                  "description": "Report Message"
                }
              ]
            },
            "description": "Submit reports for a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b47ea2d-d54d-450e-bbdc-8eb0491ea2b2"
            }
          ]
        },
        {
          "id": "b2f2e055-439e-49f6-a731-05fa6e0cff25",
          "name": "getActivities",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/activities"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "per_page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of realtime activities on the project, such as translation suggestion and translation approval."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8e63d59-7f66-4620-a1d8-549252320b2b"
            }
          ]
        },
        {
          "id": "397e7ee0-57a8-4d08-bca7-05032d17439e",
          "name": "getActivity",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/activities/:activityId"
              ],
              "variable": [
                {
                  "id": "activityId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single realtime activity.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8eda86ab-5698-4834-937a-cdf5c7b07e66"
            }
          ]
        },
        {
          "id": "67f4cc99-4400-417a-b780-30bedaa8b26e",
          "name": "submitComment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/activities/:activityId"
              ],
              "variable": [
                {
                  "id": "activityId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "comment",
                  "value": "{}",
                  "disabled": false,
                  "description": "Comment text"
                }
              ]
            },
            "description": "Submit a comment to an activity.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c64789d8-c64a-4252-97ce-4a68f8d3e43b"
            }
          ]
        },
        {
          "id": "180d7e67-f283-41bf-90b8-53c892f0d8db",
          "name": "getActivityComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/activities/:activityId/comments"
              ],
              "variable": [
                {
                  "id": "activityId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of comments belonging to this activity.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b24befa8-c556-4151-80b5-f3b45e03bc94"
            }
          ]
        },
        {
          "id": "37654a03-e733-4d0e-85c3-c5679046766b",
          "name": "getComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/comments"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "per_page",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of activity comments throughout the whole project.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0f2ad54-51bd-43c2-bb40-d1b5ca691f48"
            }
          ]
        },
        {
          "id": "b95ef609-79a2-4ea7-a40a-401950dd2ceb",
          "name": "getDocuments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/documents"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of documents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11480009-a93d-41ea-95ff-290e24c36a2a"
            }
          ]
        },
        {
          "id": "94872a71-85fd-4ace-a059-a78d1cb905e7",
          "name": "createDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/documents"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "documents",
                  "value": "[{}]",
                  "disabled": false,
                  "description": "You can add as many files as you want in documents[] parameter"
                },
                {
                  "key": "schemes",
                  "value": "[{}]",
                  "disabled": false,
                  "description": "JSON string"
                }
              ]
            },
            "description": "Upload a new document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "903bf61c-6cf0-4f8f-9ae0-520299d05e4d"
            }
          ]
        },
        {
          "id": "fb604c20-bf45-41af-9e2e-afd1ff467ea3",
          "name": "getDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/documents/:documentId"
              ],
              "variable": [
                {
                  "id": "documentId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get single document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26d7ea2b-b847-4fcb-a1ec-8004ee91b01a"
            }
          ]
        },
        {
          "id": "320e5ff8-cb03-4e71-9060-8ee214f8da53",
          "name": "updateDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/documents/:documentId"
              ],
              "variable": [
                {
                  "id": "documentId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "documents",
                  "value": "{}",
                  "disabled": false,
                  "description": "Single file data"
                },
                {
                  "key": "schemes",
                  "value": "{}",
                  "disabled": false,
                  "description": "JSON string"
                }
              ]
            },
            "description": "Update the document. File name and contents will replaced with the new one."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7304d9e6-cc70-4c9b-b9f0-2fd918199050"
            }
          ]
        },
        {
          "id": "e8ceb81b-2ac7-48ef-93c8-e21014dcbe17",
          "name": "deleteDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/documents/:documentId"
              ],
              "variable": [
                {
                  "id": "documentId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete the document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ef86dc2-c593-4348-8ad3-46cfb9d0db30"
            }
          ]
        },
        {
          "id": "515ccd87-2526-4538-89b0-d50780271319",
          "name": "downloadDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/documents/:documentId/download"
              ],
              "variable": [
                {
                  "id": "documentId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Download a document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc2f123f-eb24-4224-8561-fa8affa5eed2"
            }
          ]
        },
        {
          "id": "32a07017-3923-4629-abf9-ce2479ed3a12",
          "name": "getGlossaries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/glossaries"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of glossaries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98d77c3e-aaf8-4b26-bf2d-8a158a5139cf"
            }
          ]
        },
        {
          "id": "ca42d597-05df-4b56-9562-cd4b5c962b7d",
          "name": "createGlossary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/glossaries"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "glossaries",
                  "value": "{}",
                  "disabled": false,
                  "description": "You can only add one glossary, even though the name suggests multiple glossaries"
                }
              ]
            },
            "description": "Upload a new glossary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a3ff900-af34-4b46-88a1-e4b05bc3ec8b"
            }
          ]
        },
        {
          "id": "5570f54e-4ed0-49ed-87b3-dcea5f32eb6f",
          "name": "getGlossary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/glossaries/:glossaryId"
              ],
              "variable": [
                {
                  "id": "glossaryId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get single glossary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cd23c9d-fc58-42e8-a975-e2ab2920e23d"
            }
          ]
        },
        {
          "id": "ef0d4b16-42f2-41cb-8541-f897aba45b0d",
          "name": "updateGlossary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/glossaries/:glossaryId"
              ],
              "variable": [
                {
                  "id": "glossaryId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "glossaries",
                  "value": "{}",
                  "disabled": false,
                  "description": "Single file data"
                }
              ]
            },
            "description": "Update the glossary. File name and contents will replaced with the new one."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d03056df-97ff-44ca-bc3d-63cdc822b9d8"
            }
          ]
        },
        {
          "id": "4b192e7a-ad49-420f-861d-80086b739af5",
          "name": "deleteGlossary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/glossaries/:glossaryId"
              ],
              "variable": [
                {
                  "id": "glossaryId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete the glossary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54387ac3-e1eb-458e-9028-64cfb312f474"
            }
          ]
        },
        {
          "id": "4a75a4af-9641-4e6d-9ae0-712dbdb2cc22",
          "name": "downloadGlossary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/glossaries/:glossaryId/download"
              ],
              "variable": [
                {
                  "id": "glossaryId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Download a glossary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f19dd0f2-66d0-4d77-9721-642595c6f49a"
            }
          ]
        },
        {
          "id": "49a7d731-d0d5-4af0-8bc5-68ba2c468a17",
          "name": "getStyleGuides",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/styleguides"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of style guides."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "485ca682-c5f4-44bd-81a6-86f5f1f72cda"
            }
          ]
        },
        {
          "id": "1fa32cf2-11b0-4745-95e8-eef7aabd7913",
          "name": "createStyleGuide",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/styleguides"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "styleguides",
                  "value": "[{}]",
                  "disabled": false,
                  "description": "You can add as many files as you want in styleguides[] parameter"
                }
              ]
            },
            "description": "Upload a new style guide."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79feb93e-f412-41e4-81ed-f77d3748443b"
            }
          ]
        },
        {
          "id": "8a0e94e3-cf01-4a02-aa1c-ac5ac783ab04",
          "name": "getStyleGuide",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/styleguides/:styleGuideId"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "styleGuideId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get single style guide."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f17145e0-6aaf-411c-93ae-10800dafd945"
            }
          ]
        },
        {
          "id": "68e7870c-cc87-47cf-8f00-4a4b2be235e5",
          "name": "updateStyleGuide",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/styleguides/:styleGuideId"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "styleGuideId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "styleguides",
                  "value": "{}",
                  "disabled": false,
                  "description": "Single file data"
                }
              ]
            },
            "description": "Update the style guide. File name and contents will replaced with the new one."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7871b417-5bff-4b1b-94b6-bfa843f594bd"
            }
          ]
        },
        {
          "id": "ea18241f-35a4-4757-919e-485798cb20a3",
          "name": "deleteStyleGuide",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/styleguides/:styleGuideId"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "styleGuideId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete the style guide."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8796084-1d17-4354-b214-2f7bd2d704eb"
            }
          ]
        },
        {
          "id": "65464511-cfcb-436b-afd6-53912ade21d0",
          "name": "downloadStyleGuide",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/styleguides/:styleGuideId/download"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "styleGuideId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Download a style guide."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eecf1ba5-f7aa-4c64-a03b-846fe7a6a028"
            }
          ]
        }
      ]
    },
    {
      "name": "Styleguide",
      "item": [
        {
          "id": "798c12d8-501e-4b26-92c7-4dcb8b3acab9",
          "name": "downloadGlobalStyleGuide",
          "request": {
            "url": "http://api.motaword.com/styleguide",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Download your corporate account's global style guide. This endpoint is available only for corporate account customers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64e11bcc-17e9-4c70-bd90-8ce287bd1bea"
            }
          ]
        },
        {
          "id": "d5ac50f0-b8dd-4649-8953-ead6a6fbd9a7",
          "name": "updateGlobalStyleGuide",
          "request": {
            "url": "http://api.motaword.com/styleguide",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "styleguide",
                  "value": "{}",
                  "disabled": false,
                  "description": "Style guide file"
                }
              ]
            },
            "description": "Update your corporate account's global style guide. This endpoint is available only for corporate account customers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0891b0e5-d680-4ee2-baca-9abd4f9122c2"
            }
          ]
        }
      ]
    },
    {
      "name": "Token",
      "item": [
        {
          "id": "2f9db15d-2bd9-40f2-aeb3-f46b6ea04fe4",
          "name": "getAccessToken",
          "request": {
            "url": "http://api.motaword.com/token",
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "HTTP Basic Authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "grant_type",
                  "value": "{}",
                  "disabled": false,
                  "description": "OAuth2 grant type"
                }
              ]
            },
            "description": "MotaWord API is using OAuth2 procedures when authenticating or authorizing your API call. Currently, we only allow Client Credential type flow."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "581ef344-0e8d-44ce-b823-02b815c77d03"
            }
          ]
        }
      ]
    }
  ]
}