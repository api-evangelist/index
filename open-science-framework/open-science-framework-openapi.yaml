swagger: "2.0"
x-collection-name: Open Science Framework
x-complete: 1
info:
  title: Open Science Framework
  description: osf-provides-free-and-open-source-project-management-support-for-researchers-across-the-entire-research-lifecycle--as-a-collaboration-tool-osf-helps-researchers-work-on-projects-privately-with-a-limited-number-of-collaborators-and-make-parts-of-their-projects-public-or-make-all-the-project-publicly-accessible-for-broader-dissemination--as-a-workflow-system-osf-enables-connections-to-the-many-services-researchers-already-use-to-streamline-their-process-and-increase-efficiency--as-a-flexible-repository-it-can-store-and-archive-research-data-protocols-and-materials--
  contact:
    name: OSF
    url: https://osf.io/support
    email: support@osf.io
  version: "2.0"
host: test-api.osf.io
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    get:
      summary: Root
      description: |-
        Welcome to the Open Science Framework API. With this API you can access users, projects, components, logs, and files from the [Open Science Framework](https://osf.io/). The Open Science Framework (OSF) is a free, open-source service maintained by the [Center for Open Science](http://cos.io/).

        #### Returns
        A JSON object with `meta` and `links` keys.

        The `meta` key contains information such as a welcome message from the API, the specified version of the request, and the full representation of the current user, if authentication credentials were provided in the request.

        The `links` key contains links to the following entity collections: [addons](), [collections](), [institutions](#Institutions_institutions_list), [licenses](#Licenses_license_list), [metaschemas](), [nodes](#Nodes_nodes_list), [registrations](), [users](#Users_users_list)
      operationId: base_read
      x-api-path-slug: get
      responses:
        200:
          description: OK
      tags:
      - Root
  /actions/:
    get:
      summary: Actions
      description: |-
        A log can have one of many actions. The complete list of loggable actions (in the format {identifier}: {description}) is as follows:
        * `project_created`: A Node is created
        * `project_registered`: A Node is registered
        * `project_deleted`: A Node is deleted
        * `created_from`: A Node is created using an existing Node as a template
        * `pointer_created`: A Pointer is created
        * `pointer_forked`: A Pointer is forked
        * `pointer_removed`: A Pointer is removed
        * `node_removed`: A component is deleted
        * `node_forked`: A Node is forked
        ---
        * `made_public`: A Node is made public
        * `made_private`: A Node is made private
        * `tag_added`: A tag is added to a Node
        * `tag_removed`: A tag is removed from a Node
        * `edit_title`: A Node's title is changed
        * `edit_description`: A Node's description is changed
        * `updated_fields`: One or more of a Node's fields are changed
        * `external_ids_added`: An external identifier is added to a Node (e.g. DOI, ARK)
        * `view_only_link_added`: A view-only link was added to a Node
        * `view_only_link_removed`:  A view-only link was removed from a Node
        ---
        * `contributor_added`: A Contributor is added to a Node
        * `contributor_removed`: A Contributor is removed from a Node
        * `contributors_reordered`: A Contributor's position in a Node's bibliography is changed
        * `permissions_updated`: A Contributor`s permissions on a Node are changed
        * `made_contributor_visible`: A Contributor is made bibliographically visible on a Node
        * `made_contributor_invisible`: A Contributor is made bibliographically invisible on a Node
        ---
        * `wiki_updated`: A Node's wiki is updated
        * `wiki_deleted`: A Node's wiki is deleted
        * `wiki_renamed`: A Node's wiki is renamed
        * `made_wiki_public`: A Node's wiki is made public
        * `made_wiki_private`: A Node's wiki is made private
        ---
        * `addon_added`: An add-on is linked to a Node
        * `addon_removed`: An add-on is unlinked from a Node
        * `addon_file_moved`: A File in a Node's linked add-on is moved
        * `addon_file_copied`: A File in a Node's linked add-on is copied
        * `addon_file_renamed`: A File in a Node's linked add-on is renamed
        * `node_authorized`: An addon is authorized for a project
        * `node_deauthorized`: An addon is deauthorized for a project
        * `folder_created`: A Folder is created in a Node's linked add-on
        * `file_added`: A File is added to a Node's linked add-on
        * `file_updated`: A File is updated on a Node's linked add-on
        * `file_removed`: A File is removed from a Node's linked add-on
        * `file_restored`: A File is restored in a Node's linked add-on
        ---
        * `comment_added`: A Comment is added to some item
        * `comment_removed`: A Comment is removed from some item
        * `comment_updated`: A Comment is updated on some item
        ---
        * `embargo_initiated`: An embargoed Registration is proposed on a Node
        * `embargo_approved`: A proposed Embargo of a Node is approved
        * `embargo_cancelled`: A proposed Embargo of a Node is cancelled
        * `embargo_completed`: A proposed Embargo of a Node is completed
        * `retraction_initiated`: A Withdrawal of a Registration is proposed
        * `retraction_approved`: A Withdrawal of a Registration is approved
        * `retraction_cancelled`: A Withdrawal of a Registration is cancelled
        * `registration_initiated`: A Registration of a Node is proposed
        * `registration_approved`: A proposed Registration is approved
        * `registration_cancelled`: A proposed Registration is cancelled
      operationId: logs_actions
      x-api-path-slug: actions-get
      responses:
        200:
          description: OK
      tags:
      - Actions
  /addons/:
    get:
      summary: List all addons
      description: |-
        A paginated list of addons configurable with the OSF
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 addons. Each resource in the array is a separate addon object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        This request should never return an error.
      operationId: addons_list
      x-api-path-slug: addons-get
      responses:
        200:
          description: OK
      tags:
      - Addons
  /citations/styles/:
    get:
      summary: List all citation styles
      description: |-
        A paginated list of all standard citation styles available for rendering citations.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 citation styles. Each resource in the array is a separate citation syle and contains the full representation of the citation style object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        This request should never return an error.
        #### Filtering
        You can optionally request that the response only include citation styles that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/citations/styles/?filter[title]=open.

        Citation styles may be filtered by their `id`, `title`, `short-title`, and `summary`.
      operationId: citations_styles_list
      x-api-path-slug: citationsstyles-get
      responses:
        200:
          description: OK
      tags:
      - Citations
      - Styles
  /citations/styles/{style_id}/:
    get:
      summary: Retrieve a citation style
      description: |-
        Retrieves the details of a citation style.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the requested citation style, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: citations_styles_read
      x-api-path-slug: citationsstylesstyle-id-get
      parameters:
      - in: path
        name: style_id
        description: The unique identifier of the citation style
      responses:
        200:
          description: OK
      tags:
      - Citations
      - Styles
      - Style
  /comments/{comment_id}/:
    delete:
      summary: Delete a comment
      description: |-
        Deletes a comment. This action can be undone by setting deleted to False in a comment update request.
        #### Returns
        If the request is successful, no content is returned.

        If the request is unsuccessful, a JSON object with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: comments_delete
      x-api-path-slug: commentscomment-id-delete
      parameters:
      - in: path
        name: comment_id
        description: The unique identifier of the comment you wish to delete
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Comment
    get:
      summary: Retrieve a comment
      description: |-
        Retrieves the details of a comment
        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested comment, if the request was successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: comments_read
      x-api-path-slug: commentscomment-id-get
      parameters:
      - in: path
        name: comment_id
        description: The unique identifier of the comment you wish to retrieve
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Comment
    put:
      summary: Update a comment
      description: |-
        Updates the specified comment by setting the values of the parameters passed. Any parameters not provided will be left unchanged.
        #### Returns
        Returns JSON with a `data` key containing the new representation of the updated comment, if the request is successful.

        If the request is unsuccessful, JSON with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: comments_put
      x-api-path-slug: commentscomment-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: comment_id
        description: The unique identifier of the comment you wish to update
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Comment
  /files/{file_id}/:
    get:
      summary: Retrieve a file
      description: |-
        Retrieves the details of a file (or folder)
        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested file, if the request was successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
        ###Waterbutler API actions

        Files can be modified through the Waterbutler API routes found in `links` (`new_folder`, `move`, `upload`, `download`, and `delete`).

        #### Download (files)

        To download a file, issue a GET request against the download link. The response will have the Content-Disposition header set, which will will trigger a download in a browser.

        #### Create Subfolder (folders)

        You can create a subfolder of an existing folder by issuing a PUT request against the new_folder link. The ?kind=folder portion of the query parameter is already included in the new_folder link. The name of the new subfolder should be provided in the name query parameter. The response will contain a WaterButler folder entity. If a folder with that name already exists in the parent directory, the server will return a 409 Conflict error response.

        #### Upload New File (folders)


          To upload a file to a folder, issue a PUT request to the folder's upload link with the raw file data in the request body, and the kind and name query parameters set to 'file' and the desired name of the file. The response will contain a WaterButler file entity that describes the new file. If a file with the same name already exists in the folder, the server will return a 409 Conflict error response.


        #### Update Existing File (file)

        To update an existing file, issue a PUT request to the file's upload link with the raw file data in the request body and the kind query parameter set to "file". The update action will create a new version of the file. The response will contain a WaterButler file entity that describes the updated file.

        #### Rename (files, folders)

        To rename a file or folder, issue a POST request to the move link with the action body parameter set to "rename" and the rename body parameter set to the desired name. The response will contain either a folder entity or file entity with the new name.

        #### Move & Copy (files, folders)

        Move and copy actions both use the same request structure, a POST to the move url, but with different values for the action body parameters. The path parameter is also required and should be the OSF path attribute of the folder being written to. The rename and conflict parameters are optional. If you wish to change the name of the file or folder at its destination, set the rename parameter to the new name. The conflict param governs how name clashes are resolved. Possible values are replace and keep. replace is the default and will overwrite the file that already exists in the target folder. keep will attempt to keep both by adding a suffix to the new file's name until it no longer conflicts. The suffix will be ' (x)' where x is a increasing integer starting from 1. This behavior is intended to mimic that of the OS X Finder. The response will contain either a folder entity or file entity with the new name.
        Files and folders can also be moved between nodes and providers. The resource parameter is the id of the node under which the file/folder should be moved. It must agree with the path parameter, that is the path must identify a valid folder under the node identified by resource. Likewise, the provider parameter may be used to move the file/folder to another storage provider, but both the resource and path parameters must belong to a node and folder already extant on that provider. Both resource and provider default to the current node and providers.
        If a moved/copied file is overwriting an existing file, a 200 OK response will be returned. Otherwise, a 201 Created will be returned.

        #### Delete (file, folders)

        To delete a file or folder send a DELETE request to the delete link. Nothing will be returned in the response body.
      operationId: files_detail
      x-api-path-slug: filesfile-id-get
      parameters:
      - in: path
        name: file_id
        description: The unique identifier of the file you wish to retrieve
      responses:
        200:
          description: OK
      tags:
      - Files
      - File
    patch:
      summary: Update a file
      description: |-
        Updates the specified file by setting the values of the parameters passed. Any parameters not provided will be left unchanged.
        #### Returns
        Returns JSON with a `data` key containing the new representation of the updated file, if the request is successful.

        If the request is unsuccessful, JSON with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: files_patch
      x-api-path-slug: filesfile-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: file_id
        description: The unique identifier of the file you wish to update
      responses:
        200:
          description: OK
      tags:
      - Files
      - File
  /files/{file_id}/versions/:
    get:
      summary: List all file versions
      description: |-
        A paginated list of all file versions.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 file versions. Each resource in the array is a separate file version object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: files_versions
      x-api-path-slug: filesfile-idversions-get
      parameters:
      - in: path
        name: file_id
        description: The unique identifier of the file from which you want to retrieve
          versions
      responses:
        200:
          description: OK
      tags:
      - Files
      - File
      - Versions
  /files/{file_id}/versions/{version_id}/:
    get:
      summary: Retrieve a file version
      description: |-
        Retrieves the details of a file version
        ####Returns

        Returns a JSON object with a `data` key containing the representation of the requested file, if the request was successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: files_version_detail
      x-api-path-slug: filesfile-idversionsversion-id-get
      parameters:
      - in: path
        name: file_id
        description: The unique identifier of the file from which you want to retrieve
          versions
      - in: path
        name: version_id
        description: The file version number you want to retrieve
      responses:
        200:
          description: OK
      tags:
      - Files
      - File
      - Versions
      - Version
  /institutions/:
    get:
      summary: List all institutions
      description: |-
        A paginated list of all verified institutions.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 institutions. Each resource in the array is a separate institution object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        This request should never return an error.
        #### Filtering
        You can optionally request that the response only include institutions that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/institutions/?filter[id]=cos.

        Institutions may be filtered by their `id`, `name`, and `auth_url`
      operationId: institutions_list
      x-api-path-slug: institutions-get
      responses:
        200:
          description: OK
      tags:
      - Institutions
  /institutions/{institution_id}/:
    get:
      summary: Retrieve an institution
      description: |-
        Retrieves the details of an institution
        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested institution, if the request was successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: institutions_detail
      x-api-path-slug: institutionsinstitution-id-get
      parameters:
      - in: path
        name: institution_id
        description: The unique identifier of the institution you wish to retrieve
      responses:
        200:
          description: OK
      tags:
      - Institutions
      - Institution
  /institutions/{institution_id}/nodes/:
    get:
      summary: List all affiliated nodes
      description: |-
        A paginated list of all nodes affiliated with an institution.
        #### Versioning
        As of version `2.2`, affiliated components (in addition to affiliated top-level projects) are returned from this endpoint.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 nodes. Each resource in the array is a separate nodes object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
        #### Filtering
        You can optionally request that the response only include nodes that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/institutions/cos/nodes?filter[title]=science.

        Nodes may be filtered by their `id`, `title`, `description`, `public`, `tags`, `category`, `date_created`, `date_modified`, `root`, `parent`, `contributors`, and `preprint`
      operationId: institutions_node_list
      x-api-path-slug: institutionsinstitution-idnodes-get
      parameters:
      - in: path
        name: institution_id
        description: The unique identifier of the institution you wish to retrieve
      responses:
        200:
          description: OK
      tags:
      - Institutions
      - Institution
      - Nodes
  /institutions/{institution_id}/registrations/:
    get:
      summary: List all affiliated registrations
      description: |-
        A paginated list of all registrations affiliated with an institution.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 registrations. Each resource in the array is a separate users object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
        #### Filtering
        You can optionally request that the response only include registrations that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/institutions/cos/registrations?filter[title]=science.

        Registrations may be filtered by their  `id`, `title`, `description`, `public`, `tags`, `category`, `date_created`, `date_modified`, `root`, `parent`, `contributors`, and `preprint`
      operationId: institutions_registration_list
      x-api-path-slug: institutionsinstitution-idregistrations-get
      parameters:
      - in: path
        name: institution_id
        description: The unique identifier of the institution you wish to retrieve
      responses:
        200:
          description: OK
      tags:
      - Institutions
      - Institution
      - Registrations
  /institutions/{institution_id}/users/:
    get:
      summary: List all affiliated users
      description: |-
        A paginated list of all users affiliated with an institution.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 users. Each resource in the array is a separate users object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
        #### Filtering
        You can optionally request that the response only include users that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/institutions/cos/users?filter[family_name]=Nosek.

        Users may be filtered by their `id`, `full_name`, `given_name`, `middle_names`, and `family_name`
      operationId: institutions_users_list
      x-api-path-slug: institutionsinstitution-idusers-get
      parameters:
      - in: path
        name: institution_id
        description: The unique identifier of the institution you wish to retrieve
      responses:
        200:
          description: OK
      tags:
      - Institutions
      - Institution
      - Users
  /license/{license_id}/:
    get:
      summary: Retrieve a license
      description: |-
        Retrieves the details of a license.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the requested license, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: licenses_read
      x-api-path-slug: licenselicense-id-get
      parameters:
      - in: path
        name: license_id
        description: The unique identifier of the license
      responses:
        200:
          description: OK
      tags:
      - License
      - License
  /licenses/:
    get:
      summary: List all licenses
      description: |-
        A paginated list of licenses. The returned licenses are sorted by their name.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.
        The `data` key contains an array of 10 licenses. Each resource in the array is a separate license object and contains the full representation of the license, meaning additional requests to a license's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        This request should never return an error.
        #### Filtering
        You can optionally request that the response only include licenses that match your filters by utilizing the `filter` query parameter, e.g. [https://api.osf.io/v2/licenses/?filter[name]=apache](https://api.osf.io/v2/licenses/?filter[name]=apache).

        Licenses may be filtered by their `id`, and `name`.
      operationId: license_list
      x-api-path-slug: licenses-get
      responses:
        200:
          description: OK
      tags:
      - Licenses
  /logs/{log_id}/:
    get:
      summary: Retrieve a log
      description: |-
        Retrieves the details of a log.
        A log is permanent immutable record of a node's history. A log is created when a user performs one of many actions. See the [actions](#Logs_logs_actions) section for more details.
        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested log, if the request was successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: logs_read
      x-api-path-slug: logslog-id-get
      parameters:
      - in: path
        name: log_id
        description: The unique identifier of the log you wish to retrieve
      responses:
        200:
          description: OK
      tags:
      - Logs
      - Log
  /metaschemas/:
    get:
      summary: List all metaschemas
      description: |-
        A paginated list of all active metaschemas.
        Metaschemas describe the supplemental questions that accompany a registration.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 metaschemas. Each resource in the array is a separate metaschema object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        This request should never return an error.
      operationId: metaschemas_list
      x-api-path-slug: metaschemas-get
      responses:
        200:
          description: OK
      tags:
      - Metaschemas
  /metaschemas/{metaschema_id}:
    get:
      summary: Retrieve a metaschema
      description: |-
        Retrieves the details of a given metaschema.

        Metaschemas describe the supplemental questions that accompany a registration.

        #### Returns
        Returns a JSON object with a `data` key containing the representation of the requested metaschema, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: metaschemas_read
      x-api-path-slug: metaschemasmetaschema-id-get
      parameters:
      - in: path
        name: metaschema_id
        description: The unique identifier of the metaschema
      responses:
        200:
          description: OK
      tags:
      - Metaschemas
      - Metaschema
  /nodes/:
    get:
      summary: List all nodes
      description: |-
        A paginated list of nodes, representing projects and components, on the OSF.

        The returned nodes are those which are public or which the user has access to view.

        The returned nodes are sorted by their `date_modified`, with the most recently updated nodes appearing first.

        Registrations cannot be accessed through this endpoint (use the [registrations](#Registrations_registrations_list) endpoints instead).
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 nodes. Each resource in the array is a separate node object and contains the full representation of the node, meaning additional requests to a node's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        This request should never return an error.
        #### Filtering
        You can optionally request that the response only include nodes that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/nodes/?filter[title]=reproducibility.

        Nodes may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, `preprint`, and `contributors`.

        Most fields are string fields and will be filtered using simple substring matching. Public and preprint are boolean fields, and can be filtered using truthy values, such as **true**, **false**, **0** or **1**. Note that quoting true or false in the query will cause the match to fail.
      operationId: nodes_list
      x-api-path-slug: nodes-get
      responses:
        200:
          description: OK
      tags:
      - Nodes
    post:
      summary: Create a node
      description: |-
        Creates a new node.

        On the OSF, nodes are considered **projects** or **components**. The difference between a project and a component is that a project is a top-level node, and a component is a child of a project.

        Additionally, nodes have a `category` field that includes **project** as an option. The categorization determines what icon is displayed with the node on the OSF, and helps with search organization. Projects (top-level nodes) may have a category other than project, and components (children) may have a category of **project**.
        #### Required
        Required fields for creating a node include:

        &nbsp;&nbsp;&nbsp;&nbsp`title`

        &nbsp;&nbsp;&nbsp;&nbsp`category`

        Note: Nodes default to **private** unless the `public` field is explicitly set to **true** in the request payload.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the created node, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_create
      x-api-path-slug: nodes-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Nodes
  /nodes/{node_id}/:
    delete:
      summary: Delete a node
      description: |-
        Permanently deletes a node. This action cannot be undone.
        #### Permissions
        Only project administrators may delete a node. Attempting to delete a node for which you are not an administrator will result in a **403 Forbidden** response.
        #### Returns
        If the request is successful, no content is returned.

        If the request is unsuccessful, a JSON object with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_delete
      x-api-path-slug: nodesnode-id-delete
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
    get:
      summary: Retrieve a node
      description: |-
        Retrieves the details of a given node (project or component).
        #### Permissions
        Only project contributors may retrieve the details of a private node. Attempting to retreive a private node for which you are not a contributor will result in a **403 Forbidden** response.

        Authentication is not required to view the details of a public node, as public nodes give read-only access to everyone.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the requested node, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_read
      x-api-path-slug: nodesnode-id-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
    patch:
      summary: Update a node
      description: |-
        Updates a node by setting the values of the attributes specified in the request body. Any unspecified attributes will be left unchanged.

        Nodes can be updated with either a **PUT** or **PATCH** request. The `title` and `category` fields are mandatory in a **PUT** request, and optional in a **PATCH**.
        #### Permissions
        Only write contributors may update a node. Attempting to update a node for which you do not have write access will result in a **403 Forbidden** response.
        #### Returns
        Returns a JSON object with a `data` key containing the new representation of the updated node, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_partial_update
      x-api-path-slug: nodesnode-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
  /nodes/{node_id}/addons/:
    get:
      summary: List all addons
      description: |-
        A paginated list of addons connected to the given node or project.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of at most 10 addon objects. Each resource in the array is a separate addon object and contains the full representation of the addon, meaning additional requests to a addon's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
      operationId: nodes_addons_list
      x-api-path-slug: nodesnode-idaddons-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Addons
  /nodes/{node_id}/addons/{provider}/:
    get:
      summary: Retrieve an addon
      description: |-
        Retrieve details of an individual addon connected to this node.
        #### Permissions
        NodeSettings that are attached to public nodes will give read-only access to everyone. Private nodes require explicit read permission. Write and admin access are the same for public and private nodes. Administrators on a parent node have implicit read permissions for all child nodes.
        Any users with write or admin access to the node are able to deauthorize an enabled addon, but only the addon authorizer is able to change the configuration (i.e. selected folder) of an already-configured NodeSettings entity.
        #### Returns
        Returns a JSON object with a `data` key containing the details of the requested addon, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_addon_read
      x-api-path-slug: nodesnode-idaddonsprovider-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      - in: path
        name: provider
        description: The unique identifier of the addon
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Addons
      - Provider
    patch:
      summary: Update an addon
      description: |-
        Updates a node addon by setting the values of the attributes specified in the request body. Any unspecified attributes will be left unchanged.

        Node addon can be updated with either a **PUT** or **PATCH** request. The `external_account_id`, `enabled`, and `folder_id` fields are mandatory in a **PUT**, and optional in **PATCH**. Non-string values will be accepted and stringified, however we make no promises about the stringification output.

        To delete or deauthorize a node addon, issue a **PUT** with all fields set to `null` or `False`, or a **PATCH** with enabled set `False`.
        #### Permissions
        NodeSettings that are attached to public nodes will give read-only access to everyone. Private nodes require explicit read permission. Write and admin access are the same for public and private nodes. Administrators on a parent node have implicit read permissions for all child nodes.
        Any users with write or admin access to the node are able to deauthorize an enabled addon, but only the addon authorizer is able to change the configuration (i.e. selected folder) of an already-configured NodeSettings entity.

        #### Returns
        Returns a JSON object with a `data` key containing the new representation of the updated node addon, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_node_addon_update
      x-api-path-slug: nodesnode-idaddonsprovider-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: node_id
        description: The unique identifier of the node
      - in: path
        name: provider
        description: The unique identifier of the addon
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Addons
      - Provider
  /nodes/{node_id}/addons/{provider}/folders/:
    get:
      summary: List all addon folders
      description: |-
        A paginated list of folders retrieved from the associated third-party (provider) service.
        #### Permissions
        Folders are visible only to the user that authorized the addon.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of addon folder objects. Each resource in the array is a separate addon folder object and contains the full representation of the addon folder, meaning additional requests to a addon folder's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
      operationId: nodes_addons_folders_list
      x-api-path-slug: nodesnode-idaddonsproviderfolders-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      - in: path
        name: provider
        description: The unique identifier of the provider
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Addons
      - Provider
      - Folders
  /nodes/{node_id}/children/:
    get:
      summary: List all child nodes
      description: |-
        A paginated list of the next level child nodes for the given node. The returned nodes are sorted by their `date_modified`, with the most recently updated child nodes appearing first.

        The list will include child nodes that are public, as well as child nodes that are private, if the authenticated user has permission to view them.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 child nodes. If the given node has zero child nodes, the `data` key will contain an empty array. Each resource in the array is a separate node object and contains the full representation of the child node, meaning additional requests to the child node's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        This request should never return an error.
        #### Filtering
        You can optionally request that the response only include nodes that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/nodes/ezcuj/children/?filter[title]=reproducibility.

        Nodes may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, `preprint`, and `contributors`.

        Most fields are string fields and will be filtered using simple substring matching. Public and preprint are boolean fields, and can be filtered using truthy values, such as **true**, **false**, **0** or **1**. Note that quoting true or false in the query will cause the match to fail.
      operationId: nodes_children_list
      x-api-path-slug: nodesnode-idchildren-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Children
    post:
      summary: Create a child node
      description: |-
        Creates a new child node.

        Note: Creating a child node via this endpoint will function the same as creating a node via the node list endpoint, but the child node will have the given node set as its parent.
        #### Permissions
        Only write contributors may create children nodes.
        #### Required
        Required fields for creating a node include:

        &nbsp;&nbsp;&nbsp;&nbsp`title`

        &nbsp;&nbsp;&nbsp;&nbsp`category`

        Note: nodes default to **private** unless the `public` field is explicitly set to **true** in the request payload.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the created node, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_children_create
      x-api-path-slug: nodesnode-idchildren-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Children
  /nodes/{node_id}/citation/:
    get:
      summary: Retrieve citation details
      description: |-
        The citation details for a node, in CSL format.
        #### Returns
        Returns a JSON object with a `data` key that contains the representation of the details necessary for the node citation.
      operationId: nodes_citation_list
      x-api-path-slug: nodesnode-idcitation-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Citation
  /nodes/{node_id}/citation/{style_id}/:
    get:
      summary: Retrieve a styled citation
      description: |-
        The citation for a node in a specific style.
        #### Returns
        Returns a JSON object with a `data` key that contains the representation of the node citation, in the requested style.
      operationId: nodes_citation_read
      x-api-path-slug: nodesnode-idcitationstyle-id-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      - in: path
        name: style_id
        description: The unique identifier of the citation style
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Citation
      - Style
  /nodes/{node_id}/comments/:
    get:
      summary: List all comments
      description: |-
        A paginated list of comments related to a given node.

        The returned comments are sorted by their creation date, with the most recent comments appearing first.
        ####Permissions
        Comments on public nodes are given read-only access to everyone.

        If the node comment-level is `private`, only contributors have permission to comment.

        If the comment-level is `public`, any logged-in OSF user can comment.

        Comments on private nodes are only visible to contributors and administrators on the parent node.
        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of comment objects. Each resource in the array is a separate comment object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        #### Filtering
        You can optionally request that the response only include comments that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/nodes/ezcuj/comments/?filter[target_id]=jg7sezmdnt93

        Nodes may be filtered by their `deleted`, `target_id`, `date_created`, `date_modified`.

        Most fields are string fields and will be filtered using simple substring matching. Public and preprint are boolean fields, and can be filtered using truthy values, such as **true**, **false**, **0** or **1**. Note that quoting `true` or `false` in the query will cause the match to fail.
      operationId: nodes_comments_list
      x-api-path-slug: nodesnode-idcomments-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Comments
    post:
      summary: Create a comment
      description: |-
        Create a comment on a given node overview page or a reply to a comment on that node.

        To create a comment on the node overview page, the target `type` would be "nodes" and the target `id` would be the node `id`.

        To reply to a comment on this node, the target `type` would be "comments" and the target `id` would be the `id` of the comment to reply to.
        ####Required
        A relationship object with a `data` key, containing the target (`comments` or `nodes`) type and a target `id` is required.
        In addition, the `content` attribute describing the relationship between the node and the comment is required.
        ####Returns
        Returns a JSON object with a data key containing the representation of the new comment, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_comment_create
      x-api-path-slug: nodesnode-idcomments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: node_id
        description: The unique identifier of the node you want to comment on
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Comments
  /nodes/{node_id}/contributors/:
    get:
      summary: List all contributors
      description: |-
        A paginated list of the node's contributors, sorted by their index.

        Contributors are users who can make changes to the node or, in the case of private nodes, have read access to the node.

        Contributors are categorized as either "bibliographic" or "non-bibliographic". From a permissions standpoint, both are the same, but bibliographic contributors are included in citations and are listed on the project overview page on the OSF, while non-bibliographic contributors are not.

        Note that if an anonymous view_only key is being used to view the list of contributors, the user relationship will not be exposed and the contributor ID will be an empty string.

        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 contributors. Each resource in the array contains the full representation of the contributor, meaning additional requests to a contributor's detail view are not necessary. Additionally, the full representation of the user this contributor represents is automatically embedded within the `data` key of the response.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        #### Filtering
        You can optionally request that the response only include contributors that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/nodes/y9jdt/contributors/?filter[bibliographic]=true.

        Contributors may be filtered by their `bibliographic` and `permission` attributes.
      operationId: nodes_contributors_list
      x-api-path-slug: nodesnode-idcontributors-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Contributors
    post:
      summary: Create a contributor
      description: |-
        Adds a contributor to a node, effectively creating a relationship between the node and a user.

        Contributors are users who can make changes to the node or, in the case of private nodes, have read access to the node.

        Contributors are categorized as either "bibliographic" or "non-bibliographic" contributors. From a permissions standpoint, both are the same, but bibliographic contributors are included in citations and are listed on the project overview page on the OSF, while non-bibliographic contributors are not.
        #### Permissions
        Only project administrators can add contributors to a node.
        #### Required
        A relationship object with a `data` key, containing the `users` type and valid user ID is required.

        All attributes describing the relationship between the node and the user are optional.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the new contributor, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_contributors_create
      x-api-path-slug: nodesnode-idcontributors-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Contributors
  /nodes/{node_id}/contributors/{user_id}/:
    delete:
      summary: Delete a contributor
      description: |-
        Removes a contributor from a node. This request only removes the relationship between the node and the user, it does not delete the user itself.

        A node must always have at least one admin, and attempting to remove the only admin from a node will result in a **400 Bad Request** response.
        #### Permissions
        A user can remove themselves as a node contributor. Otherwise, only project administrators can remove contributors.
        #### Returns
        If the request is successful, no content is returned.

        If the request is unsuccessful, a JSON object with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_contributors_delete
      x-api-path-slug: nodesnode-idcontributorsuser-id-delete
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Contributors
      - User
    get:
      summary: Retrieve a contributor
      description: |-
        Retrieves the details of a given contributor.

        Contributors are users who can make changes to the node or, in the case of private nodes, have read access to the node.

        Contributors are categorized as either "bibliographic" or "non-bibliographic". From a permissions standpoint, both are the same, but bibliographic contributors are included in citations and are listed on the project overview page on the OSF, while non-bibliographic contributors are not.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the requested contributor, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_contributors_read
      x-api-path-slug: nodesnode-idcontributorsuser-id-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Contributors
      - User
    patch:
      summary: Update a contributor
      description: |-
        Updates a contributor by setting the values of the attributes specified in the request body. Any unspecified attributes will be left unchanged.

        Contributors can be updated with either a **PUT** or **PATCH** request. Since this endpoint has no mandatory attributes, PUT and PATCH are functionally the same.
        #### Permissions
        Only project administrators can update the contributors on a node.
        #### Returns
        Returns a JSON object with a `data` key containing the new representation of the updated contributor, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.

        If the given user is not already in the contributor list, a 404 Not Found error will be returned. A node must always have at least one admin, and any attempt to downgrade the permissions of a sole admin will result in a 400 Bad Request error.
      operationId: nodes_contributors_partial_update
      x-api-path-slug: nodesnode-idcontributorsuser-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: node_id
        description: The unique identifier of the node
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Contributors
      - User
  /nodes/{node_id}/draft_registrations/:
    get:
      summary: List all draft registrations
      description: |-
        A paginated list of all of the draft registrations of a given node.

        Draft registrations contain the supplemental registration questions that accompany a registration. A registration is a frozen version of the project that can never be edited or deleted, but can be withdrawn.

        Your original project remains editable but will now have the draft registration linked to it.
        #### Permissions
        Only project administrators may view draft registrations.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 draft registrations. Each resource in the array is a separate draft registration object and contains the full representation of the draft registration, meaning additional requests to a draft registration's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
      operationId: nodes_draft_registrations_list
      x-api-path-slug: nodesnode-iddraft-registrations-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Draft
      - Registrations
    post:
      summary: Create a draft registration
      description: |-
        Initiate a draft registration of the current node.
        Draft registrations contain the supplemental registration questions that accompany a registration. A registration is a frozen version of the project that can never be edited or deleted, but can be withdrawn.

        Your original project remains editable but will now have the draft registration linked to it.
        #### Permissions
        Only project administrators may view create registrations.
        #### Required
        Required fields for creating a draft registration include:

        &nbsp;&nbsp;&nbsp;&nbsp`registration_supplement`
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the created draft registration, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_draft_registrations_create
      x-api-path-slug: nodesnode-iddraft-registrations-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Draft
      - Registrations
  /nodes/{node_id}/draft_registrations/{draft_id}/:
    delete:
      summary: Delete a draft registration
      description: |-
        Permanently deletes a draft registration. A draft that has already been registered cannot be deleted.
        #### Permissions
        Only project administrators may delete draft registrations.
        #### Returns
        If the request is successful, no content is returned.

        If the request is unsuccessful, a JSON object with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes]() to understand why this request may have failed.
      operationId: nodes_draft_registrations_delete
      x-api-path-slug: nodesnode-iddraft-registrationsdraft-id-delete
      parameters:
      - in: path
        name: draft_id
        description: The unique identifier of the draft registration
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Draft
      - Registrations
      - Draft
    get:
      summary: Retrieve a draft registration
      description: |-
        Retrieve the details of a given draft registration.
        Draft registrations contain the supplemental registration questions that accompany a registration. A registration is a frozen version of the project that can never be edited or deleted, but can be withdrawn.

        Your original project remains editable but will now have the draft registration linked to it.
        #### Permissions
        Only project administrators may view draft registrations.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the requested draft registration, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_draft_registrations_read
      x-api-path-slug: nodesnode-iddraft-registrationsdraft-id-get
      parameters:
      - in: path
        name: draft_id
        description: The unique identifier of the draft registration
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Draft
      - Registrations
      - Draft
    patch:
      summary: Update a draft registration
      description: |-
        Updates a draft registration by setting the values of the attributes specified in the request body. Any unspecified attributes will be left unchanged.

        Draft registrations contain the supplemental registration questions that accompany a registration. Answer the questions in the draft registration supplement by sending update requests until you are ready to submit the draft.

        The registration supplement of a draft registration cannot be updated after the draft has been created.

        When updating a draft registration, `registration_metadata` is required. It must be a dictionary with keys as question ids in the registration form, and values as nested dictionaries matching the specific format in the [registration schema](TODO: link me pls).

        If a question is multiple-choice, the question response must exactly match one of the possible choices.
        #### Permissions
        Only project administrators may update draft registrations.
        #### Returns
        Returns a JSON object with a `data` key containing the new representation of the updated draft registration, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_draft_registrations_partial_update
      x-api-path-slug: nodesnode-iddraft-registrationsdraft-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: draft_id
        description: The unique identifier of the draft registration
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Draft
      - Registrations
      - Draft
  /nodes/{node_id}/files/:
    get:
      summary: List all storage providers
      description: |-
        List of all storage providers that are configured for this node

        Users of the OSF may access their data on a [number of cloud-storage services](https://api.osf.io/v2/#storage-providers) that have integrations with the OSF. We call these **providers**. By default, every node has access to the OSF-provided storage but may use as many of the supported providers as desired.


        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of files. Each resource in the array is a separate file object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        Note: In the OSF filesystem model, providers are treated as folders, but with special properties that distinguish them from regular folders. Every provider folder is considered a root folder, and may not be deleted through the regular file API.
      operationId: nodes_providers_list
      x-api-path-slug: nodesnode-idfiles-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Files
  /nodes/{node_id}/files/providers/{provider}/:
    get:
      summary: Retrieve a storage provider
      description: |-
        Retrieves the details of a storage provider enabled on this node.
        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested file object, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_providers_read
      x-api-path-slug: nodesnode-idfilesprovidersprovider-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      - in: path
        name: provider
        description: The unique identifier of the storage provider
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Files
      - Providers
      - Provider
  /nodes/{node_id}/files/{provider}/:
    get:
      summary: List all node files
      description: |-
        List of all the files/folders that are attached to your project for a given storage provider.
        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of files. Each resource in the array is a separate file object and contains the full representation of the file.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        ####Filtering

        You can optionally request that the response only include files that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/nodes/ezcuj/files/osfstorage/?filter[kind]=file

        Node files may be filtered by `id`, `name`, `node`, `kind`, `path`, `provider`, `size`, and `last_touched`.

        ###Waterbutler API actions

        Files can be modified through the Waterbutler API routes found in `links` (`new_folder`, `move`, `upload`, `download`, and `delete`).

        #### Download (files)

        To download a file, issue a GET request against the download link. The response will have the Content-Disposition header set, which will will trigger a download in a browser.

        #### Create Subfolder (folders)

        You can create a subfolder of an existing folder by issuing a PUT request against the new_folder link. The ?kind=folder portion of the query parameter is already included in the new_folder link. The name of the new subfolder should be provided in the name query parameter. The response will contain a WaterButler folder entity. If a folder with that name already exists in the parent directory, the server will return a 409 Conflict error response.

        #### Upload New File (folders)

        To upload a file to a folder, issue a PUT request to the folder's upload link with the raw file data in the request body, and the kind and name query parameters set to 'file' and the desired name of the file. The response will contain a WaterButler file entity that describes the new file. If a file with the same name already exists in the folder, the server will return a 409 Conflict error response.

        #### Update Existing File (file)

        To update an existing file, issue a PUT request to the file's upload link with the raw file data in the request body and the kind query parameter set to "file". The update action will create a new version of the file. The response will contain a WaterButler file entity that describes the updated file.

        #### Rename (files, folders)

        To rename a file or folder, issue a POST request to the move link with the action body parameter set to "rename" and the rename body parameter set to the desired name. The response will contain either a folder entity or file entity with the new name.

        #### Move & Copy (files, folders)

        Move and copy actions both use the same request structure, a POST to the move url, but with different values for the action body parameters. The path parameter is also required and should be the OSF path attribute of the folder being written to. The rename and conflict parameters are optional. If you wish to change the name of the file or folder at its destination, set the rename parameter to the new name. The conflict param governs how name clashes are resolved. Possible values are replace and keep. replace is the default and will overwrite the file that already exists in the target folder. keep will attempt to keep both by adding a suffix to the new file's name until it no longer conflicts. The suffix will be ' (x)' where x is a increasing integer starting from 1. This behavior is intended to mimic that of the OS X Finder. The response will contain either a folder entity or file entity with the new name.
        Files and folders can also be moved between nodes and providers. The resource parameter is the id of the node under which the file/folder should be moved. It must agree with the path parameter, that is the path must identify a valid folder under the node identified by resource. Likewise, the provider parameter may be used to move the file/folder to another storage provider, but both the resource and path parameters must belong to a node and folder already extant on that provider. Both resource and provider default to the current node and providers.
        If a moved/copied file is overwriting an existing file, a 200 OK response will be returned. Otherwise, a 201 Created will be returned.

        #### Delete (file, folders)

        To delete a file or folder send a DELETE request to the delete link. Nothing will be returned in the response body.
      operationId: nodes_files_list
      x-api-path-slug: nodesnode-idfilesprovider-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      - in: path
        name: provider
        description: The unique identifier of the storage provider
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Files
      - Provider
  /nodes/{node_id}/files/{provider}/{path}/:
    get:
      summary: Retrieve a file
      description: |-
        Retrieves the details of a file attached to given node (project or component) for the given storage provider.
        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested file object, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_files_read
      x-api-path-slug: nodesnode-idfilesproviderpath-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      - in: path
        name: path
        description: The unique identifier of the file path
      - in: path
        name: provider
        description: The unique identifier of the storage provider
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Files
      - Provider
      - Path
  /nodes/{node_id}/forks/:
    get:
      summary: List all forks of this node
      description: |-
        A paginated list of the current node's forks. The returned fork nodes are sorted by their `forked_date`, with the most recently forked nodes appearing first.

        Forking a project creates a copy of an existing node and all of its contents. The fork always points back to the original node, forming a network of nodes.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 forked nodes. If the current node has zero forked nodes, the `data` key will contain an empty array. Each resource in the array is a separate node object and contains the full representation of the forked node, meaning additional requests to the forked node's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        This request should never return an error.
      operationId: nodes_forks_list
      x-api-path-slug: nodesnode-idforks-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Forks
    post:
      summary: Create a fork of this node
      description: |-
        Creates a fork of the given node.

        Forking a project creates a copy of an existing node and all of its contents. The fork always points back to the original node, forming a network of nodes.

        You might use a fork to copy another's work to build on and extend. For example, a professor may create an OSF project of materials for individual student use. Each student forks the project to have his or her own copy of the materials to start his/her own work.

        When creating a fork, your fork will only contain public components of the current node and components for which you are a contributor. Private components that you do not have access to will not be forked.
        #### Required
        There are no required attributes when creating a fork, as all of the forked node's attributes will be copied from the current node.

        The `title` field is optional, with the default title being "Fork of " prepended to the current node's title.
        #### Returns
        Returns a JSON object with a `data` key containing the complete srepresentation of the forked node, if the request is successful.
        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: nodes_forks_create
      x-api-path-slug: nodesnode-idforks-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Forks
  /nodes/{node_id}/identifiers/:
    get:
      summary: List all identifiers
      description: |-
        List all identifiers associated with a given node.
        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of identifiers. Each resource in the array is a separate identifier object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        ####Filtering

        You can optionally request that the response only include nodes that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/nodes/ezcuj/identifiers/?filter[category]=ark

        Identifiers may be filtered by their `category` e.g `ark` or `doi`.
      operationId: nodes_identifiers_list
      x-api-path-slug: nodesnode-ididentifiers-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Nodeentifiers
  /nodes/{node_id}/institutions/:
    get:
      summary: List all institutions
      description: |-
        List of all institutions affiliated with this node.
        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 affilited institutions. Each resource in the array is a separate institution object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
      operationId: nodes_institutions_list
      x-api-path-slug: nodesnode-idinstitutions-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Institutions
  /nodes/{node_id}/linked_nodes/:
    get:
      summary: List all linked nodes
      description: |-
        List of all nodes linked to the given node.
        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 nodes. Each resource in the array is a separate node object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        ####Filtering
        You can optionally request that the response only include nodes that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/nodes/?filter[title]=reproducibility.

        Nodes may be filtered by their `title`, `category`, `description`, `public`, `registration`, or `tags`. `title`, `description`, and `category` are string fields and will be filteres using simple substring matching. `public`, `registration` are boolean and can be filtered using truthy values, such as `true`, `false`, `0`, `1`. `tags` is an array of simple strings.
      operationId: nodes_linked_nodes_list
      x-api-path-slug: nodesnode-idlinked-nodes-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Linked
      - Nodes
  /nodes/{node_id}/logs/:
    get:
      summary: List all logs
      description: |-
        A paginated list of all logs associated with a given node.

        The returned logs are sorted by their `date`, with the most recents logs appearing first.

        This list includes the logs of the specified node as well as the logs of that node's children to which the current user has read-only access.

        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 logs. Each resource in the array is a separate logs object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        ####Filtering
        You can optionally request that the response only include logs that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/nodes/ezcuj/logs/?filter[action]=made_private.

        Nodes may be filtered by their `action`, and `date`.
      operationId: nodes_logs_list
      x-api-path-slug: nodesnode-idlogs-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Logs
  /nodes/{node_id}/preprints/:
    get:
      summary: List all preprints
      description: |-
        A paginated list of preprints related to a given node. The returned preprints are sorted by their creation date, with the most recent preprints appearing first.

        **Note: This API endpoint is under active development, and is subject to change in the future.**
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 preprints. Each resource in the array is a separate preprint object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
      operationId: nodes_preprints_list
      x-api-path-slug: nodesnode-idpreprints-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Preprints
  /nodes/{node_id}/registrations/:
    get:
      summary: List all registrations
      description: |-
        List of all registrations of the given node.
        ####Returns

        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 registrations. Each resource in the array is a separate registrations object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        ####Filtering

        You can optionally request that the response only include registrations that match your filters by utilizing the filter query parameter, e.g. https://api.osf.io/v2/registrations/?filter[title]=open.

        Registrations may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, and `contributors`.
      operationId: nodes_registrations_list
      x-api-path-slug: nodesnode-idregistrations-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Registrations
  /nodes/{node_id}/view_only_links/:
    get:
      summary: List all view only links
      description: |-
        List of view only links on a node.
        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 view only links. Each resource in the array is a view only link object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        ####Permissions

        View only links on a node, public or private, are readable and writeable only by users that are administrators on the node.

        ####Filtering

        You can optionally request that the response only include view only links that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/nodes/ezcuj/view_only_links/?filter[anonymous]=true.

        View Only Links may be filtered based on their `name`, `anonymous` and `date_created` fields. Possible comparison operators include 'gt' (greater than), 'gte'(greater than or equal to), 'lt' (less than) and 'lte' (less than or equal to). The date must be in the format YYYY-MM-DD and the time is optional.
      operationId: nodes_view_only_links_list
      x-api-path-slug: nodesnode-idview-only-links-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - View
      - Only
      - Links
  /nodes/{node_id}/view_only_links/{link_id}/:
    get:
      summary: Retrieve a view only link
      description: |-
        Retrieves the details of a view only link on a node.
        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested view only link, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
        ####Permissions

        View only links on a node, public or private, are readable and writeable only by users that are administrators on the node.
      operationId: nodes_view_only_links_read
      x-api-path-slug: nodesnode-idview-only-linkslink-id-get
      parameters:
      - in: path
        name: link_id
        description: The unique identifier of the view only link
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - View
      - Only
      - Links
      - Link
  /nodes/{node_id}/wikis/:
    get:
      summary: List all wikis
      description: |-
        List of wiki pages on a node.
        ####Returns
        Paginated list of the node's current wiki page versions ordered by their date_modified. Each resource contains the full representation of the wiki, meaning additional requests to an individual wiki's detail view are not necessary.

        Note that if an anonymous view_only key is being used, the user relationship will not be exposed.

        If the request is unsuccessful, a JSON object with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
        #### Filtering
        Wiki pages can be filtered based on their `name` and `date_modified` fields.
        + `filter[name]=<Str>` -- filter wiki pages by name
        + `filter[date_modified][comparison_operator]=YYYY-MM-DDTH:M:S` -- filter wiki pages based on date modified.

        Possible comparison operators include 'gt' (greater than), 'gte'(greater than or equal to), 'lt' (less than) and 'lte' (less than or equal to). The date must be in the format YYYY-MM-DD and the time is optional.
      operationId: nodes_wikis_list
      x-api-path-slug: nodesnode-idwikis-get
      parameters:
      - in: path
        name: node_id
        description: The unique identifier of the node
      responses:
        200:
          description: OK
      tags:
      - Nodes
      - Node
      - Wikis
  /preprint_providers/:
    get:
      summary: List all preprint providers
      description: |-
        A paginated list of all preprint providers. The returned preprint providers are sorted by their creation date, with the most recent preprints appearing first.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 preprint providers. Each resource in the array is a separate preprint provider object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        This request should never return an error.
        #### Filtering
        You can optionally request that the response only include preprint providers that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/preprint_providers/?filter[id]=osf.

        Preprint Providers may be filtered by their `id`, `name`,  and `description`
      operationId: preprint_provider_list
      x-api-path-slug: preprint-providers-get
      responses:
        200:
          description: OK
      tags:
      - Preprint
      - Providers
  /preprint_providers/{preprint_provider_id}/:
    get:
      summary: Retrieve a preprint provider
      description: |-
        Retrieves the details of a preprint provider.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the requested preprint provider, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.

        #### Acceptable Subjects Structure
        Each preprint provider specifies acceptable subjects.
        `subjects_acceptable` is an array found in `attributes`.
        Subjects consist of general parent subjects (e.g., Engineering), more specific child subjects (e.g., Aerospace Engineering), and even more specific grandchild subjects (e.g., Aerodynamics and Fluid Mechanics). Subjects can only be nested 3 deep.


            "subjects_acceptable": [
                [
                    [
                        # Parent Subject:
                        # Architecture
                        "584240d954be81056ceca9e5",

                        # Child Subject:
                        # Architectural Engineering
                        "584240da54be81056cecac87"
                    ],
                    # Include all Architectural Engineering's children:
                    true
                ],
                [
                    [
                        # Parent Subject:
                        # Engineering
                        "584240da54be81056cecaca9",

                        # Child Subject:
                        # Aerospace Engineering
                        "584240db54be81056cecacd6",

                        # Grandchild Subject:
                        # Aerodynamics and Fluid Mechanics
                        "584240da54be81056cecaa74"
                    ],
                    # All nestings 3 deep must be false
                    false
                ]
            ]

        The above structure would allow Architecture, Architectural Engineering, all of Architectural Engineering's children, Engineering, Aerospace Engineering, and Aerodynamics and Fluid Mechanics.
      operationId: preprint_provider_detail
      x-api-path-slug: preprint-providerspreprint-provider-id-get
      parameters:
      - in: path
        name: preprint_provider_id
        description: The unique identifier of the preprint provider
      responses:
        200:
          description: OK
      tags:
      - Preprint
      - Providers
      - Preprint
      - Provider
  /preprint_providers/{preprint_provider_id}/licenses/:
    get:
      summary: List all licenses
      description: |-
        A paginated list of the licenses allowed bya preprint provider.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 preprint providers. Each resource in the array is a separate preprint provider object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: preprint_provider_licenses_list
      x-api-path-slug: preprint-providerspreprint-provider-idlicenses-get
      parameters:
      - in: path
        name: preprint_provider_id
        description: The unique identifier of the preprint provider
      responses:
        200:
          description: OK
      tags:
      - Preprint
      - Providers
      - Preprint
      - Provider
      - Licenses
  /preprint_providers/{preprint_provider_id}/preprints/:
    get:
      summary: List all preprints
      description: |-
        A paginated list of preprints from the specified preprint provider. The returned preprints are sorted by their creation date, with the most recent preprints appearing first.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 preprints. Each resource in the array is a separate preprint object.

        The `links` key contains a dictionary with keys that can be used for [pagination](#Introduction_pagination).

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.

        #### Filtering
        You can optionally request that the response only include preprints that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/preprint_providers/osf/preprints/?filter[is_published]=true.

        Preprints may be filtered by their `id`, `is_published`, `date_created`, `date_modified`, and `provider`.
      operationId: preprint_providers_preprints_list
      x-api-path-slug: preprint-providerspreprint-provider-idpreprints-get
      parameters:
      - in: path
        name: preprint_provider_id
        description: The unique identifier of the preprint provider
      responses:
        200:
          description: OK
      tags:
      - Preprint
      - Providers
      - Preprint
      - Provider
      - Preprints
  /preprint_providers/{preprint_provider_id}/taxonomies/:
    get:
      summary: List all taxonomies
      description: |-
        A paginated list of the taxonomies for a preprint provider. The returned preprint providers taxonomies are sorted by their creation date, with the most recent preprints appearing first.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 preprint providers. Each resource in the array is a separate preprint provider object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: preprint_provider_taxonomies_list
      x-api-path-slug: preprint-providerspreprint-provider-idtaxonomies-get
      parameters:
      - in: path
        name: preprint_provider_id
        description: The unique identifier of the preprint provider
      responses:
        200:
          description: OK
      tags:
      - Preprint
      - Providers
      - Preprint
      - Provider
      - Taxonomies
  /preprints/:
    get:
      summary: List all preprints
      description: |-
        A paginated list of preprints from all preprint providers. The returned preprints are sorted by their creation date, with the most recent preprints appearing first.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 preprints. Each resource in the array is a separate preprint object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        This request should never return an error.
        #### Filtering
        You can optionally request that the response only include preprints that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/preprints/?filter[provider]=socarxiv.

        Preprints may be filtered by their `id`, `is_published`, `date_created`, `date_modified`, and `provider`.
      operationId: preprints_list
      x-api-path-slug: preprints-get
      responses:
        200:
          description: OK
      tags:
      - Preprints
    post:
      summary: Create a preprint
      description: |-
        Creates a new preprint.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the created preprint, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes]() to understand why this request may have failed.
      operationId: preprints_create
      x-api-path-slug: preprints-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Preprints
  /preprints/{preprint_id}/:
    get:
      summary: Retrieve a preprint
      description: |-
        Retrieves the details of a preprint.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the requested preprint, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: preprints_read
      x-api-path-slug: preprintspreprint-id-get
      parameters:
      - in: path
        name: preprint_id
        description: The unique identifier of the preprint
      responses:
        200:
          description: OK
      tags:
      - Preprints
      - Preprint
    patch:
      summary: Update a preprint
      description: |-
        Updates the specified preprint by setting the values of the parameters passed. Any parameters not provided will be left unchanged.
        #### Returns
        Returns a JSON object with a `data` key containing the new representation of the updated preprint, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes]() to understand why this request may have failed.
      operationId: preprints_partial_update
      x-api-path-slug: preprintspreprint-id-patch
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: preprint_id
        description: The unique identifier of the preprint
      responses:
        200:
          description: OK
      tags:
      - Preprints
      - Preprint
  /preprints/{preprint_id}/citation/:
    get:
      summary: Retrieve citation details
      description: |-
        The citation details for a preprint, in CSL format.
        #### Returns
        Returns a JSON object with a `data` key that contains the representation of the details necessary for the preprint citation.
      operationId: preprints_citation_list
      x-api-path-slug: preprintspreprint-idcitation-get
      parameters:
      - in: path
        name: preprint_id
        description: The unique identifier of the preprint whose citation you wish
          to retrieve
      responses:
        200:
          description: OK
      tags:
      - Preprints
      - Preprint
      - Citation
  /preprints/{preprint_id}/citation/{style_id}/:
    get:
      summary: Retrieve a styled citation
      description: |-
        The citation for a preprint in a specific style.
        #### Returns
        Returns a JSON object with a `data` key that contains the representation of the preprint citation, in the requested style.
      operationId: preprints_citation_read
      x-api-path-slug: preprintspreprint-idcitationstyle-id-get
      parameters:
      - in: path
        name: preprint_id
        description: The unique identifier of the preprint
      - in: path
        name: style_id
        description: The unique identifier of the citation style
      responses:
        200:
          description: OK
      tags:
      - Preprints
      - Preprint
      - Citation
      - Style
  /registrations/:
    get:
      summary: List all registrations
      description: |-
        A paginated list of registrations on the OSF to which the user has access.

        The returned registrations are those which are public or which the user has access to view.

        Non-registered nodes cannot be accessed through this endpoint (use the [nodes](#Nodes_nodes_list) endpoints instead).

        #### Registrations
        A registration on the OSF creates a frozen, time-stamped version of a project that cannot be edited or deleted. The *original project* can still be edited, while the registered version cannot.

        Registrations can be made public immediately or embargoed for up to 4 years.

        #### Withdrawals
        Registrations cannot be deleted, but they can be withdrawn. Withdrawing a registration removes the content of the registration but leaves behind basic metadata. A withdrawn registration will display a limited subset of information, namely, title, description, date_created, date_registered, date_withdrawn, registration, withdrawn, withdrawal_justification, and registration supplement. All other fields will be displayed as null. Additionally, the only relationship that remains accesible for a withdrawn registration is the contributors. All other relationships will return a **403 Forbidden** response.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 registrations. Each resource in the array is a separate registration object and contains the full representation of the registration, meaning additional requests to a registration's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        This request should never return an error.
        #### Filtering
        You can optionally request that the response only include registrations that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/?filter[title]=open.

        Registrations may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, and `contributors`.
      operationId: registrations_list
      x-api-path-slug: registrations-get
      responses:
        200:
          description: OK
      tags:
      - Registrations
  /registrations/{registration_id}/:
    get:
      summary: Retrieve a registration
      description: |-
        Retrieve the details of a given registration.
        #### Permissions
        Only project contributors may retrieve the details of a registration that is embargoed, or has not yet been made public. Attempting to retrieve a private registration for which you are not a contributor will result in a **403 Forbidden** response.

        Authentication is not required to view the details of a public registration, as public registrations give read-only access to everyone.
        #### Registrations
        A registration on the OSF creates a frozen, time-stamped version of a project that cannot be edited or deleted. The *original project* can still be edited, while the registered version cannot.

        Registrations can be made public immediately or embargoed for up to 4 years.

        #### Withdrawals
        Registrations cannot be deleted, but they can be withdrawn. Withdrawing a registration removes the content of the registration but leaves behind basic metadata. A withdrawn registration will display a limited subset of information, namely, title, description, date_created, date_registered, date_withdrawn, registration, withdrawn, withdrawal_justification, and registration supplement. All other fields will be displayed as null. Additionally, the only relationship that remains accesible for a withdrawn registration is the contributors. All other relationships will return a **403 Forbidden** response.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the requested registration, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: registrations_read
      x-api-path-slug: registrationsregistration-id-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
    patch:
      summary: Update a registration
      description: |-
        Updates a registration's privacy from **private** to **public**.

        Registrations can be updated with either a **PUT** or **PATCH** request. The `public` field is the only field that can be modified on a registration

        Registrations can only be turned from private to public, not vice versa.
        #### Permissions
        Only project administrators may update a registration.
        #### Returns
        Returns a JSON object with a `data` key containing the new representation of the updated registration, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: registrations_partial_update
      x-api-path-slug: registrationsregistration-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
  /registrations/{registration_id}/children/:
    get:
      summary: List all child registrations
      description: |-
        A paginated list of children of a registration.

        The list consists of the next level child registrations for the given registration. The returned registrations are sorted by their `date_modified`, with the most recently updated child registrations appearing first.

        The list will include child registrations that are public, as well as child registrations that are private, if the authenticated user has permission to view them.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 child registrations. If the given registration has zero child registrations, the `data` key will contain an empty array. Each resource in the array is a separate registration object and contains the full representation of the child registration.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        #### Filtering
        You can optionally request that the response only include registrations that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/children/?filter[title]=reproducibility.

        Registrations may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, and `contributors`.

        Most fields are string fields and will be filtered using simple substring matching. Public is a boolean field, and can be filtered using truthy values, such as **true**, **false**, **0** or **1**. Note that quoting true or false in the query will cause the match to fail.
      operationId: registrations_children_list
      x-api-path-slug: registrationsregistration-idchildren-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Children
  /registrations/{registration_id}/citations/:
    get:
      summary: List all citation styles
      description: |-
        A paginated list of the registration's alternative citation styles

        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 citation styles. Each resource in the array is a separate citation styles object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        #### Filtering
        You can optionally request that the response only include citation styles that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/citations/?filter[title]=open.

        Citation styles may be filtered by their `id`, `title`, `short-title`, and `summary`.
      operationId: registrations_citations_list
      x-api-path-slug: registrationsregistration-idcitations-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Citations
  /registrations/{registration_id}/citations/{citation_id}/:
    get:
      summary: Retrieve a citation
      description: |-
        Retrieves the citation style details for a registration, in CSL format.
        #### Returns
        Returns a JSON object with a `data` key that contains the representation of the details necessary for the citation style.
      operationId: registrations_citation_read
      x-api-path-slug: registrationsregistration-idcitationscitation-id-get
      parameters:
      - in: path
        name: citation_id
        description: The unique identifier of the citation
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Citations
      - Citation
  /registrations/{registration_id}/comments/:
    get:
      summary: List all comments
      description: |-
        A paginated list of the registration's comments.

        The returned comments are sorted by their creation date, with the most recent comments appearing first.
        ####Permissions
        Comments of public registrations are given read-only access to everyone.

        If the comment-level is `private`, only registration contributors have permission to comment.

        If the comment-level is `public`, any logged-in OSF user can comment.

        Comments of private registrations are only visible to contributors and administrators on the registration.
        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of comment objects. Each resource in the array is a separate comment object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        #### Filtering
        You can optionally request that the response only include comments that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wuerf/comments/?filter[target]=wuerf

        Comments may be filtered by their `deleted`, `target`, `date_created`, `date_modified`.

        Most fields are string fields and will be filtered using simple substring matching. Deleted is a boolean field, and can be filtered using truthy values, such as **true**, **false**, **0** or **1**. Note that quoting `true` or `false` in the query will cause the match to fail.
      operationId: registrations_comments_list
      x-api-path-slug: registrationsregistration-idcomments-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Comments
  /registrations/{registration_id}/contributors/:
    get:
      summary: List all contributors
      description: |-
        A paginated list of all contributors on this registration.
        The returned contributors are sorted by their index.

        Contributors are users who can make changes to the registration or, in the case of private registration, have read access to the registration.

        Contributors are categorized as either "bibliographic" or "non-bibliographic". From a permissions standpoint, both are the same, but bibliographic contributors are included in citations and are listed in the contributors list on the OSF, while non-bibliographic contributors are not.

        Note that if an anonymous view_only key is being used to view the list of contributors, the user relationship will not be exposed and the contributor ID will be an empty string.

        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 contributors. Each resource in the array contains the full representation of the contributor. Additionally, the full representation of the user this contributor represents is automatically embedded within the `data` key of the response.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        #### Filtering
        You can optionally request that the response only include contributors that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wu3a4/contributors/?filter[bibliographic]=true.

        Contributors may be filtered by their `bibliographic` and `permission` attributes.
      operationId: registrations_contributors_list
      x-api-path-slug: registrationsregistration-idcontributors-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Contributors
  /registrations/{registration_id}/contributors/{user_id}/:
    get:
      summary: Retrieve a contributor
      description: |-
        Retrieves the details of a contributor on this registration.

        #### Returns
        Returns a JSON object with a `data` key containing the representation of the requested contributor, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: registrations_contributors_read
      x-api-path-slug: registrationsregistration-idcontributorsuser-id-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Contributors
      - User
  /registrations/{registration_id}/files/:
    get:
      summary: List all storage providers
      description: |-
        A paginated list of storage providers enabled on the registration

        Users of the OSF may access their data on a [number of cloud-storage services](https://api.osf.io/v2/#storage-providers) that have integrations with the OSF. We call these **providers**. By default, every node has access to the OSF-provided storage but may use as many of the supported providers as desired.


        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 files. Each resource in the array is a separate file object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        Note: In the OSF filesystem model, providers are treated as folders, but with special properties that distinguish them from regular folders. Every provider folder is considered a root folder, and may not be deleted through the regular file API.
      operationId: registrations_providers_list
      x-api-path-slug: registrationsregistration-idfiles-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Files
  /registrations/{registration_id}/files/{provider}/:
    get:
      summary: List all files
      description: |-
        List of all the registration's files/folders for a given storage provider.

        ####Returns

        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of files. Each resource in the array is a separate file object and contains the full representation of the file.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        ####Filtering

        You can optionally request that the response only include files that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/files/osfstorage/?filter[kind]=file

        Files may be filtered by `id`, `name`, `node`, `kind`, `path`, `provider`, `size`, and `last_touched`.
      operationId: registrations_files_list
      x-api-path-slug: registrationsregistration-idfilesprovider-get
      parameters:
      - in: path
        name: provider
        description: The unique identifier of the storage provider
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Files
      - Provider
  /registrations/{registration_id}/files/{provider}/{path}/:
    get:
      summary: Retrieve a file
      description: |-
        Retrieves the details of a registration file for the given storage provider.
        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested registration file object, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: registrations_files_read
      x-api-path-slug: registrationsregistration-idfilesproviderpath-get
      parameters:
      - in: path
        name: path
        description: The unique identifier of the file path
      - in: path
        name: provider
        description: The unique identifier of the storage provider
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Files
      - Provider
      - Path
  /registrations/{registration_id}/forks/:
    get:
      summary: List all forks
      description: |-
        A paginated list of the registration???s forks

        The returned forks are sorted by their `forked_date`, with the most recent forks appearing first.

        Forking a registration creates a copy of an existing registration and all of its contents.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 forks. If the current registration has no fork, the `data` key will contain an empty array. Each resource in the array is a separate registration object and contains the full representation of the registration's fork.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
      operationId: registrations_forks_list
      x-api-path-slug: registrationsregistration-idforks-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Forks
    post:
      summary: Create a fork
      description: |-
        Creates a fork of the given registration.

        Forking a project creates a copy of an existing registration and all of its contents. The fork always points back to the original registration, forming a network of registrations.

        You might use a fork to copy another's work to build on and extend. For example, a professor may create an OSF project of materials for individual student use. Each student forks the project to have his or her own copy of the materials to start his/her own work.

        When creating a fork, your fork will only contain public components of the current registration and components for which you are a contributor. Private components that you do not have access to will not be forked.
        #### Required
        There are no required attributes when creating a fork, as all of the forked registration's attributes will be copied from the current registration.

        The `title` field is optional, with the default title being "Fork of " prepended to the current registration's title.
        #### Returns
        Returns a JSON object with a `data` key containing the complete representation of the forked registration, if the request is successful.
        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: registrations_forks_create
      x-api-path-slug: registrationsregistration-idforks-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Forks
  /registrations/{registration_id}/identifiers/:
    get:
      summary: List all identifiers
      description: |-
        A paginated list of the registration's identifiers.
        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of identifiers. Each resource in the array is a separate identifier object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        ####Filtering

        You can optionally request that the response only include registrations that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/identifiers/?filter[category]=ark

        Identifiers may be filtered by their `category` e.g `ark` or `doi`.
      operationId: registrations_identifiers_list
      x-api-path-slug: registrationsregistration-ididentifiers-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registrationentifiers
  /registrations/{registration_id}/institutions/:
    get:
      summary: List all institutions
      description: |-
        A paginated list of institutions affiliated with the registration.
        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 affiliated institutions. Each resource in the array is a separate institution object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
      operationId: registrations_institutions_list
      x-api-path-slug: registrationsregistration-idinstitutions-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Institutions
  /registrations/{registration_id}/linked_nodes/:
    get:
      summary: List all linked nodes
      description: |-
        List of all nodes linked to the registration.
        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 nodes. Each resource in the array is a separate node object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        ####Filtering
        You can optionally request that the response only include nodes that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/linked_nodes/?filter[title]=reproducibility/?filter[title]=reproducibility.

        Nodes may be filtered by their `title`, `category`, `description`, `public`, `registration`, or `tags`. `title`, `description`, and `category` are string fields and will be filteres using simple substring matching. `public`, `registration` are boolean and can be filtered using truthy values, such as `true`, `false`, `0`, `1`. `tags` is an array of simple strings.
      operationId: registrations_linked_nodes_list
      x-api-path-slug: registrationsregistration-idlinked-nodes-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Linked
      - Nodes
  /registrations/{registration_id}/logs/:
    get:
      summary: List all logs
      description: |-
        A paginated list of the registration's logs.

        The returned logs are sorted by their `date`, with the most recents logs appearing first.

        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 logs. Each resource in the array is a separate logs object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        ####Filtering
        You can optionally request that the response only include logs that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wucr8/logs/?filter[action]=made_private.

        Logs may be filtered by their `action`, and `date`.
      operationId: registrations_logs_list
      x-api-path-slug: registrationsregistration-idlogs-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Logs
  /registrations/{registration_id}/view_only_links/:
    get:
      summary: List all view only links
      description: |-
        A paginated list of view only links created for this registration.
        ####Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 view only links. Each resource in the array is a view only link object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        ####Permissions

        View only links on a registration, public or private, are readable and writeable only by users that are administrators on the registration.

        ####Filtering

        You can optionally request that the response only include view only links that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/registrations/wu3a4/view_only_links/?filter[anonymous]=true.

        View Only Links may be filtered based on their `name`, `anonymous` and `date_created` fields. Possible comparison operators include 'gt' (greater than), 'gte'(greater than or equal to), 'lt' (less than) and 'lte' (less than or equal to). The date must be in the format YYYY-MM-DD and the time is optional.
      operationId: registrations_view_only_links_list
      x-api-path-slug: registrationsregistration-idview-only-links-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - View
      - Only
      - Links
  /registrations/{registration_id}/view_only_links/{link_id}/:
    get:
      summary: Retrieve a view only link
      description: |-
        Retrieves the details of a view only link created from this registration.
        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested view only link, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
        ####Permissions

        View only links on a registration, public or private, are readable and writeable only by users that are administrators on the registration.
      operationId: registrations_view_only_links_read
      x-api-path-slug: registrationsregistration-idview-only-linkslink-id-get
      parameters:
      - in: path
        name: link_id
        description: The unique identifier of the view only link
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - View
      - Only
      - Links
      - Link
  /registrations/{registration_id}/wikis/:
    get:
      summary: List all wikis
      description: |-
        A paginated list of the registration's wiki pages
        ####Returns
        A list of all registration's current wiki page versions ordered by their date_modified. Each resource contains the full representation of the wiki, meaning additional requests to an individual wiki's detail view are not necessary.

        If the request is unsuccessful, a JSON object with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
        #### Filtering
        Wiki pages can be filtered based on their `name` and `date_modified` fields.
        + `filter[name]=<Str>` -- filter wiki pages by name
        + `filter[date_modified][comparison_operator]=YYYY-MM-DDTH:M:S` -- filter wiki pages based on date modified.

        Possible comparison operators include 'gt' (greater than), 'gte'(greater than or equal to), 'lt' (less than) and 'lte' (less than or equal to). The date must be in the format YYYY-MM-DD and the time is optional.
      operationId: registrations_wikis_list
      x-api-path-slug: registrationsregistration-idwikis-get
      parameters:
      - in: path
        name: registration_id
        description: The unique identifier of the registration
      responses:
        200:
          description: OK
      tags:
      - Registrations
      - Registration
      - Wikis
  /taxonomies/:
    get:
      summary: List all taxonomies
      description: |-
        A paginated list of all [bepress disciplines taxonomies](https://www.bepress.com/wp-content/uploads/2016/12/Digital-Commons-Disciplines-taxonomy-2017-01.pdf).
        Note: this API endpoint is under active development, and is subject to change in the future.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 taxonomies. Each resource in the array is a separate taxonomy object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        This request should never return an error.
        #### Filtering
        You can optionally request that the response only include taxonomies that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/taxonomies/?filter['id']='{taxonomy_id}'.

        Taxonomies may be filtered by their `id`, `parents`, and `text`.
      operationId: taxonomies_list
      x-api-path-slug: taxonomies-get
      responses:
        200:
          description: OK
      tags:
      - Taxonomies
  /taxonomies/{taxonomy_id}/:
    get:
      summary: Retrieve a taxonomy
      description: |-
        Retrieves the details of a taxonomy.
        #### Returns

        Returns a JSON object with a `data` key containing the representation of the requested taxonomy, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: taxonomies_read
      x-api-path-slug: taxonomiestaxonomy-id-get
      parameters:
      - in: path
        name: taxonomy_id
        description: The unique identifier of the taxonomy
      responses:
        200:
          description: OK
      tags:
      - Taxonomies
      - Taxonomy
  /users/:
    get:
      summary: List all users
      description: |-
        A paginated list of all users registered on the OSF. The returned users are sorted by their `date_registered`, with the most recently registered users appearing first.

        The subroute `/users/me/` is a special endpoint that always points to the currently logged-in user.
        #### Versioning
        As of version `2.3`, merged users will not be returned from this endpoint.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 users. Each resource in the array is a separate users object and contains the full representation of the user, meaning additional requests to a user's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        This request should never return an error.
        #### Filtering
        You can optionally request that the response only include nodes that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/users/?filter[family_name]=Nosek.

        Users may be filtered by their `id`, `full_name`, `given_name`, `middle_name`, or `family_name`.
      operationId: users_list
      x-api-path-slug: users-get
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{user_id}/:
    get:
      summary: Retrieve a user
      description: |-
        Retrieves the details of a given users.

        The returned information includes the user's bibliographic information and the date the user was registered.

        Additionally, relationships to the list of institutions with which the user is affiliated, and to the list of nodes which the user contributes to (that the requesting user has permission to see) are returned.

        If `me` is given as the `user_id` in the request path, the record of the currently logged-in user will be returned.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the requested user, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: users_read
      x-api-path-slug: usersuser-id-get
      parameters:
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
    patch:
      summary: Update a user
      description: |-
        Updates a user by setting the values of the attributes specified in the request body. Any unspecified attributes will be left unchanged.

        Users can be updated with either a **PUT** or **PATCH** request. The `full_name` field is mandatory in a **PUT** request, and optional in a **PATCH**.

        **Note**: if you make a PUT/PATCH request to the `/users/me/` endpoint, you must still provide your full user ID in the ID field of the request. We do not support using the `me` alias in request bodies at this time.
        #### Returns
        Returns a JSON object with a `data` key containing the new representation of the updated node, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: users_partial_update
      x-api-path-slug: usersuser-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
  /users/{user_id}/addons/:
    get:
      summary: List all user addons
      description: |-
        A paginated list of authorized user addons

        #### Permissions

        User addons are visible only to the user that authorized the addon.

        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 addons. Each resource in the array is a separate addon object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.

        Attempting to request the accounts for an addon that is not enabled will result in a **404 Not Found** response.
      operationId: users_addons_list
      x-api-path-slug: usersuser-idaddons-get
      parameters:
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Addons
  /users/{user_id}/addons/{provider}/:
    get:
      summary: Retrieve a user addon
      description: |-
        Retrieves the details of an authorized user addon

        #### Permissions

        User addons are visible only to the user that authorized the addon.

        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested user addon, if the request was successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.

        Attempting to request the accounts for an addon that is not enabled will result in a **404 Not Found** response.
      operationId: users_addons_read
      x-api-path-slug: usersuser-idaddonsprovider-get
      parameters:
      - in: path
        name: provider
        description: The unique identifier of the addon provider
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Addons
      - Provider
  /users/{user_id}/addons/{provider}/accounts/:
    get:
      summary: List all addon accounts
      description: |-
        A paginated list of addon accounts authorized by this user.

        #### Permissions

        Addon accounts are visible only to the user that authorized the account.

        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of at most 10 addon account objects. Each resource in the array is a separate  addon account object and contains the full representation of the addon account.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
      operationId: Users_addon_accounts_list
      x-api-path-slug: usersuser-idaddonsprovideraccounts-get
      parameters:
      - in: path
        name: provider
        description: The unique identifier of the addon provider
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Addons
      - Provider
      - Accounts
  /users/{user_id}/addons/{provider}/accounts/{account_id}/:
    get:
      summary: Retrieve an addon account
      description: |-
        Retrieves the details of an addon account

        #### Permissions

        Addon accounts are visible only to the user that authorized the account.

        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested addon account, if the request was successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: Users_addon_accounts_read
      x-api-path-slug: usersuser-idaddonsprovideraccountsaccount-id-get
      parameters:
      - in: path
        name: account_id
        description: The unique identifier of the addon account
      - in: path
        name: provider
        description: The unique identifier of the addon provider
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Addons
      - Provider
      - Accounts
      - Account
  /users/{user_id}/institutions/:
    get:
      summary: List all institutions
      description: |-
        A paginated list of institutions that the user is affiliated with.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 institutions. Each resource in the array is a complete institution object and contains the full representation of the institution, meaning additional requests to a institution's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
      operationId: users_institutions_list
      x-api-path-slug: usersuser-idinstitutions-get
      parameters:
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Institutions
  /users/{user_id}/nodes/:
    get:
      summary: List all nodes
      description: |-
        A paginated list of nodes that the user is a contributor to. The returned nodes are sorted by their `date_modified`, with the most recently updated nodes appearing first.

        If the user ID in the path is the same as the logged-in user, all nodes will be returned. Otherwise, only the user's public nodes will be returned.

        User registrations are not available at this endpoint.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 nodes. Each resource in the array is a separate node object and contains the full representation of the node, meaning additional requests to a node's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        #### Filtering
        You can optionally request that the response only include nodes that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/users/cdi38/nodes/?filter[title]=open.

        Nodes may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, `preprint`, and `contributors`.
      operationId: users_nodes_list
      x-api-path-slug: usersuser-idnodes-get
      parameters:
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Nodes
  /users/{user_id}/preprints/:
    get:
      summary: List all preprints
      description: |-
        A paginated list of preprints that the user contributes to. The returned preprints are sorted by their creation date, with the most recent preprints appearing first.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 preprints. Each resource in the array is a complete preprint object and contains the full representation of the preprint, meaning additional requests to a preprint's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        #### Filtering
        You can optionally request that the response only include preprints that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/users/cdi38/preprints/?filter[provider]=psyarxiv.

        Preprints may be filtered by their `id`, `is_published`, `date_created`, `date_modified`, and `provider`.
      operationId: users_preprints_list
      x-api-path-slug: usersuser-idpreprints-get
      parameters:
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Preprints
  /users/{user_id}/registrations/:
    get:
      summary: List all registrations
      description: |-
        A paginated list of registrations that the user is a contributor to. The returned registrations are sorted by their `date_modified`, with the most recently updated registrations appearing first.

        If the user ID in the path is the same as the logged-in user, all registrations will be returned. Otherwise, only the user's public registrations will be returned.

        User nodes are not available at this endpoint.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 registrations. Each resource in the array is a separate registration object and contains the full representation of the registration, meaning additional requests to a registration's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).
        #### Filtering
        You can optionally request that the response only include registrations that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/users/cdi38/registrations/?filter[title]=replication.

        Registrations may be filtered by their `id`, `title`, `category`, `description`, `public`, `tags`, `date_created`, `date_modified`, `root`, `parent`, and `contributors`.
      operationId: users_registrations_list
      x-api-path-slug: usersuser-idregistrations-get
      parameters:
      - in: path
        name: user_id
        description: The unique identifier of the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Registrations
  /view_only_links/{link_id}/:
    get:
      summary: Retrieve a view only link
      description: |-
        Retrieves details about a specific view only link.
        ####Permissions
        Only project administrators may retrieve the details of a view only link. Attempting to retrieve a view only link without appropriate permissions will result in a 403 Forbidden response.
        #### Returns
        Returns a JSON object with a `data` key containing the representation of the requested view only link, if the request is successful.
        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: view_only_links_read
      x-api-path-slug: view-only-linkslink-id-get
      parameters:
      - in: path
        name: link_id
        description: The unique identifier of the view only link
      responses:
        200:
          description: OK
      tags:
      - View
      - Only
      - Links
      - Link
  /view_only_links/{link_id}/nodes/:
    get:
      summary: List all nodes
      description: |-
        The list of nodes which this view only link gives read-only access to.
        #### Permissions
        Only project administrators may retrieve the nodes of a view only link. Attempting to retrieve a view only link without appropriate permissions will result in a 403 Forbidden response.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.
        The `data` key contains an array of up to 10 nodes. Each resource in the array is a separate node object and contains the full representation of the node, meaning additional requests to a node's detail view are not necessary.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: view_only_links_node_list
      x-api-path-slug: view-only-linkslink-idnodes-get
      parameters:
      - in: path
        name: link_id
        description: The unique identifier of the view only link
      responses:
        200:
          description: OK
      tags:
      - View
      - Only
      - Links
      - Link
      - Nodes
  /wikis/{wiki_id}/:
    get:
      summary: Retrieve a Wiki
      description: |-
        Retrieves the details about a specific wiki.
        A wiki is a collection of markdown text pages that can be used to describe the project or dataset of contained in the attached node.
        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested wiki, if the request was successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: wiki_read
      x-api-path-slug: wikiswiki-id-get
      parameters:
      - in: path
        name: wiki_id
        description: The unique identifier of the wiki
      responses:
        200:
          description: OK
      tags:
      - Wikis
      - Wiki
  /wikis/{wiki_id}/content/:
    get:
      summary: Retrieve the Content of a Wiki
      description: |-
        Retrieves the plaintext content of a wiki in markdown format.
        ####Returns
        Returns `text/markdown` of the wiki content itself.
        If the request is unsuccessful, plaintext with the error message will be displayed.
      operationId: wiki_content
      x-api-path-slug: wikiswiki-idcontent-get
      parameters:
      - in: path
        name: wiki_id
        description: The unique identifier of the wiki
      responses:
        200:
          description: OK
      tags:
      - Wikis
      - Wiki
      - Content