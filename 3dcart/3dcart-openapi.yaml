swagger: "2.0"
x-collection-name: 3dcart
x-complete: 1
info:
  title: _3dCartWebAPI
  version: 1.0.0
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/Cart:
    post:
      summary: Adds a new cart to the system
      description: Adds a new cart to the system.
      operationId: Carts_Post
      x-api-path-slug: 3dcartwebapiv1cart-post
      parameters:
      - in: body
        name: cart
        description: A Json or XML object containing the new cart
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Cart
      - To
      - System
  /3dCartWebAPI/v1/Cart/{orderkey}:
    get:
      summary: Get a specific cart
      description: Get a specific cart.
      operationId: Carts_GetCart
      x-api-path-slug: 3dcartwebapiv1cartorderkey-get
      parameters:
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Cart
    put:
      summary: This method is used to update a single cart record in the database.
        The {orderkey} parameter specifies which cart record to update.
      description: This method is used to update a single cart record in the database.
        the {orderkey} parameter specifies which cart record to update..
      operationId: Carts_Update
      x-api-path-slug: 3dcartwebapiv1cartorderkey-put
      parameters:
      - in: body
        name: cart
        description: A Json or XML object containing the cart
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Cart
      - Record
      - In
      - Database
      - ""
      - Orderkey
      - Parameter
      - Specifies
      - Which
      - Cart
      - Record
      - To
      - Update
    delete:
      summary: Delete a Cart in the system
      description: Delete a cart in the system.
      operationId: Carts_Delete
      x-api-path-slug: 3dcartwebapiv1cartorderkey-delete
      parameters:
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Cart
      - In
      - System
  /3dCartWebAPI/v1/Cart/{orderkey}/Item:
    post:
      summary: Adds a new item to a cart
      description: Adds a new item to a cart.
      operationId: Carts_Post
      x-api-path-slug: 3dcartwebapiv1cartorderkeyitem-post
      parameters:
      - in: body
        name: item
        description: A Json or XML object containing the new cart item
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Item
      - To
      - Cart
  /3dCartWebAPI/v1/Cart/{orderkey}/Item/{cartitemid}:
    put:
      summary: Updates a specific item from a specific Cart
      description: Updates a specific item from a specific cart.
      operationId: Carts_Update
      x-api-path-slug: 3dcartwebapiv1cartorderkeyitemcartitemid-put
      parameters:
      - in: path
        name: cartitemid
        description: The unique index ID of an Item
      - in: body
        name: item
        description: A Json or XML object containing the new cart item
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Item
      - From
      - Specific
      - Cart
    delete:
      summary: Deletes a CartItem in the system
      description: Deletes a cartitem in the system.
      operationId: Carts_Delete
      x-api-path-slug: 3dcartwebapiv1cartorderkeyitemcartitemid-delete
      parameters:
      - in: path
        name: cartitemid
        description: The unique index ID of an Item
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - CartItem
      - In
      - System
  /3dCartWebAPI/v1/Categories:
    get:
      summary: Get all Categories
      description: Get all categories.
      operationId: Category_GetAllCategories
      x-api-path-slug: 3dcartwebapiv1categories-get
      parameters:
      - in: query
        name: category
        description: Name of the Category
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Categories
    put:
      summary: This method is used to update multiple category records in the database.
        No {categoryid} parameters should be included.
      description: This method is used to update multiple category records in the
        database. no {categoryid} parameters should be included..
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categories-put
      parameters:
      - in: body
        name: categories
        description: A Json or XML object containing the new categories
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Category
      - Records
      - In
      - Database
      - ""
      - "No"
      - Categoryid
      - Parameters
      - Should
      - Be
      - Included
    post:
      summary: Adds a new category to the system
      description: Adds a new category to the system.
      operationId: Category_Post
      x-api-path-slug: 3dcartwebapiv1categories-post
      parameters:
      - in: body
        name: category
        description: A Json or XML object containing the new category
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Category
      - To
      - System
  /3dCartWebAPI/v1/Categories/{categoryid}:
    put:
      summary: This method is used to update a single category record in the database.
        The {categoryid} parameter specifies which category to update.
      description: This method is used to update a single category record in the database.
        the {categoryid} parameter specifies which category to update..
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categoriescategoryid-put
      parameters:
      - in: body
        name: category
        description: A Json or XML object containing the new category
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryid
        description: Category ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Category
      - Record
      - In
      - Database
      - ""
      - Categoryid
      - Parameter
      - Specifies
      - Which
      - Category
      - To
      - Update
  /3dCartWebAPI/v1/Categories/{categoryid}/Options:
    get:
      summary: Get the options from a specific Category
      description: Get the options from a specific category.
      operationId: Category_GetAllCategoryOptions
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptions-get
      parameters:
      - in: path
        name: categoryid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Options
      - From
      - Specific
      - Category
    put:
      summary: Updates a collection of options from a specific Category
      description: Updates a collection of options from a specific category.
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptions-put
      parameters:
      - in: path
        name: categoryid
        description: CategoryID
      - in: body
        name: options
        description: A Json or XML object containing the new options
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Options
      - From
      - Specific
      - Category
    post:
      summary: Adds a new OptionSet to the system
      description: Adds a new optionset to the system.
      operationId: Category_Post
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptions-post
      parameters:
      - in: path
        name: categoryid
        description: Category ID
      - in: body
        name: optionset
        description: A Json or XML object containing the new optionset
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - OptionSet
      - To
      - System
  /3dCartWebAPI/v1/Categories/{categoryid}/Options/{optionsetid}:
    put:
      summary: Updates specific options from a specific Category
      description: Updates specific options from a specific category.
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptionsoptionsetid-put
      parameters:
      - in: path
        name: categoryid
        description: CategoryID
      - in: body
        name: option
        description: A Json or XML object containing the new options
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: optionsetid
        description: OptionSetID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Options
      - From
      - Specific
      - Category
  /3dCartWebAPI/v1/Categories/{categoryid}/Products:
    get:
      summary: Get all products from a specific category
      description: Get all products from a specific category.
      operationId: Products_GetAllProductsFromCategory
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidproducts-get
      parameters:
      - in: path
        name: categoryid
        description: ID of the category
      - in: query
        name: categoryspecial
        description: Category Special Flag
      - in: query
        name: costfrom
        description: Cost of a product
      - in: query
        name: costto
        description: Cost of a product
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: freeshipping
        description: Free Shipping Flag
      - in: query
        name: giftcertificate
        description: Gift Certificate Flag
      - in: query
        name: hide
        description: Hide Flag
      - in: query
        name: homespecial
        description: Home Special Flag
      - in: query
        name: lastupdateend
        description: End Date that the product was last updated (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: lastupdatestart
        description: Start Date that the product was last updated (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: name
        description: Name of the product
      - in: query
        name: nonsearchable
        description: Non-Searchable Flag
      - in: query
        name: nontax
        description: Non-Taxable Flag
      - in: query
        name: notforsale
        description: Not For Sale Flag
      - in: query
        name: offset
        description: Starting point for the return data
      - in: query
        name: onsale
        description: On Sale Flag
      - in: query
        name: pricefrom
        description: Price of a product
      - in: query
        name: priceto
        description: Price of a product
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: query
        name: rewarddisable
        description: Disable Rewards Flag
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: selfship
        description: Ships by itself Flag
      - in: query
        name: sku
        description: SKU Code of the product
      - in: query
        name: stockfrom
        description: Stock of a product
      - in: query
        name: stockto
        description: Stock of a product
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Products
      - From
      - Specific
      - Category
  /3dCartWebAPI/v1/Categories/{id}:
    get:
      summary: Get a Category
      description: Get a category.
      operationId: Category_GetCategory
      x-api-path-slug: 3dcartwebapiv1categoriesid-get
      parameters:
      - in: path
        name: id
        description: Category ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Category
    delete:
      summary: Deletes a Category in the system
      description: Deletes a category in the system.
      operationId: Category_Delete
      x-api-path-slug: 3dcartwebapiv1categoriesid-delete
      parameters:
      - in: path
        name: id
        description: Category ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Category
      - In
      - System
  /3dCartWebAPI/v1/CRM:
    get:
      summary: Get all CRMs
      description: Get all crms.
      operationId: CRM_GetAllCRMs
      x-api-path-slug: 3dcartwebapiv1crm-get
      parameters:
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: custid
        description: Customer Id associated with the CRM
      - in: query
        name: customeremail
        description: Customer Email
      - in: query
        name: customeripaddress
        description: Customer Ip Address
      - in: query
        name: customername
        description: Customer Name
      - in: query
        name: customerphone
        description: Customer Phone
      - in: query
        name: departmentid
        description: Department of the CRM
      - in: query
        name: lastactionenddate
        description: Date Last Action (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: lastactionstartdate
        description: Date Opened (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: query
        name: openedenddate
        description: Date Last Action (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: openedstartdate
        description: Date Opened (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: orderid
        description: Order Id associated with the CRM
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: query
        name: productid
        description: Product Id associated with the CRM
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: statusid
        description: Status of the CRM
      - in: query
        name: subject
        description: Subject of the CRM
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - CRMs
    post:
      summary: Adds a new CRM to the system
      description: Adds a new crm to the system.
      operationId: CRM_PostCRM
      x-api-path-slug: 3dcartwebapiv1crm-post
      parameters:
      - in: body
        name: crm
        description: A Json or XML object containing the new CRM
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - CRM
      - To
      - System
  /3dCartWebAPI/v1/CRM/{crmid}/message:
    get:
      summary: Get all the messages from a specific CRM
      description: Get all the messages from a specific crm.
      operationId: CRM_GetAllCRMMessages
      x-api-path-slug: 3dcartwebapiv1crmcrmidmessage-get
      parameters:
      - in: path
        name: crmid
        description: CRM ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Messages
      - From
      - Specific
      - CRM
  /3dCartWebAPI/v1/CRM/{crmid}/message/{msgid}:
    get:
      summary: Get a specific Message
      description: Get a specific message.
      operationId: CRM_GetCRMMessage
      x-api-path-slug: 3dcartwebapiv1crmcrmidmessagemsgid-get
      parameters:
      - in: path
        name: crmid
        description: CRM ID
      - in: path
        name: msgid
        description: Message ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Message
    delete:
      summary: Delete a CRM Message in the system
      description: Delete a crm message in the system.
      operationId: CRM_DeleteCRM
      x-api-path-slug: 3dcartwebapiv1crmcrmidmessagemsgid-delete
      parameters:
      - in: path
        name: crmid
        description: CrmID
      - in: path
        name: msgid
        description: MessageID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - CRM
      - Message
      - In
      - System
  /3dCartWebAPI/v1/CRM/{id}:
    get:
      summary: Get a specific CRM
      description: Get a specific crm.
      operationId: CRM_GetCRM
      x-api-path-slug: 3dcartwebapiv1crmid-get
      parameters:
      - in: path
        name: id
        description: CRM ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Specific
      - CRM
    put:
      summary: This method is used to update a single CRM record in the database.
        The {id} parameter specifies which CRM record to update.
      description: This method is used to update a single crm record in the database.
        the {id} parameter specifies which crm record to update..
      operationId: CRM_UpdateCRM
      x-api-path-slug: 3dcartwebapiv1crmid-put
      parameters:
      - in: body
        name: crm
        description: A Json or XML object containing the new product
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Crm ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - CRM
      - Record
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - CRM
      - Record
      - To
      - Update
    delete:
      summary: Delete a CRM in the system
      description: Delete a crm in the system.
      operationId: CRM_DeleteCRM
      x-api-path-slug: 3dcartwebapiv1crmid-delete
      parameters:
      - in: path
        name: id
        description: CrmID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - CRM
      - In
      - System
  /3dCartWebAPI/v1/CRM/{id}/message:
    post:
      summary: Adds a new CRM Message to the system
      description: Adds a new crm message to the system.
      operationId: CRM_PostMessage
      x-api-path-slug: 3dcartwebapiv1crmidmessage-post
      parameters:
      - in: path
        name: id
        description: Id of the CRM where the message will be added
      - in: body
        name: message
        description: A Json or XML object containing the new CRM message
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - CRM
      - Message
      - To
      - System
  /3dCartWebAPI/v1/CRM/department:
    get:
      summary: Get all CRM Departments
      description: Get all crm departments.
      operationId: CRM_GetAllCRMDepartments
      x-api-path-slug: 3dcartwebapiv1crmdepartment-get
      parameters:
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - CRM
      - Departments
  /3dCartWebAPI/v1/CRM/department/{id}:
    put:
      summary: This method is used to update a single CRM Department record in the
        database. The {id} parameter specifies which CRM Department record to update.
      description: This method is used to update a single crm department record in
        the database. the {id} parameter specifies which crm department record to
        update..
      operationId: CRM_UpdateDepartment
      x-api-path-slug: 3dcartwebapiv1crmdepartmentid-put
      parameters:
      - in: body
        name: department
        description: A Json or XML object containing the new Department
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Department ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - CRM
      - Department
      - Record
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - CRM
      - Department
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/CRM/savedreply:
    get:
      summary: Get all CRMs
      description: Get all crms.
      operationId: CRM_GetAllCRMSavedReplies
      x-api-path-slug: 3dcartwebapiv1crmsavedreply-get
      parameters:
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: title
        description: Title
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - CRMs
    post:
      summary: Adds a new CRM SaveReply to the system
      description: Adds a new crm savereply to the system.
      operationId: CRM_PostSavedReply
      x-api-path-slug: 3dcartwebapiv1crmsavedreply-post
      parameters:
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: savereply
        description: A Json or XML object containing the new CRM SavedReply
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - CRM
      - SaveReply
      - To
      - System
  /3dCartWebAPI/v1/CRM/savedreply/{id}:
    get:
      summary: Get a specific CRM Saved Reply
      description: Get a specific crm saved reply.
      operationId: CRM_GetCRMSavedReply
      x-api-path-slug: 3dcartwebapiv1crmsavedreplyid-get
      parameters:
      - in: path
        name: id
        description: CRM Saved Reply ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Specific
      - CRM
      - Saved
      - Reply
    put:
      summary: This method is used to update a single CRM SavedReply record in the
        database. The {id} parameter specifies which CRM SavedReply record to update.
      description: This method is used to update a single crm savedreply record in
        the database. the {id} parameter specifies which crm savedreply record to
        update..
      operationId: CRM_UpdateSavedReply
      x-api-path-slug: 3dcartwebapiv1crmsavedreplyid-put
      parameters:
      - in: path
        name: id
        description: SavedReply ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: savedreply
        description: A Json or XML object containing the new SavedReply
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - CRM
      - SavedReply
      - Record
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - CRM
      - SavedReply
      - Record
      - To
      - Update
    delete:
      summary: Delete a CRM SavedReply in the system
      description: Delete a crm savedreply in the system.
      operationId: CRM_DeleteCRMSavedReply
      x-api-path-slug: 3dcartwebapiv1crmsavedreplyid-delete
      parameters:
      - in: path
        name: id
        description: SavedReplyID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - CRM
      - SavedReply
      - In
      - System
  /3dCartWebAPI/v1/CRM/status:
    get:
      summary: Get all CRM Status
      description: Get all crm status.
      operationId: CRM_GetAllCRMStatus
      x-api-path-slug: 3dcartwebapiv1crmstatus-get
      parameters:
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - CRM
      - Status
  /3dCartWebAPI/v1/CRM/status/{id}:
    put:
      summary: This method is used to update a single CRM Status record in the database.
        The {id} parameter specifies which CRM Status record to update.
      description: This method is used to update a single crm status record in the
        database. the {id} parameter specifies which crm status record to update..
      operationId: CRM_UpdateStatus
      x-api-path-slug: 3dcartwebapiv1crmstatusid-put
      parameters:
      - in: path
        name: id
        description: Status ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: status
        description: A Json or XML object containing the new Status
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - CRM
      - Status
      - Record
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - CRM
      - Status
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/CustomerGroups:
    get:
      summary: Get all CustomerGroups
      description: Get all customergroups.
      operationId: CustomerGroups_GetAllCustomerGroups
      x-api-path-slug: 3dcartwebapiv1customergroups-get
      parameters:
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - CustomerGroups
    put:
      summary: This method updates a collection of customer groups in the database.
        No URL parameters should be included.
      description: This method updates a collection of customer groups in the database.
        no url parameters should be included..
      operationId: CustomerGroups_Update
      x-api-path-slug: 3dcartwebapiv1customergroups-put
      parameters:
      - in: body
        name: customergroups
        description: A Json or XML object containing the customer group
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Updates
      - Collection
      - Of
      - Customer
      - Groups
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
    post:
      summary: Adds a new customer group to the system
      description: Adds a new customer group to the system.
      operationId: CustomerGroups_Post
      x-api-path-slug: 3dcartwebapiv1customergroups-post
      parameters:
      - in: body
        name: customergroup
        description: A Json or XML object containing the new customer group
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Customer
      - Group
      - To
      - System
  /3dCartWebAPI/v1/CustomerGroups/{customergroupid}:
    put:
      summary: This method is used to update a single customer group in the database.
        The {id} parameter specifies which customer group to update.
      description: This method is used to update a single customer group in the database.
        the {id} parameter specifies which customer group to update..
      operationId: CustomerGroups_Update
      x-api-path-slug: 3dcartwebapiv1customergroupscustomergroupid-put
      parameters:
      - in: body
        name: customergroup
        description: A Json or XML object containing the customer group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customergroupid
        description: Customer Group ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Customer
      - Group
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - Customer
      - Group
      - To
      - Update
  /3dCartWebAPI/v1/CustomerGroups/{id}:
    get:
      summary: Get a CustomerGroup
      description: Get a customergroup.
      operationId: CustomerGroups_GetCustomerGroup
      x-api-path-slug: 3dcartwebapiv1customergroupsid-get
      parameters:
      - in: path
        name: id
        description: Customer Group ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - CustomerGroup
    delete:
      summary: Deletes a customer group in the system
      description: Deletes a customer group in the system.
      operationId: CustomerGroups_Delete
      x-api-path-slug: 3dcartwebapiv1customergroupsid-delete
      parameters:
      - in: path
        name: id
        description: Customer Group ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Customer
      - Group
      - In
      - System
  /3dCartWebAPI/v1/CustomerGroups/{id}/Customers:
    get:
      summary: Get Customers from a Customer Group
      description: Get customers from a customer group.
      operationId: Customers_GetCustomerFromCustomerGroup
      x-api-path-slug: 3dcartwebapiv1customergroupsidcustomers-get
      parameters:
      - in: query
        name: city
        description: City of the Customer
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: country
        description: Country name of the Customer
      - in: query
        name: email
        description: Email of the Customer
      - in: query
        name: firstname
        description: Firstname of the Customer
      - in: path
        name: id
        description: Customer Group ID
      - in: query
        name: lastname
        description: Lastname of the Customer
      - in: query
        name: lastupdateend
        description: End Date that the product was last updated (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: lastupdatestart
        description: Start Date that the product was last updated (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: query
        name: phone
        description: Phone of the Customer
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: state
        description: State of the Customer
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Customers
      - From
      - Customer
      - Group
  /3dCartWebAPI/v1/Customers:
    get:
      summary: Get all Customers
      description: Get all customers.
      operationId: Customers_GetAllCustomers
      x-api-path-slug: 3dcartwebapiv1customers-get
      parameters:
      - in: query
        name: city
        description: City of the Customer
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: country
        description: Country name of the Customer
      - in: query
        name: email
        description: Email of the Customer
      - in: query
        name: firstname
        description: Firstname of the Customer
      - in: query
        name: lastname
        description: Lastname of the Customer
      - in: query
        name: lastupdateend
        description: End Date that the product was last updated (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: lastupdatestart
        description: Start Date that the product was last updated (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: query
        name: phone
        description: Phone of the Customer
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: state
        description: State of the Customer
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Customers
    put:
      summary: This method is used to update multiple customers in the system. No
        URL parameters should be included.
      description: This method is used to update multiple customers in the system.
        no url parameters should be included..
      operationId: Customers_Update
      x-api-path-slug: 3dcartwebapiv1customers-put
      parameters:
      - in: body
        name: customers
        description: A Json or XML object containing the new customer
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Customers
      - In
      - System
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
    post:
      summary: Adds a new customer to the system
      description: Adds a new customer to the system.
      operationId: Customers_Post
      x-api-path-slug: 3dcartwebapiv1customers-post
      parameters:
      - in: body
        name: customer
        description: A Json or XML object containing the new customer
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Customer
      - To
      - System
  /3dCartWebAPI/v1/Customers/{customerid}:
    put:
      summary: This method is used to update a single customer record in the database.
        The {id} parameter specifies which customer record to update.
      description: This method is used to update a single customer record in the database.
        the {id} parameter specifies which customer record to update..
      operationId: Customers_Update
      x-api-path-slug: 3dcartwebapiv1customerscustomerid-put
      parameters:
      - in: body
        name: customer
        description: A Json or XML object containing the new customer
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: customerid
        description: Customer ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Customer
      - Record
      - In
      - Database
      - ""
      - Id
      - Parameter
      - Specifies
      - Which
      - Customer
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/Customers/{id}:
    get:
      summary: Get a Customer
      description: Get a customer.
      operationId: Customers_GetAllCustomers
      x-api-path-slug: 3dcartwebapiv1customersid-get
      parameters:
      - in: path
        name: id
        description: Customer ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Customer
    delete:
      summary: Deletes a Customer in the system
      description: Deletes a customer in the system.
      operationId: Customers_Delete
      x-api-path-slug: 3dcartwebapiv1customersid-delete
      parameters:
      - in: path
        name: id
        description: Customer ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Customer
      - In
      - System
  /3dCartWebAPI/v1/Distributors:
    get:
      summary: Get all Distributors
      description: Get all distributors.
      operationId: Distributors_GetAllDistributors
      x-api-path-slug: 3dcartwebapiv1distributors-get
      parameters:
      - in: query
        name: city
        description: City of the Distributor
      - in: query
        name: company
        description: Company Name of the Distributor
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: country
        description: Country name of the Distributor
      - in: query
        name: email
        description: Email of the Distributor
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: query
        name: phone
        description: Phone of the Distributor
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: state
        description: State of the Distributor
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Distributors
    put:
      summary: This method is used to update multiple distributor records in the database.
        No {distributorid} parameters should be included.
      description: This method is used to update multiple distributor records in the
        database. no {distributorid} parameters should be included..
      operationId: Distributors_Update
      x-api-path-slug: 3dcartwebapiv1distributors-put
      parameters:
      - in: body
        name: distributors
        description: A Json or XML object containing the new distributors
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Distributor
      - Records
      - In
      - Database
      - ""
      - "No"
      - Distributorid
      - Parameters
      - Should
      - Be
      - Included
    post:
      summary: Adds a new distributor to the system
      description: Adds a new distributor to the system.
      operationId: Distributors_Post
      x-api-path-slug: 3dcartwebapiv1distributors-post
      parameters:
      - in: body
        name: distributor
        description: A Json or XML object containing the new distributor
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Distributor
      - To
      - System
  /3dCartWebAPI/v1/Distributors/{distributorid}:
    put:
      summary: This method is used to update a single distributor record in the database.
        The {distributorid} parameter specifies which distributor to update.
      description: This method is used to update a single distributor record in the
        database. the {distributorid} parameter specifies which distributor to update..
      operationId: Distributors_Update
      x-api-path-slug: 3dcartwebapiv1distributorsdistributorid-put
      parameters:
      - in: body
        name: distributor
        description: A Json or XML object containing the new distributor
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: distributorid
        description: Distributor ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Distributor
      - Record
      - In
      - Database
      - ""
      - Distributorid
      - Parameter
      - Specifies
      - Which
      - Distributor
      - To
      - Update
  /3dCartWebAPI/v1/Distributors/{distributorid}/Products:
    get:
      summary: Get all products from a specific distributor
      description: Get all products from a specific distributor.
      operationId: Products_GetAllProductsFromDistributor
      x-api-path-slug: 3dcartwebapiv1distributorsdistributoridproducts-get
      parameters:
      - in: query
        name: categoryspecial
        description: Category Special Flag
      - in: query
        name: costfrom
        description: Cost of a product
      - in: query
        name: costto
        description: Cost of a product
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: path
        name: distributorid
        description: ID of the distributor
      - in: query
        name: freeshipping
        description: Free Shipping Flag
      - in: query
        name: giftcertificate
        description: Gift Certificate Flag
      - in: query
        name: hide
        description: Hide Flag
      - in: query
        name: homespecial
        description: Home Special Flag
      - in: query
        name: lastupdateend
        description: End Date that the product was last updated (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: lastupdatestart
        description: Start Date that the product was last updated (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: name
        description: Name of the product
      - in: query
        name: nonsearchable
        description: Non-Searchable Flag
      - in: query
        name: nontax
        description: Non-Taxable Flag
      - in: query
        name: notforsale
        description: Not For Sale Flag
      - in: query
        name: offset
        description: Starting point for the return data
      - in: query
        name: onsale
        description: On Sale Flag
      - in: query
        name: pricefrom
        description: Price of a product
      - in: query
        name: priceto
        description: Price of a product
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: query
        name: rewarddisable
        description: Disable Rewards Flag
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: selfship
        description: Ships by itself Flag
      - in: query
        name: sku
        description: SKU Code of the product
      - in: query
        name: stockfrom
        description: Stock of a product
      - in: query
        name: stockto
        description: Stock of a product
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Products
      - From
      - Specific
      - Distributor
  /3dCartWebAPI/v1/Distributors/{id}:
    get:
      summary: Get a Distributor
      description: Get a distributor.
      operationId: Distributors_GetAllDistributors
      x-api-path-slug: 3dcartwebapiv1distributorsid-get
      parameters:
      - in: path
        name: id
        description: Distributor ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Distributor
    delete:
      summary: Deletes a Distributor in the system
      description: Deletes a distributor in the system.
      operationId: Distributors_Delete
      x-api-path-slug: 3dcartwebapiv1distributorsid-delete
      parameters:
      - in: path
        name: id
        description: Distributor ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Distributor
      - In
      - System
  /3dCartWebAPI/v1/GiftRegistries:
    get:
      summary: Get all GiftRegistries
      description: Get all giftregistries.
      operationId: GiftRegistries_GetAllGiftRegistries
      x-api-path-slug: 3dcartwebapiv1giftregistries-get
      parameters:
      - in: query
        name: catalogid
        description: Catalog ID
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: dateendcreated
        description: Created Date End (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: dateendevent
        description: Event Date End (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: dateendexpiration
        description: Expiration Date End (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: datestartcreated
        description: Created Date Start (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: datestartevent
        description: Event Date Start (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: datestartexpiration
        description: Expiration Date Start (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: sku
        description: SKU Code of the product
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - GiftRegistries
  /3dCartWebAPI/v1/GiftRegistries/{giftregistryid}:
    get:
      summary: Get a specific GiftRegistry
      description: Get a specific giftregistry.
      operationId: GiftRegistries_GetGiftRegistry
      x-api-path-slug: 3dcartwebapiv1giftregistriesgiftregistryid-get
      parameters:
      - in: path
        name: giftregistryid
        description: Gift Resitry ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Specific
      - GiftRegistry
  /3dCartWebAPI/v1/GiftRegistries/{giftregistryid}/Items:
    get:
      summary: Gets the items from a specific Gift Registry
      description: Gets the items from a specific gift registry.
      operationId: GiftRegistries_GetAllGiftRegistryItem
      x-api-path-slug: 3dcartwebapiv1giftregistriesgiftregistryiditems-get
      parameters:
      - in: path
        name: giftregistryid
        description: Gift Registry ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Items
      - From
      - Specific
      - Gift
      - Registry
  /3dCartWebAPI/v1/Manufacturers:
    get:
      summary: Get all Manufacturers
      description: Get all manufacturers.
      operationId: Manufacturer_GetAllManufacturers
      x-api-path-slug: 3dcartwebapiv1manufacturers-get
      parameters:
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: manufacturer
        description: Name of the Manufacturer
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Manufacturers
    put:
      summary: This method is used to update multiple manufacturers in the database.
        No URL parameters should be included.
      description: This method is used to update multiple manufacturers in the database.
        no url parameters should be included..
      operationId: Manufacturer_Update
      x-api-path-slug: 3dcartwebapiv1manufacturers-put
      parameters:
      - in: body
        name: manufacturers
        description: A Json or XML object containing the new manufacturers
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Manufacturers
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
    post:
      summary: Adds a new manufacturer to the system
      description: Adds a new manufacturer to the system.
      operationId: Manufacturer_Post
      x-api-path-slug: 3dcartwebapiv1manufacturers-post
      parameters:
      - in: body
        name: manufacturer
        description: A Json or XML object containing the new manufacturer
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Manufacturer
      - To
      - System
  /3dCartWebAPI/v1/Manufacturers/{id}:
    get:
      summary: Get a Manufacturer
      description: Get a manufacturer.
      operationId: Manufacturer_GetManufacturer
      x-api-path-slug: 3dcartwebapiv1manufacturersid-get
      parameters:
      - in: path
        name: id
        description: Manufacturer ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Manufacturer
    delete:
      summary: Deletes a Manufacturer in the system
      description: Deletes a manufacturer in the system.
      operationId: Manufacturer_Delete
      x-api-path-slug: 3dcartwebapiv1manufacturersid-delete
      parameters:
      - in: path
        name: id
        description: Manufacturer ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Manufacturer
      - In
      - System
  /3dCartWebAPI/v1/Manufacturers/{manufacturerid}:
    put:
      summary: This method is used to update a single manufacturer record in the database.
        The {manufacturerid} parameter specifies which manufacturer record to update.
      description: This method is used to update a single manufacturer record in the
        database. the {manufacturerid} parameter specifies which manufacturer record
        to update..
      operationId: Manufacturer_Update
      x-api-path-slug: 3dcartwebapiv1manufacturersmanufacturerid-put
      parameters:
      - in: body
        name: manufacturer
        description: A Json or XML object containing the new manufacturer
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: manufacturerid
        description: Manufacturer ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Manufacturer
      - Record
      - In
      - Database
      - ""
      - Manufacturerid
      - Parameter
      - Specifies
      - Which
      - Manufacturer
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/Manufacturers/{manufacturerid}/Products:
    get:
      summary: Get all products from a specific manufacturer
      description: Get all products from a specific manufacturer.
      operationId: Products_GetAllProductsFromManufacturer
      x-api-path-slug: 3dcartwebapiv1manufacturersmanufactureridproducts-get
      parameters:
      - in: query
        name: categoryspecial
        description: Category Special Flag
      - in: query
        name: costfrom
        description: Cost of a product
      - in: query
        name: costto
        description: Cost of a product
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: freeshipping
        description: Free Shipping Flag
      - in: query
        name: giftcertificate
        description: Gift Certificate Flag
      - in: query
        name: hide
        description: Hide Flag
      - in: query
        name: homespecial
        description: Home Special Flag
      - in: query
        name: lastupdateend
        description: End Date that the product was last updated (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: lastupdatestart
        description: Start Date that the product was last updated (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: path
        name: manufacturerid
        description: ID of the manufacturer
      - in: query
        name: name
        description: Name of the product
      - in: query
        name: nonsearchable
        description: Non-Searchable Flag
      - in: query
        name: nontax
        description: Non-Taxable Flag
      - in: query
        name: notforsale
        description: Not For Sale Flag
      - in: query
        name: offset
        description: Starting point for the return data
      - in: query
        name: onsale
        description: On Sale Flag
      - in: query
        name: pricefrom
        description: Price of a product
      - in: query
        name: priceto
        description: Price of a product
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: query
        name: rewarddisable
        description: Disable Rewards Flag
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: selfship
        description: Ships by itself Flag
      - in: query
        name: sku
        description: SKU Code of the product
      - in: query
        name: stockfrom
        description: Stock of a product
      - in: query
        name: stockto
        description: Stock of a product
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Products
      - From
      - Specific
      - Manufacturer
  /3dCartWebAPI/v1/Orders:
    get:
      summary: ""
      description: .
      operationId: Orders_GetAllOrders
      x-api-path-slug: 3dcartwebapiv1orders-get
      parameters:
      - in: query
        name: billingemail
      - in: query
        name: countonly
      - in: query
        name: dateend
      - in: query
        name: datestart
      - in: query
        name: invoicenumber
      - in: query
        name: invoicenumberend
      - in: query
        name: invoicenumberstart
      - in: query
        name: invoiceprefix
      - in: query
        name: lastupdateend
      - in: query
        name: lastupdatestart
      - in: query
        name: limit
      - in: query
        name: offset
      - in: query
        name: orderstatus
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - ""
    put:
      summary: This method is used to update multiple orders in the database. No URL
        parameters should be included.
      description: This method is used to update multiple orders in the database.
        no url parameters should be included..
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1orders-put
      parameters:
      - in: body
        name: orders
        description: A Json or XML object containing the orders
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Orders
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
    post:
      summary: Adds a new order to the system
      description: Adds a new order to the system.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1orders-post
      parameters:
      - in: query
        name: bypassorderemail
        description: will bypass sending the customer new order email if normally
          applicable
      - in: query
        name: bypassorderprocessing
        description: will bypass/ignore stock updates, gift certificates generation,
          rewards, etc
      - in: body
        name: order
        description: A Json or XML object containing the new order
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Order
      - To
      - System
  /3dCartWebAPI/v1/Orders/{orderid}:
    get:
      summary: Get a specific order
      description: Get a specific order.
      operationId: Orders_GetOrder
      x-api-path-slug: 3dcartwebapiv1ordersorderid-get
      parameters:
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Order
    put:
      summary: This method is used to update a single order record in the database.
        The {orderid} parameter specifies which order record to update.
      description: This method is used to update a single order record in the database.
        the {orderid} parameter specifies which order record to update..
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderid-put
      parameters:
      - in: body
        name: order
        description: A Json or XML object containing the order
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Order
      - Record
      - In
      - Database
      - ""
      - Orderid
      - Parameter
      - Specifies
      - Which
      - Order
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/Orders/{orderid}/Items:
    get:
      summary: Gets the items from a specific Order
      description: Gets the items from a specific order.
      operationId: Orders_GetAllOrderItems
      x-api-path-slug: 3dcartwebapiv1ordersorderiditems-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Items
      - From
      - Specific
      - Order
    put:
      summary: Updates a collection of items from a specific Order
      description: Updates a collection of items from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderiditems-put
      parameters:
      - in: body
        name: items
        description: A Json or XML object containing the new items
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Items
      - From
      - Specific
      - Order
    post:
      summary: Adds a new item on the order
      description: Adds a new item on the order.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1ordersorderiditems-post
      parameters:
      - in: body
        name: item
        description: A Json or XML object containing the new item
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Item
      - "On"
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Items/{itemindexid}:
    put:
      summary: Updates a specific item from a specific Product
      description: Updates a specific item from a specific product.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderiditemsitemindexid-put
      parameters:
      - in: body
        name: item
        description: A Json or XML object containing the new item
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: itemindexid
        description: The unique indexID of an Item
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Item
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Orders/{orderid}/Questions:
    get:
      summary: Gets the questions from a specific Order
      description: Gets the questions from a specific order.
      operationId: Orders_GetAllOrderQuestions
      x-api-path-slug: 3dcartwebapiv1ordersorderidquestions-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Questions
      - From
      - Specific
      - Order
    put:
      summary: Updates a collection of questions from a specific Order
      description: Updates a collection of questions from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidquestions-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: questions
        description: A Json or XML object containing the new questions
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Questions
      - From
      - Specific
      - Order
    post:
      summary: Adds a new question on the order
      description: Adds a new question on the order.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1ordersorderidquestions-post
      parameters:
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: question
        description: A Json or XML object containing the new question
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Question
      - "On"
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Questions/{questionanswerindexid}:
    put:
      summary: Updates a specific question from a specific Product
      description: Updates a specific question from a specific product.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidquestionsquestionanswerindexid-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: question
        description: A Json or XML object containing the new question
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: questionanswerindexid
        description: QuestionID
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Question
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Orders/{orderid}/Shipments:
    get:
      summary: Gets the shipments from a specific Order
      description: Gets the shipments from a specific order.
      operationId: Orders_GetAllOrderShipments
      x-api-path-slug: 3dcartwebapiv1ordersorderidshipments-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: path
        name: orderid
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Shipments
      - From
      - Specific
      - Order
    put:
      summary: Updates a collection of shipments from a specific Order
      description: Updates a collection of shipments from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidshipments-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: shipments
        description: A Json or XML object containing the new shipments
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Shipments
      - From
      - Specific
      - Order
    post:
      summary: Adds a new shipment on the order
      description: Adds a new shipment on the order.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1ordersorderidshipments-post
      parameters:
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: shipment
        description: A Json or XML object containing the new shipment
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Shipment
      - "On"
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Shipments/{shipmentid}:
    put:
      summary: Updates a specific shipment from a specific Order
      description: Updates a specific shipment from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidshipmentsshipmentid-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: shipment
        description: A Json or XML object containing the new shipment
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: shipmentid
        description: ShipmentID
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Shipment
      - From
      - Specific
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Transactions:
    get:
      summary: Gets the transactions from a specific Order
      description: Gets the transactions from a specific order.
      operationId: Orders_GetAllOrderTransactions
      x-api-path-slug: 3dcartwebapiv1ordersorderidtransactions-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Transactions
      - From
      - Specific
      - Order
    put:
      summary: Updates a collection of transactions from a specific Order
      description: Updates a collection of transactions from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidtransactions-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: transactions
        description: A Json or XML object containing the new transactions
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Transactions
      - From
      - Specific
      - Order
    post:
      summary: Adds a new transaction on the order
      description: Adds a new transaction on the order.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1ordersorderidtransactions-post
      parameters:
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: transaction
        description: A Json or XML object containing the new transaction
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Transaction
      - "On"
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Transactions/{transactionindexid}:
    put:
      summary: Updates a specific transaction from a specific Product
      description: Updates a specific transaction from a specific product.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidtransactionstransactionindexid-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: transaction
        description: A Json or XML object containing the new transaction
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: transactionindexid
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Transaction
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/OrderStatus:
    get:
      summary: Get all OrderStatus
      description: Get all orderstatus.
      operationId: OrderStatus_GetAllOrderStatus
      x-api-path-slug: 3dcartwebapiv1orderstatus-get
      parameters:
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - OrderStatus
  /3dCartWebAPI/v1/OrderStatus/{id}:
    get:
      summary: Get an OrderStatus
      description: Get an orderstatus.
      operationId: OrderStatus_GetOrderStatus
      x-api-path-slug: 3dcartwebapiv1orderstatusid-get
      parameters:
      - in: path
        name: id
        description: OrderStatus ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - OrderStatus
  /3dCartWebAPI/v1/PaymentTokens:
    get:
      summary: Get all Payment Tokens
      description: Get all payment tokens.
      operationId: PaymentToken_GetAllPaymentTokens
      x-api-path-slug: 3dcartwebapiv1paymenttokens-get
      parameters:
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Tokens
    put:
      summary: This method is used to update multiple paymenttokens in the database.
        No URL parameters should be included.
      description: This method is used to update multiple paymenttokens in the database.
        no url parameters should be included..
      operationId: PaymentToken_Update
      x-api-path-slug: 3dcartwebapiv1paymenttokens-put
      parameters:
      - in: body
        name: paymenttokens
        description: A Json or XML object containing the new PaymentTokens
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Paymenttokens
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
    post:
      summary: Adds a new paymenttoken to the system
      description: Adds a new paymenttoken to the system.
      operationId: PaymentToken_Post
      x-api-path-slug: 3dcartwebapiv1paymenttokens-post
      parameters:
      - in: body
        name: paymenttoken
        description: A Json or XML object containing the new manufacturer
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Paymenttoken
      - To
      - System
  /3dCartWebAPI/v1/PaymentTokens/{id}:
    get:
      summary: Get a Payment Token
      description: Get a payment token.
      operationId: PaymentToken_GetPaymentToken
      x-api-path-slug: 3dcartwebapiv1paymenttokensid-get
      parameters:
      - in: path
        name: id
        description: PaymentTokenID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Token
    delete:
      summary: Deletes a Payment Token in the system
      description: Deletes a payment token in the system.
      operationId: PaymentToken_Delete
      x-api-path-slug: 3dcartwebapiv1paymenttokensid-delete
      parameters:
      - in: path
        name: id
        description: PaymentTokenID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Payment
      - Token
      - In
      - System
  /3dCartWebAPI/v1/PaymentTokens/{paymenttokenid}:
    put:
      summary: This method is used to update a single paymenttoken record in the database.
        The {paymenttokenid} parameter specifies which paymenttoken record to update.
      description: This method is used to update a single paymenttoken record in the
        database. the {paymenttokenid} parameter specifies which paymenttoken record
        to update..
      operationId: PaymentToken_Update
      x-api-path-slug: 3dcartwebapiv1paymenttokenspaymenttokenid-put
      parameters:
      - in: body
        name: paymenttoken
        description: A Json or XML object containing the new paymenttoken
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: paymenttokenid
        description: PaymentTokenID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Paymenttoken
      - Record
      - In
      - Database
      - ""
      - Paymenttokenid
      - Parameter
      - Specifies
      - Which
      - Paymenttoken
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/Products:
    get:
      summary: Get all products
      description: Get all products.
      operationId: Products_GetAllProducts
      x-api-path-slug: 3dcartwebapiv1products-get
      parameters:
      - in: query
        name: categoryspecial
        description: Category Special Flag
      - in: query
        name: costfrom
        description: Cost of a product
      - in: query
        name: costto
        description: Cost of a product
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: freeshipping
        description: Free Shipping Flag
      - in: query
        name: giftcertificate
        description: Gift Certificate Flag
      - in: query
        name: hide
        description: Hide Flag
      - in: query
        name: homespecial
        description: Home Special Flag
      - in: query
        name: lastupdateend
        description: End Date that the product was last updated (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: lastupdatestart
        description: Start Date that the product was last updated (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: name
        description: Name of the product
      - in: query
        name: nonsearchable
        description: Non-Searchable Flag
      - in: query
        name: nontax
        description: Non-Taxable Flag
      - in: query
        name: notforsale
        description: Not For Sale Flag
      - in: query
        name: offset
        description: Starting point for the return data
      - in: query
        name: onsale
        description: On Sale Flag
      - in: query
        name: pricefrom
        description: Price of a product
      - in: query
        name: priceto
        description: Price of a product
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: query
        name: rewarddisable
        description: Disable Rewards Flag
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: selfship
        description: Ships by itself Flag
      - in: query
        name: sku
        description: SKU Code of the product
      - in: query
        name: stockfrom
        description: Stock of a product
      - in: query
        name: stockto
        description: Stock of a product
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Products
    put:
      summary: This method is used to update multiple products in the database. No
        URL parameters should be included.
      description: This method is used to update multiple products in the database.
        no url parameters should be included..
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1products-put
      parameters:
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: products
        description: A Json or XML object containing the new product(s)
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Products
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
    post:
      summary: Adds a new product to the system
      description: Adds a new product to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1products-post
      parameters:
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: product
        description: A Json or XML object containing the new product
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Product
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}:
    get:
      summary: Get a product
      description: Get a product.
      operationId: Products_GetProduct
      x-api-path-slug: 3dcartwebapiv1productscatalogid-get
      parameters:
      - in: path
        name: catalogid
        description: Catalogid of the item
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Product
    put:
      summary: This method is used to update a single product record in the database.
        The {catalogid} parameter specifies which product record to update.
      description: This method is used to update a single product record in the database.
        the {catalogid} parameter specifies which product record to update..
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogid-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: product
        description: A Json or XML object containing the new product
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Product
      - Record
      - In
      - Database
      - ""
      - Catalogid
      - Parameter
      - Specifies
      - Which
      - Product
      - Record
      - To
      - Update
    delete:
      summary: Deletes a product in the system
      description: Deletes a product in the system.
      operationId: Products_Delete
      x-api-path-slug: 3dcartwebapiv1productscatalogid-delete
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Product
      - In
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/AdvancedOptions:
    get:
      summary: Get the advanced options from a specific Product
      description: Get the advanced options from a specific product.
      operationId: Products_GetAllProductAdvancedOptions
      x-api-path-slug: 3dcartwebapiv1productscatalogidadvancedoptions-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Advanced
      - Options
      - From
      - Specific
      - Product
    put:
      summary: Updates a collection of advanced options from a specific Product
      description: Updates a collection of advanced options from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidadvancedoptions-put
      parameters:
      - in: body
        name: advancedoptions
        description: A Json or XML object containing the new advanced options
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Advanced
      - Options
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/AdvancedOptions/{advancedoptioncode}:
    put:
      summary: Updates specific advanced options from a specific Product
      description: Updates specific advanced options from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidadvancedoptionsadvancedoptioncode-put
      parameters:
      - in: body
        name: advancedoption
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: advancedoptioncode
        description: AdvancedOptionCode
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Advanced
      - Options
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/Categories:
    get:
      summary: Get the categories from a specific Product
      description: Get the categories from a specific product.
      operationId: Products_GetAllProductCategories
      x-api-path-slug: 3dcartwebapiv1productscatalogidcategories-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Categories
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/Discount:
    get:
      summary: Get the discounts from a specific Product
      description: Get the discounts from a specific product.
      operationId: Products_GetAllProductDiscount
      x-api-path-slug: 3dcartwebapiv1productscatalogiddiscount-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Discounts
      - From
      - Specific
      - Product
    put:
      summary: Updates a collection of discounts from a specific Product
      description: Updates a collection of discounts from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogiddiscount-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: discounts
        description: A Json or XML object containing the new discount
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Discounts
      - From
      - Specific
      - Product
    post:
      summary: Adds a new discount to the system
      description: Adds a new discount to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogiddiscount-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: body
        name: discount
        description: A Json or XML object containing the new discount
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Discount
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/Discount/{discountid}:
    put:
      summary: Updates a specific discount from a specific Product
      description: Updates a specific discount from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogiddiscountdiscountid-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: discount
        description: A Json or XML object containing the new discounts
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: discountid
        description: DiscountID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Discount
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/Distributors:
    get:
      summary: Get the distributors from a specific Product
      description: Get the distributors from a specific product.
      operationId: Products_GetAllProductDistributors
      x-api-path-slug: 3dcartwebapiv1productscatalogiddistributors-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Distributors
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/EProducts:
    get:
      summary: Get the EProducts from a specific Product
      description: Get the eproducts from a specific product.
      operationId: Products_GetAllProductEProducts
      x-api-path-slug: 3dcartwebapiv1productscatalogideproducts-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - EProducts
      - From
      - Specific
      - Product
    put:
      summary: Updates a collection of eproducts from a specific Product
      description: Updates a collection of eproducts from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogideproducts-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: eproducts
        description: A Json or XML object containing the new features
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Eproducts
      - From
      - Specific
      - Product
    post:
      summary: Adds a new eproduct to the system
      description: Adds a new eproduct to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogideproducts-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: body
        name: eproduct
        description: A Json or XML object containing the new eproduct
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Eproduct
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/EProducts/{filenumber}:
    put:
      summary: Updates a specific eproduct from a specific Product
      description: Updates a specific eproduct from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogideproductsfilenumber-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: eproduct
        description: A Json or XML object containing the new features
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: filenumber
        description: FileNumber
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Eproduct
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/Features:
    get:
      summary: Get the features from a specific Product
      description: Get the features from a specific product.
      operationId: Products_GetAllProductFeatures
      x-api-path-slug: 3dcartwebapiv1productscatalogidfeatures-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Features
      - From
      - Specific
      - Product
    put:
      summary: Updates a collection of features from a specific Product
      description: Updates a collection of features from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidfeatures-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: features
        description: A Json or XML object containing the new features
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Features
      - From
      - Specific
      - Product
    post:
      summary: Adds a new feature to the system
      description: Adds a new feature to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogidfeatures-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: body
        name: feature
        description: A Json or XML object containing the new feature
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Feature
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/Features/{featureid}:
    put:
      summary: Updates a specific feature from a specific Product
      description: Updates a specific feature from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidfeaturesfeatureid-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: feature
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: featureid
        description: FeatureID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Feature
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/Images:
    get:
      summary: Get the images from a specific Product
      description: Get the images from a specific product.
      operationId: Products_GetAllProductImages
      x-api-path-slug: 3dcartwebapiv1productscatalogidimages-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Images
      - From
      - Specific
      - Product
    put:
      summary: Updates a collection of images from a specific Product
      description: Updates a collection of images from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidimages-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: images
        description: A Json or XML object containing the new images
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Images
      - From
      - Specific
      - Product
    post:
      summary: Adds a new image to the system
      description: Adds a new image to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogidimages-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: body
        name: image
        description: A Json or XML object containing the new image
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Image
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/Images/{imagegalleryid}:
    put:
      summary: Updates a specific image from a specific Product
      description: Updates a specific image from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidimagesimagegalleryid-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: image
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: imagegalleryid
        description: ImageGalleryID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Image
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/Options:
    get:
      summary: Get the options from a specific Product
      description: Get the options from a specific product.
      operationId: Products_GetAllProductOptions
      x-api-path-slug: 3dcartwebapiv1productscatalogidoptions-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Options
      - From
      - Specific
      - Product
    put:
      summary: Updates a collection of options from a specific Product
      description: Updates a collection of options from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidoptions-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: options
        description: A Json or XML object containing the new options
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Options
      - From
      - Specific
      - Product
    post:
      summary: Adds a new OptionSet to the system
      description: Adds a new optionset to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogidoptions-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: body
        name: optionset
        description: A Json or XML object containing the new optionset
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - OptionSet
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/Options/{optionsetid}:
    put:
      summary: Updates specific options from a specific Product
      description: Updates specific options from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidoptionsoptionsetid-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: option
        description: A Json or XML object containing the new options
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: optionsetid
        description: OptionSetID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Options
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/Related:
    get:
      summary: Get the related products from a specific Product
      description: Get the related products from a specific product.
      operationId: Products_GetAllProductRelated
      x-api-path-slug: 3dcartwebapiv1productscatalogidrelated-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Related
      - Products
      - From
      - Specific
      - Product
    put:
      summary: Updates a collection of related products from a specific Product
      description: Updates a collection of related products from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidrelated-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: relatedproducts
        description: A Json or XML object containing the new related products
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Related
      - Products
      - From
      - Specific
      - Product
    post:
      summary: Adds a new related product to the system
      description: Adds a new related product to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogidrelated-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: relatedproduct
        description: A Json or XML object containing the new related product
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Related
      - Product
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/Related/{relatedindexid}:
    put:
      summary: Updates a specific related product from a specific Product
      description: Updates a specific related product from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidrelatedrelatedindexid-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: path
        name: relatedindexid
        description: RelatedIndexID
      - in: body
        name: relatedproduct
        description: A Json or XML object containing the new related products
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Related
      - Product
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/Serials:
    get:
      summary: Get the serials from a specific Product
      description: Get the serials from a specific product.
      operationId: Products_GetAllProductSerials
      x-api-path-slug: 3dcartwebapiv1productscatalogidserials-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Serials
      - From
      - Specific
      - Product
    put:
      summary: Updates a collection of serials from a specific Product
      description: Updates a collection of serials from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidserials-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: serials
        description: A Json or XML object containing the new serials
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Serials
      - From
      - Specific
      - Product
    post:
      summary: Adds a new serial to the system
      description: Adds a new serial to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogidserials-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: serial
        description: A Json or XML object containing the new serial
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Serial
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/Serials/{serialid}:
    put:
      summary: Updates a specific serial from a specific Product
      description: Updates a specific serial from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidserialsserialid-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: serial
        description: A Json or XML object containing the new features
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: serialid
        description: FeatureID
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Serial
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/skuinfo:
    get:
      summary: Get all products (SKUInfo section only)
      description: Get all products (skuinfo section only).
      operationId: Products_GetAllProductsSKUInfo
      x-api-path-slug: 3dcartwebapiv1productscatalogidskuinfo-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: name
        description: Name of the product
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: sku
        description: SKU Code of the product
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Products
      - (SKUInfo
      - Section
      - Only)
  /3dCartWebAPI/v1/Products/{catalogid}/UpSelling:
    get:
      summary: Get the upselling products from a specific Product
      description: Get the upselling products from a specific product.
      operationId: Products_GetAllProductUpSelling
      x-api-path-slug: 3dcartwebapiv1productscatalogidupselling-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Upselling
      - Products
      - From
      - Specific
      - Product
    put:
      summary: Updates a collection of upselling items from a specific Product
      description: Updates a collection of upselling items from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidupselling-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: upsellingitems
        description: A Json or XML object containing the new upselling items
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Upselling
      - Items
      - From
      - Specific
      - Product
    post:
      summary: Adds a new upselling item to the system
      description: Adds a new upselling item to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogidupselling-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: upsellingitem
        description: A Json or XML object containing the new upselling item
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Upselling
      - Item
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/UpSelling/{upsellingindexid}:
    put:
      summary: Updates a specific Upselling Item from a specific Product
      description: Updates a specific upselling item from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidupsellingupsellingindexid-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: path
        name: upsellingindexid
        description: UpSellingIndexID
      - in: body
        name: upsellingitem
        description: A Json or XML object containing the new upselling tem
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Upselling
      - Item
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/skuinfo:
    get:
      summary: Get all products (SKUInfo section only)
      description: Get all products (skuinfo section only).
      operationId: Products_GetAllProductsSKUInfo
      x-api-path-slug: 3dcartwebapiv1productsskuinfo-get
      parameters:
      - in: query
        name: catalogid
        description: Catalog ID
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: name
        description: Name of the product
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: sku
        description: SKU Code of the product
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Products
      - (SKUInfo
      - Section
      - Only)
  /3dCartWebAPI/v1/RMA:
    get:
      summary: Get all RMAs
      description: Get all rmas.
      operationId: RMA_GetAllRMAs
      x-api-path-slug: 3dcartwebapiv1rma-get
      parameters:
      - in: query
        name: catalogid
        description: CatalogID
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: dateend
        description: Date End (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: datestart
        description: Date Start (mm/dd/yyyy hh:mm:ss)
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: query
        name: rmamethodid
        description: Method of the RMA
      - in: query
        name: rmareasonid
        description: Reason of the RMA
      - in: query
        name: rmastatusid
        description: Status of the RMA
      - in: header
        name: SecureURL
        description: SecureURL
      - in: query
        name: sku
        description: SKU Code of the product
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - RMAs
  /3dCartWebAPI/v1/RMA/{rmaid}:
    get:
      summary: Get a specific RMA
      description: Get a specific rma.
      operationId: RMA_GetRMA
      x-api-path-slug: 3dcartwebapiv1rmarmaid-get
      parameters:
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: path
        name: rmaid
        description: RMA ID
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Specific
      - RMA
  /3dCartWebAPI/v1/RMA/{rmaid}/Items:
    get:
      summary: Gets the items from a specific RMA
      description: Gets the items from a specific rma.
      operationId: RMA_GetAllRMAItem
      x-api-path-slug: 3dcartwebapiv1rmarmaiditems-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: path
        name: rmaid
        description: Order ID
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Items
      - From
      - Specific
      - RMA
  /3dCartWebAPI/v1/StoreSettings:
    get:
      summary: Get the Store Settings
      description: Get the store settings.
      operationId: StoreSettings_GetStoreSettings
      x-api-path-slug: 3dcartwebapiv1storesettings-get
      parameters:
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Store
      - Settings
    put:
      summary: This method is used to update the Store Settings in the database.
      description: This method is used to update the store settings in the database..
      operationId: StoreSettings_UpdateStoreSettings
      x-api-path-slug: 3dcartwebapiv1storesettings-put
      parameters:
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: settings
        description: A Json or XML object containing the Store Settings
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Store
      - Settings
      - In
      - Database