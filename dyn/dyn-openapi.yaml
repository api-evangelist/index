swagger: "2.0"
x-collection-name: Dyn
x-complete: 1
info:
  title: Dyn
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  accounts:
    get:
      summary: Retrieve email sub-accounts
      description: Retrieving a list of up to 25 Email Sub-Accounts
      operationId: getAccounts
      x-api-path-slug: accounts-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: startindex
        description: An integer to indicate the starting index of where to begin the
          list of sub-accounts
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Email
      - Accounts
    post:
      summary: Create an Email Sub-Account (API)
      description: Creating an Email Sub-Account using the API requires specific syntax
        for the REST API.
      operationId: postAccounts
      x-api-path-slug: accounts-post
      parameters:
      - in: query
        name: address
        description: Address
      - in: query
        name: apikey
        description: Required
      - in: query
        name: bounceurl
        description: Bounce Postback URL
      - in: query
        name: city
        description: City
      - in: query
        name: companyname
        description: Required
      - in: query
        name: country
        description: Two-letter English abbreviation, based on the ISO 3166 standard
      - in: query
        name: generatenewapikey
        description: Used to create a new API key for an existing account (1 or 0)
      - in: query
        name: password
        description: Required
      - in: query
        name: phone
        description: Required
      - in: query
        name: spamurl
        description: Spam Postback URL
      - in: query
        name: state
        description: State
      - in: query
        name: timezone
        description: The timezone of the account, in [+/-]h
      - in: query
        name: tracklinks
        description: Toggle click tracking (1 or 0)
      - in: query
        name: trackopens
        description: Toggle open tracking (1 or 0)
      - in: query
        name: trackunsubscribes
        description: Toggle automatic list-unsubscribe support (1 or 0)
      - in: query
        name: username
        description: Required
      - in: query
        name: zipcode
        description: Zip
      responses:
        200:
          description: OK
      tags:
      - Create.Email
      - Accounts
      - (API)
    put:
      summary: Updating an Email Sub-Account
      description: Updating an Email Sub-Account
      operationId: putAccounts
      x-api-path-slug: accounts-put
      parameters:
      - in: query
        name: address
        description: Address
      - in: query
        name: apikey
        description: Required
      - in: query
        name: bounceurl
        description: Bounce Postback URL
      - in: query
        name: city
        description: City
      - in: query
        name: companyname
        description: Required
      - in: query
        name: country
        description: Two-letter English abbreviation, based on the ISO 3166 standard
      - in: query
        name: generatenewapikey
        description: Used to create a new API key for an existing account (1 or 0)
      - in: query
        name: password
        description: Required
      - in: query
        name: phone
        description: Required
      - in: query
        name: spamurl
        description: Spam Postback URL
      - in: query
        name: state
        description: State
      - in: query
        name: timezone
        description: The timezone of the account, in [+/-]h
      - in: query
        name: tracklinks
        description: Toggle click tracking (1 or 0)
      - in: query
        name: trackopens
        description: Toggle open tracking (1 or 0)
      - in: query
        name: trackunsubscribes
        description: Toggle automatic list-unsubscribe support
      - in: query
        name: unsubscribeurl
        description: Unsubscribe postback URL
      - in: query
        name: username
        description: Required
      - in: query
        name: zipcode
        description: Zip
      responses:
        200:
          description: OK
      tags:
      - Updating.Email
      - Accounts
  accounts/delete:
    post:
      summary: Deleting an Email Sub-Account
      description: Deleting an Email Sub-Account
      operationId: postAccountsDelete
      x-api-path-slug: accountsdelete-post
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: username
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Deleting.Email
      - Accounts
  opens/count:
    get:
      summary: Email Open Count
      description: Returns total number of opens for the specified account for the
        specified date range. Including a date range is highly recommended.
      operationId: getOpensCount
      x-api-path-slug: openscount-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: emailaddress
        description: Email address of recipient for filtering
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: u00a0Email address of sender for filtering
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - .Email
      - Open
      - Count
  recipients/activate:
    post:
      summary: Activate Recipient(s)
      description: Activating a specified Recipientu2019s status
      operationId: postRecipientsActivate
      x-api-path-slug: recipientsactivate-post
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: emailaddress
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Recipients
  recipients/status:
    get:
      summary: Retrieve Recipient(s) Status
      description: Retrieve Recipient(s) Status
      operationId: getRecipientsStatus
      x-api-path-slug: recipientsstatus-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: emailaddress
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Recipients
      - Status
  reports/bounces:
    get:
      summary: Retrieve Email Bounces
      description: Retrieving the Email SPAM Complaints
      operationId: getReportsBounces
      x-api-path-slug: reportsbounces-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: bounce_code - Indicates the code associated with the bounced Email.
      - in: query
        name: bounce_code_id - The numeric code determined by the bounce processor.
      - in: query
        name: bounce_rule - Indicates the rule that caused this email to bounce.
      - in: query
        name: bounce_type
        description: Type of bounce for filtering
      - in: query
        name: bounce_type_id - Indicates whether the bounce type is a hard or soft
          bounce.nValid Values:n1 - Hard Bouncen2 - Soft Bounce
      - in: query
        name: emailaddress
        description: Email address of recipient for filtering
      - in: query
        name: endtime
        description: Required
      - in: query
        name: noheaders
        description: Determines whether or not headers are included in the response
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: sender_id
        description: Identifying number of the sender
      - in: query
        name: startindex
        description: Number indicating where to begin reporting results
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Email
      - Bounces
  reports/bounces/count:
    get:
      summary: Retrieve Count of Email Bounces
      description: Retrieving a total count of Email bounces using the API requires
        specific syntax for the REST API.
      operationId: getReportsBouncesCount
      x-api-path-slug: reportsbouncescount-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Count
      - of
      - Email
      - Bounces
  reports/clicks:
    get:
      summary: Reports on Clicks
      description: Returns a list of links clicked for the specified account during
        the specified date range. Including a date range is highly recommended.
      operationId: getReportsClicks
      x-api-path-slug: reportsclicks-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: emailaddress
        description: Email address of recipient for filtering
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: startindex
        description: Starting index value (optional)
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Clicks
  reports/clicks/count:
    get:
      summary: Retrieve Count of Email Links Clicked
      description: Retrieving a total of Email links clicked
      operationId: getReportsClicksCount
      x-api-path-slug: reportsclickscount-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: domainu00a0
        description: Domain of the recipient, such as &#8220;gmail
      - in: query
        name: emailaddress
        description: Email address of recipient for filteringu0010
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filteringu0010
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Count
      - of
      - Email
      - Links
      - Clicked
  reports/clicks/count/unique:
    get:
      summary: Retrieve Count of Email Links Clicked
      description: Retrieving a total of Email links clicked
      operationId: getReportsClicksCountUnique
      x-api-path-slug: reportsclickscountunique-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: domainu00a0
        description: Domain of the recipient, such as &#8220;gmail
      - in: query
        name: emailaddress
        description: Email address of recipient for filteringu0010
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filteringu0010
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Count
      - of
      - Email
      - Links
      - Clicked
  reports/clicks/unique:
    get:
      summary: Unique Click Report
      description: Returns a list of unique links clicked for the specified account
        during the specified date range. Including a date range is highly recommended.
      operationId: getReportsClicksUnique
      x-api-path-slug: reportsclicksunique-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: emailaddress
        description: Email address of recipient for filtering
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: startindex
        description: Starting index value (optional)
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Unique
      - Click
      - Report
  reports/complaints:
    get:
      summary: Retrieve Email SPAM Complaints
      description: Retrieve Email SPAM Complaints
      operationId: getReportsComplaints
      x-api-path-slug: reportscomplaints-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: startindex
        description: Number indicating where to begin reporting results
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Email
      - SPAM
      - Complaints
  reports/complaints/count:
    get:
      summary: Retrieve Count of Email SPAM Complaints
      description: Retrieving a total count of Email complaints
      operationId: getReportsComplaintsCount
      x-api-path-slug: reportscomplaintscount-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: endtime
        description: Required
      - in: query
        name: starttime
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Count
      - of
      - Email
      - SPAM
      - Complaints
  reports/delivered:
    get:
      summary: Retrieve Emails Delivered
      description: Retrieve Emails Delivered
      operationId: getReportsDelivered
      x-api-path-slug: reportsdelivered-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: startindex
        description: Number indicating where to begin reporting results
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Emails
      - Delivered
  reports/delivered/count:
    get:
      summary: Retrieve Count of Emails Delivered
      description: Retrieve Count of Emails Delivered
      operationId: getReportsDeliveredCount
      x-api-path-slug: reportsdeliveredcount-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Count
      - of
      - Emails
      - Delivered
  reports/issues:
    get:
      summary: Retrieve Email Issues
      description: Retrieve Email Issues
      operationId: getReportsIssues
      x-api-path-slug: reportsissues-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: emailaddress
        description: Email address of recipient for filtering
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: sender_id
        description: Identifying number of the sender
      - in: query
        name: startindex
        description: Number indicating where to begin reporting results
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Email
      - Issues
  reports/issues/count:
    get:
      summary: Retrieve Count of Email Issues
      description: Retrieving a total count of Email issues
      operationId: getReportsIssuesCount
      x-api-path-slug: reportsissuescount-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: endtime
        description: Required
      - in: query
        name: starttime
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Count
      - of
      - Email
      - Issues
  reports/opens/count/unique:
    get:
      summary: Retrieve Count of Email Opens
      description: Returns total number of unique opens for the specified account
        for the specified date range. Including a date range is highly recommended.
      operationId: getReportsOpensCountUnique
      x-api-path-slug: reportsopenscountunique-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: emailaddress
        description: Email address of recipient for filtering
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: u00a0Email address of sender for filtering
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Count
      - of
      - Email
      - Opens
  reports/sent:
    get:
      summary: Retrieve Emails Sent
      description: Retrieve Emails Sent
      operationId: getReportsSent
      x-api-path-slug: reportssent-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: startindex
        description: Number indicating where to begin reporting results
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Emails
      - Sent
  reports/sent/count:
    get:
      summary: Retrieve Count of Emails Sent
      description: Retrieve Count of Emails Sent
      operationId: getReportsSentCount
      x-api-path-slug: reportssentcount-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Count
      - of
      - Emails
      - Sent
  send:
    post:
      summary: Send Email
      description: Sending Email
      operationId: postSend
      x-api-path-slug: send-post
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: bcc
        description: Address(es) to blind copy the email to
      - in: query
        name: bodyhtml
        description: The text/html version of the email; this field may be encoded
          in 7-bit, 8-bit, quoted-printable, or base64
      - in: query
        name: bodytext
        description: The plain/text version of the email; this field may be encoded
          in Base64 (recommended), quoted-printable, 8-bit, or 7-bit
      - in: query
        name: cc
        description: Address(es) to copy the email to
      - in: query
        name: comments
        description: Additional comments about the message
      - in: query
        name: from
        description: Required
      - in: query
        name: importance
        description: A hint from the originator on how important the message is
      - in: query
        name: inreplyto
        description: One or more message identifier(s) of the original message(s)
          to which the current message is a reply
      - in: query
        name: keywords
        description: A comma-separated list of important words and phrases useful
          for recipient
      - in: query
        name: messageid
        description: A unique message identifier that can be passed in via the api
          and override the Dyn automatically generated message id
      - in: query
        name: priority
        description: Values are either normal, urgent, or non-urgent
      - in: query
        name: references
        description: The message identifier(s) of other message(s) to which the current
          message may be related
      - in: query
        name: replyby
        description: The date and time by which a reply is requested
      - in: query
        name: replyto
        description: The email address for the recipient to reply to
      - in: query
        name: resent-date
        description: The date and time that a message is resent in the same format
          as replyby
      - in: query
        name: resent-from
        description: The email address of the person who has resent the message, or
          on whose behalf the message has been resent
      - in: query
        name: resent-messageid
        description: Contains a message identifier for a resent message
      - in: query
        name: resent-replyto
        description: Resent Reply-to in the same format as the replyto header
      - in: query
        name: resent-sender
        description: The email address of the person who has resent the message, if
          this is different from the resent-from value
      - in: query
        name: sender
        description: This is the email address of the agent responsible for sending
          the message
      - in: query
        name: sensitivity
        description: How sensitive it is to disclose this message with values that
          can be either personal, private or company confidential
      - in: query
        name: subject
        description: Required
      - in: query
        name: to
        description: Required
      - in: query
        name: xheaders
        description: Any additional custom X-headers to send in the email
      responses:
        200:
          description: OK
      tags:
      - Send
      - Email
  suppressions:
    get:
      summary: Retrieve Suppression Email Addresses
      description: Retrieving a list of Email addresses on the suppression list
      operationId: getSuppressions
      x-api-path-slug: suppressions-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: startdate
        description: Start date/time range in full, ISO 8601 format
      - in: query
        name: startindex
        description: Starting index value
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Suppression
      - Email
      - resses
    post:
      summary: Add Email Address to Suppression List
      description: Adding one or more recipients to the suppression list
      operationId: postSuppressions
      x-api-path-slug: suppressions-post
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: emailaddress
        description: Required
      responses:
        200:
          description: OK
      tags:
      - .Email
      - ress
      - to
      - Suppression
      - List
  suppressions/count:
    get:
      summary: Retrieve Suppression Count
      description: Retrieving the count of Email addresses on the suppression list
      operationId: getSuppressionsCount
      x-api-path-slug: suppressionscount-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: enddate
        description: End date/time range in full, ISO 8601 format
      - in: query
        name: startdate
        description: Start date/time range in full, ISO 8601 format
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Suppression
      - Count
  xheaders:
    get:
      summary: Retrieving a list of custom X-header field names
      description: Retrieving a list of custom X-header field names
      operationId: getXheaders
      x-api-path-slug: xheaders-get
      parameters:
      - in: query
        name: apikey
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Retrievinglist
      - of
      - custom
      - X-header
      - field
      - names
    post:
      summary: Update Email X-Headers
      description: Updating the custom x-headers of an Email account
      operationId: postXheaders
      x-api-path-slug: xheaders-post
      parameters:
      - in: query
        name: apikey
        description: Required
      responses:
        200:
          description: OK
      tags:
      - .Email
      - X-Headers