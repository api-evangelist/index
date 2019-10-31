swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 1
info:
  title: Broadleaf Commerce API
  description: the-default-broadleaf-commerce-apis
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /auditevents:
    get:
      summary: Get Auditevents
      description: Get auditevents.
      operationId: getAuditevents
      x-api-path-slug: auditevents-get
      parameters:
      - in: query
        name: after
        description: after
      - in: query
        name: principal
        description: principal
      - in: query
        name: type
        description: type
      responses:
        200:
          description: OK
      tags:
      - Auditevents
  /auditevents.json:
    get:
      summary: Get Auditevents
      description: Get auditevents.
      operationId: getAuditevents.json
      x-api-path-slug: auditevents-json-get
      parameters:
      - in: query
        name: after
        description: after
      - in: query
        name: principal
        description: principal
      - in: query
        name: type
        description: type
      responses:
        200:
          description: OK
      tags:
      - Auditevents
  /autoconfig:
    get:
      summary: Get Autoconfig
      description: Get autoconfig.
      operationId: getAutoconfig
      x-api-path-slug: autoconfig-get
      responses:
        200:
          description: OK
      tags:
      - Autoconfig
  /autoconfig.json:
    get:
      summary: Get Autoconfig
      description: Get autoconfig.
      operationId: getAutoconfig.json
      x-api-path-slug: autoconfig-json-get
      responses:
        200:
          description: OK
      tags:
      - Autoconfig
  /beans:
    get:
      summary: Get Beans
      description: Get beans.
      operationId: getBeans
      x-api-path-slug: beans-get
      responses:
        200:
          description: OK
      tags:
      - Beans
  /beans.json:
    get:
      summary: Get Beans
      description: Get beans.
      operationId: getBeans.json
      x-api-path-slug: beans-json-get
      responses:
        200:
          description: OK
      tags:
      - Beans
  /cart:
    get:
      summary: Get Cart
      description: Get cart.
      operationId: getCart
      x-api-path-slug: cart-get
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Cart
    post:
      summary: Post Cart
      description: Post cart.
      operationId: postCart
      x-api-path-slug: cart-post
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Cart
  /cart/checkout:
    post:
      summary: Post Cart Checkout
      description: Post cart checkout.
      operationId: postCartCheckout
      x-api-path-slug: cartcheckout-post
      parameters:
      - in: query
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
  /cart/checkout/payment:
    post:
      summary: Post Cart Checkout Payment
      description: Post cart checkout payment.
      operationId: postCartCheckoutPayment
      x-api-path-slug: cartcheckoutpayment-post
      parameters:
      - in: query
        name: cartId
        description: cartId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
  /cart/checkout/payment/{customerPaymentId}:
    post:
      summary: Post Cart Checkout Payment Customerpaymentid
      description: Post cart checkout payment customerpaymentid.
      operationId: postCartCheckoutPaymentCustomerpayment
      x-api-path-slug: cartcheckoutpaymentcustomerpaymentid-post
      parameters:
      - in: query
        name: amount
        description: amount
      - in: query
        name: cartId
        description: cartId
      - in: query
        name: currency
        description: currency
      - in: path
        name: customerPaymentId
        description: customerPaymentId
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
      - Customerpaymentid
  /cart/checkout/payment/{paymentId}:
    delete:
      summary: Delete Cart Checkout Payment Paymentid
      description: Delete cart checkout payment paymentid.
      operationId: deleteCartCheckoutPaymentPayment
      x-api-path-slug: cartcheckoutpaymentpaymentid-delete
      parameters:
      - in: query
        name: cartId
        description: cartId
      - in: path
        name: paymentId
        description: paymentId
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
      - Paymentid
  /cart/checkout/payment/{paymentId}/transaction:
    put:
      summary: Put Cart Checkout Payment Paymentid Transaction
      description: Put cart checkout payment paymentid transaction.
      operationId: putCartCheckoutPaymentPaymentTransaction
      x-api-path-slug: cartcheckoutpaymentpaymentidtransaction-put
      parameters:
      - in: query
        name: cartId
        description: cartId
      - in: path
        name: paymentId
        description: paymentId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
      - Paymentid
      - Transaction
  /cart/checkout/payments:
    get:
      summary: Get Cart Checkout Payments
      description: Get cart checkout payments.
      operationId: getCartCheckoutPayments
      x-api-path-slug: cartcheckoutpayments-get
      parameters:
      - in: query
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payments
  /cart/{cartId}:
    get:
      summary: Get Cart
      description: Get cart.
      operationId: getCartCart
      x-api-path-slug: cartcartid-get
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Cart
  /cart/{cartId}/attributes:
    put:
      summary: Put Cart Attributes
      description: Put cart attributes.
      operationId: putCartCartAttributes
      x-api-path-slug: cartcartidattributes-put
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: requestParams
        description: requestParams
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Attributes
    delete:
      summary: Delete Cart Attributes
      description: Delete cart attributes.
      operationId: deleteCartCartAttributes
      x-api-path-slug: cartcartidattributes-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: requestParams
        description: requestParams
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Attributes
  /cart/{cartId}/item:
    post:
      summary: Post Cart Item
      description: Post cart item.
      operationId: postCartCartItem
      x-api-path-slug: cartcartiditem-post
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: body
        name: orderItemWrapper
        description: orderItemWrapper
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: priceOrder
        description: priceOrder
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Item
  /cart/{cartId}/item/{itemId}/attributes:
    put:
      summary: Put Cart Item Attributes
      description: Put cart item attributes.
      operationId: putCartCartItemItemAttributes
      x-api-path-slug: cartcartiditemitemidattributes-put
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: requestParams
        description: requestParams
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Item
      - Attributes
    delete:
      summary: Delete Cart Item Attributes
      description: Delete cart item attributes.
      operationId: deleteCartCartItemItemAttributes
      x-api-path-slug: cartcartiditemitemidattributes-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: requestParams
        description: requestParams
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Item
      - Attributes
  /cart/{cartId}/items/{itemId}:
    put:
      summary: Put Cart Items
      description: Put cart items.
      operationId: putCartCartItemsItem
      x-api-path-slug: cartcartiditemsitemid-put
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: query
        name: quantity
        description: quantity
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Items
    delete:
      summary: Delete Cart Items
      description: Delete cart items.
      operationId: deleteCartCartItemsItem
      x-api-path-slug: cartcartiditemsitemid-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: priceOrder
        description: priceOrder
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Items
  /cart/{cartId}/offer/{promoCode}:
    post:
      summary: Post Cart Offer Promocode
      description: Post cart offer promocode.
      operationId: postCartCartOfferPromocode
      x-api-path-slug: cartcartidofferpromocode-post
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: path
        name: promoCode
        description: promoCode
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Offer
      - Promocode
    delete:
      summary: Delete Cart Offer Promocode
      description: Delete cart offer promocode.
      operationId: deleteCartCartOfferPromocode
      x-api-path-slug: cartcartidofferpromocode-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: path
        name: promoCode
        description: promoCode
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Offer
      - Promocode
  /cart/{cartId}/offers:
    delete:
      summary: Delete Cart Offers
      description: Delete cart offers.
      operationId: deleteCartCartOffers
      x-api-path-slug: cartcartidoffers-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Offers
  /catalog/categories:
    get:
      summary: Get Catalog Categories
      description: Get catalog categories.
      operationId: getCatalogCategories
      x-api-path-slug: catalogcategories-get
      parameters:
      - in: query
        name: limit
        description: limit
      - in: query
        name: name
        description: name
      - in: query
        name: offset
        description: offset
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Categories
  /catalog/category:
    get:
      summary: Get Catalog Category
      description: Get catalog category.
      operationId: getCatalogCategory
      x-api-path-slug: catalogcategory-get
      parameters:
      - in: query
        name: productLimit
        description: productLimit
      - in: query
        name: productOffset
        description: productOffset
      - in: query
        name: searchParameter
        description: searchParameter
      - in: query
        name: subcategoryLimit
        description: subcategoryLimit
      - in: query
        name: subcategoryOffset
        description: subcategoryOffset
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
  /catalog/category/{categoryId}:
    get:
      summary: Get Catalog Category
      description: Get catalog category.
      operationId: getCatalogCategoryCategory
      x-api-path-slug: catalogcategorycategoryid-get
      parameters:
      - in: path
        name: categoryId
        description: categoryId
      - in: query
        name: productLimit
        description: productLimit
      - in: query
        name: productOffset
        description: productOffset
      - in: query
        name: subcategoryLimit
        description: subcategoryLimit
      - in: query
        name: subcategoryOffset
        description: subcategoryOffset
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
  /catalog/category/{categoryId}/activeSubcategories:
    get:
      summary: Get Catalog Category Active Subcategories
      description: Get catalog category active subcategories.
      operationId: getCatalogCategoryCategoryActivesubcategories
      x-api-path-slug: catalogcategorycategoryidactivesubcategories-get
      parameters:
      - in: path
        name: categoryId
        description: categoryId
      - in: query
        name: limit
        description: limit
      - in: query
        name: offset
        description: offset
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
      - Active
      - Subcategories
  /catalog/category/{categoryId}/attributes:
    get:
      summary: Get Catalog Category Attributes
      description: Get catalog category attributes.
      operationId: getCatalogCategoryCategoryAttributes
      x-api-path-slug: catalogcategorycategoryidattributes-get
      parameters:
      - in: path
        name: categoryId
        description: categoryId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
      - Attributes
  /catalog/category/{categoryId}/categories:
    get:
      summary: Get Catalog Category Categories
      description: Get catalog category categories.
      operationId: getCatalogCategoryCategoryCategories
      x-api-path-slug: catalogcategorycategoryidcategories-get
      parameters:
      - in: query
        name: active
        description: active
      - in: path
        name: categoryId
        description: categoryId
      - in: query
        name: limit
        description: limit
      - in: query
        name: offset
        description: offset
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
      - Categories
  /catalog/category/{id}/media:
    get:
      summary: Get Catalog Category Media
      description: Get catalog category media.
      operationId: getCatalogCategoryMedia
      x-api-path-slug: catalogcategoryidmedia-get
      parameters:
      - in: path
        name: id
        description: id
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
      - Media
  /catalog/product/{id}:
    get:
      summary: Get Catalog Product
      description: Get catalog product.
      operationId: getCatalogProduct
      x-api-path-slug: catalogproductid-get
      parameters:
      - in: path
        name: id
        description: id
      - in: query
        name: includePriceData
        description: includePriceData
      - in: query
        name: includePromotionMessages
        description: includePromotionMessages
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
  /catalog/product/{productId}/attributes:
    get:
      summary: Get Catalog Product Attributes
      description: Get catalog product attributes.
      operationId: getCatalogProductProductAttributes
      x-api-path-slug: catalogproductproductidattributes-get
      parameters:
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Attributes
  /catalog/product/{productId}/categories:
    get:
      summary: Get Catalog Product Categories
      description: Get catalog product categories.
      operationId: getCatalogProductProductCategories
      x-api-path-slug: catalogproductproductidcategories-get
      parameters:
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Categories
  /catalog/product/{productId}/crosssale:
    get:
      summary: Get Catalog Product Crosssale
      description: Get catalog product crosssale.
      operationId: getCatalogProductProductCrosssale
      x-api-path-slug: catalogproductproductidcrosssale-get
      parameters:
      - in: query
        name: limit
        description: limit
      - in: query
        name: offset
        description: offset
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Crosssale
  /catalog/product/{productId}/defaultSku:
    get:
      summary: Get Catalog Product Default sku
      description: Get catalog product default sku.
      operationId: getCatalogProductProductDefaultsku
      x-api-path-slug: catalogproductproductiddefaultsku-get
      parameters:
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Default
      - Sku
  /catalog/product/{productId}/media:
    get:
      summary: Get Catalog Product Media
      description: Get catalog product media.
      operationId: getCatalogProductProductMedia
      x-api-path-slug: catalogproductproductidmedia-get
      parameters:
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Media
  /catalog/product/{productId}/skus:
    get:
      summary: Get Catalog Product Skus
      description: Get catalog product skus.
      operationId: getCatalogProductProductSkus
      x-api-path-slug: catalogproductproductidskus-get
      parameters:
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Skus
  /catalog/product/{productId}/upsale:
    get:
      summary: Get Catalog Product Upsale
      description: Get catalog product upsale.
      operationId: getCatalogProductProductUpsale
      x-api-path-slug: catalogproductproductidupsale-get
      parameters:
      - in: query
        name: limit
        description: limit
      - in: query
        name: offset
        description: offset
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Upsale
  /catalog/search:
    get:
      summary: Get Catalog Search
      description: Get catalog search.
      operationId: getCatalogSearch
      x-api-path-slug: catalogsearch-get
      parameters:
      - in: query
        name: includePriceData
        description: includePriceData
      - in: query
        name: includePromotionMessages
        description: includePromotionMessages
      - in: query
        name: page
        description: page
      - in: query
        name: pageSize
        description: pageSize
      - in: query
        name: q
        description: q
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Search
  /catalog/search/category/{categoryId}:
    get:
      summary: Get Catalog Search Category
      description: Get catalog search category.
      operationId: getCatalogSearchCategoryCategory
      x-api-path-slug: catalogsearchcategorycategoryid-get
      parameters:
      - in: path
        name: categoryId
        description: categoryId
      - in: query
        name: includePriceData
        description: includePriceData
      - in: query
        name: includePromotionMessages
        description: includePromotionMessages
      - in: query
        name: page
        description: page
      - in: query
        name: pageSize
        description: pageSize
      - in: query
        name: q
        description: q
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Search
      - Category
  /catalog/sku/inventory:
    get:
      summary: Get Catalog Sku Inventory
      description: Get catalog sku inventory.
      operationId: getCatalogSkuInventory
      x-api-path-slug: catalogskuinventory-get
      parameters:
      - in: query
        name: id
        description: id
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Sku
      - Inventory
  /catalog/sku/{skuId}:
    get:
      summary: Get Catalog Sku Skuid
      description: Get catalog sku skuid.
      operationId: getCatalogSkuSku
      x-api-path-slug: catalogskuskuid-get
      parameters:
      - in: path
        name: skuId
        description: skuId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Sku
      - Skuid
  /catalog/sku/{skuId}/attributes:
    get:
      summary: Get Catalog Sku Skuid Attributes
      description: Get catalog sku skuid attributes.
      operationId: getCatalogSkuSkuAttributes
      x-api-path-slug: catalogskuskuidattributes-get
      parameters:
      - in: path
        name: skuId
        description: skuId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Sku
      - Skuid
      - Attributes
  /catalog/sku/{skuId}/media:
    get:
      summary: Get Catalog Sku Skuid Media
      description: Get catalog sku skuid media.
      operationId: getCatalogSkuSkuMedia
      x-api-path-slug: catalogskuskuidmedia-get
      parameters:
      - in: path
        name: skuId
        description: skuId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Sku
      - Skuid
      - Media
  /configprops:
    get:
      summary: Get Configprops
      description: Get configprops.
      operationId: getConfigprops
      x-api-path-slug: configprops-get
      responses:
        200:
          description: OK
      tags:
      - Configprops
  /configprops.json:
    get:
      summary: Get Configprops
      description: Get configprops.
      operationId: getConfigprops.json
      x-api-path-slug: configprops-json-get
      responses:
        200:
          description: OK
      tags:
      - Configprops
  /customer:
    get:
      summary: Get Customer
      description: Get customer.
      operationId: getCustomer
      x-api-path-slug: customer-get
      parameters:
      - in: query
        name: email
        description: email
      responses:
        200:
          description: OK
      tags:
      - Customer
    post:
      summary: Post Customer
      description: Post customer.
      operationId: postCustomer
      x-api-path-slug: customer-post
      parameters:
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
    put:
      summary: Put Customer
      description: Put customer.
      operationId: putCustomer
      x-api-path-slug: customer-put
      parameters:
      - in: query
        name: customerId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
  /customer/address:
    get:
      summary: Get Customer Address
      description: Get customer address.
      operationId: getCustomerAddress
      x-api-path-slug: customeraddress-get
      parameters:
      - in: query
        name: addressName
        description: addressName
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Ress
    put:
      summary: Put Customer Address
      description: Put customer address.
      operationId: putCustomerAddress
      x-api-path-slug: customeraddress-put
      parameters:
      - in: query
        name: customerId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Ress
  /customer/address/{addressId}:
    put:
      summary: Put Customer Address Addressid
      description: Put customer address addressid.
      operationId: putCustomerAddressAddress
      x-api-path-slug: customeraddressaddressid-put
      parameters:
      - in: path
        name: addressId
        description: addressId
      - in: query
        name: customerId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Ress
      - Ressid
  /customer/address/{addressName}:
    delete:
      summary: Delete Customer Address Addressname
      description: Delete customer address addressname.
      operationId: deleteCustomerAddressAddressname
      x-api-path-slug: customeraddressaddressname-delete
      parameters:
      - in: path
        name: addressName
        description: addressName
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Ress
      - Ressname
  /customer/addresses:
    get:
      summary: Get Customer Addresses
      description: Get customer addresses.
      operationId: getCustomerAddresses
      x-api-path-slug: customeraddresses-get
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Resses
    delete:
      summary: Delete Customer Addresses
      description: Delete customer addresses.
      operationId: deleteCustomerAddresses
      x-api-path-slug: customeraddresses-delete
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Resses
  /customer/attribute:
    put:
      summary: Put Customer Attribute
      description: Put customer attribute.
      operationId: putCustomerAttribute
      x-api-path-slug: customerattribute-put
      parameters:
      - in: query
        name: customerId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Attribute
  /customer/attribute/{attributeName}:
    delete:
      summary: Delete Customer Attribute Attributename
      description: Delete customer attribute attributename.
      operationId: deleteCustomerAttributeAttributename
      x-api-path-slug: customerattributeattributename-delete
      parameters:
      - in: path
        name: attributeName
        description: attributeName
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Attribute
      - Attributename
  /customer/attributes:
    delete:
      summary: Delete Customer Attributes
      description: Delete customer attributes.
      operationId: deleteCustomerAttributes
      x-api-path-slug: customerattributes-delete
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Attributes
  /customer/password:
    post:
      summary: Post Customer Password
      description: Post customer password.
      operationId: postCustomerPassword
      x-api-path-slug: customerpassword-post
      parameters:
      - in: body
        name: changePasswordForm
        description: changePasswordForm
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Password
  /customer/payment:
    get:
      summary: Get Customer Payment
      description: Get customer payment.
      operationId: getCustomerPayment
      x-api-path-slug: customerpayment-get
      parameters:
      - in: query
        name: customerId
      - in: query
        name: paymentId
        description: paymentId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payment
    post:
      summary: Post Customer Payment
      description: Post customer payment.
      operationId: postCustomerPayment
      x-api-path-slug: customerpayment-post
      parameters:
      - in: query
        name: customerId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payment
  /customer/payment/{paymentId}:
    put:
      summary: Put Customer Payment Paymentid
      description: Put customer payment paymentid.
      operationId: putCustomerPaymentPayment
      x-api-path-slug: customerpaymentpaymentid-put
      parameters:
      - in: query
        name: customerId
      - in: path
        name: paymentId
        description: paymentId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payment
      - Paymentid
    delete:
      summary: Delete Customer Payment Paymentid
      description: Delete customer payment paymentid.
      operationId: deleteCustomerPaymentPayment
      x-api-path-slug: customerpaymentpaymentid-delete
      parameters:
      - in: query
        name: customerId
      - in: path
        name: paymentId
        description: paymentId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payment
      - Paymentid
  /customer/payments:
    get:
      summary: Get Customer Payments
      description: Get customer payments.
      operationId: getCustomerPayments
      x-api-path-slug: customerpayments-get
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payments
    delete:
      summary: Delete Customer Payments
      description: Delete customer payments.
      operationId: deleteCustomerPayments
      x-api-path-slug: customerpayments-delete
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Payments
  /docsreload:
    get:
      summary: Get Docsreload
      description: Get docsreload.
      operationId: getDocsreload
      x-api-path-slug: docsreload-get
      responses:
        200:
          description: OK
      tags:
      - Docsreload
    head:
      summary: Head Docsreload
      description: Head docsreload.
      operationId: headDocsreload
      x-api-path-slug: docsreload-head
      responses:
        200:
          description: OK
      tags:
      - Head
      - Docsreload
    post:
      summary: Post Docsreload
      description: Post docsreload.
      operationId: postDocsreload
      x-api-path-slug: docsreload-post
      responses:
        200:
          description: OK
      tags:
      - Docsreload
    put:
      summary: Put Docsreload
      description: Put docsreload.
      operationId: putDocsreload
      x-api-path-slug: docsreload-put
      responses:
        200:
          description: OK
      tags:
      - Docsreload
    delete:
      summary: Delete Docsreload
      description: Delete docsreload.
      operationId: deleteDocsreload
      x-api-path-slug: docsreload-delete
      responses:
        200:
          description: OK
      tags:
      - Docsreload
    options:
      summary: Options Docsreload
      description: Options docsreload.
      operationId: optionsDocsreload
      x-api-path-slug: docsreload-options
      responses:
        200:
          description: OK
      tags:
      - Options
      - Docsreload
    patch:
      summary: Patch Docsreload
      description: Patch docsreload.
      operationId: patchDocsreload
      x-api-path-slug: docsreload-patch
      responses:
        200:
          description: OK
      tags:
      - Docsreload
  /dump:
    get:
      summary: Get Dump
      description: Get dump.
      operationId: getDump
      x-api-path-slug: dump-get
      responses:
        200:
          description: OK
      tags:
      - Dump
  /dump.json:
    get:
      summary: Get Dump
      description: Get dump.
      operationId: getDump.json
      x-api-path-slug: dump-json-get
      responses:
        200:
          description: OK
      tags:
      - Dump
  /env:
    get:
      summary: Get Env
      description: Get env.
      operationId: getEnv
      x-api-path-slug: env-get
      responses:
        200:
          description: OK
      tags:
      - Env
  /env.json:
    get:
      summary: Get Env
      description: Get env.
      operationId: getEnv.json
      x-api-path-slug: env-json-get
      responses:
        200:
          description: OK
      tags:
      - Env
  /env/{name}:
    get:
      summary: Get Env Name
      description: Get env name.
      operationId: getEnvName
      x-api-path-slug: envname-get
      parameters:
      - in: path
        name: name
        description: name
      responses:
        200:
          description: OK
      tags:
      - Env
      - Name
  /error:
    get:
      summary: Get Error
      description: Get error.
      operationId: getError
      x-api-path-slug: error-get
      responses:
        200:
          description: OK
      tags:
      - Error
    head:
      summary: Head Error
      description: Head error.
      operationId: headError
      x-api-path-slug: error-head
      responses:
        200:
          description: OK
      tags:
      - Head
      - Error
    post:
      summary: Post Error
      description: Post error.
      operationId: postError
      x-api-path-slug: error-post
      responses:
        200:
          description: OK
      tags:
      - Error
    put:
      summary: Put Error
      description: Put error.
      operationId: putError
      x-api-path-slug: error-put
      responses:
        200:
          description: OK
      tags:
      - Error
    delete:
      summary: Delete Error
      description: Delete error.
      operationId: deleteError
      x-api-path-slug: error-delete
      responses:
        200:
          description: OK
      tags:
      - Error
    options:
      summary: Options Error
      description: Options error.
      operationId: optionsError
      x-api-path-slug: error-options
      responses:
        200:
          description: OK
      tags:
      - Options
      - Error
    patch:
      summary: Patch Error
      description: Patch error.
      operationId: patchError
      x-api-path-slug: error-patch
      responses:
        200:
          description: OK
      tags:
      - Error
  /health:
    get:
      summary: Get Health
      description: Get health.
      operationId: getHealth
      x-api-path-slug: health-get
      responses:
        200:
          description: OK
      tags:
      - Health
  /health.json:
    get:
      summary: Get Health
      description: Get health.
      operationId: getHealth.json
      x-api-path-slug: health-json-get
      responses:
        200:
          description: OK
      tags:
      - Health
  /heapdump:
    get:
      summary: Get Heapdump
      description: Get heapdump.
      operationId: getHeapdump
      x-api-path-slug: heapdump-get
      parameters:
      - in: query
        name: live
        description: live
      responses:
        200:
          description: OK
      tags:
      - Heapdump
  /heapdump.json:
    get:
      summary: Get Heapdump
      description: Get heapdump.
      operationId: getHeapdump.json
      x-api-path-slug: heapdump-json-get
      parameters:
      - in: query
        name: live
        description: live
      responses:
        200:
          description: OK
      tags:
      - Heapdump
  /info:
    get:
      summary: Get Info
      description: Get info.
      operationId: getInfo
      x-api-path-slug: info-get
      responses:
        200:
          description: OK
      tags:
      - Info
  /info.json:
    get:
      summary: Get Info
      description: Get info.
      operationId: getInfo.json
      x-api-path-slug: info-json-get
      responses:
        200:
          description: OK
      tags:
      - Info
  /logfile:
    get:
      summary: Get Logfile
      description: Get logfile.
      operationId: getLogfile
      x-api-path-slug: logfile-get
      responses:
        200:
          description: OK
      tags:
      - Logfile
    head:
      summary: Head Logfile
      description: Head logfile.
      operationId: headLogfile
      x-api-path-slug: logfile-head
      responses:
        200:
          description: OK
      tags:
      - Head
      - Logfile
  /logfile.json:
    get:
      summary: Get Logfile
      description: Get logfile.
      operationId: getLogfile.json
      x-api-path-slug: logfile-json-get
      responses:
        200:
          description: OK
      tags:
      - Logfile
    head:
      summary: Head Logfile
      description: Head logfile.
      operationId: headLogfile.json
      x-api-path-slug: logfile-json-head
      responses:
        200:
          description: OK
      tags:
      - Head
      - Logfile
  /loggers:
    get:
      summary: Get Loggers
      description: Get loggers.
      operationId: getLoggers
      x-api-path-slug: loggers-get
      responses:
        200:
          description: OK
      tags:
      - Loggers
  /loggers.json:
    get:
      summary: Get Loggers
      description: Get loggers.
      operationId: getLoggers.json
      x-api-path-slug: loggers-json-get
      responses:
        200:
          description: OK
      tags:
      - Loggers
  /loggers/{name}:
    get:
      summary: Get Loggers Name
      description: Get loggers name.
      operationId: getLoggersName
      x-api-path-slug: loggersname-get
      parameters:
      - in: path
        name: name
        description: name
      responses:
        200:
          description: OK
      tags:
      - Loggers
      - Name
    post:
      summary: Post Loggers Name
      description: Post loggers name.
      operationId: postLoggersName
      x-api-path-slug: loggersname-post
      parameters:
      - in: body
        name: configuration
        description: configuration
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: name
      responses:
        200:
          description: OK
      tags:
      - Loggers
      - Name
  /mappings:
    get:
      summary: Get Mappings
      description: Get mappings.
      operationId: getMappings
      x-api-path-slug: mappings-get
      responses:
        200:
          description: OK
      tags:
      - Mappings
  /mappings.json:
    get:
      summary: Get Mappings
      description: Get mappings.
      operationId: getMappings.json
      x-api-path-slug: mappings-json-get
      responses:
        200:
          description: OK
      tags:
      - Mappings
  /metrics:
    get:
      summary: Get Metrics
      description: Get metrics.
      operationId: getMetrics
      x-api-path-slug: metrics-get
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /metrics.json:
    get:
      summary: Get Metrics
      description: Get metrics.
      operationId: getMetrics.json
      x-api-path-slug: metrics-json-get
      responses:
        200:
          description: OK
      tags:
      - Metrics
  /metrics/{name}:
    get:
      summary: Get Metrics Name
      description: Get metrics name.
      operationId: getMetricsName
      x-api-path-slug: metricsname-get
      parameters:
      - in: path
        name: name
        description: name
      responses:
        200:
          description: OK
      tags:
      - Metrics
      - Name
  /orders:
    get:
      summary: Get Orders
      description: Get orders.
      operationId: getOrders
      x-api-path-slug: orders-get
      parameters:
      - in: query
        name: orderNumber
        description: orderNumber
      - in: query
        name: orderStatus
        description: orderStatus
      responses:
        200:
          description: OK
      tags:
      - Orders
  /orders/summary:
    get:
      summary: Get Orders Summary
      description: Get orders summary.
      operationId: getOrdersSummary
      x-api-path-slug: orderssummary-get
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Summary
  /orders/{orderId}:
    get:
      summary: Get Orders Orderid
      description: Get orders orderid.
      operationId: getOrdersOrder
      x-api-path-slug: ordersorderid-get
      parameters:
      - in: path
        name: orderId
        description: orderId
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Orderid
  /preview/**:
    get:
      summary: Get Preview **
      description: Get preview **.
      operationId: getPreview**
      x-api-path-slug: preview-get
      responses:
        200:
          description: OK
      tags:
      - Preview
      - '**'
    head:
      summary: Head Preview **
      description: Head preview **.
      operationId: headPreview**
      x-api-path-slug: preview-head
      responses:
        200:
          description: OK
      tags:
      - Head
      - Preview
      - '**'
    post:
      summary: Post Preview **
      description: Post preview **.
      operationId: postPreview**
      x-api-path-slug: preview-post
      responses:
        200:
          description: OK
      tags:
      - Preview
      - '**'
    put:
      summary: Put Preview **
      description: Put preview **.
      operationId: putPreview**
      x-api-path-slug: preview-put
      responses:
        200:
          description: OK
      tags:
      - Preview
      - '**'
    delete:
      summary: Delete Preview **
      description: Delete preview **.
      operationId: deletePreview**
      x-api-path-slug: preview-delete
      responses:
        200:
          description: OK
      tags:
      - Preview
      - '**'
    options:
      summary: Options Preview **
      description: Options preview **.
      operationId: optionsPreview**
      x-api-path-slug: preview-options
      responses:
        200:
          description: OK
      tags:
      - Options
      - Preview
      - '**'
    patch:
      summary: Patch Preview **
      description: Patch preview **.
      operationId: patchPreview**
      x-api-path-slug: preview-patch
      responses:
        200:
          description: OK
      tags:
      - Preview
      - '**'
  /promotion-messages/{productId}:
    get:
      summary: Get Promotion Messages
      description: Get promotion messages.
      operationId: getPromotionMessagesProduct
      x-api-path-slug: promotionmessagesproductid-get
      parameters:
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Promotion
      - Messages
  /ratings/{itemId}:
    get:
      summary: Get Ratings
      description: Get ratings.
      operationId: getRatingsItem
      x-api-path-slug: ratingsitemid-get
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: ratingType
        description: ratingType
      responses:
        200:
          description: OK
      tags:
      - Ratings
    head:
      summary: Head Ratings
      description: Head ratings.
      operationId: headRatingsItem
      x-api-path-slug: ratingsitemid-head
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: ratingType
        description: ratingType
      responses:
        200:
          description: OK
      tags:
      - Head
      - Ratings
    post:
      summary: Post Ratings
      description: Post ratings.
      operationId: postRatingsItem
      x-api-path-slug: ratingsitemid-post
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: ratingType
        description: ratingType
      responses:
        200:
          description: OK
      tags:
      - Ratings
    put:
      summary: Put Ratings
      description: Put ratings.
      operationId: putRatingsItem
      x-api-path-slug: ratingsitemid-put
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: ratingType
        description: ratingType
      responses:
        200:
          description: OK
      tags:
      - Ratings
    delete:
      summary: Delete Ratings
      description: Delete ratings.
      operationId: deleteRatingsItem
      x-api-path-slug: ratingsitemid-delete
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: ratingType
        description: ratingType
      responses:
        200:
          description: OK
      tags:
      - Ratings
    options:
      summary: Options Ratings
      description: Options ratings.
      operationId: optionsRatingsItem
      x-api-path-slug: ratingsitemid-options
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: ratingType
        description: ratingType
      responses:
        200:
          description: OK
      tags:
      - Options
      - Ratings
    patch:
      summary: Patch Ratings
      description: Patch ratings.
      operationId: patchRatingsItem
      x-api-path-slug: ratingsitemid-patch
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: ratingType
        description: ratingType
      responses:
        200:
          description: OK
      tags:
      - Ratings
  /related-products:
    get:
      summary: Get Related Products
      description: Get related products.
      operationId: getRelatedProducts
      x-api-path-slug: relatedproducts-get
      parameters:
      - in: query
        name: categoryId
        description: categoryId
      - in: query
        name: categoryKey
        description: categoryKey
      - in: query
        name: includePriceData
        description: includePriceData
      - in: query
        name: includePromotionMessages
        description: includePromotionMessages
      - in: query
        name: productId
        description: productId
      - in: query
        name: productKey
        description: productKey
      - in: query
        name: quantity
        description: quantity
      - in: query
        name: type
        description: type
      responses:
        200:
          description: OK
      tags:
      - Related
      - Products
  /shipping/options:
    get:
      summary: Get Shipping Options
      description: Get shipping options.
      operationId: getShippingOptions
      x-api-path-slug: shippingoptions-get
      parameters:
      - in: query
        name: fulfillmentType
        description: fulfillmentType
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Options
  /shipping/{cartId}/estimate:
    get:
      summary: Get Shipping Estimate
      description: Get shipping estimate.
      operationId: getShippingCartEstimate
      x-api-path-slug: shippingcartidestimate-get
      parameters:
      - in: path
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Estimate
    head:
      summary: Head Shipping Estimate
      description: Head shipping estimate.
      operationId: headShippingCartEstimate
      x-api-path-slug: shippingcartidestimate-head
      parameters:
      - in: path
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Head
      - Shipping
      - Estimate
    post:
      summary: Post Shipping Estimate
      description: Post shipping estimate.
      operationId: postShippingCartEstimate
      x-api-path-slug: shippingcartidestimate-post
      parameters:
      - in: path
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Estimate
    put:
      summary: Put Shipping Estimate
      description: Put shipping estimate.
      operationId: putShippingCartEstimate
      x-api-path-slug: shippingcartidestimate-put
      parameters:
      - in: path
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Estimate
    delete:
      summary: Delete Shipping Estimate
      description: Delete shipping estimate.
      operationId: deleteShippingCartEstimate
      x-api-path-slug: shippingcartidestimate-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Estimate
    options:
      summary: Options Shipping Estimate
      description: Options shipping estimate.
      operationId: optionsShippingCartEstimate
      x-api-path-slug: shippingcartidestimate-options
      parameters:
      - in: path
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Options
      - Shipping
      - Estimate
    patch:
      summary: Patch Shipping Estimate
      description: Patch shipping estimate.
      operationId: patchShippingCartEstimate
      x-api-path-slug: shippingcartidestimate-patch
      parameters:
      - in: path
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Estimate
  /shipping/{cartId}/group:
    post:
      summary: Post Shipping Group
      description: Post shipping group.
      operationId: postShippingCartGroup
      x-api-path-slug: shippingcartidgroup-post
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Group
  /shipping/{cartId}/group/{fulfillmentGroupId}:
    delete:
      summary: Delete Shipping Group Fulfillmentgroupid
      description: Delete shipping group fulfillmentgroupid.
      operationId: deleteShippingCartGroupFulfillmentgroup
      x-api-path-slug: shippingcartidgroupfulfillmentgroupid-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: path
        name: fulfillmentGroupId
        description: fulfillmentGroupId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Group
      - Fulfillmentgroupid
    patch:
      summary: Patch Shipping Group Fulfillmentgroupid
      description: Patch shipping group fulfillmentgroupid.
      operationId: patchShippingCartGroupFulfillmentgroup
      x-api-path-slug: shippingcartidgroupfulfillmentgroupid-patch
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: path
        name: fulfillmentGroupId
        description: fulfillmentGroupId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Group
      - Fulfillmentgroupid
  /shipping/{cartId}/group/{fulfillmentGroupId}/item:
    post:
      summary: Post Shipping Group Fulfillmentgroupid Item
      description: Post shipping group fulfillmentgroupid item.
      operationId: postShippingCartGroupFulfillmentgroupItem
      x-api-path-slug: shippingcartidgroupfulfillmentgroupiditem-post
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: path
        name: fulfillmentGroupId
        description: fulfillmentGroupId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Group
      - Fulfillmentgroupid
      - Item
  /shipping/{cartId}/group/{fulfillmentGroupId}/item/{itemId}:
    delete:
      summary: Delete Shipping Group Fulfillmentgroupid Item
      description: Delete shipping group fulfillmentgroupid item.
      operationId: deleteShippingCartGroupFulfillmentgroupItemItem
      x-api-path-slug: shippingcartidgroupfulfillmentgroupiditemitemid-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: path
        name: fulfillmentGroupId
        description: fulfillmentGroupId
      - in: path
        name: itemId
        description: itemId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Group
      - Fulfillmentgroupid
      - Item
  /shipping/{cartId}/group/{fulfillmentGroupId}/option/{fulfillmentOptionId}:
    put:
      summary: Put Shipping Group Fulfillmentgroupid Option Fulfillmentoptionid
      description: Put shipping group fulfillmentgroupid option fulfillmentoptionid.
      operationId: putShippingCartGroupFulfillmentgroupOptionFulfillmentoption
      x-api-path-slug: shippingcartidgroupfulfillmentgroupidoptionfulfillmentoptionid-put
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: path
        name: fulfillmentGroupId
        description: fulfillmentGroupId
      - in: path
        name: fulfillmentOptionId
        description: fulfillmentOptionId
      - in: query
        name: priceOrder
        description: priceOrder
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Group
      - Fulfillmentgroupid
      - Option
      - Fulfillmentoptionid
  /shipping/{cartId}/groups:
    get:
      summary: Get Shipping Groups
      description: Get shipping groups.
      operationId: getShippingCartGroups
      x-api-path-slug: shippingcartidgroups-get
      parameters:
      - in: path
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Groups
    delete:
      summary: Delete Shipping Groups
      description: Delete shipping groups.
      operationId: deleteShippingCartGroups
      x-api-path-slug: shippingcartidgroups-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: priceOrder
        description: priceOrder
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Groups
  /shipping/{cartId}/{fulfillmentGroupId}/address:
    put:
      summary: Put Shipping Fulfillmentgroupid Address
      description: Put shipping fulfillmentgroupid address.
      operationId: putShippingCartFulfillmentgroupAddress
      x-api-path-slug: shippingcartidfulfillmentgroupidaddress-put
      parameters:
      - in: body
        name: address
        description: address
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: cartId
        description: cartId
      - in: path
        name: fulfillmentGroupId
        description: fulfillmentGroupId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Fulfillmentgroupid
      - Ress
  /trace:
    get:
      summary: Get Trace
      description: Get trace.
      operationId: getTrace
      x-api-path-slug: trace-get
      responses:
        200:
          description: OK
      tags:
      - Trace
  /trace.json:
    get:
      summary: Get Trace
      description: Get trace.
      operationId: getTrace.json
      x-api-path-slug: trace-json-get
      responses:
        200:
          description: OK
      tags:
      - Trace
  /wishlist:
    get:
      summary: Get Wishlist
      description: Get wishlist.
      operationId: getWishlist
      x-api-path-slug: wishlist-get
      parameters:
      - in: query
        name: wishlistName
        description: wishlistName
      responses:
        200:
          description: OK
      tags:
      - Wishlist
    post:
      summary: Post Wishlist
      description: Post wishlist.
      operationId: postWishlist
      x-api-path-slug: wishlist-post
      parameters:
      - in: query
        name: wishlistName
        description: wishlistName
      responses:
        200:
          description: OK
      tags:
      - Wishlist
  /wishlist/configure-item:
    post:
      summary: Post Wishlist Configure Item
      description: Post wishlist configure item.
      operationId: postWishlistConfigureItem
      x-api-path-slug: wishlistconfigureitem-post
      parameters:
      - in: body
        name: orderItemWrapper
        description: orderItemWrapper
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: wishlistName
        description: wishlistName
      responses:
        200:
          description: OK
      tags:
      - Wishlist
      - Configure
      - Item
  /wishlist/item:
    post:
      summary: Post Wishlist Item
      description: Post wishlist item.
      operationId: postWishlistItem
      x-api-path-slug: wishlistitem-post
      parameters:
      - in: body
        name: orderItemWrapper
        description: orderItemWrapper
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: wishlistName
        description: wishlistName
      responses:
        200:
          description: OK
      tags:
      - Wishlist
      - Item
  /wishlist/items/{itemId}:
    put:
      summary: Put Wishlist Items
      description: Put wishlist items.
      operationId: putWishlistItemsItem
      x-api-path-slug: wishlistitemsitemid-put
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: quantity
        description: quantity
      - in: query
        name: wishlistName
        description: wishlistName
      responses:
        200:
          description: OK
      tags:
      - Wishlist
      - Items
    delete:
      summary: Delete Wishlist Items
      description: Delete wishlist items.
      operationId: deleteWishlistItemsItem
      x-api-path-slug: wishlistitemsitemid-delete
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: wishlistName
        description: wishlistName
      responses:
        200:
          description: OK
      tags:
      - Wishlist
      - Items
  /wishlist/items/{itemId}/move:
    post:
      summary: Post Wishlist Items Move
      description: Post wishlist items move.
      operationId: postWishlistItemsItemMove
      x-api-path-slug: wishlistitemsitemidmove-post
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: wishlistName
        description: wishlistName
      responses:
        200:
          description: OK
      tags:
      - Wishlist
      - Items
      - Move