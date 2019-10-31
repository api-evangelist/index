swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 1
info:
  title: Entertainment Express
  description: your-gateway-to-building-incredible-movie-tv-and-game-content-discovery-experiences-
  version: "2.0"
host: ee.iva-api.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Analytics/City/:
    get:
      summary: Get Viewers by City.
      description: No required parameters, DateValue defaults to Today..
      operationId: GetAnalyticsViewersByCity
      x-api-path-slug: analyticscity-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - City
  /Analytics/Country/:
    get:
      summary: Get Viewers by Country.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsViewersByCountry
      x-api-path-slug: analyticscountry-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - Country
  /Analytics/EngagementActions/:
    get:
      summary: GetAnalyticEngagementActions
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticEngagementActions
      x-api-path-slug: analyticsengagementactions-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - EngagementActions
  /Analytics/EngagementTimes/:
    get:
      summary: Get View count by Frequency.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsEngagementTimes
      x-api-path-slug: analyticsengagementtimes-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - EngagementTimes
  /Analytics/GBUsage/:
    get:
      summary: Get GBUsage by Customer ID.
      description: Requires a valid Customer ID.
      operationId: GetAnalyticsGBUsage
      x-api-path-slug: analyticsgbusage-get
      parameters:
      - in: query
        name: Month
        description: Report month
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Year
        description: Report year
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - GBUsage
  /Analytics/MostActive/:
    get:
      summary: Get Most Active Visitors by IP.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsMostActive
      x-api-path-slug: analyticsmostactive-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - MostActive
  /Analytics/PlatformHardware/:
    get:
      summary: Get Viewers by Platform Hardware.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsViewersByPlatformHardware
      x-api-path-slug: analyticsplatformhardware-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - PlatformHardware
  /Analytics/PlatformOS/:
    get:
      summary: Get Viewers by Platform OS.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsViewersByPlatformOS
      x-api-path-slug: analyticsplatformos-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - PlatformOS
  /Analytics/RecentVisitors/:
    get:
      summary: Get Most Recent Visitors by Time.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsRecentVisitors
      x-api-path-slug: analyticsrecentvisitors-get
      parameters:
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - RecentVisitors
  /Analytics/Summary/:
    get:
      summary: Get Summary by Customer ID.
      description: Requires a valid Customer ID.
      operationId: GetAnalyticsSummary
      x-api-path-slug: analyticssummary-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: ReportTag
        description: Report Tag filter
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - Summary
  /Analytics/TitleReport/:
    get:
      summary: Get Title Report by PublishedID.
      description: Requires a valid published ID.
      operationId: GetAnalyticsTitleReport
      x-api-path-slug: analyticstitlereport-get
      parameters:
      - in: query
        name: End
        description: Report end date
      - in: query
        name: PublishedId
        description: Title published ID
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - TitleReport
  /Analytics/VideoLog/:
    get:
      summary: Get Views by Video.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsViewsByVideoLog
      x-api-path-slug: analyticsvideolog-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - VideoLog
  /Analytics/Viewers/:
    get:
      summary: Get viewers by Day.
      description: Optional DateValue for length of report.
      operationId: GetAnalyticsViewers
      x-api-path-slug: analyticsviewers-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: ReportTag
        description: Report Tag filter
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - Viewers
  /Analytics/Views/:
    get:
      summary: Get views by Day.
      description: Optional DateValue for length of report.
      operationId: GetAnalyticsViews
      x-api-path-slug: analyticsviews-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: ReportTag
        description: Report Tag filter
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - Views
  /Analytics/WebBrowsers/:
    get:
      summary: Get Viewers by Web Browser.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsViewersByWebBrowsers
      x-api-path-slug: analyticswebbrowsers-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - WebBrowsers
  /Changes/Episodes/History/:
    get:
      summary: Returns list of unique EpisodeId changes greater than or equal to date
        (UTC)
      description: For each updated episode ID, pull the full episode data for that
        ID and update.
      operationId: GetEpisodeChangeHistory
      x-api-path-slug: changesepisodeshistory-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Episodes
      - History
  /Changes/Episodes/HistoryWithEntity/:
    get:
      summary: Returns list of unique EpisodeId and Entity changes greater than or
        equal to date (UTC).
      description: Lists each episode ID that has changed as well as the entity in
        the object that changed.
      operationId: GetEpisodeChangeHistoryWithEntity
      x-api-path-slug: changesepisodeshistorywithentity-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Episodes
      - HistoryWithEntity
  /Changes/Movies/History/:
    get:
      summary: Returns list of unique MovieId changes greater than or equal to date
        (UTC).
      description: Use to get the ID's of the movies that have been added or changed
        and use /Movies/{ID} to get back the object with the updated data and replace
        in your database.
      operationId: GetMovieChangeHistory
      x-api-path-slug: changesmovieshistory-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Movies
      - History
  /Changes/Movies/HistoryWithEntity/:
    get:
      summary: Returns list of unique MovieId and Entity changes greater than or equal
        to date (UTC).
      description: Same as /Changes/Movies/History but with the specific entities
        that have changed inside the MovieResponse.
      operationId: GetMovieChangeHistoryWithEntity
      x-api-path-slug: changesmovieshistorywithentity-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Movies
      - HistoryWithEntity
  /Changes/People/History/:
    get:
      summary: Returns list of unique PersonId changes greater than or equal to date
        (UTC).
      description: Requires a valid Date.
      operationId: GetPersonChangeHistory
      x-api-path-slug: changespeoplehistory-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - People
      - History
  /Changes/People/HistoryWithEntity/:
    get:
      summary: Returns list of unique PersonId and Entity changes greater than or
        equal to date (UTC).
      description: Requires a valid Date.
      operationId: GetPersonChangeHistoryWithEntity
      x-api-path-slug: changespeoplehistorywithentity-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - People
      - HistoryWithEntity
  /Changes/Seasons/History/:
    get:
      summary: Returns list of unique SeasonId changes greater than or equal to date
        (UTC).
      description: Use if you want to check for specific updates to season records.
      operationId: GetSeasonChangeHistory
      x-api-path-slug: changesseasonshistory-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Seasons
      - History
  /Changes/Seasons/HistoryWithEntity/:
    get:
      summary: Returns list of unique SeasonId and Entity changes greater than or
        equal to date (UTC).
      description: Returns list of new or changed SeasonIds with the entity that has
        changed.
      operationId: GetSeasonChangeHistoryWithEntity
      x-api-path-slug: changesseasonshistorywithentity-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Seasons
      - HistoryWithEntity
  /Changes/Shows/History/:
    get:
      summary: Returns list of unique ShowId changes greater than or equal to date
        (UTC).
      description: All new and updated shows from requested date and time.  When a
        record gets updated, use the ID to get the full show object and replace the
        data in your cache.
      operationId: GetShowChangeHistory
      x-api-path-slug: changesshowshistory-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Shows
      - History
  /Changes/Shows/HistoryWithEntity/:
    get:
      summary: Returns list of unique ShowId and Entity changes greater than or equal
        to date (UTC).
      description: Returns a list of ShowId and entity of any show that has been updated.
      operationId: GetShowChangeHistoryWithEntity
      x-api-path-slug: changesshowshistorywithentity-get
      parameters:
      - in: query
        name: Date
        description: Starting date
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Shows
      - HistoryWithEntity
  /Charts/Movies/Boxoffice:
    get:
      summary: Returns list of movies based on the weekend box office revenue.
      description: Returns top 10 box office movies.
      operationId: GetChartMoviesBoxoffice
      x-api-path-slug: chartsmoviesboxoffice-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - Charts
      - Movies
      - Boxoffice
  /Charts/Movies/MostAnticipated:
    get:
      summary: Returns list of Most Anticipated movies based on IVA data.
      description: Requires Skip and Take. Maximum page size is 100.
      operationId: GetChartMoviesMostAnticipated
      x-api-path-slug: chartsmoviesmostanticipated-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - Charts
      - Movies
      - MostAnticipated
  /Charts/Movies/Popular:
    get:
      summary: Returns list of popular movies.
      description: Requires Skip and Take. Maximum page size is 100.
      operationId: GetChartMoviesPopular
      x-api-path-slug: chartsmoviespopular-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - Charts
      - Movies
      - Popular
  /Charts/People/Popular:
    get:
      summary: Returns list of popular celebrities based on IVA data.
      description: Requires Skip and Take. Maximum page size is 100.
      operationId: GetChartPeoplePopular
      x-api-path-slug: chartspeoplepopular-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - Charts
      - People
      - Popular
  /Charts/Shows/Popular:
    get:
      summary: Returns a list of shows based on popularity.
      description: Requires Skip and Take. Maximum page size is 100.
      operationId: GetChartShowsPopular
      x-api-path-slug: chartsshowspopular-get
      parameters:
      - in: query
        name: Skip
        description: Skips records using for paging results
      - in: query
        name: Take
        description: Limits the total items returned
      responses:
        200:
          description: OK
      tags:
      - Charts
      - Shows
      - Popular
  /Common/Companies/:
    get:
      summary: Paged list of companies.
      description: 'Companies are listed in a movie, show, or game response as those
        whom are involved with the program.  EX: Universal Pictures.'
      operationId: GetCompanies
      x-api-path-slug: commoncompanies-get
      parameters:
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Common
      - Companies
  /Common/Countries/:
    get:
      summary: Returns a list of countries.
      description: List of Countries, ISO codes and Country IDs used throughout the
        API.
      operationId: GetCountries
      x-api-path-slug: commoncountries-get
      responses:
        200:
          description: OK
      tags:
      - Common
      - Countries
  /Common/ImageTypes/:
    get:
      summary: List of image types contained in the database.
      description: 'A list of image types available in the IVA database. **EX: Poster**'
      operationId: GetImageTypes
      x-api-path-slug: commonimagetypes-get
      responses:
        200:
          description: OK
      tags:
      - Common
      - ImageTypes
  /Common/Languages/:
    get:
      summary: Gets all languages.
      description: Returns a list of languages used in the API as well as the ISO
        code and language ID.
      operationId: GetLanguages
      x-api-path-slug: commonlanguages-get
      responses:
        200:
          description: OK
      tags:
      - Common
      - Languages
  /Common/Tags/:
    get:
      summary: Gets all tags.
      description: Paged list of all tags used in the API.
      operationId: GetTags
      x-api-path-slug: commontags-get
      parameters:
      - in: query
        name: Skip
        description: Offset for paging
      - in: query
        name: Take
        description: Maximum number of rows returned
      responses:
        200:
          description: OK
      tags:
      - Common
      - Tags
  /Common/VideoTypes/:
    get:
      summary: Gets all VideoTypes.
      description: Returns a list of the types of videos that can be associated to
        a title.
      operationId: GetVideoTypes
      x-api-path-slug: commonvideotypes-get
      responses:
        200:
          description: OK
      tags:
      - Common
      - VideoTypes
  /ExternalIds/GracenoteMovie:
    get:
      summary: Returns list of all MovieId, Gracenote Id pairs.
      description: Not accessible with a Demo account.  **Special permissions needed**
        for access to this operation.  Contact [Sales](mailto:sales@internetvideoarchive.com).
      operationId: GetGracenoteMovieIds
      x-api-path-slug: externalidsgracenotemovie-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - GracenoteMovie
  /ExternalIds/GracenoteShow:
    get:
      summary: Returns list of all ShowId, Gracenote Id pairs.
      description: Not accessible with a Demo account. **Special permissions needed**
        for access to this operation. Contact [Sales](mailto:sales@internetvideoarchive.com).
      operationId: GetGracenoteShowIds
      x-api-path-slug: externalidsgracenoteshow-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - GracenoteShow
  /ExternalIds/ImdbMovie:
    get:
      summary: Returns list of all MovieId, IMDB Id pairs.
      description: Ingest this ID map to create connections between the objects in
        your existing database with an IMDB ID to the IVA Movie objects.
      operationId: GetImdbMovieIds
      x-api-path-slug: externalidsimdbmovie-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - ImdbMovie
  /ExternalIds/ImdbShow:
    get:
      summary: Returns list of all MovieId, Tmdb Id pairs.
      description: ngest this ID map to create connections between the objects in
        your existing database with an IMDB ID to the IVA Show objects.
      operationId: GetImdbShowIds
      x-api-path-slug: externalidsimdbshow-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - ImdbShow
  /ExternalIds/RoviMovie:
    get:
      summary: Returns list of all MovieId, Tivo Id pairs.
      description: Not accessible with a Demo account. **Special permissions needed**
        for access to this operation. Contact [Sales](mailto:sales@internetvideoarchive.com).
      operationId: GetTivoMovieIds
      x-api-path-slug: externalidsrovimovie-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - RoviMovie
  /ExternalIds/RoviShow:
    get:
      summary: Returns list of all ShowId, Tivo Id pairs.
      description: Not accessible with a Demo account. **Special permissions needed**
        for access to this operation. Contact [Sales](mailto:sales@internetvideoarchive.com).
      operationId: GetTivoShowIds
      x-api-path-slug: externalidsrovishow-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - RoviShow
  /ExternalIds/TmdbMovie:
    get:
      summary: Returns list of all MovieId, Tmdb Id pairs.
      description: Use to link a TMDB ID to an IVA Movie ID.
      operationId: GetTmdbMovieIds
      x-api-path-slug: externalidstmdbmovie-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - TmdbMovie
  /ExternalIds/TmdbShow:
    get:
      summary: Returns list of all ShowId, TMDB Id pairs.
      description: Use to link a TMDB ID to an IVA Show ID.
      operationId: GetTmdbShowIds
      x-api-path-slug: externalidstmdbshow-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - TmdbShow
  /ExternalIds/Webedia:
    get:
      summary: Returns list of all MovieId, Webedia Id pairs.
      description: Not accessible with a Demo account. **Special permissions needed**
        for access to this operation. Contact [Sales](mailto:sales@internetvideoarchive.com).
      operationId: GetWebediaMovieIds
      x-api-path-slug: externalidswebedia-get
      parameters:
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - ExternalIds
      - Webedia
  /Find/Movie/:
    get:
      summary: Find a movie using third party ID.
      description: "Use FindMovie with a third party ID like IMDB, TMDB, Gracenote,
        Tivo, etc. to find the corresponding movie in the IVA database.  For a full
        list of supported ID types see /Movies/AlternateIdTypes. \n\n\n\n`Recommendation:
        Use with small data sets or for a proof of concept. `"
      operationId: FindMovie
      x-api-path-slug: findmovie-get
      parameters:
      - in: query
        name: Id
        description: Required third party ID of Movie
      - in: query
        name: IdType
        description: Required third party ID type of MovieAlternateId
      - in: query
        name: Includes
        description: List of additional objects to include in the movie object
      responses:
        200:
          description: OK
      tags:
      - Find
      - Movie
  /Find/Show/:
    get:
      summary: Find a TV show using a third party ID.
      description: 'Use FindShow with a third party ID like IMDB, TMDB, Gracenote,
        Tivo, etc. to find the corresponding TV show in the IVA database. For a full
        list of supported ID types see /Shows/AlternateIdTypes. `Recommendation: Use
        with small data sets or for a proof of concept. `'
      operationId: FindShow
      x-api-path-slug: findshow-get
      parameters:
      - in: query
        name: Id
        description: Required third party ID of Show
      - in: query
        name: IdType
        description: Required third party ID type of ShowAlternateId
      - in: query
        name: Includes
        description: List of additional objects to include in the show response
      responses:
        200:
          description: OK
      tags:
      - Find
      - Show
  /GoWatchIt/Episodes/{Id}/Availabilities:
    get:
      summary: Get GoWatchIt Episode Availability.
      description: Returns GoWatchit episode availability by Entertainment Episode
        ID. Special permission is required to access this endpoint.
      operationId: GetGoWatchItEpisodeAvailabilities
      x-api-path-slug: gowatchitepisodesidavailabilities-get
      parameters:
      - in: query
        name: ApiKey
        description: Required GoWatchIt API key
      - in: path
        name: Id
        description: Required ID of Entertainment Episode
      responses:
        200:
          description: OK
      tags:
      - GoWatchIt
      - Episodes
      - Id
      - Availabilities
  /GoWatchIt/Movies/{Id}/Availabilities:
    get:
      summary: Get GoWatchIt Movie Availability.
      description: Returns GoWatchIt movie availability by Entertainment Movie ID.  Special
        permission is required to access this endpoint.  Contact [Sales](mailto:Sales@InternetVideoArchive.com)
        for more information.
      operationId: GetGoWatchItMovieAvailabilities
      x-api-path-slug: gowatchitmoviesidavailabilities-get
      parameters:
      - in: query
        name: ApiKey
        description: Required GoWatchIt API key
      - in: path
        name: Id
        description: Required ID of Entertainment Movie
      responses:
        200:
          description: OK
      tags:
      - GoWatchIt
      - Movies
      - Id
      - Availabilities
  /GoWatchIt/Seasons/{Id}/Availabilities:
    get:
      summary: Get GoWatchIt Season Availability.
      description: Returns GoWatchIt season availability by Entertainment Season ID.  Special
        permission is required to access this endpoint.  Contact [Sales](mailto:Sales@InternetVideoArchive.com)
        for more information.
      operationId: GetGoWatchItSeasonAvailabilities
      x-api-path-slug: gowatchitseasonsidavailabilities-get
      parameters:
      - in: query
        name: ApiKey
        description: Required GoWatchIt API key
      - in: path
        name: Id
        description: Required ID of Entertainment Season
      responses:
        200:
          description: OK
      tags:
      - GoWatchIt
      - Seasons
      - Id
      - Availabilities
  /GoWatchIt/Shows/{Id}/Availabilities:
    get:
      summary: Get GoWatchItShow Availability.
      description: Returns GoWatchIt show availability by Entertainment Show ID.  Special
        permission is required to access this endpoint. Please contact [Sales](mailto:Sales@InternetVideoArchive.com)
        for more information.
      operationId: GetGoWatchItShowAvailabilities
      x-api-path-slug: gowatchitshowsidavailabilities-get
      parameters:
      - in: query
        name: ApiKey
        description: Required GoWatchIt API key
      - in: path
        name: Id
        description: Required ID of Entertainment Show
      responses:
        200:
          description: OK
      tags:
      - GoWatchIt
      - Shows
      - Id
      - Availabilities
  /Images/Batch:
    post:
      summary: Returns a list of batch image responses links based on filepath.
      description: Requires a list filepath.
      operationId: GetImageBatch
      x-api-path-slug: imagesbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: FilePath
        description: List of Filepaths
      responses:
        200:
          description: OK
      tags:
      - Images
      - Batch
  /Images/ScreenCaptures/Batch:
    post:
      summary: Returns a list of screen capture responses.
      description: Requires a list of filepaths.
      operationId: GetScreenCaptureBatch
      x-api-path-slug: imagesscreencapturesbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: FilePath
        description: List of Filepaths
      responses:
        200:
          description: OK
      tags:
      - Images
      - ScreenCaptures
      - Batch
  /Images/ScreenCaptures/Redirect:
    get:
      summary: Redirect to a screen capture based on filepath.
      description: "Requires a valid filepath of a video asset screen capture.  \n\n`Note:
        The swagger U/I does not support redirects.`"
      operationId: GetScreenCapture
      x-api-path-slug: imagesscreencapturesredirect-get
      parameters:
      - in: query
        name: FilePath
        description: Filepath of Image
      - in: query
        name: Redirect
        description: Redirect to the image
      responses:
        200:
          description: OK
      tags:
      - Images
      - ScreenCaptures
      - Redirect
  /Images/{FilePath}/Redirect:
    get:
      summary: Redirect to an image based on filepath.
      description: "Images should be downloaded and stored on the client server. Use
        /Common/ImageTypes to see a list of available image types.  \n\n\n`Note: The
        swagger U/I does not support redirects.`"
      operationId: GetImage
      x-api-path-slug: imagesfilepathredirect-get
      parameters:
      - in: path
        name: FilePath
        description: Filepath of Image
      - in: query
        name: Redirect
        description: Redirect to the image
      responses:
        200:
          description: OK
      tags:
      - Images
      - FilePath
      - Redirect
  /Metacritic/Movie/{Id}:
    get:
      summary: Get Metacritic Movie information.
      description: Returns Metacritic Movie information by Entertainment Movie ID.
      operationId: GetMetacriticMovie
      x-api-path-slug: metacriticmovieid-get
      parameters:
      - in: path
        name: Id
        description: Required ID of Entertainment Movie
      responses:
        200:
          description: OK
      tags:
      - Metacritic
      - Movie
      - Id
  /Metacritic/TV/{Id}:
    get:
      summary: Get Metacritic TV information.
      description: Returns Metacritic TV information by Entertainment Show ID.
      operationId: GetMetacriticTv
      x-api-path-slug: metacritictvid-get
      parameters:
      - in: path
        name: Id
        description: Required ID of Entertainment Show
      - in: query
        name: SeasonNumber
        description: Number of season
      responses:
        200:
          description: OK
      tags:
      - Metacritic
      - TV
      - Id
  /MovieTickets/Cultures:
    get:
      summary: Get MovieTickets Cultures.
      description: Returns MovieTickets Cultures.
      operationId: GetMovieTicketsCultures
      x-api-path-slug: movieticketscultures-get
      responses:
        200:
          description: OK
      tags:
      - MovieTickets
      - Cultures
  /MovieTickets/Movies/ComingSoon:
    get:
      summary: Get MovieTickets Movies releasing soon.
      description: Returns MovieTickets Movies releasing soon.
      operationId: GetMovieTicketsMoviesComingSoon
      x-api-path-slug: movieticketsmoviescomingsoon-get
      parameters:
      - in: query
        name: Culture
        description: Culture to retrieve response
      - in: query
        name: PageNumber
        description: Page number for paging results
      - in: query
        name: PageSize
        description: Limits the total items returned
      responses:
        200:
          description: OK
      tags:
      - MovieTickets
      - Movies
      - ComingSoon
  /MovieTickets/Movies/NowPlaying:
    get:
      summary: Get MovieTickets Movies in theaters.
      description: Returns MovieTickets Movies currently in theaters.
      operationId: GetMovieTicketsMoviesNowPlaying
      x-api-path-slug: movieticketsmoviesnowplaying-get
      parameters:
      - in: query
        name: Culture
        description: Culture to retrieve response
      - in: query
        name: PageNumber
        description: Page number for paging results
      - in: query
        name: PageSize
        description: Limits the total items returned
      responses:
        200:
          description: OK
      tags:
      - MovieTickets
      - Movies
      - NowPlaying
  /MovieTickets/Performances:
    get:
      summary: Get MovieTickets Performances.
      description: Returns MovieTickets Performances by MovieTickets Theater ID, Entertainment
        Movie ID, and ScheduleDate.
      operationId: GetMovieTicketsPerformances
      x-api-path-slug: movieticketsperformances-get
      parameters:
      - in: query
        name: Culture
        description: Culture to retrieve response
      - in: query
        name: EntertainmentMovieIds
        description: Required ID/IDs of Entertainment Movies
      - in: query
        name: ScheduleDate
        description: Date to get scheduled performances
      - in: query
        name: TheaterIds
        description: Required ID/IDs of MovieTickets Theaters
      responses:
        200:
          description: OK
      tags:
      - MovieTickets
      - Performances
  /MovieTickets/Theaters:
    get:
      summary: Get MovieTickets Theaters.
      description: Returns MovieTickets Theaters by postal code.
      operationId: GetMovieTicketsTheaters
      x-api-path-slug: movieticketstheaters-get
      parameters:
      - in: query
        name: Culture
        description: Culture to retrieve response
      - in: query
        name: Distance
        description: Required distaince in meters
      - in: query
        name: Latitude
        description: Latitude coordinate
      - in: query
        name: Longitude
        description: Longitude coordinate
      - in: query
        name: PageNumber
        description: Page number for paging results
      - in: query
        name: PageSize
        description: Limits the total items returned
      - in: query
        name: PostalCode
        description: Postal code
      responses:
        200:
          description: OK
      tags:
      - MovieTickets
      - Theaters
  /Movies/All:
    get:
      summary: Returns a paged list of all movies.
      description: "By default the API will only return basic title information. Additional
        objects can be included by passing the object in the Includes parameter.   \n\n\n`Subscriptions
        with \"Limited\" data will only be able to include basic title information
        and Videos.`"
      operationId: GetAllMovies
      x-api-path-slug: moviesall-get
      parameters:
      - in: query
        name: Includes
        description: List of additional objects to include in the movie objectSearch
          movie by OriginalTitle
      - in: query
        name: Skip
        description: Skips records using for paging results
      - in: query
        name: Take
        description: Limits the total items returned
      responses:
        200:
          description: OK
      tags:
      - Movies
  /Movies/AlternateIdTypes:
    get:
      summary: Returns all MovieAlternateIdTypes.
      description: "Movie alternate ID types refer to 3rd party IDs that IVA matches
        its own movie IDs.  **EX: IMDB, TMDB**.  \n\n`Use to get the Id of the ID
        type to use with /Find/Movie.`"
      operationId: GetMovieAlternateIdTypes
      x-api-path-slug: moviesalternateidtypes-get
      responses:
        200:
          description: OK
      tags:
      - Movies
      - AlternateIdTypes
  /Movies/ComingSoon/:
    get:
      summary: Returns list of all Movies coming to US Theaters.
      description: |-
        Requires Skip and Take. Maximum page size is 10.

        By default the API will only return basic title information.
        Additional objects can be included by passing the object in the Includes parameter in a comma separated list.
      operationId: GetMoviesComingSoon
      x-api-path-slug: moviescomingsoon-get
      parameters:
      - in: query
        name: Includes
        description: List of additional objects to include in the movie response
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - Movies
      - ComingSoon
  /Movies/InTheaters/:
    get:
      summary: Returns list of all Movies currently in US Theaters.
      description: |-
        Requires Skip and Take. Maximum page size is 10.

        By default the API will only return basic title information.
        Additional objects can be included by passing the object in the Includes parameter in a comma separated list.
      operationId: GetMoviesInTheaters
      x-api-path-slug: moviesintheaters-get
      parameters:
      - in: query
        name: Includes
        description: List of additional objects to include in the movie response
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - Movies
      - InTheaters
  /Movies/Match/:
    get:
      summary: Perform a match to Entertainment using Title, Year, Cast and Director.
        Returns best match and score for the match.
      description: Use to match IVA movie data to another data source using title,
        year, cast etc.
      operationId: MatchToMovie
      x-api-path-slug: moviesmatch-get
      parameters:
      - in: query
        name: AlternateTitles
        description: Alternate Titles of movie to be matched
      - in: query
        name: Cast
        description: Cast members of movie to be matched
      - in: query
        name: Directors
        description: Directors of movie to be matched
      - in: query
        name: StringDistance
        description: For fuzzy title match, default is 4, set to 0 for no fuzzy match
      - in: query
        name: Title
        description: Title of movie to be matched
      - in: query
        name: Year
        description: Release Year of movie to be matched
      responses:
        200:
          description: OK
      tags:
      - Movies
      - Match
  /Movies/MovieCertifications:
    get:
      summary: Returns all Movie Certifications
      description: Returns all Movie Certifications used in a movie response with
        the Releases object.
      operationId: GetMovieCertifications
      x-api-path-slug: moviesmoviecertifications-get
      responses:
        200:
          description: OK
      tags:
      - Movies
      - MovieCertifications
  /Movies/MovieGenres:
    get:
      summary: Returns all Movie Genres.
      description: List of all movie genres used in the API.
      operationId: GetMovieGenres
      x-api-path-slug: moviesmoviegenres-get
      responses:
        200:
          description: OK
      tags:
      - Movies
      - MovieGenres
  /Movies/ReleaseTypes:
    get:
      summary: Returns all Movie ReleaseTypes
      description: 'Release type refers to the release. **EX: Theatrical, Home Video,
        etc.**'
      operationId: GetMovieReleaseTypes
      x-api-path-slug: moviesreleasetypes-get
      responses:
        200:
          description: OK
      tags:
      - Movies
      - ReleaseTypes
  /Movies/SearchAndDiscover:
    get:
      summary: Search and discover movies.
      description: |-
        Searchable Fields:
        Title, AlternateTitles, Genres, OriginalReleaseDate, UnitedStatesReleaseDate, GermanyReleaseDate, FranceReleaseDate, UnitedKingdomReleaseDate, ItalyReleaseDate, JapanReleaseDate, Tags, Cast, Directors, Descriptions, Ratings, OriginalLanguage.
        [Syntax Ref](https://docs.microsoft.com/en-us/rest/api/searchservice/simple-query-syntax-in-azure-search)

        Filterable Fields:
        ID, Title, AlternateTitles, Genres, OriginalReleaseDate, UnitedStatesReleaseDate, GermanyReleaseDate, FranceReleaseDate, UnitedKingdomReleaseDate, ItalyReleaseDate, JapanReleaseDate, Year, Tags, Cast, Directors, Descriptions, HasVideo, PosterFilePath, Ratings, OriginalLanguage, Runtime, Budget, Revenue, Created, Modified.
        [Syntax Ref](https://docs.microsoft.com/en-us/rest/api/searchservice/odata-expression-syntax-for-azure-search)
      operationId: SearchAndDiscoverMovie
      x-api-path-slug: moviessearchanddiscover-get
      parameters:
      - in: query
        name: Filter
        description: Expression to filter results
      - in: query
        name: IncludeTotalResultCount
        description: Includes total results in response
      - in: query
        name: OrderBy
        description: List of field names to sort results
      - in: query
        name: SearchFields
        description: List of field names to search using term
      - in: query
        name: SearchMode
        description: Specifies whether ANY or ALL of the search terms must be matched
          in order to count the item as a match
      - in: query
        name: SelectFields
        description: List of field names to be returned in the object
      - in: query
        name: Skip
        description: Skip number of results
      - in: query
        name: term
        description: Term to search for
      - in: query
        name: Top
        description: Limit results
      responses:
        200:
          description: OK
      tags:
      - Movies
      - SearchAndDiscover
  /Movies/{Id}:
    get:
      summary: Returns movie data for a specific IVA MovieId.
      description: "By default the API will only return basic title information. Additional
        objects can be included by passing the object in the Includes parameter.   \n\n\n`Subscriptions
        with \"Limited\" data will only be able to include basic title information
        and Videos.`"
      operationId: GetMovie
      x-api-path-slug: moviesid-get
      parameters:
      - in: path
        name: Id
        description: Required ID of Movie
      - in: query
        name: Includes
        description: List of additional objects to include in the movie response
      responses:
        200:
          description: OK
      tags:
      - Movies
      - Id
  /People/All:
    get:
      summary: Gets all People.
      description: Returns a AllPeopleResponse object containing a list of all poeple.
      operationId: GetAllPeople
      x-api-path-slug: peopleall-get
      parameters:
      - in: query
        name: Includes
        description: List of additional objects to include in the person response
      - in: query
        name: Skip
        description: Skips records using for paging results
      - in: query
        name: Take
        description: Limits the total items returned
      responses:
        200:
          description: OK
      tags:
      - People
  /People/RankedSearch/:
    get:
      summary: Find Person by Name ordered by rank.
      description: Find person using name ordered by rank.
      operationId: GetPersonRankedSearch
      x-api-path-slug: peoplerankedsearch-get
      parameters:
      - in: query
        name: StartsWith
      responses:
        200:
          description: OK
      tags:
      - People
      - RankedSearch
  /People/{Id}:
    get:
      summary: Returns information on a person.
      description: BETA - By default the API will only return basic People information.
        Additional objects can be included by passing the object in the Includes parameter.
      operationId: GetPerson
      x-api-path-slug: peopleid-get
      parameters:
      - in: path
        name: Id
        description: Required ID of Person
      - in: query
        name: Includes
        description: List of additional objects to include in the person response
      responses:
        200:
          description: OK
      tags:
      - People
      - Id
  /People/{Id}/Filmography:
    get:
      summary: Get a Person's Filmography.
      description: Requires a valid Person ID.
      operationId: GetFilmography
      x-api-path-slug: peopleidfilmography-get
      parameters:
      - in: path
        name: Id
      responses:
        200:
          description: OK
      tags:
      - People
      - Id
      - Filmography
  /SDKs/{Client}:
    get:
      summary: Returns a zip file of client SDK.
      description: Generate and download SDK's for using the API.  Requires a subscription
        key for authorization and a valid client.
      operationId: GetSDK
      x-api-path-slug: sdksclient-get
      parameters:
      - in: path
        name: Client
        description: Client SDK
      - in: query
        name: RedirectToFile
        description: Redirect to download the zipped SDK
      responses:
        200:
          description: OK
      tags:
      - SDKs
      - Client
  /Shows/All:
    get:
      summary: Returns a paged list of all TV shows.
      description: "By default the API will only return basic title information. Additional
        objects can be included by passing the object in the Includes parameter. \n\n\n`Subscriptions
        with \"Limited\" data will only be able to include basic title information,
        Videos, EpisodicVideos, and SeasonVideos.`"
      operationId: GetAllShows
      x-api-path-slug: showsall-get
      parameters:
      - in: query
        name: Includes
        description: List of additional objects to include in the show object
      - in: query
        name: Skip
        description: Skips records using for paging results
      - in: query
        name: Take
        description: Limits the total items returned
      responses:
        200:
          description: OK
      tags:
      - Shows
  /Shows/AlternateIdTypes:
    get:
      summary: Get all AlternateIdTypes.
      description: 'Alternate Id types refer to the 3rd party ID sets IVA data has
        matched.  **Ex: IMDB**'
      operationId: GetShowAlternateIdTypes
      x-api-path-slug: showsalternateidtypes-get
      responses:
        200:
          description: OK
      tags:
      - Shows
      - AlternateIdTypes
  /Shows/Match/:
    get:
      summary: Perform a match to Entertainment using Title, Year, Cast and Director.
        Returns best match and score for the match.
      description: Use to match IVA show data to another data source using title,
        director, cast, etc.
      operationId: MatchToShow
      x-api-path-slug: showsmatch-get
      parameters:
      - in: query
        name: AlternateTitles
        description: Alternate Titles of Show to be matched
      - in: query
        name: Cast
        description: Cast members of Show to be matched
      - in: query
        name: Directors
        description: Directors of Show to be matched
      - in: query
        name: StringDistance
        description: For fuzzy title match, default is 4, set to 0 for no fuzzy match
      - in: query
        name: Title
        description: Title of Show to be matched
      - in: query
        name: Year
        description: Release Year of Show to be matched
      responses:
        200:
          description: OK
      tags:
      - Shows
      - Match
  /Shows/ReleaseTypes:
    get:
      summary: Returns a list of Show Release Types.
      description: Release types refer to the type of release and are used in the
        releases object for a show.
      operationId: GetShowReleaseTypes
      x-api-path-slug: showsreleasetypes-get
      responses:
        200:
          description: OK
      tags:
      - Shows
      - ReleaseTypes
  /Shows/SearchAndDiscover:
    get:
      summary: Search and discover shows.
      description: |-
        Searchable Fields: Title, AlternateTitles, Genres, Tags, Cast, Directors, Descriptions, Ratings, OriginalLanguage. [Syntax Ref](https://docs.microsoft.com/en-us/rest/api/searchservice/simple-query-syntax-in-azure-search)

        Filterable Fields: Id, Title, AlternateTitles, Genres, OriginalAirDate, Year, Tags, Cast, Directors, Descriptions, HasVideo, ImageFilePath, Ratings, OriginalLanguage, Created, Modified, NumberOfSeasons, NumberOfEpisodes. [Syntax Ref](https://docs.microsoft.com/en-us/rest/api/searchservice/simple-query-syntax-in-azure-search)
      operationId: SearchAndDiscoverShow
      x-api-path-slug: showssearchanddiscover-get
      parameters:
      - in: query
        name: Filter
        description: Expression to filter results
      - in: query
        name: IncludeTotalResultCount
        description: Includes total results in response
      - in: query
        name: OrderBy
        description: List of field names to sort results
      - in: query
        name: SearchFields
        description: List of field names to search using term
      - in: query
        name: SearchMode
        description: Specifies whether ANY or ALL of the search terms must be matched
          in order to count the item as a match
      - in: query
        name: SelectFields
        description: List of field names to be returned in the object
      - in: query
        name: Skip
        description: Skip number of results
      - in: query
        name: term
        description: Term to search for
      - in: query
        name: Top
        description: Limit results
      responses:
        200:
          description: OK
      tags:
      - Shows
      - SearchAndDiscover
  /Shows/Season/:
    get:
      summary: Get Season by ShowId and Season Number.
      description: Use the IVA ShowId and a season number to get a season details
        and video asset data.
      operationId: GetSeasonByNumber
      x-api-path-slug: showsseason-get
      parameters:
      - in: query
        name: Id
        description: Id of a Show
      - in: query
        name: SeasonNumber
        description: Number of a Season belonging to a Show
      responses:
        200:
          description: OK
      tags:
      - Shows
      - Season
  /Shows/Seasons/Episode/:
    get:
      summary: Get Episode by ShowId, Season Number and Episode Number.
      description: Some use cases find it useful to be able to pass a season number
        and episode number of a known show to get the data for that exact episode.
      operationId: GetEpisodeByNumber
      x-api-path-slug: showsseasonsepisode-get
      parameters:
      - in: query
        name: EpisodeNumber
        description: Required EpisodeNumber
      - in: query
        name: Id
        description: Required Id of the Show
      - in: query
        name: SeasonNumber
        description: Required SeasonNumber
      responses:
        200:
          description: OK
      tags:
      - Shows
      - Seasons
      - Episode
  /Shows/Seasons/Episodes/{Id}:
    get:
      summary: Returns an Episode object for a requested Episode ID.
      description: Returns the episode details for a specific episode ID.
      operationId: GetEpisode
      x-api-path-slug: showsseasonsepisodesid-get
      parameters:
      - in: path
        name: Id
        description: Required ID of an Episode
      - in: query
        name: Includes
        description: List of additional objects to include in the episode response
      responses:
        200:
          description: OK
      tags:
      - Shows
      - Seasons
      - Episodes
      - Id
  /Shows/Seasons/{Id}:
    get:
      summary: Get Season by SeasonId.
      description: Use with a SeasonId to return details for a season including any
        video asset data.
      operationId: GetSeason
      x-api-path-slug: showsseasonsid-get
      parameters:
      - in: path
        name: Id
        description: Id of a Season
      - in: query
        name: Includes
        description: List of additional objects to include in the season response
      responses:
        200:
          description: OK
      tags:
      - Shows
      - Seasons
      - Id
  /Shows/ShowCertifications:
    get:
      summary: Returns a list of Show Certifications.
      description: List of Show Certifications and definitions.
      operationId: GetShowCertifications
      x-api-path-slug: showsshowcertifications-get
      responses:
        200:
          description: OK
      tags:
      - Shows
      - ShowCertifications
  /Shows/ShowGenres:
    get:
      summary: Get all Show Genres.
      description: Returns a list of all the show genres used in the IVA database.
      operationId: GetShowGenres
      x-api-path-slug: showsshowgenres-get
      responses:
        200:
          description: OK
      tags:
      - Shows
      - ShowGenres
  /Shows/{Id}:
    get:
      summary: Get Show by Show ID.
      description: "By default the API will only return basic title information. Additional
        objects can be included by passing the object in the Includes parameter.  \n\n\n`Subscriptions
        with \"Limited\" data will only be able to include basic title information,
        Videos, EpisodicVideos, and SeasonVideos.`"
      operationId: GetShow
      x-api-path-slug: showsid-get
      parameters:
      - in: path
        name: Id
        description: Required ID of Show
      - in: query
        name: Includes
        description: List of additional objects to include in the show response
      responses:
        200:
          description: OK
      tags:
      - Shows
      - Id
  /Shows/{Id}/Seasons/{SeasonNumber}:
    get:
      summary: Get Season by ShowId and Season Number.
      description: Depreciated. Use GetSeasonBySeasonNumber instead.  Requires a valid
        ShowId and Season Number.
      operationId: GetSeasonBySeasonNumber
      x-api-path-slug: showsidseasonsseasonnumber-get
      parameters:
      - in: path
        name: Id
        description: Id of a Show
      - in: query
        name: Includes
        description: List of additional objects to include in the season response
      - in: path
        name: SeasonNumber
        description: Number of a Season belonging to a Show
      responses:
        200:
          description: OK
      tags:
      - Shows
      - Id
      - Seasons
      - SeasonNumber
  /Shows/{Id}/Seasons/{SeasonNumber}/Episodes/{EpisodeNumber}:
    get:
      summary: Get Episode by ShowId, Season Number and Episode Number.
      description: Requires a valid ShowId, Season Number and Episode Number.
      operationId: GetEpisodeByEpisodeNumber
      x-api-path-slug: showsidseasonsseasonnumberepisodesepisodenumber-get
      parameters:
      - in: path
        name: EpisodeNumber
        description: Required EpisodeNumber
      - in: path
        name: Id
        description: Required Id of the Show
      - in: query
        name: Includes
        description: List of additional objects to include in the episode response
      - in: path
        name: SeasonNumber
        description: Required SeasonNumber
      responses:
        200:
          description: OK
      tags:
      - Shows
      - Id
      - Seasons
      - SeasonNumber
      - Episodes
      - EpisodeNumber
  /Tests/TestDateTime/:
    get:
      summary: Returns translated time from IVA or an error if invalid.
      description: Entertainment Express APIs use date time format ISO 8601.  Use
        this API to test your date time format to see if it translates to a valid
        time on our server.
      operationId: GetTestDateTime
      x-api-path-slug: teststestdatetime-get
      parameters:
      - in: query
        name: DateTime
        description: DateTime to test format from API
      responses:
        200:
          description: OK
      tags:
      - Tests
      - TestDateTime
  /TheatricalMovies/:
    get:
      summary: Returns list of all US Theatrical Movie objects.
      description: 'Deprecated. Use /Movies/InTheaters or /Movies/ComingSoon instead.
        Returns all movies with a US Theatrical Release Date > today - 60 days.  Use
        the includes parameter to include additional objects related to the movie.  The
        includes parameter takes a comma separated list of objects.  **EX: Genres,Descriptions,Videos**'
      operationId: GetTheatricalMovies
      x-api-path-slug: theatricalmovies-get
      parameters:
      - in: query
        name: Includes
        description: List of additional objects to include in the movie response
      - in: query
        name: Skip
        description: Determines where to start page
      - in: query
        name: Take
        description: Determines the page size
      responses:
        200:
          description: OK
      tags:
      - TheatricalMovies
  /TvMedia/genres/movies:
    get:
      summary: ""
      description: Gets list of movie genres.
      operationId: GetTvMediaMovieGenres
      x-api-path-slug: tvmediagenresmovies-get
      parameters:
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Genres
      - Movies
  /TvMedia/genres/shows:
    get:
      summary: ""
      description: Gets list of show genres.
      operationId: GetTvMediaShowGenres
      x-api-path-slug: tvmediagenresshows-get
      parameters:
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Genres
      - Shows
  /TvMedia/genres/sports:
    get:
      summary: ""
      description: Gets list of sports genres.
      operationId: GetTvMediaSportGenres
      x-api-path-slug: tvmediagenressports-get
      parameters:
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Genres
      - Sports
  /TvMedia/leagues:
    get:
      summary: ""
      description: Gets list of sports leagues.
      operationId: GetTvMediaLeagues
      x-api-path-slug: tvmedialeagues-get
      parameters:
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Leagues
  /TvMedia/leagues/{LeagueID}/listings:
    get:
      summary: ""
      description: Retrieve listings for a given leagueID.
      operationId: GetTvMediaLeagueListings
      x-api-path-slug: tvmedialeaguesleagueidlistings-get
      parameters:
      - in: query
        name: AdultContent
        description: Defaults to 1 (allowed)
      - in: query
        name: Channel
        description: Include only channel(s) with this number, single or array values
          accepted
      - in: query
        name: DescriptiveVideoOnly
        description: Only displays listings which are flagged as being broadcast with
          Descriptive Video
      - in: query
        name: Detail
        description: Set level of detail for response
      - in: query
        name: DisplayArtwork
        description: Displays the Artwork information
      - in: query
        name: End
        description: UTC end time in ISO8601
      - in: query
        name: EndChan
        description: Highest channel
      - in: query
        name: ExcludeChan
        description: Exclude channels by number, single or array values accepted
      - in: query
        name: ExcludeShowType
        description: Exclude only these show type ID(s), array or single values accepted
      - in: query
        name: ExcludeStation
        description: Filter out station IDs; array or single value accepted
      - in: query
        name: Id
        description: ListingID, array or single values accepted
      - in: query
        name: League
        description: Get only sports listings in the given league ID(s)
      - in: path
        name: LeagueID
        description: League ID
      - in: query
        name: LineupID
        description: Lineup ID
      - in: query
        name: LiveOnly
        description: Only displays live listings
      - in: query
        name: NewShowsOnly
        description: Get new shows only
      - in: query
        name: NotYetStarted
        description: Only displays listings which are starting on or after the given
          start time
      - in: query
        name: Search
        description: 'search value: can be a show, episode, movie, team, league, person,
          etc'
      - in: query
        name: ShowType
        description: Include only these show type ID(s), array or single values accepted
      - in: query
        name: SportEventsOnly
        description: Get sporting events only
      - in: query
        name: SportType
        description: Get only sports listings of type sportTypeID
      - in: query
        name: Start
        description: UTC start time in ISO8601
      - in: query
        name: StartChan
        description: Lowest channel
      - in: query
        name: Station
        description: Filter by station ID
      - in: query
        name: Team
        description: Filter by teams playing by name(teams
      - in: query
        name: TimeZone
        description: Set a timezone or time offset for listing times (listDateTime
          property)
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Leagues
      - LeagueID
      - Listings
  /TvMedia/leagues/{LeagueID}/teams:
    get:
      summary: ""
      description: Gets list of teams in a league.
      operationId: GetTvMediaTeams
      x-api-path-slug: tvmedialeaguesleagueidteams-get
      parameters:
      - in: path
        name: LeagueID
        description: League ID
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Leagues
      - LeagueID
      - Teams
  /TvMedia/lineups:
    get:
      summary: ""
      description: Get lineups by postal code.
      operationId: GetTvMediaLineupsByPostalCode
      x-api-path-slug: tvmedialineups-get
      parameters:
      - in: query
        name: Detail
        description: Set level of detail for response
      - in: query
        name: LineupType
        description: Filter by lineup type, valid types are OTA, SAT, CAB, IPTV
      - in: query
        name: PostalCode
        description: Postal code
      - in: query
        name: ProviderId
        description: Filter by provider ID
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Lineups
  /TvMedia/lineups/browse:
    get:
      summary: ""
      description: Starting point for lineup browser, returns available countries.
      operationId: GetTvMediaCountries
      x-api-path-slug: tvmedialineupsbrowse-get
      parameters:
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Lineups
      - Browse
  /TvMedia/lineups/browse/{CountryID}:
    get:
      summary: ""
      description: Browse regions by country.
      operationId: GetTvMediaRegions
      x-api-path-slug: tvmedialineupsbrowsecountryid-get
      parameters:
      - in: path
        name: CountryID
        description: Country abbreviation
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Lineups
      - Browse
      - CountryID
  /TvMedia/lineups/browse/{CountryID}/{RegionID}:
    get:
      summary: ""
      description: Get service areas for a specific country and region.
      operationId: GetTvMediaServiceAreas
      x-api-path-slug: tvmedialineupsbrowsecountryidregionid-get
      parameters:
      - in: path
        name: CountryID
        description: Country abbreviation
      - in: path
        name: RegionID
        description: Region abbreviation
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Lineups
      - Browse
      - CountryID
      - RegionID
  /TvMedia/lineups/browse/{CountryID}/{RegionID}/{AreaID}:
    get:
      summary: ""
      description: Get lineups by AreaID.
      operationId: GetTvMediaLineupsByAreaID
      x-api-path-slug: tvmedialineupsbrowsecountryidregionidareaid-get
      parameters:
      - in: path
        name: AreaID
        description: Service area ID
      - in: path
        name: CountryID
        description: Country abbreviation
      - in: query
        name: Detail
        description: Set level of detail for response
      - in: query
        name: LineupType
        description: Filter by lineup type, valid types are OTA, SAT, CAB, IPTV
      - in: query
        name: ProviderId
        description: Filter by provider ID
      - in: path
        name: RegionID
        description: Region abbreviation
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Lineups
      - Browse
      - CountryID
      - RegionID
      - AreaID
  /TvMedia/lineups/geo:
    get:
      summary: ""
      description: Get lineups by latitude and longitude.
      operationId: GetTvMediaLineupsByLatitudeLongitude
      x-api-path-slug: tvmedialineupsgeo-get
      parameters:
      - in: query
        name: Detail
        description: Set level of detail for response
      - in: query
        name: Latitude
        description: Latitude (geographic coordinate)
      - in: query
        name: LineupType
        description: Filter by lineup type, valid types are OTA, SAT, CAB, IPTV
      - in: query
        name: Longitude
        description: Longitude (geographic coordinate)
      - in: query
        name: ProviderId
        description: Filter by provider ID
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Lineups
      - Geo
  /TvMedia/lineups/{LineupID}:
    get:
      summary: ""
      description: Get lineups by specific LineupID.
      operationId: GetTvMediaLineupByID
      x-api-path-slug: tvmedialineupslineupid-get
      parameters:
      - in: query
        name: Detail
        description: Set level of detail for response
      - in: path
        name: LineupID
        description: Lineup ID
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Lineups
      - LineupID
  /TvMedia/lineups/{LineupID}/listings:
    get:
      summary: ""
      description: Retrieve individual listings for a given lineup ordered by start
        time (listDateTime) and channel number; unless using the search parameter,
        in which case they will be ordered by search term relevance.
      operationId: GetTvMediaLineupListings
      x-api-path-slug: tvmedialineupslineupidlistings-get
      parameters:
      - in: query
        name: AdultContent
        description: Defaults to 1 (allowed)
      - in: query
        name: Channel
        description: Include only channel(s) with this number, single or array values
          accepted
      - in: query
        name: DescriptiveVideoOnly
        description: Only displays listings which are flagged as being broadcast with
          Descriptive Video
      - in: query
        name: Detail
        description: Set level of detail for response
      - in: query
        name: DisplayArtwork
        description: Displays the Artwork information
      - in: query
        name: End
        description: UTC end time in ISO8601
      - in: query
        name: EndChan
        description: Highest channel
      - in: query
        name: ExcludeChan
        description: Exclude channels by number, single or array values accepted
      - in: query
        name: ExcludeShowType
        description: Exclude only these show type ID(s), array or single values accepted
      - in: query
        name: ExcludeStation
        description: Filter out station IDs; array or single value accepted
      - in: query
        name: Id
        description: ListingID, array or single values accepted
      - in: query
        name: League
        description: Get only sports listings in the given league ID(s)
      - in: path
        name: LineupID
        description: Lineup ID
      - in: query
        name: LiveOnly
        description: Only displays live listings
      - in: query
        name: NewShowsOnly
        description: Get new shows only
      - in: query
        name: NotYetStarted
        description: Only displays listings which are starting on or after the given
          start time
      - in: query
        name: Search
        description: 'search value: can be a show, episode, movie, team, league, person,
          etc'
      - in: query
        name: ShowType
        description: Include only these show type ID(s), array or single values accepted
      - in: query
        name: SportEventsOnly
        description: Get sporting events only
      - in: query
        name: SportType
        description: Get only sports listings of type sportTypeID
      - in: query
        name: Start
        description: UTC start time in ISO8601
      - in: query
        name: StartChan
        description: Lowest channel
      - in: query
        name: Station
        description: Filter by station ID
      - in: query
        name: Team
        description: Filter by teams playing by name(teams
      - in: query
        name: TimeZone
        description: Set a timezone or time offset for listing times (listDateTime
          property)
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Lineups
      - LineupID
      - Listings
  /TvMedia/lineups/{LineupID}/listings/grid:
    get:
      summary: ""
      description: A collection of listings grouped by channel and ordered by listDateTime.
        The grid dimensions ( time x channels ) can be modified by using the start,
        end, startchan and maxchan parameters. Channels without any listings will
        be returned with an empty listings collection.
      operationId: GetTvMediaLineupListingsGrid
      x-api-path-slug: tvmedialineupslineupidlistingsgrid-get
      parameters:
      - in: query
        name: AdultContent
        description: Defaults to 1 (allowed)
      - in: query
        name: Channel
        description: Include only channel(s) with this number, single or array values
          accepted
      - in: query
        name: DescriptiveVideoOnly
        description: Only displays listings which are flagged as being broadcast with
          Descriptive Video
      - in: query
        name: Detail
        description: Set level of detail for response
      - in: query
        name: DisplayArtwork
        description: Displays the Artwork information
      - in: query
        name: End
        description: UTC end time in ISO8601
      - in: query
        name: EndChan
        description: Highest channel
      - in: query
        name: ExcludeChan
        description: Exclude channels by number, single or array values accepted
      - in: query
        name: ExcludeShowType
        description: Exclude only these show type ID(s), array or single values accepted
      - in: query
        name: ExcludeStation
        description: Filter out station IDs; array or single value accepted
      - in: query
        name: Id
        description: ListingID, array or single values accepted
      - in: query
        name: League
        description: Get only sports listings in the given league ID(s)
      - in: path
        name: LineupID
        description: Lineup ID
      - in: query
        name: LiveOnly
        description: Only displays live listings
      - in: query
        name: NewShowsOnly
        description: Get new shows only
      - in: query
        name: NotYetStarted
        description: Only displays listings which are starting on or after the given
          start time
      - in: query
        name: Search
        description: 'search value: can be a show, episode, movie, team, league, person,
          etc'
      - in: query
        name: ShowType
        description: Include only these show type ID(s), array or single values accepted
      - in: query
        name: SportEventsOnly
        description: Get sporting events only
      - in: query
        name: SportType
        description: Get only sports listings of type sportTypeID
      - in: query
        name: Start
        description: UTC start time in ISO8601
      - in: query
        name: StartChan
        description: Lowest channel
      - in: query
        name: Station
        description: Filter by station ID
      - in: query
        name: Team
        description: Filter by teams playing by name(teams
      - in: query
        name: TimeZone
        description: Set a timezone or time offset for listing times (listDateTime
          property)
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Lineups
      - LineupID
      - Listings
      - Grid
  /TvMedia/lineups/{LineupID}/listings/highlights:
    get:
      summary: ""
      description: Retrieves featured listings. setting a start and/or end time for
        every request is a highly recommended.
      operationId: GetTvMediaLineupListingsHighlights
      x-api-path-slug: tvmedialineupslineupidlistingshighlights-get
      parameters:
      - in: query
        name: AdultContent
        description: Defaults to 1 (allowed)
      - in: query
        name: Channel
        description: Include only channel(s) with this number, single or array values
          accepted
      - in: query
        name: DescriptiveVideoOnly
        description: Only displays listings which are flagged as being broadcast with
          Descriptive Video
      - in: query
        name: Detail
        description: Set level of detail for response
      - in: query
        name: DisplayArtwork
        description: Displays the Artwork information
      - in: query
        name: End
        description: UTC end time in ISO8601
      - in: query
        name: EndChan
        description: Highest channel
      - in: query
        name: ExcludeChan
        description: Exclude channels by number, single or array values accepted
      - in: query
        name: ExcludeShowType
        description: Exclude only these show type ID(s), array or single values accepted
      - in: query
        name: ExcludeStation
        description: Filter out station IDs; array or single value accepted
      - in: query
        name: Id
        description: ListingID, array or single values accepted
      - in: query
        name: League
        description: Get only sports listings in the given league ID(s)
      - in: path
        name: LineupID
        description: Lineup ID
      - in: query
        name: LiveOnly
        description: Only displays live listings
      - in: query
        name: NewShowsOnly
        description: Get new shows only
      - in: query
        name: NotYetStarted
        description: Only displays listings which are starting on or after the given
          start time
      - in: query
        name: Search
        description: 'search value: can be a show, episode, movie, team, league, person,
          etc'
      - in: query
        name: ShowType
        description: Include only these show type ID(s), array or single values accepted
      - in: query
        name: SportEventsOnly
        description: Get sporting events only
      - in: query
        name: SportType
        description: Get only sports listings of type sportTypeID
      - in: query
        name: Start
        description: UTC start time in ISO8601
      - in: query
        name: StartChan
        description: Lowest channel
      - in: query
        name: Station
        description: Filter by station ID
      - in: query
        name: Team
        description: Filter by teams playing by name(teams
      - in: query
        name: TimeZone
        description: Set a timezone or time offset for listing times (listDateTime
          property)
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Lineups
      - LineupID
      - Listings
      - Highlights
  /TvMedia/reference/lineups:
    get:
      summary: ""
      description: Get list of generic lineup IDs that can be used.  A 'generic' lineup
        is not a real lineup, but a collection of stations defined by TV Media.  Any
        listing retrieved using a generic lineup will not return any channel number
        information, as it is irrelevant.
      operationId: GetTvMediaGenericLineups
      x-api-path-slug: tvmediareferencelineups-get
      parameters:
      - in: query
        name: Detail
        description: Set level of detail for response
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Reference
      - Lineups
  /TvMedia/stations/{StationID}:
    get:
      summary: ""
      description: Gets station details by ID.
      operationId: GetTvMediaStation
      x-api-path-slug: tvmediastationsstationid-get
      parameters:
      - in: path
        name: StationID
        description: Station ID
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Stations
      - StationID
  /TvMedia/stations/{StationID}/listings:
    get:
      summary: Stations are not tied to lineups, therefore no channel numbers will
        be present in the response, unlike most other listing operations.
      description: Get listings for a given station.
      operationId: GetTvMediaListingsByStation
      x-api-path-slug: tvmediastationsstationidlistings-get
      parameters:
      - in: query
        name: AdultContent
        description: Defaults to 1 (allowed)
      - in: query
        name: Channel
        description: Include only channel(s) with this number, single or array values
          accepted
      - in: query
        name: DescriptiveVideoOnly
        description: Only displays listings which are flagged as being broadcast with
          Descriptive Video
      - in: query
        name: Detail
        description: Set level of detail for response
      - in: query
        name: DisplayArtwork
        description: Displays the Artwork information
      - in: query
        name: End
        description: UTC end time in ISO8601
      - in: query
        name: EndChan
        description: Highest channel
      - in: query
        name: ExcludeChan
        description: Exclude channels by number, single or array values accepted
      - in: query
        name: ExcludeShowType
        description: Exclude only these show type ID(s), array or single values accepted
      - in: query
        name: ExcludeStation
        description: Filter out station IDs; array or single value accepted
      - in: query
        name: Id
        description: ListingID, array or single values accepted
      - in: query
        name: League
        description: Get only sports listings in the given league ID(s)
      - in: query
        name: LiveOnly
        description: Only displays live listings
      - in: query
        name: NewShowsOnly
        description: Get new shows only
      - in: query
        name: NotYetStarted
        description: Only displays listings which are starting on or after the given
          start time
      - in: query
        name: Search
        description: 'search value: can be a show, episode, movie, team, league, person,
          etc'
      - in: query
        name: ShowType
        description: Include only these show type ID(s), array or single values accepted
      - in: query
        name: SportEventsOnly
        description: Get sporting events only
      - in: query
        name: SportType
        description: Get only sports listings of type sportTypeID
      - in: query
        name: Start
        description: UTC start time in ISO8601
      - in: query
        name: StartChan
        description: Lowest channel
      - in: query
        name: Station
        description: Filter by station ID
      - in: path
        name: StationID
        description: Station ID
      - in: query
        name: Team
        description: Filter by teams playing by name(teams
      - in: query
        name: TimeZone
        description: Set a timezone or time offset for listing times (listDateTime
          property)
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Stations
      - StationID
      - Listings
  /TvMedia/teams/{TeamID}:
    get:
      summary: ""
      description: Gets details for a specific team.
      operationId: GetTvMediaTeamById
      x-api-path-slug: tvmediateamsteamid-get
      parameters:
      - in: path
        name: TeamID
        description: Team ID
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Teams
      - TeamID
  /TvMedia/teams/{TeamID}/listings:
    get:
      summary: ""
      description: Retrieve listings for a given TeamID.
      operationId: GetTvMediaTeamListings
      x-api-path-slug: tvmediateamsteamidlistings-get
      parameters:
      - in: query
        name: AdultContent
        description: Defaults to 1 (allowed)
      - in: query
        name: Channel
        description: Include only channel(s) with this number, single or array values
          accepted
      - in: query
        name: DescriptiveVideoOnly
        description: Only displays listings which are flagged as being broadcast with
          Descriptive Video
      - in: query
        name: Detail
        description: Set level of detail for response
      - in: query
        name: DisplayArtwork
        description: Displays the Artwork information
      - in: query
        name: End
        description: UTC end time in ISO8601
      - in: query
        name: EndChan
        description: Highest channel
      - in: query
        name: ExcludeChan
        description: Exclude channels by number, single or array values accepted
      - in: query
        name: ExcludeShowType
        description: Exclude only these show type ID(s), array or single values accepted
      - in: query
        name: ExcludeStation
        description: Filter out station IDs; array or single value accepted
      - in: query
        name: Id
        description: ListingID, array or single values accepted
      - in: query
        name: League
        description: Get only sports listings in the given league ID(s)
      - in: query
        name: LineupID
        description: Lineup ID
      - in: query
        name: LiveOnly
        description: Only displays live listings
      - in: query
        name: NewShowsOnly
        description: Get new shows only
      - in: query
        name: NotYetStarted
        description: Only displays listings which are starting on or after the given
          start time
      - in: query
        name: Search
        description: 'search value: can be a show, episode, movie, team, league, person,
          etc'
      - in: query
        name: ShowType
        description: Include only these show type ID(s), array or single values accepted
      - in: query
        name: SportEventsOnly
        description: Get sporting events only
      - in: query
        name: SportType
        description: Get only sports listings of type sportTypeID
      - in: query
        name: Start
        description: UTC start time in ISO8601
      - in: query
        name: StartChan
        description: Lowest channel
      - in: query
        name: Station
        description: Filter by station ID
      - in: query
        name: Team
        description: Filter by teams playing by name(teams
      - in: path
        name: TeamID
        description: Team ID
      - in: query
        name: TimeZone
        description: Set a timezone or time offset for listing times (listDateTime
          property)
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Teams
      - TeamID
      - Listings
  /Videos/GetVideo/{Id}:
    get:
      summary: Returns a URL to a requested video.
      description: "Returns a URL to the requested video. [Video Format Specs](https://developer.iva-api.com/docs/v1/video-formats)\n\n**Formats:**
        MP4 = 4, HLS = 11, Dash = 14, HSS = 12, HDS = 13\n\n**MP4 KbRate:** 80, 212,
        450, 750, 1500, 2500(HD sources only), 5000 (sources >=  1080p)  \n\n**Adaptive
        Min/Max rate:** 212000, 350000, 600000, 1200000, 2000000, 2500000, 3500000
        \ \n\n `URLs requested with a Demo account will always return max 750 kbps
        video.  Full commercial account required for higher bitrates.`"
      operationId: GetVideo
      x-api-path-slug: videosgetvideoid-get
      parameters:
      - in: query
        name: end
        description: Position in seconds to end video playback
      - in: query
        name: Expires
        description: UTC Time to video link should expire
      - in: query
        name: Format
        description: Video format
      - in: path
        name: Id
        description: Id of the Video from either MovieVideo, ShowVideo, SeasonVideo,
          EpisodeVideo object
      - in: query
        name: KbRate
        description: Video bitrate required for MP4 content
      - in: query
        name: MaxRate
        description: Adaptive Minimum rate
      - in: query
        name: MinRate
        description: Adaptive Maximum rate
      - in: query
        name: ReportTag
        description: Report tag used in video analytics
      - in: query
        name: start
        description: Position in seconds to start video playback
      responses:
        200:
          description: OK
      tags:
      - Videos
      - Video
      - Id
  /XroadMedia/recommendations:
    get:
      summary: Returns a list of recommendations from XRoadMedia for a movie or show.
      description: Get recommendations for movie or show.
      operationId: GetXRoadMediaRecommendations
      x-api-path-slug: xroadmediarecommendations-get
      parameters:
      - in: query
        name: MovieId
        description: Source MovieId for recommendations
      - in: query
        name: ShowId
        description: Source ShowId for recommendations
      - in: query
        name: Type
        description: Type of recommendation response
      responses:
        200:
          description: OK
      tags:
      - XroadMedia
      - Recommendations