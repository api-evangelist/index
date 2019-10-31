swagger: "2.0"
x-collection-name: TradeStation
x-complete: 1
info:
  title: Tradestation API
  description: this-document-describes-the-resources-that-make-up-the-official-tradestationapi--if-you-have-any-problems-or-requests-please-contact-supportmailtowebapitradestation-com-overviewthe-tradestation-api-is-reachable-at-the-baseurlhttpsapi-tradestation-comv2current-versionthe-latest-version-is-20160101-but-currently-we-are-in-transition-so-bydefault-all-requests-receive-the-20101026-version-for-backwards-compatibility-always-explicitly-request-this-version-by-adding-the-apiversionquerystring-parameter-as-shown-belowhttpsapi-tradestation-comv2dataquotemsftapiversion20160101note-this-will-ensure-your-application-will-not-be-broken-when-we-deprecatethe-20101026-version-in-favor-of-20160101-or-newer-versions-sim-vs-livewe-also-offer-a-simulatorsim-api-for-paper-trading-that-is-identicalto-the-live-api-in-all-ways-except-it-uses-fake-trading-accounts-seeded-withfake-money-and-orders-are-not-actually-executed--only-simulated-executionsoccur-with-instant-fills-to-access-the-sim-environment-you-must-change-your-baseurl-tohttpssimapi-tradestation-comv2warning-tradestation-is-not-liable-for-mistakes-made-by-applicationsthat-allow-users-to-switch-between-sim-and-live-environments--why-offer-a-simulatortransactional-api-calls-such-as-order-execution-offers-users-or-applicationsthe-ability-to-experiment-within-a-simulated-trading-system-so-that-realaccounts-and-money-are-not-affected-and-trades-are-not-actually-executed-other-potential-usecases-learning-how-to-use-applications-via-paper-trading--exploring-tradestation-api-behavior-without-financial-ramifications-testing-apps-and-websites-before-making-them-live-to-customers-enabling-users-to-trybeforetheybuy-with-apps-that-use-the-tradestation-api-hosting-trading-competitions-or-gameshttp-requestsall-api-access-is-over-https-and-accessed-from-the-httpsapi-tradestation-com-all-data-is-sent-and-received-as-json-with-some-limited-support-for-xml-example-requestcurl-i-httpsapi-tradestation-comv2dataquotemsftapiversion20160101http1-1-200-okcachecontrol-privatecontentlength-1545contenttype-applicationdefaultjson-charsetutf8accesscontrolalloworigin-apiversion-20160101date-wed-30-nov-2016-015145-gmt---json----common-conventions-blank-fields-may-either-be-included-as-null-or-omitted-so-please-support-both--all-timestamps-are-returned-in-epoch-timehttpsen-wikipedia-orgwikiunix-time-format-unless-stated-otherwise-http-streamingthe-tradestation-api-offers-http-streaming-responses-for-some-specializedresources-including-intraday-barcharts-quote-changes-and-quote-snapshots-these-streams-conform-to-rfc2616-for-http1-1-streaming-with-some-slightmodifications--the-http-streaming-mechanism-keeps-a-request-open-indefinitely---it-never-terminates-the-request-or-closes-the-connection-even-after-the-server-pushes-data-to-the-client---this-mechanism-significantly-reduces-the-network-latency-because-the-client-and-the-server-do-not-need-to-open-and-close-the-connection--the-basic-life-cycle-of-an-application-using-http-streaming-is-as-follows-1---the-client-makes-an-initial-request-and-then-waits-for-a-----response--2---the-server-defers-the-response-to-a-poll-request-until-an-update-----is-available-or-until-a-particular-status-or-timeout-has-----occurred--3---whenever-an-update-is-available-the-server-sends-it-back-to-the-----client-as-a-part-of-the-response--4---the-data-sent-by-the-server-does-not-terminate-the-request-or-the-----connection---the-server-returns-to-step-3--the-http-streaming-mechanism-is-based-on-the-capability-of-the-server-to-send-several-pieces-of-information-in-the-same-response-without-terminating-the-request-or-the-connection-source-rfc6202-page-7httpstools-ietf-orghtmlrfc6202page7-http-streaming-resources-are-identified-under-in-this-documentation-as-suchall-other-resources-conform-to-the-http-request-pattern-instead-the-http-streaming-response-is-returned-with-the-following-headers----transferencoding-chunked--contenttype-applicationvnd-tradestation-streamsjson--note-the-contentlength-header-is-typically-omitted-since-the-responsebody-size-is-unknown-streams-consist-of-a-series-of-chunks-that-contain-individual-json-objectsto-be-parsed-separately-rather-than-as-a-whole-response-body-one-unique-thing-about-tradestations-http-streams-is-they-also-can-terminateunlike-a-canonical-http1-1-stream-streams-terminate-with-a-nonjson-string-prefixed-with-one-of-the-following---end---errorin-the-case-of-error-it-will-often-be-followed-by-an-error-message-likeerror--a-timeout-occurred-after-waiting-15000msin-either-case-the-http-client-must-terminate-the-http-stream-and-end-thehttp-request-lifetime-as-a-result-of-these-messages--in-the-case-of-errorthe-client-application-may-add-a-delay-before-rerequesting-the-http-stream--how-to-handle-http-chunked-encoded-streamshealthy-chunkedencoded-streams-emit-variable-length-chunks-that-containparsable-json-for-exampleget-httpssim-api-tradestation-comv2streambarchartdji1minute1226201601242017access-tokenhttp1-1-200-okdate-wed-14-jun-2017-011736-gmtcontenttype-applicationvnd-tradestation-streamsjsontransferencoding-chunkedconnection-keepaliveaccesscontrolalloworigin-cachecontrol-private114close19956-09downticks26downvolume940229high19961-77low19943-46open19943-46status13timestampdate1482849060000totalticks59totalvolume3982533unchangedticks0unchangedvolume0upticks33upvolume3042304openinterest0112close19950-82downticks32downvolume440577high19959-15low19947-34open19955-64status13timestampdate1482849120000totalticks60totalvolume761274unchangedticks0unchangedvolume0upticks28upvolume320697openinterest0endtypically-this-will-stream-forever-unless-a-network-interruption-or-servicedisruption-occurs--it-is-up-to-the-client-to-properly-handle-stream-lifetimeand-connection-closing--how-to-parse-json-chunksin-order-to-process-these-chunks-api-consumers-should-first-read-theresponse-buffer-then-dechunk-the-plaintext-strings-and-finally-identifynew-json-objects-by-applying-tokenizing-techniques-to-the-resulting-textstream-using-either-a-streaming-json-parser-regex-a-lexerparser-orbruteforce-string-indexing-logic-a-simple-but-effective-technique-is-after-dechunking-to-simply-parse-basedupon-the-n-newline-character-delimiter-written-to-the-end-of-eachjson-object--however-a-more-robust-solution-is-less-likely-to-break-later--variable-length-json-chunkingas-a-developer-be-careful-with-how-you-parse-http-streams-because-theapis-or-intermediate-proxies-may-chunk-json-objects-many-different-ways--using-http-streaming-several-application-messages-can-be-sent-within-a-single-http-response---the-separation-of-the-response-stream-into-application-messages-needs-to-be-performed-at-the-application-level-and-not-at-the-http-level---in-particular-it-is-not-possible-to-use-the-http-chunks-as-application-message-delimiters-since-intermediate-proxies-might-rechunk-the-message-stream-for-example-by-combining-different-chunks-into-a-longer-one---this-issue-does-not-affect-the-http-long-polling-technique-which-provides-a-canonical-framing-technique-each-application-message-can-be-sent-in-a-different-http-response-source-rfc6202-section-3-2httpstools-ietf-orghtmlrfc6202section3-2translation-be-prepared-for-json-objects-that-span-chunks--you-may-seechunks-with-varying-numbers-of-json-objects-including-exactly-1-json-object-per-chunk-at-least-1-json-object-per-chunk-1-json-object-split-across-2-or-more-chunksexample-of-2-json-objects-in-1-chunkget-httpssim-api-tradestation-comv2streambarchartdji1minute1226201601242017access-tokenhttp1-1-200-okdate-wed-14-jun-2017-011736-gmtcontenttype-applicationvnd-tradestation-streamsjsontransferencoding-chunkedconnection-keepaliveaccesscontrolalloworigin-cachecontrol-private22dclose19956-09downticks26downvolume940229high19961-77low19943-46open19943-46status13timestampdate1482849060000totalticks59totalvolume3982533unchangedticks0unchangedvolume0upticks33upvolume3042304openinterest0close19950-82downticks32downvolume440577high19959-15low19947-34open19955-64status13timestampdate1482849120000totalticks60totalvolume761274unchangedticks0unchangedvolume0upticks28upvolume320697openinterest0endexample-of-1-json-objects-split-across-2-chunksget-httpssim-api-tradestation-comv2streambarchartdji1minute1226201601242017access-tokenhttp1-1-200-okdate-wed-14-jun-2017-011736-gmtcontenttype-applicationvnd-tradestation-streamsjsontransferencoding-chunkedconnection-keepaliveaccesscontrolalloworigin-cachecontrol-private40close71-65downticks45downvolume5406high71-67loc2w71-65open71-66status13timestampdate1497016260000totalticks77totalvolume17270unchangedticks0unchangedvolume0upticks32upvolume11864openinterest0endthis-is-allowed-by-the-http1-1-specification-but-can-be-confusing-or-leadto-bugs-in-client-applications-if-you-try-to-depend-parsing-json-alongthe-http-chunkboundaries-because-even-if-it-works-during-testing-later-ifusers-connect-from-a-different-network-it-may-change-the-chunking-behavior-for-example-if-you-are-at-a-coffee-shop-with-wifi-which-employs-anhttp-proxy-then-it-may-buffer-the-stream-and-change-the-chunking-boundaryfrom-1-json-object-per-chunk-to-splitting-each-json-object-across-2-or-3-in-fact-the-http1-1-spec-clearly-advises-developers-of-proxies-to-alwaysrechunk-http-streams-so-this-is-almost-a-guarantee-to-happen-in-the-wild-http-streaming-api-consumers-should-be-prepared-to-support-all-variations-rate-limitingthe-tradestation-api-rate-limits-on-the-number-of-requests-a-given-user-client-can-make-to-the-api-in-order-to-ensure-fairness-between-users-andprevent-abuse-to-our-network--each-api-key-is-allocated-quota-settings-uponcreation--these-settings-are-applied-on-a-peruser-basis--if-the-quota-isexceeded-an-http-response-of-403-quota-exceeded-will-bereturned--quotas-are-reset-on-a-5minute-interval-based-on-when-the-userissued-the-first-request--resource-categoriesthe-rate-limit-applies-to-the-following-resourcecategories-resourcecategory------------------------------quota--interval--------accounts---------------------------------------250----5minute--order-details----------------------------------250----5minute--balances---------------------------------------250----5minute--positions--------------------------------------250----5minute--data-quotes------------------------------------250----5minute--quote-change-stream----------------------------500----5minute--quote-snapshot-stream--------------------------500----5minute--barchart-stream--------------------------------500----5minute--tickbar-stream---------------------------------500----5minute--intervalsquotas-have-windows-that-last-for-a-limited-time-intervalgenerally-5minutes--once-the-user-has-exceeded-the-maximum-request-countall-future-requests-will-fail-with-a-403-error-until-the-interval-expires-rate-limit-intervals-do-not-slide-based-upon-the-number-of-requests-they-arefixed-at-a-point-in-time-starting-from-the-very-first-request-for-thatcategory-of-resource---after-the-interval-expires-the-cycle-willstart-over-at-zero-and-the-user-can-make-more-requests--example-aa-user-logs-into-the-tradestation-webapi-with-your-application-and-issues-arequest-to-v2elitetraderaccounts--as-a-result-the-requestquota-is-incremented-by-one-for-the-accounts-resourcecategory--the-userthen-issues-250-more-requests-immediately-to-v2elitetraderaccounts-the-last-request-fails-with-403-quota-exceeded--all-subsequent-requestscontinue-to-fail-until-the-5minute-interval-expires-from-the-time-of-thevery-first-request--example-ba-user-logs-into-the-tradestation-webapi-with-your-application-and-issues-arequest-to-v2dataquoteibmnflxmsftamznaapl--as-a-result-therequest-quota-is-incremented-by-one-for-the-data-quotesresourcecategory--the-user-then-immediately-issues-the-same-request-250-moretimes--the-last-request-fails-with-403-quota-exceeded--allsubsequent-requests-continue-to-fail-until-the-5minute-interval-expiresfrom-the-time-of-the-first-request-example-throttled-requestget-httpsapi-tradestation-comv2dataquotesibmnflxmsftamznaapl-http1-1host-api-tradestation-comauthorization-bearer-ee45vkdqsnlbcmi0q2rqti82sfdmsve0sxmyofo5z3dzvzdzdkaccept-applicationjsonexample-failed-responsehttp1-1-403-quota-exceededcontentlength-15server-microsoftiis7-5xaspnetversion-4-0-30319date-tue-06-dec-2011-205032-gmthtmlbodyquota-exceededbodyhtml
  termsOfService: http://elasticbeanstalk-us-east-1-525856068889.s3.amazonaws.com/wp-content/uploads/2014/03/Guidelines_For_Acceptance.pdf
  contact:
    name: TradeStation API Team
    url: https://developer.tradestation.com/webapi
    email: webapi@tradestation.com
  version: 1.0.0
host: api.tradestation.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /data/symbol/{symbol}:
    get:
      summary: Get Symbol Info
      description: |-
        Finds the given symbol and returns a collection of fields describing the
        symbol, its origin exchange, and other pertinant information.
      operationId: getSymbol
      x-api-path-slug: datasymbolsymbol-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: symbol
        description: Symbol to lookup
      responses:
        200:
          description: Successful response
      tags:
      - Symbol
      - Info
  /data/symbols/suggest/{text}:
    get:
      summary: Suggest Symbols
      description: |-
        Suggests symbols semantically based upon partial input of symbol name,
        company name, or description
      operationId: suggestsymbols
      x-api-path-slug: datasymbolssuggesttext-get
      parameters:
      - in: query
        name: $filter
        description: An OData filter to apply to the results
      - in: query
        name: $top
        description: The top number of results to return
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: text
        description: Symbol text for suggestion
      responses:
        200:
          description: Successful response
      tags:
      - Suggest
      - Symbols
  /data/symbols/search/{criteria}:
    get:
      summary: Search for Symbols
      description: |-
        Searches symbols based upon input criteria including Name, Category and
        Country.
      operationId: searchSymbols
      x-api-path-slug: datasymbolssearchcriteria-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: criteria
        description: 'Criteria are represented as Key/value pairs (`&` separated):`N`:
          Name of Symbol'
      responses:
        200:
          description: Successful response
      tags:
      - SearchSymbols
  /data/quote/{symbols}:
    get:
      summary: Get Quote
      description: Gets the latest Level2 Quote for the given Symbol
      operationId: getQuotes
      x-api-path-slug: dataquotesymbols-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: symbols
        description: 1 or more Symbol Names (comma-separated)
      responses:
        200:
          description: Successful response
      tags:
      - Quote
  /stream/quote/changes/{symbols}:
    get:
      summary: Stream Quote Changes
      description: |-
        Streams the latest Quote information for the given Symbols. The first chunk in the stream is a full quote snapshot - subsequent chunks only contain fields of the quote object that have changed since the last chunk.

        An invalid symbol name will result in a response of this form - {"Symbol":"BADEXAMPLESYMBOL","Error":"FAILED, EX_INVALID_SYMBOL"}

        If the user is not entitled for the symbol requested, response will be of this form - {"Symbol":"EXAMPLESYMBOL","Error":"FAILED, EX_NOT_ENTITLED"}
      operationId: streamQuotesChanges
      x-api-path-slug: streamquotechangessymbols-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: symbols
        description: 1 or more Symbol Names (comma-separated)
      - in: header
        name: Transfer-Encoding
        description: a header with the value of `Chunked` must be passed to streaming
          resources
      responses:
        200:
          description: Successful response
      tags:
      - Stream
      - Quote
      - Changes
  /stream/quote/snapshots/{symbols}:
    get:
      summary: Stream Quote Snapshots
      description: |-
        Streams the latest Quote for the given Symbols. Each chunk is a full quote object.

        An invalid symbol name will result in a response of this form - {"Symbol":"BADSYMBOLEXAMPLE","Error":"FAILED, EX_INVALID_SYMBOL"}

        If the user is not entitled for the symbol requested, response will be of this form - {"Symbol":"EXAMPLESYMBOL","Error":"FAILED, EX_NOT_ENTITLED"}
      operationId: streamQuotesSnapshots
      x-api-path-slug: streamquotesnapshotssymbols-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: symbols
        description: 1 or more Symbol Names (comma-separated)
      responses:
        200:
          description: Successful response
      tags:
      - Stream
      - Quote
      - Snapshots
  /stream/barchart/{symbol}/{interval}/{unit}/{startDate}:
    get:
      summary: Stream BarChart - Starting on Date
      description: Streams barchart data starting from startDate, each bar filling
        quantity of unit.
      operationId: streamBarchartsFromStartDate
      x-api-path-slug: streambarchartsymbolintervalunitstartdate-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: interval
        description: Interval that each bar will consist of
      - in: query
        name: SessionTemplate
        description: United States (US) stock market session templates, that extend
          bars returned to include those outside of the regular trading session
      - in: path
        name: startDate
        description: The starting date to begin streaming bars from
      - in: path
        name: symbol
        description: A Symbol Name
      - in: path
        name: unit
        description: Unit of time for each bar interval
      responses:
        200:
          description: Successful response
      tags:
      - Stream
      - BarChart
      - '-'
      - Starting
      - "On"
      - Date
  /stream/barchart/{symbol}/{interval}/{unit}/{startDate}/{endDate}:
    get:
      summary: Stream BarChart - Date Range
      description: Streams barchart data starting from startDate to end date, each
        bar filling interval of unit.
      operationId: streamBarchartsFromStartDateToEndDate
      x-api-path-slug: streambarchartsymbolintervalunitstartdateenddate-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: endDate
        description: The ending date for bars streamed
      - in: path
        name: interval
        description: Interval that each bar will consist of
      - in: query
        name: SessionTemplate
        description: United States (US) stock market session templates, that extend
          bars returned to include those outside of the regular trading session
      - in: path
        name: startDate
        description: The starting date to begin streaming bars from
      - in: path
        name: symbol
        description: A Symbol Name
      - in: path
        name: unit
        description: Unit of time for each bar interval
      responses:
        200:
          description: Successful response
      tags:
      - Stream
      - BarChart
      - '-'
      - Date
      - Range
  /stream/barchart/{symbol}/{interval}/{unit}/{barsBack}/{lastDate}/...:
    get:
      summary: Stream BarChart - Bars Back
      description: Streams barchart data starting from a number of bars back from
        last date, each bar filling interval of unit.
      operationId: streamBarchartsBarsBack
      x-api-path-slug: streambarchartsymbolintervalunitbarsbacklastdate----get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: barsBack
        description: The number of bars to stream, going back from time 00:00:00 of
          the day specified in lastDate
      - in: path
        name: interval
        description: Interval that each bar will consist of
      - in: path
        name: lastDate
        description: The date to use as the end point when getting bars back
      - in: query
        name: SessionTemplate
        description: United States (US) stock market session templates, that extend
          bars returned to include those outside of the regular trading session
      - in: path
        name: symbol
        description: A Symbol Name
      - in: path
        name: unit
        description: Unit of time for each bar interval
      responses:
        200:
          description: Successful response
      tags:
      - Stream
      - BarChart
      - '-'
      - Bars
      - Back
  /stream/barchart/{symbol}/{interval}/{unit}:
    get:
      summary: Stream BarChart - Days Back
      description: Streams barchart data starting from a number of days back from
        last date, each bar filling interval of unit.
      operationId: streamBarchartsDaysBack
      x-api-path-slug: streambarchartsymbolintervalunit-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: query
        name: daysBack
        description: The number of bars to stream, going back from time 00:00:00 of
          the day specified in lastDate
      - in: path
        name: interval
        description: Interval that each bar will consist of
      - in: query
        name: lastDate
        description: The date to use as the end point when getting days back
      - in: query
        name: SessionTemplate
        description: United States (US) stock market session templates, that extend
          bars returned to include those outside of the regular trading session
      - in: path
        name: symbol
        description: A Symbol Name
      - in: path
        name: unit
        description: Unit of time for each bar interval
      responses:
        200:
          description: Successful response
      tags:
      - Stream
      - BarChart
      - '-'
      - Days
      - Back
  /stream/tickbars/{symbol}/{interval}/{barsBack}:
    get:
      summary: Stream Tick Bars
      description: Streams tick bars data from a number of bars back, each bar returned
        separated by interval number of ticks.
      operationId: streamTickBars
      x-api-path-slug: streamtickbarssymbolintervalbarsback-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: barsBack
        description: The number of bars to stream, going back from current time
      - in: path
        name: interval
        description: Interval for each bar returned (in ticks)
      - in: path
        name: symbol
        description: A Symbol Name
      responses:
        200:
          description: Successful response
      tags:
      - Stream
      - Tick
      - Bars
  /data/symbollists:
    get:
      summary: Get all Symbol Lists
      description: Gets a list of all Symbol Lists
      operationId: getSymbolLists
      x-api-path-slug: datasymbollists-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      responses:
        200:
          description: Successful response
      tags:
      - Symbol
      - Lists
  /data/symbollists/{symbol_list_id}:
    get:
      summary: Get Symbol List
      description: Gets a specific Symbol List
      operationId: getSymbolListByID
      x-api-path-slug: datasymbollistssymbol-list-id-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: symbol_list_id
        description: A valid Symbol List ID
      responses:
        200:
          description: Successful response
      tags:
      - Symbol
      - List
  /data/symbollists/{symbol_list_id}/symbols:
    get:
      summary: Get Symbols in a Symbol List
      description: Gets the Symbols for a specific Symbol List
      operationId: getSymbolListSymbolsByID
      x-api-path-slug: datasymbollistssymbol-list-idsymbols-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: symbol_list_id
        description: A valid Symbol List ID
      responses:
        200:
          description: Successful response
      tags:
      - Symbols
      - In
      - Symbol
      - List
  /users/{user_id}/accounts:
    get:
      summary: Get User Accounts
      description: Returns all accounts for the given user
      operationId: getAccountsByUserID
      x-api-path-slug: usersuser-idaccounts-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: user_id
        description: User ID for Accounts Lookup
      responses:
        200:
          description: Successful response
      tags:
      - User
      - Accounts
  /accounts/{account_keys}/balances:
    get:
      summary: Get Account Balances
      description: Returns the Balance for the given accounts
      operationId: getBalancesByAccounts
      x-api-path-slug: accountsaccount-keysbalances-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: account_keys
        description: 1 or more Account Keys
      responses:
        200:
          description: Successful response
      tags:
      - Account
      - Balances
  /accounts/{account_keys}/positions:
    get:
      summary: Get Account Positions
      description: Returns the Positions for the given accounts
      operationId: getPositionsByAccounts
      x-api-path-slug: accountsaccount-keyspositions-get
      parameters:
      - in: query
        name: $filter
        description: An OData v2
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: account_keys
        description: 1 or more Account Keys
      responses:
        200:
          description: Successful response
      tags:
      - Account
      - Positions
  /accounts/{account_keys}/orders:
    get:
      summary: Get Account Orders
      description: |-
        Returns the Orders for the given accounts sorted descending, most recent order first.

        #### Stateless Connection
        Since the web-API provides a stateless connection, it only supports fetching the current state of Orders. If it is needed to display the intermediate state changes, it should be executed at client level.
      operationId: getOrdersByAccounts
      x-api-path-slug: accountsaccount-keysorders-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: account_keys
        description: 1 or more Account Keys
      - in: query
        name: pageNum
        description: Conveys the page number to return, given a set of orders and
          a page size
      - in: query
        name: pageSize
        description: Conveys the number of order items to return in the request
      - in: query
        name: since
        description: Start Date from which to pull older orders
      responses:
        200:
          description: Successful response
      tags:
      - Account
      - Orders
  /orders/confirm:
    post:
      summary: Confirm Order
      description: |-
        Returns estimated cost and commission information for an order without the order actually being placed. The fields that are returned in the response depend on the order type.
        The following shows the different fields that will be returned.

        **Base Confirmation**  (All confirmations will have these fields)
        * Route
        * Duration
        * Account
        * SummaryMessage
        * OrderConfirmId

        **Equity Confirmation** (Base Confirmation fields + the following)
        * EstimatedPrice
        * EstimatedPriceDisplay
        * EstimatedCost
        * EstimatedCostDisplay
        * EstimatedCommission
        * EstimatedCommissionDisplay
        * DebitCreditEstimatedCost
        * DebitCreditEstimatedCostDisplay

        **Forex Confirmation** (Base Confirmation fields + the following)
        * BaseCurrency
        * CounterCurrency
        * InitialMarginDisplay

        **Futures Confirmation** (Base Confirmation fields + the following)
        * ProductCurrency
        * AccountCurrency
        * EstimatedCost
        * EstimatedPrice
        * EstimatedPriceDisplay
        * InitialMarginDisplay
        * EstimatedCommission
        * EstimatedCommissionDisplay
      operationId: postOrderConfirm
      x-api-path-slug: ordersconfirm-post
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Confirm
      - Order
  /orders:
    post:
      summary: Submit Order
      description: Submits 1 or more orders
      operationId: postOrder
      x-api-path-slug: orders-post
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Submit
      - Order
  /orders/{order_id}:
    delete:
      summary: Cancel Order
      description: Cancels an open order. You cannot cancel an order that has been
        filled.
      operationId: cancelOrder
      x-api-path-slug: ordersorder-id-delete
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: order_id
        description: An existing Order ID
      responses:
        200:
          description: Successful response
      tags:
      - Cancel
      - Order
    put:
      summary: Update Order
      description: |-
        Updates (Cancels & Replaces) an open order. You cannot update an order
        that has been filled.

        Rules:

         | Original order type              | Fields to update                 | Can only change order type to |
         | -------------------------------- | -------------------------------- | ----------------------------- |
         | Limit Orders                     | Quantity, Stop Price             | Market                        |
         | Stop Orders                      | Quantity, Stop Price             | Market                        |
         | Stop Limit Orders                | Quantity, Stop Price, Stop Limit | Market                        |
         | Stop Market Trailing Stop Orders | Quantity                         | Market                        |
         | Trailing Stop Orders             | Offset type and value            | Market                        |
      operationId: cancelReplaceOrder
      x-api-path-slug: ordersorder-id-put
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: order_id
        description: An existing Order ID
      responses:
        200:
          description: Successful response
      tags:
      - Order
  /orders/groups/confirm:
    post:
      summary: Confirm Group Order
      description: |-
        Returns estimated cost and commission information for a group of orders (OCO, BRK) without the orders actually being placed

        **Base Confirmation**  (All confirmations will have these fields)
        * Route
        * Duration
        * Account
        * SummaryMessage
        * OrderConfirmId

        **Equity Confirmation** (Base Confirmation fields + the following)
        * EstimatedPrice
        * EstimatedPriceDisplay
        * EstimatedCost
        * EstimatedCostDisplay
        * EstimatedCommission
        * EstimatedCommissionDisplay

        **Forex Confirmation** (Base Confirmation fields + the following)
        * BaseCurrency
        * CounterCurrency
        * InitialMarginDisplay

        **Futures Confirmation** (Base Confirmation fields + the following)
        * ProductCurrency
        * AccountCurrency
        * EstimatedCost
        * EstimatedPrice
        * EstimatedPriceDisplay
        * InitialMarginDisplay
        * EstimatedCommission
        * EstimatedCommissionDisplay
      operationId: postOrderGroupsConfirm
      x-api-path-slug: ordersgroupsconfirm-post
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Confirm
      - Group
      - Order
  /orders/groups:
    post:
      summary: Submit Group Order
      description: "Submits a group order such as Bracket and OCO Orders.\n\n####
        Order Cancels Order (OCO)\nAn OCO order is a group of orders whereby if one
        of the orders is filled\nor partially-filled, then all of the other orders
        in the group are\ncancelled.\n\n#### Bracket OCO Orders\nA bracket order is
        a special instance of an OCO (Order Cancel Order).\nBracket orders are used
        to exit an existing position. They are designed\nto limit loss and lock in
        profit by ???bracketing??? an order with a\nsimultaneous stop and limit order.\n\nBracket
        orders are limited so that the orders are all for the same\nsymbol and are
        on the same side of the market (either all to sell or\nall to cover), and
        they are restricted to closing transactions.\n\nThe reason that they follow
        these rules is because the orders need to be\nable to auto decrement when
        a partial fill occurs with one of the orders.\nFor example, if the customer
        has a sell limit order for 1000 shares and\na sell stop order for 1000 shares,
        and the limit order is partially\nfilled for 500 shares, then the customer
        would want the stop to remain\nopen, but it should automatically decrement
        the order to 500 shares to\nmatch the remaining open position.\n\n### Errors\nWhen
        a submitted order fails, it can be seen in two different ways:\n-\tImmediately
        rejected during submit to the Orders API with a 400 HTTP status code.\n-\tAccepted
        by the API with a 200 HTTP status code, but you will see the order with a
        status of ???REJ??? (rejected) when you fetch the Order from the /v2/accounts/{id}/orders
        API\n\n#### NOTE\nWhen a group order is submitted, the order execution system
        treats each sibling order as an individual order. Thus, the system does not
        validate that each order has the same Quantity, and currently it is not able
        to update a bracket order as one transaction, instead you must update each
        order within a bracket.\n\nIn order to prevent errors, please validate the
        data on the client side."
      operationId: postOrderGroup
      x-api-path-slug: ordersgroups-post
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Submit
      - Group
      - Order
  /orderexecution/activationtriggers:
    get:
      summary: Request Available Activation Triggers
      description: To place orders with activation triggers, a valid TriggerKey must
        be sent with the order.  This resource provides the available trigger methods
        with their corresponding key.
      operationId: getActivationTriggers
      x-api-path-slug: orderexecutionactivationtriggers-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      responses:
        200:
          description: Successful response
      tags:
      - Request
      - Available
      - Activation
      - Triggers