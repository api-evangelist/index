swagger: "2.0"
x-collection-name: Kentico Cloud
x-complete: 1
info:
  title: Kentico Cloud
  description: this-is-a-collection-of-resources-you-can-find-within-the-kentico-cloud-developer-hubhttpsdeveloper-kenticocloud-com--kentico-cloudhttpskenticocloud-com-is-a-cloudfirst-headless-cms-that-allows-you-to-distribute-content-to-any-channel-and-device-websites-mobile-devices-mixed-reality-devices-presentation-kiosks-etc--through-an-api-certain-apis-require-that-you-include-the-authorization-header--find-more-in-httpsdeveloper-kenticocloud-comreferenceauthentication-
  version: 1.0.0
host: deliver.kenticocloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /975bf280-fd91-488c-994c-2f04416e5ee3/items:
    get:
      summary: Order articles by publish date
      description: Filter the content items by content type by including the `order`
        query parameter and a content element codename.
      operationId: 975bf280Fd91488c994c2f04416e5ee3ItemsGet8
      x-api-path-slug: 975bf280fd91488c994c2f04416e5ee3items-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: order
      - in: query
        name: system.type
      responses:
        200:
          description: OK
      tags:
      - Order
      - Articles
      - By
      - Publish
      - Date
  /items/3120ec15-a4a2-47ec-8ccd-c85ac8ac5ba5:
    get:
      summary: View a content item by ID
      description: Retrieve metadata information about a content item specified by
        its internal ID.
      operationId: Items3120ec15A4a247ec8ccdC85ac8ac5ba5Get
      x-api-path-slug: items3120ec15a4a247ec8ccdc85ac8ac5ba5-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Content
      - Item
      - By
      - ID
    put:
      summary: Update a content item by ID
      description: Update an existing content item specified by its internal ID.
      operationId: Items3120ec15A4a247ec8ccdC85ac8ac5ba5Put
      x-api-path-slug: items3120ec15a4a247ec8ccdc85ac8ac5ba5-put
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Content
      - Item
      - By
      - ID
    delete:
      summary: Delete a content item by ID
      description: Delete a content item specified by its internal ID. Note that deleting
        a content item deletes all of its language variants as well.
      operationId: Items3120ec15A4a247ec8ccdC85ac8ac5ba5Delete2
      x-api-path-slug: items3120ec15a4a247ec8ccdc85ac8ac5ba5-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Content
      - Item
      - By
      - ID
  /14372844-0a5d-434a-8423-605b8a631623/items:
    get:
      summary: Filtering based on date with Delivery API
      description: |-
        Filter content items directly in the API call using the `element.element_codename` query parameter and *publish from* and *publish until* elements.

        See <https://developer.kenticocloud.com/docs/scheduling-content-unpublishing#section-filtering-by-date-with-the-delivery-api> for more details.
      operationId: 143728440a5d434a8423605b8a631623ItemsGet
      x-api-path-slug: 143728440a5d434a8423605b8a631623items-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: elements.publish_until[gt]
      - in: query
        name: system.type
      responses:
        200:
          description: OK
      tags:
      - Filtering
      - Based
      - "On"
      - Date
      - Delivery
      - API
  /items/codename/on_roasts:
    get:
      summary: View a content item by codename
      description: Retrieve metadata information about a content item specified by
        its codename.
      operationId: ItemsCodenameOnRoastsGet
      x-api-path-slug: itemscodenameon-roasts-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Content
      - Item
      - By
      - Codename
    put:
      summary: Update a content item by codename
      description: Update an existing content item specified by its codename.
      operationId: ItemsCodenameOnRoastsPut
      x-api-path-slug: itemscodenameon-roasts-put
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Content
      - Item
      - By
      - Codename
    delete:
      summary: Delete a content item by codename
      description: |-
        Delete a content item specified by its codename.

        Note that deleting a content item deletes all of its language variants as well.
      operationId: ItemsCodenameOnRoastsDelete
      x-api-path-slug: itemscodenameon-roasts-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Content
      - Item
      - By
      - Codename
  /items/3120ec15-a4a2-47ec-8ccd-c85ac8ac5ba5/variants/codename/en-US:
    get:
      summary: View a language variant by language codename
      description: Retrieve content of a variant of a content item. The content item
        is specified by its internal ID and the project language is specified by its
        codename.
      operationId: Items3120ec15A4a247ec8ccdC85ac8ac5ba5VariantsCodenameEnUSGet
      x-api-path-slug: items3120ec15a4a247ec8ccdc85ac8ac5ba5variantscodenameenus-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Language
      - Variant
      - By
      - Language
      - Codename
    put:
      summary: Upsert a variant by language codename
      description: "Add content to a variant in an active project language, or update
        an existing language variant. The content item is specified by its internal
        ID and the project language is specified by its codename.\r\n\r\n**Note:**
        Only the elements specified in the request body will be modified. Any existing
        comments attached to these elements will be lost on update."
      operationId: Items3120ec15A4a247ec8ccdC85ac8ac5ba5VariantsCodenameEnUSPut
      x-api-path-slug: items3120ec15a4a247ec8ccdc85ac8ac5ba5variantscodenameenus-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Upsert
      - Variant
      - By
      - Language
      - Codename
    delete:
      summary: Delete a variant by language codename
      description: "Delete a specific language variant. The content item is specified
        by its external ID and the project language is specified by its codename.\r\n\r\nNote
        that when you delete the last variant of a content item, the whole content
        item is deleted."
      operationId: Items3120ec15A4a247ec8ccdC85ac8ac5ba5VariantsCodenameEnUSDelete3
      x-api-path-slug: items3120ec15a4a247ec8ccdc85ac8ac5ba5variantscodenameenus-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Variant
      - By
      - Language
      - Codename
  /items/external-id/ext-cafe-brno-59713/variants/codename/en-US:
    put:
      summary: Adding localized content
      description: "Add content in a specific language to your new content item by
        performing an upsert.\r\n\r\n* In the request URL, you need to specify the
        content item you are importing to (for example, `/items/external-id/ext-cafe-brno-59713`)
        and the language of the variant (for example, `/variants/codename/en-US`).\r\n*
        The request body must contain the `elements` object in which you specify only
        the content elements you want to update. Omitted elements will remain unchanged.\r\n\r\nSee
        <https://developer.kenticocloud.com/docs/importing-to-kentico-cloud#section-2-adding-localized-content>
        for more details."
      operationId: ItemsExternalIdExtCafeBrno59713VariantsCodenameEnUSPut
      x-api-path-slug: itemsexternalidextcafebrno59713variantscodenameenus-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Ing
      - Localized
      - Content
  /visitor/569030c7-52a5-44f5-a243-c5285b3eb24e/7888c9a3824a11f1/segments:
    get:
      summary: List segments of a visitor
      description: Retrieve the names of segments that the specified visitor belongs
        to.
      operationId: Visitor569030c752a544f5A243C5285b3eb24e7888c9a3824a11f1SegmentsGet
      x-api-path-slug: visitor569030c752a544f5a243c5285b3eb24e7888c9a3824a11f1segments-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Segments
      - Of
      - Visitor
  /items/external-id/ext-cafe-brno-59713:
    put:
      summary: Creating a content item
      description: "One of the ways to import content to your project is to send a
        PUT request to the `<cmApiUrl>/items/external-id/<your item ID>` endpoint.\r\n\r\nIn
        the body of the request, specify these properties:\r\n\r\n* `name` \u2013
        string with a display name of the new content item.\r\n* `type` \u2013 reference
        to a content type.\r\n* (Optional) `sitemap_locations` \u2013 array of references
        to sitemap locations.\r\n\r\nSee <https://developer.kenticocloud.com/docs/importing-to-kentico-cloud#section-1-creating-a-content-item>
        for more details."
      operationId: ItemsExternalIdExtCafeBrno59713Put
      x-api-path-slug: itemsexternalidextcafebrno59713-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Creating
      - Content
      - Item
  /items/3120ec15-a4a2-47ec-8ccd-c85ac8ac5ba5/variants/00000000-0000-0000-0000-000000000000:
    get:
      summary: View a language variant by language ID
      description: Retrieve content of a language variant of a content item. Both
        the content item and the project language are specified by their internal
        IDs.
      operationId: Items3120ec15A4a247ec8ccdC85ac8ac5ba5Variants00000000000000000000000000000000Get
      x-api-path-slug: items3120ec15a4a247ec8ccdc85ac8ac5ba5variants00000000000000000000000000000000-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Language
      - Variant
      - By
      - Language
      - ID
    put:
      summary: Upsert a variant by language ID
      description: "Add content to a variant in an active project language, or update
        an existing language variant. Both the content item and project language are
        specified by their internal IDs.\r\n\r\n**Note:** Only the elements specified
        in the request body will be modified. Any existing comments attached to these
        elements will be lost on update."
      operationId: Items3120ec15A4a247ec8ccdC85ac8ac5ba5Variants00000000000000000000000000000000Put
      x-api-path-slug: items3120ec15a4a247ec8ccdc85ac8ac5ba5variants00000000000000000000000000000000-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Upsert
      - Variant
      - By
      - Language
      - ID
    delete:
      summary: Delete a variant by language ID
      description: "Delete a specific language variant. Both the content item and
        the project language are specified by their internal IDs.\r\n\r\nNote that
        when you delete the last variant of a content item, the whole content item
        is deleted."
      operationId: Items3120ec15A4a247ec8ccdC85ac8ac5ba5Variants00000000000000000000000000000000Delete
      x-api-path-slug: items3120ec15a4a247ec8ccdc85ac8ac5ba5variants00000000000000000000000000000000-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Variant
      - By
      - Language
      - ID
  /assets/external-id/which-brewing-fits-you:
    get:
      summary: View an asset by external ID
      description: Retrieve information about a single asset specified by its external
        ID.
      operationId: AssetsExternalIdWhichBrewingFitsYouGet
      x-api-path-slug: assetsexternalidwhichbrewingfitsyou-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Asset
      - By
      - External
      - ID
    put:
      summary: Upsert an asset by external ID
      description: "Add a new asset or update an existing asset specified by its external
        ID.\r\n\r\n**Note:** If no asset with the specified external ID exists in
        the project, the system will try to create one. For existing assets, the API
        updates only the specified asset's descriptions and title."
      operationId: AssetsExternalIdWhichBrewingFitsYouPut
      x-api-path-slug: assetsexternalidwhichbrewingfitsyou-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Upsert
      - Asset
      - By
      - External
      - ID
    delete:
      summary: Delete an asset by ID
      description: Removes an unused asset specified by its external ID.
      operationId: AssetsExternalIdWhichBrewingFitsYouDelete
      x-api-path-slug: assetsexternalidwhichbrewingfitsyou-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Asset
      - By
      - ID
  /assets:
    get:
      summary: List assets
      description: Retrieve a dynamically paginated list of assets.
      operationId: AssetsGet
      x-api-path-slug: assets-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Assets
    post:
      summary: Add an asset
      description: "Use a file reference to link an existing [binary file](https://developer.kenticocloud.com/v1/reference#content-management-api-upload-file)
        to a new asset. You can also create assets by upserting (`PUT /assets/external-id/<external_id>`),
        see [Upsert an asset](https://developer.kenticocloud.com/v1/reference#content-management-api-upsert-asset-by-external-id).\r\n\r\n**Note:**
        Each binary file can be referenced only by a single asset."
      operationId: AssetsPost
      x-api-path-slug: assets-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Asset
  /8d155914-6674-4f17-8104-3b1c5c2b37e4/items/partner_promotion:
    get:
      summary: Displaying the right content
      description: |-
        Retrieve one personalization variant you want to display. To learn more about retrieving content, consult the [Delivery API reference](https://developer.kenticocloud.com/reference#delivery-api).

        See <https://developer.kenticocloud.com/docs/personalizing-content#section-displaying-the-right-content> for more examples.
      operationId: 8d15591466744f1781043b1c5c2b37e4ItemsPartnerPromotionGet
      x-api-path-slug: 8d15591466744f1781043b1c5c2b37e4itemspartner-promotion-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Displaying
      - Right
      - Content
  /assets/fcbb12e6-66a3-4672-85d9-d502d16b8d9c:
    get:
      summary: View an asset by ID
      description: "Modifies properties of an asset specified by its internal ID.\r\n\r\nNote:
        This endpoint only allows updating of asset descriptions and title."
      operationId: AssetsFcbb12e666a3467285d9D502d16b8d9cGet
      x-api-path-slug: assetsfcbb12e666a3467285d9d502d16b8d9c-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Asset
      - By
      - ID
    put:
      summary: Update an asset by ID
      description: Retrieve a dynamically paginated list of assets.
      operationId: AssetsFcbb12e666a3467285d9D502d16b8d9cPut
      x-api-path-slug: assetsfcbb12e666a3467285d9d502d16b8d9c-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Asset
      - By
      - ID
    delete:
      summary: Delete an asset by ID
      description: Removes an unused asset specified by its internal ID.
      operationId: AssetsFcbb12e666a3467285d9D502d16b8d9cDelete
      x-api-path-slug: assetsfcbb12e666a3467285d9d502d16b8d9c-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Asset
      - By
      - ID
  /items/external-id/59713/variants/00000000-0000-0000-0000-000000000000:
    get:
      summary: View a language variant by language ID
      description: Retrieve content of a variant of a content item. The content item
        is specified by its external ID and the project language is specified by its
        internal ID.
      operationId: ItemsExternalId59713Variants00000000000000000000000000000000Get
      x-api-path-slug: itemsexternalid59713variants00000000000000000000000000000000-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Language
      - Variant
      - By
      - Language
      - ID
    put:
      summary: Upsert a variant by language ID
      description: "Add content to a variant in an active project language, or update
        an existing language variant. The content item is specified by its external
        ID and the project language is specified by its internal ID.\r\n\r\n**Note:**
        Only the elements specified in the request body will be modified. Any existing
        comments attached to these elements will be lost on update."
      operationId: ItemsExternalId59713Variants00000000000000000000000000000000Put
      x-api-path-slug: itemsexternalid59713variants00000000000000000000000000000000-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Upsert
      - Variant
      - By
      - Language
      - ID
    delete:
      summary: Delete a variant by language ID
      description: "Delete a specific language variant. The content item is specified
        by its external ID and the project language is specified by its internal ID.\r\n\r\nNote
        that when you delete the last variant of a content item, the whole content
        item is deleted."
      operationId: ItemsExternalId59713Variants00000000000000000000000000000000Delete
      x-api-path-slug: itemsexternalid59713variants00000000000000000000000000000000-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Variant
      - By
      - Language
      - ID
  /items/external-id/59713/variants/codename/en-US:
    get:
      summary: View a language variant by language codename
      description: Retrieve content of a variant of a content item. The content item
        is specified by its external ID and the project language is specified by its
        codename.
      operationId: ItemsExternalId59713VariantsCodenameEnUSGet
      x-api-path-slug: itemsexternalid59713variantscodenameenus-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Language
      - Variant
      - By
      - Language
      - Codename
    put:
      summary: Upsert a variant by language codename
      description: "Add content to a variant in an active project language, or update
        an existing language variant. The content item is specified by its external
        ID and the project language is specified by its codename.\r\n\r\n**Note:**
        Only the elements specified in the request body will be modified. Any existing
        comments attached to these elements will be lost on update."
      operationId: ItemsExternalId59713VariantsCodenameEnUSPut
      x-api-path-slug: itemsexternalid59713variantscodenameenus-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Upsert
      - Variant
      - By
      - Language
      - Codename
  /contact:
    post:
      summary: Create a contact profile
      description: Submit the visitor's email address and other information.
      operationId: ContactPost
      x-api-path-slug: contact-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Profile
  /activity:
    post:
      summary: Record a custom activity
      description: Log a custom action for a specified visitor.
      operationId: ActivityPost
      x-api-path-slug: activity-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Record
      - Custom
      - Activity
  /session:
    post:
      summary: Record a new session
      description: Log a new session for a specified visitor.
      operationId: SessionPost
      x-api-path-slug: session-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Record
      - New
      - Session
  /975bf280-fd91-488c-994c-2f04416e5ee3/items/on_roasts:
    get:
      summary: Getting localized content items
      description: |-
        Get a content item in a specific language variant by using the `language` parameter.

        See [Getting localized content items](https://developer.kenticocloud.com/docs/localization#section-getting-localized-content-items) for more details.
      operationId: 975bf280Fd91488c994c2f04416e5ee3ItemsOnRoastsGet3
      x-api-path-slug: 975bf280fd91488c994c2f04416e5ee3itemson-roasts-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: language
      responses:
        200:
          description: OK
      tags:
      - Ting
      - Localized
      - Content
      - Items
  /items/external-id/59713:
    get:
      summary: View a content Item by external ID
      description: Retrieve metadata information about a content item specified by
        its external ID.
      operationId: ItemsExternalId59713Get
      x-api-path-slug: itemsexternalid59713-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Content
      - Item
      - By
      - External
      - ID
    put:
      summary: Update a content item by external ID
      description: "Add a new content item or update an existing content item specified
        by its external ID.\r\n\r\n**Note:** If no content item with the specified
        external ID exists in the project, the system will try to create one. For
        existing content items, the API updates the content item's name and sitemap
        locations.\r\nYou can also specify the external ID when [adding content items](https://developer.kenticocloud.com/v1/reference#content-management-api-add-item)
        via the POST method."
      operationId: ItemsExternalId59713Put
      x-api-path-slug: itemsexternalid59713-put
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Content
      - Item
      - By
      - External
      - ID
  /items/codename/on_roasts/variants:
    get:
      summary: List language variants
      description: Retrieve a list of language variants of a content item specified
        by its codename.
      operationId: ItemsCodenameOnRoastsVariantsGet
      x-api-path-slug: itemscodenameon-roastsvariants-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Language
      - Variants
  /975bf280-fd91-488c-994c-2f04416e5ee3/taxonomies/personas:
    get:
      summary: View a taxonomy group
      description: |-
        Retrieve a specific taxonomy group from your project by specifying its codename.

        See <https://developer.kenticocloud.com/v1/reference#view-a-taxonomy-group> for more details.
      operationId: 975bf280Fd91488c994c2f04416e5ee3TaxonomiesPersonasGet
      x-api-path-slug: 975bf280fd91488c994c2f04416e5ee3taxonomiespersonas-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Taxonomy
      - Group
  /uid/7888c9a3824a11f1:
    get:
      summary: View data of visitor by ID
      description: ""
      operationId: Uid7888c9a3824a11f1Get
      x-api-path-slug: uid7888c9a3824a11f1-get
      responses:
        200:
          description: OK
      tags:
      - View
      - Data
      - Of
      - Visitor
      - By
      - ID
    delete:
      summary: Delete data of visitor by ID
      description: ""
      operationId: Uid7888c9a3824a11f1Delete
      x-api-path-slug: uid7888c9a3824a11f1-delete
      responses:
        200:
          description: OK
      tags:
      - Data
      - Of
      - Visitor
      - By
      - ID
  /items/3120ec15-a4a2-47ec-8ccd-c85ac8ac5ba5/variants:
    get:
      summary: List language variants
      description: Retrieve a list of language variants of a content item specified
        by its internal ID.
      operationId: Items3120ec15A4a247ec8ccdC85ac8ac5ba5VariantsGet
      x-api-path-slug: items3120ec15a4a247ec8ccdc85ac8ac5ba5variants-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Language
      - Variants
  /975bf280-fd91-488c-994c-2f04416e5ee3/types/coffee:
    get:
      summary: View a content type
      description: |-
        Retrieve a specific content type from your project by specifying its codename.

        See <https://developer.kenticocloud.com/v1/reference#view-a-content-type> for more details.
      operationId: 975bf280Fd91488c994c2f04416e5ee3TypesCoffeeGet
      x-api-path-slug: 975bf280fd91488c994c2f04416e5ee3typescoffee-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Content
      - Type
  /segment/569030c7-52a5-44f5-a243-c5285b3eb24e/{SegmentName}/visitors:
    get:
      summary: List visitors of a segment
      description: Retrieve visitors that match the specified segment.
      operationId: Segment569030c752a544f5A243C5285b3eb24eVisitorsBySegmentNameGet
      x-api-path-slug: segment569030c752a544f5a243c5285b3eb24esegmentnamevisitors-get
      parameters:
      - in: path
        name: SegmentName
      responses:
        200:
          description: OK
      tags:
      - List
      - Visitors
      - Of
      - Segment
  /items:
    get:
      summary: List content items
      description: Retrieve a dynamically paginated list of content items.
      operationId: ItemsGet
      x-api-path-slug: items-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Content
      - Items
    post:
      summary: Add a content item
      description: |-
        Create a new content item based on a specific content type. Content items do NOT contain any content themselves, but serve as wrappers for individual language variants.

        See <https://developer.kenticocloud.com/v1/reference#content-management-api-add-item> for details about adding content to a specific language variant.

        If you are importing content from a different system and want to use the same identifiers for your content as in the previous system, you can use the `external_id` body attribute to set a custom identifier for the new content item.
      operationId: ItemsPost
      x-api-path-slug: items-post
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Content
      - Item
  /975bf280-fd91-488c-994c-2f04416e5ee3/taxonomies:
    get:
      summary: List taxonomy groups
      description: |-
        Retrieve a paginated list of taxonomy groups in your project.

        By default, the API returns all taxonomy groups ordered alphabetically by codename, but [pagination can be customized](https://developer.kenticocloud.com/v1/reference#listing-response).

        See <https://developer.kenticocloud.com/v1/reference#list-taxonomy-groups> for more details.
      operationId: 975bf280Fd91488c994c2f04416e5ee3TaxonomiesGet
      x-api-path-slug: 975bf280fd91488c994c2f04416e5ee3taxonomies-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Taxonomy
      - Groups
  /visitor/569030c7-52a5-44f5-a243-c5285b3eb24e/e3e9e191a12b9257/segment:
    get:
      summary: Retrieving visitor's segments
      description: "Use the Personalization API to retrieve the list of segments that
        the specified visitor belongs to.\n\n* Authenticate the request using your
        Personalization API Key.\n* Specify the User ID of the visitor you are asking
        about.\n \nSee <https://developer.kenticocloud.com/docs/personalizing-content#section-retrieving-visitor-s-segments>
        for more details."
      operationId: Visitor569030c752a544f5A243C5285b3eb24eE3e9e191a12b9257SegmentGet
      x-api-path-slug: visitor569030c752a544f5a243c5285b3eb24ee3e9e191a12b9257segment-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Retrieving
      - Visitors
      - Segments
  /items/codename/on_roasts/variants/00000000-0000-0000-0000-000000000000:
    get:
      summary: View a language variant by language ID
      description: Retrieve content of a variant of a content item. The content item
        is specified by codename and the project language is specified its internal
        ID.
      operationId: ItemsCodenameOnRoastsVariants00000000000000000000000000000000Get
      x-api-path-slug: itemscodenameon-roastsvariants00000000000000000000000000000000-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Language
      - Variant
      - By
      - Language
      - ID
    put:
      summary: Upsert a variant by language ID
      description: "Add content to a variant in an active project language, or update
        an existing language variant. The content item is specified by its codename
        and the project language is specified by its internal ID.\r\n\r\n**Note:**
        Only the elements specified in the request body will be modified. Any existing
        comments attached to these elements will be lost on update."
      operationId: ItemsCodenameOnRoastsVariants00000000000000000000000000000000Put
      x-api-path-slug: itemscodenameon-roastsvariants00000000000000000000000000000000-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Upsert
      - Variant
      - By
      - Language
      - ID
    delete:
      summary: Delete a variant by language ID
      description: "Delete a specific language variant. The content item is specified
        by codename and the project language is specified its internal ID.\r\n\r\nNote
        that when you delete the last variant of a content item, the whole content
        item is deleted."
      operationId: ItemsCodenameOnRoastsVariants00000000000000000000000000000000Delete
      x-api-path-slug: itemscodenameon-roastsvariants00000000000000000000000000000000-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Variant
      - By
      - Language
      - ID
  /975bf280-fd91-488c-994c-2f04416e5ee3/types:
    get:
      summary: List content types
      description: |-
        Retrieve a list of content types in your project.

        See <https://developer.kenticocloud.com/v1/reference#list-content-types> for more details.
      operationId: 975bf280Fd91488c994c2f04416e5ee3TypesGet
      x-api-path-slug: 975bf280fd91488c994c2f04416e5ee3types-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Content
      - Types
  /items/codename/on_roasts/variants/codename/en-US:
    get:
      summary: View a language variant by language codename
      description: Retrieve content of a language variant of a content item. Both
        the content item and the language are specified by their codenames.
      operationId: ItemsCodenameOnRoastsVariantsCodenameEnUSGet
      x-api-path-slug: itemscodenameon-roastsvariantscodenameenus-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Language
      - Variant
      - By
      - Language
      - Codename
    put:
      summary: Upsert a variant by language codename
      description: "Add content to a variant in an active project language, or update
        an existing language variant. Both the content item and project language are
        specified by their codenames.\r\n\r\n**Note:** Only the elements specified
        in the request body will be modified. Any existing comments attached to these
        elements will be lost on update."
      operationId: ItemsCodenameOnRoastsVariantsCodenameEnUSPut
      x-api-path-slug: itemscodenameon-roastsvariantscodenameenus-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Upsert
      - Variant
      - By
      - Language
      - Codename
  /:
    get:
      summary: Getting items by localized URL slug
      description: "Get a *Home* content item whose URL slug in Spanish is *inicio*
        by using the following parameters:\n\n* `language=es-ES` \u2013 specifies
        the codename of the requested language.\n* `system.type=home` \u2013 filters
        content items by their content type.\n* `elements.url_pattern=inicio` \u2013
        filters content items by a value of a specific content element.\n\nSee [Getting
        items by localized URL slug](https://developer.kenticocloud.com/docs/localization#section-getting-items-by-localized-url-slug)
        for more details."
      operationId: UnnammedEndpointGet
      x-api-path-slug: get
      responses:
        200:
          description: OK
      tags:
      - Ting
      - Items
      - By
      - Localized
      - URL
      - Slug
  /validate:
    post:
      summary: Validate project content
      description: "Check your project's content items for issues, such as:\r\n\r\n*
        Content elements are [referencing](https://developer.kenticocloud.com/v1/reference#content-management-api-reference-object)
        non-existing objects.\r\n* Values of certain content elements do not meet
        the limitations set in content types.\r\n\r\nUse the endpoint after successfully
        importing content to your project."
      operationId: ValidatePost
      x-api-path-slug: validate-post
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Validate
      - Project
      - Content
  /items/external-id/59713/variants:
    get:
      summary: List language variants
      description: Retrieve a list of language variants of a content item specified
        by its external ID.
      operationId: ItemsExternalId59713VariantsGet
      x-api-path-slug: itemsexternalid59713variants-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Language
      - Variants
  /email/lola.mira@blabla.com:
    get:
      summary: View data of visitor by email
      description: ""
      operationId: EmailLolaMiraBlablaComGet
      x-api-path-slug: emaillola-mirablabla-com-get
      responses:
        200:
          description: OK
      tags:
      - View
      - Data
      - Of
      - Visitor
      - By
      - Email
    delete:
      summary: Delete data of visitor by email
      description: ""
      operationId: EmailLolaMiraBlablaComDelete
      x-api-path-slug: emaillola-mirablabla-com-delete
      responses:
        200:
          description: OK
      tags:
      - Data
      - Of
      - Visitor
      - By
      - Email
  /files/which-brewing-fits-you-1080px.jpg:
    post:
      summary: Upload a binary file
      description: "Add a new file. The uploaded file will not be visible in the Kentico
        Cloud UI unless there is an asset using it, see how to [add an asset](https://developer.kenticocloud.com/v1/reference#content-management-api-add-asset).\r\n\r\n**Note:**
        Maximum size limit for binary files is 100 MB."
      operationId: FilesWhichBrewingFitsYou1080pxJpgPost
      x-api-path-slug: fileswhichbrewingfitsyou1080px-jpg-post
      parameters:
      - in: header
        name: Content-Length
        description: Specifies the size of the binary file in bytes
      - in: header
        name: Content-Type
        description: Specifies the media type of the binary data
      - in: formData
        name: File
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Binary
      - File
  /which_brewing_fits_you_:
    get:
      summary: Previewing an article
      description: |-
        Preview a specific content item.

        See <https://developer.kenticocloud.com/docs/preview-content-via-api> for details.
      operationId: WhichBrewingFitsYouGet
      x-api-path-slug: which-brewing-fits-you--get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Previewing
      - Article
  /975bf280-fd91-488c-994c-2f04416e5ee3/types/coffee/elements/processing:
    get:
      summary: View a content type element
      description: |-
        Retrieve a specific content type element by specifying its codename and its parent content type.

        See <https://developer.kenticocloud.com/v1/reference#view-a-content-type-element> for more details.
      operationId: 975bf280Fd91488c994c2f04416e5ee3TypesCoffeeElementsProcessingGet
      x-api-path-slug: 975bf280fd91488c994c2f04416e5ee3typescoffeeelementsprocessing-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Content
      - Type
      - Element