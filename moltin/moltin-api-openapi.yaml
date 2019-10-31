swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/customers/{customerID}/addresses/{addressID}:
    get:
      summary: Get an Address
      description: Get an address.
      operationId: V2CustomersAddressesByCustomerIDAndAddressIDGet
      x-api-path-slug: v2customerscustomeridaddressesaddressid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: addressID
      - in: header
        name: Content-Type
      - in: path
        name: customerID
      responses:
        200:
          description: Successful response
      tags:
      - Addresses
    put:
      summary: Update an Address
      description: Update an address.
      operationId: V2CustomersAddressesByCustomerIDAndAddressIDPut
      x-api-path-slug: v2customerscustomeridaddressesaddressid-put
      parameters:
      - in: header
        name: Accept
      - in: path
        name: addressID
      - in: header
        name: Content-Type
      - in: path
        name: customerID
      responses:
        200:
          description: Successful response
      tags:
      - Addresses
    delete:
      summary: Delete an Address
      description: Delete an address.
      operationId: V2CustomersAddressesByCustomerIDAndAddressIDDelete
      x-api-path-slug: v2customerscustomeridaddressesaddressid-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: addressID
      - in: header
        name: Content-Type
      - in: path
        name: customerID
      responses:
        200:
          description: Successful response
      tags:
      - Addresses
  /v2/promotions/{promotionID}/codes:
    get:
      summary: Get a list of promotion codes
      description: Get a list of promotion codes.
      operationId: V2PromotionsCodesByPromotionIDGet
      x-api-path-slug: v2promotionspromotionidcodes-get
      parameters:
      - in: header
        name: Content-Type
      - in: path
        name: promotionID
      responses:
        200:
          description: Successful response
      tags:
      - Promotion
      - Codes
    post:
      summary: Create promotion codes
      description: Create promotion codes.
      operationId: V2PromotionsCodesByPromotionIDPost
      x-api-path-slug: v2promotionspromotionidcodes-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: promotionID
      responses:
        200:
          description: Successful response
      tags:
      - Promotion
      - Codes
  /v2/customers/{customerID}/addresses:
    get:
      summary: Get an list of Addresses
      description: Get an list of addresses.
      operationId: V2CustomersAddressesByCustomerIDGet2
      x-api-path-slug: v2customerscustomeridaddresses-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: customerID
      responses:
        200:
          description: Successful response
      tags:
      - Addresseses
    post:
      summary: Create an Address
      description: Create an address.
      operationId: V2CustomersAddressesByCustomerIDPost
      x-api-path-slug: v2customerscustomeridaddresses-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
        description: Change default locale
      - in: path
        name: customerID
      - in: header
        name: X-Moltin-Customer-Token
        description: Change from default currency
      responses:
        200:
          description: Successful response
      tags:
      - Addresses
  /v2/integrations/{integrationID}:
    get:
      summary: Get an Integration
      description: Get an integration.
      operationId: V2IntegrationsByIntegrationIDGet
      x-api-path-slug: v2integrationsintegrationid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: integrationID
      responses:
        200:
          description: Successful response
      tags:
      - Integration
    put:
      summary: Update an Integration
      description: Update an integration.
      operationId: V2IntegrationsByIntegrationIDPut
      x-api-path-slug: v2integrationsintegrationid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: integrationID
      responses:
        200:
          description: Successful response
      tags:
      - Integration
    delete:
      summary: Delete an Integration
      description: Delete an integration.
      operationId: V2IntegrationsByIntegrationIDDelete
      x-api-path-slug: v2integrationsintegrationid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: integrationID
      responses:
        200:
          description: Successful response
      tags:
      - Integration
  /v2/brands/{brandID}:
    get:
      summary: Get a Brand
      description: Get a brand.
      operationId: V2BrandsByBrandIDGet
      x-api-path-slug: v2brandsbrandid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      - in: query
        name: include
      responses:
        200:
          description: Successful response
      tags:
      - Brands
    put:
      summary: Update a Brand
      description: Update a brand.
      operationId: V2BrandsByBrandIDPut
      x-api-path-slug: v2brandsbrandid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
    delete:
      summary: Delete a Brand
      description: Delete a brand.
      operationId: V2BrandsByBrandIDDelete
      x-api-path-slug: v2brandsbrandid-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
  /v2/flows:
    get:
      summary: Get all flows
      description: Get all flows.
      operationId: V2FlowsGet2
      x-api-path-slug: v2flows-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Flows
    post:
      summary: Create a flow
      description: Create a flow.
      operationId: V2FlowsPost
      x-api-path-slug: v2flows-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Flow
  /v2/customers/{customerID}:
    get:
      summary: Get a Customer
      description: Get a customer.
      operationId: V2CustomersByCustomerIDGet
      x-api-path-slug: v2customerscustomerid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: customerID
      - in: header
        name: X-Moltin-Customer-Token
        description: A customer token
      responses:
        200:
          description: Successful response
      tags:
      - Customer
    put:
      summary: Update a Customer
      description: Update a customer.
      operationId: V2CustomersByCustomerIDPut
      x-api-path-slug: v2customerscustomerid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: customerID
      - in: header
        name: X-Moltin-Customer-Token
      responses:
        200:
          description: Successful response
      tags:
      - Customer
    delete:
      summary: Delete a Customer
      description: Deletes a customer.
      operationId: V2CustomersByCustomerIDDelete
      x-api-path-slug: v2customerscustomerid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: customerID
      - in: header
        name: X-Moltin-Customer-Token
      responses:
        200:
          description: Successful response
      tags:
      - Customer
  /v2/flows/{flowSlug}/entries/{entryID}:
    get:
      summary: Get an entry
      description: Get an entry.
      operationId: V2FlowsEntriesByFlowSlugAndEntryIDGet
      x-api-path-slug: v2flowsflowslugentriesentryid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: entryID
      - in: path
        name: flowSlug
      responses:
        200:
          description: Successful response
      tags:
      - Entry
    put:
      summary: Update an entry
      description: Update an entry.
      operationId: V2FlowsEntriesByFlowSlugAndEntryIDPut
      x-api-path-slug: v2flowsflowslugentriesentryid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: entryID
      - in: path
        name: flowSlug
      responses:
        200:
          description: Successful response
      tags:
      - Entry
    delete:
      summary: Delete an entry
      description: Delete an entry.
      operationId: V2FlowsEntriesByFlowSlugAndEntryIDDelete
      x-api-path-slug: v2flowsflowslugentriesentryid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: entryID
      - in: path
        name: flowSlug
      responses:
        200:
          description: Successful response
      tags:
      - Entry
  /v2/orders/{orderID}:
    get:
      summary: Get a single order
      description: Get a single order.
      operationId: V2OrdersByOrderIDGet
      x-api-path-slug: v2ordersorderid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: orderID
      responses:
        200:
          description: Successful response
      tags:
      - Single
      - Order
    put:
      summary: Update an order
      description: |-
        Transactions are created and updated automatically whenever you make a payment request. When a payment is successful, the transaction ID returned from the gateway will be attached to the transaction.

        It is possible for an order to have more than one transaction attached as each attempted payment will be created as a new transaction.
      operationId: V2OrdersByOrderIDPut
      x-api-path-slug: v2ordersorderid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: orderID
      responses:
        200:
          description: Successful response
      tags:
      - Order
  /v2/products/{productID}/relationships/variations:
    put:
      summary: Update Product <=> Variations Relationships
      description: '`Product Variation`''s specified in the payload willbe related
        to the `Product` any relatiosnhips to `Product Variation`''s **NOT** specified
        in payload will be removed.'
      operationId: V2ProductsRelationshipsVariationsByProductIDPut
      x-api-path-slug: v2productsproductidrelationshipsvariations-put
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variations
      - Relationships
    post:
      summary: Create Product <=> Variations Relationships
      description: Here you can add and remove `Product Variation`'s to a product.
        `Product Variation`'s specified in the payload willbe related to the product.
      operationId: V2ProductsRelationshipsVariationsByProductIDPost
      x-api-path-slug: v2productsproductidrelationshipsvariations-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variations
      - Relationships
    delete:
      summary: Delete Product <=> Variations Relationships
      description: Here you can add and remove `Product Variation`'s to a product.
        Only relationships to `Product Variation`'s specified in the payload will
        be removed.
      operationId: V2ProductsRelationshipsVariationsByProductIDDelete
      x-api-path-slug: v2productsproductidrelationshipsvariations-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variations
      - Relationships
  /v2/brands/{brandID}/relationships/parent:
    put:
      summary: Update Parent Brand Relationship
      description: Update parent brand relationship.
      operationId: V2BrandsRelationshipsParentByBrandIDPut
      x-api-path-slug: v2brandsbrandidrelationshipsparent-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Brands
      - Relationship
    post:
      summary: Create Parent Brand Relationship
      description: Create parent brand relationship.
      operationId: V2BrandsRelationshipsParentByBrandIDPost
      x-api-path-slug: v2brandsbrandidrelationshipsparent-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Brands
      - Relationship
    delete:
      summary: Delete Parent Brand Relationship
      description: Delete parent brand relationship.
      operationId: V2BrandsRelationshipsParentByBrandIDDelete
      x-api-path-slug: v2brandsbrandidrelationshipsparent-delete
      parameters:
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Brands
      - Relationship
  /v2/promotions/{promotionID}:
    get:
      summary: Get a promotion
      description: Get a promotion.
      operationId: V2PromotionsByPromotionIDGet
      x-api-path-slug: v2promotionspromotionid-get
      parameters:
      - in: header
        name: Content-Type
      - in: path
        name: promotionID
      responses:
        200:
          description: Successful response
      tags:
      - Promotion
    put:
      summary: Update promotion
      description: Update promotion.
      operationId: V2PromotionsByPromotionIDPut
      x-api-path-slug: v2promotionspromotionid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: promotionID
      responses:
        200:
          description: Successful response
      tags:
      - Promotion
    delete:
      summary: Delete Promotion
      description: Delete promotion.
      operationId: V2PromotionsByPromotionIDDelete
      x-api-path-slug: v2promotionspromotionid-delete
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: promotionID
      responses:
        200:
          description: Successful response
      tags:
      - Promotion
  '/v2/carts/{CART_REFERENCE} ':
    delete:
      summary: Delete Cart
      description: |-
        Update an existing item in a cart. The updated cart contents are returned if the call is successful.

        **Note:** `{item_id}` in the path is the identifier for the item in the cart **OR** productID.

        When updating custom itesm you must use the identifier in the cart - you can update more properties of a custom cart item.
      operationId: V2CartsByCARTREFERENCEDelete
      x-api-path-slug: v2cartscart-reference-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: CART_REFERENCE
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Cart
  /v2/settings:
    get:
      summary: Get Settings Attributes
      description: Get settings attributes.
      operationId: V2SettingsGet2
      x-api-path-slug: v2settings-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Settings
      - Attributes
    put:
      summary: Update Settings
      description: Update settings.
      operationId: V2SettingsPut
      x-api-path-slug: v2settings-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Settings
  /v2/categories/{categoryID}:
    get:
      summary: Get a Category
      description: Get a category.
      operationId: V2CategoriesByCategoryIDGet
      x-api-path-slug: v2categoriescategoryid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category
    put:
      summary: Update a Category
      description: Update a category.
      operationId: V2CategoriesByCategoryIDPut
      x-api-path-slug: v2categoriescategoryid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category
    delete:
      summary: Delete a Category
      description: Delete a category.
      operationId: V2CategoriesByCategoryIDDelete
      x-api-path-slug: v2categoriescategoryid-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category
  /v2/carts/123456/items:
    get:
      summary: Get the items in a cart
      description: Get the items in a cart.
      operationId: V2Carts123456ItemsGet
      x-api-path-slug: v2carts123456items-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Items
      - Cart
    post:
      summary: Add a promotion to a cart
      description: |-
        Update an existing item in a cart. The updated cart contents are returned if the call is successful.

        **Note:** `{item_id}` in the path is the identifier for the item in the cart **OR** productID.

        When updating custom itesm you must use the identifier in the cart - you can update more properties of a custom cart item.
      operationId: V2Carts123456ItemsPost2
      x-api-path-slug: v2carts123456items-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Promotion
      - To
      - Cart
  /v2/products/{productID}/relationships/files:
    put:
      summary: Update Products <=> Files Relationships
      description: '`File`''s specified in the payload willbe related to the product
        any relatiosnhips to `File`''s **NOT** specified in payload will be removed.'
      operationId: V2ProductsRelationshipsFilesByProductIDPut
      x-api-path-slug: v2productsproductidrelationshipsfiles-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Files
      - Relationships
    post:
      summary: Create Products <=> Files Relationships
      description: Here you can add `File`'s to a product. `File`'s specified in the
        payload willbe related to the product.
      operationId: V2ProductsRelationshipsFilesByProductIDPost
      x-api-path-slug: v2productsproductidrelationshipsfiles-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Files
      - Relationships
    delete:
      summary: Delete Products <=> Files Relationship
      description: Here you can delete a relationship between a `Product` and `File`'s.
        Only relationships to `File`'s specified in the payload will be removed.
      operationId: V2ProductsRelationshipsFilesByProductIDDelete
      x-api-path-slug: v2productsproductidrelationshipsfiles-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Files
      - Relationship
  /v2/integrations/attributes:
    get:
      summary: Get Integration Attributes
      description: Get integration attributes.
      operationId: V2IntegrationsAttributesGet
      x-api-path-slug: v2integrationsattributes-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Integration
      - Attributes
  /v2/gateways/braintree:
    put:
      summary: Braintree - Update
      description: This endpoint allows you to pay for an order using Braintree and
        a users credit card.
      operationId: V2GatewaysBraintreePut
      x-api-path-slug: v2gatewaysbraintree-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Braintree
      - '-'
  /v2/collections/{collectionID}/relationships/collections:
    post:
      summary: Create Collection Relationships
      description: Create collection relationships.
      operationId: V2CollectionsRelationshipsCollectionsByCollectionIDPost
      x-api-path-slug: v2collectionscollectionidrelationshipscollections-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Collection
      - Relationships
  /v2/integrations/{integrationID}/logs:
    get:
      summary: Get Logs for an Integration
      description: Get logs for an integration.
      operationId: V2IntegrationsLogsByIntegrationIDGet
      x-api-path-slug: v2integrationsintegrationidlogs-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: integrationID
      responses:
        200:
          description: Successful response
      tags:
      - Logsan
      - Integration
  /v2/categories/{categoryID}/relationships/children:
    put:
      summary: Update Child Category Relationships
      description: Update child category relationships.
      operationId: V2CategoriesRelationshipsChildrenByCategoryIDPut
      x-api-path-slug: v2categoriescategoryidrelationshipschildren-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Category
      - Relationships
    delete:
      summary: Delete Child Category Relationships
      description: Delete child category relationships.
      operationId: V2CategoriesRelationshipsChildrenByCategoryIDDelete
      x-api-path-slug: v2categoriescategoryidrelationshipschildren-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Category
      - Relationships
  /v2/collections:
    get:
      summary: Get Collections List
      description: Get collections list.
      operationId: V2CollectionsGet
      x-api-path-slug: v2collections-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Collections
      - List
    post:
      summary: Create a Collection
      description: Create a collection.
      operationId: V2CollectionsPost
      x-api-path-slug: v2collections-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Collection
  /categories/{categoryID}/relationships/children:
    post:
      summary: Create Child Category Relationships
      description: Create child category relationships.
      operationId: CategoriesRelationshipsChildrenByCategoryIDPost
      x-api-path-slug: categoriescategoryidrelationshipschildren-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Category
      - Relationships
  /v2/carts/123456:
    get:
      summary: Get a Cart
      description: Get a cart.
      operationId: V2Carts123456Get
      x-api-path-slug: v2carts123456-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Cart
  /v2/collections/{collectionID}:
    get:
      summary: Get a Collection
      description: Get a collection.
      operationId: V2CollectionsByCollectionIDGet
      x-api-path-slug: v2collectionscollectionid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      - in: query
        name: filter
      - in: query
        name: include
      - in: query
        name: page[limit]
      - in: query
        name: page[offset]
      - in: query
        name: sort
      responses:
        200:
          description: Successful response
      tags:
      - Collection
    put:
      summary: Update a Collection
      description: Update a collection.
      operationId: V2CollectionsByCollectionIDPut
      x-api-path-slug: v2collectionscollectionid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Collection
    delete:
      summary: Delete a Collection
      description: Delete a collection.
      operationId: V2CollectionsByCollectionIDDelete
      x-api-path-slug: v2collectionscollectionid-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Collection
  '/v2/inventories ':
    get:
      summary: Get all stock
      description: Get all stock.
      operationId: V2InventoriesGet
      x-api-path-slug: v2inventories-get
      responses:
        200:
          description: Successful response
      tags:
      - Stock
  /v2/flows/{flowID}:
    get:
      summary: Get a flow
      description: Get a flow.
      operationId: V2FlowsByFlowIDGet
      x-api-path-slug: v2flowsflowid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: flowID
      responses:
        200:
          description: Successful response
      tags:
      - Flow
    put:
      summary: Update a flow
      description: Update a flow.
      operationId: V2FlowsByFlowIDPut
      x-api-path-slug: v2flowsflowid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: flowID
      responses:
        200:
          description: Successful response
      tags:
      - Flow
    delete:
      summary: Delete a flow
      description: Delete a flow.
      operationId: V2FlowsByFlowIDDelete
      x-api-path-slug: v2flowsflowid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: flowID
      responses:
        200:
          description: Successful response
      tags:
      - Flow
  /v2/gateways/adyen:
    put:
      summary: Adyen - Card Update
      description: This endpoint allows you to pay for an order using Braintree and
        a users credit card.
      operationId: V2GatewaysAdyenPut
      x-api-path-slug: v2gatewaysadyen-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Adyen
      - '-'
      - Card
  /v2/carts/123456/items/{itemID}:
    put:
      summary: Update an item in a cart
      description: |-
        Update an existing item in a cart. The updated cart contents are returned if the call is successful.

        **Note:** `{item_id}` in the path is the identifier for the item in the cart **OR** productID.

        When updating custom itesm you must use the identifier in the cart - you can update more properties of a custom cart item.
      operationId: V2Carts123456ItemsByItemIDPut
      x-api-path-slug: v2carts123456itemsitemid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: itemID
      responses:
        200:
          description: Successful response
      tags:
      - Item
      - Cart
  /v2/flows/{flowSlug}/entries/{ENTRY_ID}/relationships/{flowSlug}:
    put:
      summary: Update Entry Relationship(s)
      description: Update entry relationship(s).
      operationId: V2FlowsEntriesRelationshipsFlowSlugByFlowSlugAndENTRYIDPut
      x-api-path-slug: v2flowsflowslugentriesentry-idrelationshipsflowslug-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: ENTRY_ID
      - in: path
        name: flowSlug
      responses:
        200:
          description: Successful response
      tags:
      - Entry
      - Relationship(s)
    delete:
      summary: Delete Entry Relationship(s)
      description: Delete entry relationship(s).
      operationId: V2FlowsEntriesRelationshipsFlowSlugByFlowSlugAndENTRYIDDelete
      x-api-path-slug: v2flowsflowslugentriesentry-idrelationshipsflowslug-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: ENTRY_ID
      - in: path
        name: flowSlug
      responses:
        200:
          description: Successful response
      tags:
      - Entry
      - Relationship(s)
  /v2/inventories/{productID}/transactions:
    get:
      summary: Stock transactions for a product
      description: Stock transactions for a product.
      operationId: V2InventoriesTransactionsByProductIDGet
      x-api-path-slug: v2inventoriesproductidtransactions-get
      parameters:
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Stock
      - Transactionsa
      - Products
    post:
      summary: Create a stock transaction for a product
      description: Create a stock transaction for a product.
      operationId: V2InventoriesTransactionsByProductIDPost
      x-api-path-slug: v2inventoriesproductidtransactions-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Stock
      - Transactiona
      - Products
  /v2/products/{productID}:
    get:
      summary: Get a Product
      description: Get a product.
      operationId: V2ProductsByProductIDGet
      x-api-path-slug: v2productsproductid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
    put:
      summary: Update a Product
      description: Update a product.
      operationId: V2ProductsByProductIDPut
      x-api-path-slug: v2productsproductid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
    delete:
      summary: Delete a Product
      description: Delete a product.
      operationId: V2ProductsByProductIDDelete
      x-api-path-slug: v2productsproductid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
  /v2/products/{productID}/relationships/brands:
    put:
      summary: Update Product <=> Brands Relationships
      description: Here you can set relations `Brand`'s to a product. The result of
        this request will set relationships between product and the specified brnads
        in teh payload and remove any other relations the product had with brands.
      operationId: V2ProductsRelationshipsBrandsByProductIDPut
      x-api-path-slug: v2productsproductidrelationshipsbrands-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Brandss
      - Relationships
    post:
      summary: Create Product <=> Brands Relationships
      description: Here you can add `Brand`'s to a product. The `Brand`'s found in
        the payload will be added to any other relationships to `Brand`'s present.
      operationId: V2ProductsRelationshipsBrandsByProductIDPost
      x-api-path-slug: v2productsproductidrelationshipsbrands-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Brandss
      - Relationships
    delete:
      summary: Delete Products <=> Brands Relationships
      description: Here you can delete a relationship between a `Product` and `Brand`'s.
        Only those relationshops to `Brand`'s specified in the paylaod will be removed.
      operationId: V2ProductsRelationshipsBrandsByProductIDDelete2
      x-api-path-slug: v2productsproductidrelationshipsbrands-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Brands
      - Relationships
  /v2/files/{fileID}:
    get:
      summary: Get a file
      description: Get a file.
      operationId: V2FilesByFileIDGet
      x-api-path-slug: v2filesfileid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: fileID
      responses:
        200:
          description: Successful response
      tags:
      - File
    delete:
      summary: Delete a file
      description: Delete a file.
      operationId: V2FilesByFileIDDelete
      x-api-path-slug: v2filesfileid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: fileID
      responses:
        200:
          description: Successful response
      tags:
      - File
  /v2/fields:
    get:
      summary: Get a field list
      description: Get a field list.
      operationId: V2FieldsGet
      x-api-path-slug: v2fields-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Field
      - List
    post:
      summary: Create a field
      description: Create a field.
      operationId: V2FieldsPost
      x-api-path-slug: v2fields-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Field
  /v2/brands/{brandID}/relationships/children:
    put:
      summary: Update Child Brand Relationship
      description: Update child brand relationship.
      operationId: V2BrandsRelationshipsChildrenByBrandIDPut
      x-api-path-slug: v2brandsbrandidrelationshipschildren-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Brands
      - Relationship
    post:
      summary: Create Child Brand Relationship
      description: Create child brand relationship.
      operationId: V2BrandsRelationshipsChildrenByBrandIDPost
      x-api-path-slug: v2brandsbrandidrelationshipschildren-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Brands
      - Relationship
    delete:
      summary: Update Child Brand Relationship Copy
      description: Update child brand relationship copy.
      operationId: V2BrandsRelationshipsChildrenByBrandIDDelete
      x-api-path-slug: v2brandsbrandidrelationshipschildren-delete
      parameters:
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Brands
      - Relationship
      - Copy
  /v2/collections/{collectionID}/relationships/parent:
    put:
      summary: Update Parent Collection Relationship
      description: Update parent collection relationship.
      operationId: V2CollectionsRelationshipsParentByCollectionIDPut
      x-api-path-slug: v2collectionscollectionidrelationshipsparent-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Collection
      - Relationship
    post:
      summary: Create Parent Collection Relationship
      description: Create parent collection relationship.
      operationId: V2CollectionsRelationshipsParentByCollectionIDPost
      x-api-path-slug: v2collectionscollectionidrelationshipsparent-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Collection
      - Relationship
    delete:
      summary: Delete Parent Collection Relationship
      description: Delete parent collection relationship.
      operationId: V2CollectionsRelationshipsParentByCollectionIDDelete
      x-api-path-slug: v2collectionscollectionidrelationshipsparent-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Collection
      - Relationship
  /v2/variations/{variationID}:
    get:
      summary: Get a Product Variation
      description: Get a product variation.
      operationId: V2VariationsByVariationIDGet
      x-api-path-slug: v2variationsvariationid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: variationID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variation
    put:
      summary: Update a Product Variation
      description: Update a product variation.
      operationId: V2VariationsByVariationIDPut
      x-api-path-slug: v2variationsvariationid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: variationID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variation
    delete:
      summary: Delete a Product Variation
      description: Delete a product variation.
      operationId: V2VariationsByVariationIDDelete
      x-api-path-slug: v2variationsvariationid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: variationID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variation
  /v2/customers:
    get:
      summary: Get Customers List
      description: Get customers list.
      operationId: V2CustomersGet
      x-api-path-slug: v2customers-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: filter
      - in: query
        name: page[limit]
      - in: query
        name: page[offset]
      - in: query
        name: sort
      responses:
        200:
          description: Successful response
      tags:
      - Customers
      - List
    post:
      summary: Create a Customer
      description: Create a customer.
      operationId: V2CustomersPost
      x-api-path-slug: v2customers-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Customer
  /v2/products/{productID}/build:
    post:
      summary: Build Child Products
      description: Build child products.
      operationId: V2ProductsBuildByProductIDPost
      x-api-path-slug: v2productsproductidbuild-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Build
      - Child
      - Products
  /oauth/access_token:
    post:
      summary: Client credential token
      description: |-
        An access token will allow you to make requests for your store. We support two types of token: `client_credentials` and `implicit`.

        An `implcit` token is typically used for situations where you are requesting data on the client side and you are exposing your public key - such as JavaScript - and adding your client secret would be disastrous. You will only be able to perform a limited number of operations on the API endpoints.

        A `client_credentials` token is used when the credentials are not publicly exposed, usually a server side language such as PHP. You will be able to perform all operations on API endpoints.

        A `refresh_token` type can be used when you have an existing token which you would like to extend the life of. When your `grant_type` is `refresh_token` you must also provide the original token in the `refresh_token` field.
      operationId: OauthAccessTokenPost2
      x-api-path-slug: oauthaccess-token-post
      parameters:
      - in: header
        name: Accept
      - in: formData
        name: client_id
        description: Replace with the values from your dashboard
      - in: formData
        name: client_secret
        description: Replace with the values from your dashboard
      - in: header
        name: Content-Type
      - in: formData
        name: grant_type
        description: client_credentials | implicit | refresh_token
      responses:
        200:
          description: Successful response
      tags:
      - Client
      - Credential
      - Token
  /v2/collections/tree:
    get:
      summary: Get Collection tree
      description: Get collection tree.
      operationId: V2CollectionsTreeGet
      x-api-path-slug: v2collectionstree-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Collection
      - Tree
  /v2/products/{ProductID}relationships/brands:
    post:
      summary: Create Products <=> Main Image Relationships
      description: |-
        Here you can add a `Main Image` to a product. The `Main Image` will be a file and that file will be shown as the first image for the product it is related to.

        It's worth noting that you can only have 1 main image so unlike other relationships, you will be passing an object instead of an array in the body.

        In the Object, the type will be `main_image` and the ID will be the ID of the file you wish to make the main image for that product.
      operationId: V2ProductsRelationshipsBrandsByProductIDPost2
      x-api-path-slug: v2productsproductidrelationshipsbrands-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: ProductID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Main
      - Image
      - Relationships
    delete:
      summary: Delete Products <=> Main Image Relationships
      description: |-
        Here you can delete the `Main Image` from a product.

        In the Object payload, the type will be `main_image` and the ID will be the ID of the main image you wish to delete from that product.
      operationId: V2ProductsRelationshipsBrandsByProductIDDelete
      x-api-path-slug: v2productsproductidrelationshipsbrands-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: ProductID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Main
      - Image
      - Relationships
  /v2/flows/{flowSlug}/entries:
    get:
      summary: Get all entries on a flow
      description: Get all entries on a flow.
      operationId: V2FlowsEntriesByFlowSlugGet
      x-api-path-slug: v2flowsflowslugentries-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: flowSlug
      responses:
        200:
          description: Successful response
      tags:
      - Entries
      - "On"
      - Flow
    post:
      summary: Create an entry
      description: Create an entry.
      operationId: V2FlowsEntriesByFlowSlugPost
      x-api-path-slug: v2flowsflowslugentries-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: flowSlug
      responses:
        200:
          description: Successful response
      tags:
      - Entry
  /v2/fields/{fieldID}:
    get:
      summary: Get a field
      description: Get a field.
      operationId: V2FieldsByFieldIDGet
      x-api-path-slug: v2fieldsfieldid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: fieldID
      responses:
        200:
          description: Successful response
      tags:
      - Field
    put:
      summary: Update a field
      description: Update a field.
      operationId: V2FieldsByFieldIDPut
      x-api-path-slug: v2fieldsfieldid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: fieldID
      responses:
        200:
          description: Successful response
      tags:
      - Field
    delete:
      summary: Delete a field
      description: Delete a field.
      operationId: V2FieldsByFieldIDDelete
      x-api-path-slug: v2fieldsfieldid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: fieldID
      responses:
        200:
          description: Successful response
      tags:
      - Field
  /v2/carts/123456/checkout:
    post:
      summary: Checkout using customer id
      description: |-
        Converts a cart to an incomplete order. The original cart will remain and can be modified and checked out again if required.

        The new order will be returned and `data.meta.payment_gateways` will contain an array of the available payment gateways for this order.
      operationId: V2Carts123456CheckoutPost2
      x-api-path-slug: v2carts123456checkout-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Checkout
      - Using
      - Customer
      - Id
  /v2/products/{productID}/relationships/categories:
    put:
      summary: Update Product <=> Categories Relationships
      description: Here you can update `Categories` to a product. `Categories` specified
        in the payload willbe related to the product any relatiosnhips to `Categories`
        **NOT** specified in payload will be removed.
      operationId: V2ProductsRelationshipsCategoriesByProductIDPut
      x-api-path-slug: v2productsproductidrelationshipscategories-put
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Categories
      - Relationships
    post:
      summary: Create Product <=> Categories Relationships
      description: Here you can add `Categories` to a product. `Categories` specified
        in the payload willbe related to the product.
      operationId: V2ProductsRelationshipsCategoriesByProductIDPost
      x-api-path-slug: v2productsproductidrelationshipscategories-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Categories
      - Relationships
    delete:
      summary: Delete Product <=> Categories Relationships
      description: Here you can delete a relationship between a `Product` and `Category`.
        Only relationships to `Categories` specified in the payload will be removed.
      operationId: V2ProductsRelationshipsCategoriesByProductIDDelete
      x-api-path-slug: v2productsproductidrelationshipscategories-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Categories
      - Relationships
  /v2/variations:
    get:
      summary: Get Product Variations List
      description: Get product variations list.
      operationId: V2VariationsGet
      x-api-path-slug: v2variations-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variations
      - List
    post:
      summary: Create a Product Variation
      description: Create a product variation.
      operationId: V2VariationsPost
      x-api-path-slug: v2variations-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variation
  /v2/brands/tree:
    get:
      summary: Get a Brand tree
      description: Get a brand tree.
      operationId: V2BrandsTreeGet
      x-api-path-slug: v2brandstree-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
      - Tree
  /v2/flows/{flowSlug}/fields:
    get:
      summary: Get all fields on a flow
      description: Get all fields on a flow.
      operationId: V2FlowsFieldsByFlowSlugGet
      x-api-path-slug: v2flowsflowslugfields-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: flowSlug
      responses:
        200:
          description: Successful response
      tags:
      - Fields
      - "On"
      - Flow
  /v2/currencies:
    get:
      summary: Get Currencies List
      description: Get currencies list.
      operationId: V2CurrenciesGet
      x-api-path-slug: v2currencies-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Currencies
      - List
    post:
      summary: Create a Currency
      description: Create a currency.
      operationId: V2CurrenciesPost
      x-api-path-slug: v2currencies-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Currency
  /v2/products/{productID}/relationships/collections:
    put:
      summary: Update Products <=> Collections Relationships
      description: '`Collection`''s specified in the payload willbe related to the
        product any relatiosnhips to `Collection`''s **NOT** specified in payload
        will be removed.'
      operationId: V2ProductsRelationshipsCollectionsByProductIDPut
      x-api-path-slug: v2productsproductidrelationshipscollections-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Collections
      - Relationships
    post:
      summary: Create Products <=> Collections Relationships
      description: Here you can add `Collection`'s to a product. `Collection`'s specified
        in the payload willbe related to the product.
      operationId: V2ProductsRelationshipsCollectionsByProductIDPost
      x-api-path-slug: v2productsproductidrelationshipscollections-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Collections
      - Relationships
    delete:
      summary: Delete Products <=> Collections Relationships
      description: Here you can delete a relationship between a `Product` and `Collections`.
        Only relationships to `Collections` specified in the payload will be removed.
      operationId: V2ProductsRelationshipsCollectionsByProductIDDelete
      x-api-path-slug: v2productsproductidrelationshipscollections-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Collections
      - Relationships
  /v2/currencies/{currencyID}:
    get:
      summary: Get a Currency
      description: Get a currency.
      operationId: V2CurrenciesByCurrencyIDGet
      x-api-path-slug: v2currenciescurrencyid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: currencyID
      responses:
        200:
          description: Successful response
      tags:
      - Currency
    put:
      summary: Update a Currency
      description: Update a currency.
      operationId: V2CurrenciesByCurrencyIDPut
      x-api-path-slug: v2currenciescurrencyid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: currencyID
      responses:
        200:
          description: Successful response
      tags:
      - Currency
    delete:
      summary: Delete a Currency
      description: Delete a currency.
      operationId: V2CurrenciesByCurrencyIDDelete
      x-api-path-slug: v2currenciescurrencyid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: currencyID
      responses:
        200:
          description: Successful response
      tags:
      - Currency
  /v2/variations/{variationID}/options/{optionID}:
    put:
      summary: Update a Product Variation Option
      description: Update a product variation option.
      operationId: V2VariationsOptionsByVariationIDAndOptionIDPut
      x-api-path-slug: v2variationsvariationidoptionsoptionid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: optionID
      - in: path
        name: variationID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variation
      - Option
    delete:
      summary: Delete a Product Variation Option
      description: Delete a product variation option.
      operationId: V2VariationsOptionsByVariationIDAndOptionIDDelete
      x-api-path-slug: v2variationsvariationidoptionsoptionid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: optionID
      - in: path
        name: variationID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variation
      - Option
  /v2/categories/{parentCatID}/relationships/parent:
    put:
      summary: Update Parent Category Parent
      description: Update parent category parent.
      operationId: V2CategoriesRelationshipsParentByParentCatIDPut
      x-api-path-slug: v2categoriesparentcatidrelationshipsparent-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: parentCatID
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Category
      - Parent
  /v2/gateways:
    get:
      summary: Get a list of gateways
      description: This endpoint allows you to pay for an order using Braintree and
        a users credit card.
      operationId: V2GatewaysGet
      x-api-path-slug: v2gateways-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Gateways
  /v2/variations/{variationID}/options/{optionID}/modifiers/{modifierID}:
    put:
      summary: Update Product Modifier
      description: Update product modifier.
      operationId: V2VariationsOptionsModifiersModifierIDByVariationIDAndOptionIDPut
      x-api-path-slug: v2variationsvariationidoptionsoptionidmodifiersmodifierid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: modifierID
      - in: path
        name: optionID
      - in: path
        name: variationID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Modifier
    delete:
      summary: Delete Product Modifier
      description: Delete product modifier.
      operationId: V2VariationsOptionsModifiersModifierIDByVariationIDAndOptionIDDelete
      x-api-path-slug: v2variationsvariationidoptionsoptionidmodifiersmodifierid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: modifierID
      - in: path
        name: optionID
      - in: path
        name: variationID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Modifier
  /categories/{categoryID}/relationships/categories:
    delete:
      summary: Delete Category-Category Relationships
      description: Delete category-category relationships.
      operationId: CategoriesRelationshipsCategoriesByCategoryIDDelete
      x-api-path-slug: categoriescategoryidrelationshipscategories-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category-Category
      - Relationships
  /v2/variations/{variationID}/options/{optionID}/modifiers:
    post:
      summary: Create Product Modifier
      description: Create product modifier.
      operationId: V2VariationsOptionsModifiersByVariationIDAndOptionIDPost
      x-api-path-slug: v2variationsvariationidoptionsoptionidmodifiers-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: optionID
      - in: path
        name: variationID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Modifier
  /v2/brands/attributes:
    get:
      summary: Get Brand Attributes
      description: Get brand attributes.
      operationId: V2BrandsAttributesGet
      x-api-path-slug: v2brandsattributes-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
      - Attributes
  /v2/gateways/stripe:
    get:
      summary: Get a gateway (stripe)
      description: This endpoint allows you to pay for an order using Braintree and
        a users credit card.
      operationId: V2GatewaysStripeGet
      x-api-path-slug: v2gatewaysstripe-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Gateway
      - (stripe)
  /v2/collections/{collectionID}/relationships/children:
    put:
      summary: Update Child Collection Relationship
      description: Update child collection relationship.
      operationId: V2CollectionsRelationshipsChildrenByCollectionIDPut
      x-api-path-slug: v2collectionscollectionidrelationshipschildren-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Collection
      - Relationship
    post:
      summary: Create Child Collection Relationships
      description: Create child collection relationships.
      operationId: V2CollectionsRelationshipsChildrenByCollectionIDPost
      x-api-path-slug: v2collectionscollectionidrelationshipschildren-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Collection
      - Relationships
    delete:
      summary: Delete Child Collection Relationship
      description: Delete child collection relationship.
      operationId: V2CollectionsRelationshipsChildrenByCollectionIDDelete
      x-api-path-slug: v2collectionscollectionidrelationshipschildren-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Collection
      - Relationship
  /v2/categories/{categoryID}/relationships/categories:
    post:
      summary: Create Parent Category Relationship
      description: Using this endpoint you can create a relationship between a category
        and a parent category. When returning the category tree, you will see this
        relationship in place.
      operationId: V2CategoriesRelationshipsCategoriesByCategoryIDPost
      x-api-path-slug: v2categoriescategoryidrelationshipscategories-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Category
      - Relationship
  /v2/carts/123456/items/{cartItemID}:
    delete:
      summary: Delete an item from a cart
      description: |-
        Delete an item from a cart. The remaining cart contents are returned on a successful delete.

        **Note:** `{item_id}` in the path is the identifier for the item in the cart rather than the product_id
      operationId: V2Carts123456ItemsByCartItemIDDelete
      x-api-path-slug: v2carts123456itemscartitemid-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cartItemID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Item
      - From
      - Cart
  /orders/{orderID}/items:
    get:
      summary: Get Order Items
      description: Get order items.
      operationId: OrdersItemsByOrderIDGet
      x-api-path-slug: ordersorderiditems-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: orderID
      responses:
        200:
          description: Successful response
      tags:
      - Order
      - Items
  /v2/inventories/{productID}:
    get:
      summary: Get stock for a product
      description: Get stock for a product.
      operationId: V2InventoriesByProductIDGet
      x-api-path-slug: v2inventoriesproductid-get
      parameters:
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Stocka
      - Products
  /v2/integrations/{integrationID}/jobs:
    get:
      summary: Get all Jobs for an Integration
      description: Get all jobs for an integration.
      operationId: V2IntegrationsJobsByIntegrationIDGet
      x-api-path-slug: v2integrationsintegrationidjobs-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: integrationID
      responses:
        200:
          description: Successful response
      tags:
      - Jobsan
      - Integration
  /v2/integrations/{integrationID}/jobs/{integrationJobID}/logs:
    get:
      summary: Get Logs for a Job
      description: Get logs for a job.
      operationId: V2IntegrationsJobsLogsByIntegrationIDAndIntegrationJobIDGet
      x-api-path-slug: v2integrationsintegrationidjobsintegrationjobidlogs-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: integrationID
      - in: path
        name: integrationJobID
      responses:
        200:
          description: Successful response
      tags:
      - Logsa
      - Job
  /v2/integrations:
    get:
      summary: Get Integrations list
      description: Get integrations list.
      operationId: V2IntegrationsGet
      x-api-path-slug: v2integrations-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Integrations
      - List
    post:
      summary: Create an Integration
      description: Create an integration.
      operationId: V2IntegrationsPost
      x-api-path-slug: v2integrations-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Integration
  /v2/orders/{orderID}/transactions/{TransactionID}/capture:
    post:
      summary: Capture an authorize
      description: Capture an authorize.
      operationId: V2OrdersTransactionsCaptureByOrderIDAndTransactionIDPost
      x-api-path-slug: v2ordersorderidtransactionstransactionidcapture-post
      parameters:
      - in: header
        name: Content-Type
      - in: path
        name: orderID
      - in: path
        name: TransactionID
      responses:
        200:
          description: Successful response
      tags:
      - Capture
      - Authorize
  /categories/attributes:
    get:
      summary: Get Category Attributes
      description: Get category attributes.
      operationId: CategoriesAttributesGet
      x-api-path-slug: categoriesattributes-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category
      - Attributes
  /v2/products/attributes:
    get:
      summary: Get Product Attributes
      description: Get product attributes.
      operationId: V2ProductsAttributesGet
      x-api-path-slug: v2productsattributes-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Attributes
  /v2/orders/{ORDER_ID}/transactions/{TRANSACTION_ID}/capture:
    put:
      summary: Stripe - Card Update
      description: This endpoint allows you to pay for an order using Braintree and
        a users credit card.
      operationId: V2OrdersTransactionsCaptureByORDERIDAndTRANSACTIONIDPut
      x-api-path-slug: v2ordersorder-idtransactionstransaction-idcapture-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: ORDER_ID
      - in: path
        name: TRANSACTION_ID
      responses:
        200:
          description: Successful response
      tags:
      - Stripe
      - '-'
      - Card
  /v2/categories/{categoryID}/relationships/parent:
    delete:
      summary: Delete Parent Category Parent
      description: Delete parent category parent.
      operationId: V2CategoriesRelationshipsParentByCategoryIDDelete
      x-api-path-slug: v2categoriescategoryidrelationshipsparent-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Category
      - Parent
  /v2/files:
    get:
      summary: Get all files
      description: Get all files.
      operationId: V2FilesGet
      x-api-path-slug: v2files-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: filter
      - in: query
        name: page[limit]
      - in: query
        name: page[offset]
      - in: query
        name: sort
      responses:
        200:
          description: Successful response
      tags:
      - Files
    post:
      summary: Create a file
      description: Create a file.
      operationId: V2FilesPost
      x-api-path-slug: v2files-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - File
  /v2/categories:
    get:
      summary: Get Categories List
      description: Get categories list.
      operationId: V2CategoriesGet
      x-api-path-slug: v2categories-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Categories
      - List
    post:
      summary: Create a Category
      description: Create a category.
      operationId: V2CategoriesPost
      x-api-path-slug: v2categories-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category
  /v2/categories/categories/tree:
    get:
      summary: Category Tree
      description: Category tree.
      operationId: V2CategoriesCategoriesTreeGet
      x-api-path-slug: v2categoriescategoriestree-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category
      - Tree
  /carts/{cartRef}:
    delete:
      summary: Delete a Cart
      description: Removes all items in a cart.
      operationId: CartsByCartRefDelete
      x-api-path-slug: cartscartref-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cartRef
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Cart
  /v2/integrations/logs:
    get:
      summary: Get all Logs
      description: Get all logs.
      operationId: V2IntegrationsLogsGet
      x-api-path-slug: v2integrationslogs-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Logs
  /v2/brands:
    get:
      summary: Get a list of Brands
      description: Get a list of brands.
      operationId: V2BrandsGet
      x-api-path-slug: v2brands-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
    post:
      summary: Create a Brand
      description: Create a brand.
      operationId: V2BrandsPost
      x-api-path-slug: v2brands-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
  /v2/promotions:
    get:
      summary: Get a list of promotions
      description: Get a list of promotions.
      operationId: V2PromotionsGet
      x-api-path-slug: v2promotions-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Promotions
    post:
      summary: Create a promotion
      description: Create a promotion.
      operationId: V2PromotionsPost
      x-api-path-slug: v2promotions-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Promotion
  '/v2/customers/tokens ':
    post:
      summary: Generate a customer token
      description: Generate a customer token.
      operationId: V2CustomersTokensPost
      x-api-path-slug: v2customerstokens-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Generate
      - Customer
      - Token
  /v2/brands/{brandID}/relationships/brands:
    post:
      summary: Create Brand Relationships
      description: Create brand relationships.
      operationId: V2BrandsRelationshipsBrandsByBrandIDPost
      x-api-path-slug: v2brandsbrandidrelationshipsbrands-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
      - Relationships
  /v2/products:
    get:
      summary: Get Products List
      description: Get products list.
      operationId: V2ProductsGet
      x-api-path-slug: v2products-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: filter
      - in: query
        name: include
      - in: query
        name: page[limit]
      - in: query
        name: page[offset]
      - in: query
        name: sort
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - List
    post:
      summary: Create a new Product
      description: Create a new product.
      operationId: V2ProductsPost
      x-api-path-slug: v2products-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - New
      - Products
  /v2/flows/{flowSlug}/entries/{entryID}/relationships/{fieldSlug}:
    post:
      summary: Create Entry Relationship(s)
      description: Create entry relationship(s).
      operationId: V2FlowsEntriesRelationshipsFieldSlugByFlowSlugAndEntryIDPost
      x-api-path-slug: v2flowsflowslugentriesentryidrelationshipsfieldslug-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: entryID
      - in: path
        name: fieldSlug
      - in: path
        name: flowSlug
      responses:
        200:
          description: Successful response
      tags:
      - Entry
      - Relationship(s)
  /v2/categories/tree:
    get:
      summary: Get Categories Tree
      description: Get categories tree.
      operationId: V2CategoriesTreeGet
      x-api-path-slug: v2categoriestree-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Categories
      - Tree
  /v2/variations/{variationID}/options:
    post:
      summary: Create a Product Variation Option
      description: Create a product variation option.
      operationId: V2VariationsOptionsByVariationIDPost
      x-api-path-slug: v2variationsvariationidoptions-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: variationID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variation
      - Option
  /v2/orders:
    get:
      summary: Get all orders
      description: Get all orders.
      operationId: V2OrdersGet
      x-api-path-slug: v2orders-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Orders