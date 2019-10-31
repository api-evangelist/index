{
  "info": {
    "name": "Ge.tt  REST API Users Me",
    "_postman_id": "b9611d54-4406-47a4-937d-0ebc1fa6513a",
    "description": "Returns your user information:",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Files",
      "item": [
        {
          "id": "142eb99b-7cc1-41c6-980b-22e75ab8ead2",
          "name": "post1FilesSharenameCreate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/create"
              ],
              "query": [
                {
                  "key": "accesstoken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "To upload files to Ge.tt you must first create the file under a given share. You do that by posting the filename:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58a0286e-5492-4846-924d-6455f2896c19"
            }
          ]
        },
        {
          "id": "920b4967-0bcd-49d5-88f5-da31827bbbe6",
          "name": "get1FilesSharenameFile",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/:fileid"
              ],
              "variable": [
                {
                  "id": "fileid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the state of a file. This returns the following data:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f23bb61-fad6-4a6b-a2be-55120e26c48a"
            }
          ]
        },
        {
          "id": "0379bc53-ae85-43cd-b29f-479fc60c7131",
          "name": "get1FilesSharenameFileBlob",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/:fileid/blob"
              ],
              "variable": [
                {
                  "id": "fileid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Will redirect to the binary content of the file"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2eef8165-1b71-4985-840e-b46fa1a2d57e"
            }
          ]
        },
        {
          "id": "ab7c501d-5832-4992-81a8-84bce58aae6b",
          "name": "get1FilesSharenameFileBlobThumb",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/:fileid/blob/thumb"
              ],
              "variable": [
                {
                  "id": "fileid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Will redirect to a thumbnail of the binary file. Currently only available for images."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49501789-c460-4794-87b6-47e5a59e62d0"
            }
          ]
        },
        {
          "id": "ff8a2416-730a-4f93-b6a3-f5d76e572009",
          "name": "post1FilesSharenameFileDestroy",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/:fileid/destroy"
              ],
              "query": [
                {
                  "key": "accesstoken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "fileid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a file and the binary contents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f14cbbfc-3a3f-4807-892e-9f15eb61140b"
            }
          ]
        },
        {
          "id": "f61f0a95-68cc-4aa1-aa5a-6d087943b431",
          "name": "get1FilesSharenameFileUpload",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/:fileid/upload"
              ],
              "query": [
                {
                  "key": "accesstoken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "fileid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get upload urls to the file. This returns a new PUT and POST url for you to upload the file to.nOBS You can also choose to use the put- or posturl that you were previously given to override the file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0435286-a146-4c3d-b180-b0792ea0a201"
            }
          ]
        }
      ]
    },
    {
      "name": "Shares",
      "item": [
        {
          "id": "28688ae6-4b23-4d49-8d6d-e49f8bb64250",
          "name": "get1Shares",
          "request": {
            "url": "http://open.ge.tt/1/1/shares?accesstoken=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all your shares and the containing files:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3dea3d0-e396-4312-8776-5819d9bb8a1c"
            }
          ]
        },
        {
          "id": "5623d866-7893-40b4-9f24-6b8a4e6f2c3d",
          "name": "post1SharesCreate",
          "request": {
            "url": "http://open.ge.tt/1/1/shares/create?accesstoken=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new share. The request body is optional but can look like:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13bda8bc-f29d-4db4-bc49-776e15f05ba2"
            }
          ]
        },
        {
          "id": "4362d3da-cb58-478a-a9c4-454073ae0a24",
          "name": "get1SharesSharename",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/shares/:sharename"
              ],
              "variable": [
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists a share."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f23c868-5e8f-472d-ae09-d6fcb34c010d"
            }
          ]
        },
        {
          "id": "f350db11-b9e6-4e80-918f-7c9b828b8bae",
          "name": "post1SharesSharenameDestroy",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/shares/:sharename/destroy"
              ],
              "query": [
                {
                  "key": "accesstoken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a share and all of its files."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0f8dbc2-f1df-4591-99f6-7e53a8fb7d5c"
            }
          ]
        },
        {
          "id": "bc99195f-51c7-4c4d-9db5-9f99873635b2",
          "name": "post1SharesSharenameUpdate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/shares/:sharename/update"
              ],
              "query": [
                {
                  "key": "accesstoken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a share. Currently you can only update the title"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb9c66b4-6dfc-416e-8958-2488bbebf94c"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "feef3833-da76-4015-b181-6ac968b0b06c",
          "name": "post1UsersLogin",
          "request": {
            "url": "http://open.ge.tt/1/1/users/login",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "The API is based on oauth with an xauth handshake. The request body looks like this:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a900c2e7-0c76-4075-ac4c-ab6000d42173"
            }
          ]
        },
        {
          "id": "1d735a6f-2c27-48bc-a33f-c61f0e060ac8",
          "name": "get1UsersMe",
          "request": {
            "url": "http://open.ge.tt/1/1/users/me?accesstoken=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns your user information:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8d67218-34f8-42a3-b773-3d95761a8e9d"
            }
          ]
        }
      ]
    }
  ]
}