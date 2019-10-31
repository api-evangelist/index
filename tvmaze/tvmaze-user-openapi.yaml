swagger: "2.0"
x-collection-name: TVmaze
x-complete: 1
info:
  title: TVmaze user
  description: access-to-the-user-api-is-only-possible-for-users-with-a-premiumhttpwww-tvmaze-compremium-account--a-user-can-only-access-their-own-user-data-authentication-uses-http-basic--use-the-tvmaze-username-as-authentication-username-and-the-tvmaze-api-key-as-authentication-password--your-api-key-can-be-found-on-your-dashboardhttpwww-tvmaze-comdashboard--to-try-out-these-api-calls-from-this-page-click-the-authorize-button-on-top-and-input-your-credentials-
  version: "1.0"
host: api.tvmaze.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/episodes:
    get:
      summary: Get User Episodes
      description: Get user episodes.
      operationId: getUserEpisodes
      x-api-path-slug: userepisodes-get
      parameters:
      - in: query
        name: show_id
        description: Only return episodes from this specific show
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Episodes
  /user/episodes/{episode_id}:
    delete:
      summary: Delete User Episodes
      description: Delete user episodes.
      operationId: deleteUserEpisodesEpisode
      x-api-path-slug: userepisodesepisode-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Episodes
    get:
      summary: Get User Episodes
      description: Get user episodes.
      operationId: getUserEpisodesEpisode
      x-api-path-slug: userepisodesepisode-id-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Episodes
    parameters:
      summary: Parameters User Episodes
      description: Parameters user episodes.
      operationId: parametersUserEpisodesEpisode
      x-api-path-slug: userepisodesepisode-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Episodes
    put:
      summary: Put User Episodes
      description: Set `marked_at` to `NULL` or leave it out to use the current time.
      operationId: putUserEpisodesEpisode
      x-api-path-slug: userepisodesepisode-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Episodes
  /user/follows/networks:
    get:
      summary: Get User Follows Networks
      description: Get user follows networks.
      operationId: getUserFollowsNetworks
      x-api-path-slug: userfollowsnetworks-get
      parameters:
      - in: query
        name: embed
        description: Embed full network info
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Networks
  /user/follows/networks/{network_id}:
    delete:
      summary: Delete User Follows Networks
      description: Delete user follows networks.
      operationId: deleteUserFollowsNetworksNetwork
      x-api-path-slug: userfollowsnetworksnetwork-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Networks
    get:
      summary: Get User Follows Networks
      description: Get user follows networks.
      operationId: getUserFollowsNetworksNetwork
      x-api-path-slug: userfollowsnetworksnetwork-id-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Networks
    parameters:
      summary: Parameters User Follows Networks
      description: Parameters user follows networks.
      operationId: parametersUserFollowsNetworksNetwork
      x-api-path-slug: userfollowsnetworksnetwork-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Follows
      - Networks
    put:
      summary: Put User Follows Networks
      description: Put user follows networks.
      operationId: putUserFollowsNetworksNetwork
      x-api-path-slug: userfollowsnetworksnetwork-id-put
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Networks
  /user/follows/people:
    get:
      summary: Get User Follows People
      description: Get user follows people.
      operationId: getUserFollowsPeople
      x-api-path-slug: userfollowspeople-get
      parameters:
      - in: query
        name: embed
        description: Embed full person info
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - People
  /user/follows/people/{person_id}:
    delete:
      summary: Delete User Follows People Person
      description: Delete user follows people person.
      operationId: deleteUserFollowsPeoplePerson
      x-api-path-slug: userfollowspeopleperson-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - People
      - Person
    get:
      summary: Get User Follows People Person
      description: Get user follows people person.
      operationId: getUserFollowsPeoplePerson
      x-api-path-slug: userfollowspeopleperson-id-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - People
      - Person
    parameters:
      summary: Parameters User Follows People Person
      description: Parameters user follows people person.
      operationId: parametersUserFollowsPeoplePerson
      x-api-path-slug: userfollowspeopleperson-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Follows
      - People
      - Person
    put:
      summary: Put User Follows People Person
      description: Put user follows people person.
      operationId: putUserFollowsPeoplePerson
      x-api-path-slug: userfollowspeopleperson-id-put
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - People
      - Person
  /user/follows/shows:
    get:
      summary: Get User Follows Shows
      description: Get user follows shows.
      operationId: getUserFollowsShows
      x-api-path-slug: userfollowsshows-get
      parameters:
      - in: query
        name: embed
        description: Embed full show info
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Shows
  /user/follows/shows/{show_id}:
    delete:
      summary: Delete User Follows Shows
      description: Delete user follows shows.
      operationId: deleteUserFollowsShowsShow
      x-api-path-slug: userfollowsshowsshow-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Shows
    get:
      summary: Get User Follows Shows
      description: Get user follows shows.
      operationId: getUserFollowsShowsShow
      x-api-path-slug: userfollowsshowsshow-id-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Shows
    parameters:
      summary: Parameters User Follows Shows
      description: Parameters user follows shows.
      operationId: parametersUserFollowsShowsShow
      x-api-path-slug: userfollowsshowsshow-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Follows
      - Shows
    put:
      summary: Put User Follows Shows
      description: Put user follows shows.
      operationId: putUserFollowsShowsShow
      x-api-path-slug: userfollowsshowsshow-id-put
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Shows
  /user/follows/webchannels:
    get:
      summary: Get User Follows Webchannels
      description: Get user follows webchannels.
      operationId: getUserFollowsWebchannels
      x-api-path-slug: userfollowswebchannels-get
      parameters:
      - in: query
        name: embed
        description: Embed full webchannel info
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Webchannels
  /user/follows/webchannels/{webchannel_id}:
    delete:
      summary: Delete User Follows Webchannels Webchannel
      description: Delete user follows webchannels webchannel.
      operationId: deleteUserFollowsWebchannelsWebchannel
      x-api-path-slug: userfollowswebchannelswebchannel-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Webchannels
      - Webchannel
    get:
      summary: Get User Follows Webchannels Webchannel
      description: Get user follows webchannels webchannel.
      operationId: getUserFollowsWebchannelsWebchannel
      x-api-path-slug: userfollowswebchannelswebchannel-id-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Webchannels
      - Webchannel
    parameters:
      summary: Parameters User Follows Webchannels Webchannel
      description: Parameters user follows webchannels webchannel.
      operationId: parametersUserFollowsWebchannelsWebchannel
      x-api-path-slug: userfollowswebchannelswebchannel-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Follows
      - Webchannels
      - Webchannel
    put:
      summary: Put User Follows Webchannels Webchannel
      description: Put user follows webchannels webchannel.
      operationId: putUserFollowsWebchannelsWebchannel
      x-api-path-slug: userfollowswebchannelswebchannel-id-put
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Follows
      - Webchannels
      - Webchannel
  /user/votes/episodes:
    get:
      summary: Get User Votes Episodes
      description: Get user votes episodes.
      operationId: getUserVotesEpisodes
      x-api-path-slug: uservotesepisodes-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Episodes
  /user/votes/episodes/{episode_id}:
    delete:
      summary: Delete User Votes Episodes
      description: Delete user votes episodes.
      operationId: deleteUserVotesEpisodesEpisode
      x-api-path-slug: uservotesepisodesepisode-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Episodes
    get:
      summary: Get User Votes Episodes
      description: Get user votes episodes.
      operationId: getUserVotesEpisodesEpisode
      x-api-path-slug: uservotesepisodesepisode-id-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Episodes
    parameters:
      summary: Parameters User Votes Episodes
      description: Parameters user votes episodes.
      operationId: parametersUserVotesEpisodesEpisode
      x-api-path-slug: uservotesepisodesepisode-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Votes
      - Episodes
    put:
      summary: Put User Votes Episodes
      description: Put user votes episodes.
      operationId: putUserVotesEpisodesEpisode
      x-api-path-slug: uservotesepisodesepisode-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Episodes
  /user/votes/shows:
    get:
      summary: Get User Votes Shows
      description: Get user votes shows.
      operationId: getUserVotesShows
      x-api-path-slug: uservotesshows-get
      parameters:
      - in: query
        name: embed
        description: Embed full show info
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Shows
  /user/votes/shows/{show_id}:
    delete:
      summary: Delete User Votes Shows
      description: Delete user votes shows.
      operationId: deleteUserVotesShowsShow
      x-api-path-slug: uservotesshowsshow-id-delete
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Shows
    get:
      summary: Get User Votes Shows
      description: Get user votes shows.
      operationId: getUserVotesShowsShow
      x-api-path-slug: uservotesshowsshow-id-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Shows
    parameters:
      summary: Parameters User Votes Shows
      description: Parameters user votes shows.
      operationId: parametersUserVotesShowsShow
      x-api-path-slug: uservotesshowsshow-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Television
      - Parameters
      - User
      - Votes
      - Shows
    put:
      summary: Put User Votes Shows
      description: Set `voted_at` to `NULL` or leave it out to use the current time.
      operationId: putUserVotesShowsShow
      x-api-path-slug: uservotesshowsshow-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Votes
      - Shows