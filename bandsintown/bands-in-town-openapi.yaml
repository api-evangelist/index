swagger: "2.0"
x-collection-name: Bandsintown
x-complete: 1
info:
  title: Bandsintown API
  description: the-bandsintown-api-is-designed-for-enterprise-partners-and-artists-with-websites-media-players-andor-mobile-applications-that-would-like-to-list-an-artists-events-and-provide-their-users-with-the-ability-to-buy-tickets-and-rsvp-to-these-events--it-offers-readonly-access-to-artist-info-and-artist-events-artist-info-returns-the-link-to-the-bandsintown-artist-page-the-link-to-the-artist-photo-the-current-number-of-trackers-and-more-artist-events-returns-the-list-of-upcoming-events-including-their-date-and-time-venue-name-and-location-ticket-links-lineup-description-and-the-link-to-the-bandsintown-event-page-
  contact:
    name: Bandsintown
    url: https://bandsintown.com/
  version: 1.0.0
host: rest.bandsintown.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /artists/{artistname}:
    get:
      summary: Get artist information
      description: Get artist information
      operationId: artist
      x-api-path-slug: artistsartistname-get
      parameters:
      - in: query
        name: app_id
        description: The application ID assigned to you by Bandsintown
      - in: path
        name: artistname
        description: The name of the artist
      responses:
        200:
          description: OK
      tags:
      - Bands
      - Music
      - Concerts
  /artists/{artistname}/events:
    get:
      summary: Get all upcoming artist events or all past and upcoming events within
        a date range
      description: artist events
      operationId: artistEvents
      x-api-path-slug: artistsartistnameevents-get
      parameters:
      - in: query
        name: app_id
        description: The application ID assigned to you by Bandsintown
      - in: path
        name: artistname
        description: The name of the artist
      - in: query
        name: date
        description: Date range of requested shows e
      responses:
        200:
          description: OK
      tags:
      - Bands
      - Music
      - Concerts