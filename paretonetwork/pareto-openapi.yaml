swagger: "2.0"
x-collection-name: ParetoNetwork
x-complete: 1
info:
  title: PARETO NETWORK API
  description: the-pareto-network-api-is-used-by-sentinels-to-catalogue-and-relay-information-between-nodes--interacting-with-a-pareto-sentinel-uses-this-standardized-restful-api--authentication-is-done-using-a-json-web-token-jwt-stored-as-a-secure-browser-cookie--any-restful-client-will-need-to-set-the-cookie--here-is-a-tutorial-for-getting-the-initial-cookie-httpsblog-pareto-networkhowtousetheparetosentinelapi434afb75aace
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sign:
    post:
      summary: Cookie authentication
      description: Test the hash between a message and public key. If the test is
        passed, a cookie is stored. The parameters of this request are gotten from
        MetaMask
      operationId: postSign
      x-api-path-slug: sign-post
      responses:
        200:
          description: OK
      tags:
      - Sign
  /rank:
    get:
      summary: Get the list of all addresses sorted by rank
      description: Get all the addresses sorted by rank. The ranking is gotten from
        the Ethereum score
      operationId: getRank
      x-api-path-slug: rank-get
      responses:
        200:
          description: OK
      tags:
      - Rank
  /auth:
    get:
      summary: Test if user is properly authenticated
      description: Simple authenticated method to determine if user is properly authenticated.
      operationId: getAuth
      x-api-path-slug: auth-get
      responses:
        200:
          description: OK
      tags:
      - Auth
  /unsign:
    post:
      summary: Unsign http client for the current user
      description: Manage unsign proccess. Delete cookie with header set-cookie
      operationId: postUnsign
      x-api-path-slug: unsign-post
      responses:
        200:
          description: OK
      tags:
      - Unsign
  /address:
    get:
      summary: Get the information of the current user
      description: Get the information of the current user. The current user is fetched
        using the auth cookie.
      operationId: getAddress
      x-api-path-slug: address-get
      responses:
        200:
          description: OK
      tags:
      - Address
  /address/{address}:
    get:
      summary: Get the information of a specific user
      description: Get the information of a specific user.
      operationId: getAddressAddress
      x-api-path-slug: addressaddress-get
      parameters:
      - in: path
        name: address
        description: address to use
      responses:
        200:
          description: OK
      tags:
      - Address
      - Address
  /content:
    get:
      summary: Get the content about the actionable investing intels
      description: Get all available content about the actionable investing intels.
      operationId: getContent
      x-api-path-slug: content-get
      responses:
        200:
          description: OK
      tags:
      - Content
  /content/me:
    get:
      summary: Get the content available for current user
      description: Get the content available for current user
      operationId: getContentMe
      x-api-path-slug: contentme-get
      responses:
        200:
          description: OK
      tags:
      - Content
      - Me
  /userinfo:
    get:
      summary: Get the information of the profile user
      description: Get the information of the current user. The current user is fetched
        using the auth cookie.
      operationId: getUserinfo
      x-api-path-slug: userinfo-get
      parameters:
      - in: query
        name: latest
        description: if true force update ranking
      responses:
        200:
          description: OK
      tags:
      - Userinfo
  /userinfo/{address}:
    get:
      summary: Get the profile of a specific user
      description: Get the profile of a specific user.
      operationId: getUserinfoAddress
      x-api-path-slug: userinfoaddress-get
      parameters:
      - in: path
        name: address
        description: address to use
      responses:
        200:
          description: OK
      tags:
      - Userinfo
      - Address
  /updateuser:
    post:
      summary: Update the profile of the current user
      description: Update the profile of the current user
      operationId: postUpdateuser
      x-api-path-slug: updateuser-post
      responses:
        200:
          description: OK
      tags:
      - Updateuser
  /profile-image:
    get:
      summary: Get the image profile
      description: Get the image profile
      operationId: getProfileImage
      x-api-path-slug: profileimage-get
      parameters:
      - in: query
        name: image
        description: resource to be gotten
      responses:
        200:
          description: OK
      tags:
      - Profile
      - Image
  /upload-profile:
    post:
      summary: Upload image
      description: Upload Image
      operationId: postUploadProfile
      x-api-path-slug: uploadprofile-post
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Profile