swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /articles:
    get:
      summary: Get Articles
      description: Get articles.
      operationId: getArticles
      x-api-path-slug: articles-get
      parameters:
      - in: query
        name: exclude_featured
        description: Number of featured articles to exclude
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: query
        description: Whats being searched for
      responses:
        200:
          description: OK
      tags:
      - Articles
  /categories:
    get:
      summary: Get Categories
      description: List of supported product categories
      operationId: getCategories
      x-api-path-slug: categories-get
      responses:
        200:
          description: OK
      tags:
      - Categories
  /categories/flat:
    get:
      summary: Get Categories Flat
      description: Get categories flat.
      operationId: getCategoriesFlat
      x-api-path-slug: categoriesflat-get
      responses:
        200:
          description: OK
      tags:
      - Categories
      - Flat
  /categories/taxonomy:
    get:
      summary: Get Categories Taxonomy
      description: Full taxonomy tree of categories including middle categories
      operationId: getCategoriesTaxonomy
      x-api-path-slug: categoriestaxonomy-get
      responses:
        200:
          description: OK
      tags:
      - Categories
      - Taxonomy
  /categories/{product_type}/{category}:
    get:
      summary: Get Categories Product Type Category
      description: Get categories product type category.
      operationId: getCategoriesProductTypeCategory
      x-api-path-slug: categoriesproduct-typecategory-get
      parameters:
      - in: path
        name: category
      - in: path
        name: product_type
      responses:
        200:
          description: OK
      tags:
      - Categories
      - Product
      - Type
      - Category
  /categories/{uuid}:
    get:
      summary: Get Categories Uu
      description: Get category details
      operationId: getCategoriesUu
      x-api-path-slug: categoriesuuid-get
      parameters:
      - in: path
        name: uuid
      responses:
        200:
          description: OK
      tags:
      - Categories
      - Uuid
  /comparison_shopping_pages:
    get:
      summary: Get Comparison Shopping Pages
      description: Returns a set of comparison shopping pages based on the current
        params
      operationId: getComparisonShoppingPages
      x-api-path-slug: comparison-shopping-pages-get
      responses:
        200:
          description: OK
      tags:
      - Comparison
      - Shopping
      - Pages
  /comparison_shopping_pages/find:
    get:
      summary: Get Comparison Shopping Pages Find
      description: Get comparison shopping pages find.
      operationId: getComparisonShoppingPagesFind
      x-api-path-slug: comparison-shopping-pagesfind-get
      parameters:
      - in: query
        name: id
        description: ID of the comparison shopping page
      - in: query
        name: slug
        description: Slug of the comparison shopping page
      responses:
        200:
          description: OK
      tags:
      - Comparison
      - Shopping
      - Pages
      - Find
  /comparison_shopping_pages/{id}:
    get:
      summary: Get Comparison Shopping Pages
      description: Get comparison shopping pages.
      operationId: getComparisonShoppingPages
      x-api-path-slug: comparison-shopping-pagesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Comparison
      - Shopping
      - Pages
      - Id
  /comparison_shopping_pages/{id}/listings:
    get:
      summary: Get Comparison Shopping Pages Listings
      description: Return new or used listings for a comparison shopping page
      operationId: getComparisonShoppingPagesListings
      x-api-path-slug: comparison-shopping-pagesidlistings-get
      parameters:
      - in: query
        name: condition
        description: Condition of the listing
      - in: path
        name: id
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      responses:
        200:
          description: OK
      tags:
      - Comparison
      - Shopping
      - Pages
      - Id
      - Listings
  /comparison_shopping_pages/{id}/reviews:
    get:
      summary: Get Comparison Shopping Pages Reviews
      description: View reviews of a comparison shopping page
      operationId: getComparisonShoppingPagesReviews
      x-api-path-slug: comparison-shopping-pagesidreviews-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Comparison
      - Shopping
      - Pages
      - Id
      - Reviews
  /conversations/{conversation_id}/offer:
    post:
      summary: Post Conversations Conversation Offer
      description: Make an offer to the other participant in the conversation
      operationId: postConversationsConversationOffer
      x-api-path-slug: conversationsconversation-idoffer-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: conversation_id
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - Conversation
      - Id
      - Offer
  /conversations/{id}/offer:
    post:
      summary: Post Conversations Offer
      description: Make an offer to the other participant in the conversation
      operationId: postConversationsOffer
      x-api-path-slug: conversationsidoffer-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - Id
      - Offer
  /countries:
    get:
      summary: Get Countries
      description: Retrieve a list of country codes with corresponding subregions
      operationId: getCountries
      x-api-path-slug: countries-get
      responses:
        200:
          description: OK
      tags:
      - Countries
  /csps:
    get:
      summary: Get Csps
      description: Returns a set of comparison shopping pages based on the current
        params
      operationId: getCsps
      x-api-path-slug: csps-get
      responses:
        200:
          description: OK
      tags:
      - Csps
  /csps/categories:
    get:
      summary: Get Csps Categories
      description: Get csps categories.
      operationId: getCspsCategories
      x-api-path-slug: cspscategories-get
      responses:
        200:
          description: OK
      tags:
      - Csps
      - Categories
  /curated_sets/{slug}:
    get:
      summary: Get Curated Sets Slug
      description: Get curated sets slug.
      operationId: getCuratedSetsSlug
      x-api-path-slug: curated-setsslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Curated
      - Sets
      - Slug
  /currencies/display:
    get:
      summary: Get Currencies Display
      description: List of supported display currencies for browsing listings
      operationId: getCurrenciesDisplay
      x-api-path-slug: currenciesdisplay-get
      responses:
        200:
          description: OK
      tags:
      - Currencies
      - Display
  /currencies/listing:
    get:
      summary: Get Currencies Listing
      description: List of supported listing currencies for shops
      operationId: getCurrenciesListing
      x-api-path-slug: currencieslisting-get
      responses:
        200:
          description: OK
      tags:
      - Currencies
      - Listing
  /feedback/{feedback_id}:
    get:
      summary: Get Feedback Feedback
      description: Get feedback feedback.
      operationId: getFeedbackFeedback
      x-api-path-slug: feedbackfeedback-id-get
      parameters:
      - in: path
        name: feedback_id
      responses:
        200:
          description: OK
      tags:
      - Feedback
      - Feedback
      - Id
  /handpicked/{slug}:
    get:
      summary: Get Handpicked Slug
      description: Get results from a handpicked collection
      operationId: getHandpickedSlug
      x-api-path-slug: handpickedslug-get
      parameters:
      - in: query
        name: accepts_gift_cards
        description: If true, include only items that accept gift cards
      - in: query
        name: accepts_payment_plans
        description: If true, only show items that can be purchased with a payment
          plan
      - in: query
        name: auction_price_max
        description: Maximum current auction price
      - in: query
        name: category
        description: Category slug from /api/categories
      - in: query
        name: conditions
        description: 'Condition: all,new,b-stock,used,non-functioning'
      - in: query
        name: currency
        description: The currency to be used for the price filters
      - in: query
        name: decade
        description: 'Decade: e'
      - in: query
        name: exclude_auctions
        description: If true, exclude auctions
      - in: query
        name: finish
        description: Visual finish of the item, common for guitars
      - in: query
        name: handmade
        description: Handmade items only
      - in: query
        name: item_city
        description: City where item is located
      - in: query
        name: item_country
        description: DEPRECATED - Country code where item is located
      - in: query
        name: item_region
        description: Country code where item is located
      - in: query
        name: item_state
        description: State or region code where item is located
      - in: query
        name: listing_type
        description: 'Type of listing: auctions,offers'
      - in: query
        name: make
        description: Make(s)/brand of item (e
      - in: query
        name: model
        description: Model of item (e
      - in: query
        name: must_not
        description: Search term negation
      - in: query
        name: not_ids
        description: Listing ID negation
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: preferred_seller
        description: If true, include only items by Reverb Preferred Sellers
      - in: query
        name: price_max
        description: Maximum price of search results (USD)
      - in: query
        name: price_min
        description: Minimum price of search results (USD)
      - in: query
        name: product_type
        description: Product type slug from /api/categories
      - in: query
        name: query
        description: Search query
      - in: query
        name: ships_to
        description: Limit search to items that ship to this country code
      - in: query
        name: shop
        description: Slug of shop to search
      - in: query
        name: shop_id
        description: ID of shop to search
      - in: path
        name: slug
      - in: query
        name: watchers_count_min
        description: Minimum number of watchers (used to find popular items)
      - in: query
        name: year_max
        description: Maximum year of manufacture
      - in: query
        name: year_min
        description: Minumum year of manufacture
      responses:
        200:
          description: OK
      tags:
      - Handpicked
      - Slug
  /listing_conditions:
    get:
      summary: Get Listing Conditions
      description: List of supported product conditions
      operationId: getListingConditions
      x-api-path-slug: listing-conditions-get
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Conditions
  /listings:
    get:
      summary: Get Listings
      description: Default search of listings includes only used & handmade. Add a
        filter to view all listings or use the /listings/all endpoint.
      operationId: getListings
      x-api-path-slug: listings-get
      parameters:
      - in: query
        name: accepts_gift_cards
        description: If true, include only items that accept gift cards
      - in: query
        name: accepts_payment_plans
        description: If true, only show items that can be purchased with a payment
          plan
      - in: query
        name: auction_price_max
        description: Maximum current auction price
      - in: query
        name: category
        description: Category slug from /api/categories
      - in: query
        name: conditions
        description: 'Condition: all,new,b-stock,used,non-functioning'
      - in: query
        name: currency
        description: The currency to be used for the price filters
      - in: query
        name: decade
        description: 'Decade: e'
      - in: query
        name: exclude_auctions
        description: If true, exclude auctions
      - in: query
        name: finish
        description: Visual finish of the item, common for guitars
      - in: query
        name: handmade
        description: Handmade items only
      - in: query
        name: item_city
        description: City where item is located
      - in: query
        name: item_country
        description: DEPRECATED - Country code where item is located
      - in: query
        name: item_region
        description: Country code where item is located
      - in: query
        name: item_state
        description: State or region code where item is located
      - in: query
        name: listing_type
        description: 'Type of listing: auctions,offers'
      - in: query
        name: make
        description: Make(s)/brand of item (e
      - in: query
        name: model
        description: Model of item (e
      - in: query
        name: must_not
        description: Search term negation
      - in: query
        name: not_ids
        description: Listing ID negation
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: preferred_seller
        description: If true, include only items by Reverb Preferred Sellers
      - in: query
        name: price_max
        description: Maximum price of search results (USD)
      - in: query
        name: price_min
        description: Minimum price of search results (USD)
      - in: query
        name: product_type
        description: Product type slug from /api/categories
      - in: query
        name: query
        description: Search query
      - in: query
        name: ships_to
        description: Limit search to items that ship to this country code
      - in: query
        name: shop
        description: Slug of shop to search
      - in: query
        name: shop_id
        description: ID of shop to search
      - in: query
        name: watchers_count_min
        description: Minimum number of watchers (used to find popular items)
      - in: query
        name: year_max
        description: Maximum year of manufacture
      - in: query
        name: year_min
        description: Minumum year of manufacture
      responses:
        200:
          description: OK
      tags:
      - Listings
    post:
      summary: Post Listings
      description: Create a listing
      operationId: postListings
      x-api-path-slug: listings-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Listings
  /listings/all:
    get:
      summary: Get Listings All
      description: All listings including used, handmade, and brand new
      operationId: getListingsAll
      x-api-path-slug: listingsall-get
      parameters:
      - in: query
        name: accepts_gift_cards
        description: If true, include only items that accept gift cards
      - in: query
        name: accepts_payment_plans
        description: If true, only show items that can be purchased with a payment
          plan
      - in: query
        name: auction_price_max
        description: Maximum current auction price
      - in: query
        name: category
        description: Category slug from /api/categories
      - in: query
        name: conditions
        description: 'Condition: all,new,b-stock,used,non-functioning'
      - in: query
        name: currency
        description: The currency to be used for the price filters
      - in: query
        name: decade
        description: 'Decade: e'
      - in: query
        name: exclude_auctions
        description: If true, exclude auctions
      - in: query
        name: finish
        description: Visual finish of the item, common for guitars
      - in: query
        name: handmade
        description: Handmade items only
      - in: query
        name: item_city
        description: City where item is located
      - in: query
        name: item_country
        description: DEPRECATED - Country code where item is located
      - in: query
        name: item_region
        description: Country code where item is located
      - in: query
        name: item_state
        description: State or region code where item is located
      - in: query
        name: listing_type
        description: 'Type of listing: auctions,offers'
      - in: query
        name: make
        description: Make(s)/brand of item (e
      - in: query
        name: model
        description: Model of item (e
      - in: query
        name: must_not
        description: Search term negation
      - in: query
        name: not_ids
        description: Listing ID negation
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: preferred_seller
        description: If true, include only items by Reverb Preferred Sellers
      - in: query
        name: price_max
        description: Maximum price of search results (USD)
      - in: query
        name: price_min
        description: Minimum price of search results (USD)
      - in: query
        name: product_type
        description: Product type slug from /api/categories
      - in: query
        name: query
        description: Search query
      - in: query
        name: ships_to
        description: Limit search to items that ship to this country code
      - in: query
        name: shop
        description: Slug of shop to search
      - in: query
        name: shop_id
        description: ID of shop to search
      - in: query
        name: watchers_count_min
        description: Minimum number of watchers (used to find popular items)
      - in: query
        name: year_max
        description: Maximum year of manufacture
      - in: query
        name: year_min
        description: Minumum year of manufacture
      responses:
        200:
          description: OK
      tags:
      - Listings
  /listings/facets/seller_location:
    get:
      summary: Get Listings Facets Seller Location
      description: Get listings facets seller location.
      operationId: getListingsFacetsSellerLocation
      x-api-path-slug: listingsfacetsseller-location-get
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Facets
      - Seller
      - Location
  /listings/{id}/negotiation:
    get:
      summary: Get Listings Negotiation
      description: Returns the latest negotiation for the requesting user given a
        listing id
      operationId: getListingsNegotiation
      x-api-path-slug: listingsidnegotiation-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Id
      - Negotiation
  /listings/{id}/offer:
    post:
      summary: Post Listings Offer
      description: Make an offer to the seller of a listing
      operationId: postListingsOffer
      x-api-path-slug: listingsidoffer-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Id
      - Offer
  /listings/{listing_id}/bump:
    get:
      summary: Get Listings Listing Bump
      description: View available bump tiers and stats for a listing
      operationId: getListingsListingBump
      x-api-path-slug: listingslisting-idbump-get
      parameters:
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Bump
  /listings/{listing_id}/bump/{budget_type}:
    post:
      summary: Post Listings Listing Bump Budget Type
      description: Post listings listing bump budget type.
      operationId: postListingsListingBumpBudgetType
      x-api-path-slug: listingslisting-idbumpbudget-type-post
      parameters:
      - in: path
        name: budget_type
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Bump
      - Budget
      - Type
  /listings/{listing_id}/conversations:
    post:
      summary: Post Listings Listing Conversations
      description: Post listings listing conversations.
      operationId: postListingsListingConversations
      x-api-path-slug: listingslisting-idconversations-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Conversations
  /listings/{listing_id}/images:
    get:
      summary: Get Listings Listing Images
      description: View the images associated with a particular listing
      operationId: getListingsListingImages
      x-api-path-slug: listingslisting-idimages-get
      parameters:
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Images
  /listings/{listing_id}/images/{image_id}:
    delete:
      summary: Delete Listings Listing Images Image
      description: Delete listings listing images image.
      operationId: deleteListingsListingImagesImage
      x-api-path-slug: listingslisting-idimagesimage-id-delete
      parameters:
      - in: path
        name: image_id
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Images
      - Image
      - Id
  /listings/{listing_id}/product_bundle:
    get:
      summary: Get Listings Listing Product Bundle
      description: Find a product bundle attached to a listing
      operationId: getListingsListingProductBundle
      x-api-path-slug: listingslisting-idproduct-bundle-get
      parameters:
      - in: query
        name: for_seller
        description: Pass to see non-live bundles as the seller
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Product
      - Bundle
  /listings/{listing_id}/sales:
    get:
      summary: Get Listings Listing Sales
      description: See all sales that include a listing.
      operationId: getListingsListingSales
      x-api-path-slug: listingslisting-idsales-get
      parameters:
      - in: path
        name: listing_id
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Listing
      - Id
      - Sales
  /listings/{slug}:
    delete:
      summary: Delete Listings Slug
      description: Delete a draft listing. Cannot be used on non-drafts.
      operationId: deleteListingsSlug
      x-api-path-slug: listingsslug-delete
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
    get:
      summary: Get Listings Slug
      description: Get listings slug.
      operationId: getListingsSlug
      x-api-path-slug: listingsslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
    put:
      summary: Put Listings Slug
      description: Put listings slug.
      operationId: putListingsSlug
      x-api-path-slug: listingsslug-put
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
  /listings/{slug}/edit:
    get:
      summary: Get Listings Slug Edit
      description: Get listings slug edit.
      operationId: getListingsSlugEdit
      x-api-path-slug: listingsslugedit-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
      - Edit
  /listings/{slug}/flag:
    post:
      summary: Post Listings Slug Flag
      description: Flag a listing for inappropriate content or fraud
      operationId: postListingsSlugFlag
      x-api-path-slug: listingsslugflag-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
      - Flag
  /listings/{slug}/reviews:
    get:
      summary: Get Listings Slug Reviews
      description: Get listings slug reviews.
      operationId: getListingsSlugReviews
      x-api-path-slug: listingsslugreviews-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
      - Reviews
    post:
      summary: Post Listings Slug Reviews
      description: Create a review for a listing
      operationId: postListingsSlugReviews
      x-api-path-slug: listingsslugreviews-post
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
      - Reviews
  /listings/{slug}/similar_listings:
    get:
      summary: Get Listings Slug Similar Listings
      description: Get listings slug similar listings.
      operationId: getListingsSlugSimilarListings
      x-api-path-slug: listingsslugsimilar-listings-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Listings
      - Slug
      - Similar
      - Listings
  /my/account:
    get:
      summary: Get My Account
      description: Get account details
      operationId: getMyAccount
      x-api-path-slug: myaccount-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Account
    put:
      summary: Put My Account
      description: Update account details
      operationId: putMyAccount
      x-api-path-slug: myaccount-put
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - My
      - Account
  /my/addresses:
    get:
      summary: Get My Addresses
      description: See all addresses in your address book
      operationId: getMyAddresses
      x-api-path-slug: myaddresses-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Addresses
    post:
      summary: Post My Addresses
      description: Create a new address in your address book
      operationId: postMyAddresses
      x-api-path-slug: myaddresses-post
      responses:
        200:
          description: OK
      tags:
      - My
      - Addresses
  /my/addresses/{address_id}:
    delete:
      summary: Delete My Addresses Address
      description: Delete an existing address in your address book
      operationId: deleteMyAddressesAddress
      x-api-path-slug: myaddressesaddress-id-delete
      parameters:
      - in: path
        name: address_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Addresses
      - Address
      - Id
    put:
      summary: Put My Addresses Address
      description: Update an existing address in your address book
      operationId: putMyAddressesAddress
      x-api-path-slug: myaddressesaddress-id-put
      parameters:
      - in: path
        name: address_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Addresses
      - Address
      - Id
  /my/conversations:
    get:
      summary: Get My Conversations
      description: Get a list of your conversations
      operationId: getMyConversations
      x-api-path-slug: myconversations-get
      parameters:
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: search
        description: Query string to search conversations by
      - in: query
        name: unread_only
        description: Show unread conversations only
      responses:
        200:
          description: OK
      tags:
      - My
      - Conversations
    post:
      summary: Post My Conversations
      description: Post my conversations.
      operationId: postMyConversations
      x-api-path-slug: myconversations-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - My
      - Conversations
  /my/conversations/{conversation_id}/messages:
    post:
      summary: Post My Conversations Conversation Messages
      description: Post my conversations conversation messages.
      operationId: postMyConversationsConversationMessages
      x-api-path-slug: myconversationsconversation-idmessages-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: conversation_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Conversations
      - Conversation
      - Id
      - Messages
  /my/conversations/{id}:
    get:
      summary: Get My Conversations
      description: Display conversation details with messages in natural time order
        (oldest to newest)
      operationId: getMyConversations
      x-api-path-slug: myconversationsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Conversations
      - Id
    put:
      summary: Put My Conversations
      description: Mark a conversation read/unread
      operationId: putMyConversations
      x-api-path-slug: myconversationsid-put
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Conversations
      - Id
  /my/counts:
    get:
      summary: Get My Counts
      description: Get your actionable status counts
      operationId: getMyCounts
      x-api-path-slug: mycounts-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Counts
  /my/curated_set/product/{product_id}:
    delete:
      summary: Delete My Curated Set Product Product
      description: Delete my curated set product product.
      operationId: deleteMyCuratedSetProductProduct
      x-api-path-slug: mycurated-setproductproduct-id-delete
      parameters:
      - in: path
        name: product_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Curated
      - Set
      - Product
      - Product
      - Id
    post:
      summary: Post My Curated Set Product Product
      description: Post my curated set product product.
      operationId: postMyCuratedSetProductProduct
      x-api-path-slug: mycurated-setproductproduct-id-post
      parameters:
      - in: path
        name: product_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Curated
      - Set
      - Product
      - Product
      - Id
  /my/feed:
    get:
      summary: Get My Feed
      description: Get listings from your feed
      operationId: getMyFeed
      x-api-path-slug: myfeed-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Feed
  /my/feed/customize:
    get:
      summary: Get My Feed Customize
      description: get your feed customization options
      operationId: getMyFeedCustomize
      x-api-path-slug: myfeedcustomize-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Feed
      - Customize
  /my/feed/grid:
    get:
      summary: Get My Feed Gr
      description: Get my feed gr.
      operationId: getMyFeedGr
      x-api-path-slug: myfeedgrid-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Feed
      - Grid
  /my/feedback/received:
    get:
      summary: Get My Feedback Received
      description: List of received feedback
      operationId: getMyFeedbackReceived
      x-api-path-slug: myfeedbackreceived-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Feedback
      - Received
  /my/feedback/sent:
    get:
      summary: Get My Feedback Sent
      description: List of sent feedback
      operationId: getMyFeedbackSent
      x-api-path-slug: myfeedbacksent-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Feedback
      - Sent
  /my/follows:
    get:
      summary: Get My Follows
      description: See what the user is following
      operationId: getMyFollows
      x-api-path-slug: myfollows-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
  /my/follows/articles:
    get:
      summary: Get My Follows Articles
      description: Returns a user's ArticleCategoryFollows
      operationId: getMyFollowsArticles
      x-api-path-slug: myfollowsarticles-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Articles
    post:
      summary: Post My Follows Articles
      description: Set a user's ArticleCategoryFollows
      operationId: postMyFollowsArticles
      x-api-path-slug: myfollowsarticles-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Articles
  /my/follows/brands/{slug}:
    delete:
      summary: Delete My Follows Brands Slug
      description: Delete my follows brands slug.
      operationId: deleteMyFollowsBrandsSlug
      x-api-path-slug: myfollowsbrandsslug-delete
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Brands
      - Slug
    get:
      summary: Get My Follows Brands Slug
      description: Get my follows brands slug.
      operationId: getMyFollowsBrandsSlug
      x-api-path-slug: myfollowsbrandsslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Brands
      - Slug
    post:
      summary: Post My Follows Brands Slug
      description: Post my follows brands slug.
      operationId: postMyFollowsBrandsSlug
      x-api-path-slug: myfollowsbrandsslug-post
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Brands
      - Slug
  /my/follows/categories/{category}/{subcategory}:
    delete:
      summary: Delete My Follows Categories Category Subcategory
      description: Delete my follows categories category subcategory.
      operationId: deleteMyFollowsCategoriesCategorySubcategory
      x-api-path-slug: myfollowscategoriescategorysubcategory-delete
      parameters:
      - in: path
        name: category
      - in: path
        name: subcategory
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Categories
      - Category
      - Subcategory
    get:
      summary: Get My Follows Categories Category Subcategory
      description: Get my follows categories category subcategory.
      operationId: getMyFollowsCategoriesCategorySubcategory
      x-api-path-slug: myfollowscategoriescategorysubcategory-get
      parameters:
      - in: path
        name: category
      - in: path
        name: subcategory
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Categories
      - Category
      - Subcategory
    post:
      summary: Post My Follows Categories Category Subcategory
      description: Post my follows categories category subcategory.
      operationId: postMyFollowsCategoriesCategorySubcategory
      x-api-path-slug: myfollowscategoriescategorysubcategory-post
      parameters:
      - in: path
        name: category
      - in: path
        name: subcategory
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Categories
      - Category
      - Subcategory
  /my/follows/categories/{identifier}:
    delete:
      summary: Delete My Follows Categories Entifier
      description: Delete my follows categories entifier.
      operationId: deleteMyFollowsCategoriesEntifier
      x-api-path-slug: myfollowscategoriesidentifier-delete
      parameters:
      - in: path
        name: identifier
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Categories
      - Identifier
    get:
      summary: Get My Follows Categories Entifier
      description: Get my follows categories entifier.
      operationId: getMyFollowsCategoriesEntifier
      x-api-path-slug: myfollowscategoriesidentifier-get
      parameters:
      - in: path
        name: identifier
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Categories
      - Identifier
    post:
      summary: Post My Follows Categories Entifier
      description: Post my follows categories entifier.
      operationId: postMyFollowsCategoriesEntifier
      x-api-path-slug: myfollowscategoriesidentifier-post
      parameters:
      - in: path
        name: identifier
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Categories
      - Identifier
  /my/follows/collections/{slug}:
    delete:
      summary: Delete My Follows Collections Slug
      description: Delete my follows collections slug.
      operationId: deleteMyFollowsCollectionsSlug
      x-api-path-slug: myfollowscollectionsslug-delete
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Collections
      - Slug
    get:
      summary: Get My Follows Collections Slug
      description: Get my follows collections slug.
      operationId: getMyFollowsCollectionsSlug
      x-api-path-slug: myfollowscollectionsslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Collections
      - Slug
    post:
      summary: Post My Follows Collections Slug
      description: Post my follows collections slug.
      operationId: postMyFollowsCollectionsSlug
      x-api-path-slug: myfollowscollectionsslug-post
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Collections
      - Slug
  /my/follows/handpicked/{slug}:
    delete:
      summary: Delete My Follows Handpicked Slug
      description: Delete my follows handpicked slug.
      operationId: deleteMyFollowsHandpickedSlug
      x-api-path-slug: myfollowshandpickedslug-delete
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Handpicked
      - Slug
    get:
      summary: Get My Follows Handpicked Slug
      description: Follow status for a handpicked collection
      operationId: getMyFollowsHandpickedSlug
      x-api-path-slug: myfollowshandpickedslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Handpicked
      - Slug
    post:
      summary: Post My Follows Handpicked Slug
      description: Post my follows handpicked slug.
      operationId: postMyFollowsHandpickedSlug
      x-api-path-slug: myfollowshandpickedslug-post
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Handpicked
      - Slug
  /my/follows/search:
    get:
      summary: Get My Follows Search
      description: Follow status for a search
      operationId: getMyFollowsSearch
      x-api-path-slug: myfollowssearch-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Search
    post:
      summary: Post My Follows Search
      description: Post my follows search.
      operationId: postMyFollowsSearch
      x-api-path-slug: myfollowssearch-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Search
  /my/follows/shops/{slug}:
    delete:
      summary: Delete My Follows Shops Slug
      description: Delete my follows shops slug.
      operationId: deleteMyFollowsShopsSlug
      x-api-path-slug: myfollowsshopsslug-delete
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Shops
      - Slug
    get:
      summary: Get My Follows Shops Slug
      description: Get my follows shops slug.
      operationId: getMyFollowsShopsSlug
      x-api-path-slug: myfollowsshopsslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Shops
      - Slug
    post:
      summary: Post My Follows Shops Slug
      description: Post my follows shops slug.
      operationId: postMyFollowsShopsSlug
      x-api-path-slug: myfollowsshopsslug-post
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Shops
      - Slug
  /my/follows/{follow_id}:
    delete:
      summary: Delete My Follows Follow
      description: Delete my follows follow.
      operationId: deleteMyFollowsFollow
      x-api-path-slug: myfollowsfollow-id-delete
      parameters:
      - in: path
        name: follow_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Follow
      - Id
  /my/follows/{follow_id}/alert:
    delete:
      summary: Delete My Follows Follow Alert
      description: Delete my follows follow alert.
      operationId: deleteMyFollowsFollowAlert
      x-api-path-slug: myfollowsfollow-idalert-delete
      parameters:
      - in: path
        name: follow_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Follow
      - Id
      - Alert
    post:
      summary: Post My Follows Follow Alert
      description: Post my follows follow alert.
      operationId: postMyFollowsFollowAlert
      x-api-path-slug: myfollowsfollow-idalert-post
      parameters:
      - in: path
        name: follow_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Follow
      - Id
      - Alert
  /my/listings:
    get:
      summary: Get My Listings
      description: Retrieve a list of live listings for the seller. To search all
        listings specify state=all
      operationId: getMyListings
      x-api-path-slug: mylistings-get
      parameters:
      - in: query
        name: accepts_gift_cards
        description: If true, include only items that accept gift cards
      - in: query
        name: accepts_payment_plans
        description: If true, only show items that can be purchased with a payment
          plan
      - in: query
        name: auction_price_max
        description: Maximum current auction price
      - in: query
        name: category
        description: Category slug from /api/categories
      - in: query
        name: conditions
        description: 'Condition: all,new,b-stock,used,non-functioning'
      - in: query
        name: currency
        description: The currency to be used for the price filters
      - in: query
        name: decade
        description: 'Decade: e'
      - in: query
        name: exclude_auctions
        description: If true, exclude auctions
      - in: query
        name: finish
        description: Visual finish of the item, common for guitars
      - in: query
        name: handmade
        description: Handmade items only
      - in: query
        name: item_city
        description: City where item is located
      - in: query
        name: item_country
        description: DEPRECATED - Country code where item is located
      - in: query
        name: item_region
        description: Country code where item is located
      - in: query
        name: item_state
        description: State or region code where item is located
      - in: query
        name: listing_type
        description: 'Type of listing: auctions,offers'
      - in: query
        name: make
        description: Make(s)/brand of item (e
      - in: query
        name: model
        description: Model of item (e
      - in: query
        name: must_not
        description: Search term negation
      - in: query
        name: not_ids
        description: Listing ID negation
      - in: query
        name: preferred_seller
        description: If true, include only items by Reverb Preferred Sellers
      - in: query
        name: price_max
        description: Maximum price of search results (USD)
      - in: query
        name: price_min
        description: Minimum price of search results (USD)
      - in: query
        name: product_type
        description: Product type slug from /api/categories
      - in: query
        name: query
        description: Search query
      - in: query
        name: ships_to
        description: Limit search to items that ship to this country code
      - in: query
        name: shop
        description: Slug of shop to search
      - in: query
        name: shop_id
        description: ID of shop to search
      - in: query
        name: sku
        description: Find a listing by sku
      - in: query
        name: state
        description: 'Available: [all, draft, ended, live, ordered, sold_out, suspended,
          seller_unavailable]'
      - in: query
        name: watchers_count_min
        description: Minimum number of watchers (used to find popular items)
      - in: query
        name: year_max
        description: Maximum year of manufacture
      - in: query
        name: year_min
        description: Minumum year of manufacture
      responses:
        200:
          description: OK
      tags:
      - My
      - Listings
  /my/listings/drafts:
    get:
      summary: Get My Listings Drafts
      description: Retrieve a list your draft listings
      operationId: getMyListingsDrafts
      x-api-path-slug: mylistingsdrafts-get
      parameters:
      - in: query
        name: accepts_gift_cards
        description: If true, include only items that accept gift cards
      - in: query
        name: accepts_payment_plans
        description: If true, only show items that can be purchased with a payment
          plan
      - in: query
        name: auction_price_max
        description: Maximum current auction price
      - in: query
        name: category
        description: Category slug from /api/categories
      - in: query
        name: conditions
        description: 'Condition: all,new,b-stock,used,non-functioning'
      - in: query
        name: currency
        description: The currency to be used for the price filters
      - in: query
        name: decade
        description: 'Decade: e'
      - in: query
        name: exclude_auctions
        description: If true, exclude auctions
      - in: query
        name: finish
        description: Visual finish of the item, common for guitars
      - in: query
        name: handmade
        description: Handmade items only
      - in: query
        name: item_city
        description: City where item is located
      - in: query
        name: item_country
        description: DEPRECATED - Country code where item is located
      - in: query
        name: item_region
        description: Country code where item is located
      - in: query
        name: item_state
        description: State or region code where item is located
      - in: query
        name: listing_type
        description: 'Type of listing: auctions,offers'
      - in: query
        name: make
        description: Make(s)/brand of item (e
      - in: query
        name: model
        description: Model of item (e
      - in: query
        name: must_not
        description: Search term negation
      - in: query
        name: not_ids
        description: Listing ID negation
      - in: query
        name: preferred_seller
        description: If true, include only items by Reverb Preferred Sellers
      - in: query
        name: price_max
        description: Maximum price of search results (USD)
      - in: query
        name: price_min
        description: Minimum price of search results (USD)
      - in: query
        name: product_type
        description: Product type slug from /api/categories
      - in: query
        name: query
        description: Search query
      - in: query
        name: ships_to
        description: Limit search to items that ship to this country code
      - in: query
        name: shop
        description: Slug of shop to search
      - in: query
        name: shop_id
        description: ID of shop to search
      - in: query
        name: watchers_count_min
        description: Minimum number of watchers (used to find popular items)
      - in: query
        name: year_max
        description: Maximum year of manufacture
      - in: query
        name: year_min
        description: Minumum year of manufacture
      responses:
        200:
          description: OK
      tags:
      - My
      - Listings
      - Drafts
  /my/listings/negotiations:
    get:
      summary: Get My Listings Negotiations
      description: Get a list of active negotiations as a seller
      operationId: getMyListingsNegotiations
      x-api-path-slug: mylistingsnegotiations-get
      parameters:
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      responses:
        200:
          description: OK
      tags:
      - My
      - Listings
      - Negotiations
  /my/listings/{slug}/state/end:
    put:
      summary: Put My Listings Slug State End
      description: Put my listings slug state end.
      operationId: putMyListingsSlugStateEnd
      x-api-path-slug: mylistingsslugstateend-put
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - My
      - Listings
      - Slug
      - State
      - End
  /my/lists:
    get:
      summary: Get My Lists
      description: Get a list of your lists (wishlist, watch list, etc)
      operationId: getMyLists
      x-api-path-slug: mylists-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Lists
  /my/negotiations/buying:
    get:
      summary: Get My Negotiations Buying
      description: Get a list of active negotiations as a buyer
      operationId: getMyNegotiationsBuying
      x-api-path-slug: mynegotiationsbuying-get
      parameters:
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      responses:
        200:
          description: OK
      tags:
      - My
      - Negotiations
      - Buying
  /my/negotiations/{id}:
    get:
      summary: Get My Negotiations
      description: Get my negotiations.
      operationId: getMyNegotiations
      x-api-path-slug: mynegotiationsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Negotiations
      - Id
  /my/negotiations/{id}/accept:
    post:
      summary: Post My Negotiations Accept
      description: Post my negotiations accept.
      operationId: postMyNegotiationsAccept
      x-api-path-slug: mynegotiationsidaccept-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Negotiations
      - Id
      - Accept
  /my/negotiations/{id}/counter:
    post:
      summary: Post My Negotiations Counter
      description: Post my negotiations counter.
      operationId: postMyNegotiationsCounter
      x-api-path-slug: mynegotiationsidcounter-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Negotiations
      - Id
      - Counter
  /my/negotiations/{id}/decline:
    post:
      summary: Post My Negotiations Decline
      description: Post my negotiations decline.
      operationId: postMyNegotiationsDecline
      x-api-path-slug: mynegotiationsiddecline-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Negotiations
      - Id
      - Decline
  /my/orders/awaiting_feedback:
    get:
      summary: Get My Orders Awaiting Feedback
      description: List of orders that need feedback
      operationId: getMyOrdersAwaitingFeedback
      x-api-path-slug: myordersawaiting-feedback-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Awaiting
      - Feedback
  /my/orders/buying/all:
    get:
      summary: Get My Orders Buying All
      description: Returns all orders, newest first.
      operationId: getMyOrdersBuyingAll
      x-api-path-slug: myordersbuyingall-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Buying
  /my/orders/buying/unpaid:
    get:
      summary: Get My Orders Buying Unpa
      description: Returns unpaid orders, newest first.
      operationId: getMyOrdersBuyingUnpa
      x-api-path-slug: myordersbuyingunpaid-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Buying
      - Unpaid
  /my/orders/buying/{id}:
    get:
      summary: Get My Orders Buying
      description: Returns order details for a buyer
      operationId: getMyOrdersBuying
      x-api-path-slug: myordersbuyingid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Buying
      - Id
  /my/orders/buying/{id}/mark_received:
    post:
      summary: Post My Orders Buying Mark Received
      description: Marks an order as received by the buyer
      operationId: postMyOrdersBuyingMarkReceived
      x-api-path-slug: myordersbuyingidmark-received-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Buying
      - Id
      - Mark
      - Received
  /my/orders/selling/all:
    get:
      summary: Get My Orders Selling All
      description: Get all seller orders, newest first.
      operationId: getMyOrdersSellingAll
      x-api-path-slug: myorderssellingall-get
      parameters:
      - in: query
        name: created_end_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: created_start_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: updated_end_date
        description: Filter by date modified in ISO8601 format - e
      - in: query
        name: updated_start_date
        description: Filter by date modified in ISO8601 format - e
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
  /my/orders/selling/awaiting_shipment:
    get:
      summary: Get My Orders Selling Awaiting Shipment
      description: Get seller orders awaiting shipment, newest first.
      operationId: getMyOrdersSellingAwaitingShipment
      x-api-path-slug: myorderssellingawaiting-shipment-get
      parameters:
      - in: query
        name: created_end_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: created_start_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: updated_end_date
        description: Filter by date modified in ISO8601 format - e
      - in: query
        name: updated_start_date
        description: Filter by date modified in ISO8601 format - e
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Awaiting
      - Shipment
  /my/orders/selling/buyer_history/{buyer_id}:
    get:
      summary: Get My Orders Selling Buyer History Buyer
      description: Get my orders selling buyer history buyer.
      operationId: getMyOrdersSellingBuyerHistoryBuyer
      x-api-path-slug: myorderssellingbuyer-historybuyer-id-get
      parameters:
      - in: path
        name: buyer_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Buyer
      - History
      - Buyer
      - Id
  /my/orders/selling/unpaid:
    get:
      summary: Get My Orders Selling Unpa
      description: Get unpaid seller orders, newest first.
      operationId: getMyOrdersSellingUnpa
      x-api-path-slug: myorderssellingunpaid-get
      parameters:
      - in: query
        name: created_end_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: created_start_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: updated_end_date
        description: Filter by date modified in ISO8601 format - e
      - in: query
        name: updated_start_date
        description: Filter by date modified in ISO8601 format - e
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Unpaid
  /my/orders/selling/{id}:
    get:
      summary: Get My Orders Selling
      description: Returns order details for a seller
      operationId: getMyOrdersSelling
      x-api-path-slug: myorderssellingid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Id
  /my/orders/selling/{id}/mark_picked_up:
    post:
      summary: Post My Orders Selling Mark Picked Up
      description: Post my orders selling mark picked up.
      operationId: postMyOrdersSellingMarkPickedUp
      x-api-path-slug: myorderssellingidmark-picked-up-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Id
      - Mark
      - Picked
      - Up
  /my/orders/selling/{id}/ship:
    post:
      summary: Post My Orders Selling Ship
      description: Post my orders selling ship.
      operationId: postMyOrdersSellingShip
      x-api-path-slug: myorderssellingidship-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Id
      - Ship
  /my/orders/selling/{order_id}/refund_requests:
    post:
      summary: Post My Orders Selling Order Refund Requests
      description: Post my orders selling order refund requests.
      operationId: postMyOrdersSellingOrderRefundRequests
      x-api-path-slug: myorderssellingorder-idrefund-requests-post
      parameters:
      - in: path
        name: order_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Order
      - Id
      - Refund
      - Requests
  /my/payments/selling:
    get:
      summary: Get My Payments Selling
      description: Get my payments selling.
      operationId: getMyPaymentsSelling
      x-api-path-slug: mypaymentsselling-get
      parameters:
      - in: query
        name: created_end_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: created_start_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: offset
      - in: query
        name: order_id
        description: Look up payments by order id
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: updated_end_date
        description: Filter by date modified in ISO8601 format - e
      - in: query
        name: updated_start_date
        description: Filter by date modified in ISO8601 format - e
      responses:
        200:
          description: OK
      tags:
      - My
      - Payments
      - Selling
  /my/payments/selling/{id}:
    get:
      summary: Get My Payments Selling
      description: Get my payments selling.
      operationId: getMyPaymentsSelling
      x-api-path-slug: mypaymentssellingid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Payments
      - Selling
      - Id
  /my/payouts:
    get:
      summary: Get My Payouts
      description: Get a list of payouts
      operationId: getMyPayouts
      x-api-path-slug: mypayouts-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Payouts
  /my/payouts/{id}/line_items:
    get:
      summary: Get My Payouts Line Items
      description: Read the line items of a payout
      operationId: getMyPayoutsLineItems
      x-api-path-slug: mypayoutsidline-items-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Payouts
      - Id
      - Line
      - Items
  /my/refund_requests/selling:
    get:
      summary: Get My Refund Requests Selling
      description: Get a list of refund requests as a seller
      operationId: getMyRefundRequestsSelling
      x-api-path-slug: myrefund-requestsselling-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Refund
      - Requests
      - Selling
  /my/refund_requests/selling/{id}:
    put:
      summary: Put My Refund Requests Selling
      description: Update a refund request for a sold order
      operationId: putMyRefundRequestsSelling
      x-api-path-slug: myrefund-requestssellingid-put
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Refund
      - Requests
      - Selling
      - Id
  /my/viewed_listings:
    get:
      summary: Get My Viewed Listings
      description: Get a list of your recently viewed listings.
      operationId: getMyViewedListings
      x-api-path-slug: myviewed-listings-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Viewed
      - Listings
  /my/wishlist:
    get:
      summary: Get My Wishlist
      description: Get a list of wishlisted items
      operationId: getMyWishlist
      x-api-path-slug: mywishlist-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Wishlist
  /my/wishlist/{id}:
    delete:
      summary: Delete My Wishlist
      description: Remove a listing from your wishlist
      operationId: deleteMyWishlist
      x-api-path-slug: mywishlistid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Wishlist
      - Id
    put:
      summary: Put My Wishlist
      description: Add a listing to your wishlist
      operationId: putMyWishlist
      x-api-path-slug: mywishlistid-put
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Wishlist
      - Id
  /orders/{order_id}/feedback/buyer:
    get:
      summary: Get Orders Order Feedback Buyer
      description: Feedback details for an order's buyer
      operationId: getOrdersOrderFeedbackBuyer
      x-api-path-slug: ordersorder-idfeedbackbuyer-get
      parameters:
      - in: path
        name: order_id
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Order
      - Id
      - Feedback
      - Buyer
    post:
      summary: Post Orders Order Feedback Buyer
      description: Add feedback about an order's buyer
      operationId: postOrdersOrderFeedbackBuyer
      x-api-path-slug: ordersorder-idfeedbackbuyer-post
      parameters:
      - in: path
        name: order_id
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Order
      - Id
      - Feedback
      - Buyer
  /orders/{order_id}/feedback/seller:
    get:
      summary: Get Orders Order Feedback Seller
      description: Feedback details for an order's seller
      operationId: getOrdersOrderFeedbackSeller
      x-api-path-slug: ordersorder-idfeedbackseller-get
      parameters:
      - in: path
        name: order_id
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Order
      - Id
      - Feedback
      - Seller
    post:
      summary: Post Orders Order Feedback Seller
      description: Add feedback about an order's seller
      operationId: postOrdersOrderFeedbackSeller
      x-api-path-slug: ordersorder-idfeedbackseller-post
      parameters:
      - in: path
        name: order_id
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Order
      - Id
      - Feedback
      - Seller
  /payment_methods:
    get:
      summary: Get Payment Methods
      description: Get list of payment methods
      operationId: getPaymentMethods
      x-api-path-slug: payment-methods-get
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Methods
  /priceguide:
    get:
      summary: Get Pricegue
      description: Search the Price Guide
      operationId: getPricegue
      x-api-path-slug: priceguide-get
      parameters:
      - in: query
        name: query
        description: Search query
      responses:
        200:
          description: OK
      tags:
      - Priceguide
  /priceguide/{id}:
    get:
      summary: Get Pricegue
      description: Retrieve a Price Guide
      operationId: getPricegue
      x-api-path-slug: priceguideid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Priceguide
      - Id
  /priceguide/{id}/transactions:
    get:
      summary: Get Pricegue Transactions
      description: Get a list of paginated transactions for a price guide.
      operationId: getPricegueTransactions
      x-api-path-slug: priceguideidtransactions-get
      parameters:
      - in: query
        name: condition
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Priceguide
      - Id
      - Transactions
  /priceguide/{id}/transactions/summary:
    get:
      summary: Get Pricegue Transactions Summary
      description: Get a summary of transactions for a given price guide
      operationId: getPricegueTransactionsSummary
      x-api-path-slug: priceguideidtransactionssummary-get
      parameters:
      - in: query
        name: condition
      - in: path
        name: id
      - in: query
        name: number_of_months
      responses:
        200:
          description: OK
      tags:
      - Priceguide
      - Id
      - Transactions
      - Summary
  /products/reviews/{id}:
    get:
      summary: Get Products Reviews
      description: Get products reviews.
      operationId: getProductsReviews
      x-api-path-slug: productsreviewsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Products
      - Reviews
      - Id
    put:
      summary: Put Products Reviews
      description: Put products reviews.
      operationId: putProductsReviews
      x-api-path-slug: productsreviewsid-put
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Products
      - Reviews
      - Id
  /products/{slug}/reviews:
    get:
      summary: Get Products Slug Reviews
      description: View reviews of a comparison shopping page
      operationId: getProductsSlugReviews
      x-api-path-slug: productsslugreviews-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Products
      - Slug
      - Reviews
    post:
      summary: Post Products Slug Reviews
      description: Create a review for a product
      operationId: postProductsSlugReviews
      x-api-path-slug: productsslugreviews-post
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Products
      - Slug
      - Reviews
  /sales/reverb:
    get:
      summary: Get Sales Reverb
      description: View upcoming and live Reverb official sales.
      operationId: getSalesReverb
      x-api-path-slug: salesreverb-get
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Reverb
  /sales/seller:
    get:
      summary: Get Sales Seller
      description: View your created sales.
      operationId: getSalesSeller
      x-api-path-slug: salesseller-get
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Seller
  /sales/{sale_id}/listings:
    delete:
      summary: Delete Sales Sale Listings
      description: Remove a listing from a sale
      operationId: deleteSalesSaleListings
      x-api-path-slug: salessale-idlistings-delete
      parameters:
      - in: path
        name: sale_id
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Sale
      - Id
      - Listings
    post:
      summary: Post Sales Sale Listings
      description: Post sales sale listings.
      operationId: postSalesSaleListings
      x-api-path-slug: salessale-idlistings-post
      parameters:
      - in: path
        name: sale_id
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Sale
      - Id
      - Listings
  /sales/{slug}:
    get:
      summary: Get Sales Slug
      description: Get sales slug.
      operationId: getSalesSlug
      x-api-path-slug: salesslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Slug
  /shipping/providers:
    get:
      summary: Get Shipping Provers
      description: List of supported shipping providers
      operationId: getShippingProvers
      x-api-path-slug: shippingproviders-get
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Providers
  /shipping/regions:
    get:
      summary: Get Shipping Regions
      description: Get shipping regions.
      operationId: getShippingRegions
      x-api-path-slug: shippingregions-get
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Regions
  /shop:
    get:
      summary: Get Shop
      description: Get your own shop details
      operationId: getShop
      x-api-path-slug: shop-get
      responses:
        200:
          description: OK
      tags:
      - Shop
    put:
      summary: Put Shop
      description: Update your shop profile
      operationId: putShop
      x-api-path-slug: shop-put
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Shop
  /shop/listing_conditions:
    get:
      summary: Get Shop Listing Conditions
      description: List of supported product conditions
      operationId: getShopListingConditions
      x-api-path-slug: shoplisting-conditions-get
      responses:
        200:
          description: OK
      tags:
      - Shop
      - Listing
      - Conditions
  /shop/payment_methods:
    get:
      summary: Get Shop Payment Methods
      description: Get accepted payment methods
      operationId: getShopPaymentMethods
      x-api-path-slug: shoppayment-methods-get
      responses:
        200:
          description: OK
      tags:
      - Shop
      - Payment
      - Methods
  /shop/vacation:
    delete:
      summary: Delete Shop Vacation
      description: Disable vacation mode. All listings will be re-enabled.
      operationId: deleteShopVacation
      x-api-path-slug: shopvacation-delete
      responses:
        200:
          description: OK
      tags:
      - Shop
      - Vacation
    get:
      summary: Get Shop Vacation
      description: Returns shop vacation status
      operationId: getShopVacation
      x-api-path-slug: shopvacation-get
      responses:
        200:
          description: OK
      tags:
      - Shop
      - Vacation
    post:
      summary: Post Shop Vacation
      description: Enable vacation mode. All listings will be unavailable until vacation
        mode is turned off.
      operationId: postShopVacation
      x-api-path-slug: shopvacation-post
      responses:
        200:
          description: OK
      tags:
      - Shop
      - Vacation
  /shops/{id}/storefronts:
    get:
      summary: Get Shops Storefronts
      description: Get storefront details on a shop.
      operationId: getShopsStorefronts
      x-api-path-slug: shopsidstorefronts-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Id
      - Storefronts
  /shops/{shop_id}/shipping_profiles:
    get:
      summary: Get Shops Shop Shipping Profiles
      description: List of shipping profiles for your shop
      operationId: getShopsShopShippingProfiles
      x-api-path-slug: shopsshop-idshipping-profiles-get
      parameters:
      - in: path
        name: shop_id
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Shop
      - Id
      - Shipping
      - Profiles
  /shops/{slug}:
    get:
      summary: Get Shops Slug
      description: Get details on a shop.
      operationId: getShopsSlug
      x-api-path-slug: shopsslug-get
      parameters:
      - in: query
        name: include_listing_count
        description: Include the live listing count in the response
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Slug
  /shops/{slug}/feedback:
    get:
      summary: Get Shops Slug Feedback
      description: Get shops slug feedback.
      operationId: getShopsSlugFeedback
      x-api-path-slug: shopsslugfeedback-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Slug
      - Feedback
  /shops/{slug}/feedback/buyer:
    get:
      summary: Get Shops Slug Feedback Buyer
      description: Get seller's feedback as a buyer
      operationId: getShopsSlugFeedbackBuyer
      x-api-path-slug: shopsslugfeedbackbuyer-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Slug
      - Feedback
      - Buyer
  /shops/{slug}/feedback/seller:
    get:
      summary: Get Shops Slug Feedback Seller
      description: Get seller's feedback as a seller
      operationId: getShopsSlugFeedbackSeller
      x-api-path-slug: shopsslugfeedbackseller-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Shops
      - Slug
      - Feedback
      - Seller
  /wants:
    get:
      summary: Get Wants
      description: A list of wanted items by the user
      operationId: getWants
      x-api-path-slug: wants-get
      responses:
        200:
          description: OK
      tags:
      - Wants
  /wants/{id}:
    delete:
      summary: Delete Wants
      description: Unmark an item wanted.
      operationId: deleteWants
      x-api-path-slug: wantsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Wants
      - Id
    put:
      summary: Put Wants
      description: Mark an item wanted. Returns 200 on success or 422 on failure.
      operationId: putWants
      x-api-path-slug: wantsid-put
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Wants
      - Id
  /webhooks/registrations:
    get:
      summary: Get Webhooks Registrations
      description: Get webhooks registrations.
      operationId: getWebhooksRegistrations
      x-api-path-slug: webhooksregistrations-get
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - Registrations
    post:
      summary: Post Webhooks Registrations
      description: Post webhooks registrations.
      operationId: postWebhooksRegistrations
      x-api-path-slug: webhooksregistrations-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - Registrations
  /webhooks/registrations/{id}:
    delete:
      summary: Delete Webhooks Registrations
      description: Delete webhooks registrations.
      operationId: deleteWebhooksRegistrations
      x-api-path-slug: webhooksregistrationsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - Registrations
      - Id
    get:
      summary: Get Webhooks Registrations
      description: Get details of a webhook registration
      operationId: getWebhooksRegistrations
      x-api-path-slug: webhooksregistrationsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - Registrations
      - Id
  /accounts:
    post:
      summary: Post Accounts
      description: Create an account.
      operationId: postAccounts
      x-api-path-slug: accounts-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /articles/featured:
    get:
      summary: Get Articles Featured
      description: See featured Reverb blog posts
      operationId: getArticlesFeatured
      x-api-path-slug: articlesfeatured-get
      responses:
        200:
          description: OK
      tags:
      - Articles
      - Featured
  /articles/recently_featured:
    get:
      summary: Get Articles Recently Featured
      description: Get articles recently featured.
      operationId: getArticlesRecentlyFeatured
      x-api-path-slug: articlesrecently-featured-get
      responses:
        200:
          description: OK
      tags:
      - Articles
      - Recently
      - Featured
  /articles/{slug}:
    get:
      summary: Get Articles Slug
      description: Display a single article
      operationId: getArticlesSlug
      x-api-path-slug: articlesslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Articles
      - Slug
  /articles/{slug}/related-listings:
    get:
      summary: Get Articles Slug Related Listings
      description: Find listings related to an article
      operationId: getArticlesSlugRelatedListings
      x-api-path-slug: articlesslugrelatedlistings-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Articles
      - Slug
      - Related-listings
  /auth/forgot_password:
    post:
      summary: Post Auth Forgot Password
      description: Send a password reset email
      operationId: postAuthForgotPassword
      x-api-path-slug: authforgot-password-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Auth
      - Forgot
      - Password
  /auth/logout:
    put:
      summary: Put Auth Logout
      description: Logout (primarily for mobile clients)
      operationId: putAuthLogout
      x-api-path-slug: authlogout-put
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Auth
      - Logout
  /autosuggest:
    get:
      summary: Get Autosuggest
      description: Autosuggest terms for searches
      operationId: getAutosuggest
      x-api-path-slug: autosuggest-get
      responses:
        200:
          description: OK
      tags:
      - Autosuggest
  /cart:
    get:
      summary: Get Cart
      description: Get all cart items
      operationId: getCart
      x-api-path-slug: cart-get
      responses:
        200:
          description: OK
      tags:
      - Cart
  /cart/move_to_watch_list/{cart_item_id}:
    post:
      summary: Post Cart Move To Watch List Cart Item
      description: Remove a cart item and add it to watch list
      operationId: postCartMoveToWatchListCartItem
      x-api-path-slug: cartmove-to-watch-listcart-item-id-post
      parameters:
      - in: path
        name: cart_item_id
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Move
      - To
      - Watch
      - List
      - Cart
      - Item
      - Id
  /cart/{id}:
    delete:
      summary: Delete Cart
      description: Remove a product from the cart
      operationId: deleteCart
      x-api-path-slug: cartid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Id
    post:
      summary: Post Cart
      description: Add product to the cart
      operationId: postCart
      x-api-path-slug: cartid-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Id
    put:
      summary: Put Cart
      description: Update cart item details
      operationId: putCart
      x-api-path-slug: cartid-put
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Id
  /collections:
    get:
      summary: Get Collections
      description: List of curated collections
      operationId: getCollections
      x-api-path-slug: collections-get
      responses:
        200:
          description: OK
      tags:
      - Collections
  /collections/{slug}:
    get:
      summary: Get Collections Slug
      description: Get collections slug.
      operationId: getCollectionsSlug
      x-api-path-slug: collectionsslug-get
      parameters:
      - in: path
        name: slug
      responses:
        200:
          description: OK
      tags:
      - Collections
      - Slug
  /my/orders/buying/buying_history/{seller_id}:
    get:
      summary: Get My Orders Buying Buying History Seller
      description: Get my orders buying buying history seller.
      operationId: getMyOrdersBuyingBuyingHistorySeller
      x-api-path-slug: myordersbuyingbuying-historyseller-id-get
      parameters:
      - in: path
        name: seller_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Buying
      - Buying
      - History
      - Seller
      - Id
  /shop/stats:
    get:
      summary: Get Shop Stats
      description: Get listings stats
      operationId: getShopStats
      x-api-path-slug: shopstats-get
      responses:
        200:
          description: OK
      tags:
      - Shop
      - Stats
  /shop/stats/activity:
    get:
      summary: Get Shop Stats Activity
      description: Get shop activity for a particular time period
      operationId: getShopStatsActivity
      x-api-path-slug: shopstatsactivity-get
      parameters:
      - in: query
        name: end_time
        description: Filter by date in ISO8601 format - e
      - in: query
        name: start_time
        description: Filter by date in ISO8601 format - e
      responses:
        200:
          description: OK
      tags:
      - Shop
      - Stats
      - Activity
  /vinyl/listings:
    get:
      summary: Get Vinyl Listings
      description: Get vinyl listings.
      operationId: getVinylListings
      x-api-path-slug: vinyllistings-get
      parameters:
      - in: query
        name: merchandising_uuid
        description: Merchandising UUID of the release
      responses:
        200:
          description: OK
      tags:
      - Vinyl
      - Listings
    post:
      summary: Post Vinyl Listings
      description: Post vinyl listings.
      operationId: postVinylListings
      x-api-path-slug: vinyllistings-post
      responses:
        200:
          description: OK
      tags:
      - Vinyl
      - Listings
  /vinyl/listings/{id}:
    get:
      summary: Get Vinyl Listings
      description: Get vinyl listings.
      operationId: getVinylListings
      x-api-path-slug: vinyllistingsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Vinyl
      - Listings
      - Id