swagger: "2.0"
x-collection-name: BigCommerce
x-complete: 1
info:
  title: BigCommerce API V3
  description: collection-of-requests-for-interacting-with-bigcommerces-v3-api
  version: 1.0.0
host: api.bigcommerce.com
basePath: /stores
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{store-hash}/v3/catalog/products/{id}/images:
    get:
      summary: Retrieve images for a single product
      description: GET request for retrieving images associated with a product
      operationId: V3CatalogProductsImagesByStoreHashAndIdGet
      x-api-path-slug: storehashv3catalogproductsidimages-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store-hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Imagesa
      - Single
      - Product
    post:
      summary: Upload a new product image to a single product
      description: Adds a new product image from a publicly accessible URL. May fail
        if the hosting website is forcing HTTPS connections with TLS 1.0 (as this
        has been deprecated).
      operationId: V3CatalogProductsImagesByStoreHashAndIdPost
      x-api-path-slug: storehashv3catalogproductsidimages-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store-hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Upload
      - New
      - Product
      - Image
      - To
      - Single
      - Product
  /{store-hash}/v3/catalog/products/{id}:
    get:
      summary: Retrieve a single product with expanded sub-resources
      description: Request a single product with expanded variant information
      operationId: V3CatalogProductsByStoreHashAndIdGet
      x-api-path-slug: storehashv3catalogproductsid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: include
      - in: path
        name: store-hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Single
      - Product
      - Expanded
      - Sub-resources
    put:
      summary: Update a product in the catalog
      description: Updates a single product's information in the catalog
      operationId: V3CatalogProductsByStoreHashAndIdPut
      x-api-path-slug: storehashv3catalogproductsid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store-hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - In
      - Catalog
    delete:
      summary: Delete a single product by ID
      description: Deleting a single product from the catalog by product ID
      operationId: V3CatalogProductsByStoreHashAndIdDelete
      x-api-path-slug: storehashv3catalogproductsid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store-hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Product
      - By
      - ID
  /{store_hash}/v3/catalog/products/{id}/videos/{id}:
    get:
      summary: Retrieve a video on a product
      description: ""
      operationId: V3CatalogProductsVideosIdByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogproductsidvideosid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Video
      - "On"
      - Product
    put:
      summary: Updates an video on a product
      description: ""
      operationId: V3CatalogProductsVideosIdByStoreHashAndIdPut
      x-api-path-slug: store-hashv3catalogproductsidvideosid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - S
      - Video
      - "On"
      - Product
    delete:
      summary: Delete a video on a product
      description: ""
      operationId: V3CatalogProductsVideosIdByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogproductsidvideosid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Video
      - "On"
      - Product
  /{store_hash}/v3/catalog/products/variants:
    get:
      summary: Retrieve variant with parameters
      description: Returns a `Variant` object list from the BigCommerce Catalog.
      operationId: V3CatalogProductsVariantsByStoreHashGet
      x-api-path-slug: store-hashv3catalogproductsvariants-get
      parameters:
      - in: query
        name: sku
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Variant
      - Parameters
  /{store_hash}/v3/catalog/products/{id}/videos:
    get:
      summary: Retrieve all videos for a single product
      description: ""
      operationId: V3CatalogProductsVideosByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogproductsidvideos-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - ""
      - Videosa
      - Single
      - Product
    post:
      summary: Add a video to a product using a video ID from Youtube
      description: Creates an video on a product using a video ID from Youtube
      operationId: V3CatalogProductsVideosByStoreHashAndIdPost
      x-api-path-slug: store-hashv3catalogproductsidvideos-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Video
      - To
      - Product
      - Using
      - Video
      - ID
      - From
      - Youtube
  /{store_hash}/v3/catalog/categories/{id}:
    get:
      summary: Retrieve a single category
      description: ""
      operationId: V3CatalogCategoriesByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogcategoriesid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Single
      - Category
    put:
      summary: Update a category
      description: Update a `Category` in the BigCommerce Catalog
      operationId: V3CatalogCategoriesByStoreHashAndIdPut
      x-api-path-slug: store-hashv3catalogcategoriesid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Category
    delete:
      summary: Delete a single category
      description: ""
      operationId: V3CatalogCategoriesByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogcategoriesid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Category
  /{store_hash}/v3/catalog/brands/{id}/image:
    post:
      summary: Upload an image for a brand
      description: ""
      operationId: V3CatalogBrandsImageByStoreHashAndIdPost
      x-api-path-slug: store-hashv3catalogbrandsidimage-post
      parameters:
      - in: path
        name: id
      - in: formData
        name: image_file
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Upload
      - Imagea
      - Brand
    delete:
      summary: Delete a brand image
      description: Delete a `Brand` image the BigCommerce Catalog
      operationId: V3CatalogBrandsImageByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogbrandsidimage-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Brand
      - Image
  /{store-hash}/v3/catalog/products:
    get:
      summary: Retrieve all products with expanded sub-resources
      description: Shows full product data with a single GET request
      operationId: V3CatalogProductsByStoreHashGet
      x-api-path-slug: storehashv3catalogproducts-get
      parameters:
      - in: query
        name: include
      - in: path
        name: store-hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - ""
      - Products
      - Expanded
      - Sub-resources
    post:
      summary: Create a new product with variants
      description: Sample request for creating a new product with variants through
        V3 Catalog API
      operationId: V3CatalogProductsByStoreHashPost
      x-api-path-slug: storehashv3catalogproducts-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: store-hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Product
      - Variants
    delete:
      summary: Delete multiple products
      description: Deletes products that aren't marked as visible using a filter parameter
      operationId: V3CatalogProductsByStoreHashDelete
      x-api-path-slug: storehashv3catalogproducts-delete
      parameters:
      - in: query
        name: is_visible
      - in: path
        name: store-hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Multiple
      - Products
  /{store_hash}/v3/catalog/summary:
    get:
      summary: Returns a lightweight inventory summary
      description: Returns a lightweight inventory summary from the BigCommerce Catalog.
      operationId: V3CatalogSummaryByStoreHashGet
      x-api-path-slug: store-hashv3catalogsummary-get
      parameters:
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Returns
      - Lightweight
      - Inventory
      - Summary
  /{store_hash}/v3/catalog/products/{id}/options:
    get:
      summary: Retrieve an array of product options
      description: ""
      operationId: V3CatalogProductsOptionsByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogproductsidoptions-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Array
      - Of
      - Product
      - Options
    post:
      summary: Create a product option
      description: ""
      operationId: V3CatalogProductsOptionsByStoreHashAndIdPost
      x-api-path-slug: store-hashv3catalogproductsidoptions-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - Option
  /{store_hash}/v3/catalog/categories/{id}/image:
    post:
      summary: Create an image for a category
      description: ""
      operationId: V3CatalogCategoriesImageByStoreHashAndIdPost
      x-api-path-slug: store-hashv3catalogcategoriesidimage-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Imagea
      - Category
    delete:
      summary: Delete a category image
      description: ""
      operationId: V3CatalogCategoriesImageByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogcategoriesidimage-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Category
      - Image
  /{store_hash}/v3/catalog/products/{id}/modifiers:
    get:
      summary: Retrieve an array of product modifiers
      description: ""
      operationId: V3CatalogProductsModifiersByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogproductsidmodifiers-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Array
      - Of
      - Product
      - Modifiers
    post:
      summary: Create a product modifier
      description: ""
      operationId: V3CatalogProductsModifiersByStoreHashAndIdPost
      x-api-path-slug: store-hashv3catalogproductsidmodifiers-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - Modifier
  /{store-hash}/v3/catalog/products/{id}/images/{id}:
    get:
      summary: Retrieve a single product image's data
      description: GET request for a specific product image by ID
      operationId: V3CatalogProductsImagesIdByStoreHashAndIdGet
      x-api-path-slug: storehashv3catalogproductsidimagesid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store-hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Single
      - Product
      - Images
      - Data
    put:
      summary: Update product image information
      description: This is used to update the information for an existing product
        image
      operationId: V3CatalogProductsImagesIdByStoreHashAndIdPut
      x-api-path-slug: storehashv3catalogproductsidimagesid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store-hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - Image
      - Information
    delete:
      summary: Delete a single product image
      description: Delete a product image and it's description
      operationId: V3CatalogProductsImagesIdByStoreHashAndIdDelete
      x-api-path-slug: storehashv3catalogproductsidimagesid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store-hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Product
      - Image
  /{store_hash}/v3/catalog/brands:
    get:
      summary: Retrieve brands
      description: ""
      operationId: V3CatalogBrandsByStoreHashGet
      x-api-path-slug: store-hashv3catalogbrands-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: page
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Brands
    post:
      summary: Create a new brand
      description: ""
      operationId: V3CatalogBrandsByStoreHashPost
      x-api-path-slug: store-hashv3catalogbrands-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Brand
    delete:
      summary: Delete a brand or brands
      description: Delete one or more `Brand` objects from the BigCommerce Catalog
      operationId: V3CatalogBrandsByStoreHashDelete
      x-api-path-slug: store-hashv3catalogbrands-delete
      parameters:
      - in: query
        name: page_title
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Brand
      - Brands
  /{store_hash}/v3/customers/subscribers:
    get:
      summary: Returns all newsletter subscribers
      description: Returns a paginated Subscribers collection.
      operationId: V3CustomersSubscribersByStoreHashGet
      x-api-path-slug: store-hashv3customerssubscribers-get
      parameters:
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Returns
      - ""
      - Newsletter
      - Subscribers
    post:
      summary: Create a new subscriber
      description: ""
      operationId: V3CustomersSubscribersByStoreHashPost
      x-api-path-slug: store-hashv3customerssubscribers-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Subscriber
    delete:
      summary: Delete a group of subscribers by parameter
      description: ""
      operationId: V3CustomersSubscribersByStoreHashDelete
      x-api-path-slug: store-hashv3customerssubscribers-delete
      parameters:
      - in: query
        name: date_created
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Group
      - Of
      - Subscribers
      - By
      - Parameter
  /{store_hash}/v3/catalog/categories:
    get:
      summary: Retrieve categories
      description: Returns a paginated categories collection from the BigCommerce
        Catalog
      operationId: V3CatalogCategoriesByStoreHashGet
      x-api-path-slug: store-hashv3catalogcategories-get
      parameters:
      - in: query
        name: is_visible
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Categories
    post:
      summary: Create a new category
      description: ""
      operationId: V3CatalogCategoriesByStoreHashPost
      x-api-path-slug: store-hashv3catalogcategories-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Category
    delete:
      summary: Delete a category or categories
      description: ""
      operationId: V3CatalogCategoriesByStoreHashDelete
      x-api-path-slug: store-hashv3catalogcategories-delete
      parameters:
      - in: query
        name: is_visible
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Category
      - Categories
  /{store_hash}/v3/catalog/categories/tree:
    get:
      summary: Retrieve category structure/tree
      description: ""
      operationId: V3CatalogCategoriesTreeByStoreHashGet
      x-api-path-slug: store-hashv3catalogcategoriestree-get
      parameters:
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Category
      - Structure
      - Tree
  /{store_hash}/v3/catalog/products/{id}/variants/{id}:
    get:
      summary: Retrieve a single variant
      description: Get a `Variant` object.
      operationId: V3CatalogProductsVariantsIdByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogproductsidvariantsid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Single
      - Variant
    put:
      summary: Update a variant
      description: Update a `Variant` object.
      operationId: V3CatalogProductsVariantsIdByStoreHashAndIdPut
      x-api-path-slug: store-hashv3catalogproductsidvariantsid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Variant
    delete:
      summary: Delete a variant
      description: Delete a `Variant`
      operationId: V3CatalogProductsVariantsIdByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogproductsidvariantsid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Variant
  /{store_hash}/v3/catalog/products/{id}/modifiers/{id}:
    get:
      summary: Retrieve a product modifier
      description: ""
      operationId: V3CatalogProductsModifiersIdByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogproductsidmodifiersid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Product
      - Modifier
    put:
      summary: Update a product modifier
      description: ""
      operationId: V3CatalogProductsModifiersIdByStoreHashAndIdPut
      x-api-path-slug: store-hashv3catalogproductsidmodifiersid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - Modifier
    delete:
      summary: Delete a product's modifier
      description: ""
      operationId: V3CatalogProductsModifiersIdByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogproductsidmodifiersid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Products
      - Modifier
  /{store_hash}/v3/customers/subscribers/{id}:
    get:
      summary: Return a single subscriber by ID
      description: ""
      operationId: V3CustomersSubscribersByStoreHashAndIdGet
      x-api-path-slug: store-hashv3customerssubscribersid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Return
      - Single
      - Subscriber
      - By
      - ID
    put:
      summary: Update a single subscriber
      description: ""
      operationId: V3CustomersSubscribersByStoreHashAndIdPut
      x-api-path-slug: store-hashv3customerssubscribersid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Subscriber
    delete:
      summary: Delete a single subscriber by ID
      description: ""
      operationId: V3CustomersSubscribersByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3customerssubscribersid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Subscriber
      - By
      - ID
  /{store_id}/v3/catalog/products/{id}/options/{id}:
    put:
      summary: Update a product option
      description: ""
      operationId: V3CatalogProductsOptionsIdByStoreIdAndIdPut
      x-api-path-slug: store-idv3catalogproductsidoptionsid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_id
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - Option
  /{store_hash}/v3/catalog/brands/{id}:
    get:
      summary: Retrieve a brand
      description: ""
      operationId: V3CatalogBrandsByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogbrandsid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Brand
    put:
      summary: Update a brand
      description: ""
      operationId: V3CatalogBrandsByStoreHashAndIdPut
      x-api-path-slug: store-hashv3catalogbrandsid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Brand
    delete:
      summary: Delete a brand
      description: ""
      operationId: V3CatalogBrandsByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogbrandsid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Brand
  /{store_hash}/v3/catalog/products/{id}/options/{id}:
    get:
      summary: Retrieve a product option
      description: Gets `Option` object by product id and option id.
      operationId: V3CatalogProductsOptionsIdByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogproductsidoptionsid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Product
      - Option
    delete:
      summary: Delete a product option
      description: ""
      operationId: V3CatalogProductsOptionsIdByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogproductsidoptionsid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - Option
  /{store_hash}/v3/catalog/products/{id}/modifiers/{id}/values/{id}/image:
    post:
      summary: Add an image to a modifier value
      description: "Add an image to a modifier value that will show on the storefront
        when it\u2019s selected"
      operationId: V3CatalogProductsModifiersIdValuesIdImageByStoreHashAndIdPost
      x-api-path-slug: store-hashv3catalogproductsidmodifiersidvaluesidimage-post
      parameters:
      - in: path
        name: id
      - in: formData
        name: image_file
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Image
      - To
      - Modifier
      - Value
    delete:
      summary: Delete the image associated with a modifier
      description: Delete the image applied to show when the modifier value is selected
      operationId: V3CatalogProductsModifiersIdValuesIdImageByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogproductsidmodifiersidvaluesidimage-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Image
      - Associated
      - Modifier
  /{store_hash}/v3/catalog/products/{id}/variants/{id}/image:
    post:
      summary: Upload a variant image
      description: ""
      operationId: V3CatalogProductsVariantsIdImageByStoreHashAndIdPost
      x-api-path-slug: store-hashv3catalogproductsidvariantsidimage-post
      parameters:
      - in: path
        name: id
      - in: formData
        name: image_file
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Upload
      - Variant
      - Image
  /{store_hash}/v3/catalog/products/{id}/variants:
    get:
      summary: Retrieve a list of variants
      description: Returns a `Variant` object list from the BigCommerce Catalog.
      operationId: V3CatalogProductsVariantsByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogproductsidvariants-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - List
      - Of
      - Variants
    post:
      summary: Create a variant
      description: ""
      operationId: V3CatalogProductsVariantsByStoreHashAndIdPost
      x-api-path-slug: store-hashv3catalogproductsidvariants-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Variant