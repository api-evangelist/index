swagger: "2.0"
x-collection-name: Wikipedia
x-complete: 1
info:
  title: Wikipedia
  description: this-api-provides-cacheable-and-straightforward-access-to-wikimedia-content-and-data-in-machinereadable-formats-
  termsOfService: https://wikimediafoundation.org/wiki/Terms_of_Use
  contact:
    name: the Wikimedia Services team
    url: http://mediawiki.org/wiki/REST_API
  version: v1
host: wikimedia.org
basePath: /api/rest_v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /media/math/check/{type}:
    post:
      summary: Check and normalize a TeX formula.
      description: |-
        Checks the supplied TeX formula for correctness and returns the
        normalised formula representation as well as information about
        identifiers. Available types are tex and inline-tex. The response
        contains the `x-resource-location` header which can be used to retrieve
        the render of the checked formula in one of the supported rendering
        formats. Just append the value of the header to `/media/math/{format}/`
        and perform a GET request against that URL.

        Stability: [stable](https://www.mediawiki.org/wiki/API_versioning#Stable).
      operationId: checks-the-supplied-tex-formula-for-correctness-and-returns-thenormalised-formula-representation-as-
      x-api-path-slug: mediamathchecktype-post
      parameters:
      - in: formData
        name: q
        description: The formula to check
      - in: path
        name: type
        description: The input type of the given formula; can be tex or inline-tex
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /media/math/formula/{hash}:
    get:
      summary: Get a previously-stored formula
      description: |-
        Returns the previously-stored formula via `/media/math/check/{type}` for
        the given hash.

        Stability: [stable](https://www.mediawiki.org/wiki/API_versioning#Stable).
      operationId: returns-the-previouslystored-formula-via-mediamathchecktype-forthe-given-hashstability-stablehttpsww
      x-api-path-slug: mediamathformulahash-get
      parameters:
      - in: path
        name: hash
        description: The hash string of the previous POST data
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /media/math/render/{format}/{hash}:
    get:
      summary: Get rendered formula in the given format.
      description: |-
        Given a request hash, renders a TeX formula into its mathematic
        representation in the given format. When a request is issued to the
        `/media/math/check/{format}` POST endpoint, the response contains the
        `x-resource-location` header denoting the hash ID of the POST data. Once
        obtained, this endpoint has to be used to obtain the actual render.

        Stability: [stable](https://www.mediawiki.org/wiki/API_versioning#Stable).
      operationId: given-a-request-hash-renders-a-tex-formula-into-its-mathematicrepresentation-in-the-given-format-whe
      x-api-path-slug: mediamathrenderformathash-get
      parameters:
      - in: path
        name: format
        description: The output format; can be svg or mml
      - in: path
        name: hash
        description: The hash string of the previous POST data
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/bytes-difference/absolute/aggregate/{project}/{editor-type}/{page-type}/{granularity}/{start}/{end}:
    get:
      summary: |-
        Get the sum of absolute value of text bytes difference between current edit and
        previous one.
      description: |-
        Given a Mediawiki project and a date range, returns a timeseries of absolute bytes
        difference sums. You can filter by editors-type (all-editor-types, anonymous, group-bot,
        name-bot, user) and page-type (all-page-types, content, non-content). You can choose
        between daily and monthly granularity as well.

        - Stability: [experimental](https://www.mediawiki.org/wiki/API_versioning#Experimental)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-mediawiki-project-and-a-date-range-returns-a-timeseries-of-absolute-bytesdifference-sums-you
      x-api-path-slug: metricsbytesdifferenceabsoluteaggregateprojecteditortypepagetypegranularitystartend-get
      parameters:
      - in: path
        name: editor-type
        description: If you want to filter by editor-type, use one of anonymous, group-bot
          (registeredaccounts belonging to the bot group), name-bot (registered accounts
          not belonging tothe bot group but having bot-like names) or user (registered
          account not in bot groupnor having bot-like name)
      - in: path
        name: end
        description: The date of the last day to include, in YYYYMMDD format
      - in: path
        name: granularity
        description: Time unit for the response data
      - in: path
        name: page-type
        description: If you want to filter by page-type, use one of content (edits
          on pages in contentnamespaces) or non-content (edits on pages in non-content
          namespaces)
      - in: path
        name: project
        description: The name of any Wikimedia project formatted like {language code}
      - in: path
        name: start
        description: The date of the first day to include, in YYYYMMDD format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/bytes-difference/net/aggregate/{project}/{editor-type}/{page-type}/{granularity}/{start}/{end}:
    get:
      summary: Get the sum of net text bytes difference between current edit and previous
        one.
      description: |-
        Given a Mediawiki project and a date range, returns a timeseries of bytes difference net
        sums. You can filter by editors-type (all-editor-types, anonymous, group-bot, name-bot,
        user) and page-type (all-page-types, content or non-content). You can choose between
        daily and monthly granularity as well.

        - Stability: [experimental](https://www.mediawiki.org/wiki/API_versioning#Experimental)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-mediawiki-project-and-a-date-range-returns-a-timeseries-of-bytes-difference-netsums-you-can-
      x-api-path-slug: metricsbytesdifferencenetaggregateprojecteditortypepagetypegranularitystartend-get
      parameters:
      - in: path
        name: editor-type
        description: If you want to filter by editor-type, use one of anonymous, group-bot
          (registeredaccounts belonging to the bot group), name-bot (registered accounts
          not belonging tothe bot group but having bot-like names) or user (registered
          account not in bot groupnor having bot-like name)
      - in: path
        name: end
        description: The date of the last day to include, in YYYYMMDD format
      - in: path
        name: granularity
        description: Time unit for the response data
      - in: path
        name: page-type
        description: If you want to filter by page-type, use one of content (edits
          on pages in contentnamespaces) or non-content (edits on pages in non-content
          namespaces)
      - in: path
        name: project
        description: The name of any Wikimedia project formatted like {language code}
      - in: path
        name: start
        description: The date of the first day to include, in YYYYMMDD format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/edited-pages/aggregate/{project}/{editor-type}/{page-type}/{activity-level}/{granularity}/{start}/{end}:
    get:
      summary: Get edited-pages counts for a project.
      description: |-
        Given a Mediawiki project and a date range, returns a timeseries of its edited-pages counts.
        You can filter by editor-type (all-editor-types, anonymous, group-bot, name-bot, user),
        page-type (all-page-types, content or non-content) or activity-level (1..4-edits,
        5..24-edits, 25..99-edits, 100..-edits). You can choose between daily and monthly
        granularity as well.

        - Stability: [experimental](https://www.mediawiki.org/wiki/API_versioning#Experimental)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-mediawiki-project-and-a-date-range-returns-a-timeseries-of-its-editedpages-countsyou-can-fil
      x-api-path-slug: metricseditedpagesaggregateprojecteditortypepagetypeactivitylevelgranularitystartend-get
      parameters:
      - in: path
        name: activity-level
        description: If you want to filter by activity-level, use one of 1
      - in: path
        name: editor-type
        description: If you want to filter by editor-type, use one of anonymous, group-bot
          (registeredaccounts belonging to the bot group), name-bot (registered accounts
          not belonging tothe bot group but having bot-like names) or user (registered
          account not in bot groupnor having bot-like name)
      - in: path
        name: end
        description: The date of the last day to include, in YYYYMMDD format
      - in: path
        name: granularity
        description: The time unit for the response data
      - in: path
        name: page-type
        description: If you want to filter by page-type, use one of content (edited-pages
          in contentnamespaces) or non-content (edited-pages in non-content namespaces)
      - in: path
        name: project
        description: The name of any Wikimedia project formatted like {language code}
      - in: path
        name: start
        description: The date of the first day to include, in YYYYMMDD format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/edited-pages/new/{project}/{editor-type}/{page-type}/{granularity}/{start}/{end}:
    get:
      summary: Get new pages counts for a project.
      description: |-
        Given a Mediawiki project and a date range, returns a timeseries of its new pages counts.
        You can filter by editor type (all-editor-types, anonymous, group-bot, name-bot, user)
        or page-type (all-page-types, content or non-content). You can choose between daily and
        monthly granularity as well.
        The new pages value is computed as follow:
          [number of created pages] - [number of deleted pages] + [number of restored pages]
        for the chosen filters.

        - Stability: [experimental](https://www.mediawiki.org/wiki/API_versioning#Experimental)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-mediawiki-project-and-a-date-range-returns-a-timeseries-of-its-new-pages-countsyou-can-filte
      x-api-path-slug: metricseditedpagesnewprojecteditortypepagetypegranularitystartend-get
      parameters:
      - in: path
        name: editor-type
        description: If you want to filter by editor-type, use one of anonymous, group-bot
          (registeredaccounts belonging to the bot group), name-bot (registered accounts
          not belongingto the bot group but having bot-like names) or user (registered
          account not in botgroup nor having bot-like name)
      - in: path
        name: end
        description: The date of the last day to include, in YYYYMMDD format
      - in: path
        name: granularity
        description: The time unit for the response data
      - in: path
        name: page-type
        description: If you want to filter by page-type, use one of content (new pages
          in contentnamespaces) or non-content (new pages in non-content namespaces)
      - in: path
        name: project
        description: The name of any Wikimedia project formatted like {language code}
      - in: path
        name: start
        description: The date of the first day to include, in YYYYMMDD format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/edited-pages/top-by-absolute-bytes-difference/{project}/{editor-type}/{page-type}/{granularity}/{start}/{end}:
    get:
      summary: Get top 100 edited-pages by absolute bytes-difference.
      description: |-
        Given a Mediawiki project and a date range, returns a timeseries of the top 100 edited-pages
        by absolute bytes-difference. You can filter by editor-type (all-editor-types, anonymous,
        group-bot, name-bot, user) or page-type (all-page-types, content or non-content). You can
        choose between daily and monthly granularity as well.

        - Stability: [experimental](https://www.mediawiki.org/wiki/API_versioning#Experimental)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-mediawiki-project-and-a-date-range-returns-a-timeseries-of-the-top-100-editedpagesby-absolut
      x-api-path-slug: metricseditedpagestopbyabsolutebytesdifferenceprojecteditortypepagetypegranularitystartend-get
      parameters:
      - in: path
        name: editor-type
        description: If you want to filter by editor-type, use one of anonymous, group-bot
          (registeredaccounts belonging to the bot group), name-bot (registered accounts
          not belonging tothe bot group but having bot-like names) or user (registered
          account not in bot groupnor having bot-like name)
      - in: path
        name: end
        description: The date of the last day to include, in YYYYMMDD format
      - in: path
        name: granularity
        description: Time unit for the response data
      - in: path
        name: page-type
        description: If you want to filter by page-type, use one of content (edits
          on pages in contentnamespaces) or non-content (edits on pages in non-content
          namespaces)
      - in: path
        name: project
        description: The name of any Wikimedia project formatted like {language code}
      - in: path
        name: start
        description: The date of the first day to include, in YYYYMMDD format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/edited-pages/top-by-edits/{project}/{editor-type}/{page-type}/{granularity}/{start}/{end}:
    get:
      summary: Get top 100 edited-pages by edits count.
      description: |-
        Given a Mediawiki project and a date range, returns a timeseries of the top 100 edited-pages
        by edits count. You can filter by editor-type (all-editor-types, anonymous, group-bot,
        name-bot, user) or page-type (all-page-types, content or non-content). You can choose
        between daily and monthly granularity as well.

        - Stability: [experimental](https://www.mediawiki.org/wiki/API_versioning#Experimental)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-mediawiki-project-and-a-date-range-returns-a-timeseries-of-the-top-100-editedpagesby-edits-c
      x-api-path-slug: metricseditedpagestopbyeditsprojecteditortypepagetypegranularitystartend-get
      parameters:
      - in: path
        name: editor-type
        description: If you want to filter by editor-type, use one of anonymous, group-bot
          (registeredaccounts belonging to the bot group), name-bot (registered accounts
          not belonging tothe bot group but having bot-like names) or user (registered
          account not in bot groupnor having bot-like name)
      - in: path
        name: end
        description: The date of the last day to include, in YYYYMMDD format
      - in: path
        name: granularity
        description: Time unit for the response data
      - in: path
        name: page-type
        description: If you want to filter by page-type, use one of content (edits
          on pages in contentnamespaces) or non-content (edits on pages in non-content
          namespaces)
      - in: path
        name: project
        description: The name of any Wikimedia project formatted like {language code}
      - in: path
        name: start
        description: The date of the first day to include, in YYYYMMDD format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/edited-pages/top-by-net-bytes-difference/{project}/{editor-type}/{page-type}/{granularity}/{start}/{end}:
    get:
      summary: Get top 100 edited-pages by net bytes-difference.
      description: |-
        Given a Mediawiki project and a date range, returns a timeseries of the top 100 edited-pages
        by net bytes-difference. You can filter by editor-type (all-editor-types, anonymous,
        group-bot, name-bot, user) or page-type (all-page-types, content or non-content). You can
        choose between daily and monthly granularity as well.

        - Stability: [experimental](https://www.mediawiki.org/wiki/API_versioning#Experimental)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-mediawiki-project-and-a-date-range-returns-a-timeseries-of-the-top-100-editedpagesby-net-byt
      x-api-path-slug: metricseditedpagestopbynetbytesdifferenceprojecteditortypepagetypegranularitystartend-get
      parameters:
      - in: path
        name: editor-type
        description: If you want to filter by editor-type, use one of anonymous, group-bot
          (registeredaccounts belonging to the bot group), name-bot (registered accounts
          not belonging tothe bot group but having bot-like names) or user (registered
          account not in bot groupnor having bot-like name)
      - in: path
        name: end
        description: The date of the last day to include, in YYYYMMDD format
      - in: path
        name: granularity
        description: Time unit for the response data
      - in: path
        name: page-type
        description: If you want to filter by page-type, use one of content (edits
          on pages in contentnamespaces) or non-content (edits on pages in non-content
          namespaces)
      - in: path
        name: project
        description: The name of any Wikimedia project formatted like {language code}
      - in: path
        name: start
        description: The date of the first day to include, in YYYYMMDD format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/editors/aggregate/{project}/{editor-type}/{page-type}/{activity-level}/{granularity}/{start}/{end}:
    get:
      summary: Get editors counts for a project.
      description: |-
        Given a Mediawiki project and a date range, returns a timeseries of its editors counts.
        You can filter by editory-type (all-editor-types, anonymous, group-bot, name-bot, user),
        page-type (all-page-types, content or non-content) or activity-level (1..4-edits,
        5..24-edits, 25..99-edits or 100..-edits). You can choose between daily and monthly
        granularity as well.

        - Stability: [experimental](https://www.mediawiki.org/wiki/API_versioning#Experimental)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-mediawiki-project-and-a-date-range-returns-a-timeseries-of-its-editors-countsyou-can-filter-
      x-api-path-slug: metricseditorsaggregateprojecteditortypepagetypeactivitylevelgranularitystartend-get
      parameters:
      - in: path
        name: activity-level
        description: If you want to filter by activity-level, use one of 1
      - in: path
        name: editor-type
        description: If you want to filter by editor-type, use one of anonymous, group-bot
          (registeredaccounts belonging to the bot group), name-bot (registered accounts
          not belongingto the bot group but having bot-like names) or user (registered
          account not in botgroup nor having bot-like name)
      - in: path
        name: end
        description: The date of the last day to include, in YYYYMMDD format
      - in: path
        name: granularity
        description: The time unit for the response data
      - in: path
        name: page-type
        description: If you want to filter by page-type, use one of content (edits
          made in contentnamespaces) or non-content (edits made in non-content namespaces)
      - in: path
        name: project
        description: The name of any Wikimedia project formatted like {language code}
      - in: path
        name: start
        description: The date of the first day to include, in YYYYMMDD format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/editors/top-by-absolute-bytes-difference/{project}/{editor-type}/{page-type}/{granularity}/{start}/{end}:
    get:
      summary: Get top 100 editors by absolute bytes-difference.
      description: |-
        Given a Mediawiki project and a date range, returns a timeseries of the top 100 editors by
        absolute bytes-difference. You can filter by editor-type (all-editor-types, anonymous,
        group-bot, name-bot, user) or page-type (all-page-types, content or non-content). You can
        choose between daily and monthly granularity as well. The user_id returned is either the
        mediawiki user_id if user is registered, or his/her IP if the user is anonymous.

        - Stability: [experimental](https://www.mediawiki.org/wiki/API_versioning#Experimental)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-mediawiki-project-and-a-date-range-returns-a-timeseries-of-the-top-100-editors-byabsolute-by
      x-api-path-slug: metricseditorstopbyabsolutebytesdifferenceprojecteditortypepagetypegranularitystartend-get
      parameters:
      - in: path
        name: editor-type
        description: If you want to filter by editor-type, use one of anonymous, group-bot
          (registeredaccounts belonging to the bot group), name-bot (registered accounts
          not belonging tothe bot group but having bot-like names) or user (registered
          account not in bot groupnor having bot-like name)
      - in: path
        name: end
        description: The date of the last day to include, in YYYYMMDD format
      - in: path
        name: granularity
        description: Time unit for the response data
      - in: path
        name: page-type
        description: If you want to filter by page-type, use one of content (edits
          on pages in contentnamespaces) or non-content (edits on pages in non-content
          namespaces)
      - in: path
        name: project
        description: The name of any Wikimedia project formatted like {language code}
      - in: path
        name: start
        description: The date of the first day to include, in YYYYMMDD format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/editors/top-by-edits/{project}/{editor-type}/{page-type}/{granularity}/{start}/{end}:
    get:
      summary: Get top 100 editors by edits count.
      description: |-
        Given a Mediawiki project and a date range, returns a timeseries of the top 100 editors by
        edits count. You can filter by editor-type (all-editor-types, anonymous, group-bot,
        name-bot, user) or page-type (all-page-types, content or non-content). You can choose
        between daily and monthly granularity as well. The user_id returned is either the
        mediawiki user_id if user is registered, or his/her IP if the user is anonymous.

        - Stability: [experimental](https://www.mediawiki.org/wiki/API_versioning#Experimental)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-mediawiki-project-and-a-date-range-returns-a-timeseries-of-the-top-100-editors-byedits-count
      x-api-path-slug: metricseditorstopbyeditsprojecteditortypepagetypegranularitystartend-get
      parameters:
      - in: path
        name: editor-type
        description: If you want to filter by editor-type, use one of anonymous, group-bot
          (registeredaccounts belonging to the bot group), name-bot (registered accounts
          not belonging tothe bot group but having bot-like names) or user (registered
          account not in bot groupnor having bot-like name)
      - in: path
        name: end
        description: The date of the last day to include, in YYYYMMDD format
      - in: path
        name: granularity
        description: Time unit for the response data
      - in: path
        name: page-type
        description: If you want to filter by page-type, use one of content (edits
          on pages in contentnamespaces) or non-content (edits on pages in non-content
          namespaces)
      - in: path
        name: project
        description: The name of any Wikimedia project formatted like {language code}
      - in: path
        name: start
        description: The date of the first day to include, in YYYYMMDD format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/editors/top-by-net-bytes-difference/{project}/{editor-type}/{page-type}/{granularity}/{start}/{end}:
    get:
      summary: Get top 100 editors by net bytes-difference.
      description: |-
        Given a Mediawiki project and a date range, returns a timeseries of the top 100 editors by
        net bytes-difference. You can filter by editor-type (all-editor-types, anonymous, group-bot,
        name-bot, user) or page-type (all-page-types, content or non-content). You can choose
        between daily and monthly granularity as well. The user_id returned is either the mediawiki
        user_id if user is registered, or his/her IP if the user is anonymous.

        - Stability: [experimental](https://www.mediawiki.org/wiki/API_versioning#Experimental)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-mediawiki-project-and-a-date-range-returns-a-timeseries-of-the-top-100-editors-bynet-bytesdi
      x-api-path-slug: metricseditorstopbynetbytesdifferenceprojecteditortypepagetypegranularitystartend-get
      parameters:
      - in: path
        name: editor-type
        description: If you want to filter by editor-type, use one of anonymous, group-bot
          (registeredaccounts belonging to the bot group), name-bot (registered accounts
          not belonging tothe bot group but having bot-like names) or user (registered
          account not in bot groupnor having bot-like name)
      - in: path
        name: end
        description: The date of the last day to include, in YYYYMMDD format
      - in: path
        name: granularity
        description: Time unit for the response data
      - in: path
        name: page-type
        description: If you want to filter by page-type, use one of content (edits
          on pages in contentnamespaces) or non-content (edits on pages in non-content
          namespaces)
      - in: path
        name: project
        description: The name of any Wikimedia project formatted like {language code}
      - in: path
        name: start
        description: The date of the first day to include, in YYYYMMDD format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/edits/aggregate/{project}/{editor-type}/{page-type}/{granularity}/{start}/{end}:
    get:
      summary: Get edits counts for a project.
      description: |-
        Given a Mediawiki project and a date range, returns a timeseries of edits counts.
        You can filter by editors-type (all-editor-types, anonymous, bot, registered) and
        page-type (all-page-types, content or non-content). You can choose between daily and
        monthly granularity as well.

        - Stability: [experimental](https://www.mediawiki.org/wiki/API_versioning#Experimental)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-mediawiki-project-and-a-date-range-returns-a-timeseries-of-edits-countsyou-can-filter-by-edi
      x-api-path-slug: metricseditsaggregateprojecteditortypepagetypegranularitystartend-get
      parameters:
      - in: path
        name: editor-type
        description: If you want to filter by editor-type, use one of anonymous, group-bot
          (registeredaccounts belonging to the bot group), name-bot (registered accounts
          not belongingto the bot group but having bot-like names) or user (registered
          account not in botgroup nor having bot-like name)
      - in: path
        name: end
        description: The date of the last day to include, in YYYYMMDD format
      - in: path
        name: granularity
        description: The time unit for the response data
      - in: path
        name: page-type
        description: If you want to filter by page-type, use one of content (edits
          on pages in contentnamespaces) or non-content (edits on pages in non-content
          namespaces)
      - in: path
        name: project
        description: The name of any Wikimedia project formatted like {language code}
      - in: path
        name: start
        description: The date of the first day to include, in YYYYMMDD format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/legacy/pagecounts/aggregate/{project}/{access-site}/{granularity}/{start}/{end}:
    get:
      summary: Given a project and a date range, returns a timeseries of pagecounts.
        You can filter by access site (mobile or desktop) and you can choose between
        monthly, daily and hourly granularity as well.
      description: |-
        Given a project and a date range, returns a timeseries of pagecounts.
        You can filter by access site (mobile or desktop) and you can choose between monthly,
        daily and hourly granularity as well.

        - Stability: [experimental](https://www.mediawiki.org/wiki/API_versioning#Experimental)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-project-and-a-date-range-returns-a-timeseries-of-pagecountsyou-can-filter-by-access-site-mob
      x-api-path-slug: metricslegacypagecountsaggregateprojectaccesssitegranularitystartend-get
      parameters:
      - in: path
        name: access-site
        description: If you want to filter by access site, use one of desktop-site
          or mobile-site
      - in: path
        name: end
        description: The timestamp of the last hour/day/month to include, in YYYYMMDDHH
          format
      - in: path
        name: granularity
        description: The time unit for the response data
      - in: path
        name: project
        description: The name of any Wikimedia project formatted like {language code}
      - in: path
        name: start
        description: The timestamp of the first hour/day/month to include, in YYYYMMDDHH
          format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/pageviews/aggregate/{project}/{access}/{agent}/{granularity}/{start}/{end}:
    get:
      summary: Get pageview counts for a project.
      description: |-
        Given a date range, returns a timeseries of pageview counts. You can filter by project,
        access method and/or agent type. You can choose between daily and hourly granularity
        as well.

        - Stability: [stable](https://www.mediawiki.org/wiki/API_versioning#Stable)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-date-range-returns-a-timeseries-of-pageview-counts-you-can-filter-by-projectaccess-method-an
      x-api-path-slug: metricspageviewsaggregateprojectaccessagentgranularitystartend-get
      parameters:
      - in: path
        name: access
        description: If you want to filter by access method, use one of desktop, mobile-app
          or mobile-web
      - in: path
        name: agent
        description: If you want to filter by agent type, use one of user or spider
      - in: path
        name: end
        description: The timestamp of the last hour/day/month to include, in YYYYMMDDHH
          format
      - in: path
        name: granularity
        description: The time unit for the response data
      - in: path
        name: project
        description: If you want to filter by project, use the domain of any Wikimedia
          project,for example en
      - in: path
        name: start
        description: The timestamp of the first hour/day/month to include, in YYYYMMDDHH
          format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/pageviews/per-article/{project}/{access}/{agent}/{article}/{granularity}/{start}/{end}:
    get:
      summary: Get pageview counts for a page.
      description: |-
        Given a Mediawiki article and a date range, returns a daily timeseries of its pageview
        counts. You can also filter by access method and/or agent type.

        - Stability: [stable](https://www.mediawiki.org/wiki/API_versioning#Stable)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-mediawiki-article-and-a-date-range-returns-a-daily-timeseries-of-its-pageviewcounts-you-can-
      x-api-path-slug: metricspageviewsperarticleprojectaccessagentarticlegranularitystartend-get
      parameters:
      - in: path
        name: access
        description: If you want to filter by access method, use one of desktop, mobile-appor
          mobile-web
      - in: path
        name: agent
        description: If you want to filter by agent type, use one of user, bot or
          spider
      - in: path
        name: article
        description: The title of any article in the specified project
      - in: path
        name: end
        description: The date of the last day to include, in YYYYMMDD or YYYYMMDDHH
          format
      - in: path
        name: granularity
        description: The time unit for the response data
      - in: path
        name: project
        description: If you want to filter by project, use the domain of any Wikimedia
          project,for example en
      - in: path
        name: start
        description: The date of the first day to include, in YYYYMMDD or YYYYMMDDHH
          format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/pageviews/top-by-country/{project}/{access}/{year}/{month}:
    get:
      summary: Get pageviews by country and access method.
      description: |-
        Lists the pageviews to this project, split by country of origin for a given month.
        Because of privacy reasons, pageviews are given in a bucketed format, and countries
        with less than 100 views do not get reported.
        Stability: [experimental](https://www.mediawiki.org/wiki/API_versioning#Experimental)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: lists-the-pageviews-to-this-project-split-by-country-of-origin-for-a-given-monthbecause-of-privacy-r
      x-api-path-slug: metricspageviewstopbycountryprojectaccessyearmonth-get
      parameters:
      - in: path
        name: access
        description: If you want to filter by access method, use one of desktop, mobile-app
          or mobile-web
      - in: path
        name: month
        description: The month of the date for which to retrieve top countries, in
          MM format
      - in: path
        name: project
        description: If you want to filter by project, use the domain of any Wikimedia
          project,for example en
      - in: path
        name: year
        description: The year of the date for which to retrieve top countries, in
          YYYY format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/pageviews/top/{project}/{access}/{year}/{month}/{day}:
    get:
      summary: Get the most viewed articles for a project.
      description: |-
        Lists the 1000 most viewed articles for a given project and timespan (month or day).
        You can filter by access method.

        - Stability: [stable](https://www.mediawiki.org/wiki/API_versioning#Stable)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: lists-the-1000-most-viewed-articles-for-a-given-project-and-timespan-month-or-dayyou-can-filter-by-a
      x-api-path-slug: metricspageviewstopprojectaccessyearmonthday-get
      parameters:
      - in: path
        name: access
        description: If you want to filter by access method, use one of desktop, mobile-app
          or mobile-web
      - in: path
        name: day
        description: The day of the date for which to retrieve top articles, in DD
          format
      - in: path
        name: month
        description: The month of the date for which to retrieve top articles, in
          MM format
      - in: path
        name: project
        description: If you want to filter by project, use the domain of any Wikimedia
          project,for example en
      - in: path
        name: year
        description: The year of the date for which to retrieve top articles, in YYYY
          format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/registered-users/new/{project}/{granularity}/{start}/{end}:
    get:
      summary: Get newly registered users counts for a project.
      description: |-
        Given a Mediawiki project and a date range, returns a timeseries of its newly registered
        users counts. You can choose between daily and monthly granularity. The newly registered
        users value is computed with self-created users only, not auto-login created ones.

        - Stability: [experimental](https://www.mediawiki.org/wiki/API_versioning#Experimental)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-mediawiki-project-and-a-date-range-returns-a-timeseries-of-its-newly-registeredusers-counts-
      x-api-path-slug: metricsregisteredusersnewprojectgranularitystartend-get
      parameters:
      - in: path
        name: end
        description: The date of the last day to include, in YYYYMMDD format
      - in: path
        name: granularity
        description: The time unit for the response data
      - in: path
        name: project
        description: The name of any Wikimedia project formatted like {language code}
      - in: path
        name: start
        description: The date of the first day to include, in YYYYMMDD format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /metrics/unique-devices/{project}/{access-site}/{granularity}/{start}/{end}:
    get:
      summary: Get unique devices count per project
      description: |-
        Given a project and a date range, returns a timeseries of unique devices counts.
        You need to specify a project, and can filter by accessed site (mobile or desktop).
        You can choose between daily and hourly granularity as well.

        - Stability: [stable](https://www.mediawiki.org/wiki/API_versioning#Stable)
        - Rate limit: 100 req/s
        - License: Data accessible via this endpoint is available under the
          [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).
      operationId: given-a-project-and-a-date-range-returns-a-timeseries-of-unique-devices-countsyou-need-to-specify-a-
      x-api-path-slug: metricsuniquedevicesprojectaccesssitegranularitystartend-get
      parameters:
      - in: path
        name: access-site
        description: If you want to filter by accessed site, use one of desktop-site
          or mobile-site
      - in: path
        name: end
        description: The timestamp of the last day/month to include, in YYYYMMDD format
      - in: path
        name: granularity
        description: The time unit for the response data
      - in: path
        name: project
        description: If you want to filter by project, use the domain of any Wikimedia
          project,for example en
      - in: path
        name: start
        description: The timestamp of the first day/month to include, in YYYYMMDD
          format
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /transform/html/from/{from_lang}/to/{to_lang}:
    post:
      summary: Machine-translate content
      description: |-
        Fetches the machine translation for the posted content from the source
        to the destination language.

        Stability: [unstable](https://www.mediawiki.org/wiki/API_versioning#Unstable)
      operationId: fetches-the-machine-translation-for-the-posted-content-from-the-sourceto-the-destination-languagesta
      x-api-path-slug: transformhtmlfromfrom-langtoto-lang-post
      parameters:
      - in: path
        name: from_lang
        description: The source language code
      - in: formData
        name: html
        description: The HTML content to translate
      - in: path
        name: to_lang
        description: The target language code
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /transform/html/from/{from_lang}/to/{to_lang}/{provider}:
    post:
      summary: Machine-translate content
      description: |-
        Fetches the machine translation for the posted content from the source
        to the destination language.

        Stability: [unstable](https://www.mediawiki.org/wiki/API_versioning#Unstable)
      operationId: fetches-the-machine-translation-for-the-posted-content-from-the-sourceto-the-destination-languagesta
      x-api-path-slug: transformhtmlfromfrom-langtoto-langprovider-post
      parameters:
      - in: path
        name: from_lang
        description: The source language code
      - in: formData
        name: html
        description: The HTML content to translate
      - in: path
        name: provider
        description: The machine translation provider id
      - in: path
        name: to_lang
        description: The target language code
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /transform/list/languagepairs/:
    get:
      summary: Lists the language pairs supported by the back-end
      description: |-
        Fetches the list of language pairs the back-end service can translate

        Stability: [unstable](https://www.mediawiki.org/wiki/API_versioning#Unstable)
      operationId: fetches-the-list-of-language-pairs-the-backend-service-can-translatestability-unstablehttpswwwmediaw
      x-api-path-slug: transformlistlanguagepairs-get
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /transform/list/pair/{from}/{to}/:
    get:
      summary: Lists the tools available for a language pair
      description: |-
        Fetches the list of tools that are available for the given pair of languages.

        Stability: [unstable](https://www.mediawiki.org/wiki/API_versioning#Unstable)
      operationId: fetches-the-list-of-tools-that-are-available-for-the-given-pair-of-languagesstability-unstablehttpsw
      x-api-path-slug: transformlistpairfromto-get
      parameters:
      - in: path
        name: from
        description: The source language code
      - in: path
        name: to
        description: The target language code
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /transform/list/tool/{tool}/:
    get:
      summary: Lists the tools and language pairs available for the given tool category
      description: |-
        Fetches the list of tools and all of the language pairs it can translate

        Stability: [unstable](https://www.mediawiki.org/wiki/API_versioning#Unstable)
      operationId: fetches-the-list-of-tools-and-all-of-the-language-pairs-it-can-translatestability-unstablehttpswwwme
      x-api-path-slug: transformlisttooltool-get
      parameters:
      - in: path
        name: tool
        description: The tool category to list tools and language pairs for
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /transform/word/from/{from_lang}/to/{to_lang}/{word}:
    get:
      summary: Fetch the dictionary meaning of a word
      description: |-
        Fetches the dictionary meaning of a word from a language and displays
        it in the target language.

        Stability: [unstable](https://www.mediawiki.org/wiki/API_versioning#Unstable)
      operationId: fetches-the-dictionary-meaning-of-a-word-from-a-language-and-displaysit-in-the-target-languagestabil
      x-api-path-slug: transformwordfromfrom-langtoto-langword-get
      parameters:
      - in: path
        name: from_lang
        description: The source language code
      - in: path
        name: to_lang
        description: The target language code
      - in: path
        name: word
        description: The word to lookup
      responses:
        200:
          description: OK
      tags:
      - Wiki
  /transform/word/from/{from_lang}/to/{to_lang}/{word}/{provider}:
    get:
      summary: Fetch the dictionary meaning of a word
      description: |-
        Fetches the dictionary meaning of a word from a language and displays
        it in the target language.

        Stability: [unstable](https://www.mediawiki.org/wiki/API_versioning#Unstable)
      operationId: fetches-the-dictionary-meaning-of-a-word-from-a-language-and-displaysit-in-the-target-languagestabil
      x-api-path-slug: transformwordfromfrom-langtoto-langwordprovider-get
      parameters:
      - in: path
        name: from_lang
        description: The source language code
      - in: path
        name: provider
        description: The dictionary provider id
      - in: path
        name: to_lang
        description: The target language code
      - in: path
        name: word
        description: The word to lookup
      responses:
        200:
          description: OK
      tags:
      - Wiki