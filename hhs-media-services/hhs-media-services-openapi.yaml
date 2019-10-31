swagger: "2.0"
x-collection-name: HHS Media Services
x-complete: 1
info:
  title: HHS Media Services
  description: div-classswaggeruiwrap-extrafooterh3common-features--behaviorsh3----div-classfeatures--------ul------------listrong-sort-paramstrong-supports-multi-column-sorting-through-the-use-of-commas-as-delimiters-and-a-hyphen-to-denote-descending-order-----------------br----------------strongspanexamplesspanstrong----------------ul--------------------lispan-classexamplenamespanspan-classdescriptionsort-results-by-name-ascendingspanli--------------------lispan-classexamplenamespanspan-classdescriptionsort-results-by-name-descendingspanli--------------------lispan-classexamplenameidspanspan-classdescriptionsort-results-by-name-descending-and-then-by-id-ascendingspanli--------------------lispan-classexampleiddatecontentauthoredspanspan-classdescriptionsort-results-by-id-ascending-and-then-date-descendingspanli----------------ul------------li------------listrongdate-formatsstrong-date-input-format-is-expected-to-be-based-on-a-hrefhttpwww-ietf-orgrfcrfc3339-txtrfc-3339a--br----------------spanstrongexamplestrongspan----------------ulli20131118t184301zliul------------li--------ul----divdiv
  termsOfService: http://www.hhs.gov/web/socialmedia/policies/tos.html#ready
  version: "2"
host: api.digitalmedia.hhs.gov
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /resources.json:
    get:
      summary: Get Resources by search query
      description: Returns the list of Resources matching the search query 'q'.The
        search query 'q' is a Lucene query.The syntax for a Lucene query can be found
        here.
      operationId: getResources
      x-api-path-slug: resources-json-get
      parameters:
      - in: query
        name: q
        description: The search query supplied by the user
      responses:
        200:
          description: OK
      tags:
      - Resources
  /resources/campaigns.json:
    get:
      summary: Get Campaigns
      description: Returns the list of Campaigns.
      operationId: getCampaigns
      x-api-path-slug: resourcescampaigns-json-get
      parameters:
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: sort
        description: '* Set of fields to sort the records by'
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Campaigns
  /resources/campaigns/{id}.json:
    get:
      summary: Get Campaign by ID
      description: Returns the Campaign identified by the 'id'.
      operationId: getCampaignById
      x-api-path-slug: resourcescampaignsid-json-get
      parameters:
      - in: path
        name: id
        description: The id of the record to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Campaigns
      - Id
  /resources/campaigns/{id}/media.json:
    get:
      summary: Get MediaItems by Campaign ID
      description: Returns the list of MediaItems for the Campaign identified by the
        'id'.
      operationId: getMediaByCampaignId
      x-api-path-slug: resourcescampaignsidmedia-json-get
      parameters:
      - in: path
        name: id
        description: The id of the campaign to find media items for
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: sort
        description: The name of the property to which sorting will be applied
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Campaigns
      - Id
      - Media
  /resources/campaigns/{id}/syndicate.json:
    get:
      summary: Get MediaItems for Campaign
      description: Renders the list of MediaItems associated with the Campaign identified
        by the 'id'.
      operationId: renders-the-list-of-mediaitems-associated-with-the-campaign-identified-by-the-id-
      x-api-path-slug: resourcescampaignsidsyndicate-json-get
      parameters:
      - in: query
        name: displayMethod
        description: Method used to render an html request
      - in: path
        name: id
        description: The id of the record to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Campaigns
      - Id
      - Syndicate
  /resources/languages.json:
    get:
      summary: Get Languages
      description: Returns the list Languages.
      operationId: getLanguages
      x-api-path-slug: resourceslanguages-json-get
      parameters:
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: sort
        description: '* Set of fields to sort the records by'
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Languages
  /resources/languages/{id}.json:
    get:
      summary: Get Language by ID
      description: Returns the Language identified by the 'id'.
      operationId: getLanguageById
      x-api-path-slug: resourceslanguagesid-json-get
      parameters:
      - in: path
        name: id
        description: The id of the language to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Languages
      - Id
  /resources/media.json:
    get:
      summary: Get MediaItems
      description: Returns the list of MediaItems matching the specified query parameters.
      operationId: getMedia
      x-api-path-slug: resourcesmedia-json-get
      parameters:
      - in: query
        name: collectionId
        description: Restrict filtering to media items in a specific collection
      - in: query
        name: contentAuthoredBeforeDate
        description: Find all media items authored before the provided day (RFC 3339,
          time ignored)
      - in: query
        name: contentAuthoredInRange
        description: Find all media items authored between the provided start and
          end days (RFC 3339, comma separated, time ignored)
      - in: query
        name: contentAuthoredSinceDate
        description: Find all media items authored since the provided day (RFC 3339,
          time ignored)
      - in: query
        name: contentPublishedBeforeDate
        description: Find all media items published before the provided day (RFC 3339,
          time ignored)
      - in: query
        name: contentPublishedInRange
        description: Find all media items published between the provided start and
          end days (RFC 3339, comma separated, time ignored)
      - in: query
        name: contentPublishedSinceDate
        description: Find all media items published since the provided day (RFC 3339,
          time ignored)
      - in: query
        name: contentReviewedBeforeDate
        description: Find all media items reviewed before the provided day (RFC 3339,
          time ignored)
      - in: query
        name: contentReviewedInRange
        description: Find all media items reviewed between the provided start and
          end days (RFC 3339, comma separated, time ignored)
      - in: query
        name: contentReviewedSinceDate
        description: Find all media items reviewed since the provided day (RFC 3339,
          time ignored)
      - in: query
        name: contentUpdatedBeforeDate
        description: Find all media items updated before the provided day (RFC 3339,
          time ignored)
      - in: query
        name: contentUpdatedInRange
        description: Find all media items updated between the provided start and end
          days (RFC 3339, comma separated, time ignored)
      - in: query
        name: contentUpdatedSinceDate
        description: Find all media items updated since the provided day (RFC 3339,
          time ignored)
      - in: query
        name: createdBy
        description: Find all media items containing the createdBy value
      - in: query
        name: customThumbnailUrl
        description: Find all media items which have the provided customThumbnailUrl,
          case insensitive
      - in: query
        name: customThumbnailUrlContains
        description: Find all media items which contain the provided partial customThumbnailUrl,
          case insensitive
      - in: query
        name: dateContentAuthored
        description: Find all media items authored on the provided day (RFC 3339,
          time ignored)
      - in: query
        name: dateContentPublished
        description: Find all media items published on the provided day (RFC 3339,
          time ignored)
      - in: query
        name: dateContentReviewed
        description: Find all media items reviewed on the provided day (RFC 3339,
          time ignored)
      - in: query
        name: dateContentUpdated
        description: Find all media items updated on the provided day (RFC 3339, time
          ignored)
      - in: query
        name: dateSyndicationCaptured
        description: Find all media items authored on the provided day (RFC 3339,
          time ignored)
      - in: query
        name: dateSyndicationUpdated
        description: Find all media items updated on the provided day, (RFC 3339,
          time ignored)
      - in: query
        name: descriptionContains
        description: Find all media items containing the provided partial description,
          case insensitive
      - in: query
        name: hash
        description: Find all media items which match the provided hash, case insensitive
      - in: query
        name: hashContains
        description: Find all media items which match the provided partial hash, case
          insensitive
      - in: query
        name: languageId
        description: Find all media items written in the language specified by Id
      - in: query
        name: languageIsoCode
        description: Find all media items written in the language specified by 639-2
          isoCode , case insensitive
      - in: query
        name: languageName
        description: Find all media items written in the language specified by name,
          case insensitive
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: mediaTypes
        description: Find all media items belonging to the specified media type[s]
      - in: query
        name: name
        description: Find all media items containing the provided name, case insensitive
      - in: query
        name: nameContains
        description: Find all media items containing the partial name, case insensitive
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: order
        description: '* The ascending or descending order'
      - in: query
        name: restrictToSet
        description: Find only media from within the supplied list of Ids
      - in: query
        name: sort
        description: '* Set of fields to sort the records by'
      - in: query
        name: sourceAcronym
        description: Find all media items that belong to the source specified by acronym,
          case insensitive
      - in: query
        name: sourceAcronymContains
        description: Find all media items that belong to the source specified by partial
          acronym, case insensitive
      - in: query
        name: sourceId
        description: Find all media items that belong to the source specified by Id
      - in: query
        name: sourceName
        description: Find all media items that belong to the source specified by name,
          case insensitive
      - in: query
        name: sourceNameContains
        description: Find all media items that belong to the source specified by partial
          name, case insensitive
      - in: query
        name: sourceUrl
        description: Find all media items which have the provided sourceUrl, case
          insensitive
      - in: query
        name: sourceUrlContains
        description: Find all media items which contain the provided partial sourceUrl,
          case insensitive
      - in: query
        name: syndicationCapturedBeforeDate
        description: Find all media items authored before the provided day (RFC 3339,
          time ignored)
      - in: query
        name: syndicationCapturedInRange
        description: Find all media items authored between the provided start and
          end days (RFC 3339, comma separated, time ignored)
      - in: query
        name: syndicationCapturedSinceDate
        description: Find all media items authored since the provided day (RFC 3339,
          time ignored)
      - in: query
        name: syndicationUpdatedBeforeDate
        description: Find all media items updated before the provided day, (RFC 3339,
          time ignored)
      - in: query
        name: syndicationUpdatedInRange
        description: Find all media items updated between the provided start and end
          days, (RFC 3339, comma separated, time ignored)
      - in: query
        name: syndicationUpdatedSinceDate
        description: Find all media items updated since the provided day, (RFC 3339,
          time ignored)
      - in: query
        name: syndicationVisibleBeforeDate
        description: Find all media items visible before the provided day, (RFC 3339,
          time ignored)
      - in: query
        name: syndicationVisibleInRange
        description: Find all media items visible between the provided start and end
          days, (RFC 3339, comma separated, time ignored)
      - in: query
        name: syndicationVisibleSinceDate
        description: Find all media items visible since the provided day, (RFC 3339,
          time ignored)
      - in: query
        name: tagIds
        description: Find only media items tagged with the specified tag Ids
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
  /resources/media/featured.json:
    get:
      summary: Get the list of featured content in the syndication system
      description: Get the list of featured content in the syndication system
      operationId: getFeaturedMedia
      x-api-path-slug: resourcesmediafeatured-json-get
      parameters:
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: How many records to offset the query by
      - in: query
        name: sort
        description: '* Set of fields to sort the records by'
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Featured
  /resources/media/mostPopularMedia.json:
    get:
      summary: Get MediaItems by popularity
      description: Returns the list of MediaItems with the highest ratings.
      operationId: getMostPopularMedia
      x-api-path-slug: resourcesmediamostpopularmedia-json-get
      parameters:
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - MostPopularMedia
  /resources/media/searchResults.json:
    get:
      summary: Get MediaItems by search query
      description: Returns the list of MediaItems matching the search query 'q'.The
        search query 'q' is a Lucene query.The syntax for a Lucene query can be found
        here
      operationId: searchMedia
      x-api-path-slug: resourcesmediasearchresults-json-get
      parameters:
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: q
        description: The search query supplied by the user
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - SearchResults
  /resources/media/{id}.json:
    get:
      summary: Get MediaItem by ID
      description: Returns the MediaItem identified by the 'id'.
      operationId: getMediaById
      x-api-path-slug: resourcesmediaid-json-get
      parameters:
      - in: path
        name: id
        description: The id of the record to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Id
  /resources/media/{id}/content:
    get:
      summary: Get content for MediaItem
      description: Returns the raw content (html, image, etc...) for the MediaItem
        identified by the 'id'.
      operationId: getMediaContentById
      x-api-path-slug: resourcesmediaidcontent-get
      parameters:
      - in: query
        name: calledByBuild
        description: The method that called this method
      - in: path
        name: id
        description: The id of the media to show content for
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Id
      - Content
  /resources/media/{id}/embed.json:
    get:
      summary: Get embed code for MediaItem
      description: Returns the javascript or iframe embed code for the MediaItem identified
        by 'id'.
      operationId: getMediaEmbedById
      x-api-path-slug: resourcesmediaidembed-json-get
      parameters:
      - in: query
        name: displayMethod
        description: Method used to render an html request
      - in: query
        name: divId
        description: Should the div to insert content into have a specific name?
      - in: query
        name: excludeDiv
        description: Should the div to insert content into be omitted?
      - in: query
        name: excludeJquery
        description: Should a reference to the JQuery Library be omitted?
      - in: query
        name: flavor
        description: Currently supports iframe, defaults to javascript
      - in: query
        name: height
        description: The height of the generated iframe
      - in: path
        name: id
        description: The id of the media to get embed code for
      - in: query
        name: iframeName
        description: The name of the iframe element
      - in: query
        name: width
        description: The width of the generated iframe
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Id
      - Embed
  /resources/media/{id}/preview.jpg:
    get:
      summary: Get JPG preview for MediaItem
      description: Returns the JPG preview, where applicable, for the MediaItem identified
        by the 'id'.
      operationId: getMediaPreviewById
      x-api-path-slug: resourcesmediaidpreview-jpg-get
      parameters:
      - in: path
        name: id
        description: The id of the media to get a preview for
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Id
      - Preview
      - Jpg
  /resources/media/{id}/ratings.json:
    get:
      summary: Get Ratings for MediaItem
      description: Get the Ratings (number of 'likes') for the MediaItem identified
        by the 'id'.
      operationId: getMediaRatingsById
      x-api-path-slug: resourcesmediaidratings-json-get
      parameters:
      - in: path
        name: id
        description: The ID of the media item to like
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Id
      - Ratings
  /resources/media/{id}/relatedMedia.json:
    get:
      summary: Get related MediaItems by ID
      description: Returns the list of MediaItems related to the MediaItem identified
        by the 'id'.
      operationId: getRelatedMediaById
      x-api-path-slug: resourcesmediaidrelatedmedia-json-get
      parameters:
      - in: path
        name: id
        description: The id of the media item to get related media for
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: sort
        description: Which field to sort the records by
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Id
      - RelatedMedia
  /resources/media/{id}/syndicate.json:
    get:
      summary: Get syndicated content for MediaItem
      description: Returns the syndicated content for a given MediaItem in the specified
        'format' (HTML or JSON).
      operationId: getMediaSyndicateById
      x-api-path-slug: resourcesmediaidsyndicate-json-get
      parameters:
      - in: query
        name: autoplay
        description: If content is a video, the embeded video will auto play when
          loaded
      - in: query
        name: cssClass
        description: The css class to target for extraction
      - in: query
        name: font-size
        description: Set font size (in points) of p, div, and span tags
      - in: path
        name: id
        description: The id of the media to show embed code for
      - in: query
        name: imageFloat
        description: Accepts valid CSS float options, such as left or right
      - in: query
        name: imageMargin
        description: Accepts 4 CSV values representing pixel sizes of margin similar
          to CSS
      - in: query
        name: rel
        description: If content is a video, related items will be shown at the end
          of playback
      - in: query
        name: stripBreaks
        description: Remove break tags from content
      - in: query
        name: stripClasses
        description: Remove class attributes from content (except syndicate)
      - in: query
        name: stripImages
        description: Remove image tags from content
      - in: query
        name: stripScripts
        description: Remove script tags from content
      - in: query
        name: stripStyles
        description: Remove in-line styles from content
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Id
      - Syndicate
  /resources/media/{id}/thumbnail.jpg:
    get:
      summary: Get JPG thumbnail for MediaItem
      description: Returns the JPG thumbnail, where applicable, for the MediaItem
        identified by the 'id'.
      operationId: getMediaThumbnailById
      x-api-path-slug: resourcesmediaidthumbnail-jpg-get
      parameters:
      - in: path
        name: id
        description: The id of the media to get a thumbnail for
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Id
      - Thumbnail
      - Jpg
  /resources/media/{id}/youtubeMetaData.json:
    get:
      summary: Get Youtube metadata for MediaItem
      description: Returns the Youtube metadata, where applicable, for the MediaItem
        identified by the 'id'.
      operationId: getMediaYoutubeMetaDataById
      x-api-path-slug: resourcesmediaidyoutubemetadata-json-get
      parameters:
      - in: path
        name: id
        description: The id of the video to show meta data for
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Media
      - Id
      - YoutubeMetaData
  /resources/mediaTypes.json:
    get:
      summary: Get MediaTypes
      description: Returns the list of available MediaTypes.
      operationId: getMediaTypes
      x-api-path-slug: resourcesmediatypes-json-get
      responses:
        200:
          description: OK
      tags:
      - Resources
      - MediaTypes
  /resources/sources.json:
    get:
      summary: Get Sources
      description: Returns the list of Sources.
      operationId: getSources
      x-api-path-slug: resourcessources-json-get
      parameters:
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: sort
        description: '* Set of fields to sort the records by'
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Sources
  /resources/sources/{id}.json:
    get:
      summary: Get Source by ID
      description: Returns the Source identified by the 'id'.
      operationId: getSourceById
      x-api-path-slug: resourcessourcesid-json-get
      parameters:
      - in: path
        name: id
        description: The id of the source to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Sources
      - Id
  /resources/sources/{id}/syndicate.json:
    get:
      summary: Get MediaItems for Source
      description: Renders the list of MediaItems associated with the Source identified
        by the 'id'.
      operationId: renders-the-list-of-mediaitems-associated-with-the-source-identified-by-the-id-
      x-api-path-slug: resourcessourcesidsyndicate-json-get
      parameters:
      - in: query
        name: displayMethod
        description: Method used to render an html request
      - in: path
        name: id
        description: The id of the record to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Sources
      - Id
      - Syndicate
  /resources/tags.json:
    get:
      summary: Get Tags
      description: Returns the list of Tags matching the specified query parameters
        in the specified 'format'.
      operationId: getTags
      x-api-path-slug: resourcestags-json-get
      parameters:
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: mediaId
        description: Return tags associated with the supplied media id
      - in: query
        name: name
        description: Return tags[s] matching the supplied name
      - in: query
        name: nameContains
        description: Return tags which contain the supplied partial name
      - in: query
        name: offset
        description: Return records starting at the offset index
      - in: query
        name: sort
        description: The name of the property to which sorting will be applied
      - in: query
        name: typeId
        description: Return tags belonging to the supplied tag type id
      - in: query
        name: typeName
        description: Return tags belonging to the supplied tag type name
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Tags
  /resources/tags/tagLanguages.json:
    get:
      summary: Get TagLanguages
      description: Returns the list of TagLanguages
      operationId: getTagLanguages
      x-api-path-slug: resourcestagstaglanguages-json-get
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Tags
      - TagLanguages
  /resources/tags/tagTypes.json:
    get:
      summary: Get TagTypes
      description: Returns the list of TagTypes
      operationId: getTagTypes
      x-api-path-slug: resourcestagstagtypes-json-get
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Tags
      - TagTypes
  /resources/tags/{id}.json:
    get:
      summary: Get Tag by ID
      description: Returns the Tag identified by the 'id' in the specified 'format'.
      operationId: getTagById
      x-api-path-slug: resourcestagsid-json-get
      parameters:
      - in: path
        name: id
        description: The id of the record to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Tags
      - Id
  /resources/tags/{id}/media.json:
    get:
      summary: Get MediaItems for Tag
      description: Returns the list of MediaItems associated with the Tag identified
        by the 'id'.
      operationId: getMediaByTagId
      x-api-path-slug: resourcestagsidmedia-json-get
      parameters:
      - in: path
        name: id
        description: The id of the record to look up
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: sort
        description: The name of the property to which sorting will be applied
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Tags
      - Id
      - Media
  /resources/tags/{id}/related.json:
    get:
      summary: Get related Tags by ID
      description: Returns the list of Tags related to the Tag identified by the 'id'
        in the specified format.
      operationId: getRelatedTagsById
      x-api-path-slug: resourcestagsidrelated-json-get
      parameters:
      - in: path
        name: id
        description: The id of the tag to look up
      - in: query
        name: max
        description: The maximum number of records to return
      - in: query
        name: offset
        description: The offset of the records set to return for pagination
      - in: query
        name: sort
        description: The name of the property to which sorting will be applied
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Tags
      - Id
      - Related
  /resources/tags/{id}/syndicate.json:
    get:
      summary: Get MediaItems for Tag
      description: Renders the list of MediaItems associated with the Tag identified
        by the 'id'.
      operationId: renders-the-list-of-mediaitems-associated-with-the-tag-identified-by-the-id-
      x-api-path-slug: resourcestagsidsyndicate-json-get
      parameters:
      - in: query
        name: displayMethod
        description: Method used to render an html request
      - in: path
        name: id
        description: The id of the record to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - Tags
      - Id
      - Syndicate
  /resources/userMediaLists/{id}.json:
    get:
      summary: Get UserMediaList by ID
      description: Get a specific user media list by 'id'.
      operationId: getUserMediaList
      x-api-path-slug: resourcesusermedialistsid-json-get
      parameters:
      - in: query
        name: displayMethod
        description: Method used to render an html request
      - in: path
        name: id
        description: The id of the record to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - UserMediaLists
      - Id