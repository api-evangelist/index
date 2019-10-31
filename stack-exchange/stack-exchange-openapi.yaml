swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 1
info:
  title: Stack Exchange
  description: stack-exchange-is-a-network-of-130-qa-communities-including-stack-overflow-
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /access-tokens/{accessTokens}:
    get:
      summary: Get Acces Tokens
      description: "Reads the properties for a set of access tokens.\n \n{accessTokens}
        can contain up to 20 access tokens. These are obtained by authenticating a
        user using OAuth 2.0.\n \nThis method returns a list of access_tokens."
      operationId: reads-the-properties-for-a-set-of-access-tokens-accesstokens-can-contain-up-to-20-access-tokens-thes
      x-api-path-slug: accesstokensaccesstokens-get
      parameters:
      - in: path
        name: accessTokens
        description: String list (semicolon delimited)
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Authentication
      - Access Tokens
  /access-tokens/{accessTokens}/invalidate:
    get:
      summary: Invalidate Acces Tokens
      description: "Immediately expires the access tokens passed. This method is meant
        to allow an application to discard any active access tokens it no longer needs.\n
        \n{accessTokens} can contain up to 20 access tokens. These are obtained by
        authenticating a user using OAuth 2.0.\n \nThis method returns a list of access_tokens."
      operationId: immediately-expires-the-access-tokens-passed-this-method-is-meant-to-allow-an-application-to-discard
      x-api-path-slug: accesstokensaccesstokensinvalidate-get
      parameters:
      - in: path
        name: accessTokens
        description: String list (semicolon delimited)
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Authentication
      - Access Tokens
  /answers:
    get:
      summary: Get Answers
      description: "Returns all the undeleted answers in the system.\n \nThe sorts
        accepted by this method operate on the follow fields of the answer object:\n
        - activity - last_activity_date\n - creation - creation_date\n - votes - score\n
        \ activity is the default sort.\n \n It is possible to create moderately complex
        queries using sort, min, max, fromdate, and todate.\n \nThis method returns
        a list of answers."
      operationId: returns-all-the-undeleted-answers-in-the-system-the-sorts-accepted-by-this-method-operate-on-the-fol
      x-api-path-slug: answers-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: Filter the discussion
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Answers
  /answers/{ids}:
    get:
      summary: Get Answer
      description: "Gets the set of answers identified by ids.\n \nThis is meant for
        batch fetcing of questions. A useful trick to poll for updates is to sort
        by activity, with a minimum date of the last time you polled.\n \n{ids} can
        contain up to 100 semicolon delimited ids, to find ids programatically look
        for answer_id on answer objects.\n \nThe sorts accepted by this method operate
        on the follow fields of the answer object:\n - activity - last_activity_date\n
        - creation - creation_date\n - votes - score\n  activity is the default sort.\n
        \n It is possible to create moderately complex queries using sort, min, max,
        fromdate, and todate.\n \nThis method returns a list of answers."
      operationId: gets-the-set-of-answers-identified-by-ids-this-is-meant-for-batch-fetcing-of-questions-a-useful-tric
      x-api-path-slug: answersids-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Answers
  /answers/{ids}/comments:
    get:
      summary: Get Answer Comments
      description: "Gets the comments on a set of answers.\n \nIf you know that you
        have an answer id and need the comments, use this method. If you know you
        have a question id, use /questions/{id}/comments. If you are unsure, use /posts/{id}/comments.\n
        \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
        look for answer_id on answer objects.\n \nThe sorts accepted by this method
        operate on the follow fields of the comment object:\n - creation - creation_date\n
        - votes - score\n  creation is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of comments."
      operationId: gets-the-comments-on-a-set-of-answers-if-you-know-that-you-have-an-answer-id-and-need-the-comments-u
      x-api-path-slug: answersidscomments-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = creation => datesort = votes => number
      - in: query
        name: min
        description: sort = creation => datesort = votes => number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Answers
      - comments
  /apps/{accessTokens}/de-authenticate:
    get:
      summary: De-Authenticate Token
      description: "Passing valid access_tokens to this method causes the application
        that created them to be de-authorized by the user associated with each access_token.
        This will remove the application from their apps tab, and cause all other
        existing access_tokens to be destroyed.\n \nThis method is meant for uninstalling
        applications, recovering from access_token leaks, or simply as a stronger
        form of /access-tokens/{accessTokens}/invalidate.\n \nNothing prevents a user
        from re-authenticate to an application that has de-authenticated itself, the
        user will be prompted to approve the application again however.\n \n{accessTokens}
        can contain up to 20 access tokens. These are obtained by authenticating a
        user using OAuth 2.0.\n \nThis method returns a list of access_tokens."
      operationId: passing-valid-access-tokens-to-this-method-causes-the-application-that-created-them-to-be-deauthoriz
      x-api-path-slug: appsaccesstokensdeauthenticate-get
      parameters:
      - in: path
        name: accessTokens
        description: String list (semicolon delimited)
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Authentication
      - Access Tokens
  /badges:
    get:
      summary: Get Badges
      description: "Returns all the badges in the system.\n \nBadge sorts are a tad
        complicated. For the purposes of sorting (and min/max) tag_based is considered
        to be greater than named.\n \nThis means that you can get a list of all tag
        based badges by passing min=tag_based, and conversely all the named badges
        by passing max=named, with sort=type.\n \nFor ranks, bronze is greater than
        silver which is greater than gold. Along with sort=rank, set max=gold for
        just gold badges, max=silver&min=silver for just silver, and min=bronze for
        just bronze.\n \nrank is the default sort.\n \nThis method returns a list
        of badges."
      operationId: returns-all-the-badges-in-the-system-badge-sorts-are-a-tad-complicated-for-the-purposes-of-sorting-a
      x-api-path-slug: badges-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: inname
      - in: query
        name: max
        description: sort = rank => stringsort = name => stringsort = type => string
      - in: query
        name: min
        description: sort = rank => stringsort = name => stringsort = type => string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Badges
  /badges/name:
    get:
      summary: Get Badge Name
      description: "Gets all explicitly named badges in the system.\n \nA named badged
        stands in opposition to a tag-based badge. These are referred to as general
        badges on the sites themselves.\n \nFor the rank sort, bronze is greater than
        silver which is greater than gold. Along with sort=rank, set max=gold for
        just gold badges, max=silver&min=silver for just silver, and min=bronze for
        just bronze.\n \nrank is the default sort.\n \nThis method returns a list
        of badges."
      operationId: gets-all-explicitly-named-badges-in-the-system-a-named-badged-stands-in-opposition-to-a-tagbased-bad
      x-api-path-slug: badgesname-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: inname
      - in: query
        name: max
        description: sort = rank => stringsort = name => string
      - in: query
        name: min
        description: sort = rank => stringsort = name => string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Badges
  /badges/recipients:
    get:
      summary: Get Badge Recipients
      description: "Returns recently awarded badges in the system.\n \nAs these badges
        have been awarded, they will have the badge.user property set.\n \nThis method
        returns a list of badges."
      operationId: returns-recently-awarded-badges-in-the-system-as-these-badges-have-been-awarded-they-will-have-the-b
      x-api-path-slug: badgesrecipients-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Badges
      - Recipients
  /badges/tags:
    get:
      summary: Get Badge Tags
      description: "Returns the badges that are awarded for participation in specific
        tags.\n \nFor the rank sort, bronze is greater than silver which is greater
        than gold. Along with sort=rank, set max=gold for just gold badges, max=silver&min=silver
        for just silver, and min=bronze for just bronze.\n \nrank is the default sort.\n
        \nThis method returns a list of badges."
      operationId: returns-the-badges-that-are-awarded-for-participation-in-specific-tags-for-the-rank-sort-bronze-is-g
      x-api-path-slug: badgestags-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: inname
      - in: query
        name: max
        description: sort = rank => stringsort = name => string
      - in: query
        name: min
        description: sort = rank => stringsort = name => string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Badges
  /badges/{ids}:
    get:
      summary: Get Badge
      description: "Gets the badges identified in id.\n \nNote that badge ids are
        not constant across sites, and thus should be looked up via the /badges method.
        A badge id on a single site is, however, guaranteed to be stable.\n \nBadge
        sorts are a tad complicated. For the purposes of sorting (and min/max) tag_based
        is considered to be greater than named.\n \nThis means that you can get a
        list of all tag based badges by passing min=tag_based, and conversely all
        the named badges by passing max=named, with sort=type.\n \nFor ranks, bronze
        is greater than silver which is greater than gold. Along with sort=rank, set
        max=gold for just gold badges, max=silver&min=silver for just silver, and
        min=bronze for just bronze.\n \nrank is the default sort.\n \n{ids} can contain
        up to 100 semicolon delimited ids, to find ids programatically look for badge_id
        on badge objects.\n \nThis method returns a list of badges."
      operationId: gets-the-badges-identified-in-id-note-that-badge-ids-are-not-constant-across-sites-and-thus-should-b
      x-api-path-slug: badgesids-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = rank => stringsort = name => stringsort = type => string
      - in: query
        name: min
        description: sort = rank => stringsort = name => stringsort = type => string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Badges
  /badges/{ids}/recipients:
    get:
      summary: Get Badge Recipients
      description: "Returns recently awarded badges in the system, constrained to
        a certain set of badges.\n \nAs these badges have been awarded, they will
        have the badge.user property set.\n \n{ids} can contain up to 100 semicolon
        delimited ids, to find ids programatically look for badge_id on badge objects.\n
        \nThis method returns a list of badges."
      operationId: returns-recently-awarded-badges-in-the-system-constrained-to-a-certain-set-of-badges-as-these-badges
      x-api-path-slug: badgesidsrecipients-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Badges
  /comments:
    get:
      summary: Get Comments
      description: "Gets all the comments on the site.\n \nIf you're filtering for
        interesting comments (by score, creation date, etc.) make use of the sort
        paramter with appropriate min and max values.\n \nIf you're looking to query
        conversations between users, instead use the /users/{ids}/mentioned and /users/{ids}/comments/{toid}
        methods.\n \nThe sorts accepted by this method operate on the follow fields
        of the comment object:\n - creation - creation_date\n - votes - score\n  creation
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of comments."
      operationId: gets-all-the-comments-on-the-site-if-youre-filtering-for-interesting-comments-by-score-creation-date
      x-api-path-slug: comments-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = creation => datesort = votes => number
      - in: query
        name: min
        description: sort = creation => datesort = votes => number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Comments
  /comments/{ids}:
    get:
      summary: Get Comment
      description: "Gets the comments identified in id.\n \nThis method is most useful
        if you have a cache of comment ids obtained through other means (such as /questions/{id}/comments)
        but suspect the data may be stale.\n \n{ids} can contain up to 100 semicolon
        delimited ids, to find ids programatically look for comment_id on comment
        objects.\n \nThe sorts accepted by this method operate on the follow fields
        of the comment object:\n - creation - creation_date\n - votes - score\n  creation
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of comments."
      operationId: gets-the-comments-identified-in-id-this-method-is-most-useful-if-you-have-a-cache-of-comment-ids-obt
      x-api-path-slug: commentsids-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = creation => datesort = votes => number
      - in: query
        name: min
        description: sort = creation => datesort = votes => number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Comments
  /comments/{id}/delete:
    post:
      summary: Delete Comment
      description: "Deletes a comment.\n \nUse an access_token with write_access to
        delete a comment.\n \nIn practice, this method will never return an object."
      operationId: deletes-a-comment-use-an-access-token-with-write-access-to-delete-a-comment-in-practice-this-method-
      x-api-path-slug: commentsiddelete-post
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: preview
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Comments
  /comments/{id}/edit:
    post:
      summary: Edit Comment
      description: "Edit an existing comment.\n \nUse an access_token with write_access
        to edit an existing comment.\n \nThis method return the created comment."
      operationId: edit-an-existing-comment-use-an-access-token-with-write-access-to-edit-an-existing-comment-this-meth
      x-api-path-slug: commentsidedit-post
      parameters:
      - in: query
        name: body
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: preview
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Comments
  /errors:
    get:
      summary: Get Errors
      description: "Returns the various error codes that can be produced by the API.\n
        \nThis method is provided for discovery, documentation, and testing purposes,
        it is not expected many applications will consume it during normal operation.\n
        \nFor testing purposes, look into the /errors/{id} method which simulates
        errors given a code.\n \nThis method returns a list of errors."
      operationId: returns-the-various-error-codes-that-can-be-produced-by-the-api-this-method-is-provided-for-discover
      x-api-path-slug: errors-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Errors
  /errors/{id}:
    get:
      summary: Get Error
      description: "This method allows you to generate an error.\n \nThis method is
        only intended for use when testing an application or library. Unlike other
        methods in the API, its contract is not frozen, and new error codes may be
        added at any time.\n \nThis method results in an error, which will be expressed
        with a 400 HTTP status code and setting the error* properties on the wrapper
        object."
      operationId: this-method-allows-you-to-generate-an-error-this-method-is-only-intended-for-use-when-testing-an-app
      x-api-path-slug: errorsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Errors
  /events:
    get:
      summary: Get Event
      description: "Returns a stream of events that have occurred on the site.\n \nThe
        API considers the following \"events\":\n - posting a question\n - posting
        an answer\n - posting a comment\n - editing a post\n - creating a user\n  \n
        \nEvents are only accessible for 15 minutes after they occurred, and by default
        only events in the last 5 minutes are returned. You can specify the age of
        the oldest event returned by setting the since parameter.\n \nIt is advised
        that developers batch events by ids and make as few subsequent requests to
        other methods as possible.\n \nThis method returns a list of events."
      operationId: returns-a-stream-of-events-that-have-occurred-on-the-site-the-api-considers-the-following-events--po
      x-api-path-slug: events-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: since
        description: Unix date
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Events
  /filters/create:
    get:
      summary: Create Filter
      description: "Creates a new filter given a list of includes, excludes, a base
        filter, and whether or not this filter should be \"unsafe\".\n \nFilter \"safety\"
        is defined as follows. Any string returned as a result of an API call with
        a safe filter will be inline-able into HTML without script-injection concerns.
        That is to say, no additional sanitizing (encoding, HTML tag stripping, etc.)
        will be necessary on returned strings. Applications that wish to handle sanitizing
        themselves should create an unsafe filter. All filters are safe by default,
        under the assumption that double-encoding bugs are more desirable than script
        injections.\n \nIf no base filter is specified, the default filter is assumed.
        When building a filter from scratch, the none built-in filter is useful.\n
        \nWhen the size of the parameters being sent to this method grows to large,
        problems can occur. This method will accept POST requests to mitigate this.\n
        \nIt is not expected that many applications will call this method at runtime,
        filters should be pre-calculated and \"baked in\" in the common cases. Furthermore,
        there are a number of built-in filters which cover common use cases.\n \nThis
        method returns a single filter."
      operationId: creates-a-new-filter-given-a-list-of-includes-excludes-a-base-filter-and-whether-or-not-this-filter-
      x-api-path-slug: filterscreate-get
      parameters:
      - in: query
        name: base
      - in: query
        name: exclude
        description: String list (semicolon delimited)
      - in: query
        name: include
        description: String list (semicolon delimited)
      - in: query
        name: unsafe
      responses:
        200:
          description: OK
      tags:
      - Files
  /filters/{filters}:
    get:
      summary: Get Filters
      description: "Returns the fields included by the given filters, and the \"safeness\"
        of those filters.\n \nIt is not expected that this method will be consumed
        by many applications at runtime, it is provided to aid in debugging.\n \n{filters}
        can contain up to 20 semicolon delimited filters. Filters are obtained via
        calls to /filters/create, or by using a built-in filter.\n \nThis method returns
        a list of filters."
      operationId: returns-the-fields-included-by-the-given-filters-and-the-safeness-of-those-filters-it-is-not-expecte
      x-api-path-slug: filtersfilters-get
      parameters:
      - in: path
        name: filters
        description: String list (semicolon delimited)
      responses:
        200:
          description: OK
      tags:
      - Files
  /inbox:
    get:
      summary: Get Inbox
      description: "Returns a user's inbox.\n \nThis method requires an access_token,
        with a scope containing \"read_inbox\".\n \nThis method returns a list of
        inbox items."
      operationId: returns-a-users-inbox-this-method-requires-an-access-token-with-a-scope-containing-read-inbox-this-m
      x-api-path-slug: inbox-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Email
      - Inbox
  /inbox/unread:
    get:
      summary: Unread Inbox
      description: "Returns the unread items in a user's inbox.\n \nThis method requires
        an access_token, with a scope containing \"read_inbox\".\n \nThis method returns
        a list of inbox items."
      operationId: returns-the-unread-items-in-a-users-inbox-this-method-requires-an-access-token-with-a-scope-containi
      x-api-path-slug: inboxunread-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: since
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Email
      - Inbox
  /info:
    get:
      summary: Get Information
      description: "Returns a collection of statistics about the site.\n \nData to
        facilitate per-site customization, discover related sites, and aggregate statistics
        is all returned by this method.\n \nThis data is cached very aggressively,
        by design. Query sparingly, ideally no more than once an hour.\n \nThis method
        returns an info object."
      operationId: returns-a-collection-of-statistics-about-the-site-data-to-facilitate-persite-customization-discover-
      x-api-path-slug: info-get
      parameters:
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Information
  /me:
    get:
      summary: Get Me
      description: "Returns the user associated with the passed access_token.\n \nThis
        method returns a user."
      operationId: returns-the-user-associated-with-the-passed-access-token-this-method-returns-a-user
      x-api-path-slug: me-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: min
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Self
  /me/answers:
    get:
      summary: My Answers
      description: "Returns the answers owned by the user associated with the given
        access_token.\n \nThis method returns a list of answers."
      operationId: returns-the-answers-owned-by-the-user-associated-with-the-given-access-token-this-method-returns-a-l
      x-api-path-slug: meanswers-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Answers
  /me/associated:
    get:
      summary: My Assocated
      description: "Returns all of a user's associated accounts, given an access_token
        for them.\n \nThis method returns a list of network users."
      operationId: returns-all-of-a-users-associated-accounts-given-an-access-token-for-them-this-method-returns-a-list
      x-api-path-slug: meassociated-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Associated
  /me/badges:
    get:
      summary: My Badges
      description: "Returns the badges earned by the user associated with the given
        access_token.\n \nThis method returns a list of badges."
      operationId: returns-the-badges-earned-by-the-user-associated-with-the-given-access-token-this-method-returns-a-l
      x-api-path-slug: mebadges-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = rank => stringsort = name => stringsort = type => string
      - in: query
        name: min
        description: sort = rank => stringsort = name => stringsort = type => string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Badges
  /me/comments:
    get:
      summary: My Comments
      description: "Returns the comments owned by the user associated with the given
        access_token.\n \nThis method returns a list of comments."
      operationId: returns-the-comments-owned-by-the-user-associated-with-the-given-access-token-this-method-returns-a-
      x-api-path-slug: mecomments-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = creation => datesort = votes => number
      - in: query
        name: min
        description: sort = creation => datesort = votes => number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Comments
  /me/comments/{toId}:
    get:
      summary: My Comments
      description: "Returns the comments owned by the user associated with the given
        access_token that are in reply to the user identified by {toId}.\n \nThis
        method returns a list of comments."
      operationId: returns-the-comments-owned-by-the-user-associated-with-the-given-access-token-that-are-in-reply-to-t
      x-api-path-slug: mecommentstoid-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = creation => datesort = votes => number
      - in: query
        name: min
        description: sort = creation => datesort = votes => number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      - in: path
        name: toId
      responses:
        200:
          description: OK
      tags:
      - Comments
  /me/favorites:
    get:
      summary: My Favorites
      description: "Returns the questions favorites by the user associated with the
        given access_token.\n \nThis method returns a list of questions."
      operationId: returns-the-questions-favorites-by-the-user-associated-with-the-given-access-token-this-method-retur
      x-api-path-slug: mefavorites-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = added => date
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = added => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Favorites
  /me/inbox:
    get:
      summary: My Inbox
      description: "Returns the user identified by access_token's inbox.\n \nThis
        method requires an access_token, with a scope containing \"read_inbox\".\n
        \nThis method returns a list of inbox items."
      operationId: returns-the-user-identified-by-access-tokens-inbox-this-method-requires-an-access-token-with-a-scope
      x-api-path-slug: meinbox-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Email
      - Inbox
  /me/inbox/unread:
    get:
      summary: My Inbox Unread
      description: "Returns the unread items in the user identified by access_token's
        inbox.\n \nThis method requires an access_token, with a scope containing \"read_inbox\".\n
        \nThis method returns a list of inbox items."
      operationId: returns-the-unread-items-in-the-user-identified-by-access-tokens-inbox-this-method-requires-an-acces
      x-api-path-slug: meinboxunread-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: since
        description: Unix date
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Email
      - Inbox
  /me/mentioned:
    get:
      summary: My Mentions
      description: "Returns the comments mentioning the user associated with the given
        access_token.\n \nThis method returns a list of comments."
      operationId: returns-the-comments-mentioning-the-user-associated-with-the-given-access-token-this-method-returns-
      x-api-path-slug: mementioned-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = creation => datesort = votes => number
      - in: query
        name: min
        description: sort = creation => datesort = votes => number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Mentioned
  /me/merges:
    get:
      summary: My Merges
      description: "Returns a record of merges that have occurred involving a user
        identified by an access_token.\n \nThis method allows you to take now invalid
        account ids and find what account they've become, or take currently valid
        account ids and find which ids were equivalent in the past.\n \nThis is most
        useful when confirming that an account_id is in fact \"new\" to an application.\n
        \nAccount merges can happen for a wide range of reasons, applications should
        not make assumptions that merges have particular causes.\n \nNote that accounts
        are managed at a network level, users on a site may be merged due to an account
        level merge but there is no guarantee that a merge has an effect on any particular
        site.\n \nThis method returns a list of account_merge."
      operationId: returns-a-record-of-merges-that-have-occurred-involving-a-user-identified-by-an-access-token-this-me
      x-api-path-slug: memerges-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Merges
  /me/notifications:
    get:
      summary: My Notiications
      description: "Returns a user's notifications, given an access_token.\n \nThis
        method requires an access_token, with a scope containing \"read_inbox\".\n
        \nThis method returns a list of notifications."
      operationId: returns-a-users-notifications-given-an-access-token-this-method-requires-an-access-token-with-a-scop
      x-api-path-slug: menotifications-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /me/notifications/unread:
    get:
      summary: My Notiications Unread
      description: "Returns a user's unread notifications, given an access_token.\n
        \nThis method requires an access_token, with a scope containing \"read_inbox\".\n
        \nThis method returns a list of notifications."
      operationId: returns-a-users-unread-notifications-given-an-access-token-this-method-requires-an-access-token-with
      x-api-path-slug: menotificationsunread-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /me/privileges:
    get:
      summary: My Priveleges
      description: "Returns the privileges the user identified by access_token has.\n
        \nThis method returns a list of privileges."
      operationId: returns-the-privileges-the-user-identified-by-access-token-has-this-method-returns-a-list-of-privile
      x-api-path-slug: meprivileges-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Privileges
  /me/questions:
    get:
      summary: My Questions
      description: "Returns the questions owned by the user associated with the given
        access_token.\n \nThis method returns a list of questions."
      operationId: returns-the-questions-owned-by-the-user-associated-with-the-given-access-token-this-method-returns-a
      x-api-path-slug: mequestions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /me/questions/featured:
    get:
      summary: My Questions Featured
      description: "Returns the questions that have active bounties offered by the
        user associated with the given access_token.\n \nThis method returns a list
        of questions."
      operationId: returns-the-questions-that-have-active-bounties-offered-by-the-user-associated-with-the-given-access
      x-api-path-slug: mequestionsfeatured-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /me/questions/no-answers:
    get:
      summary: My Questions No Answers
      description: "Returns the questions owned by the user associated with the given
        access_token that have no answers.\n \nThis method returns a list of questions."
      operationId: returns-the-questions-owned-by-the-user-associated-with-the-given-access-token-that-have-no-answers-
      x-api-path-slug: mequestionsnoanswers-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /me/questions/unaccepted:
    get:
      summary: My Questions Unaccepted
      description: "Returns the questions owned by the user associated with the given
        access_token that have no accepted answer.\n \nThis method returns a list
        of questions."
      operationId: returns-the-questions-owned-by-the-user-associated-with-the-given-access-token-that-have-no-accepted
      x-api-path-slug: mequestionsunaccepted-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /me/questions/unanswered:
    get:
      summary: My Questions Unanswered
      description: "Returns the questions owned by the user associated with the given
        access_token that are not considered answered.\n \nThis method returns a list
        of questions."
      operationId: returns-the-questions-owned-by-the-user-associated-with-the-given-access-token-that-are-not-consider
      x-api-path-slug: mequestionsunanswered-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /me/reputation:
    get:
      summary: My Reputation
      description: "Returns the reputation changed for the user associated with the
        given access_token.\n \nThis method returns a list of reputation changes."
      operationId: returns-the-reputation-changed-for-the-user-associated-with-the-given-access-token-this-method-retur
      x-api-path-slug: mereputation-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Reputation
  /me/reputation-history:
    get:
      summary: My Reputation History
      description: "Returns user's public reputation history.\n \nThis method returns
        a list of reputation_history."
      operationId: returns-users-public-reputation-history-this-method-returns-a-list-of-reputation-history
      x-api-path-slug: mereputationhistory-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Reputation
  /me/reputation-history/full:
    get:
      summary: My Reputation History Full
      description: "Returns user's full reputation history, including private events.\n
        \n This method requires an access_token, with a scope containing \"private_info\".\n
        \nThis method returns a list of reputation_history."
      operationId: returns-users-full-reputation-history-including-private-events--this-method-requires-an-access-token
      x-api-path-slug: mereputationhistoryfull-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Reputation
  /me/suggested-edits:
    get:
      summary: Suggested Edits
      description: "Returns the suggested edits the user identified by access_token
        has submitted.\n \nThis method returns a list of suggested-edits."
      operationId: returns-the-suggested-edits-the-user-identified-by-access-token-has-submitted-this-method-returns-a-
      x-api-path-slug: mesuggestededits-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: min
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Suggested Edits
  /me/tags:
    get:
      summary: My Tags
      description: "Returns the tags the user identified by the access_token passed
        is active in.\n \nThis method returns a list of tags."
      operationId: returns-the-tags-the-user-identified-by-the-access-token-passed-is-active-in-this-method-returns-a-l
      x-api-path-slug: metags-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: min
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
  /me/tags/{tags}/top-answers:
    get:
      summary: My Tags Top Answers
      description: "Returns the top 30 answers the user associated with the given
        access_token has posted in response to questions with the given tags.\n \nThis
        method returns a list of answers."
      operationId: returns-the-top-30-answers-the-user-associated-with-the-given-access-token-has-posted-in-response-to
      x-api-path-slug: metagstagstopanswers-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: path
        name: tags
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Anwers
  /me/tags/{tags}/top-questions:
    get:
      summary: My Tags Top Questions
      description: "Returns the top 30 questions the user associated with the given
        access_token has posted in response to questions with the given tags.\n \nThis
        method returns a list of questions."
      operationId: returns-the-top-30-questions-the-user-associated-with-the-given-access-token-has-posted-in-response-
      x-api-path-slug: metagstagstopquestions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = hot => nonesort = week => nonesort = month => nonesort = relevance
          => none
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = hot => nonesort = week => nonesort = month => nonesort = relevance
          => none
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: path
        name: tags
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Questions
  /me/timeline:
    get:
      summary: My Timeline
      description: "Returns a subset of the actions the user identified by the passed
        access_token has taken on the site.\n \nThis method returns a list of user
        timeline objects."
      operationId: returns-a-subset-of-the-actions-the-user-identified-by-the-passed-access-token-has-taken-on-the-site
      x-api-path-slug: metimeline-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Timeline
  /me/top-answer-tags:
    get:
      summary: My Top Answer Tags
      description: "Returns the user identified by access_token's top 30 tags by answer
        score.\n \nThis method returns a list of top tag objects."
      operationId: returns-the-user-identified-by-access-tokens-top-30-tags-by-answer-score-this-method-returns-a-list-
      x-api-path-slug: metopanswertags-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Anwers
  /me/top-question-tags:
    get:
      summary: My Top Question Tags
      description: "Returns the user identified by access_token's top 30 tags by question
        score.\n \nThis method returns a list of top tag objects."
      operationId: returns-the-user-identified-by-access-tokens-top-30-tags-by-question-score-this-method-returns-a-lis
      x-api-path-slug: metopquestiontags-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Questions
  /me/write-permissions:
    get:
      summary: My Write Permissions
      description: "Returns the write permissions a user has via the api, given an
        access token.\n \nThe Stack Exchange API gives users the ability to create,
        edit, and delete certain types. This method returns whether the passed user
        is capable of performing those actions at all, as well as how many times a
        day they can.\n \nThis method does not consider the user's current quota (ie.
        if they've already exhausted it for today) nor any additional restrictions
        on write access, such as editing deleted comments.\n \nThis method returns
        a list of write_permissions."
      operationId: returns-the-write-permissions-a-user-has-via-the-api-given-an-access-token-the-stack-exchange-api-gi
      x-api-path-slug: mewritepermissions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Write Permissions
  /notifications:
    get:
      summary: Get Notifications
      description: "Returns a user's notifications.\n \nThis method requires an access_token,
        with a scope containing \"read_inbox\".\n \nThis method returns a list of
        notifications."
      operationId: returns-a-users-notifications-this-method-requires-an-access-token-with-a-scope-containing-read-inbo
      x-api-path-slug: notifications-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /notifications/unread:
    get:
      summary: Get Notifications Unread
      description: "Returns a user's unread notifications.\n \nThis method requires
        an access_token, with a scope containing \"read_inbox\".\n \nThis method returns
        a list of notifications."
      operationId: returns-a-users-unread-notifications-this-method-requires-an-access-token-with-a-scope-containing-re
      x-api-path-slug: notificationsunread-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Notifications
  /posts:
    get:
      summary: Get Posts
      description: "Fetches all posts (questions and answers) on the site.\n \nIn
        many ways this method is the union of /questions and /answers, returning both
        sets of data albeit only the common fields.\n \nMost applications should use
        the question or answer specific methods, but /posts is available for those
        rare cases where any activity is of intereset. Examples of such queries would
        be: \"all posts on Jan. 1st 2011\" or \"top 10 posts by score of all time\".\n
        \nThe sorts accepted by this method operate on the follow fields of the post
        object:\n - activity - last_activity_date\n - creation - creation_date\n -
        votes - score\n  activity is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of posts."
      operationId: fetches-all-posts-questions-and-answers-on-the-site-in-many-ways-this-method-is-the-union-of-questio
      x-api-path-slug: posts-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/{ids}:
    get:
      summary: Get Post
      description: "Fetches a set of posts by ids.\n \nThis method is meant for grabbing
        an object when unsure whether an id identifies a question or an answer. This
        is most common with user entered data.\n \n{ids} can contain up to 100 semicolon
        delimited ids, to find ids programatically look for post_id, answer_id, or
        question_id on post, answer, and question objects respectively.\n \nThe sorts
        accepted by this method operate on the follow fields of the post object:\n
        - activity - last_activity_date\n - creation - creation_date\n - votes - score\n
        \ activity is the default sort.\n \n It is possible to create moderately complex
        queries using sort, min, max, fromdate, and todate.\n \nThis method returns
        a list of posts."
      operationId: fetches-a-set-of-posts-by-ids-this-method-is-meant-for-grabbing-an-object-when-unsure-whether-an-id-
      x-api-path-slug: postsids-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Posts
  /posts/{ids}/comments:
    get:
      summary: Get Post Comments
      description: "Gets the comments on the posts identified in ids, regardless of
        the type of the posts.\n \nThis method is meant for cases when you are unsure
        of the type of the post id provided. Generally, this would be due to obtaining
        the post id directly from a user.\n \n{ids} can contain up to 100 semicolon
        delimited ids, to find ids programatically look for post_id, answer_id, or
        question_id on post, answer, and question objects respectively.\n \nThe sorts
        accepted by this method operate on the follow fields of the comment object:\n
        - creation - creation_date\n - votes - score\n  creation is the default sort.\n
        \n It is possible to create moderately complex queries using sort, min, max,
        fromdate, and todate.\n \nThis method returns a list of comments."
      operationId: gets-the-comments-on-the-posts-identified-in-ids-regardless-of-the-type-of-the-posts-this-method-is-
      x-api-path-slug: postsidscomments-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = creation => datesort = votes => number
      - in: query
        name: min
        description: sort = creation => datesort = votes => number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Comments
  /posts/{ids}/revisions:
    get:
      summary: Get Post Revisions
      description: "Returns edit revisions for the posts identified in ids.\n \n{ids}
        can contain up to 100 semicolon delimited ids, to find ids programatically
        look for post_id, answer_id, or question_id on post, answer, and question
        objects respectively.\n \nThis method returns a list of revisions."
      operationId: returns-edit-revisions-for-the-posts-identified-in-ids-ids-can-contain-up-to-100-semicolon-delimited
      x-api-path-slug: postsidsrevisions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Revisions
  /posts/{ids}/suggested-edits:
    get:
      summary: Get Posts Suggested Edits
      description: "Returns suggsted edits on the posts identified in ids.\n \n -
        creation - creation_date\n - approval - approval_date\n - rejection - rejection_date\n
        \ creation is the default sort.\n \n {ids} can contain up to 100 semicolon
        delimited ids, to find ids programatically look for post_id, answer_id, or
        question_id on post, answer, and question objects respectively.\n \nThis method
        returns a list of suggested-edits."
      operationId: returns-suggsted-edits-on-the-posts-identified-in-ids---creation--creation-date--approval--approval-
      x-api-path-slug: postsidssuggestededits-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: min
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Suggested Edits
  /posts/{id}/comments/add:
    post:
      summary: Add Comment Post
      description: "Create a new comment.\n \nUse an access_token with write_access
        to create a new comment on a post.\n \nThis method returns the created comment."
      operationId: create-a-new-comment-use-an-access-token-with-write-access-to-create-a-new-comment-on-a-post-this-me
      x-api-path-slug: postsidcommentsadd-post
      parameters:
      - in: query
        name: body
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: preview
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Posts
      - Comments
  /privileges:
    get:
      summary: Get Privileges
      description: "Returns the earnable privileges on a site.\n \nPrivileges define
        abilities a user can earn (via reputation) on any Stack Exchange site.\n \nWhile
        fairly stable, over time they do change. New ones are introduced with new
        features, and the reputation requirements change as a site matures.\n \nThis
        method returns a list of privileges."
      operationId: returns-the-earnable-privileges-on-a-site-privileges-define-abilities-a-user-can-earn-via-reputation
      x-api-path-slug: privileges-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Privileges
  /questions:
    get:
      summary: Get Questions
      description: "Gets all the questions on the site.\n \nThis method allows you
        make fairly flexible queries across the entire corpus of questions on a site.
        For example, getting all questions asked in the the week of Jan 1st 2011 with
        scores of 10 or more is a single query with parameters sort=votes&min=10&fromdate=1293840000&todate=1294444800.\n
        \nTo constrain questions returned to those with a set of tags, use the tagged
        parameter with a semi-colon delimited list of tags. This is an and contraint,
        passing tagged=c;java will return only those questions with both tags. As
        such, passing more than 5 tags will always return zero results.\n \nThe sorts
        accepted by this method operate on the follow fields of the question object:\n
        - activity - last_activity_date\n - creation - creation_date\n - votes - score\n
        - hot - by the formula ordering the hot tab Does not accept min or max\n -
        week - by the formula ordering the week tab Does not accept min or max\n -
        month - by the formula ordering the month tab Does not accept min or max\n
        \ activity is the default sort.\n \n It is possible to create moderately complex
        queries using sort, min, max, fromdate, and todate.\n \nThis method returns
        a list of questions."
      operationId: gets-all-the-questions-on-the-site-this-method-allows-you-make-fairly-flexible-queries-across-the-en
      x-api-path-slug: questions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = hot => nonesort = week => nonesort = month => nonesort = relevance
          => none
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = hot => nonesort = week => nonesort = month => nonesort = relevance
          => none
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: tagged
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /questions/featured:
    get:
      summary: Get Questions Featured
      description: "Returns all the questions with active bounties in the system.\n
        \nThe sorts accepted by this method operate on the follow fields of the question
        object:\n - activity - last_activity_date\n - creation - creation_date\n -
        votes - score\n  activity is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of questions."
      operationId: returns-all-the-questions-with-active-bounties-in-the-system-the-sorts-accepted-by-this-method-opera
      x-api-path-slug: questionsfeatured-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: tagged
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /questions/no-answers:
    get:
      summary: Get Questions No Answers
      description: "Returns questions which have received no answers.\n \nCompare
        with /questions/unanswered which mearly returns questions that the sites consider
        insufficiently well answered.\n \nThis method corresponds roughly with the
        this site tab.\n \nTo constrain questions returned to those with a set of
        tags, use the tagged parameter with a semi-colon delimited list of tags. This
        is an and contraint, passing tagged=c;java will return only those questions
        with both tags. As such, passing more than 5 tags will always return zero
        results.\n \nThe sorts accepted by this method operate on the follow fields
        of the question object:\n - activity - last_activity_date\n - creation - creation_date\n
        - votes - score\n  activity is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of questions."
      operationId: returns-questions-which-have-received-no-answers-compare-with-questionsunanswered-which-mearly-retur
      x-api-path-slug: questionsnoanswers-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: tagged
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /questions/unanswered:
    get:
      summary: Get Questions Unanswered
      description: "Returns questions the site considers to be unanswered.\n \nNote
        that just because a question has an answer, that does not mean it is considered
        answered. While the rules are subject to change, at this time a question must
        have at least one upvoted answer to be considered answered.\n \nTo constrain
        questions returned to those with a set of tags, use the tagged parameter with
        a semi-colon delimited list of tags. This is an and contraint, passing tagged=c;java
        will return only those questions with both tags. As such, passing more than
        5 tags will always return zero results.\n \nCompare with /questions/no-answers.\n
        \nThis method corresponds roughly with the unanswered tab.\n \nThe sorts accepted
        by this method operate on the follow fields of the question object:\n - activity
        - last_activity_date\n - creation - creation_date\n - votes - score\n  activity
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of questions."
      operationId: returns-questions-the-site-considers-to-be-unanswered-note-that-just-because-a-question-has-an-answe
      x-api-path-slug: questionsunanswered-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: tagged
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /questions/{ids}:
    get:
      summary: Get Questions
      description: "Returns the questions identified in {ids}.\n \nThis is most useful
        for fetching fresh data when maintaining a cache of question ids, or polling
        for changes.\n \n{ids} can contain up to 100 semicolon delimited ids, to find
        ids programatically look for question_id on question objects.\n \nThe sorts
        accepted by this method operate on the follow fields of the question object:\n
        - activity - last_activity_date\n - creation - creation_date\n - votes - score\n
        \ activity is the default sort.\n \n It is possible to create moderately complex
        queries using sort, min, max, fromdate, and todate.\n \nThis method returns
        a list of questions."
      operationId: returns-the-questions-identified-in-ids-this-is-most-useful-for-fetching-fresh-data-when-maintaining
      x-api-path-slug: questionsids-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /questions/{ids}/answers:
    get:
      summary: Get Question Answers
      description: "Gets the answers to a set of questions identified in id.\n \nThis
        method is most useful if you have a set of interesting questions, and you
        wish to obtain all of their answers at once or if you are polling for new
        or updates answers (in conjunction with sort=activity).\n \n{ids} can contain
        up to 100 semicolon delimited ids, to find ids programatically look for question_id
        on question objects.\n \nThe sorts accepted by this method operate on the
        follow fields of the answer object:\n - activity - last_activity_date\n -
        creation - creation_date\n - votes - score\n  activity is the default sort.\n
        \n It is possible to create moderately complex queries using sort, min, max,
        fromdate, and todate.\n \nThis method returns a list of answers."
      operationId: gets-the-answers-to-a-set-of-questions-identified-in-id-this-method-is-most-useful-if-you-have-a-set
      x-api-path-slug: questionsidsanswers-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
      - Answers
  /questions/{ids}/comments:
    get:
      summary: Get Question Comments
      description: "Gets the comments on a question.\n \nIf you know that you have
        an question id and need the comments, use this method. If you know you have
        a answer id, use /answers/{ids}/comments. If you are unsure, use /posts/{ids}/comments.\n
        \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
        look for question_id on question objects.\n \nThe sorts accepted by this method
        operate on the follow fields of the comment object:\n - creation - creation_date\n
        - votes - score\n  creation is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of comments."
      operationId: gets-the-comments-on-a-question-if-you-know-that-you-have-an-question-id-and-need-the-comments-use-t
      x-api-path-slug: questionsidscomments-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = creation => datesort = votes => number
      - in: query
        name: min
        description: sort = creation => datesort = votes => number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
      - Linked
  /questions/{ids}/linked:
    get:
      summary: Get Question Linked
      description: "Gets questions which link to those questions identified in {ids}.\n
        \nThis method only considers questions that are linked within a site, and
        will never return questions from another Stack Exchange site.\n \nA question
        is considered \"linked\" when it explicitly includes a hyperlink to another
        question, there are no other heuristics.\n \n{ids} can contain up to 100 semicolon
        delimited ids, to find ids programatically look for question_id on question
        objects.\n \nThe sorts accepted by this method operate on the follow fields
        of the question object:\n - activity - last_activity_date\n - creation - creation_date\n
        - votes - score\n - rank - a priority sort by site applies, subject to change
        at any time Does not accept min or max\n  activity is the default sort.\n
        \n It is possible to create moderately complex queries using sort, min, max,
        fromdate, and todate.\n \nThis method returns a list of questions."
      operationId: gets-questions-which-link-to-those-questions-identified-in-ids-this-method-only-considers-questions-
      x-api-path-slug: questionsidslinked-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = rank => none
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = rank => none
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
      - Linked
  /questions/{ids}/related:
    get:
      summary: Get Question Related
      description: "Returns questions that the site considers related to those identified
        in {ids}.\n \nThe algorithm for determining if questions are related is not
        documented, and subject to change at any time. Futhermore, these values are
        very heavily cached, and may not update immediately after a question has been
        editted. It is also not guaranteed that a question will be considered related
        to any number (even non-zero) of questions, and a consumer should be able
        to handle a variable number of returned questions.\n \n{ids} can contain up
        to 100 semicolon delimited ids, to find ids programatically look for question_id
        on question objects.\n \nThe sorts accepted by this method operate on the
        follow fields of the question object:\n - activity - last_activity_date\n
        - creation - creation_date\n - votes - score\n - rank - a priority sort by
        site applies, subject to change at any time Does not accept min or max\n  activity
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of questions."
      operationId: returns-questions-that-the-site-considers-related-to-those-identified-in-ids-the-algorithm-for-deter
      x-api-path-slug: questionsidsrelated-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = rank => none
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = rank => none
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
      - Related
  /questions/{ids}/timeline:
    get:
      summary: Get Question AnsweTimeliners
      description: "Returns a subset of the events that have happened to the questions
        identified in id.\n \nThis provides data similar to that found on a question's
        timeline page.\n \nVoting data is scrubbed to deter inferencing of voter identity.\n
        \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
        look for question_id on question objects.\n \nThis method returns a list of
        question timeline events."
      operationId: returns-a-subset-of-the-events-that-have-happened-to-the-questions-identified-in-id-this-provides-da
      x-api-path-slug: questionsidstimeline-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
      - Timeline
  /revisions/{ids}:
    get:
      summary: Get Revisions
      description: "Returns edit revisions identified by ids in {ids}.\n \n{ids} can
        contain up to 20 semicolon delimited ids, to find ids programatically look
        for revision_guid on revision objects. Note that unlike most other id types
        in the API, revision_guid is a string.\n \nThis method returns a list of revisions."
      operationId: returns-edit-revisions-identified-by-ids-in-ids-ids-can-contain-up-to-20-semicolon-delimited-ids-to-
      x-api-path-slug: revisionsids-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Guid list (semicolon delimited)
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Revisions
  /search:
    get:
      summary: Search
      description: "Searches a site for any questions which fit the given criteria.\n
        \nThis method is intentionally quite limited. For more general searching,
        you should use a proper internet search engine restricted to the domain of
        the site in question.\n \nAt least one of tagged or intitle must be set on
        this method. nottagged is only used if tagged is also set, for performance
        reasons.\n \ntagged and nottagged are semi-colon delimited list of tags. At
        least 1 tag in tagged will be on each returned question if it is passed, making
        it the OR equivalent of the AND version of tagged on /questions.\n \nThe sorts
        accepted by this method operate on the follow fields of the question object:\n
        - activity - last_activity_date\n - creation - creation_date\n - votes - score\n
        - relevance - matches the relevance tab on the site itself Does not accept
        min or max\n  activity is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of questions."
      operationId: searches-a-site-for-any-questions-which-fit-the-given-criteria-this-method-is-intentionally-quite-li
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: intitle
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = relevance => none
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = relevance => none
      - in: query
        name: nottagged
        description: String list (semicolon delimited)
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: tagged
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Search
  /search/advanced:
    get:
      summary: Advanced Search
      description: "Searches a site for any questions which fit the given criteria.\n
        \nSearch criteria are expressed using the following parameters:\n  - q - a
        free form text parameter, will match all question properties based on an undocumented
        algorithm.\n - accepted - true to return only questions with accepted answers,
        false to return only those without. Omit to elide constraint.\n - answers
        - the minimum number of answers returned questions must have.\n - body - text
        which must appear in returned questions' bodies.\n - closed - true to return
        only closed questions, false to return only open ones. Omit to elide constraint.\n
        - migrated - true to return only questions migrated away from a site, false
        to return only those not. Omit to elide constraint.\n - notice - true to return
        only questions with post notices, false to return only those without. Omit
        to elide constraint.\n - nottagged - a semicolon delimited list of tags, none
        of which will be present on returned questions.\n - tagged - a semicolon delimited
        list of tags, of which at least one will be present on all returned questions.\n
        - title - text which must appear in returned questions' titles.\n - user -
        the id of the user who must own the questions returned.\n - url - a url which
        must be contained in a post, may include a wildcard.\n - views - the minimum
        number of views returned questions must have.\n - wiki - true to return only
        community wiki questions, false to return only non-community wiki ones. Omit
        to elide constraint.\n  \nAt least one additional parameter must be set if
        nottagged is set, for performance reasons.\n \nThe sorts accepted by this
        method operate on the follow fields of the question object:\n - activity -
        last_activity_date\n - creation - creation_date\n - votes - score\n - relevance
        - matches the relevance tab on the site itself Does not accept min or max\n
        \ activity is the default sort.\n \n It is possible to create moderately complex
        queries using sort, min, max, fromdate, and todate.\n \nThis method returns
        a list of questions."
      operationId: searches-a-site-for-any-questions-which-fit-the-given-criteria-search-criteria-are-expressed-using-t
      x-api-path-slug: searchadvanced-get
      parameters:
      - in: query
        name: accepted
      - in: query
        name: answers
      - in: query
        name: body
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: closed
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = relevance => none
      - in: query
        name: migrated
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = relevance => none
      - in: query
        name: notice
      - in: query
        name: nottagged
        description: String list (semicolon delimited)
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: q
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: tagged
        description: String list (semicolon delimited)
      - in: query
        name: title
      - in: query
        name: todate
        description: Unix date
      - in: query
        name: url
      - in: query
        name: user
      - in: query
        name: views
      - in: query
        name: wiki
      responses:
        200:
          description: OK
      tags:
      - Search
  /similar:
    get:
      summary: Get Similar
      description: "Returns questions which are similar to a hypothetical one based
        on a title and tag combination.\n \nThis method is roughly equivalent to a
        site's related questions suggestion on the ask page.\n \nThis method is useful
        for correlating data outside of a Stack Exchange site with similar content
        within one.\n \nNote that title must always be passed as a parameter. tagged
        and nottagged are optional, semi-colon delimited lists of tags.\n \nIf tagged
        is passed it is treated as a preference, there is no guarantee that questions
        returned will have any of those tags. nottagged is treated as a requirement,
        no questions will be returned with those tags.\n \nThe sorts accepted by this
        method operate on the follow fields of the question object:\n - activity -
        last_activity_date\n - creation - creation_date\n - votes - score\n - relevance
        - order by \"how similar\" the questions are, most likely candidate first
        with a descending order Does not accept min or max\n  activity is the default
        sort.\n \n It is possible to create moderately complex queries using sort,
        min, max, fromdate, and todate.\n \nThis method returns a list of questions."
      operationId: returns-questions-which-are-similar-to-a-hypothetical-one-based-on-a-title-and-tag-combination-this-
      x-api-path-slug: similar-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = relevance => none
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = relevance => none
      - in: query
        name: nottagged
        description: String list (semicolon delimited)
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: tagged
        description: String list (semicolon delimited)
      - in: query
        name: title
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Similar
  /sites:
    get:
      summary: Get Sites
      description: "Returns all sites in the network.\n \nThis method allows for discovery
        of new sites, and changes to existing ones. Be aware that unlike normal API
        methods, this method should be fetched very infrequently, it is very unusual
        for these values to change more than once on any given day. It is suggested
        that you cache its return for at least one day, unless your app encounters
        evidence that it has changed (such as from the /info method).\n \nThe pagesize
        parameter for this method is unbounded, in acknowledgement that for many applications
        repeatedly fetching from /sites would complicate start-up tasks needlessly.\n
        \nThis method returns a list of sites."
      operationId: returns-all-sites-in-the-network-this-method-allows-for-discovery-of-new-sites-and-changes-to-existi
      x-api-path-slug: sites-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Sites
  /suggested-edits:
    get:
      summary: Get Suggested Edits
      description: "Returns all the suggested edits in the systems.\n \nThis method
        returns a list of suggested-edits.\n \nThe sorts accepted by this method operate
        on the follow fields of the suggested_edit object:\n - creation - creation_date\n
        - approval - approval_date Does not return unapproved suggested_edits\n -
        rejection - rejection_date Does not return unrejected suggested_edits\n  creation
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate."
      operationId: returns-all-the-suggested-edits-in-the-systems-this-method-returns-a-list-of-suggestededits-the-sort
      x-api-path-slug: suggestededits-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: min
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Suggested Edits
  /suggested-edits/{ids}:
    get:
      summary: Get Suggested Edit
      description: "Returns suggested edits identified in ids.\n \n{ids} can contain
        up to 100 semicolon delimited ids, to find ids programatically look for suggested_edit_id
        on suggested_edit objects.\n \nThe sorts accepted by this method operate on
        the follow fields of the suggested_edit object:\n - creation - creation_date\n
        - approval - approval_date Does not return unapproved suggested_edits\n -
        rejection - rejection_date Does not return unrejected suggested_edits\n  creation
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of suggested-edits."
      operationId: returns-suggested-edits-identified-in-ids-ids-can-contain-up-to-100-semicolon-delimited-ids-to-find-
      x-api-path-slug: suggestededitsids-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: min
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Suggested Edits
  /tags:
    get:
      summary: Get Tags
      description: "Returns the tags found on a site.\n \nThe inname parameter lets
        a consumer filter down to tags that contain a certain substring. For example,
        inname=own would return both \"download\" and \"owner\" amongst others.\n
        \nThis method returns a list of tags.\n \nThe sorts accepted by this method
        operate on the follow fields of the tag object:\n - popular - count\n - activity
        - the creation_date of the last question asked with the tag\n - name - name\n
        \ popular is the default sort.\n \n It is possible to create moderately complex
        queries using sort, min, max, fromdate, and todate."
      operationId: returns-the-tags-found-on-a-site-the-inname-parameter-lets-a-consumer-filter-down-to-tags-that-conta
      x-api-path-slug: tags-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: inname
      - in: query
        name: max
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: min
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/moderator-only:
    get:
      summary: Get Tags Moderator Only
      description: "Returns the tags found on a site that only moderators can use.\n
        \nThe inname parameter lets a consumer filter down to tags that contain a
        certain substring. For example, inname=own would return both \"download\"
        and \"owner\" amongst others.\n \nThis method returns a list of tags.\n \nThe
        sorts accepted by this method operate on the follow fields of the tag object:\n
        - popular - count\n - activity - the creation_date of the last question asked
        with the tag\n - name - name\n  popular is the default sort.\n \n It is possible
        to create moderately complex queries using sort, min, max, fromdate, and todate."
      operationId: returns-the-tags-found-on-a-site-that-only-moderators-can-use-the-inname-parameter-lets-a-consumer-f
      x-api-path-slug: tagsmoderatoronly-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: inname
      - in: query
        name: max
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: min
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/required:
    get:
      summary: Get Tags Requred
      description: "Returns the tags found on a site that fulfill required tag constraints
        on questions.\n \nThe inname parameter lets a consumer filter down to tags
        that contain a certain substring. For example, inname=own would return both
        \"download\" and \"owner\" amongst others.\n \nThis method returns a list
        of tags.\n \nThe sorts accepted by this method operate on the follow fields
        of the tag object:\n - popular - count\n - activity - the creation_date of
        the last question asked with the tag\n - name - name\n  popular is the default
        sort.\n \n It is possible to create moderately complex queries using sort,
        min, max, fromdate, and todate."
      operationId: returns-the-tags-found-on-a-site-that-fulfill-required-tag-constraints-on-questions-the-inname-param
      x-api-path-slug: tagsrequired-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: inname
      - in: query
        name: max
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: min
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Required
  /tags/synonyms:
    get:
      summary: Get Tags Synonyms
      description: "Returns all tag synonyms found a site.\n \nWhen searching for
        synonyms of specific tags, it is better to use /tags/{tags}/synonyms over
        this method.\n \nThe sorts accepted by this method operate on the follow fields
        of the tag_synonym object:\n - creation - creation_date\n - applied - applied_count\n
        - activity - last_applied_date\n  creation is the default sort.\n \n It is
        possible to create moderately complex queries using sort, min, max, fromdate,
        and todate.\n \nThis method returns a list of tag_synonyms."
      operationId: returns-all-tag-synonyms-found-a-site-when-searching-for-synonyms-of-specific-tags-it-is-better-to-u
      x-api-path-slug: tagssynonyms-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = creation => datesort = applied => numbersort = activity
          => date
      - in: query
        name: min
        description: sort = creation => datesort = applied => numbersort = activity
          => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Synonyms
  /tags/{tags}/faq:
    get:
      summary: Get Tags FAQ
      description: "Returns the frequently asked questions for the given set of tags
        in {tags}.\n \nFor a question to be returned, it must have all the tags in
        {tags} and be considered \"frequently asked\". The exact algorithm for determining
        whether a question is considered a FAQ is subject to change at any time.\n
        \n{tags} can contain up to 5 individual tags per request.\n \nThis method
        returns a list of questions."
      operationId: returns-the-frequently-asked-questions-for-the-given-set-of-tags-in-tags-for-a-question-to-be-return
      x-api-path-slug: tagstagsfaq-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: path
        name: tags
        description: String list (semicolon delimited)
      responses:
        200:
          description: OK
      tags:
      - Tags
      - FAQ
  /tags/{tags}/info:
    get:
      summary: Get Tags Info
      description: "Returns tag objects representing the tags in {tags} found on the
        site.\n \nThis method diverges from the standard naming patterns to avoid
        to conflicting with existing methods, due to the free form nature of tag names.\n
        \nThis method returns a list of tags.\n \nThe sorts accepted by this method
        operate on the follow fields of the tag object:\n - popular - count\n - activity
        - the creation_date of the last question asked with the tag\n - name - name\n
        \ popular is the default sort.\n \n It is possible to create moderately complex
        queries using sort, min, max, fromdate, and todate."
      operationId: returns-tag-objects-representing-the-tags-in-tags-found-on-the-site-this-method-diverges-from-the-st
      x-api-path-slug: tagstagsinfo-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: min
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: path
        name: tags
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Information
  /tags/{tags}/related:
    get:
      summary: Get Tags Related
      description: "Returns the tags that are most related to those in {tags}.\n \nIncluding
        multiple tags in {tags} is equivalent to asking for \"tags related to tag
        #1 and tag #2\" not \"tags related to tag #1 or tag #2\".\n \ncount on tag
        objects returned is the number of question with that tag that also share all
        those in {tags}.\n \n{tags} can contain up to 4 individual tags per request.\n
        \nThis method returns a list of tags."
      operationId: returns-the-tags-that-are-most-related-to-those-in-tags-including-multiple-tags-in-tags-is-equivalen
      x-api-path-slug: tagstagsrelated-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: path
        name: tags
        description: String list (semicolon delimited)
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Related
  /tags/{tags}/synonyms:
    get:
      summary: Get Tags Synonyms
      description: "Gets all the synonyms that point to the tags identified in {tags}.
        If you're looking to discover all the tag synonyms on a site, use the /tags/synonyms
        methods instead of call this method on all tags.\n \n{tags} can contain up
        to 20 individual tags per request.\n \nThe sorts accepted by this method operate
        on the follow fields of the tag_synonym object:\n - creation - creation_date\n
        - applied - applied_count\n - activity - last_applied_date\n  creation is
        the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of tag synonyms."
      operationId: gets-all-the-synonyms-that-point-to-the-tags-identified-in-tags-if-youre-looking-to-discover-all-the
      x-api-path-slug: tagstagssynonyms-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = creation => datesort = applied => numbersort = activity
          => date
      - in: query
        name: min
        description: sort = creation => datesort = applied => numbersort = activity
          => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: path
        name: tags
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Synonyms
  /tags/{tags}/wikis:
    get:
      summary: Get Tags Wikis
      description: "Returns the wikis that go with the given set of tags in {tags}.\n
        \nBe aware that not all tags have wikis.\n \n{tags} can contain up to 20 individual
        tags per request.\n \nThis method returns a list of tag wikis."
      operationId: returns-the-wikis-that-go-with-the-given-set-of-tags-in-tags-be-aware-that-not-all-tags-have-wikis-t
      x-api-path-slug: tagstagswikis-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: path
        name: tags
        description: String list (semicolon delimited)
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Wikis
  /tags/{tag}/top-answerers/{period}:
    get:
      summary: Get Tags Top Answers
      description: "Returns the top 30 answerers active in a single tag, of either
        all-time or the last 30 days.\n \nThis is a view onto the data presented on
        the tag info page on the sites.\n \nThis method returns a list of tag score
        objects."
      operationId: returns-the-top-30-answerers-active-in-a-single-tag-of-either-alltime-or-the-last-30-days-this-is-a-
      x-api-path-slug: tagstagtopanswerersperiod-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: path
        name: period
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: path
        name: tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Top Answers
  /tags/{tag}/top-askers/{period}:
    get:
      summary: Get Tags Top Askers
      description: "Returns the top 30 askers active in a single tag, of either all-time
        or the last 30 days.\n \nThis is a view onto the data presented on the tag
        info page on the sites.\n \nThis method returns a list of tag score objects."
      operationId: returns-the-top-30-askers-active-in-a-single-tag-of-either-alltime-or-the-last-30-days-this-is-a-vie
      x-api-path-slug: tagstagtopaskersperiod-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: path
        name: period
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: path
        name: tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Top Askers
  /users:
    get:
      summary: Get Users
      description: "Returns all users on a site.\n \nThis method returns a list of
        users.\n \nThe sorts accepted by this method operate on the follow fields
        of the user object:\n - reputation - reputation\n - creation - creation_date\n
        - name - display_name\n - modified - last_modified_date\n  reputation is the
        default sort.\n \n It is possible to create moderately complex queries using
        sort, min, max, fromdate, and todate.\n \nThe inname parameter lets consumers
        filter the results down to just those users with a certain substring in their
        display name. For example, inname=kevin will return all users with both users
        named simply \"Kevin\" or those with Kevin as one of (or part of) their names;
        such as \"Kevin Montrose\"."
      operationId: returns-all-users-on-a-site-this-method-returns-a-list-of-users-the-sorts-accepted-by-this-method-op
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: inname
      - in: query
        name: max
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: min
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/moderators:
    get:
      summary: Get User Moderators
      description: "Gets those users on a site who can exercise moderation powers.\n
        \nNote, employees of Stack Exchange Inc. will be returned if they have been
        granted moderation powers on a site even if they have never been appointed
        or elected explicitly. This method checks abilities, not the manner in which
        they were obtained.\n \nThe sorts accepted by this method operate on the follow
        fields of the user object:\n - reputation - reputation\n - creation - creation_date\n
        - name - display_name\n - modified - last_modified_date\n  reputation is the
        default sort.\n \n It is possible to create moderately complex queries using
        sort, min, max, fromdate, and todate.\n \nThis method returns a list of users."
      operationId: gets-those-users-on-a-site-who-can-exercise-moderation-powers-note-employees-of-stack-exchange-inc-w
      x-api-path-slug: usersmoderators-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: min
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Moderators
  /users/moderators/elected:
    get:
      summary: Get Users Moderators Elected
      description: "Returns those users on a site who both have moderator powers,
        and were actually elected.\n \nThis method excludes Stack Exchange Inc. employees,
        unless they were actually elected moderators on a site (which can only have
        happened prior to their employment).\n \nThe sorts accepted by this method
        operate on the follow fields of the user object:\n - reputation - reputation\n
        - creation - creation_date\n - name - display_name\n - modified - last_modified_date\n
        \ reputation is the default sort.\n \n It is possible to create moderately
        complex queries using sort, min, max, fromdate, and todate.\n \nThis method
        returns a list of users."
      operationId: returns-those-users-on-a-site-who-both-have-moderator-powers-and-were-actually-elected-this-method-e
      x-api-path-slug: usersmoderatorselected-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: min
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Moderators
  /users/{ids}:
    get:
      summary: Get User
      description: "Gets the users identified in ids in {ids}.\n \nTypically this
        method will be called to fetch user profiles when you have obtained user ids
        from some other source, such as /questions.\n \n{ids} can contain up to 100
        semicolon delimited ids, to find ids programatically look for user_id on user
        or shallow_user objects.\n \nThe sorts accepted by this method operate on
        the follow fields of the user object:\n - reputation - reputation\n - creation
        - creation_date\n - name - display_name\n - modified - last_modified_date\n
        \ reputation is the default sort.\n \n It is possible to create moderately
        complex queries using sort, min, max, fromdate, and todate.\n \nThis method
        returns a list of users."
      operationId: gets-the-users-identified-in-ids-in-ids-typically-this-method-will-be-called-to-fetch-user-profiles-
      x-api-path-slug: usersids-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: min
        description: sort = reputation => numbersort = creation => datesort = name
          => stringsort = modified => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
  /users/{ids}/answers:
    get:
      summary: Get User Answers
      description: "Returns the answers the users in {ids} have posted.\n \n{ids}
        can contain up to 100 semicolon delimited ids, to find ids programatically
        look for user_id on user or shallow_user objects.\n \nThe sorts accepted by
        this method operate on the follow fields of the answer object:\n - activity
        - last_activity_date\n - creation - creation_date\n - votes - score\n  activity
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of answers."
      operationId: returns-the-answers-the-users-in-ids-have-posted-ids-can-contain-up-to-100-semicolon-delimited-ids-t
      x-api-path-slug: usersidsanswers-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Answers
  /users/{ids}/associated:
    get:
      summary: Get User Associated
      description: "Returns all of a user's associated accounts, given their account_ids
        in {ids}.\n \n{ids} can contain up to 100 semicolon delimited ids, to find
        ids programatically look for account_id on user objects.\n \nThis method returns
        a list of network_users."
      operationId: returns-all-of-a-users-associated-accounts-given-their-account-ids-in-ids-ids-can-contain-up-to-100-
      x-api-path-slug: usersidsassociated-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Users
      - Associated
  /users/{ids}/badges:
    get:
      summary: Get User Badges
      description: "Get the badges the users in {ids} have earned.\n \nBadge sorts
        are a tad complicated. For the purposes of sorting (and min/max) tag_based
        is considered to be greater than named.\n \nThis means that you can get a
        list of all tag based badges a user has by passing min=tag_based, and conversely
        all the named badges by passing max=named, with sort=type.\n \nFor ranks,
        bronze is greater than silver which is greater than gold. Along with sort=rank,
        set max=gold for just gold badges, max=silver&min=silver for just silver,
        and min=bronze for just bronze.\n \nrank is the default sort.\n \n{ids} can
        contain up to 100 semicolon delimited ids, to find ids programatically look
        for user_id on user or shallow_user objects.\n \nThis method returns a list
        of badges."
      operationId: get-the-badges-the-users-in-ids-have-earned-badge-sorts-are-a-tad-complicated-for-the-purposes-of-so
      x-api-path-slug: usersidsbadges-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = rank => stringsort = name => stringsort = type => stringsort
          = awarded => date
      - in: query
        name: min
        description: sort = rank => stringsort = name => stringsort = type => stringsort
          = awarded => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Badges
  /users/{ids}/comments:
    get:
      summary: Get User Comments
      description: "Get the comments posted by users in {ids}.\n \n{ids} can contain
        up to 100 semicolon delimited ids, to find ids programatically look for user_id
        on user or shallow_user objects.\n \nThe sorts accepted by this method operate
        on the follow fields of the comment object:\n - creation - creation_date\n
        - votes - score\n  creation is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of comments."
      operationId: get-the-comments-posted-by-users-in-ids-ids-can-contain-up-to-100-semicolon-delimited-ids-to-find-id
      x-api-path-slug: usersidscomments-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = creation => datesort = votes => number
      - in: query
        name: min
        description: sort = creation => datesort = votes => number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Comments
  /users/{ids}/comments/{toid}:
    get:
      summary: Get User Comments Told
      description: "Get the comments that the users in {ids} have posted in reply
        to the single user identified in {toid}.\n \nThis method is useful for extracting
        conversations, especially over time or across multiple posts.\n \n{ids} can
        contain up to 100 semicolon delimited ids, to find ids programatically look
        for user_id on user or shallow_user objects. {toid} can contain only 1 id,
        found in the same manner as those in {ids}.\n \nThe sorts accepted by this
        method operate on the follow fields of the comment object:\n - creation -
        creation_date\n - votes - score\n  creation is the default sort.\n \n It is
        possible to create moderately complex queries using sort, min, max, fromdate,
        and todate.\n \nThis method returns a list of comments."
      operationId: get-the-comments-that-the-users-in-ids-have-posted-in-reply-to-the-single-user-identified-in-toid-th
      x-api-path-slug: usersidscommentstoid-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = creation => datesort = votes => number
      - in: query
        name: min
        description: sort = creation => datesort = votes => number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      - in: path
        name: toid
      responses:
        200:
          description: OK
      tags:
      - Users
      - Comments
  /users/{ids}/favorites:
    get:
      summary: Get User Favorites
      description: "Get the questions that users in {ids} have favorited.\n \nThis
        method is effectively a view onto a user's favorites tab.\n \n{ids} can contain
        up to 100 semicolon delimited ids, to find ids programatically look for user_id
        on user or shallow_user objects.\n \nThe sorts accepted by this method operate
        on the follow fields of the question object:\n - activity - last_activity_date\n
        - creation - creation_date\n - votes - score\n - added - when the user favorited
        the question\n  activity is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of questions."
      operationId: get-the-questions-that-users-in-ids-have-favorited-this-method-is-effectively-a-view-onto-a-users-fa
      x-api-path-slug: usersidsfavorites-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = added => date
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = added => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Favorites
  /users/{ids}/mentioned:
    get:
      summary: Get User Mentioned
      description: "Gets all the comments that the users in {ids} were mentioned in.\n
        \nNote, to count as a mention the comment must be considered to be \"in reply
        to\" a user. Most importantly, this means that a comment can only be in reply
        to a single user.\n \n{ids} can contain up to 100 semicolon delimited ids,
        to find ids programatically look for user_id on user or shallow_user objects.\n
        \nThe sorts accepted by this method operate on the follow fields of the comment
        object:\n - creation - creation_date\n - votes - score\n  It is possible to
        create moderately complex queries using sort, min, max, fromdate, and todate.\n
        \nThis method returns a list of comments."
      operationId: gets-all-the-comments-that-the-users-in-ids-were-mentioned-in-note-to-count-as-a-mention-the-comment
      x-api-path-slug: usersidsmentioned-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = creation => datesort = votes => number
      - in: query
        name: min
        description: sort = creation => datesort = votes => number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Mentioned
  /users/{ids}/merges:
    get:
      summary: Get User Merges
      description: "Returns a record of merges that have occurred involving the passed
        account ids.\n \nThis method allows you to take now invalid account ids and
        find what account they've become, or take currently valid account ids and
        find which ids were equivalent in the past.\n \nThis is most useful when confirming
        that an account_id is in fact \"new\" to an application.\n \nAccount merges
        can happen for a wide range of reasons, applications should not make assumptions
        that merges have particular causes.\n \nNote that accounts are managed at
        a network level, users on a site may be merged due to an account level merge
        but there is no guarantee that a merge has an effect on any particular site.\n
        \nThis method returns a list of account_merge."
      operationId: returns-a-record-of-merges-that-have-occurred-involving-the-passed-account-ids-this-method-allows-yo
      x-api-path-slug: usersidsmerges-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: page
      - in: query
        name: pagesize
      responses:
        200:
          description: OK
      tags:
      - Users
      - Merges
  /users/{ids}/questions:
    get:
      summary: Get User Questions
      description: "Gets the questions asked by the users in {ids}.\n \n{ids} can
        contain up to 100 semicolon delimited ids, to find ids programatically look
        for user_id on user or shallow_user objects.\n \nThe sorts accepted by this
        method operate on the follow fields of the question object:\n - activity -
        last_activity_date\n - creation - creation_date\n - votes - score\n  activity
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of questions."
      operationId: gets-the-questions-asked-by-the-users-in-ids-ids-can-contain-up-to-100-semicolon-delimited-ids-to-fi
      x-api-path-slug: usersidsquestions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Questions
  /users/{ids}/questions/featured:
    get:
      summary: Get User Questions Featured
      description: "Gets the questions on which the users in {ids} have active bounties.\n
        \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
        look for user_id on user or shallow_user objects.\n \nThe sorts accepted by
        this method operate on the follow fields of the question object:\n - activity
        - last_activity_date\n - creation - creation_date\n - votes - score\n  activity
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of questions."
      operationId: gets-the-questions-on-which-the-users-in-ids-have-active-bounties-ids-can-contain-up-to-100-semicolo
      x-api-path-slug: usersidsquestionsfeatured-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Featured
  /users/{ids}/questions/no-answers:
    get:
      summary: Get User Questions No Answers
      description: "Gets the questions asked by the users in {ids} which have no answers.\n
        \nQuestions returns by this method actually have zero undeleted answers. It
        is completely disjoint /users/{ids}/questions/unanswered and /users/{ids}/questions/unaccepted,
        which only return questions with at least one answer, subject to other contraints.\n
        \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
        look for user_id on user or shallow_user objects.\n \nThe sorts accepted by
        this method operate on the follow fields of the question object:\n - activity
        - last_activity_date\n - creation - creation_date\n - votes - score\n  activity
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of questions."
      operationId: gets-the-questions-asked-by-the-users-in-ids-which-have-no-answers-questions-returns-by-this-method-
      x-api-path-slug: usersidsquestionsnoanswers-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Answers
  /users/{ids}/questions/unaccepted:
    get:
      summary: Get User Questions Unnacepted
      description: "Gets the questions asked by the users in {ids} which have at least
        one answer, but no accepted answer.\n \nQuestions returned by this method
        have answers, but the owner has not opted to accept any of them.\n \n{ids}
        can contain up to 100 semicolon delimited ids, to find ids programatically
        look for user_id on user or shallow_user objects.\n \nThe sorts accepted by
        this method operate on the follow fields of the question object:\n - activity
        - last_activity_date\n - creation - creation_date\n - votes - score\n  activity
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of questions."
      operationId: gets-the-questions-asked-by-the-users-in-ids-which-have-at-least-one-answer-but-no-accepted-answer-q
      x-api-path-slug: usersidsquestionsunaccepted-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Unaccepted
  /users/{ids}/questions/unanswered:
    get:
      summary: Get User Questions Unanswered
      description: "Gets the questions asked by the users in {ids} which the site
        consideres unanswered, while still having at least one answer posted.\n \nThese
        rules are subject to change, but currently any question without at least one
        upvoted or accepted answer is considered unanswered.\n \nTo get the set of
        questions that a user probably considers unanswered, the returned questions
        should be unioned with those returned by /users/{id}/questions/no-answers.
        These methods are distinct so that truly unanswered (that is, zero posted
        answers) questions can be easily separated from mearly poorly or inadequately
        answered ones.\n \n{ids} can contain up to 100 semicolon delimited ids, to
        find ids programatically look for user_id on user or shallow_user objects.\n
        \nThe sorts accepted by this method operate on the follow fields of the question
        object:\n - activity - last_activity_date\n - creation - creation_date\n -
        votes - score\n  activity is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of questions."
      operationId: gets-the-questions-asked-by-the-users-in-ids-which-the-site-consideres-unanswered-while-still-having
      x-api-path-slug: usersidsquestionsunanswered-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Unanswerd
  /users/{ids}/reputation:
    get:
      summary: Get User Reputation
      description: "Gets a subset of the reputation changes for users in {ids}.\n
        \nReputation changes are intentionally scrubbed of some data to make it difficult
        to correlate votes on particular posts with user reputation changes. That
        being said, this method returns enough data for reasonable display of reputation
        trends.\n \n{ids} can contain up to 100 semicolon delimited ids, to find ids
        programatically look for user_id on user or shallow_user objects.\n \nThis
        method returns a list of reputation objects."
      operationId: gets-a-subset-of-the-reputation-changes-for-users-in-ids-reputation-changes-are-intentionally-scrubb
      x-api-path-slug: usersidsreputation-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Reputation
  /users/{ids}/reputation-history:
    get:
      summary: Get User Reputation History
      description: "Returns users' public reputation history.\n \nThis method returns
        a list of reputation_history."
      operationId: returns-users-public-reputation-history-this-method-returns-a-list-of-reputation-history
      x-api-path-slug: usersidsreputationhistory-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Reputation
      - History
  /users/{ids}/suggested-edits:
    get:
      summary: Get User Suggested Edits
      description: "Returns the suggested edits a users in {ids} have submitted.\n
        \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
        look for user_id on user or shallow_user objects.\n \nThe sorts accepted by
        this method operate on the follow fields of the suggested_edit object:\n -
        creation - creation_date\n - approval - approval_date Does not return unapproved
        suggested_edits\n - rejection - rejection_date Does not return unrejected
        suggested_edits\n  creation is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of suggested-edits."
      operationId: returns-the-suggested-edits-a-users-in-ids-have-submitted-ids-can-contain-up-to-100-semicolon-delimi
      x-api-path-slug: usersidssuggestededits-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: min
        description: sort = creation => datesort = approval => datesort = rejection
          => date
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Suggested Edits
  /users/{ids}/tags:
    get:
      summary: Get User Tags
      description: "Returns the tags the users identified in {ids} have been active
        in.\n \nThis route corresponds roughly to user's stats tab, but does not include
        tag scores. A subset of tag scores are available (on a single user basis)
        in /users/{id}/top-answer-tags and /users/{id}/top-question-tags.\n \n{ids}
        can contain up to 100 semicolon delimited ids, to find ids programatically
        look for user_id on user or shallow_user objects.\n \nThe sorts accepted by
        this method operate on the follow fields of the tag object:\n - popular -
        count\n - activity - the creation_date of the last question asked with the
        tag\n - name - name\n  popular is the default sort.\n \n It is possible to
        create moderately complex queries using sort, min, max, fromdate, and todate.\n
        \nThis method returns a list of tags."
      operationId: returns-the-tags-the-users-identified-in-ids-have-been-active-in-this-route-corresponds-roughly-to-u
      x-api-path-slug: usersidstags-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: min
        description: sort = popular => numbersort = activity => datesort = name =>
          string
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Tags
  /users/{ids}/timeline:
    get:
      summary: Get User Timeline
      description: "Returns a subset of the actions the users in {ids} have taken
        on the site.\n \nThis method returns users' posts, edits, and earned badges
        in the order they were accomplished. It is possible to filter to just a window
        of activity using the fromdate and todate parameters.\n \n{ids} can contain
        up to 100 semicolon delimited ids, to find ids programatically look for user_id
        on user or shallow_user objects.\n \nThis method returns a list of user timeline
        objects."
      operationId: returns-a-subset-of-the-actions-the-users-in-ids-have-taken-on-the-site-this-method-returns-users-po
      x-api-path-slug: usersidstimeline-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Timiline
  /users/{id}/inbox:
    get:
      summary: Get User Inbox
      description: "Returns a user's inbox.\n \nThis method requires an access_token,
        with a scope containing \"read_inbox\".\n \nThis method is effectively an
        alias for /inbox. It is provided for consumers who make strong assumptions
        about operating within the context of a single site rather than the Stack
        Exchange network as a whole.\n \n{id} can contain a single id, to find it
        programatically look for user_id on user or shallow_user objects.\n \nThis
        method returns a list of inbox items."
      operationId: returns-a-users-inbox-this-method-requires-an-access-token-with-a-scope-containing-read-inbox-this-m
      x-api-path-slug: usersidinbox-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Email
      - Inbox
  /users/{id}/inbox/unread:
    get:
      summary: Get User Inbox Unread
      description: "Returns the unread items in a user's inbox.\n \nThis method requires
        an access_token, with a scope containing \"read_inbox\".\n \nThis method is
        effectively an alias for /inbox/unread. It is provided for consumers who make
        strong assumptions about operating within the context of a single site rather
        than the Stack Exchange network as a whole.\n \n{id} can contain a single
        id, to find it programatically look for user_id on user or shallow_user objects.\n
        \nThis method returns a list of inbox items."
      operationId: returns-the-unread-items-in-a-users-inbox-this-method-requires-an-access-token-with-a-scope-containi
      x-api-path-slug: usersidinboxunread-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: since
        description: Unix date
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Email
      - Inbox
  /users/{id}/notifications:
    get:
      summary: Get User Notifications
      description: "Returns a user's notifications.\n \nThis method requires an access_token,
        with a scope containing \"read_inbox\".\n \nThis method returns a list of
        notifications."
      operationId: returns-a-users-notifications-this-method-requires-an-access-token-with-a-scope-containing-read-inbo
      x-api-path-slug: usersidnotifications-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Notifications
  /users/{id}/notifications/unread:
    get:
      summary: Get User Notifications Unread
      description: "Returns a user's unread notifications.\n \nThis method requires
        an access_token, with a scope containing \"read_inbox\".\n \nThis method returns
        a list of notifications."
      operationId: returns-a-users-unread-notifications-this-method-requires-an-access-token-with-a-scope-containing-re
      x-api-path-slug: usersidnotificationsunread-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Notifications
  /users/{id}/privileges:
    get:
      summary: Get User Preveleges
      description: "Returns the privileges a user has.\n \nApplications are encouraged
        to calculate privileges themselves, without repeated queries to this method.
        A simple check against the results returned by /privileges and user.user_type
        would be sufficient.\n \n{id} can contain only a single, to find it programatically
        look for user_id on user or shallow_user objects.\n \nThis method returns
        a list of privileges."
      operationId: returns-the-privileges-a-user-has-applications-are-encouraged-to-calculate-privileges-themselves-wit
      x-api-path-slug: usersidprivileges-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Privileges
  /users/{id}/reputation-history/full:
    get:
      summary: Get User Reputation History Full
      description: "Returns a user's full reputation history, including private events.\n
        \nThis method requires an access_token, with a scope containing \"private_info\".\n
        \nThis method returns a list of reputation_history."
      operationId: returns-a-users-full-reputation-history-including-private-events-this-method-requires-an-access-toke
      x-api-path-slug: usersidreputationhistoryfull-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Reputation
  /users/{id}/tags/{tags}/top-answers:
    get:
      summary: Get User Tags Top Answers
      description: "Returns the top 30 answers a user has posted in response to questions
        with the given tags.\n \n{id} can contain a single id, to find it programatically
        look for user_id on user or shallow_user objects. {tags} is limited to 5 tags,
        passing more will result in an error.\n \nThe sorts accepted by this method
        operate on the follow fields of the answer object:\n - activity - last_activity_date\n
        - creation - creation_date\n - votes - score\n  activity is the default sort.\n
        \n It is possible to create moderately complex queries using sort, min, max,
        fromdate, and todate.\n \nThis method returns a list of answers."
      operationId: returns-the-top-30-answers-a-user-has-posted-in-response-to-questions-with-the-given-tags-id-can-con
      x-api-path-slug: usersidtagstagstopanswers-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: id
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: path
        name: tags
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Tags
      - Answers
  /users/{id}/tags/{tags}/top-questions:
    get:
      summary: Get User Tags Top Questions
      description: "Returns the top 30 questions a user has asked with the given tags.\n
        \n{id} can contain a single id, to find it programatically look for user_id
        on user or shallow_user objects. {tags} is limited to 5 tags, passing more
        will result in an error.\n \nThe sorts accepted by this method operate on
        the follow fields of the question object:\n - activity - last_activity_date\n
        - creation - creation_date\n - votes - score\n  activity is the default sort.\n
        \n It is possible to create moderately complex queries using sort, min, max,
        fromdate, and todate.\n \nThis method returns a list of questions."
      operationId: returns-the-top-30-questions-a-user-has-asked-with-the-given-tags-id-can-contain-a-single-id-to-find
      x-api-path-slug: usersidtagstagstopquestions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: id
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: path
        name: tags
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Tags
      - Questions
  /users/{id}/top-answer-tags:
    get:
      summary: Get User Top Answers Tags
      description: "Returns a single user's top tags by answer score.\n \nThis a subset
        of the data returned on a user's tags tab.\n \n{id} can contain a single id,
        to find it programatically look for user_id on user or shallow_user objects.\n
        \nThis method returns a list of top_tag objects."
      operationId: returns-a-single-users-top-tags-by-answer-score-this-a-subset-of-the-data-returned-on-a-users-tags-t
      x-api-path-slug: usersidtopanswertags-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Top Answer Tags
  /users/{id}/top-question-tags:
    get:
      summary: Get User Top Question Tags
      description: "Returns a single user's top tags by question score.\n \nThis a
        subset of the data returned on a user's tags tab.\n \n{id} can contain a single
        id, to find it programatically look for user_id on user or shallow_user objects.\n
        \nThis method returns a list of top_tag objects."
      operationId: returns-a-single-users-top-tags-by-question-score-this-a-subset-of-the-data-returned-on-a-users-tags
      x-api-path-slug: usersidtopquestiontags-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Users
      - Top Question Tags
  /users/{id}/write-permissions:
    get:
      summary: Get User Write Permissions
      description: "Returns the write permissions a user has via the api.\n \nThe
        Stack Exchange API gives users the ability to create, edit, and delete certain
        types. This method returns whether the passed user is capable of performing
        those actions at all, as well as how many times a day they can.\n \nThis method
        does not consider the user's current quota (ie. if they've already exhausted
        it for today) nor any additional restrictions on write access, such as editing
        deleted comments.\n \nThis method returns a list of write_permissions."
      operationId: returns-the-write-permissions-a-user-has-via-the-api-the-stack-exchange-api-gives-users-the-ability-
      x-api-path-slug: usersidwritepermissions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Write Permissions