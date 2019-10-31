swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 1
info:
  title: Eventbrite API
  description: create-manage-promote-events--add-eventmanagement-features-to-your-site--show-the-world-what-exciting-things-are-happening-around-them-
  version: 1.0.0
host: www.eventbriteapi.com
basePath: /v3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events/:
    post:
      summary: Post Events
      description: Makes a new event, and returns an event for the specified event.
      operationId: postEvents
      x-api-path-slug: events-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: event.capacity
        description: Set specific capacity (if omitted, sums ticket capacities)
        type: query
      - in: query
        name: event.category_id
        description: The category (vertical) of the event
        type: query
      - in: query
        name: event.currency
        description: Event currency (3 letter code)
        type: query
      - in: query
        name: event.description.html
        description: The description on the event page
        type: query
      - in: query
        name: event.end.timezone
        description: End time timezone (Olson format)
        type: query
      - in: query
        name: event.end.utc
        description: The end time of the event
        type: query
      - in: query
        name: event.format_id
        description: The format (general type) of the event
        type: query
      - in: query
        name: event.hide_end_date
        description: Whether the end date should be hidden
        type: query
      - in: query
        name: event.hide_start_date
        description: Whether the start date should be hidden
        type: query
      - in: query
        name: event.invite_only
        description: Only invited users can see the event page
        type: query
      - in: query
        name: event.is_reserved_seating
        description: If the event is reserved seating
        type: query
      - in: query
        name: event.listed
        description: If the event is publicly listed and searchable
        type: query
      - in: query
        name: event.logo.id
        description: (Deprecated) The logo for the event
        type: query
      - in: query
        name: event.logo_id
        description: The logo for the event
        type: query
      - in: query
        name: event.name.html
        description: The name of the event
        type: query
      - in: query
        name: event.online_event
        description: Is the event online-only (no venue)?
        type: query
      - in: query
        name: event.organizer_id
        description: The ID of the organizer of this event
        type: query
      - in: query
        name: event.password
        description: Password needed to see the event in unlisted mode
        type: query
      - in: query
        name: event.shareable
        description: If users can share the event on social media
        type: query
      - in: query
        name: event.show_pick_a_seat
        description: For reserved seating event, if attendees can pick their seats
        type: query
      - in: query
        name: event.show_remaining
        description: If the remaining number of tickets is publicly visible on the
          event page
        type: query
      - in: query
        name: event.show_seatmap_thumbnail
        description: For reserved seating event, if venue map thumbnail visible on
          the event page
        type: query
      - in: query
        name: event.source
        description: Source of the event (defaults to API)
        type: query
      - in: query
        name: event.start.timezone
        description: Start time timezone (Olson format)
        type: query
      - in: query
        name: event.start.utc
        description: The start time of the event
        type: query
      - in: query
        name: event.subcategory_id
        description: The subcategory of the event (US only)
        type: query
      - in: query
        name: event.venue_id
        description: The ID of a previously-created venue to associate with this event
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
  /events/{id}:
    get:
      summary: Get Events
      description: Returns an event for the specified event. Many of Eventbrite?s
        API use cases resolve around pulling details of a specific event within an
        Eventbrite account.
      operationId: getEvents
      x-api-path-slug: eventsid-get
      parameters:
      - in: path
        name: id
        description: Event Id
      responses:
        200:
          description: OK
      tags:
      - Events
    post:
      summary: Post Events
      description: Updates an event. Returns an event for the specified event.
      operationId: postEvents
      x-api-path-slug: eventsid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Event Id
      responses:
        200:
          description: OK
      tags:
      - Events
  /categories/{id}/:
    get:
      summary: Get Categories
      description: Gets a category by ID as category.
      operationId: getCategories
      x-api-path-slug: categoriesid-get
      responses:
        200:
          description: OK
      tags:
      - Categories
  /subcategories/:
    get:
      summary: Get Subcategories
      description: Returns a list of subcategory as subcategories.
      operationId: getSubcategories
      x-api-path-slug: subcategories-get
      responses:
        200:
          description: OK
      tags:
      - Subcategories
  /subcategories/{id}/:
    get:
      summary: Get Subcategories
      description: Gets a subcategory by ID as subcategory.
      operationId: getSubcategories
      x-api-path-slug: subcategoriesid-get
      responses:
        200:
          description: OK
      tags:
      - Subcategories
  /checkout_settings/countries_currencies/:
    get:
      summary: Get Checkout Settings Countries Currencies
      description: Get the countries and currencies which are supported by Eventbrite
        for ticket payment
      operationId: getCheckoutSettingsCountriesCurrencies
      x-api-path-slug: checkout-settingscountries-currencies-get
      responses:
        200:
          description: OK
      tags:
      - Checkout
      - Settings
      - Countries
      - Currencies
  /checkout_settings/methods/:
    get:
      summary: Get Checkout Settings Methods
      description: Get the available checkout methods to do payments given a country
        and a currency.
      operationId: getCheckoutSettingsMethods
      x-api-path-slug: checkout-settingsmethods-get
      parameters:
      - in: query
        name: country
        description: Expected methods for Country
        type: query
      - in: query
        name: currency
        description: Expected methods for Currency
        type: query
      responses:
        200:
          description: OK
      tags:
      - Checkout
      - Settings
      - Methods
  /checkout_settings/:
    get:
      summary: Get Checkout Settings
      description: Searches and returns a list of checkout_settings for the current
        user as the key checkout_settings.
      operationId: getCheckoutSettings
      x-api-path-slug: checkout-settings-get
      parameters:
      - in: query
        name: checkout_methods
        description: One or more optional (comma-separated) checkout methods by which
          to filter checkout settings
        type: query
      - in: query
        name: country
        description: An optional country code by which to filter checkout settings
        type: query
      - in: query
        name: currency
        description: An optional currency code by which to filter checkout settings
        type: query
      - in: query
        name: search_most_recent_event
        description: '&#160;'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Checkout
      - Settings
    post:
      summary: Post Checkout Settings
      description: Creates a new checkout_settings object belonging to the current
        user. Two common settings are Eventbrite Payment Processing ( checkout_method
        = &#8220;eventbrite&#8221; ) and PayPal ( checkout_method = &#8220;paypal&#8221;
        ). In addition to the checkout_method you must provide the country and currency
        proceeds from the event should be paid to.
      operationId: postCheckoutSettings
      x-api-path-slug: checkout-settings-post
      responses:
        200:
          description: OK
      tags:
      - Checkout
      - Settings
  /checkout_settings/:checkout_settings_id/:
    get:
      summary: Get Checkout Settings Checkout Settings
      description: Get a specific checkout_settings object by ID
      operationId: getCheckoutSettingsCheckoutSettings
      x-api-path-slug: checkout-settingscheckout-settings-id-get
      responses:
        200:
          description: OK
      tags:
      - Checkout
      - Settings
      - :checkout
      - Settings
  /events/:event_id/checkout_settings/:
    get:
      summary: Get Events Event Checkout Settings
      description: Gets and returns a list of checkout_settings associated with a
        given event by its event_id.
      operationId: getEventsEventCheckoutSettings
      x-api-path-slug: eventsevent-idcheckout-settings-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Checkout
      - Settings
    post:
      summary: Post Events Event Checkout Settings
      description: Associate a single or set of checkout_settings with a given event
        by its event_id. This does not add more checkout settings to the event, but
        instead replaces all checkout settings for the event with the one(s) submitted.
        The JSON post body is a string list of the checkout_settings IDs you want
        to associate.
      operationId: postEventsEventCheckoutSettings
      x-api-path-slug: eventsevent-idcheckout-settings-post
      parameters:
      - in: query
        name: checkout_settings_ids
        description: A list of IDs for checkout settings that should be linked to
          the event
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Checkout
      - Settings
  /events/:event_id/payout_settings/:
    get:
      summary: Get Events Event Payout Settings
      description: Gets and returns the payout_settings (user instrument ID) associated
        with a given event by its event_id.
      operationId: getEventsEventPayoutSettings
      x-api-path-slug: eventsevent-idpayout-settings-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Payout
      - Settings
    post:
      summary: Post Events Event Payout Settings
      description: Associate a payout user instrument ID with a given event, or clear
        the association by passing a null value for the user instrument ID.
      operationId: postEventsEventPayoutSettings
      x-api-path-slug: eventsevent-idpayout-settings-post
      parameters:
      - in: query
        name: payout_settings.user_instrument_vault_id
        description: The vault ID for the user instrument to which payouts are sent
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Payout
      - Settings
  /discounts/:discount_id/:
    get:
      summary: Get Discounts Discount
      description: Returns the cross_event_discount with the specified :discount_id.
      operationId: getDiscountsDiscount
      x-api-path-slug: discountsdiscount-id-get
      responses:
        200:
          description: OK
      tags:
      - Discounts
      - :discount
    post:
      summary: Post Discounts Discount
      description: Updates the discount with the specified :discount_id. Returns the
        updated cross_event_discount. The fields sent are the ones that are going
        to be updated, the fields that are not sent will be unchanged. The same conditions
        and notes for the discount creation apply.
      operationId: postDiscountsDiscount
      x-api-path-slug: discountsdiscount-id-post
      parameters:
      - in: query
        name: discount.amount_off
        description: Fixed reduction amount
        type: query
      - in: query
        name: discount.code
        description: Code used to activate discount
        type: query
      - in: query
        name: discount.end_date
        description: Allow use until this date
        type: query
      - in: query
        name: discount.end_date_relative
        description: Allow use until this number of seconds before the event starts
        type: query
      - in: query
        name: discount.hold_ids
        description: IDs of holds this discount can unlock
        type: query
      - in: query
        name: discount.percent_off
        description: Percentage reduction
        type: query
      - in: query
        name: discount.quantity_available
        description: Number of discount uses
        type: query
      - in: query
        name: discount.start_date
        description: Allow use from this date
        type: query
      - in: query
        name: discount.start_date_relative
        description: Allow use from this number of seconds before the event starts
        type: query
      - in: query
        name: discount.ticket_class_ids
        description: IDs of tickets to limit discount to
        type: query
      responses:
        200:
          description: OK
      tags:
      - Discounts
      - :discount
    delete:
      summary: Delete Discounts Discount
      description: |-
        Deletes the cross_event_discount with the specified :discount_id.
        Only unused discounts can be deleted.
      operationId: deleteDiscountsDiscount
      x-api-path-slug: discountsdiscount-id-delete
      responses:
        200:
          description: OK
      tags:
      - Discounts
      - :discount
  /discounts/:
    post:
      summary: Post Discounts
      description: Creates a discount. Returns the created cross_event_discount.
      operationId: postDiscounts
      x-api-path-slug: discounts-post
      parameters:
      - in: query
        name: discount.amount_off
        description: Fixed reduction amount
        type: query
      - in: query
        name: discount.code
        description: Code used to activate discount
        type: query
      - in: query
        name: discount.end_date
        description: Allow use until this date
        type: query
      - in: query
        name: discount.end_date_relative
        description: Allow use until this number of seconds before the event starts
        type: query
      - in: query
        name: discount.event_id
        description: ID of the event
        type: query
      - in: query
        name: discount.hold_ids
        description: IDs of holds this discount can unlock
        type: query
      - in: query
        name: discount.percent_off
        description: Percentage reduction
        type: query
      - in: query
        name: discount.quantity_available
        description: Number of discount uses
        type: query
      - in: query
        name: discount.start_date
        description: Allow use from this date
        type: query
      - in: query
        name: discount.start_date_relative
        description: Allow use from this number of seconds before the event starts
        type: query
      - in: query
        name: discount.ticket_class_ids
        description: IDs of tickets to limit discount to
        type: query
      - in: query
        name: discount.ticket_group_id
        description: ID of the ticket group
        type: query
      - in: query
        name: discount.type
        description: The type of discount
        type: query
      responses:
        200:
          description: OK
      tags:
      - Discounts
  /events/{id}/:
    get:
      summary: Get Events
      description: |-
        Returns an event for the specified event. Many of Eventbrite???s API use cases revolve around pulling details
        of a specific event within an Eventbrite account. Does not support fetching a repeating event series parent
        (see GET /series/:id/).
      operationId: getEvents
      x-api-path-slug: eventsid-get
      responses:
        200:
          description: OK
      tags:
      - Events
    post:
      summary: Post Events
      description: |-
        Updates an event. Returns an event for the specified event. Does not support updating a repeating event
        series parent (see POST /series/:id/).
      operationId: postEvents
      x-api-path-slug: eventsid-post
      parameters:
      - in: query
        name: event.capacity
        description: Set specific capacity (if omitted, sums ticket capacities)
        type: query
      - in: query
        name: event.category_id
        description: The category (vertical) of the event
        type: query
      - in: query
        name: event.currency
        description: Event currency (3 letter code)
        type: query
      - in: query
        name: event.description.html
        description: The description on the event page
        type: query
      - in: query
        name: event.end.timezone
        description: End time timezone (Olson format)
        type: query
      - in: query
        name: event.end.utc
        description: The end time of the event
        type: query
      - in: query
        name: event.format_id
        description: The format (general type) of the event
        type: query
      - in: query
        name: event.hide_end_date
        description: Whether the end date should be hidden
        type: query
      - in: query
        name: event.hide_start_date
        description: Whether the start date should be hidden
        type: query
      - in: query
        name: event.invite_only
        description: Only invited users can see the event page
        type: query
      - in: query
        name: event.is_reserved_seating
        description: If the event is reserved seating
        type: query
      - in: query
        name: event.listed
        description: If the event is publicly listed and searchable
        type: query
      - in: query
        name: event.logo.id
        description: (Deprecated) The logo for the event
        type: query
      - in: query
        name: event.logo_id
        description: The logo for the event
        type: query
      - in: query
        name: event.name.html
        description: The name of the event
        type: query
      - in: query
        name: event.online_event
        description: Is the event online-only (no venue)?
        type: query
      - in: query
        name: event.organizer_id
        description: The ID of the organizer of this event
        type: query
      - in: query
        name: event.password
        description: Password needed to see the event in unlisted mode
        type: query
      - in: query
        name: event.shareable
        description: If users can share the event on social media
        type: query
      - in: query
        name: event.show_pick_a_seat
        description: For reserved seating event, if attendees can pick their seats
        type: query
      - in: query
        name: event.show_remaining
        description: If the remaining number of tickets is publicly visible on the
          event page
        type: query
      - in: query
        name: event.show_seatmap_thumbnail
        description: For reserved seating event, if venue map thumbnail visible on
          the event page
        type: query
      - in: query
        name: event.source
        description: Source of the event (defaults to API)
        type: query
      - in: query
        name: event.start.timezone
        description: Start time timezone (Olson format)
        type: query
      - in: query
        name: event.start.utc
        description: The start time of the event
        type: query
      - in: query
        name: event.subcategory_id
        description: The subcategory of the event (US only)
        type: query
      - in: query
        name: event.venue_id
        description: ID of the venue
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
    delete:
      summary: Delete Events
      description: |-
        Deletes an event if the delete is permitted. In order for a delete to be permitted, there must be no pending or
        completed orders. Returns a boolean indicating success or failure of the delete.
      operationId: deleteEvents
      x-api-path-slug: eventsid-delete
      responses:
        200:
          description: OK
      tags:
      - Events
  /events/{id}/publish/:
    post:
      summary: Post Events Publish
      description: |-
        Publishes an event if it has not already been deleted. In order for publish to be permitted, the event must have all
        necessary information, including a name and description, an organizer, at least one ticket, and valid payment options.
        This API endpoint will return argument errors for event fields that fail to validate the publish requirements. Returns
        a boolean indicating success or failure of the publish.
      operationId: postEventsPublish
      x-api-path-slug: eventsidpublish-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Publish
  /events/{id}/unpublish/:
    post:
      summary: Post Events Unpublish
      description: |-
        Unpublishes an event. In order for a free event to be unpublished, it must not have any pending or completed orders,
        even if the event is in the past. In order for a paid event to be unpublished, it must not have any pending or completed
        orders, unless the event has been completed and paid out. Returns a boolean indicating success or failure of the
        unpublish.
      operationId: postEventsUnpublish
      x-api-path-slug: eventsidunpublish-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Unpublish
  /events/{id}/cancel/:
    post:
      summary: Post Events Cancel
      description: |-
        Cancels an event if it has not already been deleted. In order for cancel to be permitted, there must be no pending or
        completed orders. Returns a boolean indicating success or failure of the cancel.
      operationId: postEventsCancel
      x-api-path-slug: eventsidcancel-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Cancel
  /events/{id}/copy/:
    post:
      summary: Post Events Copy
      description: Creates a duplicate version of the event being copied. Returns
        the event object for the newly created event.
      operationId: postEventsCopy
      x-api-path-slug: eventsidcopy-post
      parameters:
      - in: query
        name: end_date
        description: The end time of the new event
        type: query
      - in: query
        name: name
        description: The name of the new event
        type: query
      - in: query
        name: start_date
        description: The start time of the new event
        type: query
      - in: query
        name: timezone
        description: timezone for the new event (Olson format)
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Copy
  /events/{id}/display_settings/:
    get:
      summary: Get Events Display Settings
      description: Retrieves the display settings for an event.
      operationId: getEventsDisplaySettings
      x-api-path-slug: eventsiddisplay-settings-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Display
      - Settings
    post:
      summary: Post Events Display Settings
      description: Updates the display settings for an event.
      operationId: postEventsDisplaySettings
      x-api-path-slug: eventsiddisplay-settings-post
      parameters:
      - in: query
        name: display_settings.show_end_date
        description: Whether to display the end date on the event listing
        type: query
      - in: query
        name: display_settings.show_facebook_friends_going
        description: Whether to display which of the user&#8217;s Facebook friends
          are going
        type: query
      - in: query
        name: display_settings.show_map
        description: Whether to display a map to the venue on the event listing
        type: query
      - in: query
        name: display_settings.show_organizer_facebook
        description: Whether to display a link to the organizer&#8217;s Facebook profile
        type: query
      - in: query
        name: display_settings.show_organizer_twitter
        description: Whether to display a link to the organizer&#8217;s Twitter profile
        type: query
      - in: query
        name: display_settings.show_remaining
        description: Whether to display the number of remaining tickets
        type: query
      - in: query
        name: display_settings.show_start_date
        description: Whether to display the start date on the event listing
        type: query
      - in: query
        name: display_settings.show_start_end_time
        description: Whether to display event start and end time on the event listing
        type: query
      - in: query
        name: display_settings.show_timezone
        description: Whether to display the event timezone on the event listing
        type: query
      - in: query
        name: display_settings.terminology
        description: 'Which terminology should be used to refer to the event (Valid
          choices are: tickets_vertical, or endurance_vertical)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Display
      - Settings
  /events/{id}/ticket_classes/:
    get:
      summary: Get Events Ticket Classes
      description: |-
        Returns a paginated response with a key of
        ticket_classes, containing a list of ticket_class.
      operationId: getEventsTicketClasses
      x-api-path-slug: eventsidticket-classes-get
      parameters:
      - in: query
        name: pos
        description: 'Only return ticket classes valid for the given point of sale
          (Valid choices are: online, or at_the_door)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Ticket
      - Classes
    post:
      summary: Post Events Ticket Classes
      description: |-
        Creates a new ticket class, returning the result as a ticket_class
        under the key ticket_class.
      operationId: postEventsTicketClasses
      x-api-path-slug: eventsidticket-classes-post
      parameters:
      - in: query
        name: ticket_class.auto_hide
        description: Hide this ticket when it is not on sale
        type: query
      - in: query
        name: ticket_class.auto_hide_after
        description: Override re-hide date for auto-hide
        type: query
      - in: query
        name: ticket_class.auto_hide_before
        description: Override reveal date for auto-hide
        type: query
      - in: query
        name: ticket_class.cost
        description: Cost of the ticket (currently currency must match event currency)
          e
        type: query
      - in: query
        name: ticket_class.description
        description: Description of the ticket
        type: query
      - in: query
        name: ticket_class.donation
        description: Is this a donation? (user-supplied cost)
        type: query
      - in: query
        name: ticket_class.free
        description: Is this a free ticket?
        type: query
      - in: query
        name: ticket_class.hidden
        description: Hide this ticket
        type: query
      - in: query
        name: ticket_class.hide_description
        description: Hide the ticket description on the event page
        type: query
      - in: query
        name: ticket_class.include_fee
        description: Absorb the fee into the displayed cost
        type: query
      - in: query
        name: ticket_class.maximum_quantity
        description: Maximum number per order (blank for unlimited)
        type: query
      - in: query
        name: ticket_class.minimum_quantity
        description: Minimum number per order
        type: query
      - in: query
        name: ticket_class.name
        description: Name of this ticket type
        type: query
      - in: query
        name: ticket_class.order_confirmation_message
        description: Order message per ticket type
        type: query
      - in: query
        name: ticket_class.quantity_total
        description: Total available number of this ticket, required for non-donation
          tickets
        type: query
      - in: query
        name: ticket_class.sales_channels
        description: A list of all supported sales channels ([&#8220;online&#8221;],
          [&#8220;online&#8221;, &#8220;atd&#8221;], [&#8220;atd&#8221;])
        type: query
      - in: query
        name: ticket_class.sales_end
        description: When the ticket stops being on sale (leave empty for &#8216;one
          hour before event start&#8217;)
        type: query
      - in: query
        name: ticket_class.sales_start
        description: When the ticket is available for sale (leave empty for &#8216;when
          event published&#8217;)
        type: query
      - in: query
        name: ticket_class.sales_start_after
        description: The ID of another ticket class - when it sells out, this class
          will go on sale
        type: query
      - in: query
        name: ticket_class.split_fee
        description: Absorb the payment fee, but show the eventbrite fee
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Ticket
      - Classes
  /events/{id}/ticket_classes/:ticket_class_id/:
    get:
      summary: Get Events Ticket Classes Ticket Class
      description: |-
        Gets and returns a single ticket_class by ID, as the key
        ticket_class.
      operationId: getEventsTicketClassesTicketClass
      x-api-path-slug: eventsidticket-classesticket-class-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Ticket
      - Classes
      - :ticket
      - Class
    post:
      summary: Post Events Ticket Classes Ticket Class
      description: Updates an existing ticket class, returning the updated result
        as a ticket_class under the key ticket_class.
      operationId: postEventsTicketClassesTicketClass
      x-api-path-slug: eventsidticket-classesticket-class-id-post
      parameters:
      - in: query
        name: ticket_class.auto_hide
        description: Hide this ticket when it is not on sale
        type: query
      - in: query
        name: ticket_class.auto_hide_after
        description: Override re-hide date for auto-hide
        type: query
      - in: query
        name: ticket_class.auto_hide_before
        description: Override reveal date for auto-hide
        type: query
      - in: query
        name: ticket_class.cost
        description: Cost of the ticket (currently currency must match event currency)
          e
        type: query
      - in: query
        name: ticket_class.description
        description: Description of the ticket
        type: query
      - in: query
        name: ticket_class.donation
        description: Is this a donation? (user-supplied cost)
        type: query
      - in: query
        name: ticket_class.free
        description: Is this a free ticket?
        type: query
      - in: query
        name: ticket_class.hidden
        description: Hide this ticket
        type: query
      - in: query
        name: ticket_class.hide_description
        description: Hide the ticket description on the event page
        type: query
      - in: query
        name: ticket_class.include_fee
        description: Absorb the fee into the displayed cost
        type: query
      - in: query
        name: ticket_class.maximum_quantity
        description: Maximum number per order (blank for unlimited)
        type: query
      - in: query
        name: ticket_class.minimum_quantity
        description: Minimum number per order
        type: query
      - in: query
        name: ticket_class.name
        description: Name of this ticket type
        type: query
      - in: query
        name: ticket_class.order_confirmation_message
        description: Order message per ticket type
        type: query
      - in: query
        name: ticket_class.quantity_total
        description: Total available number of this ticket, required for non-donation
          tickets
        type: query
      - in: query
        name: ticket_class.sales_channels
        description: A list of all supported sales channels ([&#8220;online&#8221;],
          [&#8220;online&#8221;, &#8220;atd&#8221;], [&#8220;atd&#8221;])
        type: query
      - in: query
        name: ticket_class.sales_end
        description: When the ticket stops being on sale (leave empty for &#8216;one
          hour before event start&#8217;)
        type: query
      - in: query
        name: ticket_class.sales_start
        description: When the ticket is available for sale (leave empty for &#8216;when
          event published&#8217;)
        type: query
      - in: query
        name: ticket_class.sales_start_after
        description: The ID of another ticket class - when it sells out, this class
          will go on sale
        type: query
      - in: query
        name: ticket_class.split_fee
        description: Absorb the payment fee, but show the eventbrite fee
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Ticket
      - Classes
      - :ticket
      - Class
    delete:
      summary: Delete Events Ticket Classes Ticket Class
      description: 'Deletes the ticket class. Returns {&quot;deleted&quot;: true}.'
      operationId: deleteEventsTicketClassesTicketClass
      x-api-path-slug: eventsidticket-classesticket-class-id-delete
      parameters:
      - in: query
        name: break_dependency
        description: Delete even if ticket sales depend on this ticket
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Ticket
      - Classes
      - :ticket
      - Class
  /events/{id}/canned_questions/:
    get:
      summary: Get Events Canned Questions
      description: 'This endpoint returns canned questions of a single event (examples:
        first name, last name, company, prefix, etc.). This endpoint will return question.'
      operationId: getEventsCannedQuestions
      x-api-path-slug: eventsidcanned-questions-get
      parameters:
      - in: query
        name: as_owner
        description: Return private events and more details
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Canned
      - Questions
    post:
      summary: Post Events Canned Questions
      description: Creates a new canned question; returns the result as a question.
      operationId: postEventsCannedQuestions
      x-api-path-slug: eventsidcanned-questions-post
      parameters:
      - in: query
        name: question.canned_type
        description: String value of canned_type
        type: query
      - in: query
        name: question.choices
        description: Choices for multiple choice questions
        type: query
      - in: query
        name: question.display_answer_on_order
        description: Is this question displayed on order confirmation?
        type: query
      - in: query
        name: question.parent_choice_id
        description: ID of Parent Question (for subquestions)
        type: query
      - in: query
        name: question.question.html
        description: Question displayed to the recipient
        type: query
      - in: query
        name: question.required
        description: Is an answer to this question required for registration?
        type: query
      - in: query
        name: question.respondent
        description: 'Ask this question to the ticket buyer or each attendee? (Valid
          choices are: ticket_buyer, or attendee)'
        type: query
      - in: query
        name: question.ticket_classes
        description: Tickets to which to limit this question
        type: query
      - in: query
        name: question.type
        description: 'Type of Question (Valid choices are: checkbox, dropdown, text,
          paragraph, radio, or waiver)'
        type: query
      - in: query
        name: question.waiver
        description: Waiver content for questions of type waiver
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Canned
      - Questions
  /events/{id}/questions/:
    get:
      summary: Get Events Questions
      description: |-
        Eventbrite allows event organizers to add custom questions that attendees fill
        out upon registration. This endpoint can be helpful for determining what
        custom information is collected and available per event.
      operationId: getEventsQuestions
      x-api-path-slug: eventsidquestions-get
      parameters:
      - in: query
        name: as_owner
        description: Return private events and more details
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Questions
    post:
      summary: Post Events Questions
      description: Creates a new question; returns the result as a question as the
        key question.
      operationId: postEventsQuestions
      x-api-path-slug: eventsidquestions-post
      parameters:
      - in: query
        name: question.choices
        description: Choices for multiple choice questions
        type: query
      - in: query
        name: question.display_answer_on_order
        description: Is this question displayed on order confirmation?
        type: query
      - in: query
        name: question.parent_choice_id
        description: ID of Parent Question Choice (for subquestions)
        type: query
      - in: query
        name: question.parent_id
        description: ID of Parent Question (for subquestions)
        type: query
      - in: query
        name: question.question.html
        description: Question displayed to the recipient
        type: query
      - in: query
        name: question.required
        description: Is an answer to this question required for registration?
        type: query
      - in: query
        name: question.respondent
        description: 'Ask this question to the ticket buyer or each attendee? (Valid
          choices are: ticket_buyer, or attendee)'
        type: query
      - in: query
        name: question.ticket_classes
        description: Tickets to which to limit this question
        type: query
      - in: query
        name: question.type
        description: 'Type of Question (Valid choices are: checkbox, dropdown, text,
          paragraph, radio, or waiver)'
        type: query
      - in: query
        name: question.waiver
        description: Waiver content for questions of type waiver
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Questions
  /events/{id}/questions/{id}/:
    get:
      summary: Get Events Questions
      description: This endpoint will return question for a specific question id.
      operationId: getEventsQuestions
      x-api-path-slug: eventsidquestionsid-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Questions
  /events/{id}/attendees/:attendee_id/:
    get:
      summary: Get Events Attendees Attendee
      description: Returns a single attendee by ID, as the key attendee.
      operationId: getEventsAttendeesAttendee
      x-api-path-slug: eventsidattendeesattendee-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Attendees
      - :attendee
  /events/{id}/orders/:
    get:
      summary: Get Events Orders
      description: Returns a paginated response with a key of orders, containing a
        list of order against this event.
      operationId: getEventsOrders
      x-api-path-slug: eventsidorders-get
      parameters:
      - in: query
        name: changed_since
        description: Only return orders changed on or after the time given
        type: query
      - in: query
        name: exclude_emails
        description: Don&#8217;t include orders placed by any of these emails
        type: query
      - in: query
        name: last_item_seen
        description: Only return orders changed on or after the time given and with
          an id bigger than last item seen
        type: query
      - in: query
        name: only_emails
        description: Only include orders placed by one of these emails
        type: query
      - in: query
        name: refund_request_statuses
        description: Return only orders with selected refund requests statuses
        type: query
      - in: query
        name: status
        description: 'Filter to active (attending), inactive (not attending), all
          (both) orders and all_not_deleted (active and inactive but not deleted)
          (Valid choices are: active, inactive, all, or all_not_deleted)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Orders
  /events/{id}/discounts/:
    get:
      summary: Get Events Discounts
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts
      operationId: getEventsDiscounts
      x-api-path-slug: eventsiddiscounts-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Discounts
    post:
      summary: Post Events Discounts
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts
      operationId: postEventsDiscounts
      x-api-path-slug: eventsiddiscounts-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Discounts
  /events/{id}/discounts/:discount_id/:
    get:
      summary: Get Events Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id
      operationId: getEventsDiscountsDiscount
      x-api-path-slug: eventsiddiscountsdiscount-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Discounts
      - :discount
    post:
      summary: Post Events Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id
      operationId: postEventsDiscountsDiscount
      x-api-path-slug: eventsiddiscountsdiscount-id-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Discounts
      - :discount
    delete:
      summary: Delete Events Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id
      operationId: deleteEventsDiscountsDiscount
      x-api-path-slug: eventsiddiscountsdiscount-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - Discounts
      - :discount
  /events/{id}/public_discounts/:
    get:
      summary: Get Events Public Discounts
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts
      operationId: getEventsPublicDiscounts
      x-api-path-slug: eventsidpublic-discounts-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Public
      - Discounts
    post:
      summary: Post Events Public Discounts
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts
      operationId: postEventsPublicDiscounts
      x-api-path-slug: eventsidpublic-discounts-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Public
      - Discounts
  /events/{id}/public_discounts/:discount_id/:
    get:
      summary: Get Events Public Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id
      operationId: getEventsPublicDiscountsDiscount
      x-api-path-slug: eventsidpublic-discountsdiscount-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Public
      - Discounts
      - :discount
    post:
      summary: Post Events Public Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id
      operationId: postEventsPublicDiscountsDiscount
      x-api-path-slug: eventsidpublic-discountsdiscount-id-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Public
      - Discounts
      - :discount
    delete:
      summary: Delete Events Public Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id
      operationId: deleteEventsPublicDiscountsDiscount
      x-api-path-slug: eventsidpublic-discountsdiscount-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - Public
      - Discounts
      - :discount
  /events/{id}/access_codes/:
    get:
      summary: Get Events Access Codes
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts
      operationId: getEventsAccessCodes
      x-api-path-slug: eventsidaccess-codes-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Access
      - Codes
    post:
      summary: Post Events Access Codes
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts
      operationId: postEventsAccessCodes
      x-api-path-slug: eventsidaccess-codes-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Access
      - Codes
    delete:
      summary: Delete Events Access Codes
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id
      operationId: deleteEventsAccessCodes
      x-api-path-slug: eventsidaccess-codes-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - Access
      - Codes
  /events/{id}/access_codes/:access_code_id/:
    get:
      summary: Get Events Access Codes Access Code
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id
      operationId: getEventsAccessCodesAccessCode
      x-api-path-slug: eventsidaccess-codesaccess-code-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Access
      - Codes
      - :access
      - Code
    post:
      summary: Post Events Access Codes Access Code
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id
      operationId: postEventsAccessCodesAccessCode
      x-api-path-slug: eventsidaccess-codesaccess-code-id-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Access
      - Codes
      - :access
      - Code
  /events/{id}/transfers/:
    get:
      summary: Get Events Transfers
      description: Returns a list of transfers for the event.
      operationId: getEventsTransfers
      x-api-path-slug: eventsidtransfers-get
      parameters:
      - in: query
        name: changed_since
        description: Only return transfers changed on or after the time given
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Transfers
  /events/{id}/teams/:
    get:
      summary: Get Events Teams
      description: Returns a list of attendee-team for the event.
      operationId: getEventsTeams
      x-api-path-slug: eventsidteams-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Teams
  /events/{id}/teams/{id}/:
    get:
      summary: Get Events Teams
      description: Returns information for a single attendee-team.
      operationId: getEventsTeams
      x-api-path-slug: eventsidteamsid-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Teams
  /events/{id}/teams/{id}/attendees/:
    get:
      summary: Get Events Teams Attendees
      description: Returns attendee for a single attendee-team.
      operationId: getEventsTeamsAttendees
      x-api-path-slug: eventsidteamsidattendees-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Teams
      - Attendees
  /events/:event_id/ticket_groups/:
    get:
      summary: Get Events Event Ticket Groups
      description: |-
        Get the list of ticket_group for the event with the specified :event_id.
        By default, only the ticket groups that are live are shown.
      operationId: getEventsEventTicketGroups
      x-api-path-slug: eventsevent-idticket-groups-get
      parameters:
      - in: query
        name: status
        description: 'Limits results to groups with the specific status (Valid choices
          are: live, archived, deleted, or all)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Ticket
      - Groups
  /events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/:ticket_group_id/:
    post:
      summary: Post Events Event Ticket Classes Ticket Class Ticket Groups Ticket
        Group
      description: Add the Ticket Class with the specified :ticket_class_id that belongs
        to the event with :event_id to the Ticket Group identified by :ticket_group_id.
      operationId: postEventsEventTicketClassesTicketClassTicketGroupsTicketGroup
      x-api-path-slug: eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Ticket
      - Classes
      - :ticket
      - Class
      - Ticket
      - Groups
      - :ticket
      - Group
    delete:
      summary: Delete Events Event Ticket Classes Ticket Class Ticket Groups Ticket
        Group
      description: Remove the Ticket Class with the specified :ticket_class_id that
        belongs to the event with :event_id from the Ticket Group identified by :ticket_group_id.
      operationId: deleteEventsEventTicketClassesTicketClassTicketGroupsTicketGroup
      x-api-path-slug: eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Ticket
      - Classes
      - :ticket
      - Class
      - Ticket
      - Groups
      - :ticket
      - Group
  /events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/:
    get:
      summary: Get Events Event Ticket Classes Ticket Class Ticket Groups
      description: |-
        Get the Ticket Groups for Ticket Class with the specified :ticket_class_id that belongs to the event with :event_id.
        By default, only the ticket groups that are live are shown.
      operationId: getEventsEventTicketClassesTicketClassTicketGroups
      x-api-path-slug: eventsevent-idticket-classesticket-class-idticket-groups-get
      parameters:
      - in: query
        name: status
        description: 'Limits results to groups with the specific status (Valid choices
          are: live, archived, deleted, or all)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Ticket
      - Classes
      - :ticket
      - Class
      - Ticket
      - Groups
  /events/{id}/ticket_buyer_settings/:
    get:
      summary: Get Events Ticket Buyer Settings
      description: Returns a ticket_buyer_settings for an event.
      operationId: getEventsTicketBuyerSettings
      x-api-path-slug: eventsidticket-buyer-settings-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Ticket
      - Buyer
      - Settings
    post:
      summary: Post Events Ticket Buyer Settings
      description: Updates the ticket buyer settings for an event. Returns a ticket_buyer_settings.
      operationId: postEventsTicketBuyerSettings
      x-api-path-slug: eventsidticket-buyer-settings-post
      parameters:
      - in: query
        name: ticket_buyer_settings.confirmation_message.html
        description: Confirmation message to display on order completion
        type: query
      - in: query
        name: ticket_buyer_settings.instructions.html
        description: Instructions to display on the ticket
        type: query
      - in: query
        name: ticket_buyer_settings.redirect_url
        description: Redirect to this url post-purchase
        type: query
      - in: query
        name: ticket_buyer_settings.refund_request_enabled
        description: Whether refund requests are accepted for the event
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Ticket
      - Buyer
      - Settings
  /formats/:
    get:
      summary: Get Formats
      description: Returns a list of format as formats.
      operationId: getFormats
      x-api-path-slug: formats-get
      responses:
        200:
          description: OK
      tags:
      - Formats
  /formats/{id}/:
    get:
      summary: Get Formats
      description: Gets a format by ID as format.
      operationId: getFormats
      x-api-path-slug: formatsid-get
      responses:
        200:
          description: OK
      tags:
      - Formats
  /media/{id}/:
    get:
      summary: Get Media
      description: Return an image for a given id.
      operationId: getMedia
      x-api-path-slug: mediaid-get
      parameters:
      - in: query
        name: height
        description: Optional thumbnail height (you can specify only this value or
          also width)
        type: query
      - in: query
        name: width
        description: Optional thumbnail width (you can specify only this value or
          also height)
        type: query
      responses:
        200:
          description: OK
      tags:
      - Media
  /media/upload/:
    get:
      summary: Get Media Upload
      description: See Media Uploads.
      operationId: getMediaUpload
      x-api-path-slug: mediaupload-get
      parameters:
      - in: query
        name: type
        description: 'The type of image to upload (Valid choices are: image-event-logo,
          image-event-logo-preserve-quality, image-event-view-from-seat, image-organizer-logo,
          image-user-photo, or image-structured-content)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Media
      - Upload
  /users/me/notifications/:
    get:
      summary: Get Users Me Notifications
      description: Gets a paginated response of notification objects for a determined
        user.
      operationId: getUsersMeNotifications
      x-api-path-slug: usersmenotifications-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Me
      - Notifications
  /orders/{id}/:
    get:
      summary: Get Orders
      description: Gets an order by ID an order object.
      operationId: getOrders
      x-api-path-slug: ordersid-get
      responses:
        200:
          description: OK
      tags:
      - Orders
  /users/:user_id/organizations/:
    get:
      summary: Get Users User Organizations
      description: |-
        Returns a continuated list of organizations
        accessible to the current user.
      operationId: getUsersUserOrganizations
      x-api-path-slug: usersuser-idorganizations-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - :user
      - Organizations
  /organizers/:
    post:
      summary: Post Organizers
      description: Makes a new organizer. Returns an organizer as organizer.
      operationId: postOrganizers
      x-api-path-slug: organizers-post
      parameters:
      - in: query
        name: organizer.description.html
        description: The description of the organizer
        type: query
      - in: query
        name: organizer.facebook
        description: The Facebook URL ID for the organizer
        type: query
      - in: query
        name: organizer.instagram
        description: The Instagram numeric ID for the organizer
        type: query
      - in: query
        name: organizer.logo.id
        description: The logo id of the organizer
        type: query
      - in: query
        name: organizer.long_description.html
        description: The long description of the organizer
        type: query
      - in: query
        name: organizer.name
        description: The name of the organizer
        type: query
      - in: query
        name: organizer.twitter
        description: The Twitter handle for the organizer
        type: query
      - in: query
        name: organizer.website
        description: The website for the organizer
        type: query
      responses:
        200:
          description: OK
      tags:
      - Organizers
  /organizers/{id}/:
    get:
      summary: Get Organizers
      description: Gets an organizer by ID as organizer.
      operationId: getOrganizers
      x-api-path-slug: organizersid-get
      responses:
        200:
          description: OK
      tags:
      - Organizers
    post:
      summary: Post Organizers
      description: Updates an organizer and returns it as as organizer.
      operationId: postOrganizers
      x-api-path-slug: organizersid-post
      parameters:
      - in: query
        name: organizer.description.html
        description: The description of the organizer
        type: query
      - in: query
        name: organizer.facebook
        description: The Facebook URL ID for the organizer
        type: query
      - in: query
        name: organizer.instagram
        description: The Instagram numeric ID for the organizer
        type: query
      - in: query
        name: organizer.logo.id
        description: The logo id of the organizer
        type: query
      - in: query
        name: organizer.long_description.html
        description: The long description of the organizer
        type: query
      - in: query
        name: organizer.name
        description: The name of the organizer
        type: query
      - in: query
        name: organizer.twitter
        description: The Twitter handle for the organizer
        type: query
      - in: query
        name: organizer.website
        description: The website for the organizer
        type: query
      responses:
        200:
          description: OK
      tags:
      - Organizers
  /organizers/{id}/events/:
    get:
      summary: Get Organizers Events
      description: Gets events of the organizer.
      operationId: getOrganizersEvents
      x-api-path-slug: organizersidevents-get
      parameters:
      - in: query
        name: only_public
        description: Only show public events even if viewing your own events
        type: query
      - in: query
        name: order_by
        description: 'How to order the results (Valid choices are: start_asc, start_desc,
          created_asc, or created_desc)'
        type: query
      - in: query
        name: start_date.range_end
        description: Only return events with start dates before the given date
        type: query
      - in: query
        name: start_date.range_start
        description: Only return events with start dates after the given date
        type: query
      - in: query
        name: status
        description: Only return events with a specific status set
        type: query
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - Events
  /pricing/fee_rates/:
    get:
      summary: Get Pricing Fee Rates
      description: |-
        Returns a list of fee_rate objects for the different
        currencies, countries, assortments and sales channels we sell through
        today and in the future.
      operationId: getPricingFeeRates
      x-api-path-slug: pricingfee-rates-get
      parameters:
      - in: query
        name: channel
        description: The sales channel
        type: query
      - in: query
        name: country
        description: The (ISO 3166 alpha-2 code of the) country where you want to
          know the fee rates
        type: query
      - in: query
        name: currency
        description: The (ISO 4217 3-character code of the) currency where you want
          to know the fee rates
        type: query
      - in: query
        name: item_type
        description: The item type for which get the price fee rates
        type: query
      - in: query
        name: payment_type
        description: The payment type to get the price for
        type: query
      - in: query
        name: plan
        description: The assortment package name to get the price for
        type: query
      responses:
        200:
          description: OK
      tags:
      - Pricing
      - Fee
      - Rates
  /refund_requests/{id}/:
    get:
      summary: Get Refund Requests
      description: Gets a refund-request for the specified refund request.
      operationId: getRefundRequests
      x-api-path-slug: refund-requestsid-get
      responses:
        200:
          description: OK
      tags:
      - Refund
      - Requests
    post:
      summary: Post Refund Requests
      description: Update a refund-request for a specific order. Each element in items
        is a refund-item
      operationId: postRefundRequests
      x-api-path-slug: refund-requestsid-post
      parameters:
      - in: query
        name: from_email
        description: The email of the person is making the request
        type: query
      - in: query
        name: from_name
        description: The name of the person is making the request
        type: query
      - in: query
        name: items
        description: 'A list of items formatted as: [{&#8220;order_id&#8221;: &#8220;123&#8221;},'
        type: query
      - in: query
        name: message
        description: The Message of the request
        type: query
      - in: query
        name: reason
        description: 'The reason of the request (Valid choices are: duplicate_order,
          event_cancelled, event_not_as_described, no_longer_able_to_attend, event_postponed,
          request_not_within_event_refund_policy, request_inaccurate, refunded_offline,
          or alternate_resolution_offered)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Refund
      - Requests
  /refund_requests/:
    post:
      summary: Post Refund Requests
      description: Creates a refund-request for a specific order. Each element in
        items is a refund-item
      operationId: postRefundRequests
      x-api-path-slug: refund-requests-post
      parameters:
      - in: query
        name: from_email
        description: The email of the person is making the request
        type: query
      - in: query
        name: from_name
        description: The name of the person is making the request
        type: query
      - in: query
        name: items
        description: 'A list of items formatted as: [{&#8220;order_id&#8221;: &#8220;123&#8221;},'
        type: query
      - in: query
        name: message
        description: The Message of the request
        type: query
      - in: query
        name: reason
        description: 'The reason of the request (Valid choices are: duplicate_order,
          event_cancelled, event_not_as_described, no_longer_able_to_attend, event_postponed,
          request_not_within_event_refund_policy, request_inaccurate, refunded_offline,
          or alternate_resolution_offered)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Refund
      - Requests
  /reports/sales/:
    get:
      summary: Get Reports Sales
      description: Returns a response of the aggregate sales data.
      operationId: getReportsSales
      x-api-path-slug: reportssales-get
      parameters:
      - in: query
        name: date_facet
        description: Optional date aggregation level to return data for
        type: query
      - in: query
        name: end_date
        description: Optional end date to query
        type: query
      - in: query
        name: event_ids
        description: List of public event IDs to report on
        type: query
      - in: query
        name: event_status
        description: 'Event status to filter down results by (Valid choices are: all,
          live, or ended)'
        type: query
      - in: query
        name: filter_by
        description: 'Optional filters for sales/attendees data formatted as: {&#8220;ticket_ids&#8221;:
          [1234, 5678], &#8220;currencies&#8221;: [&#8220;USD&#8221;],'
        type: query
      - in: query
        name: group_by
        description: 'Optional field to group data on (Valid choices are: payment_method,
          payment_method_application, ticket, ticket_application, currency, event_currency,
          reserved_section, event, event_ticket, event_application, country, city,
          state, source, zone, location, access_level, device_name, sales_channel_lvl_1,
          sales_channel_lvl_2, or sales_channel_lvl_3)'
        type: query
      - in: query
        name: period
        description: Time period to provide aggregation for in units of the selected
          date_facet
        type: query
      - in: query
        name: start_date
        description: Optional start date to query
        type: query
      - in: query
        name: timezone
        description: Optional timezone
        type: query
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Sales
  /reports/attendees/:
    get:
      summary: Get Reports Attendees
      description: Returns a response of the aggregate attendees data.
      operationId: getReportsAttendees
      x-api-path-slug: reportsattendees-get
      parameters:
      - in: query
        name: date_facet
        description: Optional date aggregation level to return data for
        type: query
      - in: query
        name: end_date
        description: Optional end date to query
        type: query
      - in: query
        name: event_ids
        description: List of public event IDs to report on
        type: query
      - in: query
        name: event_status
        description: 'Event status to filter down results by (Valid choices are: all,
          live, or ended)'
        type: query
      - in: query
        name: filter_by
        description: 'Optional filters for sales/attendees data formatted as: {&#8220;ticket_ids&#8221;:
          [1234, 5678], &#8220;currencies&#8221;: [&#8220;USD&#8221;],'
        type: query
      - in: query
        name: group_by
        description: 'Optional field to group data on (Valid choices are: payment_method,
          payment_method_application, ticket, ticket_application, currency, event_currency,
          reserved_section, event, event_ticket, event_application, country, city,
          state, source, zone, location, access_level, device_name, sales_channel_lvl_1,
          sales_channel_lvl_2, or sales_channel_lvl_3)'
        type: query
      - in: query
        name: period
        description: Time period to provide aggregation for in units of the selected
          date_facet
        type: query
      - in: query
        name: start_date
        description: Optional start date to query
        type: query
      - in: query
        name: timezone
        description: Optional timezone
        type: query
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Attendees
  /system/timezones/:
    get:
      summary: Get System Timezones
      description: |-
        Returns a paginated response with a key of timezones,
        containing a list of timezones.
      operationId: getSystemTimezones
      x-api-path-slug: systemtimezones-get
      responses:
        200:
          description: OK
      tags:
      - System
      - Timezones
  /system/regions/:
    get:
      summary: Get System Regions
      description: |-
        Returns a single page response with a key of regions,
        containing a list of regions.
      operationId: getSystemRegions
      x-api-path-slug: systemregions-get
      responses:
        200:
          description: OK
      tags:
      - System
      - Regions
  /system/countries/:
    get:
      summary: Get System Countries
      description: |-
        Returns a single page response with a key of countries,
        containing a list of countries.
      operationId: getSystemCountries
      x-api-path-slug: systemcountries-get
      responses:
        200:
          description: OK
      tags:
      - System
      - Countries
  /ticket_groups/:ticket_group_id/:
    get:
      summary: Get Ticket Groups Ticket Group
      description: Returns the ticket_group with the specified :ticket_group_id.
      operationId: getTicketGroupsTicketGroup
      x-api-path-slug: ticket-groupsticket-group-id-get
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - Groups
      - :ticket
      - Group
    delete:
      summary: Delete Ticket Groups Ticket Group
      description: |-
        Deletes the ticket_group with the specified :ticket_group_id.
        The status of the ticket group is changed to deleted.
      operationId: deleteTicketGroupsTicketGroup
      x-api-path-slug: ticket-groupsticket-group-id-delete
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - Groups
      - :ticket
      - Group
    post:
      summary: Post Ticket Groups Ticket Group
      description: Updates the ticket group with the specified :ticket_group_id. Returns
        the updated ticket_group.
      operationId: postTicketGroupsTicketGroup
      x-api-path-slug: ticket-groupsticket-group-id-post
      parameters:
      - in: query
        name: ticket_group.event_ticket_ids
        description: (&#8216;IDs of tickets by event id for this ticket group
        type: query
      - in: query
        name: ticket_group.name
        description: Name of ticket group
        type: query
      - in: query
        name: ticket_group.status
        description: The status of ticket group
        type: query
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - Groups
      - :ticket
      - Group
  /ticket_groups/:
    post:
      summary: Post Ticket Groups
      description: |-
        Creates a ticket group and returns the created ticket_group.
        Only up to 200 live ticket groups may be created; those with archived or deleted status are not taken into account.
      operationId: postTicketGroups
      x-api-path-slug: ticket-groups-post
      parameters:
      - in: query
        name: ticket_group.event_ticket_ids
        description: (&#8216;IDs of tickets by event id for this ticket group
        type: query
      - in: query
        name: ticket_group.name
        description: Name of ticket group
        type: query
      - in: query
        name: ticket_group.status
        description: The status of ticket group
        type: query
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - Groups
  /tracking_beacons/:
    post:
      summary: Post Tracking Beacons
      description: Makes a new tracking beacon. Returns an tracking_beacon as tracking_beacon.
        Either event_id or user_id is required for each tracking beacon. If the event_id
        is provided, the tracking pixel will fire only for that event. If the user_id
        is provided, the tracking pixel will fire for all events organized by that
        user.
      operationId: postTrackingBeacons
      x-api-path-slug: tracking-beacons-post
      parameters:
      - in: query
        name: event_id
        description: The Event ID of the event that this tracking beacon will fire
          in
        type: query
      - in: query
        name: pixel_id
        description: The Pixel ID given by the third party that will fire when a attendee
          lands on the page you are tracking
        type: query
      - in: query
        name: tracking_type
        description: The tracking pixel third party type
        type: query
      - in: query
        name: triggers
        description: The additional pixel data needed to determine which page to fire
          the tracking pixel on
        type: query
      - in: query
        name: user_id
        description: The User ID wherein the tracking beacon will be assigned to all
          of this user&#8217;s events
        type: query
      responses:
        200:
          description: OK
      tags:
      - Tracking
      - Beacons
  /tracking_beacons/:tracking_beacons_id/:
    get:
      summary: Get Tracking Beacons Tracking Beacons
      description: Returns the tracking_beacon with the specified :tracking_beacons_id.
      operationId: getTrackingBeaconsTrackingBeacons
      x-api-path-slug: tracking-beaconstracking-beacons-id-get
      parameters:
      - in: query
        name: return_fmt
        description: returned format
        type: query
      responses:
        200:
          description: OK
      tags:
      - Tracking
      - Beacons
      - :tracking
      - Beacons
    post:
      summary: Post Tracking Beacons Tracking Beacons
      description: Updates the tracking_beacons with the specified :tracking_beacons_id.
        Though event_id and user_id are not individually required, it is a requirement
        to have a tracking beacon where either one must exist. Returns an tracking_beacon
        as tracking_beacon.
      operationId: postTrackingBeaconsTrackingBeacons
      x-api-path-slug: tracking-beaconstracking-beacons-id-post
      parameters:
      - in: query
        name: event_id
        description: The Event ID of the event that this tracking beacon will fire
          in
        type: query
      - in: query
        name: pixel_id
        description: The Pixel ID given by the third party that will fire when a attendee
          lands on the page you are tracking
        type: query
      - in: query
        name: tracking_type
        description: The tracking pixel third party type
        type: query
      - in: query
        name: triggers
        description: The additional pixel data needed to determine which page to fire
          the tracking pixel on
        type: query
      - in: query
        name: user_id
        description: The User ID wherein the tracking beacon will be assigned to all
          of this user&#8217;s events
        type: query
      responses:
        200:
          description: OK
      tags:
      - Tracking
      - Beacons
      - :tracking
      - Beacons
    delete:
      summary: Delete Tracking Beacons Tracking Beacons
      description: Delete the tracking_beacons with the specified :tracking_beacons_id.
      operationId: deleteTrackingBeaconsTrackingBeacons
      x-api-path-slug: tracking-beaconstracking-beacons-id-delete
      responses:
        200:
          description: OK
      tags:
      - Tracking
      - Beacons
      - :tracking
      - Beacons
  /events/:event_id/tracking_beacons/:
    get:
      summary: Get Events Event Tracking Beacons
      description: Returns the list of tracking_beacon for the event :event_id
      operationId: getEventsEventTrackingBeacons
      x-api-path-slug: eventsevent-idtracking-beacons-get
      parameters:
      - in: query
        name: return_fmt
        description: returned format
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Tracking
      - Beacons
  /users/:user_id/tracking_beacons/:
    get:
      summary: Get Users User Tracking Beacons
      description: Returns the list of tracking_beacon for the user :user_id
      operationId: getUsersUserTrackingBeacons
      x-api-path-slug: usersuser-idtracking-beacons-get
      parameters:
      - in: query
        name: return_fmt
        description: returned format
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - :user
      - Tracking
      - Beacons
  /users/{id}/:
    get:
      summary: Get Users
      description: Returns a user for the specified user as user. If you want to get
        details about the currently authenticated user, use /users/me/.
      operationId: getUsers
      x-api-path-slug: usersid-get
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{id}/orders/:
    get:
      summary: Get Users Orders
      description: Returns a paginated response of orders, under the key orders, of
        all orders the user has placed (i.e. where the user was the person buying
        the tickets).
      operationId: getUsersOrders
      x-api-path-slug: usersidorders-get
      parameters:
      - in: query
        name: '&#160;'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Orders
  /users/{id}/organizers/:
    get:
      summary: Get Users Organizers
      description: Returns a paginated response of organizer objects that are owned
        by the user.
      operationId: getUsersOrganizers
      x-api-path-slug: usersidorganizers-get
      parameters:
      - in: query
        name: hide_unsaved
        description: 'True: Will hide organizers flagged as &#8220;unsaved&#8221;False:
          Will show organizers regardless of unsaved flag (Default value)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Organizers
  /users/{id}/owned_events/:
    get:
      summary: Get Users Owned Events
      description: |-
        Returns a paginated response of events, under
        the key events, of all events the user owns (i.e. events they are organising)
      operationId: getUsersOwnedEvents
      x-api-path-slug: usersidowned-events-get
      parameters:
      - in: query
        name: order_by
        description: 'How to order the results (Valid choices are: start_asc, start_desc,
          created_asc, created_desc, name_asc, or name_desc)'
        type: query
      - in: query
        name: show_series_parent
        description: 'True: Will show parent of a serie instead of childrenFalse:
          Will show children of a serie (Default value)'
        type: query
      - in: query
        name: status
        description: Filter by events with a specific status set
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Owned
      - Events
  /users/{id}/events/:
    get:
      summary: Get Users Events
      description: Returns a paginated response of events, under the key events, of
        all events the user has access to
      operationId: getUsersEvents
      x-api-path-slug: usersidevents-get
      parameters:
      - in: query
        name: currency_filter
        description: Filter event results by currency
        type: query
      - in: query
        name: event_group_id
        description: Filter event results by event_group_id
        type: query
      - in: query
        name: name_filter
        description: Filter event results by name
        type: query
      - in: query
        name: order_by
        description: 'How to order the results (Valid choices are: start_asc, start_desc,
          created_asc, created_desc, name_asc, or name_desc)'
        type: query
      - in: query
        name: page_size
        description: Number of records in each page
        type: query
      - in: query
        name: show_series_parent
        description: 'True: Will show parent of a serie instead of childrenFalse:
          Will show children of a serie (Default value)'
        type: query
      - in: query
        name: status
        description: Filter by events with a specific status set
        type: query
      - in: query
        name: time_filter
        description: Limits results to either past or current &amp; future events
          / orders
        type: query
      - in: query
        name: venue_filter
        description: Filter event results by venue IDs
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Events
  /organizations/{id}/events/:
    post:
      summary: Post Organizations Events
      description: Creates new events objects under an organization and returns it
        as event.
      operationId: postOrganizationsEvents
      x-api-path-slug: organizationsidevents-post
      parameters:
      - in: query
        name: event.capacity
        description: Set specific capacity (if omitted, sums ticket capacities)
        type: query
      - in: query
        name: event.category_id
        description: The category (vertical) of the event
        type: query
      - in: query
        name: event.currency
        description: Event currency (3 letter code)
        type: query
      - in: query
        name: event.description.html
        description: The description on the event page
        type: query
      - in: query
        name: event.end.timezone
        description: End time timezone (Olson format)
        type: query
      - in: query
        name: event.end.utc
        description: The end time of the event
        type: query
      - in: query
        name: event.format_id
        description: The format (general type) of the event
        type: query
      - in: query
        name: event.hide_end_date
        description: Whether the end date should be hidden
        type: query
      - in: query
        name: event.hide_start_date
        description: Whether the start date should be hidden
        type: query
      - in: query
        name: event.invite_only
        description: Only invited users can see the event page
        type: query
      - in: query
        name: event.is_reserved_seating
        description: If the event is reserved seating
        type: query
      - in: query
        name: event.listed
        description: If the event is publicly listed and searchable
        type: query
      - in: query
        name: event.logo.id
        description: (Deprecated) The logo for the event
        type: query
      - in: query
        name: event.logo_id
        description: The logo for the event
        type: query
      - in: query
        name: event.name.html
        description: The name of the event
        type: query
      - in: query
        name: event.online_event
        description: Is the event online-only (no venue)?
        type: query
      - in: query
        name: event.organizer_id
        description: The ID of the organizer of this event
        type: query
      - in: query
        name: event.password
        description: Password needed to see the event in unlisted mode
        type: query
      - in: query
        name: event.shareable
        description: If users can share the event on social media
        type: query
      - in: query
        name: event.show_pick_a_seat
        description: For reserved seating event, if attendees can pick their seats
        type: query
      - in: query
        name: event.show_remaining
        description: If the remaining number of tickets is publicly visible on the
          event page
        type: query
      - in: query
        name: event.show_seatmap_thumbnail
        description: For reserved seating event, if venue map thumbnail visible on
          the event page
        type: query
      - in: query
        name: event.source
        description: Source of the event (defaults to API)
        type: query
      - in: query
        name: event.start.timezone
        description: Start time timezone (Olson format)
        type: query
      - in: query
        name: event.start.utc
        description: The start time of the event
        type: query
      - in: query
        name: event.subcategory_id
        description: The subcategory of the event (US only)
        type: query
      - in: query
        name: event.venue_id
        description: ID of the venue
        type: query
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Events
  /users/{id}/venues/:
    get:
      summary: Get Users Venues
      description: Returns a paginated response of venue objects that are owned by
        the user.
      operationId: getUsersVenues
      x-api-path-slug: usersidvenues-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Venues
  /organizations/{id}/venues/:
    post:
      summary: Post Organizations Venues
      description: Creates new venue objects under an organization and returns it
        as venue.
      operationId: postOrganizationsVenues
      x-api-path-slug: organizationsidvenues-post
      parameters:
      - in: query
        name: venue.address.address_1
        description: The first line of the address
        type: query
      - in: query
        name: venue.address.address_2
        description: The second line of the address
        type: query
      - in: query
        name: venue.address.city
        description: The city where the venue is
        type: query
      - in: query
        name: venue.address.country
        description: The country where the venue is
        type: query
      - in: query
        name: venue.address.latitude
        description: The latitude of the coordinates for the venue
        type: query
      - in: query
        name: venue.address.longitude
        description: The longitude of the coordinates for the venue
        type: query
      - in: query
        name: venue.address.postal_code
        description: The postal_code where the venue is
        type: query
      - in: query
        name: venue.address.region
        description: The region where the venue is
        type: query
      - in: query
        name: venue.age_restriction
        description: The age restrictions for the venue
        type: query
      - in: query
        name: venue.capacity
        description: The max capacity for the venue
        type: query
      - in: query
        name: venue.google_place_id
        description: The google place id for the venue
        type: query
      - in: query
        name: venue.name
        description: The name of the venue
        type: query
      - in: query
        name: venue.organizer_id
        description: The organizer this venue belongs to (optional - leave this off
          to use the default organizer)
        type: query
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Venues
  /users/{id}/owned_event_attendees/:
    get:
      summary: Get Users Owned Event Attendees
      description: |-
        Returns a paginated response of attendees,
        under the key attendees, of attendees visiting any of the events the user owns
        (events that would be returned from /users/:id/owned_events/)
      operationId: getUsersOwnedEventAttendees
      x-api-path-slug: usersidowned-event-attendees-get
      parameters:
      - in: query
        name: changed_since
        description: Only return resource changed on or after the time given
        type: query
      - in: query
        name: status
        description: Limits results to either confirmed attendees or cancelled/refunded/etc
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Owned
      - Event
      - Attendees
  /users/{id}/owned_event_orders/:
    get:
      summary: Get Users Owned Event Orders
      description: |-
        Returns a paginated response of orders,
        under the key orders, of orders placed against any of the events the user owns
        (events that would be returned from /users/:id/owned_events/)
      operationId: getUsersOwnedEventOrders
      x-api-path-slug: usersidowned-event-orders-get
      parameters:
      - in: query
        name: changed_since
        description: Only return resource changed on or after the time given
        type: query
      - in: query
        name: exclude_emails
        description: Don&#8217;t include orders placed by any of these emails
        type: query
      - in: query
        name: only_emails
        description: Only include orders placed by one of these emails
        type: query
      - in: query
        name: status
        description: 'Filter to active (attending), inactive (not attending), or all
          (both) orders (Valid choices are: active, inactive, or all)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Owned
      - Event
      - Orders
  /users/{id}/contact_lists/:
    get:
      summary: Get Users Contact Lists
      description: |-
        Returns a list of contact_list that the user owns as the key
        contact_lists.
      operationId: getUsersContactLists
      x-api-path-slug: usersidcontact-lists-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
    post:
      summary: Post Users Contact Lists
      description: |-
        Makes a new contact_list for the user and returns it as
        contact_list.
      operationId: postUsersContactLists
      x-api-path-slug: usersidcontact-lists-post
      parameters:
      - in: query
        name: contact_list.name
        description: Name of the new contact list
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
  /users/{id}/contact_lists/:contact_list_id/:
    get:
      summary: Get Users Contact Lists Contact List
      description: Gets a user&#8217;s contact_list by ID as contact_list.
      operationId: getUsersContactListsContactList
      x-api-path-slug: usersidcontact-listscontact-list-id-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
      - :contact
      - List
    post:
      summary: Post Users Contact Lists Contact List
      description: Updates the contact_list and returns it as contact_list.
      operationId: postUsersContactListsContactList
      x-api-path-slug: usersidcontact-listscontact-list-id-post
      parameters:
      - in: query
        name: contact_list.name
        description: New name of the contact list
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
      - :contact
      - List
    delete:
      summary: Delete Users Contact Lists Contact List
      description: 'Deletes the contact list. Returns {&quot;deleted&quot;: true}.'
      operationId: deleteUsersContactListsContactList
      x-api-path-slug: usersidcontact-listscontact-list-id-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
      - :contact
      - List
  /users/{id}/contact_lists/:contact_list_id/contacts/:
    get:
      summary: Get Users Contact Lists Contact List Contacts
      description: |-
        Returns the contacts on the contact list
        as contacts.
      operationId: getUsersContactListsContactListContacts
      x-api-path-slug: usersidcontact-listscontact-list-idcontacts-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
      - :contact
      - List
      - Contacts
    post:
      summary: Post Users Contact Lists Contact List Contacts
      description: 'Adds a new contact to the contact list. Returns {&quot;created&quot;:
        true}.'
      operationId: postUsersContactListsContactListContacts
      x-api-path-slug: usersidcontact-listscontact-list-idcontacts-post
      parameters:
      - in: query
        name: contact.email
        description: Contact&#8217;s email address
        type: query
      - in: query
        name: contact.first_name
        description: Contact&#8217;s first name (or full name)
        type: query
      - in: query
        name: contact.last_name
        description: Contact&#8217;s last name
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
      - :contact
      - List
      - Contacts
    delete:
      summary: Delete Users Contact Lists Contact List Contacts
      description: |-
        Deletes the specified contact from the contact list.
        Returns {&quot;deleted&quot;: true}.
      operationId: deleteUsersContactListsContactListContacts
      x-api-path-slug: usersidcontact-listscontact-list-idcontacts-delete
      parameters:
      - in: query
        name: email
        description: Email address to remove
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
      - :contact
      - List
      - Contacts
  /users/{id}/bookmarks/:
    get:
      summary: Get Users Bookmarks
      description: Gets all the user&#8217;s saved events.
      operationId: getUsersBookmarks
      x-api-path-slug: usersidbookmarks-get
      parameters:
      - in: query
        name: bookmark_list_id
        description: Optional bookmark list id to fetch all bookmarks from
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Bookmarks
  /users/{id}/bookmarks/save/:
    post:
      summary: Post Users Bookmarks Save
      description: 'Adds a new bookmark for the user. Returns {&quot;created&quot;:
        true}.'
      operationId: postUsersBookmarksSave
      x-api-path-slug: usersidbookmarkssave-post
      parameters:
      - in: query
        name: bookmark_list_id
        description: Optional Bookmark list id to save the bookmark(s) to
        type: query
      - in: query
        name: event_id
        description: Event id to bookmark for the user
        type: query
      - in: query
        name: event_ids
        description: Event ids to batch bookmark for the user
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Bookmarks
      - Save
  /users/{id}/bookmarks/unsave/:
    post:
      summary: Post Users Bookmarks Unsave
      description: 'Removes the specified bookmark from the event for the user. Returns
        {&quot;deleted&quot;: true}.'
      operationId: postUsersBookmarksUnsave
      x-api-path-slug: usersidbookmarksunsave-post
      parameters:
      - in: query
        name: bookmark_list_id
        description: Bookmark list id to save the bookmark(s) to
        type: query
      - in: query
        name: event_id
        description: Event id to bookmark for the user
        type: query
      - in: query
        name: event_ids
        description: Event ids to batch bookmark for the user
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Bookmarks
      - Unsave
  /users/:user_id/ticket_groups/:
    get:
      summary: Get Users User Ticket Groups
      description: |-
        Returns a paginated response of ticket_group for the specified user.
        The alias me (/users/me/) may be used to refer to the currently authenticated user.
      operationId: getUsersUserTicketGroups
      x-api-path-slug: usersuser-idticket-groups-get
      parameters:
      - in: query
        name: status
        description: 'Limits results to groups with the specific status (Valid choices
          are: live, archived, deleted, or all)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - :user
      - Ticket
      - Groups
  /users/:user_id/events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/:
    post:
      summary: Post Users User Events Event Ticket Classes Ticket Class Ticket Groups
      description: |-
        Add the Ticket Class with the specified :ticket_class_id of the event with :event_id that
        belongs to the user with :user_id to many Ticket Groups specified with ticket_group_ids.
        If the list provided is empty, remove this ticket class from every ticket group.
      operationId: postUsersUserEventsEventTicketClassesTicketClassTicketGroups
      x-api-path-slug: usersuser-ideventsevent-idticket-classesticket-class-idticket-groups-post
      parameters:
      - in: query
        name: ticket_group_ids
        description: IDs of all ticket group this ticket belongs to
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - :user
      - Events
      - :event
      - Ticket
      - Classes
      - :ticket
      - Class
      - Ticket
      - Groups
  /users/:user_id/discounts/:
    get:
      summary: Get Users User Discounts
      description: |-
        Returns a paginated response of cross_event_discount for the specified user.
        This operation is only supported for the currently authenticated user. The alias me (/users/me/) may be used.
      operationId: getUsersUserDiscounts
      x-api-path-slug: usersuser-iddiscounts-get
      parameters:
      - in: query
        name: code
        description: Search term to find discounts by code/name, in an exact match
          behavior
        type: query
      - in: query
        name: code_filter
        description: Search term to filter discounts by name
        type: query
      - in: query
        name: event_id
        description: ID of the event
        type: query
      - in: query
        name: order_by
        description: 'How to order the results (Valid choices are: code_asc, code_desc,
          discount_type_asc, discount_type_desc, start_asc, or start_desc)'
        type: query
      - in: query
        name: page_size
        description: Number of records in each page
        type: query
      - in: query
        name: scope
        description: Type of discount scopes
        type: query
      - in: query
        name: ticket_group_id
        description: ID of the ticket group
        type: query
      - in: query
        name: type
        description: Filter discounts with a specific discount type set
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - :user
      - Discounts
  /users/{id}/assortment/:
    get:
      summary: Get Users Assortment
      description: Retrieve the assortment for the user.
      operationId: getUsersAssortment
      x-api-path-slug: usersidassortment-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Assortment
    post:
      summary: Post Users Assortment
      description: |-
        Set a user&#8217;s assortment and returns the assortment for the specified
        user.
      operationId: postUsersAssortment
      x-api-path-slug: usersidassortment-post
      parameters:
      - in: query
        name: plan
        description: The assortments package to upgrade/downgrade to
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Assortment
  /venues/{id}/:
    get:
      summary: Get Venues
      description: Returns a venue object.
      operationId: getVenues
      x-api-path-slug: venuesid-get
      responses:
        200:
          description: OK
      tags:
      - Venues
    post:
      summary: Post Venues
      description: Updates a venue and returns it as an object.
      operationId: postVenues
      x-api-path-slug: venuesid-post
      parameters:
      - in: query
        name: venue.address.address_1
        description: The first line of the address
        type: query
      - in: query
        name: venue.address.address_2
        description: The second line of the address
        type: query
      - in: query
        name: venue.address.city
        description: The city where the venue is
        type: query
      - in: query
        name: venue.address.country
        description: The country where the venue is
        type: query
      - in: query
        name: venue.address.latitude
        description: The latitude of the coordinates for the venue
        type: query
      - in: query
        name: venue.address.longitude
        description: The longitude of the coordinates for the venue
        type: query
      - in: query
        name: venue.address.postal_code
        description: The postal_code where the venue is
        type: query
      - in: query
        name: venue.address.region
        description: The region where the venue is
        type: query
      - in: query
        name: venue.age_restriction
        description: The age restrictions for the venue
        type: query
      - in: query
        name: venue.capacity
        description: The max capacity for the venue
        type: query
      - in: query
        name: venue.google_place_id
        description: The google place id for the venue
        type: query
      - in: query
        name: venue.name
        description: The name of the venue
        type: query
      - in: query
        name: venue.organizer_id
        description: The organizer this venue belongs to (optional - leave this off
          to use the default organizer)
        type: query
      responses:
        200:
          description: OK
      tags:
      - Venues
  /venues/:
    post:
      summary: Post Venues
      description: Creates a new venue with associated address.
      operationId: postVenues
      x-api-path-slug: venues-post
      parameters:
      - in: query
        name: venue.address.address_1
        description: The first line of the address
        type: query
      - in: query
        name: venue.address.address_2
        description: The second line of the address
        type: query
      - in: query
        name: venue.address.city
        description: The city where the venue is
        type: query
      - in: query
        name: venue.address.country
        description: The country where the venue is
        type: query
      - in: query
        name: venue.address.latitude
        description: The latitude of the coordinates for the venue
        type: query
      - in: query
        name: venue.address.longitude
        description: The longitude of the coordinates for the venue
        type: query
      - in: query
        name: venue.address.postal_code
        description: The postal_code where the venue is
        type: query
      - in: query
        name: venue.address.region
        description: The region where the venue is
        type: query
      - in: query
        name: venue.age_restriction
        description: The age restrictions for the venue
        type: query
      - in: query
        name: venue.capacity
        description: The max capacity for the venue
        type: query
      - in: query
        name: venue.google_place_id
        description: The google place id for the venue
        type: query
      - in: query
        name: venue.name
        description: The name of the venue
        type: query
      - in: query
        name: venue.organizer_id
        description: The organizer this venue belongs to (optional - leave this off
          to use the default organizer)
        type: query
      responses:
        200:
          description: OK
      tags:
      - Venues
  /venues/{id}/events/:
    get:
      summary: Get Venues Events
      description: Returns events of a given venue.
      operationId: getVenuesEvents
      x-api-path-slug: venuesidevents-get
      parameters:
      - in: query
        name: only_public
        description: Only show public events even if viewing your own events
        type: query
      - in: query
        name: order_by
        description: 'How to order the results (Valid choices are: start_asc, start_desc,
          created_asc, or created_desc)'
        type: query
      - in: query
        name: start_date.range_end
        description: Only return events with start dates before the given date
        type: query
      - in: query
        name: start_date.range_start
        description: Only return events with start dates after the given date
        type: query
      - in: query
        name: status
        description: Only return events with a specific status set
        type: query
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Events
  /webhooks/{id}/:
    get:
      summary: Get Webhooks
      description: Returns a webhook for the specified webhook as webhook.
      operationId: getWebhooks
      x-api-path-slug: webhooksid-get
      responses:
        200:
          description: OK
      tags:
      - Webhooks
    delete:
      summary: Delete Webhooks
      description: Deletes the specified webhook object.
      operationId: deleteWebhooks
      x-api-path-slug: webhooksid-delete
      responses:
        200:
          description: OK
      tags:
      - Webhooks
  /webhooks/:
    get:
      summary: Get Webhooks
      description: Returns the list of webhook objects that belong to the authenticated
        user.
      operationId: getWebhooks
      x-api-path-slug: webhooks-get
      responses:
        200:
          description: OK
      tags:
      - Webhooks
    post:
      summary: Post Webhooks
      description: Creates a webhook for the authenticated user.
      operationId: postWebhooks
      x-api-path-slug: webhooks-post
      parameters:
      - in: query
        name: actions
        description: Determines what actions will trigger the webhook
        type: query
      - in: query
        name: endpoint_url
        description: The target URL of the Webhook subscription
        type: query
      - in: query
        name: event_id
        description: The ID of the event that triggers this webhook
        type: query
      responses:
        200:
          description: OK
      tags:
      - Webhooks
  /series/:
    post:
      summary: Post Series
      description: Creates a new repeating event series. The POST data must include
        information for at least one event date in the series.
      operationId: postSeries
      x-api-path-slug: series-post
      responses:
        200:
          description: OK
      tags:
      - Series
  /series/{id}/:
    get:
      summary: Get Series
      description: Returns a repeating event series parent object for the specified
        repeating event series.
      operationId: getSeries
      x-api-path-slug: seriesid-get
      parameters:
      - in: query
        name: tracking_code
        description: Append the given tracking_code to the event URLs returned
        type: query
      responses:
        200:
          description: OK
      tags:
      - Series
    post:
      summary: Post Series
      description: |-
        Updates a repeating event series parent object, and optionally also creates more event dates or updates or deletes
        existing event dates in the series. In order for a series date to be deleted or updated, there must be no pending or
        completed orders for that date.
      operationId: postSeries
      x-api-path-slug: seriesid-post
      responses:
        200:
          description: OK
      tags:
      - Series
    delete:
      summary: Delete Series
      description: |-
        Deletes a repeating event series and all of its occurrences if the delete is permitted. In order for a delete to be
        permitted, there must be no pending or completed orders for any dates in the series. Returns a boolean indicating
        success or failure of the delete.
      operationId: deleteSeries
      x-api-path-slug: seriesid-delete
      responses:
        200:
          description: OK
      tags:
      - Series
  /series/{id}/publish/:
    post:
      summary: Post Series Publish
      description: |-
        Publishes a repeating event series and all of its occurrences that are not already canceled or deleted. Once a date is cancelled it can still be uncancelled and can be viewed by the public. A deleted date cannot be undeleted and cannot by viewed by the public. In order for
        publish to be permitted, the event must have all necessary information, including a name and description, an organizer,
        at least one ticket, and valid payment options. This API endpoint will return argument errors for event fields that
        fail to validate the publish requirements. Returns a boolean indicating success or failure of the publish.
      operationId: postSeriesPublish
      x-api-path-slug: seriesidpublish-post
      responses:
        200:
          description: OK
      tags:
      - Series
      - Publish
  /series/{id}/unpublish/:
    post:
      summary: Post Series Unpublish
      description: |-
        Unpublishes a repeating event series and all of its occurrences that are not already completed, canceled, or deleted. In
        order for a free series to be unpublished, it must not have any pending or completed orders for any dates, even past
        dates. In order for a paid series to be unpublished, it must not have any pending or completed orders for any dates,
        except that completed orders for past dates that have been completed and paid out do not prevent an unpublish. Returns
        a boolean indicating success or failure of the unpublish.
      operationId: postSeriesUnpublish
      x-api-path-slug: seriesidunpublish-post
      responses:
        200:
          description: OK
      tags:
      - Series
      - Unpublish
  /series/{id}/cancel/:
    post:
      summary: Post Series Cancel
      description: |-
        Cancels a repeating event series and all of its occurrences that are not already canceled or deleted. In order for
        cancel to be permitted, there must be no pending or completed orders for any dates in the series. Returns a boolean
        indicating success or failure of the cancel.
      operationId: postSeriesCancel
      x-api-path-slug: seriesidcancel-post
      responses:
        200:
          description: OK
      tags:
      - Series
      - Cancel
  /series/{id}/events/:
    get:
      summary: Get Series Events
      description: Returns all of the events that belong to this repeating event series.
      operationId: getSeriesEvents
      x-api-path-slug: seriesidevents-get
      parameters:
      - in: query
        name: order_by
        description: 'How to order the results (Valid choices are: start_asc, start_desc,
          created_asc, or created_desc)'
        type: query
      - in: query
        name: time_filter
        description: Limits results to either past or current &amp; future events
        type: query
      - in: query
        name: tracking_code
        description: Append the given tracking_code to the event URLs returned
        type: query
      responses:
        200:
          description: OK
      tags:
      - Series
      - Events
    post:
      summary: Post Series Events
      description: |-
        Creates more event dates or updates or deletes existing event dates in a repeating event series. In order for a series
        date to be deleted or updated, there must be no pending or completed orders for that date.
      operationId: postSeriesEvents
      x-api-path-slug: seriesidevents-post
      responses:
        200:
          description: OK
      tags:
      - Series
      - Events
  /events/search/:
    get:
      summary: Event Search
      description: This method uses our search index to find publicly listed events.
      operationId: Get_event_search_
      x-api-path-slug: eventssearch-get
      parameters:
      - in: query
        name: address
        description: The venue address
      - in: query
        name: category
        description: 'Event categories (comma seperated): conference, conventions,
          entertainment, fundraisers, meetings, other, performances, reunions, sales,
          seminars, social, sports, tradeshows, travel, religion, fairs, food, music,
          recreation'
      - in: query
        name: city
        description: The venue city
      - in: query
        name: country
        description: 2-letter country code, according to the ISO 3166 format
      - in: query
        name: count_only
        description: Only return the total number of events (???true??? or ???false???)
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: date
        description: The event start date
      - in: query
        name: date_created
        description: The date range the event was created, specified by a label or
          by exact dates
      - in: query
        name: date_modified
        description: The date range the event was modified, specified by a label or
          by exact dates
      - in: query
        name: keywords
        description: The search keywords
      - in: query
        name: latitude
        description: If ???within??? is set you can limit your search to wgs84 coordinates
          (latitude, longitude)
      - in: query
        name: longitude
        description: If ???within??? is set you can limit your search to wgs84 coordinates
          (latitude, longitude)
      - in: query
        name: max
        description: Limit the number of events returned
      - in: query
        name: organizer
        description: The organizer name
      - in: query
        name: page
        description: Allows for paging through the results of a query
      - in: query
        name: postal_code
        description: The postal/zip code of the venue
      - in: query
        name: q
        description: The query
        type: string
        format: string
      - in: query
        name: region
        description: The venue state/province/county/territory depending on the country
      - in: query
        name: since_id
        description: Returns events with id greater than ???since_id??? value
      - in: query
        name: sort_by
        description: Sort the list of events by ???id???, ???date???, ???name???,
          ???city???
      - in: query
        name: tracking_link
        description: The tracking link code to add to the event URLs
      - in: query
        name: within
        description: If ???within??? is set and the ???city??? or ???zipcode??? resolve
          to a specific geolocation, the search will be restricted to the specified
          within radius
      - in: query
        name: within_unit
        description: 'If within is set, you can specify the unit to use: ???M??? for
          miles, or ???K??? for kilometers'
      responses:
        200:
          description: OK
      tags:
      - Event
      - Search
  /event_get:
    get:
      summary: Get Event Get
      description: This method returns the data for a given event. Only public events
        are viewable if no authentication is passed.
      operationId: Get_event_get_
      x-api-path-slug: event-get-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: event_id
        description: The ID of the requested event
      responses:
        200:
          description: OK
      tags:
      - Event
      - Get
  /event_new:
    get:
      summary: Get Event New
      description: This method creates a new event. It returns the ID of the newly
        created event.
      operationId: Get_event_new_
      x-api-path-slug: event-new-get
      parameters:
      - in: query
        name: background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_border_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_header_background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_header_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: capacity
        description: The maximum number of people who can attend the event
      - in: query
        name: currency
        description: The event currency in ISO 4217 format (e
      - in: query
        name: custom_footer
        description: Custom HTML footer for your registration page
      - in: query
        name: custom_header
        description: Custom HTML header for your registration page
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: description
        description: The event description
      - in: query
        name: end_date
        description: The event end date and time, in ISO 8601 format (e
      - in: query
        name: organizer_id
        description: The event organizer ID
      - in: query
        name: personalized_url
        description: The event registration URL
      - in: query
        name: privacy
        description: 0 for a private event, 1 for a public event
      - in: query
        name: start_date
        description: The event start date and time, in ISO 8601 format (e
      - in: query
        name: status
        description: The event status
      - in: query
        name: text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: timezone
        description: The event time zone in relation to GMT (e
      - in: query
        name: title
        description: The event title
      - in: query
        name: title_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: venue_id
        description: The event venue ID
      responses:
        200:
          description: OK
      tags:
      - Event
      - New
  /event_update:
    get:
      summary: Get Event Update
      description: This method updates an existing event. Only the fields passed as
        arguments will be modified. This method returns the ID of the modified event.
      operationId: Get_event_update_
      x-api-path-slug: event-update-get
      parameters:
      - in: query
        name: background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_border_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_header_background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_header_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: capacity
        description: The maximum number of people who can attend the event
      - in: query
        name: currency
        description: The event currency in ISO 4217 format (e
      - in: query
        name: custom_footer
        description: Custom HTML footer for your registration page
      - in: query
        name: custom_header
        description: Custom HTML header for your registration page
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: description
        description: The event description
      - in: query
        name: end_date
        description: The event end date and time, in ISO 8601 format (e
      - in: query
        name: event_id
        description: The ID of the event to update
      - in: query
        name: organizer_id
        description: The event organizer ID
      - in: query
        name: personalized_url
        description: The event registration URL subdomain
      - in: query
        name: privacy
        description: 0 for a private event, 1 for a public event
      - in: query
        name: start_date
        description: The event start date and time, in ISO 8601 format (e
      - in: query
        name: status
        description: The event status
      - in: query
        name: text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: timezone
        description: The event time zone in relation to GMT (e
      - in: query
        name: title
        description: The event title
      - in: query
        name: title_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: venue_id
        description: The event venue ID
      responses:
        200:
          description: OK
      tags:
      - Event
      - Update
  /event_copy:
    get:
      summary: Get Event Copy
      description: This method duplicates an existing event, returning the ID of the
        new event.
      operationId: Get_event_copy_
      x-api-path-slug: event-copy-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: event_id
        description: The ID of the existing event
      - in: query
        name: event_name
        description: A new name for this copy of the Event
      responses:
        200:
          description: OK
      tags:
      - Event
      - Copy
  /user_list_events:
    get:
      summary: Get User List Events
      description: This method lists the events created by this user. Only public
        events are returned if no authentication is passed.
      operationId: Get_user_list_events_
      x-api-path-slug: user-list-events-get
      parameters:
      - in: query
        name: asc_or_desc
        description: Valid options include ???asc??? or results in ascending order
          or ???desc??? or descending order based on event start_date
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: do_not_display
        description: Comma separated list without spaces
      - in: query
        name: email
        description: The user email
      - in: query
        name: event_statuses
        description: Comma separated list without spaces
      responses:
        200:
          description: OK
      tags:
      - User
      - List
      - Events
  /ticket_new:
    get:
      summary: Get Ticket New
      description: This method creates new fixed-price or donation ticket types. It
        returns the ID of the newly created ticket.
      operationId: Get_ticket_new_
      x-api-path-slug: ticket-new-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: description
        description: The ticket description
      - in: query
        name: end_sales
        description: The date and time when ticket sales stop, in ISO 8601 format
          (e
      - in: query
        name: event_id
        description: The event ID
      - in: query
        name: include_fee
        description: 0 to add the Eventbrite service fee on top of ticket price, or
          1 to include it in the ticket price
      - in: query
        name: is_donation
        description: 0 for fixed-price tickets, 1 for donations
      - in: query
        name: max
        description: The maximum number of tickets per order
      - in: query
        name: min
        description: The minimum number of tickets per order
      - in: query
        name: name
        description: The ticket name
      - in: query
        name: price
        description: The ticket price
      - in: query
        name: quantity
        description: The number of tickets available
      - in: query
        name: start_sales
        description: The date and time when ticket sales start, in ISO 8601 format
          (e
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - New
  /ticket_update:
    get:
      summary: Get Ticket Update
      description: This method updates an existing ticket type. Only the fields passed
        as arguments will be modified. It returns the ID of the updated ticket.
      operationId: Get_ticket_update_
      x-api-path-slug: ticket-update-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: description
        description: The ticket description
      - in: query
        name: end_sales
        description: The date and time when ticket sales stop, in ISO 8601 format
          (e
      - in: query
        name: hide
        description: Show or hide the ticket type
      - in: query
        name: id
        description: The ticket ID
      - in: query
        name: include_fee
        description: 0 to add the Eventbrite service fee on top of ticket price, or
          1 to include it in the ticket price
      - in: query
        name: is_donation
        description: 0 for fixed-price tickets, 1 for donations
      - in: query
        name: max
        description: The maximum number of tickets per order
      - in: query
        name: min
        description: The minimum number of tickets per order
      - in: query
        name: name
        description: The ticket name
      - in: query
        name: price
        description: The ticket price
      - in: query
        name: quantity
        description: The number of tickets available
      - in: query
        name: start_sales
        description: The date and time when ticket sales start, in ISO 8601 format
          (e
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - Update
  /event_list_attendees:
    get:
      summary: Get Event List Attendees
      description: This method returns a list of attendees for a given event. If no
        authentication is passed, only publicly available attendee records will be
        returned.
      operationId: Get_event_list_attendees_
      x-api-path-slug: event-list-attendees-get
      parameters:
      - in: query
        name: count
        description: Limit the number of attendees returned
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: do_not_display
        description: Comma separated list without spaces that leaves out certain data
          returned
      - in: query
        name: event_id
        description: The ID of the event
      - in: query
        name: page
        description: Allows for paging through the results of a query
      - in: query
        name: show_full_barcodes
        description: If set to ???true???, it will return all barcodes associates
          with the attendee, plus the barcode status, device used, attendee_id, and
          barcode number
      responses:
        200:
          description: OK
      tags:
      - Event
      - List
      - Attendees
  /venue_get:
    get:
      summary: Get Venue Get
      description: This method returns a single venue by id.
      operationId: Get_venue_get_
      x-api-path-slug: venue-get-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: id
        description: The venue id
      responses:
        200:
          description: OK
      tags:
      - Venue
      - Get
  /venue_new:
    get:
      summary: Get Venue New
      description: This method creates a new venue. It returns the ID of the newly
        created venue.
      operationId: Get_venue_new_
      x-api-path-slug: venue-new-get
      parameters:
      - in: query
        name: adress
        description: The venue address (line 1)
      - in: query
        name: adress_2
        description: The venue address (line 2)
      - in: query
        name: city
        description: The venue city
      - in: query
        name: country_code
        description: 2-letter country code, according to the ISO 3166 format
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: organizer_id
        description: The ID of the related organizer
      - in: query
        name: postal_code
        description: The postal code of the venue
      - in: query
        name: region
        description: The venue state/province/county/territory depending on the country
      - in: query
        name: venue
        description: The venue name
      responses:
        200:
          description: OK
      tags:
      - Venue
      - New
  /venue_update:
    get:
      summary: Get Venue Update
      description: This method updates an existing venue. Only the fields passed as
        arguments will be modified. It returns the ID of the updated venue.
      operationId: Get_venue_update_
      x-api-path-slug: venue-update-get
      parameters:
      - in: query
        name: adress
        description: The venue address (line 1)
      - in: query
        name: adress_2
        description: The venue address (line 2)
      - in: query
        name: city
        description: The venue city
      - in: query
        name: country_code
        description: 2-letter country code, according to the ISO 3166 format
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: id
        description: The venue ID
      - in: query
        name: postal_code
        description: The postal code of the venue
      - in: query
        name: region
        description: The venue state/province/county/territory depending on the country
      - in: query
        name: venue
        description: The venue name
      responses:
        200:
          description: OK
      tags:
      - Venue
      - Update
  /user_list_venues:
    get:
      summary: Get User List Venues
      description: This method lists the venues created by this user. Requires authentication.
      operationId: Get_user_list_venues_
      x-api-path-slug: user-list-venues-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      responses:
        200:
          description: OK
      tags:
      - User
      - List
      - Venues
  /organizer_list_events:
    get:
      summary: Get Organizer List Events
      description: This method returns a list of events for a given organizer.
      operationId: Get_organizer_list_events_
      x-api-path-slug: organizer-list-events-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: id
        description: The organizer id
      responses:
        200:
          description: OK
      tags:
      - Organizer
      - List
      - Events
  /organizer_get:
    get:
      summary: Get Organizer Get
      description: This method returns a single organizer by id.
      operationId: Get_organizer_get_
      x-api-path-slug: organizer-get-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: id
        description: The organizer profile id
      responses:
        200:
          description: OK
      tags:
      - Organizer
      - Get
  /organizer_new:
    get:
      summary: Get Organizer New
      description: Many event creators prefer having a specific person identified
        as the point of contact for their event. This person is usually someone like
        the event emcee, or an on-site contact that can help with attendee check-ins
        or other issues during the event. This method creates a new organizer, and
        returns the organizer_id for the newly created resource.
      operationId: Get_organizer_new_
      x-api-path-slug: organizer-new-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: description
        description: The organizer description
      - in: query
        name: name
        description: The organizer name
      responses:
        200:
          description: OK
      tags:
      - Organizer
      - New
  /organizer_update:
    get:
      summary: Get Organizer Update
      description: This method updates an existing organizer. Only the fields passed
        as arguments will be modified. It returns the ID of the updated organizer.
      operationId: Get_organizer_update_
      x-api-path-slug: organizer-update-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: description
        description: The organizer description
      - in: query
        name: id
        description: The organizer ID
      - in: query
        name: name
        description: The organizer name
      responses:
        200:
          description: OK
      tags:
      - Organizer
      - Update
  /user_list_organizers:
    get:
      summary: Get User List Organizers
      description: This method lists the organizers created by this user. Requires
        authentication.
      operationId: Get_user_list_organizers_
      x-api-path-slug: user-list-organizers-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      responses:
        200:
          description: OK
      tags:
      - User
      - List
      - Organizers
  /user_list_tickets:
    get:
      summary: Get User List Tickets
      description: This method lists the tickets purchased by the authenticated user.
        Each transaction is an order in our system and an order may contain one or
        more tickets. Tickets to free events are included.
      operationId: Get_user_list_tickets_
      x-api-path-slug: user-list-tickets-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      responses:
        200:
          description: OK
      tags:
      - User
      - List
      - Tickets
  /user_get:
    get:
      summary: Get User Get
      description: This method returns the user account identified by the user_id
        or email request parameters. Visibility is limited to users and sub-users
        of the given user_key.
      operationId: Get_user_get_
      x-api-path-slug: user-get-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: email
        description: The email address of the subuser account
      - in: query
        name: user_id
        description: The ID of the subuser account
      responses:
        200:
          description: OK
      tags:
      - User
      - Get
  /user_new:
    get:
      summary: Get User New
      description: This method creates a new user, returning the user???s ID in the
        response.
      operationId: Get_user_new_
      x-api-path-slug: user-new-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: email
        description: The user email address
      - in: query
        name: passwd
        description: The user password
      responses:
        200:
          description: OK
      tags:
      - User
      - New
  /user_update:
    get:
      summary: Get User Update
      description: This method updates an existing user. Only the fields passed as
        arguments will be modified. It returns the ID of the updated user.
      operationId: Get_user_update_
      x-api-path-slug: user-update-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: new_email
        description: New user email address
      - in: query
        name: new_password
        description: New user password
      responses:
        200:
          description: OK
      tags:
      - User
      - Update
  /event_list_discounts:
    get:
      summary: Get Event List Discounts
      description: This method returns a list of discounts for a given event.
      operationId: Get_event_list_discounts_
      x-api-path-slug: event-list-discounts-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: id
        description: The ID of the event
      responses:
        200:
          description: OK
      tags:
      - Event
      - List
      - Discounts
  /discount_new:
    get:
      summary: Get Discount New
      description: This method creates a new discount code for a specific event. It
        returns the ID of the newly created discount code.
      operationId: Get_discount_new_
      x-api-path-slug: discount-new-get
      parameters:
      - in: query
        name: amount_off
        description: The fixed amount off the ticket price
      - in: query
        name: code
        description: The discount code
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: end_date
        description: The discount end date and time, in ISO 8601 format (e
      - in: query
        name: event_id
        description: The event ID
      - in: query
        name: percent_off
        description: The percentage off the ticket price
      - in: query
        name: quantity_available
        description: Maximum number of times this discount can be used
      - in: query
        name: start_date
        description: The discount start date and time, in ISO 8601 format (e
      - in: query
        name: tickets
        description: Comma-separated list of ticket IDs for which the discount applies
      responses:
        200:
          description: OK
      tags:
      - Discount
      - New
  /discount_update:
    get:
      summary: Get Discount Update
      description: This method is used to update an existing discount code. Only the
        fields passed as arguments will be modified. This method returns the ID of
        the modified discount code.
      operationId: Get_discount_update_
      x-api-path-slug: discount-update-get
      parameters:
      - in: query
        name: amount_off
        description: The fixed amount off the ticket price
      - in: query
        name: code
        description: The discount code
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: end_date
        description: The discount end date and time, in ISO 8601 format (e
      - in: query
        name: id
        description: The discount ID to update
      - in: query
        name: percent_off
        description: The percentage off the ticket price
      - in: query
        name: quantity_available
        description: Maximum number of times this discount can be used
      - in: query
        name: start_date
        description: The discount start date and time, in ISO 8601 format (e
      - in: query
        name: tickets
        description: Comma-separated list of ticket IDs for which the discount applies
      responses:
        200:
          description: OK
      tags:
      - Discount
      - Update
  /payment_update:
    get:
      summary: Get Payment Update
      description: This method creates or updates the payment options for this event.
        Only the fields passed as arguments will be modified.
      operationId: Get_payment_update_
      x-api-path-slug: payment-update-get
      parameters:
      - in: query
        name: accept_cash
        description: Accept ???Pay by Cash??? payments (1 or 0)
      - in: query
        name: accept_check
        description: Accept ???Pay by Check??? payments (1 or 0)
      - in: query
        name: accept_google
        description: Accept Google Checkout payments (1 or 0)
      - in: query
        name: accept_invoice
        description: Accept ???Send an Invoice??? payments (1 or 0)
      - in: query
        name: accept_paypal
        description: Accept PayPal payments (1 or 0)
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: event_id
        description: The event ID
      - in: query
        name: google_merchant_id
        description: Google Checkout Merchant ID
      - in: query
        name: google_merchant_key
        description: Google Checkout Merchant Key
      - in: query
        name: instructions_cash
        description: Instructions to attendees who want to pay by cash
      - in: query
        name: instructions_check
        description: Instructions to attendees who want to pay by check
      - in: query
        name: instructions_invoice
        description: Instructions to attendees who need to be sent an invoice
      - in: query
        name: paypal_email
        description: Your PayPal email
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Update