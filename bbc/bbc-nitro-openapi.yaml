swagger: "2.0"
x-collection-name: BBC
x-complete: 1
info:
  title: BBC Nitro
  description: bbc-nitro-is-the-bbcs-application-programming-interface-api-for-bbc-programmes-metadata-
  termsOfService: http://www.bbc.co.uk/terms/
  contact:
    name: Open Nitro Project
    url: http://developer.bbc.co.uk/
    email: nitro@bbc.co.uk
  version: 1.0.0
host: programmes.api.bbc.com
basePath: /nitro/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:
    get:
      summary: Get API definition
      description: Get API definition
      operationId: getAPI
      x-api-path-slug: get
      responses:
        200:
          description: OK
      tags:
      - ""
  /availabilities:
    get:
      summary: Discover details of on-demand availability for programmes and their
        versions
      description: Discover details of on-demand availability for programmes and their
        versions
      operationId: listAvailability
      x-api-path-slug: availabilities-get
      parameters:
      - in: query
        name: availability
        description: filter for subset of availabilities
      - in: query
        name: debug
        description: Turn on debug information (undocumented)
      - in: query
        name: descendants_of
        description: filter for subset of availabilities that have PID as ancestor
      - in: query
        name: media_set
        description: filter for subset of availabilities with media set
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: sort
        description: 'Sorts:* scheduled_start: sort chronologically by scheduled start
          time/date, ascending'
      - in: query
        name: sort_direction
        description: Sort direction
      - in: query
        name: territory
        description: filter for availabilities in given territory
      responses:
        200:
          description: OK
      tags:
      - Availabilities
  /broadcasts:
    get:
      summary: Build schedules and find metadata for TV and radio broadcasts
      description: Fetch metadata about linear Broadcasts and Services, allowing the
        generation of Television and Radio schedules and other datasets for broadcast
        items. Use /schedules instead of this feed as it is more efficient. Broadcasts
        will be deprecated in the future.
      operationId: listBroadcasts
      x-api-path-slug: broadcasts-get
      parameters:
      - in: query
        name: authority
        description: filter for subset of broadcasts that have given authority
      - in: query
        name: descendants_of
        description: filter for subset of broadcasts that are descendants of the given
          programme PID
      - in: query
        name: end_from
        description: filter for subset of broadcasts that end on or later than the
          specified datetime
      - in: query
        name: end_to
        description: filter for subset of broadcasts that end on or earlier than the
          specified datetime
      - in: query
        name: format
        description: filter for subset of broadcasts that are classified in the given
          format ID
      - in: query
        name: genre
        description: filter for subset of broadcasts that are classified in the given
          genre ID
      - in: query
        name: id
        description: filter for subset of broadcasts that have given identifier
      - in: query
        name: item
        description: filter for subset of broadcasts with the given item performed
          on it
      - in: query
        name: mixin
        description: 'Mixins:* titles: return ancestor programme titles'
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: people
        description: filter for subset of broadcasts that have given contributor
      - in: query
        name: pid
        description: filter for subset of broadcasts having given PID
      - in: query
        name: q
        description: filter for subset of broadcasts matching supplied keyword/phrase
          (boolean operators permitted)
      - in: query
        name: schedule_day
        description: filter for subset of broadcasts that start on the specified day
          (BBC time)
      - in: query
        name: schedule_day_from
        description: filter for subset of broadcasts that start on or after the specified
          day (BBC time)
      - in: query
        name: schedule_day_to
        description: filter for subset of broadcasts that start on or before the specified
          day (BBC time)
      - in: query
        name: service_master_brand
        description: filter for subset of broadcasts with given service master brand
      - in: query
        name: sid
        description: filter for subset of broadcasts that are on the specified linear
          service
      - in: query
        name: sort
        description: 'Sorts:* start_date: sort chronologically by scheduled start
          time/date, ascending'
      - in: query
        name: sort_direction
        description: Sort direction
      - in: query
        name: start_from
        description: filter for subset of broadcasts that start on or later than the
          specified datetime
      - in: query
        name: start_to
        description: filter for subset of broadcasts that start on or earlier than
          the specified datetime
      - in: query
        name: version
        description: filter for subset of broadcasts with given PID as their parent
          version
      responses:
        200:
          description: OK
      tags:
      - Broadcasts
  /groups:
    get:
      summary: 'Find metadata for curated groups: seasons, collections, galleries
        or franchises'
      description: Long-lived curated collections of programmes and more, including
        Collections, Seasons, Franchises and Galleries
      operationId: listGroups
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: embargoed
        description: Control return of embargoed items (undocumented)
      - in: query
        name: for_descendants_of
        description: filter for groups related to given programme or its descendants
      - in: query
        name: for_programme
        description: filter for subset of groups directly related to a given programme
      - in: query
        name: group
        description: filter for subset of groups which belong to the given group pid
      - in: query
        name: group_type
        description: filter for subset of groups that have the given group type
      - in: query
        name: member
        description: filter for subset of groups which contain an entity with the
          given pid as a member
      - in: query
        name: mixin
        description: 'Mixins:* alternate_images: mixin to return the alternate images
          for a group* group_for: mixin to return links to programme entities that
          group belongs to* images: mixin to add image information for a group* related_links:
          mixin to return related links for the group'
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_id
        description: filter for groups by partner ID
      - in: query
        name: partner_pid
        description: filter for groups by partner PID
      - in: query
        name: pid
        description: filter for subset of seasons, collections, galleries or franchises
          having given PID
      - in: query
        name: q
        description: filter for subset of groups matching supplied keyword/phrase
          (boolean operators permitted)
      - in: query
        name: sort
        description: 'Sorts:* pid: sort alphabetically by PID'
      - in: query
        name: sort_direction
        description: Sort direction
      responses:
        200:
          description: OK
      tags:
      - Groups
  /images:
    get:
      summary: Find metadata for images
      description: Find metadata for images, particularly those in galleries
      operationId: listImages
      x-api-path-slug: images-get
      parameters:
      - in: query
        name: embargoed
        description: Control return of embargoed items (undocumented)
      - in: query
        name: group
        description: filter for images belonging to the given group (i
      - in: query
        name: image_type
        description: filter for images by type
      - in: query
        name: is_alternate_image_for
        description: filter for alternate images by entity PID
      - in: query
        name: is_image_for
        description: filter for images by entity PID
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_id
        description: filter for images by partner ID
      - in: query
        name: partner_pid
        description: filter for images by partner PID
      - in: query
        name: pid
        description: filter for subset of images having given PID
      - in: query
        name: q
        description: filter for subset of images matching supplied keyword/phrase
          (boolean operators permitted)
      - in: query
        name: sort
        description: 'Sorts:* group_position: sort numerically by position, ascending
          only* pid: sort alphabetically by PID'
      - in: query
        name: sort_direction
        description: Sort direction
      responses:
        200:
          description: OK
      tags:
      - Images
  /items:
    get:
      summary: 'Look inside programmes to find segments: chapters, tracks and more'
      description: 'Look inside programmes to find segments: chapters, tracks and
        more'
      operationId: listItems
      x-api-path-slug: items-get
      parameters:
      - in: query
        name: authority
        description: filter for subset of items that have an ID issued by the given
          authority
      - in: query
        name: id
        description: filter for subset of items having given ID
      - in: query
        name: id_type
        description: filter for subset of items that have given an ID of the given
          type
      - in: query
        name: item_type
        description: filter for specific type(s) of items
      - in: query
        name: mixin
        description: 'Mixins:* contributions: mixin to return information about contributors
          to items* images: mixin to add image information for an item* offset: mixin
          to return programme segment offsets, works in conjunction with programme
          filter* play_event: mixin to return programme segment events, works in conjunction
          with programme or segment_event filters'
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_id
        description: filter for items by partner ID
      - in: query
        name: partner_pid
        description: filter for items by partner PID
      - in: query
        name: people
        description: filter for subset of items that have specified person involved
      - in: query
        name: pid
        description: filter for subset of items matching one of the given PIDs
      - in: query
        name: programme
        description: filter for subset of items that are part of the given programme
      - in: query
        name: q
        description: filter for subset of items matching supplied keyword/phrase (boolean
          operators permitted)
      - in: query
        name: segment_event
        description: filter for item with the given segment_event
      - in: query
        name: sort
        description: 'Sorts:* pid: sort by pid, descending'
      - in: query
        name: sort_direction
        description: Sort direction
      responses:
        200:
          description: OK
      tags:
      - Items
  /master_brands:
    get:
      summary: List all Master Brands
      description: List all Master Brands
      operationId: listMasterbrands
      x-api-path-slug: master-brands-get
      parameters:
      - in: query
        name: mid
        description: filter for subset of masterbrands that have given identifier
      - in: query
        name: mixin
        description: 'Mixins:* images: mixin to add image information for a masterbrand'
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_id
        description: filter for masterbrands by partner ID
      - in: query
        name: partner_pid
        description: filter for masterbrands by partner PID
      - in: query
        name: q
        description: filter for subset of masterbrands matching supplied keyword/phrase
          (boolean operators permitted)
      - in: query
        name: sort
        description: 'Sorts:* mid: sort by mid, ascending'
      - in: query
        name: sort_direction
        description: Sort direction
      responses:
        200:
          description: OK
      tags:
      - Master
      - Brands
  /people:
    get:
      summary: 'Find the people behind and in programmes: cast, crew, guests and more'
      description: The People feed allows you to search for the people and groups
        that contribute to programmes. This is the starting point for cast and crew
        credits, as well as finding contributors using external IDs (such as Wikipedia
        URLs)
      operationId: listPeople
      x-api-path-slug: people-get
      parameters:
      - in: query
        name: authority
        description: filter for subset of people that have an ID issued by the given
          authority
      - in: query
        name: has_external_id
        description: filter for people who have an external identifier
      - in: query
        name: id
        description: filter for subset of people having given ID
      - in: query
        name: id_type
        description: filter for subset of people that have given an ID of the given
          type
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_id
        description: filter for people by partner ID
      - in: query
        name: partner_pid
        description: filter for people by partner PID
      - in: query
        name: pid
        description: filter for subset of people having given PID
      - in: query
        name: programme
        description: filter for subset of people that have contributed to the given
          programme pid
      - in: query
        name: q
        description: filter for subset of people matching supplied keyword/phrase
          (boolean operators permitted)
      responses:
        200:
          description: OK
      tags:
      - People
  /pips:
    get:
      summary: Look inside pips entities
      description: Look inside pips entities
      operationId: listPips
      x-api-path-slug: pips-get
      parameters:
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: q
        description: filter for subset of programmes matching supplied keyword/phrase
          (boolean operators permitted)
      responses:
        200:
          description: OK
      tags:
      - Pips
  /programme_details:
    get:
      summary: Exposes programme information for a single pid
      description: Exposes programme information for a single pid
      operationId: listProgrammeDetails
      x-api-path-slug: programme-details-get
      parameters:
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_pid
        description: Filter for programme information by partner PID
      - in: query
        name: pid
        description: Filter for programme information for the provided PID
      responses:
        200:
          description: OK
      tags:
      - Programme
      - Details
  /programmes:
    get:
      summary: 'Start here for programmes metadata: Brands, Series, Episodes and Clips'
      description: Fetch metadata about Programmes (brands, series, episodes, clips).
        By applying different filter restrictions this feed can be used in many ways,
        for example to retrieve all series belonging to a brand, all the episodes
        and/or clips for a specific series, or any TLEO objects for a masterbrand.
        Other filters permit restricting to specific formats and/or genres, and you
        can request specific versions (for example Signed or Audio-Described). Parameters
        may be combined in any way suitable for your application.
      operationId: listProgrammes
      x-api-path-slug: programmes-get
      parameters:
      - in: query
        name: audio_described
        description: filter for subset of programmes that are audio-described
      - in: query
        name: availability
        description: filter for subset of programmes that have availability
      - in: query
        name: availability_entity_type
        description: additional filter when availability=available
      - in: query
        name: availability_from
        description: filter for subset of programmes that are available after or at
          the specified datetime
      - in: query
        name: availability_type
        description: filter for a subset of programmes that are available for a given
          type
      - in: query
        name: children_of
        description: filter for subset of programmes that have PID as immediate parent
      - in: query
        name: descendants_of
        description: filter for subset of programmes that have PID as ancestor
      - in: query
        name: duration
        description: filter for subset of programmes that have given duration
      - in: query
        name: embargoed
        description: Control return of embargoed items (undocumented)
      - in: query
        name: entity_type
        description: filter for subset of programmes that have given entity type
      - in: query
        name: format
        description: filter for subset of programmes with format
      - in: query
        name: genre
        description: filter for subset of programmes with genre
      - in: query
        name: group
        description: filter for subset of programmes which belong to the given group
          pid
      - in: query
        name: initial_letter
        description: filter for subset of programmes with title beginning with initial
          letter librarian style (ignoring leading The, An (Welsh), etc) 0-9 a-z
      - in: query
        name: initial_letter_end
        description: Programmes with (librarian) titles whose initial letter is equal/before
          given letter
      - in: query
        name: initial_letter_start
        description: Programmes with (librarian) titles whose initial letter is equal/after
          given letter
      - in: query
        name: initial_letter_strict
        description: filter for subset of programmes with title beginning with initial
          letter
      - in: query
        name: item
        description: filter for subset of programmes with linked to versions which
          have the given item pids
      - in: query
        name: master_brand
        description: filter for subset of programmes with master_brand
      - in: query
        name: media_set
        description: filter for subset of programmes with media set
      - in: query
        name: media_type
        description: filter for subset of programmes with media type
      - in: query
        name: mixin
        description: 'Mixins:* alternate_images: mixin to return the alternate images
          for a programme* ancestor_titles: mixin to return ancestor programme titles*
          availability: mixin to return programme availability information* available_simulcasts:
          mixin to return information about programmes that are currently available
          as simulcasts* available_versions: mixin to return information about programmes
          that are currently available on demand* available_webcasts: mixin to return
          information about programmes that are currently available as webcasts* contributions:
          mixin to return information about contributors to a programme* duration:
          mixin to return original version duration in programme concept entities*
          genre_groupings: mixin to return list of genre groupings* genre_groups:
          mixin to return list of genre groups* images: mixin to add image information
          for a programme* is_embeddable: mixin to add embeddable information for
          a programme* previous_next: mixin to return the programmes which appear
          before and after a programme (as determined by the sort applied in the request)*
          related_links: mixin to return information about related links to a programme*
          titles: mixin to return ancestor programme titles* versions_availability:
          mixin to return information about programmes that are currently available'
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_id
        description: filter for programmes by partner ID
      - in: query
        name: partner_pid
        description: filter for programmes by partner PID
      - in: query
        name: payment_type
        description: filter for a subset of programmes that are of the given payment_type
      - in: query
        name: people
        description: filter for subset of programmes with contributions by given people
          PID
      - in: query
        name: pid
        description: filter for subset of programmes having given PID
      - in: query
        name: promoted_for
        description: filter for subset of programmes which are promoted for given
          service
      - in: query
        name: q
        description: filter for subset of programmes matching supplied keyword/phrase
          (boolean operators permitted)
      - in: query
        name: signed
        description: filter for subset of programmes that are signed
      - in: query
        name: sort
        description: 'Sorts:* group_position: sort numerically by position in group,
          ascending* pid: sort alphabetically by PID, descending* position: sort numerically
          by position, ascending* promotion: sort by promotion rank, ascending* release_date:
          sort chronologically by release date, descending* relevance: sort by weighting
          of search term (use with q parameter)* scheduled_start: sort chronologically
          by scheduled start time/date, ascending* strict_title: sort alphabetically
          by title, ascending* title: sort by title librarian style (ignoring leading
          The, A, etc), ascending* tree: sort by root pid and then preorder tree sort'
      - in: query
        name: sort_direction
        description: Sort direction
      - in: query
        name: tag_name
        description: filter for subset of programmes with tag
      - in: query
        name: tag_scheme
        description: filter for subset of programmes with a tag
      - in: query
        name: tleo
        description: filter for subset of programmes that are TLEOs
      - in: query
        name: version
        description: filter for subset of programmes with given PID as one of their
          versions
      responses:
        200:
          description: OK
      tags:
      - Programmes
  /promotions:
    get:
      summary: Discover metadata for content promotions
      description: Details of short-term editorially curated "promotions", for instance
        those programmes featured on iPlayer today
      operationId: listPromotions
      x-api-path-slug: promotions-get
      parameters:
      - in: query
        name: context
        description: filter for subset of promotions belonging to a given context
      - in: query
        name: mixin
        description: 'Mixins:* related_links: mixin to return information about related
          links to a promotion'
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_id
        description: filter for promotions by partner ID
      - in: query
        name: partner_pid
        description: filter for promotions by partner PID
      - in: query
        name: pid
        description: filter for subset of promotions having given PID
      - in: query
        name: promoted_by
        description: filter for subset of promotions having given promoted by
      - in: query
        name: promoted_for
        description: filter for subset of promotions having given promoted for
      - in: query
        name: q
        description: filter for subset of promotions matching supplied keyword/phrase
          (boolean operators permitted)
      - in: query
        name: status
        description: filter for subset of promotions with status
      responses:
        200:
          description: OK
      tags:
      - Promotions
  /schedules:
    get:
      summary: Build schedules and find metadata for TV and radio broadcasts and webcasts
      description: 'Dates, Times, Schedules: when and where are programmes being shown?'
      operationId: listSchedules
      x-api-path-slug: schedules-get
      parameters:
      - in: query
        name: authority
        description: filter for subset of broadcasts and webcasts that have given
          authority
      - in: query
        name: descendants_of
        description: filter for subset of broadcasts and webcasts that are descendants
          of the given programme PID
      - in: query
        name: end_from
        description: filter for subset of broadcasts and webcasts that end on or later
          than the specified datetime
      - in: query
        name: end_to
        description: filter for subset of broadcasts and webcasts that end on or earlier
          than the specified datetime
      - in: query
        name: format
        description: filter for subset of broadcasts and webcasts that are classified
          in the given format ID
      - in: query
        name: genre
        description: filter for subset of broadcasts and webcasts that are classified
          in the given genre ID
      - in: query
        name: group
        description: filter for subset of broadcasts and webcasts that have programmes
          in the given group
      - in: query
        name: id
        description: filter for subset of broadcasts and webcasts that have given
          identifier
      - in: query
        name: id_type
        description: filter for subset of broadcasts and webcasts that have given
          id type
      - in: query
        name: item
        description: filter for subset of broadcasts and webcasts with the given item
          performed on it
      - in: query
        name: mixin
        description: 'Mixins:* ancestor_titles: return ancestor programme titles*
          images: mixin to add image information for broadcasts and webcasts* titles:
          return ancestor programme titles'
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_id
        description: filter for broadcasts and webcasts by partner ID
      - in: query
        name: partner_pid
        description: filter for broadcasts and webcasts by partner PID
      - in: query
        name: people
        description: filter for subset of broadcasts and webcasts that have given
          contributor
      - in: query
        name: pid
        description: filter for subset of broadcasts and webcasts having given PID
      - in: query
        name: q
        description: filter for subset of broadcasts and webcasts matching supplied
          keyword/phrase (boolean operators permitted)
      - in: query
        name: repeat
        description: filter to show either only repeats or non-repeats
      - in: query
        name: schedule_day
        description: filter for subset of broadcasts and webcasts that start on the
          specified day (BBC time)
      - in: query
        name: schedule_day_from
        description: filter for subset of broadcasts and webcasts that start on or
          after the specified day (BBC time)
      - in: query
        name: schedule_day_to
        description: filter for subset of broadcasts and webcasts that start on or
          before the specified day (BBC time)
      - in: query
        name: service_master_brand
        description: filter for subset of broadcasts and webcasts with given service
          master brand
      - in: query
        name: sid
        description: filter for subset of broadcasts and webcasts that are on the
          specified linear service
      - in: query
        name: sort
        description: 'Sorts:* start_date: sort chronologically by scheduled start
          time/date, ascending'
      - in: query
        name: sort_direction
        description: Sort direction
      - in: query
        name: start_from
        description: filter for subset of broadcasts and webcasts that start on or
          later than the specified datetime
      - in: query
        name: start_to
        description: filter for subset of broadcasts and webcasts that start on or
          earlier than the specified datetime
      - in: query
        name: version
        description: filter for subset of broadcasts and webcasts with given PID as
          their parent version
      responses:
        200:
          description: OK
      tags:
      - Schedules
  /schema:
    get:
      summary: Get Schema definition
      description: Get Schema definition
      operationId: getXSD
      x-api-path-slug: schema-get
      responses:
        200:
          description: OK
      tags:
      - Schema
  /services:
    get:
      summary: Information about the linear services used for broadcast transmissions
      description: The services feed exposes the linear broadcast "services" from
        PIPs. These are the actual services which broadcast programmes (eg bbc_one_oxford
        is the service for BBC One in Oxford).
      operationId: listServices
      x-api-path-slug: services-get
      parameters:
      - in: query
        name: end_from
        description: Return services that end on or later than the specified datetime
      - in: query
        name: end_to
        description: filter for subset of broadcasts that end on or earlier than the
          specified datetime
      - in: query
        name: mid
        description: filter for services by masterbrand MID
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_id
        description: filter for services by partner ID
      - in: query
        name: partner_pid
        description: filter for services by partner PID
      - in: query
        name: q
        description: filter for subset of services matching supplied keyword/phrase
          (boolean operators permitted)
      - in: query
        name: service_type
        description: filter for specified type of linear services
      - in: query
        name: sid
        description: filter for specified linear service
      - in: query
        name: start_from
        description: Return services that start on or later than the specified datetime
      - in: query
        name: start_to
        description: Return services that start earlier than the specified datetime
      responses:
        200:
          description: OK
      tags:
      - Services
  /v1/brands/{pid}:
    get:
      summary: Get raw brand
      description: Get raw brand
      operationId: Get_Raw_brand
      x-api-path-slug: v1brandspid-get
      parameters:
      - in: path
        name: pid
      responses:
        200:
          description: OK
      tags:
      - V1
      - Brands
      - Pid
  /v1/brands/{pid}/franchises/:
    get:
      summary: Get raw brand franchise
      description: Get raw brand franchises
      operationId: Get_Raw_brand franchises
      x-api-path-slug: v1brandspidfranchises-get
      parameters:
      - in: path
        name: pid
      responses:
        200:
          description: OK
      tags:
      - V1
      - Brands
      - Pid
      - Franchises
  /v1/episodes/{pid}:
    get:
      summary: Get raw episode
      description: Get raw episode
      operationId: Get_Raw_episode
      x-api-path-slug: v1episodespid-get
      parameters:
      - in: path
        name: pid
      responses:
        200:
          description: OK
      tags:
      - V1
      - Episodes
      - Pid
  /v1/episodes/{pid}/ancestors/:
    get:
      summary: Get raw ancestors
      description: Get raw ancestors
      operationId: Get_Raw_ancestors
      x-api-path-slug: v1episodespidancestors-get
      parameters:
      - in: path
        name: pid
      responses:
        200:
          description: OK
      tags:
      - V1
      - Episodes
      - Pid
      - Ancestors
  /v1/episodes/{pid}/formats/:
    get:
      summary: Get raw formats
      description: Get raw formats
      operationId: Get_Raw_formats
      x-api-path-slug: v1episodespidformats-get
      parameters:
      - in: path
        name: pid
      responses:
        200:
          description: OK
      tags:
      - V1
      - Episodes
      - Pid
      - Formats
  /v1/episodes/{pid}/genre_groups/:
    get:
      summary: Get raw genre groups
      description: Get raw genre groups
      operationId: Get_Raw_genre_groups
      x-api-path-slug: v1episodespidgenre-groups-get
      parameters:
      - in: path
        name: pid
      responses:
        200:
          description: OK
      tags:
      - V1
      - Episodes
      - Pid
      - Genre
      - Groups
  /v1/images/{pid}:
    get:
      summary: Get raw image
      description: Get raw image
      operationId: Get_Raw_image
      x-api-path-slug: v1imagespid-get
      parameters:
      - in: path
        name: pid
      responses:
        200:
          description: OK
      tags:
      - V1
      - Images
      - Pid
  /v1/master_brands/{mbid}:
    get:
      summary: Get raw masterbrand
      description: Get raw masterbrand
      operationId: Get_Raw_masterbrand
      x-api-path-slug: v1master-brandsmbid-get
      parameters:
      - in: path
        name: mbid
      responses:
        200:
          description: OK
      tags:
      - V1
      - Master
      - Brands
      - Mbid
  /v1/promotions/{pid}:
    get:
      summary: Get raw promotion
      description: Get raw promotion
      operationId: Get_Raw_promotion
      x-api-path-slug: v1promotionspid-get
      parameters:
      - in: path
        name: pid
      responses:
        200:
          description: OK
      tags:
      - V1
      - Promotions
      - Pid
  /versions:
    get:
      summary: 'Metadata on editorial programme versions: original, signed, audio-described,
        etc'
      description: 'The versions feed exposes editorial "Versions" of programmes.
        These are concepts used to capture different presentations of an overall programme:
        for example, versions of a programme may include one with sign language, one
        with audio description, one edited for content and more. Versions are also
        important to understand for broadcasts: a linear broadcast or an ondemand
        is always of a specific version, not merely of a programme.'
      operationId: listVersions
      x-api-path-slug: versions-get
      parameters:
      - in: query
        name: availability
        description: filter for subset of versions that have availability
      - in: query
        name: descendants_of
        description: filter for subset of versions having given programme PID
      - in: query
        name: embargoed
        description: Control return of embargoed items (undocumented)
      - in: query
        name: media_set
        description: filter for subset of versions with availability in the given
          media set
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_id
        description: filter for versions by partner ID
      - in: query
        name: partner_pid
        description: filter for versions by partner PID
      - in: query
        name: payment_type
        description: filter for a subset of versions that are of the given payment_type
      - in: query
        name: pid
        description: filter for subset of versions having given PID
      responses:
        200:
          description: OK
      tags:
      - Versions