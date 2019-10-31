{
  "info": {
    "name": "Sugar Sync  API Updating Workspace Information",
    "_postman_id": "66904055-ddd3-441d-933f-a52571fdf1de",
    "description": "An application can update attributes of a workspace by issuing an HTTP PUT request to the URL that representsnthe workspace resource. In addition, the app needs to provide as input, XML that identifies the new attribute values for the workspace.nUpon receiving the PUT request, the SugarSync service examines the input and updates any of the attributes that have been modified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Album",
      "item": [
        {
          "id": "7a433a5b-65e3-48c9-9cda-d304056e6584",
          "name": "retrieving-album-information",
          "request": {
            "url": "http://api.sugarsync.com/album/?max=%7B%7D&order=%7B%7D&start=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about an album, an application submits an HTTP GET request to then          album resource that represents the album."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f13e851c-2ea4-467e-af7a-743956d187b4"
            }
          ]
        }
      ]
    },
    {
      "name": "App",
      "item": [
        {
          "id": "92fb5e74-7192-4690-96b4-3878538ef4bb",
          "name": "creating-a-refresh-token",
          "request": {
            "url": "http://api.sugarsync.com/app-authorization",
            "method": "POST",
            "header": [
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "The length of the request body",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "The content type and character encoding of the response",
                "disabled": false
              },
              {
                "key": "Host",
                "value": "{}",
                "description": "The domain name of the server",
                "disabled": false
              },
              {
                "key": "User-Agent",
                "value": "{}",
                "description": "The client application implementing the network protocol for communication between          the client and server",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "An application needs to be authorized to access a users SugarSync resources through the Platform API.nTo do that, the app needs to create a refresh token. When a user first runs the application, it creates a refresh tokennby submitting a POST request that includes the users credentials to the API.nIf the request is successful, the SugarSync service grants the application permission to access the users account and returns a refresh token.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b74e32cd-c47c-4177-b83d-6960d1f4bc6b"
            }
          ]
        }
      ]
    },
    {
      "name": "Authorization",
      "item": [
        {
          "id": "fc966161-7317-4c2f-805e-aac795e9be25",
          "name": "creating-an-access-token",
          "request": {
            "url": "http://api.sugarsync.com/authorization",
            "method": "POST",
            "header": [
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "The length of the request body",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "The content type and character encoding of the response",
                "disabled": false
              },
              {
                "key": "Host",
                "value": "{}",
                "description": "The domain name of the server",
                "disabled": false
              },
              {
                "key": "User-Agent",
                "value": "{}",
                "description": "The client application implementing the network protocol for communication between          the client and server",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "An application needs to be authorized to access a users SugarSync resources through the Platform API. To do that,nthe app needs to create an access token, which allows the app to access files, folders,nand other resources within a users account. After the token is created, the app needs to specify it in the HTTP request header when it makes a request through the API to access a resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14a8a681-226c-4ef9-aa30-6f2ad1bce406"
            }
          ]
        }
      ]
    },
    {
      "name": "Contact",
      "item": [
        {
          "id": "ad895508-f80f-4c0a-84cf-d527e14af604",
          "name": "retrieving-contact-information",
          "request": {
            "url": "http://api.sugarsync.com/contact/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A contact represents another SugarSync user who has shared a folder or folders with this user.n          To retrieve information about a contact, an application submits an HTTP GET request to then          contact resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9751a7e3-f42f-4b9b-9ee2-baafd6c86151"
            }
          ]
        }
      ]
    },
    {
      "name": "File",
      "item": [
        {
          "id": "bff20c69-fd41-46a6-8bb1-aef138d8c657",
          "name": "retrieving-file-data",
          "request": {
            "url": "http://api.sugarsync.com/file",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve file data, an application submits an HTTP GET request to then          file data resource that represents the data for the file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e003e5a-22bc-4f15-b885-c124d111980a"
            }
          ]
        },
        {
          "id": "0ce6da24-8d23-420c-bd94-c5326a4c27dd",
          "name": "uploading-file-data",
          "request": {
            "url": "http://api.sugarsync.com/file",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "An application can upload data to a file by issuing an HTTP PUT request to thenfile data resource that represents the data for the file.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "073631fd-5179-4247-9ae9-11a9ef179af9"
            }
          ]
        },
        {
          "id": "1db87db9-b92c-4359-8888-bc4b98f8343b",
          "name": "retrieving-file-information",
          "request": {
            "url": "http://api.sugarsync.com/file/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about a file, an application submits an HTTP GET request to then          file resource that represents the file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1b3a0c6-29e2-456f-9b5b-614e724d8c39"
            }
          ]
        },
        {
          "id": "549c3c23-f3ad-4f63-b101-9132b0a8b827",
          "name": "updating-file-information",
          "request": {
            "url": "http://api.sugarsync.com/file/",
            "method": "PUT",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The access token",
                "disabled": false
              },
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "The length of the request body",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "The content type and character encoding of the response",
                "disabled": false
              },
              {
                "key": "Host",
                "value": "{}",
                "description": "The domain name of the server",
                "disabled": false
              },
              {
                "key": "User-Agent",
                "value": "{}",
                "description": "The client application implementing the network protocol for communication between          the client and server",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "An application can update various attributes of a file by issuing an HTTP PUT request to the URL thatnrepresents the file resource. In addition, the app needs to provide as input, XML that identifies the new attribute values for the file. Upon receiving the PUT request, the SugarSync service examines the input and updates any of the attributes that have been modified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6690c1b5-63d9-4471-8bde-b1efe7b8dd83"
            }
          ]
        },
        {
          "id": "5b879972-16ad-4891-8aef-4c1b63e2e50e",
          "name": "creating-a-new-file-version",
          "request": {
            "url": "http://api.sugarsync.com/file/",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "nAn application can create a new version of a file by submitting an HTTP POST request to the URL that represents the version history. The version history URL is returned in the &lt;versions&gt; element whenn retrieving information about a file.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d08908b2-32d3-42a6-913f-8eb939a96bb2"
            }
          ]
        },
        {
          "id": "fde0f687-77d5-4926-84db-0679f839bb4b",
          "name": "deleting-a-file",
          "request": {
            "url": "http://api.sugarsync.com/file/",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "An application can permanently delete a file by issuing an HTTP DELETE request to the URL of thenfile resource.nIts a good idea to precede DELETE requests like this with a caution note in your applications user interface.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d27fd1a9-2c54-4f3d-829f-a43aa07c3235"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "90433c3a-8ebb-47ba-9981-a1fd982ae579",
          "name": "retrieving-folder-information",
          "request": {
            "url": "http://api.sugarsync.com/folder",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about a folder, an application submits an HTTP GET request to then          folder resource that represents the folder."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53739e32-d807-4be1-96fe-558f1e3e2122"
            }
          ]
        },
        {
          "id": "18668525-0d88-4f5d-b7cd-ec8f9f1c3451",
          "name": "retrieving-folder-contents",
          "request": {
            "url": "http://api.sugarsync.com/folder/?max=%7B%7D&order=%7B%7D&start=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve the contents of a folder, an application submits an HTTP GET request to the URLn          that represents the folder contents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "793afc2c-ac4b-402d-98f6-49711403e44f"
            }
          ]
        },
        {
          "id": "44da1d64-f4da-4a51-b725-717799d684e7",
          "name": "updating-folder-information",
          "request": {
            "url": "http://api.sugarsync.com/folder/",
            "method": "PUT",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The access token",
                "disabled": false
              },
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "The length of the request body",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "The content type and character encoding of the response",
                "disabled": false
              },
              {
                "key": "Host",
                "value": "{}",
                "description": "The domain name of the server",
                "disabled": false
              },
              {
                "key": "User-Agent",
                "value": "{}",
                "description": "The client application implementing the network protocol for communication between          the client and server",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "An application can update various attributes of a folder by issuing an HTTP PUT request to the URL thatnrepresents the folder resource. In addition, the app needs to provide as input, XML that identifies the new attribute values for the folder. Upon receiving the PUT request, the SugarSync service examines the input and updates any of the attributes that have been modified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa995daf-c47b-4a0f-927c-5657238ee367"
            }
          ]
        },
        {
          "id": "4fc2d55f-f870-4d65-8474-e4d41ed59ec0",
          "name": "creating-a-folder",
          "request": {
            "url": "http://api.sugarsync.com/folder/",
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The access token",
                "disabled": false
              },
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "The length of the request body",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "The content type and character encoding of the response",
                "disabled": false
              },
              {
                "key": "Host",
                "value": "{}",
                "description": "The domain name of the server",
                "disabled": false
              },
              {
                "key": "User-Agent",
                "value": "{}",
                "description": "The client application implementing the network protocol for communication between          the client and server",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "An application can create a folder within another folder by issuing an HTTP POST request to the URL ofnthe containing folder resource.nIn addition, the application needs to provide as input, XML that identifies the display name of the folder to be created.nNote that an application can create a folder only within another folder, and not directly in a workspace."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42df877b-26bb-410e-81a2-f4635b2fafbe"
            }
          ]
        },
        {
          "id": "8598056c-ae38-4d59-93c1-5509159f07dc",
          "name": "deleting-a-folder",
          "request": {
            "url": "http://api.sugarsync.com/folder/",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "An application can permanantly delete a folder by issuing an HTTP DELETE request to the URL of thenfolder resource.nIts a good idea to precede DELETE requests like this with a caution note in your applications user interface.n"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ce6bd34-1523-4e3c-a15f-436aa3f0e202"
            }
          ]
        }
      ]
    },
    {
      "name": "ReceivedShare",
      "item": [
        {
          "id": "ecbf943b-c19c-4b64-b061-5e6bd1a4381b",
          "name": "retrieving-received-share-information",
          "request": {
            "url": "http://api.sugarsync.com/receivedShare/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about a received share (that is, a shared folder owned by another user and to whichnthis user has been granted access privileges by the owner), an application submits an HTTP GET request to the URLnthat represents the received share resource. The URL is referenced in the &lt;receivedShare&gt; element for the received share in the received shares list.nSee Retrieving the Received Shares List."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b42acb5-90d9-4267-9e8b-3c5510e7006d"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "309b6d50-4247-49c5-89f6-8fe1e97a0415",
          "name": "retrieving-user-information",
          "request": {
            "url": "http://api.sugarsync.com/user?max=%7B%7D&start=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about a SugarSync user, an application submits an HTTP GET request to thenuser resource that represents the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "baf09606-a1e1-49b9-ae6f-55e747c4ad8f"
            }
          ]
        },
        {
          "id": "bca493ec-4569-491c-a504-1bd0df29aa2c",
          "name": "retrieving-received-shares-list",
          "request": {
            "url": "http://api.sugarsync.com/user/?max=%7B%7D&start=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "One of the elements in the representation of a user resource isn&lt;receivedShares&gt;.nThe element contains a link to a list that describes the shared folders that are owned by other users and to which this user has been granted access privileges by those owners. For example:nnn&lt;?xml version=1.0 encoding=UTF-8?&gt;n&lt;user&gt;n  ...n  &lt;receivedShares&gt;https://api.sugarsync.com/user/5664947/receivedShares/contents&lt;/receivedShares&gt;n  ...n&lt;/user&gt;nnn          To retrieve the list, an application submits an HTTP GET request to the link in the &lt;receivedShares&gt;nelement.nn         Requestnn          URLn          The URL that represents the received shares list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e3f5c08-6f2c-4169-a2c2-c465ed869601"
            }
          ]
        }
      ]
    },
    {
      "name": "Workspace",
      "item": [
        {
          "id": "e31b4199-8c6b-4103-a842-479726874749",
          "name": "retrieving-workspace-information",
          "request": {
            "url": "http://api.sugarsync.com/workspace",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve information about a workspace, an application submits an HTTP GET request to then          workspace resource that represents the workspace."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "faa04e26-bbb2-4429-85f5-49f7fd084370"
            }
          ]
        },
        {
          "id": "6880d7d5-109f-4e5f-895d-6c7511c89b2b",
          "name": "retrieving-workspace-contents",
          "request": {
            "url": "http://api.sugarsync.com/workspace/?max=%7B%7D&order=%7B%7D&start=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To retrieve the contents of a workspace, an application submits an HTTP GET request to the URLn          that represents the workspace contents. Note that the contents of a workspace are the sync folders that are mappedntt  to that workspace in SugarSync."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e48c1bf9-fe08-40ff-9e0e-d285e4c44453"
            }
          ]
        },
        {
          "id": "de4f9a95-8bb9-40dc-8ca5-d3cb78ac8bc3",
          "name": "updating-workspace-information",
          "request": {
            "url": "http://api.sugarsync.com/workspace/",
            "method": "PUT",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The access token",
                "disabled": false
              },
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "The length of the request body",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "The content type and character encoding of the response",
                "disabled": false
              },
              {
                "key": "Host",
                "value": "{}",
                "description": "The domain name of the server",
                "disabled": false
              },
              {
                "key": "User-Agent",
                "value": "{}",
                "description": "The client application implementing the network protocol for communication between          the client and server",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "An application can update attributes of a workspace by issuing an HTTP PUT request to the URL that representsnthe workspace resource. In addition, the app needs to provide as input, XML that identifies the new attribute values for the workspace.nUpon receiving the PUT request, the SugarSync service examines the input and updates any of the attributes that have been modified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c7d9611-cdc9-4ac2-af06-ad34383179d6"
            }
          ]
        }
      ]
    }
  ]
}