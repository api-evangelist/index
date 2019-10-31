swagger: "2.0"
x-collection-name: Rite Kit
x-complete: 1
info:
  title: Rite Kit
  description: ritekit-api-is-based-on-rest-principles-authentication-uses-standard-oauth-2-0-processgetting-started1--sign-up-for-ritekithttpsritekit-com1--go-to-developer-dashboardhttpsritekit-comdeveloperdashboard1--click-create-a-token-button-to-get-your-client-id-and-client-secret1--study-the-documentation-below-for-more-info-on-oauth-go-to-httpoauth-net1--when-you-reach-your-free-limit-of-calls-per-month-upgrade-to-paid-tiershttpsritekit-comdeveloper-options-for-authorizing-api-calls-a-using-client-id-directlyyou-can-directly-connect-to-our-api-using-your-client-id-by-sending-it-as-a-get-query-parameter--this-option-is-simple-no-need-for-oauth-but-it-should-be-used-only-in-case-the-client-id-is-not-exposed-publicly-get--httpsapi-ritekit-comv1statsmultiplehashtagstagsphpclient-id292c6912e7710c838347ae178b4a-b-using-access-token-oauth-2-0once-you-have-valid-access-token-you-can-access-our-api-by-sending-the-token-in-the-authorization-header-bearer-or-as-a-query-access-token--see-the-oauth-2-0-section-to-learn-how-to-get-access-token-and-keep-refreshing-it-authorization-bearer-xxxxorget--httpsapi-ritekit-comv1statsmultiplehashtagstagsphpaccess-token292c6912e7710c838347ae178b4a-oauth-2-0oauthschemahttpscdn-ritekit-comassetsmedia1oauthsimple-png-get-access-tokenuse-your-client-credentials-to-get-the-token-post---httpsritekit-comoauthtoken-----------grant-typeclient-credentials-----------client-idclient-id-----------client-secretclient-secret-----------scopedata-required-grant-type--client-credentials-required-client-id-client-id-required-client-secret-client-secret-required-always-use-scopedata-response--------access-token292c6912e7710c838347ae178b4a--------token-typebearer--------expires-in-3600--------refresh-token292c6912e7710c838347ae178b4a-----refresh-tokenevery-access-token-has-a-lifetime--you-can-use-refresh-token-to-request-a-new-access-token-post---httpsritekit-comoauthtoken-----------grant-typerefresh-token-----------refresh-tokenrefresh-token-----------client-idclient-id-----------scopedata-required-grant-type--refresh-token-required-refresh-token--refresh-token-the-refresh-token-you-got-from-the-expired-token-required-client-id-client-id-required-client-secret-client-secret-required-scope-always-use-scopedata-response--------access-token292c6912e7710c838347ae178b4a--------token-typebearer--------expires-in-3600--------refresh-token292c6912e7710c838347ae178b4a----
  version: 1.0.0
host: api.ritekit.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/emoji/auto-emojify:
    get:
      summary: Auto-Emojify
      description: Returns text of the post with emoji added
      operationId: v1.emoji.auto_emojify.get
      x-api-path-slug: v1emojiautoemojify-get
      parameters:
      - in: query
        name: text
        description: Text of the post
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/emoji/suggestions:
    get:
      summary: Emoji Suggestions
      description: Returns list of emoji suggestions for a given text of the post
      operationId: v1.emoji.suggestions.get
      x-api-path-slug: v1emojisuggestions-get
      parameters:
      - in: query
        name: text
        description: Text of the post
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/images/animate:
    get:
      summary: Animate Image
      description: Returns URL of an animated GIF.
      operationId: v1.images.animate.get
      x-api-path-slug: v1imagesanimate-get
      parameters:
      - in: query
        name: type
        description: URL of the company
      - in: query
        name: url
        description: URL of the company
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/images/logo:
    get:
      summary: Company Logo
      description: Returns a company logo based on website domain. If the logo is
        not in our database yet, it will be extracted from the site on the fly. White
        logo background is automatically removed to make the logo look better on color
        backgrounds.
      operationId: v1.images.logo.get
      x-api-path-slug: v1imageslogo-get
      parameters:
      - in: query
        name: domain
        description: URL of the company
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/images/quote:
    get:
      summary: Text to Image
      description: Returns URL of an image created from text according to given style
        parameters
      operationId: v1.images.quote.get
      x-api-path-slug: v1imagesquote-get
      parameters:
      - in: query
        name: author
        description: Name of the author/source
      - in: query
        name: authorFont
        description: Font-family used for author name
      - in: query
        name: authorFontColor
        description: Font color of the author
      - in: query
        name: backgroundColor
        description: Background color for solid background type
      - in: query
        name: bgType
        description: Background type (gradient/solid)
      - in: query
        name: brandLogo
        description: URL of the brand logo
      - in: query
        name: enableHighlight
        description: Enable highlight on quote text
      - in: query
        name: fontSize
        description: Font size for the quote (author font size is calculated automatically)
      - in: query
        name: gradientColor1
        description: First color for gradient background type
      - in: query
        name: gradientColor2
        description: Second color for gradient background type
      - in: query
        name: gradientType
        description: Type of gradient background (linear/radial)
      - in: query
        name: highlightColor
        description: Color used for highlight
      - in: query
        name: quote
        description: Text of the quote
      - in: query
        name: quoteFont
        description: Font-family used for quote text
      - in: query
        name: quoteFontColor
        description: Font color of the quote text
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/influencers/hashtag/{hashtag}:
    get:
      summary: Influencers for a Hashtag
      description: Returns list of Twitter influencers for a given hashtag
      operationId: v1.influencers.hashtag.hashtag.get
      x-api-path-slug: v1influencershashtaghashtag-get
      parameters:
      - in: path
        name: hashtag
        description: 'Hashtag without # mark'
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/link/cta:
    get:
      summary: List of CTAs
      description: Returns list of available CTA for current user. Requires each user
        to authenticate with RiteKit
      operationId: v1.link.cta.get
      x-api-path-slug: v1linkcta-get
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/link/short-link:
    get:
      summary: Shorten Link
      description: Returns a shorten link with a given CTA.
      operationId: v1.link.short_link.get
      x-api-path-slug: v1linkshortlink-get
      parameters:
      - in: query
        name: cta
        description: cta id
      - in: query
        name: url
        description: URL
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/search/trending:
    get:
      summary: Trending Hashtags
      description: Returns list of hashtags currently trending on Twitter
      operationId: v1.search.trending.get
      x-api-path-slug: v1searchtrending-get
      parameters:
      - in: query
        name: green
        description: Restrict results only to green hashtags
      - in: query
        name: latin
        description: Restrict results only to hashtags with latin characters
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/stats/auto-hashtag?post={post}:
    get:
      summary: Auto-Hashtag
      description: Returns auto-hashtagged text of the post.
      operationId: v1.stats.auto_hashtag_post_post.get
      x-api-path-slug: v1statsautohashtagpostpost-get
      parameters:
      - in: path
        name: post
        description: Text of the post
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/stats/hashtag-suggestions/{topic}:
    get:
      summary: Hashtag Suggestions
      description: Returns list of hashtag suggestions and their real-time stats for
        a given topic
      operationId: v1.stats.hashtag_suggestions.topic.get
      x-api-path-slug: v1statshashtagsuggestionstopic-get
      parameters:
      - in: path
        name: topic
        description: Topic
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/stats/history/{hashtag}:
    get:
      summary: Hashtag History
      description: Returns historical stats for a given hashtag from the last 30 days
      operationId: v1.stats.history.hashtag.get
      x-api-path-slug: v1statshistoryhashtag-get
      parameters:
      - in: path
        name: hashtag
        description: 'Hashtag without # mark'
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/stats/multiple-hashtags:
    get:
      summary: Hashtag Stats
      description: Returns real-time stats for up to 100 hashtags (updated hourly).
      operationId: v1.stats.multiple_hashtags.get
      x-api-path-slug: v1statsmultiplehashtags-get
      parameters:
      - in: query
        name: tags
        description: 'Hashtag(s) without # mark'
      responses:
        200:
          description: OK
      tags:
      - ""