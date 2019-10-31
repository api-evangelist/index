swagger: "2.0"
x-collection-name: Microsoft Office 365
x-complete: 1
info:
  title: Microsoft Office 365
  description: office-365-is-the-brand-name-used-by-microsoft-for-a-group-of-software-plus-services-subscriptions-that-provides-productivity-software-and-related-services-to-its-subscribers-
  version: 1.0.0
host: outlook.office365.com
basePath: /ews/odata/Me
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /AllServices:
    get:
      summary: Get All Services
      description: Get all services.
      operationId: getAllservices
      x-api-path-slug: allservices-get
      responses:
        200:
          description: OK
      tags:
      - Allservices
  /Calendar:
    get:
      summary: Get Calendar
      description: Retrieve information about the default calendar by using the...
      operationId: getCalendar
      x-api-path-slug: calendar-get
      responses:
        200:
          description: OK
      tags:
      - Calendar
  /CalendarGroups:
    get:
      summary: Get Calendar Groups
      description: You can request all the calendar groups in a mailbox (or a f...
      operationId: getCalendargroups
      x-api-path-slug: calendargroups-get
      responses:
        200:
          description: OK
      tags:
      - Calendargroups
    post:
      summary: Add Calendar Groups
      description: You can create a calendar group by sending a POST request wi...
      operationId: postCalendargroups
      x-api-path-slug: calendargroups-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Calendargroups
  /CalendarGroups{calendargroup_id}:
    get:
      summary: Get Calendar Groups
      description: Get calendargroups calendargroup
      operationId: getCalendargroupsCalendargroup
      x-api-path-slug: calendargroupscalendargroup-id-get
      responses:
        200:
          description: OK
      tags:
      - Calendargroups
      - Calendargroup
    post:
      summary: Add Calendar Groups
      description: Post calendargroups calendargroup
      operationId: postCalendargroupsCalendargroup
      x-api-path-slug: calendargroupscalendargroup-id-post
      responses:
        200:
          description: OK
      tags:
      - Calendargroups
      - Calendargroup
    delete:
      summary: Delete Calendar Groups
      description: Deleting a calendar group is as simple as sending a DELETE r...
      operationId: deleteCalendargroupsCalendargroup
      x-api-path-slug: calendargroupscalendargroup-id-delete
      responses:
        200:
          description: OK
      tags:
      - Calendargroups
      - Calendargroup
    patch:
      summary: Patch Calendar Groups
      description: You can update a calendar group by sending a PATCH request w...
      operationId: patchCalendargroupsCalendargroup
      x-api-path-slug: calendargroupscalendargroup-id-patch
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Calendargroups
      - Calendargroup
    parameters:
      summary: Parameters Calendar Groups
      description: Parameters calendargroups calendargroup
      operationId: parametersCalendargroupsCalendargroup
      x-api-path-slug: calendargroupscalendargroup-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Calendargroups
      - Calendargroup
  /CalendarGroups{calendargroup_id}/Calendars:
    get:
      summary: Get Calendar Groups Calendars
      description: You can request all the user's calendars (or a filtered list...
      operationId: getCalendargroupsCalendargroupCalendars
      x-api-path-slug: calendargroupscalendargroup-idcalendars-get
      responses:
        200:
          description: OK
      tags:
      - Calendargroups
      - Calendargroup
      - ""
      - Calendars
    post:
      summary: Add Calendar Groups Calendars
      description: You can create a calendar by sending a POST request with a J...
      operationId: postCalendargroupsCalendargroupCalendars
      x-api-path-slug: calendargroupscalendargroup-idcalendars-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Calendargroups
      - Calendargroup
      - ""
      - Calendars
    parameters:
      summary: Parameters Calendar Groups Calendars
      description: Parameters calendargroups calendargroup  calendars
      operationId: parametersCalendargroupsCalendargroupCalendars
      x-api-path-slug: calendargroupscalendargroup-idcalendars-parameters
      responses:
        200:
          description: OK
      tags:
      - Calendargroups
      - Calendargroup
      - ""
      - Calendars
  /Calendars{calendar_id}:
    get:
      summary: Get Calendars Calendar
      description: You can also retrieve information about a specific calendar ...
      operationId: getCalendarsCalendar
      x-api-path-slug: calendarscalendar-id-get
      responses:
        200:
          description: OK
      tags:
      - Calendars
      - Calendar
    delete:
      summary: Delete Calendars Calendar
      description: Deleting a calendar is as simple as sending a DELETE request...
      operationId: deleteCalendarsCalendar
      x-api-path-slug: calendarscalendar-id-delete
      responses:
        200:
          description: OK
      tags:
      - Calendars
      - Calendar
    patch:
      summary: Patch Calendars Calendar
      description: You can update a calendar by sending a PATCH request with a ...
      operationId: patchCalendarsCalendar
      x-api-path-slug: calendarscalendar-id-patch
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Calendars
      - Calendar
    parameters:
      summary: Parameters Calendars Calendar
      description: Parameters calendars calendar
      operationId: parametersCalendarsCalendar
      x-api-path-slug: calendarscalendar-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Calendars
      - Calendar
  /Calendars{calendar_id}/Events:
    get:
      summary: Get Calendars Calendar Events
      description: You can request all the events across all calendars (or a fi...
      operationId: getCalendarsCalendarEvents
      x-api-path-slug: calendarscalendar-idevents-get
      responses:
        200:
          description: OK
      tags:
      - Calendars
      - Calendar
      - ""
      - Events
    post:
      summary: Add Calendars Calendar Events
      description: Post calendars calendar  events
      operationId: postCalendarsCalendarEvents
      x-api-path-slug: calendarscalendar-idevents-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Calendars
      - Calendar
      - ""
      - Events
    parameters:
      summary: Parameters Calendars Calendar Events
      description: Parameters calendars calendar  events
      operationId: parametersCalendarsCalendarEvents
      x-api-path-slug: calendarscalendar-idevents-parameters
      responses:
        200:
          description: OK
      tags:
      - Calendars
      - Calendar
      - ""
      - Events
  /ContactFolders{contact_folder_id}:
    get:
      summary: Get Contact Folders Contact Folder
      description: You can access the default contact folder by using the const...
      operationId: getContactfoldersContactFolder
      x-api-path-slug: contactfolderscontact-folder-id-get
      responses:
        200:
          description: OK
      tags:
      - Contactfolders
      - Contact
      - Folder
    parameters:
      summary: Parameters Contact Folders Contact Folder
      description: Parameters contactfolders contact folder
      operationId: parametersContactfoldersContactFolder
      x-api-path-slug: contactfolderscontact-folder-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Contactfolders
      - Contact
      - Folder
  /ContactFolders{contact_folder_id}/ChildFolders:
    get:
      summary: Get Contact Folders Contact Folder Childfolders
      description: All non-default contact folders are stored as children of th...
      operationId: getContactfoldersContactFolderChildfolders
      x-api-path-slug: contactfolderscontact-folder-idchildfolders-get
      responses:
        200:
          description: OK
      tags:
      - Contactfolders
      - Contact
      - Folder
      - ""
      - Childfolders
    parameters:
      summary: Parameters Contact Folders Contact Folder Childfolders
      description: Parameters contactfolders contact folder  childfolders
      operationId: parametersContactfoldersContactFolderChildfolders
      x-api-path-slug: contactfolderscontact-folder-idchildfolders-parameters
      responses:
        200:
          description: OK
      tags:
      - Contactfolders
      - Contact
      - Folder
      - ""
      - Childfolders
  /ContactFolders{contact_folder_id}/Contacts:
    get:
      summary: Get Contact Folders Contact Folder Contacts
      description: You can request all contacts (or a filtered set by using the...
      operationId: getContactfoldersContactFolderContacts
      x-api-path-slug: contactfolderscontact-folder-idcontacts-get
      responses:
        200:
          description: OK
      tags:
      - Contactfolders
      - Contact
      - Folder
      - ""
      - Contacts
    post:
      summary: Add Contact Folders Contact Folder Contacts
      description: You can create a contact by sending a POST request with a JS...
      operationId: postContactfoldersContactFolderContacts
      x-api-path-slug: contactfolderscontact-folder-idcontacts-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contactfolders
      - Contact
      - Folder
      - ""
      - Contacts
    parameters:
      summary: Parameters Contact Folders Contact Folder Contacts
      description: Parameters contactfolders contact folder  contacts
      operationId: parametersContactfoldersContactFolderContacts
      x-api-path-slug: contactfolderscontact-folder-idcontacts-parameters
      responses:
        200:
          description: OK
      tags:
      - Contactfolders
      - Contact
      - Folder
      - ""
      - Contacts
  /Contacts{contact_id}:
    get:
      summary: Get Contacts Contact
      description: You can retrieve information about a specific contact by usi...
      operationId: getContactsContact
      x-api-path-slug: contactscontact-id-get
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Contact
    post:
      summary: Add Contacts Contact
      description: You can create a contact by sending a POST request with a JS...
      operationId: postContactsContact
      x-api-path-slug: contactscontact-id-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Contact
    delete:
      summary: Delete Contacts Contact
      description: You can delete a contact by simply sending a DELETE request ...
      operationId: deleteContactsContact
      x-api-path-slug: contactscontact-id-delete
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Contact
    patch:
      summary: Patch Contacts Contact
      description: To update a contact, send a PATCH request to the URL of the ...
      operationId: patchContactsContact
      x-api-path-slug: contactscontact-id-patch
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Contact
    parameters:
      summary: Parameters Contacts Contact
      description: Parameters contacts contact
      operationId: parametersContactsContact
      x-api-path-slug: contactscontact-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Contact
  /Contacts{contact_id}/Attachments:
    get:
      summary: Get Contacts Contact Attachments
      description: To get attachments, send a GET request to the Attachments pr...
      operationId: getContactsContactAttachments
      x-api-path-slug: contactscontact-idattachments-get
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Contact
      - ""
      - Attachments
    post:
      summary: Add Contacts Contact Attachments
      description: To add an attachment to an item, send a POST request to the ...
      operationId: postContactsContactAttachments
      x-api-path-slug: contactscontact-idattachments-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Contact
      - ""
      - Attachments
    delete:
      summary: Delete Contacts Contact Attachments
      description: To delete an attachment, send a DELETE request to the URL of...
      operationId: deleteContactsContactAttachments
      x-api-path-slug: contactscontact-idattachments-delete
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Contact
      - ""
      - Attachments
    parameters:
      summary: Parameters Contacts Contact Attachments
      description: Parameters contacts contact  attachments
      operationId: parametersContactsContactAttachments
      x-api-path-slug: contactscontact-idattachments-parameters
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Contact
      - ""
      - Attachments
  /Events{event_id}:
    get:
      summary: Get Events Event
      description: You can also retrieve information about a specific event by ...
      operationId: getEventsEvent
      x-api-path-slug: eventsevent-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
    delete:
      summary: Delete Events Event
      description: Upon success, the appointment is moved to the user's Deleted...
      operationId: deleteEventsEvent
      x-api-path-slug: eventsevent-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
    patch:
      summary: Patch Events Event
      description: To update an event, send a PATCH request to the URL of the e...
      operationId: patchEventsEvent
      x-api-path-slug: eventsevent-id-patch
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
    parameters:
      summary: Parameters Events Event
      description: Parameters events event
      operationId: parametersEventsEvent
      x-api-path-slug: eventsevent-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
  /Events{event_id}/Accept:
    post:
      summary: Add Events Event Accept
      description: Post events event  accept
      operationId: postEventsEventAccept
      x-api-path-slug: eventsevent-idaccept-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
      - ""
      - Accept
    parameters:
      summary: Parameters Events Event Accept
      description: Parameters events event  accept
      operationId: parametersEventsEventAccept
      x-api-path-slug: eventsevent-idaccept-parameters
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
      - ""
      - Accept
  /Events{event_id}/Decline:
    post:
      summary: Add Events Event Decline
      description: Post events event  decline
      operationId: postEventsEventDecline
      x-api-path-slug: eventsevent-iddecline-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
      - ""
      - Decline
    parameters:
      summary: Parameters Events Event Decline
      description: Parameters events event  decline
      operationId: parametersEventsEventDecline
      x-api-path-slug: eventsevent-iddecline-parameters
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
      - ""
      - Decline
  /Events{event_id}/TentativelyAccept:
    post:
      summary: Add Events Event Tentatively Accept
      description: Post events event  tentativelyaccept
      operationId: postEventsEventTentativelyaccept
      x-api-path-slug: eventsevent-idtentativelyaccept-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
      - ""
      - Tentativelyaccept
    parameters:
      summary: Parameters Events Event Tentatively Accept
      description: Parameters events event  tentativelyaccept
      operationId: parametersEventsEventTentativelyaccept
      x-api-path-slug: eventsevent-idtentativelyaccept-parameters
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
      - ""
      - Tentativelyaccept
  /FirstSignIn:
    get:
      summary: Get Firstsignin
      description: Get firstsignin
      operationId: getFirstsignin
      x-api-path-slug: firstsignin-get
      responses:
        200:
          description: OK
      tags:
      - Firstsignin
  /Folders{folder_id}:
    get:
      summary: Get Folders Folder
      description: You can retrieve information about other folders by using th...
      operationId: getFoldersFolder
      x-api-path-slug: foldersfolder-id-get
      responses:
        200:
          description: OK
      tags:
      - Folders
      - Folder
    post:
      summary: Add Folders Folder
      description: You can create a folder by sending a POST request with a JSO...
      operationId: postFoldersFolder
      x-api-path-slug: foldersfolder-id-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Folders
      - Folder
    delete:
      summary: Delete Folders Folder
      description: To delete a folder, send a DELETE request to the URL of the ...
      operationId: deleteFoldersFolder
      x-api-path-slug: foldersfolder-id-delete
      responses:
        200:
          description: OK
      tags:
      - Folders
      - Folder
    patch:
      summary: Patch Folders Folder
      description: You can update a folder by sending a PATCH request with a JS...
      operationId: patchFoldersFolder
      x-api-path-slug: foldersfolder-id-patch
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Folders
      - Folder
    parameters:
      summary: Parameters Folders Folder
      description: Parameters folders folder
      operationId: parametersFoldersFolder
      x-api-path-slug: foldersfolder-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Folders
      - Folder
  /Folders{folder_id}/Messages:
    get:
      summary: Get Folders Folder Messages
      description: You can request all the emails and meeting requests in a fol...
      operationId: getFoldersFolderMessages
      x-api-path-slug: foldersfolder-idmessages-get
      responses:
        200:
          description: OK
      tags:
      - Folders
      - Folder
      - ""
      - Messages
    post:
      summary: Add Folders Folder Messages
      description: You can create an email by sending a POST request with a JSO...
      operationId: postFoldersFolderMessages
      x-api-path-slug: foldersfolder-idmessages-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: MessageDisposition
        description: When sending a POST request to create an email, there is an optional
          MessageDisposition query parameter that controls what happens to the message
          as it is created
      responses:
        200:
          description: OK
      tags:
      - Folders
      - Folder
      - ""
      - Messages
    parameters:
      summary: Parameters Folders Folder Messages
      description: Parameters folders folder  messages
      operationId: parametersFoldersFolderMessages
      x-api-path-slug: foldersfolder-idmessages-parameters
      responses:
        200:
          description: OK
      tags:
      - Folders
      - Folder
      - ""
      - Messages
  /Messages{event_id}/Send:
    post:
      summary: Add Messages Event Send
      description: You can send an existing email that has the IsDraft property...
      operationId: postMessagesEventSend
      x-api-path-slug: messagesevent-idsend-post
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Event
      - ""
      - Send
    parameters:
      summary: Parameters Messages Event Send
      description: Parameters messages event  send
      operationId: parametersMessagesEventSend
      x-api-path-slug: messagesevent-idsend-parameters
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Event
      - ""
      - Send
  /Messages{message_id}:
    get:
      summary: Get Messages Message
      description: You can request information about a specific email or meetin...
      operationId: getMessagesMessage
      x-api-path-slug: messagesmessage-id-get
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
    delete:
      summary: Delete Messages Message
      description: You can delete email by simply sending a DELETE request to t...
      operationId: deleteMessagesMessage
      x-api-path-slug: messagesmessage-id-delete
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
    patch:
      summary: Patch Messages Message
      description: You can update an existing email by sending a PATCH request ...
      operationId: patchMessagesMessage
      x-api-path-slug: messagesmessage-id-patch
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
    parameters:
      summary: Parameters Messages Message
      description: Parameters messages message
      operationId: parametersMessagesMessage
      x-api-path-slug: messagesmessage-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
  /Messages{message_id}/Copy:
    post:
      summary: Add Messages Message Copy
      description: Post messages message  copy
      operationId: postMessagesMessageCopy
      x-api-path-slug: messagesmessage-idcopy-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Copy
    parameters:
      summary: Parameters Messages Message Copy
      description: Parameters messages message  copy
      operationId: parametersMessagesMessageCopy
      x-api-path-slug: messagesmessage-idcopy-parameters
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Copy
  /Messages{message_id}/CreateForward:
    post:
      summary: Add Messages Message Createforward
      description: Post messages message  createforward
      operationId: postMessagesMessageCreateforward
      x-api-path-slug: messagesmessage-idcreateforward-post
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Createforward
    parameters:
      summary: Parameters Messages Message Createforward
      description: Parameters messages message  createforward
      operationId: parametersMessagesMessageCreateforward
      x-api-path-slug: messagesmessage-idcreateforward-parameters
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Createforward
  /Messages{message_id}/CreateReply:
    post:
      summary: Add Messages Message Createreply
      description: Post messages message  createreply
      operationId: postMessagesMessageCreatereply
      x-api-path-slug: messagesmessage-idcreatereply-post
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Createreply
    parameters:
      summary: Parameters Messages Message Createreply
      description: Parameters messages message  createreply
      operationId: parametersMessagesMessageCreatereply
      x-api-path-slug: messagesmessage-idcreatereply-parameters
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Createreply
  /Messages{message_id}/CreateReplyAll:
    post:
      summary: Add Messages Message Create Reply All
      description: Post messages message  createreplyall
      operationId: postMessagesMessageCreatereplyall
      x-api-path-slug: messagesmessage-idcreatereplyall-post
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Createreplyall
    parameters:
      summary: Parameters Messages Message Create Reply All
      description: Parameters messages message  createreplyall
      operationId: parametersMessagesMessageCreatereplyall
      x-api-path-slug: messagesmessage-idcreatereplyall-parameters
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Createreplyall
  /Messages{message_id}/Forward:
    post:
      summary: Add Messages Message Forward
      description: You can forward an email by using the Forward action on the ...
      operationId: postMessagesMessageForward
      x-api-path-slug: messagesmessage-idforward-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Forward
    parameters:
      summary: Parameters Messages Message Forward
      description: Parameters messages message  forward
      operationId: parametersMessagesMessageForward
      x-api-path-slug: messagesmessage-idforward-parameters
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Forward
  /Messages{message_id}/Move:
    post:
      summary: Add Messages Message Move
      description: Post messages message  move
      operationId: postMessagesMessageMove
      x-api-path-slug: messagesmessage-idmove-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Move
    parameters:
      summary: Parameters Messages Message Move
      description: Parameters messages message  move
      operationId: parametersMessagesMessageMove
      x-api-path-slug: messagesmessage-idmove-parameters
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Move
  /Messages{message_id}/Reply:
    post:
      summary: Add Messages Message Reply
      description: Post messages message  reply
      operationId: postMessagesMessageReply
      x-api-path-slug: messagesmessage-idreply-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Reply
    parameters:
      summary: Parameters Messages Message Reply
      description: Parameters messages message  reply
      operationId: parametersMessagesMessageReply
      x-api-path-slug: messagesmessage-idreply-parameters
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Reply
  /Messages{message_id}/ReplyAll:
    post:
      summary: Add Messages Message Replyall
      description: Post messages message  replyall
      operationId: postMessagesMessageReplyall
      x-api-path-slug: messagesmessage-idreplyall-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Replyall
    parameters:
      summary: Parameters Messages Message Replyall
      description: Parameters messages message  replyall
      operationId: parametersMessagesMessageReplyall
      x-api-path-slug: messagesmessage-idreplyall-parameters
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Replyall
  /Services:
    get:
      summary: Get Services
      description: Get services
      operationId: getServices
      x-api-path-slug: services-get
      responses:
        200:
          description: OK
      tags:
      - Services