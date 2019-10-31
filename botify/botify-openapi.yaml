swagger: "2.0"
x-collection-name: Botify
x-complete: 1
info:
  title: Botify
  description: botify-saas-api
  version: 1.0.0
host: api.botify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /analyses/{username}/{project_slug}:
    get:
      summary: Get Analyses Username Project Slug
      description: Get analyses username project slug.
      operationId: getAnalysesUsernameProjectSlug
      x-api-path-slug: analysesusernameproject-slug-get
      parameters:
      - in: query
        name: only_success
        description: Return only successfully finished analyses
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
    parameters:
      summary: Parameters Analyses Username Project Slug
      description: Parameters analyses username project slug.
      operationId: parametersAnalysesUsernameProjectSlug
      x-api-path-slug: analysesusernameproject-slug-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
  /analyses/{username}/{project_slug}/{analysis_slug}:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug
      description: Get analyses username project slug analysis slug.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlug
      x-api-path-slug: analysesusernameproject-sluganalysis-slug-get
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug
      description: Parameters analyses username project slug analysis slug.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlug
      x-api-path-slug: analysesusernameproject-sluganalysis-slug-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
  /analyses/{username}/{project_slug}/{analysis_slug}/crawl_statistics:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Crawl Statistics
      description: Get analyses username project slug analysis slug crawl statistics.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugCrawlStatistics
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statistics-get
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Crawl Statistics
      description: Parameters analyses username project slug analysis slug crawl statistics.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugCrawlStatistics
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statistics-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
  /analyses/{username}/{project_slug}/{analysis_slug}/crawl_statistics/time:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Crawl Statistics Time
      description: Return crawl statistics grouped by time frequency (1 min, 5 mins
        or 60 min) for an analysis
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugCrawlStatisticsTime
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statisticstime-get
      parameters:
      - in: query
        name: frequency
        description: Aggregation frequency
      - in: query
        name: limit
        description: max number of elements to retrieve
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
      - Time
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Crawl Statistics
        Time
      description: Parameters analyses username project slug analysis slug crawl statistics
        time.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugCrawlStatisticsTime
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statisticstime-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
      - Time
  /analyses/{username}/{project_slug}/{analysis_slug}/crawl_statistics/urls/{list_type}:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Crawl Statistics Urls
        List Type
      description: Return a list of 1000 latest URLs crawled (all crawled URLs or
        only URLS with HTTP errors)
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugCrawlStatisticsUrlsListType
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statisticsurlslist-type-get
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
      - Urls
      - List
      - Type
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Crawl Statistics
        Urls List Type
      description: Parameters analyses username project slug analysis slug crawl statistics
        urls list type.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugCrawlStatisticsUrlsListType
      x-api-path-slug: analysesusernameproject-sluganalysis-slugcrawl-statisticsurlslist-type-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Crawl
      - Statistics
      - Urls
      - List
      - Type
  /analyses/{username}/{project_slug}/{analysis_slug}/features/ganalytics/orphan_urls/{medium}/{source}:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Ganalytics
        Orphan Urls Medium Source
      description: 'Legacy    List of Orphan URLs. URLs which generated visits from
        the selected source according to Google Analytics data, but were not crawled
        with by the Botify crawler (either because no links to them were found on
        the website, or because the crawler was not allowed to follow these links
        according to the project settings).   For a search engine (medium: origanic;
        sources: all, aol, ask, baidu, bing, google, naver, yahoo, yandex) or a social
        network (medium: social; sources: all, facebook, google+, linkedin, pinterest,
        reddit, tumblr, twitter)'
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesGanalyticsOrphanUrlsMediumSource
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturesganalyticsorphan-urlsmediumsource-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Ganalytics
      - Orphan
      - Urls
      - Medium
      - Source
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Ganalytics
        Orphan Urls Medium Source
      description: Parameters analyses username project slug analysis slug features
        ganalytics orphan urls medium source.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesGanalyticsOrphanUrlsMediumSource
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturesganalyticsorphan-urlsmediumsource-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Ganalytics
      - Orphan
      - Urls
      - Medium
      - Source
  /analyses/{username}/{project_slug}/{analysis_slug}/features/links/percentiles:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Links Percentiles
      description: Get analyses username project slug analysis slug features links
        percentiles.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesLinksPercentiles
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeatureslinkspercentiles-get
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Links
      - Percentiles
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Links
        Percentiles
      description: Parameters analyses username project slug analysis slug features
        links percentiles.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesLinksPercentiles
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeatureslinkspercentiles-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Links
      - Percentiles
  /analyses/{username}/{project_slug}/{analysis_slug}/features/pagerank/lost:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Pagerank
        Lost
      description: Get analyses username project slug analysis slug features pagerank
        lost.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesPagerankLost
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturespageranklost-get
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Pagerank
      - Lost
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Pagerank
        Lost
      description: Parameters analyses username project slug analysis slug features
        pagerank lost.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesPagerankLost
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturespageranklost-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Pagerank
      - Lost
  /analyses/{username}/{project_slug}/{analysis_slug}/features/sitemaps/report:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Sitemaps
        Report
      description: Get global information of the sitemaps found (sitemaps indexes,
        invalid sitemaps urls, etc.)
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesSitemapsReport
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturessitemapsreport-get
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Sitemaps
      - Report
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Sitemaps
        Report
      description: Parameters analyses username project slug analysis slug features
        sitemaps report.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesSitemapsReport
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturessitemapsreport-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Sitemaps
      - Report
  /analyses/{username}/{project_slug}/{analysis_slug}/features/sitemaps/samples/out_of_config:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Sitemaps
        Samples Out Of Config
      description: Sample list of URLs which were found in your sitemaps but outside
        of the crawl perimeter defined for the project, for instance domain/subdomain
        or protocol (HTTP/HTTPS) not allowed in the crawl settings.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesSitemapsSamplesOutOfConfig
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturessitemapssamplesout-of-config-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Sitemaps
      - Samples
      - Out
      - Of
      - Config
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Sitemaps
        Samples Out Of Config
      description: Parameters analyses username project slug analysis slug features
        sitemaps samples out of config.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesSitemapsSamplesOutOfConfig
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturessitemapssamplesout-of-config-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Sitemaps
      - Samples
      - Out
      - Of
      - Config
  /analyses/{username}/{project_slug}/{analysis_slug}/features/sitemaps/samples/sitemap_only:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Sitemaps
        Samples Sitemap Only
      description: Sample list of URLs which were found in your sitemaps, within the
        project allowed scope (allowed domains/subdomains/protocols), but not found
        by the Botify crawler.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesSitemapsSamplesSitemapOnly
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturessitemapssamplessitemap-only-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Sitemaps
      - Samples
      - Sitemap
      - Only
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Sitemaps
        Samples Sitemap Only
      description: Parameters analyses username project slug analysis slug features
        sitemaps samples sitemap only.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesSitemapsSamplesSitemapOnly
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturessitemapssamplessitemap-only-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Sitemaps
      - Samples
      - Sitemap
      - Only
  /analyses/{username}/{project_slug}/{analysis_slug}/features/top_domains/domains:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Top Domains
        Domains
      description: Get analyses username project slug analysis slug features top domains
        domains.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesTopDomainsDomains
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturestop-domainsdomains-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Top
      - Domains
      - Domains
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Top
        Domains Domains
      description: Parameters analyses username project slug analysis slug features
        top domains domains.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesTopDomainsDomains
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturestop-domainsdomains-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Top
      - Domains
      - Domains
  /analyses/{username}/{project_slug}/{analysis_slug}/features/top_domains/subdomains:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Top Domains
        Subdomains
      description: Get analyses username project slug analysis slug features top domains
        subdomains.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesTopDomainsSubdomains
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturestop-domainssubdomains-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Top
      - Domains
      - Subdomains
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Top
        Domains Subdomains
      description: Parameters analyses username project slug analysis slug features
        top domains subdomains.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesTopDomainsSubdomains
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturestop-domainssubdomains-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Top
      - Domains
      - Subdomains
  /analyses/{username}/{project_slug}/{analysis_slug}/features/visits/orphan_urls/{medium}/{source}:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Features Visits Orphan
        Urls Medium Source
      description: 'List of Orphan URLs. URLs which generated visits from the selected
        source according to Google Analytics data, but were not crawled with by the
        Botify crawler (either because no links to them were found on the website,
        or because the crawler was not allowed to follow these links according to
        the project settings).   For a search engine (medium: origanic; sources: all,
        aol, ask, baidu, bing, google, naver, yahoo, yandex) or a social network (medium:
        social; sources: all, facebook, google+, linkedin, pinterest, reddit, tumblr,
        twitter)'
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugFeaturesVisitsOrphanUrlsMediumSource
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturesvisitsorphan-urlsmediumsource-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Visits
      - Orphan
      - Urls
      - Medium
      - Source
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Features Visits
        Orphan Urls Medium Source
      description: Parameters analyses username project slug analysis slug features
        visits orphan urls medium source.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugFeaturesVisitsOrphanUrlsMediumSource
      x-api-path-slug: analysesusernameproject-sluganalysis-slugfeaturesvisitsorphan-urlsmediumsource-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Features
      - Visits
      - Orphan
      - Urls
      - Medium
      - Source
  /analyses/{username}/{project_slug}/{analysis_slug}/urls:
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Urls
      description: Parameters analyses username project slug analysis slug urls.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugUrls
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurls-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
    post:
      summary: Post Analyses Username Project Slug Analysis Slug Urls
      description: Post analyses username project slug analysis slug urls.
      operationId: postAnalysesUsernameProjectSlugAnalysisSlugUrls
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurls-post
      parameters:
      - in: query
        name: area
        description: Analysis context
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      - in: body
        name: UrlsQuery
        description: Urls query
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
  /analyses/{username}/{project_slug}/{analysis_slug}/urls/aggs:
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Urls Aggs
      description: Parameters analyses username project slug analysis slug urls aggs.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugUrlsAggs
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsaggs-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Aggs
    post:
      summary: Post Analyses Username Project Slug Analysis Slug Urls Aggs
      description: Post analyses username project slug analysis slug urls aggs.
      operationId: postAnalysesUsernameProjectSlugAnalysisSlugUrlsAggs
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsaggs-post
      parameters:
      - in: query
        name: area
        description: Analysis context
      - in: body
        name: UrlsAggsQueries
        description: UrlsAggs queries
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Aggs
  /analyses/{username}/{project_slug}/{analysis_slug}/urls/datamodel:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Urls Datamodel
      description: Get analyses username project slug analysis slug urls datamodel.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugUrlsDatamodel
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsdatamodel-get
      parameters:
      - in: query
        name: area
        description: Analysis context
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Datamodel
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Urls Datamodel
      description: Parameters analyses username project slug analysis slug urls datamodel.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugUrlsDatamodel
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsdatamodel-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Datamodel
  /analyses/{username}/{project_slug}/{analysis_slug}/urls/export:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Urls Export
      description: Get analyses username project slug analysis slug urls export.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugUrlsExport
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsexport-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Export
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Urls Export
      description: Parameters analyses username project slug analysis slug urls export.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugUrlsExport
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsexport-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Export
    post:
      summary: Post Analyses Username Project Slug Analysis Slug Urls Export
      description: Creates a new UrlExport object and starts a task that will export
        the results into a csv. Returns the model id that manages the task
      operationId: postAnalysesUsernameProjectSlugAnalysisSlugUrlsExport
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsexport-post
      parameters:
      - in: query
        name: area
        description: Analysis context
      - in: body
        name: UrlsQuery
        description: Urls query
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Export
  /analyses/{username}/{project_slug}/{analysis_slug}/urls/export/{url_export_id}:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Urls Export Url Export
      description: Checks the status of an CSVUrlExportJob object. Returns json object
        with the status.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugUrlsExportUrlExport
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsexporturl-export-id-get
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Export
      - Url
      - Export
      - Id
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Urls Export
        Url Export
      description: Parameters analyses username project slug analysis slug urls export
        url export.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugUrlsExportUrlExport
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsexporturl-export-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Export
      - Url
      - Export
      - Id
  /analyses/{username}/{project_slug}/{analysis_slug}/urls/suggested_filters:
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Urls Suggested
        Filters
      description: Parameters analyses username project slug analysis slug urls suggested
        filters.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugUrlsSuggestedFilters
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlssuggested-filters-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Suggested
      - Filters
    post:
      summary: Post Analyses Username Project Slug Analysis Slug Urls Suggested Filters
      description: Return most frequent segments (= suggested patterns in the previous
        version) for a Botify Query.
      operationId: postAnalysesUsernameProjectSlugAnalysisSlugUrlsSuggestedFilters
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlssuggested-filters-post
      parameters:
      - in: query
        name: area
        description: Analysis context
      - in: body
        name: UrlsAggsQuery
        description: UrlsAggs query
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Suggested
      - Filters
  /analyses/{username}/{project_slug}/{analysis_slug}/urls/{url}:
    get:
      summary: Get Analyses Username Project Slug Analysis Slug Urls Url
      description: Get analyses username project slug analysis slug urls url.
      operationId: getAnalysesUsernameProjectSlugAnalysisSlugUrlsUrl
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsurl-get
      parameters:
      - in: query
        name: fields
        description: comma separated list of fields to return (c
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Url
    parameters:
      summary: Parameters Analyses Username Project Slug Analysis Slug Urls Url
      description: Parameters analyses username project slug analysis slug urls url.
      operationId: parametersAnalysesUsernameProjectSlugAnalysisSlugUrlsUrl
      x-api-path-slug: analysesusernameproject-sluganalysis-slugurlsurl-parameters
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Username
      - Project
      - Slug
      - Analysis
      - Slug
      - Urls
      - Url
  /projects/{username}:
    get:
      summary: Get Projects Username
      description: List all active projects for the user
      operationId: getProjectsUsername
      x-api-path-slug: projectsusername-get
      parameters:
      - in: query
        name: name
        description: Projects name
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Username
    parameters:
      summary: Parameters Projects Username
      description: Parameters projects username.
      operationId: parametersProjectsUsername
      x-api-path-slug: projectsusername-parameters
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Username
  /projects/{username}/{project_slug}/filters:
    get:
      summary: Get Projects Username Project Slug Filters
      description: List all the project's saved filters (each filter's name, ID and
        filter value)
      operationId: getProjectsUsernameProjectSlugFilters
      x-api-path-slug: projectsusernameproject-slugfilters-get
      parameters:
      - in: query
        name: page
        description: Page Number
      - in: query
        name: size
        description: Page Size
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Username
      - Project
      - Slug
      - Filters
    parameters:
      summary: Parameters Projects Username Project Slug Filters
      description: Parameters projects username project slug filters.
      operationId: parametersProjectsUsernameProjectSlugFilters
      x-api-path-slug: projectsusernameproject-slugfilters-parameters
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Username
      - Project
      - Slug
      - Filters
  /projects/{username}/{project_slug}/filters/{identifier}:
    get:
      summary: Get Projects Username Project Slug Filters Entifier
      description: Retrieves a specific saved filter's name, ID and filter value
      operationId: getProjectsUsernameProjectSlugFiltersEntifier
      x-api-path-slug: projectsusernameproject-slugfiltersidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Username
      - Project
      - Slug
      - Filters
      - Identifier
    parameters:
      summary: Parameters Projects Username Project Slug Filters Entifier
      description: Parameters projects username project slug filters entifier.
      operationId: parametersProjectsUsernameProjectSlugFiltersEntifier
      x-api-path-slug: projectsusernameproject-slugfiltersidentifier-parameters
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Username
      - Project
      - Slug
      - Filters
      - Identifier
  /projects/{username}/{project_slug}/urls/aggs:
    parameters:
      summary: Parameters Projects Username Project Slug Urls Aggs
      description: Parameters projects username project slug urls aggs.
      operationId: parametersProjectsUsernameProjectSlugUrlsAggs
      x-api-path-slug: projectsusernameproject-slugurlsaggs-parameters
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Username
      - Project
      - Slug
      - Urls
      - Aggs
    post:
      summary: Post Projects Username Project Slug Urls Aggs
      description: Project Query aggregator. It accepts multiple queries that will
        be executed on all completed analyses in the project
      operationId: postProjectsUsernameProjectSlugUrlsAggs
      x-api-path-slug: projectsusernameproject-slugurlsaggs-post
      parameters:
      - in: query
        name: area
        description: Analyses context
      - in: query
        name: last_analysis_slug
        description: Last analysis on the trend
      - in: query
        name: nb_analyses
        description: Max number of analysis to return
      - in: body
        name: UrlsAggsQueries
        description: UrlsAggs queries
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Username
      - Project
      - Slug
      - Urls
      - Aggs