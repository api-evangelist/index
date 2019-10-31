swagger: "2.0"
x-collection-name: Geneea
x-complete: 1
info:
  title: Geneea Natural Language Processing
  description: div-classapidescription----h2authenticationh2----pfor-all-calls-supply-your-api-key--a-hrefhttpswww-geneea-compricingsign-up-to-emobtain-the-keyema-p----p--------our-api-supports-both-emunencrypted-httpem-and-emencrypted-httpsem-protocols---------however-for-security-reasons-we-strongly-encourage-using-only-the-encrypted-version-----p----pthe-api-key-should-be-supplied-as-either-a-request-parameter-codeuser-keycode-or-in-codeauthorizationcode-header-p----precodeauthorization-user-key-ltyour-api-keygtcodepre----h2api-operationsh2----p--------all-api-operations-can-perform-analysis-on-supplied-raw-text-or-on-text-extracted-from-a-given-url---------optionally-one-can-supply-additional-information-which-can-make-the-result-more-precise--an-example--------of-such-information-would-be-the-language-of-text-or-a-particular-text-extractor-for-url-resources-----p----pthe-supported-types-of-analyses-arep----ul--------listronglemmatizationstrong-longrightarrow------------finds-out-lemmata-basic-forms-of-all-the-words-in-the-document---------li--------listrongcorrectionstrong-longrightarrow------------performs-correction-diacritization-on-all-the-words-in-the-document---------li--------listrongtopic-detectionstrong-longrightarrow------------determines-a-topic-of-the-document-e-g--finance-or-sports---------li--------listrongsentiment-analysisstrong-longrightarrow------------determines-a-sentiment-of-the-document-i-e--how-positive-or-negative-the-document-is---------li--------listrongnamed-entity-recognitionstrong-longrightarrow------------finds-named-entities-like-person-location-date-etc--mentioned-the-the-document---------li----ul----h2encodingh2----pthe-supplied-text-is-expected-to-be-in-utf8-encoding-this-is-especially-important-for-nonenglish-texts-p----h2returned-valuesh2----pthe-api-calls-always-return-objects-in-serialized-json-format-in-utf8-encoding-p----p--------if-any-error-occurs-the-http-response-code-will-be-in-the-range-code4xxcode-clientside-error-or--------code5xxcode-serverside-error--in-this-situation-the-body-of-the-response-will-contain-information--------about-the-error-in-json-format-with-codeexceptioncode-and-codemessagecode-values-----p----h2url-limitationsh2----p--------all-the-requests-are-semantically-codegetcode--however-for-longer-texts-you-may-run-into-issues--------with-url-length-limit--therefore-its-possible-to-always-issue-a-codepostcode-request-with-all--------the-parameters-encoded-as-a-json-in-the-request-body-----p----pexamplep----precode--------post-s1sentiment--------contenttype-applicationjson--------textthere-is-no-harm-in-being-sometimes-wrong--especially-if-one-is-promptly-found-out-----codepre----pthis-is-equivalent-to-codeget-s1sentimenttextthere20is20no20harm---codep----h2request-limitationsh2----p--------the-api-has-other-limitations-concerning-the-size-of-the-http-requests--the-maximum-allowed-size-of-any--------post-request-body-is-em512-kibem--for-request-with-a-url-resource-the-maximum-allowed-number-of--------extracted-characters-from-each-such-resource-is-em100000em-----p----h2more-informationh2----p--------a-hrefhttpsgeneea-atlassian-netwikidisplayipdtheinterpretorapipublicdocumentation-target-blank--------the-interpretor-public-documentation--------a----pdiv
  version: "1.0"
host: api.geneea.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account:
    get:
      summary: Get Account
      description: Information about current user account.
      operationId: getAccount
      x-api-path-slug: account-get
      responses:
        200:
          description: OK
      tags:
      - Account
  /s1/correction:
    get:
      summary: Get Correction
      description: Performs text correction (diacritization) on the given document.
      operationId: getS1Correction
      x-api-path-slug: s1correction-get
      parameters:
      - in: query
        name: extractor
        description: document extractor
      - in: query
        name: language
        description: document language
      - in: query
        name: returnTextInfo
      - in: query
        name: text
        description: raw document text
      - in: query
        name: url
        description: document URL
      responses:
        200:
          description: OK
      tags:
      - Correction
    post:
      summary: Post Correction
      description: Performs text correction (diacritization) on the given document.
      operationId: postS1Correction
      x-api-path-slug: s1correction-post
      parameters:
      - in: body
        name: body
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Correction
  /s1/entities:
    get:
      summary: Get Entities
      description: Performs named-entity recognition on the given document.
      operationId: getS1Entities
      x-api-path-slug: s1entities-get
      parameters:
      - in: query
        name: extractor
        description: document extractor
      - in: query
        name: language
        description: document language
      - in: query
        name: returnTextInfo
      - in: query
        name: text
        description: raw document text
      - in: query
        name: url
        description: document URL
      responses:
        200:
          description: OK
      tags:
      - Entities
    post:
      summary: Post Entities
      description: Performs named-entity recognition on the given document.
      operationId: postS1Entities
      x-api-path-slug: s1entities-post
      parameters:
      - in: body
        name: body
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Entities
  /s1/lemmatize:
    get:
      summary: Get Lemmatize
      description: Performs lemmatization on the given document.
      operationId: getS1Lemmatize
      x-api-path-slug: s1lemmatize-get
      parameters:
      - in: query
        name: extractor
        description: document extractor
      - in: query
        name: language
        description: document language
      - in: query
        name: returnTextInfo
      - in: query
        name: text
        description: raw document text
      - in: query
        name: url
        description: document URL
      responses:
        200:
          description: OK
      tags:
      - Lemmatize
    post:
      summary: Post Lemmatize
      description: Performs lemmatization on the given document.
      operationId: postS1Lemmatize
      x-api-path-slug: s1lemmatize-post
      parameters:
      - in: body
        name: body
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Lemmatize
  /s1/sentiment:
    get:
      summary: Get Sentiment
      description: Performs sentiment analysis on the given document.
      operationId: getS1Sentiment
      x-api-path-slug: s1sentiment-get
      parameters:
      - in: query
        name: extractor
        description: document extractor
      - in: query
        name: language
        description: document language
      - in: query
        name: returnTextInfo
      - in: query
        name: text
        description: raw document text
      - in: query
        name: url
        description: document URL
      responses:
        200:
          description: OK
      tags:
      - Sentiment
    post:
      summary: Post Sentiment
      description: Performs sentiment analysis on the given document.
      operationId: postS1Sentiment
      x-api-path-slug: s1sentiment-post
      parameters:
      - in: body
        name: body
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sentiment
  /s1/topic:
    get:
      summary: Get Topic
      description: Performs topic detection on the given document.
      operationId: getS1Topic
      x-api-path-slug: s1topic-get
      parameters:
      - in: query
        name: extractor
        description: document extractor
      - in: query
        name: language
        description: document language
      - in: query
        name: returnTextInfo
      - in: query
        name: text
        description: raw document text
      - in: query
        name: url
        description: document URL
      responses:
        200:
          description: OK
      tags:
      - Topic
    post:
      summary: Post Topic
      description: Performs topic detection on the given document.
      operationId: postS1Topic
      x-api-path-slug: s1topic-post
      parameters:
      - in: body
        name: body
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Topic