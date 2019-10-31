swagger: "2.0"
x-collection-name: Stride
x-complete: 1
info:
  title: Stride
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
host: api.atlassian.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /app/module/chat/conversation/chat:configuration/{key}/state:
    post:
      summary: Send app configuration updates
      description: |-
        Post app configuration updates telling the.

        Authentication required.
      operationId: AppModuleChatConversationChatConfigurationStateByKeyPost
      x-api-path-slug: appmodulechatconversationchatconfigurationkeystate-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - App
      - Module
      - Chat
      - Conversation
      - Chat
      - Configuration
      - Key
      - State
  /app/module/chat/conversation/chat:glance/{key}/state:
    post:
      summary: Send glance updates
      description: |-
        Post glance updates which will be pushed for all users within the specified context.

        Authentication required.
      operationId: AppModuleChatConversationChatGlanceStateByKeyPost
      x-api-path-slug: appmodulechatconversationchatglancekeystate-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: key
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - App
      - Module
      - Chat
      - Conversation
      - Chat
      - Glance
      - Key
      - State
  /site/{cloudId}/conversation:
    get:
      summary: Get conversation list for site
      description: Authentication required, with scope participate:conversation
      operationId: SiteConversationByCloudIdGet
      x-api-path-slug: sitecloudidconversation-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: query
        name: cursor
      - in: query
        name: include-archived
      - in: query
        name: include-private
      - in: query
        name: limit
      - in: query
        name: query
      - in: query
        name: sort
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
    post:
      summary: Create conversation
      description: Authentication required, with scope manage:conversation
      operationId: SiteConversationByCloudIdPost
      x-api-path-slug: sitecloudidconversation-post
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
  /site/{cloudId}/conversation/user/{userId}/message:
    post:
      summary: Send message to user
      description: Authentication required, with scope participate:conversation
      operationId: SiteConversationUserMessageByCloudIdAndUserIdPost
      x-api-path-slug: sitecloudidconversationuseruseridmessage-post
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - User
      - User
      - Message
  /site/{cloudId}/conversation/{conversationId}:
    get:
      summary: Get conversation details
      description: Authentication required, with scope participate:conversation
      operationId: SiteConversationByCloudIdAndConversationIdGet
      x-api-path-slug: sitecloudidconversationconversationid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
    patch:
      summary: Update conversation
      description: Authentication required, with scope manage:conversation
      operationId: SiteConversationByCloudIdAndConversationIdPatch
      x-api-path-slug: sitecloudidconversationconversationid-patch
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
  /site/{cloudId}/conversation/{conversationId}/archive:
    put:
      summary: Archive conversation
      description: Authentication required, with scope manage:conversation
      operationId: SiteConversationArchiveByCloudIdAndConversationIdPut
      x-api-path-slug: sitecloudidconversationconversationidarchive-put
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
      - Archives
  /site/{cloudId}/conversation/{conversationId}/media:
    post:
      summary: Upload a file
      description: Authentication required, with scope participate:conversation
      operationId: SiteConversationMediaByCloudIdAndConversationIdPost
      x-api-path-slug: sitecloudidconversationconversationidmedia-post
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      - in: query
        name: name
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
      - Media
  /site/{cloudId}/conversation/{conversationId}/media/{mediaId}:
    get:
      summary: Get a file
      description: Authentication required, with scope participate:conversation
      operationId: SiteConversationMediaMediaIdByCloudIdAndConversationIdGet
      x-api-path-slug: sitecloudidconversationconversationidmediamediaid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      - in: path
        name: mediaId
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
      - Media
      - Media
  /site/{cloudId}/conversation/{conversationId}/message:
    get:
      summary: Get conversation history
      description: |-
        Authentication required, with scope participate:conversation

        This method returns messages after/before a given messageIDs or/and timestamps.
        If these parameters are omitted the method returns conversation???s latest messages.
      operationId: SiteConversationMessageByCloudIdAndConversationIdGet
      x-api-path-slug: sitecloudidconversationconversationidmessage-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: afterMessage
      - in: query
        name: afterTimestamp
      - in: query
        name: beforeMessage
      - in: query
        name: beforeTimestamp
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      - in: query
        name: limit
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
      - Message
    post:
      summary: Send a message to a conversation
      description: Authentication required, with scope participate:conversation
      operationId: SiteConversationMessageByCloudIdAndConversationIdPost
      x-api-path-slug: sitecloudidconversationconversationidmessage-post
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
      - Message
  /site/{cloudId}/conversation/{conversationId}/message/recent:
    get:
      summary: Get latest messages for conversation
      description: Authentication required, with scope participate:conversation
      operationId: SiteConversationMessageRecentByCloudIdAndConversationIdGet
      x-api-path-slug: sitecloudidconversationconversationidmessagerecent-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      - in: query
        name: limit
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
      - Message
      - Recent
  /site/{cloudId}/conversation/{conversationId}/message/{messageId}:
    get:
      summary: Get message by id
      description: Authentication required, with scope participate:conversation
      operationId: SiteConversationMessageMessageIdByCloudIdAndConversationIdGet
      x-api-path-slug: sitecloudidconversationconversationidmessagemessageid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      - in: path
        name: messageId
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
      - Message
      - Message
  /site/{cloudId}/conversation/{conversationId}/message/{messageId}/context:
    get:
      summary: Get conversation history contextually
      description: |-
        Authentication required, with scope participate:conversation

        This method returns messages after and/or before a given messageID including the message itself.
        Default value for 'after' and 'before' query parameters is 0.
      operationId: SiteConversationMessageMessageIdContextByCloudIdAndConversationIdGet
      x-api-path-slug: sitecloudidconversationconversationidmessagemessageidcontext-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: after
      - in: query
        name: before
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      - in: path
        name: messageId
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
      - Message
      - Message
      - Context
  /site/{cloudId}/conversation/{conversationId}/roster:
    get:
      summary: Get conversation roster
      description: Authentication required, with scope participate:conversation
      operationId: SiteConversationRosterByCloudIdAndConversationIdGet
      x-api-path-slug: sitecloudidconversationconversationidroster-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      - in: query
        name: limit
      - in: query
        name: start
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
      - Roster
  /site/{cloudId}/conversation/{conversationId}/unarchive:
    put:
      summary: Unarchive conversation
      description: Authentication required, with scope manage:conversation
      operationId: SiteConversationUnarchiveByCloudIdAndConversationIdPut
      x-api-path-slug: sitecloudidconversationconversationidunarchive-put
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
      - Unarchive
      - Archives