swagger: "2.0"
x-collection-name: PredictHQ
x-complete: 1
info:
  title: PredictHQ API
  description: todo-add-description
  version: 1.0.0
host: api.predicthq.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/signals/{signal_id}/analysis/:
    get:
      summary: Retrieve Analysis
      description: |-
        This action returns a complete analysis of your Signal, which includes what your actual figures were, what could be expected, and what was in excess in terms of **demand**, **lead time** and **duration** and can be explained using events. Note that lead time (`lead`) and duration (`span`) analysis are only available when an `initiated` and `completed` dates are provided with data points, respectively.

        To retrieve a list of events that we estimate impacted your business at a specific date in the past, use the `signal.id` and `signal.explain` parameters with the events endpoint.

        Alternatively, to retrieve a list of predicted events that we estimate will impact your business in the future, use the `signal.id` parameter and the date range you wish a prediction for using `active` or `start`.

        See the events endpoint for more details.

        The `significance` parameter corresponds to percentage of variation in your data that is considered normal when computing excess that can be attributed to events. If you were to look at a normal distribution, it would correspond to the percentage of values that lie within a band around the mean.

        As an example:
        - ~68.27% = 1 standard deviation from the mean
        - ~95.45% = 2 standard deviations from the mean
        - ~99.73% = 3 standard deviations from the mean

        A high `significance` means that only extreme spikes and troughs will be attributed to events. We use 50% as a default, which corresponds to ~0.68 standard deviations.
      operationId: V1SignalsAnalysisBySignalIdGet
      x-api-path-slug: v1signalssignal-idanalysis-get
      parameters:
      - in: path
        name: signal_id
      responses:
        200:
          description: OK
      tags:
      - Signals
      - Signal
      - Analysis
  /v1/signals/{signal_id}/:
    get:
      summary: Retrieve A Signal
      description: This action returns a Signal according to the unique identifier
        you provide.
      operationId: V1SignalsBySignalIdGet
      x-api-path-slug: v1signalssignal-id-get
      parameters:
      - in: path
        name: signal_id
      responses:
        200:
          description: OK
      tags:
      - Signals
      - Signal
    put:
      summary: Update a Signal
      description: This action modifies a Signal according to the unique identifier
        you provide.
      operationId: V1SignalsBySignalIdPut
      x-api-path-slug: v1signalssignal-id-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: signal_id
      responses:
        200:
          description: OK
      tags:
      - Signals
      - Signal
    delete:
      summary: Delete A Signal
      description: This action will delete a Signal altogether along with the Data
        Points associated with it, according to the unique identifier you provide.
      operationId: V1SignalsBySignalIdDelete
      x-api-path-slug: v1signalssignal-id-delete
      parameters:
      - in: path
        name: signal_id
      responses:
        200:
          description: OK
      tags:
      - Signals
      - Signal
  /v1/places/:
    get:
      summary: Search Places
      description: |-
        Use the below parameters to search and filter all places. Places are sorted by relevance (location or text query proximity).

        A search requires at least one of the `q`, `id`, `country` or `location` parameters.
      operationId: V1PlacesGet
      x-api-path-slug: v1places-get
      responses:
        200:
          description: OK
      tags:
      - Places
  /v1/signals/{signal_id}/sink/:
    post:
      summary: Create Data Points
      description: |-
        Every Signal needs a series of Data Points for the API to do its job.

        Unlike the other endpoints, the Data Point sink accepts three content types for uploading your data:
        - `application/json`: A JSON array of Data Points.
        - `application/x-ldjson`: A list of JSON Data Points, one on each line.
        - `text/csv`: A list of Data Points with each column comma-separated, and column names on the first row.

        As a rule of thumb, you should limit the number of records you upload with any single request to 1,000. If you use the CSV format, make sure to repeat the CSV header with each call.

        The global rate limit applies, but to prevent any disruption on critical aspects of your systems, this endpoint will never respond with a `402 Payment Required` in case your subscription expires.

        When required details are missing for some Data Points, instead of rejecting the whole batch, the valid Data Points will be accepted, and the invalid ones will be returned as an array in the body of the response along with a description of the problem.
        If this is the case, the response code will be `202 Accepted` instead of `201 Created`.
      operationId: V1SignalsSinkBySignalIdPost
      x-api-path-slug: v1signalssignal-idsink-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: signal_id
      responses:
        200:
          description: OK
      tags:
      - Signals
      - Signal
      - Sink
  /oauth2/revoke/:
    post:
      summary: Revoking an Access Token
      description: |-
        Access Tokens never expire so once you have it, it's yours for the life of your PredictHQ API subscription.

        However, if you think your token may have been compromised, you have the power to revoke it at any time.
      operationId: Oauth2RevokePost
      x-api-path-slug: oauth2revoke-post
      parameters:
      - in: formData
        name: token
      - in: formData
        name: token_type_hint
      responses:
        200:
          description: OK
      tags:
      - Oauth2
      - Revoke
  /v1/accounts/self/:
    get:
      summary: Retrieve Account Details
      description: If you need your account details for whatever reason, it's really
        easy to get them.
      operationId: V1AccountsSelfGet
      x-api-path-slug: v1accountsself-get
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Self
  /v1/signals/:
    get:
      summary: Retrieve All Signals
      description: It's easy to get a list of all Signals that are associated with
        your account.
      operationId: V1SignalsGet
      x-api-path-slug: v1signals-get
      responses:
        200:
          description: OK
      tags:
      - Signals
    post:
      summary: Create a Signal
      description: Before you do anything else, you need to create a new Signal that
        represents a time series that's important to your business.
      operationId: V1SignalsPost
      x-api-path-slug: v1signals-post
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
      - Signals
  /v1/events/calendar/:
    get:
      summary: Retrieve Events Calendar
      description: |-
        This endpoint accepts the same parameters as the ones described in Retrieve All Events and can be used to get a calendar view of all matching events that are available to your account.

        Each day in the calendar contains aggregate counts of all _active_ events for that day.
      operationId: V1EventsCalendarGet
      x-api-path-slug: v1eventscalendar-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Calendar
  /v1/events/count/:
    get:
      summary: Retrieve Events Count
      description: This endpoint accepts the same parameters as the ones described
        in Retrieve All Events and can be used to get aggregated counts of all matching
        events that are available to your account.
      operationId: V1EventsCountGet
      x-api-path-slug: v1eventscount-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Count
  /v1/events/:
    get:
      summary: Retrieve All Events
      description: Use the below parameters to search and filter all events that are
        available to your account.
      operationId: V1EventsGet
      x-api-path-slug: v1events-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /oauth2/token/:
    post:
      summary: Requesting an Access Token
      description: |-
        When requesting an Access Token, use the `client_credentials` grant type, then request the scope or scopes you wish to have access to.

        These scopes can be any or all of the following, separated by a space:
          - `account` Grants access to the account endpoint.
          - `events` Grants access to the events endpoint.
          - `places` Grants access to the places endpoint.
          - `signals` Grants access to the signals endpoint.

        Please note that Access Tokens requested via the client_credentials grant type never expire.
      operationId: Oauth2TokenPost
      x-api-path-slug: oauth2token-post
      parameters:
      - in: formData
        name: grant_type
      - in: formData
        name: scope
      responses:
        200:
          description: OK
      tags:
      - Oauth2
      - Token
  /v1/signals/{signal_id}/dimensions/:
    get:
      summary: Retrieve All Dimensions
      description: This action returns a summary for each dimension of your Signal.
      operationId: V1SignalsDimensionsBySignalIdGet
      x-api-path-slug: v1signalssignal-iddimensions-get
      parameters:
      - in: path
        name: signal_id
      responses:
        200:
          description: OK
      tags:
      - Signals
      - Signal
      - Dimensions