swagger: "2.0"
x-collection-name: Mailjet
x-complete: 1
info:
  title: Mailjet Messages API
  description: allows-you-to-list-and-view-the-details-of-a-message-an-email-processed-by-mailjet
  version: v3
host: api.mailjet.com
basePath: v3/REST/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  message/:
    get:
      summary: Message List
      description: Allows you to list messages.
      operationId: getMessage
      x-api-path-slug: message-get
      parameters:
      - in: query
        name: Campaign
        description: Only retrieve message resources for which Campaign ID equals
          the specified value
      - in: query
        name: Contact
        description: Only retrieve message resources for which Contact ID equals the
          specified value
      - in: query
        name: MessageState
        description: Only show messages with this state
      - in: query
        name: PlanSubscription
        description: Only retrieve message resources for which PlanSubscription ID
          equals the specified value
      - in: query
        name: Sender
        description: Only show messages from this sender
      responses:
        200:
          description: OK
      tags:
      - Message
      - List
  messagehistory/:
    get:
      summary: Message History
      description: List message history resources
      operationId: getMessagehistory
      x-api-path-slug: messagehistory-get
      parameters:
      - in: path
        name: Message
        description: ID of message for which to show the history
      responses:
        200:
          description: OK
      tags:
      - Message
      - History
  messagehistory/{id}:
    get:
      summary: Message History
      description: Get the history of a message.
      operationId: getMessagehistory
      x-api-path-slug: messagehistoryid-get
      parameters:
      - in: path
        name: id
        description: ID of the message history
      responses:
        200:
          description: OK
      tags:
      - Message
      - History
  messageinformation/:
    get:
      summary: Message Information
      description: Lists the information about a message.
      operationId: getMessageinformation
      x-api-path-slug: messageinformation-get
      parameters:
      - in: query
        name: CampaignID
        description: Unique numerical ID for this object
      - in: query
        name: CampaignStatus
        description: Only retrieve campaigns with status equal to specified value
      - in: query
        name: ContactsList
        description: Only retrieve campaigns sent to specified Contacts list
      - in: query
        name: CustomCampaign
        description: Only retrieve campaigns with given Custom Value
      - in: query
        name: From
        description: Only retrieve campaigns with given From header
      - in: query
        name: FromDomain
        description: Only retrieve campaigns with given domain in From header
      - in: query
        name: FromID
        description: Only retrieve campaigns with this sender ID
      - in: query
        name: FromTS
        description: Only retrieve campaigns with SendStartAt after this timestamp
      - in: query
        name: FromType
        description: Only retrieve campaigns with FromType equal to specified value
      - in: query
        name: IsDeleted
        description: Only retrieve campaigns where isDeleted matches the specified
          value
      - in: query
        name: IsNewsletterTool
        description: Only retrieve campaigns which were started by the newsletter
          tool
      - in: query
        name: IsStarred
        description: Only retrieve campaigns which were marked as starred
      - in: query
        name: MessageStatus
        description: Only retrieve messages with status equal to specified value
      - in: query
        name: Period
        description: Set FromTS and ToTS timestamps to beginning of indicated period
          and current timestamp, respectively
      - in: query
        name: ToTS
        description: Only retrieve campaigns with SendStartAt timestamp less than
          the specified value
      responses:
        200:
          description: OK
      tags:
      - Message
      - Information
  messageinformation/{id}:
    get:
      summary: Message Information
      description: Lists a message informaiton.
      operationId: getMessageinformation
      x-api-path-slug: messageinformationid-get
      parameters:
      - in: path
        name: id
        description: ID of the message
      responses:
        200:
          description: OK
      tags:
      - Message
      - Information
  messagesentstatistics/:
    get:
      summary: Message Statistics
      description: Lists the message statistics.
      operationId: getMessagesentstatistics
      x-api-path-slug: messagesentstatistics-get
      parameters:
      - in: query
        name: AllMessages
        description: Retrieve all messages
      - in: query
        name: CampaignID
        description: Unique numerical ID for this object
      - in: query
        name: CampaignStatus
        description: Only retrieve campaigns with Status equal to specified value
      - in: query
        name: Contact
        description: Only retrieve messagesentstatistics resources for which Contact
          equals the specified value
      - in: query
        name: ContactsList
        description: Only retrieve campaigns sent to specified Contacts list
      - in: query
        name: CustomCampaign
        description: Only retrieve campaigns with given Custom Value
      - in: query
        name: From
        description: Only retrieve campaigns with given From header
      - in: query
        name: FromDomain
        description: Only retrieve campaigns with given domain in From header
      - in: query
        name: FromID
        description: Only retrieve campaigns with this sender ID
      - in: query
        name: FromTS
        description: Only retrieve campaigns with SendStartAt after this timestamp
      - in: query
        name: FromType
        description: Only retrieve campaigns with FromType equal to specified value
      - in: query
        name: IsDeleted
        description: Only retrieve campaigns where isDeleted matches the specified
          value
      - in: query
        name: IsNewsletterTool
        description: Only retrieve campaigns which were started by the newsletter
          tool
      - in: query
        name: IsStarred
        description: Only retrieve campaigns which were marked as starred
      - in: query
        name: MessageStatus
        description: Only retrieve messages with Status equal to specified value
      - in: query
        name: Period
        description: Set FromTS and ToTS timestamps to beginning of indicated period
          and current timestamp, respectively
      - in: query
        name: ShowExtraData
        description: '[ Type TBooleanFilter ]'
      - in: query
        name: ToTS
        description: Only retrieve campaigns with SendStartAt timestamp less than
          the specified value
      responses:
        200:
          description: OK
      tags:
      - Message
      - Statistics
  messagesentstatistics/{id}:
    get:
      summary: Message Statistics
      description: List message statistics.
      operationId: getMessagesentstatistics
      x-api-path-slug: messagesentstatisticsid-get
      responses:
        200:
          description: OK
      tags:
      - Message
      - Statistics
  messagestate/{id}:
    get:
      summary: Message State
      description: Returns message state.
      operationId: getMessagestate
      x-api-path-slug: messagestateid-get
      parameters:
      - in: query
        name: id
        description: Id of the message
      responses:
        200:
          description: OK
      tags:
      - Message
      - State
  messagestatistics/:
    get:
      summary: Message Statistics
      description: Message Statistics
      operationId: getMessagestatistics
      x-api-path-slug: messagestatistics-get
      parameters:
      - in: query
        name: CampaignID
        description: Unique numerical ID for this object
      - in: query
        name: CampaignStatus
        description: Only retrieve campaigns with status equal to specified value
      - in: query
        name: ContactEmail
        description: Only retrieve message statistics for this contact email address
      - in: query
        name: ContactID
        description: Unique numerical ID for this object
      - in: query
        name: ContactListID
        description: '[ Type Int64 ]'
      - in: query
        name: CustomCampaign
        description: Only retrieve campaigns with given Custom Value
      - in: query
        name: From
        description: Only retrieve campaigns with given From header
      - in: query
        name: FromDomain
        description: Only retrieve campaigns with given domain in From header
      - in: query
        name: FromID
        description: Only retrieve campaigns with this sender ID
      - in: query
        name: FromTS
        description: Only retrieve campaigns with SendStartAt after this timestamp
      - in: query
        name: FromType
        description: Only retrieve campaigns with FromType equal to specified value
      - in: query
        name: IsDeleted
        description: Only retrieve campaigns where isDeleted matches the specified
          value
      - in: query
        name: IsNewsletterTool
        description: Only retrieve campaigns which were started by the newsletter
          tool
      - in: query
        name: IsStarred
        description: Only retrieve campaigns which were marked as starred
      - in: query
        name: MessageStatus
        description: Only retrieve messages with status equal to specified value
      - in: query
        name: Period
        description: Set FromTS and ToTS timestamps to beginning of indicated period
          and current timestamp, respectively
      - in: query
        name: ToTS
        description: Only retrieve campaigns with SendStartAt timestamp less than
          the specified value
      responses:
        200:
          description: OK
      tags:
      - Message
      - Statistics
  messagestatistics/{id}:
    get:
      summary: Message Statistics
      description: Message Statistics
      operationId: getMessagestatistics
      x-api-path-slug: messagestatisticsid-get
      responses:
        200:
          description: OK
      tags:
      - Message
      - Statistics
  message{id}:
    get:
      summary: Message Detail
      description: View the details of a message.
      operationId: getMessage
      x-api-path-slug: messageid-get
      parameters:
      - in: path
        name: id
        description: Message ID
      responses:
        200:
          description: OK
      tags:
      - Message
      - Detail