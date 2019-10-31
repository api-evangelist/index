swagger: "2.0"
x-collection-name: BigOven
x-complete: 1
info:
  title: Big Oven
  description: documentationthis-is-the-documentation-for-the-partner-endpoint-of-the-bigoven-recipe-and-grocery-list-api-the-update-brings-with-it-swaggerbased-documentation--swaggerhttpswagger-io-is-an-emerging-standard-for-describing-restbased-apis-and-with-this-swaggercompliant-endpoint-above-you-can-make-readytogo-interface-libraries-for-your-code-via-swaggercodegenhttpsgithub-comswaggerapiswaggercodegen--for-instance-its-easy-to-generate-libraries-for-node-js-java-ruby-asp-net-mvc-jquery-php-and-moreyou-can-also-try-out-the-endpoint-calls-with-your-own-api-key-right-here-on-this-page--be-sure-to-enter-your-api-key-above-to-use-the-try-it-out-buttons-on-this-page-start-heredevelopers-new-to-the-bigoven-api-should-start-with-this-version-not-with-the-legacy-api--well-be-making-improvements-to-this-api-over-time-and-doing-only-bug-fixes-on-the-v1-api-to-pretend-youre-a-bigoven-user-for-instance-to-get-your-recently-viewed-recipes-or-your-grocery-list-you-need-to-pass-in-basic-authentication-information-in-the-header-just-as-with-the-v1-api--we-do-now-require-that-you-make-all-calls-via-https--you-need-to-pass-your-api-key-in-with-every-call-though-this-can-now-be-done-on-the-header-send-a-request-header-xbigovenapikey-set-to-your-api-key-value-e-g--requestxbigovenapikeyyourkeyhere-migration-notesfor-existing-partners-we-encourage-you-to-migratehttpapi2-bigoven-com-and-while-at-this-writing-we-have-no-hardandfast-termination-date-for-the-v1-api-we-strongly-prefer-that-you-migrate-by-january-1-2017--while-the-changes-arent-overly-complex-there-are-several-breaking-changes-including-refactoring-of-recipe-search-and-results-and-removal-of-support-for-xml--this-is-not-a-simply-plugandplay-replacement-to-the-v1-api--with-respect-to-an-exclusive-focus-on-json-the-world-has-spoken-and-it-prefers-json-for-restbased-apis--weve-taken-numerous-steps-to-refactor-the-api-to-make-it-more-restcompliant--note-that-this-v2-api-will-be-the-preferred-api-from-this-point-onward-so-we-encourage-developers-to-migrate-to-this-new-format--we-have-put-together-some-migration-noteswebdocumentationmigrationtov2-that-we-encourage-you-to-read-carefully-photossee-our-photos-documentationhttpapi2-bigoven-comwebdocumentationrecipeimages--for-more-information-on-usage-of-this-api-including-features-pricing-rate-limits-terms-and-conditions-please-visit-the-bigoven-api-websitehttpapi2-bigoven-com-
  termsOfService: Please see our [terms of service](http://api2.bigoven.com/web/documentation/termsofuse
  version: partner
host: api2.bigoven.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /collection/{id}:
    get:
      summary: Gets a recipe collection. A recipe collection is a curated set of recipes.
      description: Gets a recipe collection. a recipe collection is a curated set
        of recipes..
      operationId: Collection_GetCollection
      x-api-path-slug: collectionid-get
      parameters:
      - in: path
        name: id
        description: the collection identifier
      - in: query
        name: pg
        description: page number (starting with 1)
      - in: query
        name: rpp
        description: results per page
      - in: query
        name: sessionForLogging
      - in: query
        name: test
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Collection
  /collection/{id}/meta:
    get:
      summary: Gets a recipe collection metadata. A recipe collection is a curated
        set of recipes.
      description: Gets a recipe collection metadata. a recipe collection is a curated
        set of recipes..
      operationId: Collection_GetCollectionMeta
      x-api-path-slug: collectionidmeta-get
      parameters:
      - in: path
        name: id
        description: the collection identifier
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Collection
      - Meta
  /collections:
    get:
      summary: Get the list of current, seasonal recipe collections. From here, you
        can use the /collection/{id} endpoint to retrieve the recipes in those collections.
      description: Get the list of current, seasonal recipe collections. from here,
        you can use the /collection/{id} endpoint to retrieve the recipes in those
        collections..
      operationId: Collection_Collections
      x-api-path-slug: collections-get
      parameters:
      - in: query
        name: test
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Collections
  /glossary/byterm/{term}:
    get:
      summary: Get food glossary article by term (e.g., asparagus). This editorial
        is (c) BigOven and MUST carry attribution and a link back to the glossary
        entry on BigOven.com.
      description: Get food glossary article by term (e.g., asparagus). this editorial
        is (c) bigoven and must carry attribution and a link back to the glossary
        entry on bigoven.com..
      operationId: Glossary_ByTerm
      x-api-path-slug: glossarybytermterm-get
      parameters:
      - in: path
        name: term
        description: Keyword used to look up article, e
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Glossary
      - Byterm
      - Term
  /glossary/{id}:
    get:
      summary: Get food glossary article
      description: Get food glossary article.
      operationId: Glossary_Get
      x-api-path-slug: glossaryid-get
      parameters:
      - in: path
        name: id
        description: identifier of article to retrieve
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Glossary
  /grocerylist:
    delete:
      summary: Delete all the items on a grocery list; faster operation than a sync
        with deleted items.
      description: Delete all the items on a grocery list; faster operation than a
        sync with deleted items..
      operationId: GroceryList_Delete
      x-api-path-slug: grocerylist-delete
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
    get:
      summary: Get the user's grocery list.  User is determined by Basic Authentication.
      description: Get the user's grocery list.  user is determined by basic authentication..
      operationId: GroceryList_Get
      x-api-path-slug: grocerylist-get
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
  /grocerylist/department:
    post:
      summary: Departmentalize a list of strings -- used for ad-hoc grocery list item
        addition
      description: Departmentalize a list of strings -- used for ad-hoc grocery list
        item addition.
      operationId: GroceryList_Department
      x-api-path-slug: grocerylistdepartment-post
      parameters:
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
      - Department
  /grocerylist/item:
    post:
      summary: Add a single line item to the grocery list
      description: Add a single line item to the grocery list.
      operationId: GroceryList_Post
      x-api-path-slug: grocerylistitem-post
      parameters:
      - in: body
        name: newItem
        description: name, quantity, unit, notes, department
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
      - Item
  /grocerylist/item/{guid}:
    delete:
      summary: /grocerylist/item/{guid}  DELETE will delete this item assuming you
        own it.
      description: /grocerylist/item/{guid}  delete will delete this item assuming
        you own it..
      operationId: GroceryList_DeleteItemByGuid
      x-api-path-slug: grocerylistitemguid-delete
      parameters:
      - in: path
        name: guid
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
      - Item
      - Guid
    put:
      summary: Update a grocery item by GUID
      description: Update a grocery item by guid.
      operationId: GroceryList_GroceryListItemGuid
      x-api-path-slug: grocerylistitemguid-put
      parameters:
      - in: path
        name: guid
      - in: body
        name: req
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
      - Item
      - Guid
  /grocerylist/recipe:
    post:
      summary: "Add a Recipe to the grocery list.  In the request data, pass in recipeId,
        scale (scale=1.0 says to keep the recipe the same size as originally posted),
        markAsPending (true/false) to indicate that\r\n            the lines in the
        recipe should be marked"
      description: "Add a recipe to the grocery list.  in the request data, pass in
        recipeid, scale (scale=1.0 says to keep the recipe the same size as originally
        posted), markaspending (true/false) to indicate that\r\n            the lines
        in the recipe should be marked ."
      operationId: GroceryList_AddRecipe
      x-api-path-slug: grocerylistrecipe-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
      - Recipe
  /grocerylist/sync:
    post:
      summary: Synchronize the grocery list.  Call this with a POST to /grocerylist/sync
      description: Synchronize the grocery list.  call this with a post to /grocerylist/sync.
      operationId: GroceryList_PostGroceryListSync
      x-api-path-slug: grocerylistsync-post
      parameters:
      - in: body
        name: req
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Grocerylist
      - Sync
  /recipe:
    post:
      summary: Add a new recipe
      description: Add a new recipe.
      operationId: Recipe_Post
      x-api-path-slug: recipe-post
      parameters:
      - in: body
        name: recipe
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
    put:
      summary: Update a recipe
      description: Update a recipe.
      operationId: Recipe_Put
      x-api-path-slug: recipe-put
      parameters:
      - in: body
        name: recipe
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
  /recipe/autocomplete:
    get:
      summary: Given a query, return recipe titles starting with query. Query must
        be at least 3 chars in length.
      description: Given a query, return recipe titles starting with query. query
        must be at least 3 chars in length..
      operationId: Recipe_AutoComplete
      x-api-path-slug: recipeautocomplete-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: query
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Autocomplete
  /recipe/categories:
    get:
      summary: Get a list of recipe categories (the ID field can be used for include_cat
        in search parameters)
      description: Get a list of recipe categories (the id field can be used for include_cat
        in search parameters).
      operationId: Recipe_Categories
      x-api-path-slug: recipecategories-get
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Categories
  /recipe/review/replies/{replyId}:
    delete:
      summary: DELETE a reply to a given review. Authenticated user must be the one
        who originally posted the reply.
      description: Delete a reply to a given review. authenticated user must be the
        one who originally posted the reply..
      operationId: Review_DeleteReply
      x-api-path-slug: recipereviewrepliesreplyid-delete
      parameters:
      - in: path
        name: replyId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Review
      - Replies
      - ReplyId
    put:
      summary: Update (PUT) a reply to a given review. Authenticated user must be
        the original one that posted the reply.
      description: Update (put) a reply to a given review. authenticated user must
        be the original one that posted the reply..
      operationId: Review_PutReply
      x-api-path-slug: recipereviewrepliesreplyid-put
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: replyId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Review
      - Replies
      - ReplyId
  /recipe/review/{reviewId}:
    get:
      summary: "Get a given review by string-style ID. This will return a payload
        with FeaturedReply, ReplyCount.\r\n            Recommended display is to list
        top-level reviews with one featured reply underneath. \r\n            Currently,
        the FeaturedReply is the most"
      description: "Get a given review by string-style id. this will return a payload
        with featuredreply, replycount.\r\n            recommended display is to list
        top-level reviews with one featured reply underneath. \r\n            currently,
        the featuredreply is the most."
      operationId: ""
      x-api-path-slug: recipereviewreviewid-get
      parameters:
      - in: path
        name: reviewId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Review
      - ReviewId
    put:
      summary: Update a given top-level review.
      description: Update a given top-level review..
      operationId: Review_Put
      x-api-path-slug: recipereviewreviewid-put
      parameters:
      - in: body
        name: review
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: reviewId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Review
      - ReviewId
  /recipe/review/{reviewId}/replies:
    get:
      summary: Get a paged list of replies for a given review.
      description: Get a paged list of replies for a given review..
      operationId: Review_GetReplies
      x-api-path-slug: recipereviewreviewidreplies-get
      parameters:
      - in: query
        name: pg
        description: the page (int), starting with 1
      - in: path
        name: reviewId
      - in: query
        name: rpp
        description: results per page (int)
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Review
      - ReviewId
      - Replies
    post:
      summary: POST a reply to a given review. The date will be set by server. Note
        that replies no longer have star ratings, only top-level reviews do.
      description: Post a reply to a given review. the date will be set by server.
        note that replies no longer have star ratings, only top-level reviews do..
      operationId: Review_PostReply
      x-api-path-slug: recipereviewreviewidreplies-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: reviewId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Review
      - ReviewId
      - Replies
  /recipe/scan:
    post:
      summary: "POST an image as a new RecipeScan request\r\n                1)  Fetch
        the filename -- DONE\r\n                2)  Copy it to the pics/scan folder
        - ENSURE NO NAMING COLLISIONS -- DONE\r\n                3)  Create 120 thumbnail
        size  in pics/scan/120 -- D"
      description: "Post an image as a new recipescan request\r\n                1)
        \ fetch the filename -- done\r\n                2)  copy it to the pics/scan
        folder - ensure no naming collisions -- done\r\n                3)  create
        120 thumbnail size  in pics/scan/120 -- d."
      operationId: Recipe_Scan
      x-api-path-slug: recipescan-post
      parameters:
      - in: query
        name: devicetype
      - in: query
        name: lat
      - in: query
        name: lng
      - in: query
        name: test
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - Scan
  /recipe/{id}:
    delete:
      summary: Delete a Recipe (you must be authenticated as an owner of the recipe)
      description: Delete a recipe (you must be authenticated as an owner of the recipe).
      operationId: Recipe_Delete
      x-api-path-slug: recipeid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
    get:
      summary: Return full Recipe detail. Returns 403 if the recipe is owned by someone
        else.
      description: Return full recipe detail. returns 403 if the recipe is owned by
        someone else..
      operationId: Recipe_Get
      x-api-path-slug: recipeid-get
      parameters:
      - in: path
        name: id
        description: the Recipe ID to retrieve
      - in: query
        name: prefetch
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
  /recipe/{recipeId}/feedback:
    post:
      summary: Feedback on a Recipe -- for internal BigOven editors
      description: Feedback on a recipe -- for internal bigoven editors.
      operationId: Recipe_Feedback
      x-api-path-slug: reciperecipeidfeedback-post
      parameters:
      - in: body
        name: data
        description: The payload for feedback, which includes the field feedback
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: recipeId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Feedback
  /recipe/{recipeId}/image:
    post:
      summary: "POST: /recipe/{recipeId}/image?lat=42&amp;lng=21&amp;caption=this%20is%20my%20caption\r\n
        \            \r\n             Note that caption, lng and lat are all optional,
        but must go on the request URI as params because this endpoint\r\n             needs
        a m"
      description: "Post: /recipe/{recipeid}/image?lat=42&amp;lng=21&amp;caption=this%20is%20my%20caption\r\n
        \            \r\n             note that caption, lng and lat are all optional,
        but must go on the request uri as params because this endpoint\r\n             needs
        a m."
      operationId: Images_UploadRecipeImage
      x-api-path-slug: reciperecipeidimage-post
      parameters:
      - in: query
        name: caption
      - in: query
        name: lat
      - in: query
        name: lng
      - in: path
        name: recipeId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Image
  /recipe/{recipeId}/images:
    get:
      summary: Get all the images for a recipe. DEPRECATED. Please use /recipe/{recipeId}/photos.
      description: Get all the images for a recipe. deprecated. please use /recipe/{recipeid}/photos..
      operationId: Images_Get
      x-api-path-slug: reciperecipeidimages-get
      parameters:
      - in: path
        name: recipeId
        description: Recipe ID (required)
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Images
  /recipe/{recipeId}/note:
    post:
      summary: HTTP POST a new note into the system.
      description: Http post a new note into the system..
      operationId: Note_Post
      x-api-path-slug: reciperecipeidnote-post
      parameters:
      - in: body
        name: note
        description: 'a recipe note, with fields: Date (YYYY-MM-DD string), Notes
          (string), People (string), Variations (string), RecipeID (int?)'
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: recipeId
        description: recipeId (int)
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Note
  /recipe/{recipeId}/note/{noteId}:
    delete:
      summary: "Delete a review\r\n                do a DELETE Http request of /note/{ID}"
      description: "Delete a review\r\n                do a delete http request of
        /note/{id}."
      operationId: Note_Delete
      x-api-path-slug: reciperecipeidnotenoteid-delete
      parameters:
      - in: path
        name: noteId
        description: noteId (int)
      - in: path
        name: recipeId
        description: recipeId (int)
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Note
      - NoteId
    get:
      summary: Get a given note. Make sure you're passing authentication information
        in the header for the user who owns the note.
      description: Get a given note. make sure you're passing authentication information
        in the header for the user who owns the note..
      operationId: Note_Get
      x-api-path-slug: reciperecipeidnotenoteid-get
      parameters:
      - in: path
        name: noteId
        description: The note ID (note -- its not the RecipeID)
      - in: path
        name: recipeId
        description: recipe identifier (integer)
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Note
      - NoteId
    put:
      summary: HTTP PUT (update) a Recipe note (RecipeNote).
      description: Http put (update) a recipe note (recipenote)..
      operationId: Note_Put
      x-api-path-slug: reciperecipeidnotenoteid-put
      parameters:
      - in: path
        name: noteId
      - in: path
        name: recipeId
      - in: body
        name: recipeNote
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Note
      - NoteId
  /recipe/{recipeId}/notes:
    get:
      summary: recipe/100/notes
      description: Recipe/100/notes.
      operationId: Note_GetNotes
      x-api-path-slug: reciperecipeidnotes-get
      parameters:
      - in: query
        name: pg
        description: page (int, starting from 1)
      - in: path
        name: recipeId
        description: recipeId (int)
      - in: query
        name: rpp
        description: recipeId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Notes
  /recipe/{recipeId}/photos:
    get:
      summary: Get all the photos for a recipe
      description: Get all the photos for a recipe.
      operationId: Images_GetRecipePhotos
      x-api-path-slug: reciperecipeidphotos-get
      parameters:
      - in: query
        name: pg
      - in: path
        name: recipeId
        description: Recipe ID (required)
      - in: query
        name: rpp
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Photos
  /recipe/{recipeId}/related:
    get:
      summary: Get recipes related to the given recipeId
      description: Get recipes related to the given recipeid.
      operationId: Recipe_Related
      x-api-path-slug: reciperecipeidrelated-get
      parameters:
      - in: query
        name: pg
      - in: path
        name: recipeId
      - in: query
        name: rpp
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Related
  /recipe/{recipeId}/review:
    get:
      summary: Get *my* review for the recipe {recipeId}, where "me" is determined
        by standard authentication headers
      description: Get *my* review for the recipe {recipeid}, where "me" is determined
        by standard authentication headers.
      operationId: ""
      x-api-path-slug: reciperecipeidreview-get
      parameters:
      - in: path
        name: recipeId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Review
    post:
      summary: Add a new review. Only one review can be provided per {userId, recipeId}
        pair. Otherwise your review will be updated.
      description: Add a new review. only one review can be provided per {userid,
        recipeid} pair. otherwise your review will be updated..
      operationId: Review_Post
      x-api-path-slug: reciperecipeidreview-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: recipeId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Review
  /recipe/{recipeId}/review/{reviewId}:
    delete:
      summary: "Delete a review by recipeId and reviewId. DEPRECATED. Please see recipe/review/{reviewId}
        for the preferred method.\r\n            (We are moving from an integer-based
        ID system to a GUID-style string-based ID system for reviews and replies.)"
      description: "Delete a review by recipeid and reviewid. deprecated. please see
        recipe/review/{reviewid} for the preferred method.\r\n            (we are
        moving from an integer-based id system to a guid-style string-based id system
        for reviews and replies.)."
      operationId: Review_Delete
      x-api-path-slug: reciperecipeidreviewreviewid-delete
      parameters:
      - in: path
        name: recipeId
      - in: path
        name: reviewId
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Review
      - ReviewId
    get:
      summary: "Get a given review - DEPRECATED. See recipe/review/{reviewId} for
        the current usage.\r\n            Beginning in January 2017, BigOven moded
        from an integer-based ID system to a GUID-style string-based ID system for
        reviews and replies.\r\n            We"
      description: "Get a given review - deprecated. see recipe/review/{reviewid}
        for the current usage.\r\n            beginning in january 2017, bigoven moded
        from an integer-based id system to a guid-style string-based id system for
        reviews and replies.\r\n            we."
      operationId: ""
      x-api-path-slug: reciperecipeidreviewreviewid-get
      parameters:
      - in: path
        name: recipeId
        description: int
      - in: path
        name: reviewId
        description: int
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Review
      - ReviewId
    put:
      summary: "HTTP PUT (update) a recipe review. DEPRECATED. Please see recipe/review/{reviewId}
        PUT for the new endpoint.\r\n            We are moving to a string-based primary
        key system, no longer integers, for reviews and replies."
      description: "Http put (update) a recipe review. deprecated. please see recipe/review/{reviewid}
        put for the new endpoint.\r\n            we are moving to a string-based primary
        key system, no longer integers, for reviews and replies.."
      operationId: Review_PutLegacy
      x-api-path-slug: reciperecipeidreviewreviewid-put
      parameters:
      - in: path
        name: recipeId
        description: recipeId (int)
      - in: body
        name: review
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: reviewId
        description: reviewId (int)
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Review
      - ReviewId
  /recipe/{recipeId}/reviews:
    get:
      summary: Get paged list of reviews for a recipe. Each review will have at most
        one FeaturedReply, as well as a ReplyCount.
      description: Get paged list of reviews for a recipe. each review will have at
        most one featuredreply, as well as a replycount..
      operationId: Review_GetReviews
      x-api-path-slug: reciperecipeidreviews-get
      parameters:
      - in: query
        name: pg
        description: the page (int), starting with 1
      - in: path
        name: recipeId
        description: recipe id (int)
      - in: query
        name: rpp
        description: results per page (int)
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Reviews
  /recipe/{recipeId}/scans:
    get:
      summary: Gets a list of RecipeScan images for the recipe. There will be at most
        3 per recipe.
      description: Gets a list of recipescan images for the recipe. there will be
        at most 3 per recipe..
      operationId: Images_GetScanImages
      x-api-path-slug: reciperecipeidscans-get
      parameters:
      - in: path
        name: recipeId
        description: the recipe identifier (int)
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
      - RecipeId
      - Scans
  /recipes:
    get:
      summary: "Search for recipes. There are many parameters that you can apply.
        Starting with the most common, use title_kw to search within a title.\r\n
        \           Use any_kw to search across the entire recipe.\r\n            If
        you'd like to limit by course, set the"
      description: "Search for recipes. there are many parameters that you can apply.
        starting with the most common, use title_kw to search within a title.\r\n
        \           use any_kw to search across the entire recipe.\r\n            if
        you'd like to limit by course, set the."
      operationId: Recipe_RecipeSearch
      x-api-path-slug: recipes-get
      parameters:
      - in: query
        name: any_kw
        description: Search anywhere in the recipe for the keyword
      - in: query
        name: boostmine
        description: if set to true, boost my own recipes in my folders so they show
          up high in the list (at the expense of other sort orders)
      - in: query
        name: champion
        description: optional
      - in: query
        name: chs
        description: when set to 1, limit to contains-cheese (Powersearch-capable
          plan required)
      - in: query
        name: coll
        description: Limit to a collection ID number
      - in: query
        name: cps
        description: when set to 1, recipe contains pasta, set to 0 means contains
          no pasta (Powersearch-capable plan required)
      - in: query
        name: cuisine
        description: Limit to a specific cuisine
      - in: query
        name: db
      - in: query
        name: dyf
        description: when set to 1, limit to dairy-free (Powersearch-capable plan
          required)
      - in: query
        name: exclude_cat
        description: like include_cat, set this to an integer to exclude a specific
          category
      - in: query
        name: exclude_ing
        description: A CSV representing up to 3 ingredients to exclude  (Powersearch-capable
          plan required)
      - in: query
        name: filter
        description: optionally set to either myrecipes, try, favorites,added to filter
          to just the authenticated users recipe set
      - in: query
        name: folder
        description: Search in a specific folder name for the authenticated user
      - in: query
        name: glf
        description: when set to 1, limit to gluten-free (Powersearch-capable plan
          required)
      - in: query
        name: include_cat
        description: integer of the subcategory youd like to limit searches to (see
          the /recipe/categories endpoint for available id numbers)
      - in: query
        name: include_ing
        description: A CSV representing up to 3 ingredients to include, e
      - in: query
        name: include_primarycat
        description: csv indicating up to three top-level categories -- valid values
          are [appetizers,bread,breakfast,desserts,drinks,maindish,salads,sidedish,soups,marinades,other]
      - in: query
        name: ntf
        description: when set to 1, limit to nut-free (Powersearch-capable plan required)
      - in: query
        name: pg
        description: 'integer: the page number'
      - in: query
        name: photos
        description: if set to true, limit search results to photos only
      - in: query
        name: rmf
        description: when set to 1, limit to red-meat free (Powersearch-capable plan
          required)
      - in: query
        name: rpp
        description: integer; results per page
      - in: query
        name: sff
        description: when set to 1, limit to seafood-free (Powersearch-capable plan
          required)
      - in: query
        name: slf
        description: when set to 1, limit to shellfish-free (Powersearch-capable plan
          required)
      - in: query
        name: title_kw
        description: Search just in the recipe title for the keyword
      - in: query
        name: tnf
        description: when set to 1, limit to tree-nut free (Powersearch-capable plan
          required)
      - in: query
        name: token
      - in: query
        name: userId
        description: Set the target userid to search their public recipes
      - in: query
        name: username
        description: Set the target username to search their public recipes
      - in: query
        name: userset
        description: If set to a given username, itll force the search to filter to
          just that username
      - in: query
        name: vgn
        description: when set to 1, limit to vegan (Powersearch-capable plan required)
      - in: query
        name: vtn
        description: when set to 1, limit to vegetarian (Powersearch-capable plan
          required)
      - in: query
        name: wmf
        description: when set to 1, limit to white-meat free (Powersearch-capable
          plan required)
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipes
  /recipes/random:
    get:
      summary: Get a random, home-page-quality Recipe.
      description: Get a random, home-page-quality recipe..
      operationId: Recipe_GetRandomRecipe
      x-api-path-slug: recipesrandom-get
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipes
      - Random
  /recipes/raves:
    get:
      summary: Get the recipe/comment tuples for those recipes with 4 or 5 star ratings
      description: Get the recipe/comment tuples for those recipes with 4 or 5 star
        ratings.
      operationId: Recipe_Raves
      x-api-path-slug: recipesraves-get
      parameters:
      - in: query
        name: pg
        description: page, starting with 1
      - in: query
        name: rpp
        description: results per page
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipes
      - Raves
  /recipes/recentviews:
    get:
      summary: Get a list of recipes that the authenticated user has most recently
        viewed
      description: Get a list of recipes that the authenticated user has most recently
        viewed.
      operationId: Recipe_RecentViews
      x-api-path-slug: recipesrecentviews-get
      parameters:
      - in: query
        name: pg
        description: Page number starting with 1
      - in: query
        name: rpp
        description: results per page
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipes
      - Recentviews