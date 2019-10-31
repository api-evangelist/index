swagger: "2.0"
x-collection-name: Ge.tt
x-complete: 1
info:
  title: Ge.tt  REST API
  description: the-ge-tt-api-allows-you-to-use-ge-tt-in-your-own-applications--we-believe-that-our-users-should-be-able-to-access-their-files-and-share-their-content-in-their-platform-of-choice--by-using-the-api-developers-are-able-to-easily-put-their-own-content-or-the-content-of-their-users-online--at-the-same-time-they-are-able-to-use-ge-tts-unique-realtime-file-sharing-technology-where-files-are-available-before-they-are-even-uploaded-
  termsOfService: http://ge.tt/terms
  version: "1"
host: open.ge.tt
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /1/files/{sharename}/create:
    post:
      summary: Files Create
      description: 'To upload files to Ge.tt you must first create the file under
        a given share. You do that by posting the filename:'
      operationId: post1FilesSharenameCreate
      x-api-path-slug: 1filessharenamecreate-post
      parameters:
      - in: query
        name: accesstoken
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Files
      - Sharename
      - Create
  /1/files/{sharename}/{fileid}:
    get:
      summary: Files
      description: 'Get the state of a file. This returns the following data:'
      operationId: get1FilesSharenameFile
      x-api-path-slug: 1filessharenamefileid-get
      parameters:
      - in: path
        name: fileid
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Files
      - Sharename
      - Fileid
  /1/files/{sharename}/{fileid}/blob:
    get:
      summary: Files  Blob
      description: Will redirect to the binary content of the file
      operationId: get1FilesSharenameFileBlob
      x-api-path-slug: 1filessharenamefileidblob-get
      parameters:
      - in: path
        name: fileid
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Files
      - Sharename
      - Fileid
      - Blob
  /1/files/{sharename}/{fileid}/blob/thumb:
    get:
      summary: Files  Blob Thumb
      description: Will redirect to a thumbnail of the binary file. Currently only
        available for images.
      operationId: get1FilesSharenameFileBlobThumb
      x-api-path-slug: 1filessharenamefileidblobthumb-get
      parameters:
      - in: path
        name: fileid
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Files
      - Sharename
      - Fileid
      - Blob
      - Thumb
  /1/files/{sharename}/{fileid}/destroy:
    post:
      summary: Files  Destroy
      description: Delete a file and the binary contents.
      operationId: post1FilesSharenameFileDestroy
      x-api-path-slug: 1filessharenamefileiddestroy-post
      parameters:
      - in: query
        name: accesstoken
      - in: path
        name: fileid
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Files
      - Sharename
      - Fileid
      - Destroy
  /1/files/{sharename}/{fileid}/upload:
    get:
      summary: Files  Upload
      description: Get upload urls to the file. This returns a new PUT and POST url
        for you to upload the file to.nOBS You can also choose to use the put- or
        posturl that you were previously given to override the file.
      operationId: get1FilesSharenameFileUpload
      x-api-path-slug: 1filessharenamefileidupload-get
      parameters:
      - in: query
        name: accesstoken
      - in: path
        name: fileid
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Files
      - Sharename
      - Fileid
      - Upload
  /1/shares:
    get:
      summary: Shares
      description: 'Returns all your shares and the containing files:'
      operationId: get1Shares
      x-api-path-slug: 1shares-get
      parameters:
      - in: query
        name: accesstoken
      responses:
        200:
          description: OK
      tags:
      - Shares
  /1/shares/create:
    post:
      summary: Shares Create
      description: 'Creates a new share. The request body is optional but can look
        like:'
      operationId: post1SharesCreate
      x-api-path-slug: 1sharescreate-post
      parameters:
      - in: query
        name: accesstoken
      responses:
        200:
          description: OK
      tags:
      - Shares
      - Create
  /1/shares/{sharename}:
    get:
      summary: Shares
      description: Lists a share.
      operationId: get1SharesSharename
      x-api-path-slug: 1sharessharename-get
      parameters:
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Shares
      - Sharename
  /1/shares/{sharename}/destroy:
    post:
      summary: Shares Destroy
      description: Delete a share and all of its files.
      operationId: post1SharesSharenameDestroy
      x-api-path-slug: 1sharessharenamedestroy-post
      parameters:
      - in: query
        name: accesstoken
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Shares
      - Sharename
      - Destroy
  /1/shares/{sharename}/update:
    post:
      summary: Shares Update
      description: Updates a share. Currently you can only update the title
      operationId: post1SharesSharenameUpdate
      x-api-path-slug: 1sharessharenameupdate-post
      parameters:
      - in: query
        name: accesstoken
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Shares
      - Sharename
      - Update
  /1/users/login:
    post:
      summary: Users Login
      description: 'The API is based on oauth with an xauth handshake. The request
        body looks like this:'
      operationId: post1UsersLogin
      x-api-path-slug: 1userslogin-post
      responses:
        200:
          description: OK
      tags:
      - Users
      - Login
  /1/users/me:
    get:
      summary: Users Me
      description: 'Returns your user information:'
      operationId: get1UsersMe
      x-api-path-slug: 1usersme-get
      parameters:
      - in: query
        name: accesstoken
      responses:
        200:
          description: OK
      tags:
      - Users
      - Me