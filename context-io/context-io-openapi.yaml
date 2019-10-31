swagger: "2.0"
x-collection-name: Context.IO
x-complete: 1
info:
  title: Context.IO
  description: context-io-is-the-missing-email-api-that-makes-it-easy-and-fast-to-integrate-your-users-email-data-in-your-application-
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /oauth_providers:
    get:
      summary: Get Oauth Provers
      description: List configured OAuth providers.
      operationId: listOauthProviders_
      x-api-path-slug: oauth-providers-get
      responses:
        200:
          description: OK
      tags:
      - Oauth
      - Providers
    post:
      summary: Post Oauth Provers
      description: Adds a new OAuth provider.
      operationId: addOauthProviders_
      x-api-path-slug: oauth-providers-post
      parameters:
      - in: query
        name: provider_consumer_key
        description: The OAuth consumer key
      - in: query
        name: provider_consumer_secret
        description: The OAuth consumer secret
      - in: query
        name: type
        description: Identification of the OAuth provider
      responses:
        200:
          description: OK
      tags:
      - Oauth
      - Providers
  /oauth_providers/{key}:
    get:
      summary: Get Oauth Provers Key
      description: Gets information about a given OAuth provider.
      operationId: getOauthProvider_
      x-api-path-slug: oauth-providerskey-get
      parameters:
      - in: path
        name: key
        description: The consumer key for this external OAuth provider
      responses:
        200:
          description: OK
      tags:
      - Oauth
      - Providers
      - Key
    delete:
      summary: Delete Oauth Provers Key
      description: Removes a given OAuth provider.
      operationId: removeOauthProvider_
      x-api-path-slug: oauth-providerskey-delete
      parameters:
      - in: path
        name: key
        description: The consumer key for this external OAuth provider
      responses:
        200:
          description: OK
      tags:
      - Oauth
      - Providers
      - Key
  /discovery:
    get:
      summary: Get Discovery
      description: Attempts to discover IMAP settings for a given email address.
      operationId: Get_discoverEmailImapSettings_
      x-api-path-slug: discovery-get
      parameters:
      - in: query
        name: email
        description: An email address you want to discover IMAP settings for
      - in: query
        name: source_type
        description: The type of source you want to discover settings for
      responses:
        200:
          description: OK
      tags:
      - Discovery
  /connect_tokens:
    get:
      summary: Get Connect Tokens
      description: Lists connect tokens created with your API key.
      operationId: listConnectTokens_
      x-api-path-slug: connect-tokens-get
      responses:
        200:
          description: OK
      tags:
      - Connect
      - Tokens
    post:
      summary: Post Connect Tokens
      description: Obtains a new connect_token.
      operationId: Create_obtainNewConnectToken_
      x-api-path-slug: connect-tokens-post
      parameters:
      - in: query
        name: callback_url
        description: When the users mailbox is connected to your API key, the browser
          will call this url (GET)
      - in: query
        name: email
        description: The email address of the account to be added
      - in: query
        name: first_name
        description: First name of the account holder
      - in: query
        name: last_name
        description: Last name of the account holder
      - in: query
        name: service_level
        description: Sets the service level of the accounts source to be created
      responses:
        200:
          description: OK
      tags:
      - Connect
      - Tokens
  /connect_tokens/{token}:
    get:
      summary: Get Connect Tokens Token
      description: Gets information about a given connect token.
      operationId: getConnectToken_
      x-api-path-slug: connect-tokenstoken-get
      parameters:
      - in: path
        name: token
        description: The unique random token used for the graphical account creation
          process
      responses:
        200:
          description: OK
      tags:
      - Connect
      - Tokens
      - Token
    delete:
      summary: Delete Connect Tokens Token
      description: Removes a given connect token.
      operationId: removeConnectToken_
      x-api-path-slug: connect-tokenstoken-delete
      parameters:
      - in: path
        name: token
        description: The unique random token used for the graphical account creation
          process
      responses:
        200:
          description: OK
      tags:
      - Connect
      - Tokens
      - Token
  /accounts:
    get:
      summary: Get Accounts
      description: Lists accounts.
      operationId: listAccounts_
      x-api-path-slug: accounts-get
      parameters:
      - in: query
        name: email
        description: Only return account associated to this email address
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      - in: query
        name: status
        description: Only return accounts with sources whose status is of a specific
          value
      - in: query
        name: status_ok
        description: Set to 0 to get all accounts with sources that are not working
          correctly
      - in: query
        name: token
        description: The unique random token used for the graphical account creation
          process
      responses:
        200:
          description: OK
      tags:
      - Accounts
    post:
      summary: Post Accounts
      description: Adds a new account.
      operationId: addAccount_
      x-api-path-slug: accounts-post
      parameters:
      - in: query
        name: email
        description: The primary email address of the account holder
      - in: query
        name: first_name
        description: First name of the account holder
      - in: query
        name: last_name
        description: Last name of the account holder
      - in: query
        name: token
        description: The unique random token used for the graphical account creation
          process
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /accounts/{id}:
    get:
      summary: Get Accounts
      description: Gets details about a given account.
      operationId: getAccount_
      x-api-path-slug: accountsid-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
    put:
      summary: Put Accounts
      description: Modifies a given account.
      operationId: modifyAccount_
      x-api-path-slug: accountsid-put
      parameters:
      - in: query
        name: first_name
        description: First name of the account holder
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: last_name
        description: Last name of the account holder
      responses:
        200:
          description: OK
      tags:
      - Accounts
    delete:
      summary: Delete Accounts
      description: Removes a given account.
      operationId: removeAccount_
      x-api-path-slug: accountsid-delete
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /accounts/{id}/connect_tokens:
    get:
      summary: Get Accounts Connect Tokens
      description: Lists connect tokens created for an account.
      operationId: listAccountConnectTokens_
      x-api-path-slug: accountsidconnect-tokens-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Connect
      - Tokens
    post:
      summary: Post Accounts Connect Tokens
      description: Obtains a new connect_token for a specific account.
      operationId: Create_obtainNewAccountConnectToken_
      x-api-path-slug: accountsidconnect-tokens-post
      parameters:
      - in: query
        name: callback_url
        description: When the users mailbox is connected to your API key, the browser
          will call this url (GET)
      - in: query
        name: email
        description: The email address of the account to be added
      - in: query
        name: first_name
        description: First name of the account holder
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: last_name
        description: Last name of the account holder
      - in: query
        name: service_level
        description: Sets the service level of the accounts source to be created
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Connect
      - Tokens
  /accounts/{id}/connect_tokens/{token}:
    get:
      summary: Get Accounts Connect Tokens Token
      description: Gets information about a given connect token.
      operationId: getAccountConnectToken_
      x-api-path-slug: accountsidconnect-tokenstoken-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: token
        description: The unique random token used to add a second source to an existing
          account
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Connect
      - Tokens
      - Token
    delete:
      summary: Delete Accounts Connect Tokens Token
      description: Remove a given connect token.
      operationId: removeAccountConnectToken_
      x-api-path-slug: accountsidconnect-tokenstoken-delete
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: token
        description: The unique random token used to add a second source to an existing
          account
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Connect
      - Tokens
      - Token
  /accounts/{id}/contacts:
    get:
      summary: Get Accounts Contacts
      description: Lists contacts in an account.
      operationId: listAccountContacts_
      x-api-path-slug: accountsidcontacts-get
      parameters:
      - in: query
        name: active_after
        description: Only include contacts included in at least one email dated after
          a given time
      - in: query
        name: active_before
        description: Only include contacts included in at least one email dated before
          a given time
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      - in: query
        name: search
        description: String identifying the name or the email address of the contact(s)
          you are looking for
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Contacts
  /accounts/{id}/contacts/{email}:
    get:
      summary: Get Accounts Contacts Email
      description: Gets information about a given contact.
      operationId: getAccountContact_
      x-api-path-slug: accountsidcontactsemail-get
      parameters:
      - in: path
        name: email
        description: Email address of a contact
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Contacts
      - Email
  /accounts/{id}/contacts/{email}/files:
    get:
      summary: Get Accounts Contacts Email Files
      description: Lists files exchanged with a contact. Returns the latest attachments
        exchanged with one or more email addresses. By "exchanged with Mr. X" we mean
        any file attached to an email received from Mr. X, sent to Mr. X or sent by
        anyone to both Mr. X and the mailbox owner.
      operationId: listAccountContactFiles_
      x-api-path-slug: accountsidcontactsemailfiles-get
      parameters:
      - in: path
        name: email
        description: Email address of a contact
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Contacts
      - Email
      - Files
  /accounts/{id}/contacts/{email}/messages:
    get:
      summary: Get Accounts Contacts Email Messages
      description: Lists messages where a contact is present. Returns the latest email
        messages exchanged with one or more email addresses. By "exchanged with Mr.
        X" we mean any email received from Mr. X, sent to Mr. X or sent by anyone
        to both Mr. X and the mailbox owner.
      operationId: listAccountContactMessages_
      x-api-path-slug: accountsidcontactsemailmessages-get
      parameters:
      - in: path
        name: email
        description: Email address of a contact
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Contacts
      - Email
      - Messages
  /accounts/{id}/contacts/{email}/threads:
    get:
      summary: Get Accounts Contacts Email Threads
      description: Lists threads where a contact is present. Returns the latest email
        threads exchanged with one or more email addresses. By "exchanged with Mr.
        X" we mean any email received from Mr. X, sent to Mr. X or sent by anyone
        to both Mr. X and the mailbox owner.
      operationId: listAccountContactThreads_
      x-api-path-slug: accountsidcontactsemailthreads-get
      parameters:
      - in: path
        name: email
        description: Email address of a contact
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Contacts
      - Email
      - Threads
  /accounts/{id}/email_addresses:
    get:
      summary: Get Accounts Email Addresses
      description: Lists email addresses used by an account.
      operationId: listAccountEmailAddresses_
      x-api-path-slug: accountsidemail-addresses-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Email
      - Addresses
    post:
      summary: Post Accounts Email Addresses
      description: Adds a new email address as an alias for an account.
      operationId: addAccountEmailAddress_
      x-api-path-slug: accountsidemail-addresses-post
      parameters:
      - in: query
        name: email_address
        description: An email address
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Email
      - Addresses
  /accounts/{id}/email_addresses/{email}:
    post:
      summary: Post Accounts Email Addresses Email
      description: Makes this email address the primary one for the account.
      operationId: Create_setAccountEmailAddressAsPrimary_
      x-api-path-slug: accountsidemail-addressesemail-post
      parameters:
      - in: path
        name: email
        description: One of the email addresses associated to the account
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: primary
        description: Set to 1 to make this email address the primary one for the account
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Email
      - Addresses
      - Email
    delete:
      summary: Delete Accounts Email Addresses Email
      description: Removes an email address form the aliases of an account.
      operationId: removeAccountEmailAddress_
      x-api-path-slug: accountsidemail-addressesemail-delete
      parameters:
      - in: path
        name: email
        description: One of the email addresses associated to the account
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Email
      - Addresses
      - Email
  /accounts/{id}/files:
    get:
      summary: Get Accounts Files
      description: 'Lists files found as email attachments. List filters: each of
        the email, to, from, cc and bcc parameters can be set to a comma-separated
        list of email addresses. These multiple addresses are treated as an OR combination.
        You can set more than one parameter when doing this call. Multiple parameters
        are treated as an AND combination.'
      operationId: listAccountFiles_
      x-api-path-slug: accountsidfiles-get
      parameters:
      - in: query
        name: bcc
        description: Email address of a contact BCCed on the messages
      - in: query
        name: cc
        description: Email address of a contact CCed on the messages
      - in: query
        name: date_after
        description: Only include files attached to messages sent after a given timestamp
      - in: query
        name: date_before
        description: Only include files attached to messages sent before a given timestamp
      - in: query
        name: email
        description: Email address of the contact for whom you want the latest files
          exchanged with
      - in: query
        name: file_name
        description: Search for files based on their name
      - in: query
        name: from
        description: Email address of a contact files have been received from
      - in: query
        name: group_by_revisions
        description: If set to 1, the list will do an intelligent grouping of files
          to reflect occurrences of the same document
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: indexed_after
        description: Only include files attached to messages indexed after a given
          timestamp
      - in: query
        name: indexed_before
        description: Only include files attached to messages indexed before a given
          timestamp
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      - in: query
        name: to
        description: Email address of a contact files have been sent to
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
  /accounts/{id}/files/{fileId}:
    get:
      summary: Get Accounts Files Fileid
      description: Gets information about a given file.
      operationId: getAccountFile_
      x-api-path-slug: accountsidfilesfileid-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
  /accounts/{id}/files/{fileId}/changes:
    get:
      summary: Get Accounts Files Fileid Changes
      description: Lists files that can be compared with a given file.
      operationId: listComparableAccountFiles_
      x-api-path-slug: accountsidfilesfileidchanges-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
      - Changes
  /accounts/{id}/files/{fileId}/content:
    get:
      summary: Get Accounts Files Fileid Content
      description: 'Downloads a given file. Returns the content a given attachment.
        On-demand data retrieval: since we do not keep full copies of attachments
        on our servers, the file has to be retrieved from the IMAP server when this
        call is made. If the IMAP server is unreachable at the time the call is made,
        this call will return an error.'
      operationId: getAccountFileContent_
      x-api-path-slug: accountsidfilesfileidcontent-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
      - Content
  /accounts/{id}/files/{fileId}/related:
    get:
      summary: Get Accounts Files Fileid Related
      description: Lists other files related to a given file. Returns a list of files
        that are related to the given file. Currently, relation between files is based
        on how similar their names are.
      operationId: listAccountFileRelatedFiles_
      x-api-path-slug: accountsidfilesfileidrelated-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
      - Related
  /accounts/{id}/files/{fileId}/revisions:
    get:
      summary: Get Accounts Files Fileid Revisions
      description: Lists other revisions of a given file. Returns a list of revisions
        attached to other emails in the mailbox for a given file. Two files are considered
        revisions of the same document if their file names are identical outside of
        revision indicators such as dates, author initials, version numbers and keywords
        like "final" or "draft".
      operationId: listAccountFileRevisions_
      x-api-path-slug: accountsidfilesfileidrevisions-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
      - Revisions
  /accounts/{id}/messages:
    get:
      summary: Get Accounts Messages
      description: 'Lists email messages for an account. List filters: each of the
        email, to, from, cc and bcc parameters can be set to a comma-separated list
        of email addresses. These multiple addresses are treated as an OR combination.
        You can set more than one parameter when doing this call. Multiple parameters
        are treated as an AND combination.'
      operationId: listAccountMessages_
      x-api-path-slug: accountsidmessages-get
      parameters:
      - in: query
        name: bcc
        description: Email address of a contact BCCed on the messages
      - in: query
        name: body_type
        description: Used when include_body is set to get only body parts of a given
          MIME-type (i
      - in: query
        name: cc
        description: Email address of a contact CCed on the messages
      - in: query
        name: date_after
        description: Only include messages after a given timestamp
      - in: query
        name: date_before
        description: Only include messages before a given timestamp
      - in: query
        name: email
        description: Email address of the contact for whom you want the latest messages
          exchanged with
      - in: query
        name: folder
        description: Filter messages by the folder (or Gmail label)
      - in: query
        name: from
        description: Email address of a contact messages have been received from
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: include_body
        description: Set to 1 to include message bodies in the result
      - in: query
        name: include_flags
        description: Set to 1 to include IMAP flags for this message in the result
      - in: query
        name: include_headers
        description: Can be set to 0 (default), 1 or raw
      - in: query
        name: indexed_after
        description: Only include messages indexed after a given timestamp
      - in: query
        name: indexed_before
        description: Only include messages indexed before a given timestamp
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      - in: query
        name: subject
        description: Get messages whose subject matches this search string
      - in: query
        name: to
        description: Email address of a contact messages have been sent to
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Messages
  /accounts/{id}/messages/{message_id}:
    get:
      summary: Get Accounts Messages Message
      description: Gets the file, contact and other information about a given email
        message. As specified in the RFC822, the < and > at the beginning and end
        of the Message-ID are part of the value and should be included if you're putting
        an email_message_id in the url.
      operationId: getAccountMessage_
      x-api-path-slug: accountsidmessagesmessage-id-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: message_id
        description: Unique id of a message
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Messages
      - Message
    post:
      summary: Post Accounts Messages Message
      description: Copies or moves a message. Allows you to copy or move a message
        between folders. If there are more than one sources on the account, you can
        use this call to copy/move the message between these sources. In this case,
        the dst_label parameter must identify the source you want to message to be
        copied/moved to.
      operationId: Create_copyMoveAccountMessage_
      x-api-path-slug: accountsidmessagesmessage-id-post
      parameters:
      - in: query
        name: dst_folder
        description: The folder within dst_source the message should be copied to
      - in: query
        name: dst_source
        description: Label of the source you want the message copied to
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: message_id
        description: Unique id of a message
      - in: query
        name: move
        description: By default, this calls copies the original message in the destination
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Messages
      - Message
  /accounts/{id}/messages/{message_id}/body:
    get:
      summary: Get Accounts Messages Message Body
      description: 'Fetches the message body of a given email. On-demand data retrieval:
        since we do not keep full copies of emails on our servers, this call triggers
        a connection to the IMAP server to fetch the message. One thing to point out
        is we do fetch messages in such a way that large files attached to a message
        won''t make any difference in the response time. This call only returns text
        portions of messages, attachments aren''t included. To get a list of attachments
        on the message, look for the files property in the response of a message instance.
        To download the content of these attachments, use the files/content call.'
      operationId: getAccountMessageBody_
      x-api-path-slug: accountsidmessagesmessage-idbody-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: message_id
        description: Unique id of a message
      - in: query
        name: type
        description: Many emails are sent with both rich text and plain text versions
          in the message body and by default, the response of this call will include
          both
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Messages
      - Message
      - Body
  /accounts/{id}/messages/{message_id}/source:
    get:
      summary: Get Accounts Messages Message Source
      description: 'Fetches the message source. Returns the raw RFC-822 message source
        for the message (including attachments) with no parsing or decoding to any
        portions of the message. On-demand data retrieval: since we do not keep full
        copies of emails on our servers, this call triggers a connection to the IMAP
        server to fetch the message. Attachments are part of the message source so
        they will impact how fast this call responds.'
      operationId: getAccountMessageSource_
      x-api-path-slug: accountsidmessagesmessage-idsource-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: message_id
        description: Unique id of a message
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Messages
      - Message
      - Source
  /accounts/{id}/messages/{message_id}/flags:
    get:
      summary: Get Accounts Messages Message Flags
      description: 'Lists message flags for an account. On-demand data retrieval:
        to ensure up-to-date values, flags are not cached by Context.IO. This call
        triggers a connection to the IMAP server to fetch the current message flags
        before it returns.'
      operationId: listAccountMessageFlags_
      x-api-path-slug: accountsidmessagesmessage-idflags-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: message_id
        description: Unique id of a message
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Messages
      - Message
      - Flags
    post:
      summary: Post Accounts Messages Message Flags
      description: Sets message flags for a given email.
      operationId: Create_setAccountMessageFlags_
      x-api-path-slug: accountsidmessagesmessage-idflags-post
      parameters:
      - in: query
        name: answered
        description: Message has been answered
      - in: query
        name: deleted
        description: Message is deleted for later removal
      - in: query
        name: draft
        description: Message has not completed composition (marked as a draft)
      - in: query
        name: flagged
        description: Message is flagged for urgent/special attention
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: message_id
        description: Unique id of a message
      - in: query
        name: seen
        description: Message has been read
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Messages
      - Message
      - Flags
  /accounts/{id}/messages/{message_id}/headers:
    get:
      summary: Get Accounts Messages Message Headers
      description: 'Lists complete headers of a given email message. On-demand data
        retrieval: since we do not keep full copies of emails on our servers, this
        call triggers a connection to the IMAP server to fetch the message headers.'
      operationId: listAccountMessageHeaders_
      x-api-path-slug: accountsidmessagesmessage-idheaders-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: message_id
        description: Unique id of a message
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Messages
      - Message
      - Headers
  /accounts/{id}/messages/{message_id}/thread:
    get:
      summary: Get Accounts Messages Message Thread
      description: Gets information about all messages of the thread a given message
        is in. This returns an array with the same structure as getting information
        on a single message for every message in the thread.
      operationId: getAccountMessageThread_
      x-api-path-slug: accountsidmessagesmessage-idthread-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: message_id
        description: Unique id of a message
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Messages
      - Message
      - Thread
  /accounts/{id}/sources:
    get:
      summary: Get Accounts Sources
      description: Lists IMAP sources assigned for an account.
      operationId: listAccountSources_
      x-api-path-slug: accountsidsources-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: status
        description: Only return sources whose status is of a specific value
      - in: query
        name: status_ok
        description: Set to 0 to get sources that are not working correctly
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
    post:
      summary: Post Accounts Sources
      description: Adds an IMAP account to a given account.
      operationId: addAccountSource_
      x-api-path-slug: accountsidsources-post
      parameters:
      - in: query
        name: email
        description: The primary email address used to receive emails in this account
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: password
        description: Password for authentication on the IMAP server
      - in: query
        name: port
        description: Port number to connect to on the server
      - in: query
        name: provider_consumer_key
        description: The OAuth consumer key used to obtain the the token and token
          secret above for that account
      - in: query
        name: provider_token
        description: An OAuth token obtained from the IMAP account provider to be
          used to authentify on this email account
      - in: query
        name: provider_token_secret
        description: An OAuth token secret obtained from the IMAP account provider
          to be used to authentify on this email account
      - in: query
        name: server
        description: Name of IP of the IMAP server, eg
      - in: query
        name: service_level
        description: Sets the service level for the source to be created
      - in: query
        name: sync_period
        description: Sets the period at which the Context
      - in: query
        name: type
        description: Currently, the only supported type is IMAP
      - in: query
        name: username
        description: The username used to authentify an IMAP connection
      - in: query
        name: use_ssl
        description: Set to 1 if you want SSL encryption to be used when opening connections
          to the IMAP server
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
  /accounts/{id}/sources/{label}:
    get:
      summary: Get Accounts Sources Label
      description: Gets parameters and status for an IMAP source.
      operationId: getAccountSource_
      x-api-path-slug: accountsidsourceslabel-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
    put:
      summary: Put Accounts Sources Label
      description: Modifies a data source on a given account.
      operationId: modifyAccountSource_
      x-api-path-slug: accountsidsourceslabel-put
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      - in: query
        name: password
        description: New password for this source
      - in: query
        name: provider_consumer_key
        description: The OAuth consumer key used to obtain the the token and token
          secret above for that account
      - in: query
        name: provider_token
        description: An OAuth token obtained from the IMAP account provider to be
          used to authentify on this email account
      - in: query
        name: provider_token_secret
        description: An OAuth token secret obtained from the IMAP account provider
          to be used to authentify on this email account
      - in: query
        name: service_level
        description: Changes the service level for the source
      - in: query
        name: status
        description: If the status of the source is TEMP_DISABLED or DISABLED
      - in: query
        name: sync_period
        description: Changes the period at which the Context
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
    delete:
      summary: Delete Accounts Sources Label
      description: Removes a data source of an account.
      operationId: removeAccountSource_
      x-api-path-slug: accountsidsourceslabel-delete
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
  /accounts/{id}/sources/{label}/folders:
    get:
      summary: Get Accounts Sources Label Folders
      description: Lists folders in an IMAP source. Returns folders existing in a
        given IMAP account.
      operationId: listAccountSourceFolders_
      x-api-path-slug: accountsidsourceslabelfolders-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
      - Folders
  /accounts/{id}/sources/{label}/folders/{folder}:
    put:
      summary: Put Accounts Sources Label Folders Folder
      description: |-
        Creates a folder on an IMAP source. A new folder can be added to an IMAP source by PUTting the desired path under the sources/folders resource.
        Working with server-specific hierarchy delimiters:
        IMAP servers are free to use the character they want as the folder hierarchy delimiter. The bad news is they don't use the same. The good news is you don't need to know this, we take care of it.

        Then what is that delim parameter for?
        Good question. By default, we expect you to specify the folder hierarchy using / as the hierarchy delimiter. For example, to create a folder called my folder under the folder base folder, you would call:
        PUT /2.0/accounts/<id>/sources/<label>/folders/base+folder/my+folder

        No matter what's the actual hierarchy delimiter the IMAP server expects, this call will work. However, say you need to use another character as the delimiter, here's how you'd do it:
        PUT /2.0/accounts/<id>/sources/<label>/folders/base+folder.my+folder?delim=.

        Both examples above are equivalent and will have the same result no matter what the IMAP server expects as the actual hierarchy delimiter.
      operationId: createAccountSourceFolder_
      x-api-path-slug: accountsidsourceslabelfoldersfolder-put
      parameters:
      - in: query
        name: delim
        description: If / isnt fancy enough as a hierarchy delimiter when specifying
          the folder you want to create, youre free to use what you want, just make
          sure you set this delim parameter to tell us what youre using
      - in: path
        name: folder
        description: The full folder path you want to create
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
      - Folders
      - Folder
  /accounts/{id}/sources/{label}/sync:
    get:
      summary: Get Accounts Sources Label Sync
      description: Gets the sync status of a data source. Returns the timestamps for
        the last time the source has been synced with the origin mailbox.
      operationId: getAccountSourceSyncStatus_
      x-api-path-slug: accountsidsourceslabelsync-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
      - Sync
    post:
      summary: Post Accounts Sources Label Sync
      description: Triggers a sync of a data source. This will start a sync job for
        the source.
      operationId: Create_syncAccountSource_
      x-api-path-slug: accountsidsourceslabelsync-post
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: label
        description: The label property of the source instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sources
      - Label
      - Sync
  /accounts/{id}/sync:
    get:
      summary: Get Accounts Sync
      description: Gets the sync status for all sources of the account. Returns the
        timestamps for the last time a source has been synced with the origin mailbox.
      operationId: getAllAccountSourcesSyncStatus_
      x-api-path-slug: accountsidsync-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sync
    post:
      summary: Post Accounts Sync
      description: Triggers a sync of all sources on the account. This will start
        a sync job for all sources under the account.
      operationId: Create_syncAllAccountSources_
      x-api-path-slug: accountsidsync-post
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Sync
  /accounts/{id}/threads:
    get:
      summary: Get Accounts Threads
      description: Lists threads on an account.
      operationId: listAccountThreads_
      x-api-path-slug: accountsidthreads-get
      parameters:
      - in: query
        name: active_after
        description: Get threads with at least one message dated after this timestamp
      - in: query
        name: active_before
        description: Get threads with at least one message dated before this timestamp
      - in: query
        name: bcc
        description: Get threads with at least one message having this email address
          BCCed
      - in: query
        name: cc
        description: Get threads with at least one message having this email address
          CCed
      - in: query
        name: email
        description: Email address of the contact for whom you want the latest threads
      - in: query
        name: folder
        description: Filter threads by the folder (or Gmail label)
      - in: query
        name: from
        description: Get threads with at least one message sent from this email address
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: indexed_after
        description: Get threads with at least one message indexed after this timestamp
      - in: query
        name: indexed_before
        description: Get threads with at least one message indexed before this timestamp
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      - in: query
        name: started_after
        description: Get threads whose first message is dated after this timestamp
      - in: query
        name: started_before
        description: Get threads whose first message is dated before this timestamp
      - in: query
        name: subject
        description: Get threads with messages whose subject matches this search string
      - in: query
        name: to
        description: Get threads with at least one message sent to this email address
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Threads
  /accounts/{id}/threads/{thread_id}:
    get:
      summary: Get Accounts Threads Thread
      description: |-
        Returns files, contacts and messages on a given thread. The purpose is to allow Gmail extensions to easily retrieve data when users's load a conversation in the Gmail UI. Hence, threads are identified by the value of their Gmail thread prefixed with "gm-".
        For example, if the URL of a conversation in the Gmail UI is https://mail.google.com/mail/u/0/#mbox/13119ab37f00b826, you would obtain the details about this thread by calling:
        GET https://api.context.io/2.0/accounts/<accountId>/threads/gm-13119ab37f00b826

        What about threads on non-Gmail mailboxes?
        You can retrieve thread information for any message using the Thread resource of that message.
      operationId: getAccountThread_
      x-api-path-slug: accountsidthreadsthread-id-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: thread_id
        description: A gmail_thread_id prefixed with gm-
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Threads
      - Thread
  /accounts/{id}/webhooks:
    get:
      summary: Get Accounts Webhooks
      description: List WebHooks configured for an account.
      operationId: listAccountWebhooks_
      x-api-path-slug: accountsidwebhooks-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Webhooks
    post:
      summary: Post Accounts Webhooks
      description: Creates a new WebHook on an account.
      operationId: createAccountWebhook_
      x-api-path-slug: accountsidwebhooks-post
      parameters:
      - in: query
        name: callback_url
        description: A valid URL Context
      - in: query
        name: failure_notif_url
        description: A valid URL Context
      - in: query
        name: filter_cc
        description: Check for new messages where a given name or email address is
          cced
      - in: query
        name: filter_file_name
        description: Check for new messages where a file whose name matches the given
          string is attached
      - in: query
        name: filter_file_revisions
        description: Check for new message where a new revision of a given file is
          attached
      - in: query
        name: filter_folder_added
        description: Check for messages filed in a given folder
      - in: query
        name: filter_folder_removed
        description: Check for messages removed from a given folder
      - in: query
        name: filter_from
        description: Check for new messages received from a given name or email address
      - in: query
        name: filter_new_important
        description: Check for new messages automatically tagged as important by the
          Gmail Priority Inbox algorithm
      - in: query
        name: filter_subject
        description: Check for new messages with a subject matching a given string
          or regular expresion
      - in: query
        name: filter_thread
        description: Check for new messages in a given thread
      - in: query
        name: filter_to
        description: Check for new messages sent to a given name or email address
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: sync_period
        description: Desired maximum delay between the moment the email comes in the
          users mailbox and the time we call the callback_url
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Webhooks
  /accounts/{id}/webhooks/{webhook_id}:
    get:
      summary: Get Accounts Webhooks Webhook
      description: Gets properties of a given WebHook.
      operationId: getAccountWebhook_
      x-api-path-slug: accountsidwebhookswebhook-id-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: webhook_id
        description: Unique id of the webhook instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Webhooks
      - Webhook
    post:
      summary: Post Accounts Webhooks Webhook
      description: |-
        Changes properties of a given WebHook. The only property of a WebHook that can be changed is it's active property. If you want to change the filters or callback urls, delete it and create a new one.
        Changing the active property can be useful in two cases:
        - Pause/resume WebHooks: If your application needs up-to-date information when users are logged in the best option is to keep a WebHook with no filters on that account that will be resumed (setting active to 1) when the user logs in and paused (setting active to 0) when the user logs out of your app.
        - Acting upon a failure notification: If a WebHook fails, your failure_notif_url is called (see creating a WebHook) an its active property becomes 0. Set the active property back to 1 to get it working again.
      operationId: modifyAccountWebhook_
      x-api-path-slug: accountsidwebhookswebhook-id-post
      parameters:
      - in: query
        name: active
        description: The active property of a WebHook allows you to pause (set to
          0) or resume (set to 1) it
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: webhook_id
        description: Unique id of the webhook instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Webhooks
      - Webhook
    delete:
      summary: Delete Accounts Webhooks Webhook
      description: Cancels a WebHook.
      operationId: Delete_cancelAccountWebhook_
      x-api-path-slug: accountsidwebhookswebhook-id-delete
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: webhook_id
        description: Unique id of the webhook instance
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Webhooks
      - Webhook