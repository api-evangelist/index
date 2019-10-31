swagger: "2.0"
x-collection-name: Gumroad
x-complete: 1
info:
  title: Gumroad
  description: api-for-selling-of-digital-goods-and-media-
  termsOfService: https://gumroad.com/terms
  version: v1
host: api.gumroad.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /products:
    get:
      summary: Get Products
      description: Retrieve all of the existing products for the authenticated user.
      operationId: getProducts
      x-api-path-slug: products-get
      responses:
        200:
          description: OK
      tags:
      - Products
    post:
      summary: Post Products
      description: Create a new product for the user.
      operationId: postProducts
      x-api-path-slug: products-post
      parameters:
      - in: query
        name: country_available
      - in: query
        name: customizable_price
      - in: query
        name: custom_filetype
      - in: query
        name: custom_permalink
      - in: query
        name: custom_product_type
      - in: query
        name: custom_receipt
      - in: query
        name: custom_summary
      - in: query
        name: description
      - in: query
        name: max_purchase_count
      - in: query
        name: name
      - in: query
        name: preview_urlnornpreview
      - in: query
        name: price
      - in: query
        name: require_shipping
      - in: query
        name: shown_on_profile
      - in: query
        name: urlnornfile
      - in: query
        name: webhook
      responses:
        200:
          description: OK
      tags:
      - Products
  /products/:id:
    delete:
      summary: Delete Products
      description: Permanently delete a product.
      operationId: deleteProducts
      x-api-path-slug: productsid-delete
      responses:
        200:
          description: OK
      tags:
      - Products
    get:
      summary: Get Products
      description: Retrieve the details of a product.
      operationId: getProducts
      x-api-path-slug: productsid-get
      responses:
        200:
          description: OK
      tags:
      - Products
    put:
      summary: Put Products
      description: Edit an existing product.
      operationId: putProducts
      x-api-path-slug: productsid-put
      parameters:
      - in: query
        name: countries_available
      - in: query
        name: customizable_price
      - in: query
        name: custom_filetype
      - in: query
        name: custom_permalink
      - in: query
        name: custom_product_type
      - in: query
        name: custom_receipt
      - in: query
        name: custom_summary
      - in: query
        name: description
      - in: query
        name: max_purchase_count
      - in: query
        name: name
      - in: query
        name: preview_urlnornpreview
      - in: query
        name: price
      - in: query
        name: product
      - in: query
        name: require_shipping
      - in: query
        name: shown_on_profile
      - in: query
        name: subscription_duration
      - in: query
        name: urlnornfile
      - in: query
        name: webhook
      responses:
        200:
          description: OK
      tags:
      - Products
  /products/:id/enable:
    put:
      summary: Put Products Enable
      description: Enable an existing product.
      operationId: putProductsEnable
      x-api-path-slug: productsidenable-put
      responses:
        200:
          description: OK
      tags:
      - Products
      - Enable
  /products/:product_id/custom_fields:
    get:
      summary: Get Products Custom Fields
      description: Retrieve all of the existing custom fields for a product.
      operationId: getProductsProductCustomFields
      x-api-path-slug: productsproduct-idcustom-fields-get
      responses:
        200:
          description: OK
      tags:
      - Products
      - Custom
      - Fields
    post:
      summary: Post Products Custom Fields
      description: Create a new custom field for a product.
      operationId: postProductsProductCustomFields
      x-api-path-slug: productsproduct-idcustom-fields-post
      parameters:
      - in: query
        name: name
      - in: query
        name: required
      - in: query
        name: variant
      responses:
        200:
          description: OK
      tags:
      - Products
      - Custom
      - Fields
  /products/:product_id/custom_fields/:name:
    put:
      summary: Put Products Custom Fields Name
      description: Edit an existing products custom field.
      operationId: putProductsProductCustomFieldsName
      x-api-path-slug: productsproduct-idcustom-fieldsname-put
      parameters:
      - in: query
        name: required
      - in: query
        name: variant
      responses:
        200:
          description: OK
      tags:
      - Products
      - Custom
      - Fields
      - :name
  /products/:product_id/offer_codes:
    get:
      summary: Get Products Offer Codes
      description: Retrieve all of the existing offer codes for a product. Either
        amount_cents or percent_off will be returned depending if the offer code is
        a fixed amount off or a percentage off. A universal offer code is one that
        applies to all products.
      operationId: getProductsProductOfferCodes
      x-api-path-slug: productsproduct-idoffer-codes-get
      responses:
        200:
          description: OK
      tags:
      - Products
      - Offer
      - Codes
    post:
      summary: Post Products Offer Codes
      description: Create a new offer code for a product. Default offer code is in
        cents. A universal offer code is one that applies to all products.
      operationId: postProductsProductOfferCodes
      x-api-path-slug: productsproduct-idoffer-codes-post
      parameters:
      - in: query
        name: amount_off
      - in: query
        name: max_purchase_count
      - in: query
        name: name
      - in: query
        name: offer_code
      - in: query
        name: offer_type
      - in: query
        name: universal
      responses:
        200:
          description: OK
      tags:
      - Products
      - Offer
      - Codes
  /products/:product_id/offer_codes/:id:
    get:
      summary: Get Products Offer Codes
      description: Retrieve the details of a specific offer code of a product
      operationId: getProductsProductOfferCodes
      x-api-path-slug: productsproduct-idoffer-codesid-get
      responses:
        200:
          description: OK
      tags:
      - Products
      - Offer
      - Codes
    put:
      summary: Put Products Offer Codes
      description: Edit an existing products offer code.
      operationId: putProductsProductOfferCodes
      x-api-path-slug: productsproduct-idoffer-codesid-put
      parameters:
      - in: query
        name: max_purchase_count
      - in: query
        name: offer_code
      responses:
        200:
          description: OK
      tags:
      - Products
      - Offer
      - Codes
  /products/:product_id/variant_categories:
    get:
      summary: Get Products Variant Categories
      description: Retrieve all of the existing variant categories of a product.
      operationId: getProductsProductVariantCategories
      x-api-path-slug: productsproduct-idvariant-categories-get
      responses:
        200:
          description: OK
      tags:
      - Products
      - Variant
      - Categories
    post:
      summary: Post Products Variant Categories
      description: Create a new variant category on a product.
      operationId: postProductsProductVariantCategories
      x-api-path-slug: productsproduct-idvariant-categories-post
      parameters:
      - in: query
        name: title
      - in: query
        name: variant_category
      responses:
        200:
          description: OK
      tags:
      - Products
      - Variant
      - Categories
  /products/:product_id/variant_categories/:id:
    delete:
      summary: Delete Products Variant Categories
      description: Permanently delete a variant category of a product.
      operationId: deleteProductsProductVariantCategories
      x-api-path-slug: productsproduct-idvariant-categoriesid-delete
      responses:
        200:
          description: OK
      tags:
      - Products
      - Variant
      - Categories
    get:
      summary: Get Products Variant Categories
      description: Retrieve the details of a variant category of a product.
      operationId: getProductsProductVariantCategories
      x-api-path-slug: productsproduct-idvariant-categoriesid-get
      responses:
        200:
          description: OK
      tags:
      - Products
      - Variant
      - Categories
    put:
      summary: Put Products Variant Categories
      description: Edit a variant category of an existing product.
      operationId: putProductsProductVariantCategories
      x-api-path-slug: productsproduct-idvariant-categoriesid-put
      parameters:
      - in: query
        name: title
      - in: query
        name: variant_category
      responses:
        200:
          description: OK
      tags:
      - Products
      - Variant
      - Categories
  /products/:product_id/variant_categories/:variant_category_id/variants:
    post:
      summary: Post Products Variant Categories Variant Category Variants
      description: Create a new variant of a product.
      operationId: postProductsProductVariantCategoriesVariantCategoryVariants
      x-api-path-slug: productsproduct-idvariant-categoriesvariant-category-idvariants-post
      parameters:
      - in: query
        name: max_purchase_count
      - in: query
        name: name
      - in: query
        name: price_difference_cents
      - in: query
        name: variant
      responses:
        200:
          description: OK
      tags:
      - Products
      - Variant
      - Categories
      - :variant
      - Category
      - Variants
  /products/:product_id/variant_categories/:variant_category_id/variants/:id:
    delete:
      summary: Delete Products Variant Categories Variant Category Variants
      description: Permanently delete a variant of a product.
      operationId: deleteProductsProductVariantCategoriesVariantCategoryVariants
      x-api-path-slug: productsproduct-idvariant-categoriesvariant-category-idvariantsid-delete
      responses:
        200:
          description: OK
      tags:
      - Products
      - Variant
      - Categories
      - :variant
      - Category
      - Variants
    get:
      summary: Get Products Variant Categories Variant Category Variants
      description: Retrieve the details of a variant of a product.
      operationId: getProductsProductVariantCategoriesVariantCategoryVariants
      x-api-path-slug: productsproduct-idvariant-categoriesvariant-category-idvariantsid-get
      responses:
        200:
          description: OK
      tags:
      - Products
      - Variant
      - Categories
      - :variant
      - Category
      - Variants
    put:
      summary: Put Products Variant Categories Variant Category Variants
      description: Edit a variant of an existing product.
      operationId: putProductsProductVariantCategoriesVariantCategoryVariants
      x-api-path-slug: productsproduct-idvariant-categoriesvariant-category-idvariantsid-put
      parameters:
      - in: query
        name: max_purchase_count
      - in: query
        name: name
      - in: query
        name: price_difference_cents
      - in: query
        name: variant
      responses:
        200:
          description: OK
      tags:
      - Products
      - Variant
      - Categories
      - :variant
      - Category
      - Variants