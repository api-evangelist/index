swagger: "2.0"
x-collection-name: Elastic Email
x-complete: 1
info:
  title: Elastic Email SMTP API
  description: api-for-sending-and-management-email-
  version: v1
host: api.elasticemail.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  attachments/upload/:
    get:
      summary: Upload Attachment
      description: The upload attachment command is used to upload an attachment for
        sending.
      operationId: getAttachmentsUpload
      x-api-path-slug: attachmentsupload-get
      parameters:
      - in: query
        name: api_key
        description: your api key
      - in: query
        name: file
        description: The file name being uploaded
      - in: query
        name: username
        description: username
      responses:
        200:
          description: OK
      tags:
      - Attachments
      - Upload
  lists/add-contact:
    get:
      summary: Add Existing Subscriber To List
      description: Add Existing Subscriber To List
      operationId: getListsAddContact
      x-api-path-slug: listsaddcontact-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: listname
        description: name of list you wish to add subscriber to (separate by semi-colon
          to add to multiple lists)
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Add
      - Contact
  lists/create-contact:
    get:
      summary: Create New Subscriber
      description: Create New Subscriber
      operationId: getListsCreateContact
      x-api-path-slug: listscreatecontact-get
      parameters:
      - in: query
        name: api_key
        description: your api key found on the Account screen
      - in: query
        name: birthdate
        description: date of birth of the subscriber
      - in: query
        name: city
        description: city of the subscriber
      - in: query
        name: country
        description: country of the subscriber
      - in: query
        name: email
        description: email address of subscriber/recipient
      - in: query
        name: firstname
        description: first name of the subscriber
      - in: query
        name: gender
        description: male or female
      - in: query
        name: lastname
        description: last name of the subscriber
      - in: query
        name: listname
        description: the name of the list or lists (separated by semi-colon) the subscriber
          will be added to - if blank, it will just create the subscriber
      - in: query
        name: organizationname
        description: organization name the subscriber works for
      - in: query
        name: phone
        description: phone number for the subscriber
      - in: query
        name: postalcode
        description: the zip or postal code of the subscriber
      - in: query
        name: state
        description: the state or province for the subscriber
      - in: query
        name: the zip or postal code of the subscriber
        description: Your user name
      - in: query
        name: title
        description: the title for the subscriber (Mr
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Create
      - Contact
  lists/create-lists:
    get:
      summary: Create New List
      description: Create New List
      operationId: getListsCreateLists
      x-api-path-slug: listscreatelists-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: listname
        description: name of list you wish to create
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Create
      - Lists
  lists/delete:
    get:
      summary: Delete Existing List
      description: Delete Existing List
      operationId: getListsDelete
      x-api-path-slug: listsdelete-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: listname
        description: name of list you wish to delete
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Delete
  lists/delete-contact:
    get:
      summary: Delete Existing Subscriber
      description: Delete Existing Subscriber
      operationId: getListsDeleteContact
      x-api-path-slug: listsdeletecontact-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: email
        description: email address of subscriber/recipient (separate by semi-colon
          to remove multiple)
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Delete
      - Contact
  lists/remove-contact:
    get:
      summary: Remove Existing Subscriber From List
      description: Remove Existing Subscriber From List
      operationId: getListsRemoveContact
      x-api-path-slug: listsremovecontact-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: listname
        description: name of list you wish to remove subscriber from (separate by
          semi-colon to remove from multiple lists)
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Remove
      - Contact
  lists/upload-contacts:
    get:
      summary: Create Multiple Subscriber From CSV File
      description: Create Multiple Subscriber From CSV File
      operationId: getListsUploadContacts
      x-api-path-slug: listsuploadcontacts-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: birthdate
        description: date of birth of the subscriber
      - in: query
        name: city
        description: city of the subscriber
      - in: query
        name: country
        description: country of the subscriber
      - in: query
        name: email
        description: email address of subscriber/recipient
      - in: query
        name: firstname
        description: first name of the subscriber
      - in: query
        name: gender
        description: male or female
      - in: query
        name: lastname
        description: last name of the subscriber
      - in: query
        name: listname
        description: the name of the list or lists (separated by semi-colon) the subscriber
          will be added to - if blank, it will just create the subscriber
      - in: query
        name: organizationname
        description: organization name the subscriber works for
      - in: query
        name: phone
        description: phone number for the subscriber
      - in: query
        name: postalcode
        description: the zip or postal code of the subscriber
      - in: query
        name: state
        description: the state or province for the subscriber
      - in: query
        name: title
        description: the title for the subscriber (Mr
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Upload
      - Contacts
  mailer/account-details:
    get:
      summary: Account Details
      description: The Account Details command is used to determine how much credit
        you have left.
      operationId: getMailerAccountDetails
      x-api-path-slug: maileraccountdetails-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - Account
      - Details
  mailer/channel/delete:
    get:
      summary: Deleting Channel
      description: Deleting Channel
      operationId: getMailerChannelDelete
      x-api-path-slug: mailerchanneldelete-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: format
        description: csv or xml
      - in: query
        name: name
        description: channel name to delete
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - Channel
      - Delete
  mailer/channel/list:
    get:
      summary: Listing of Active Channels
      description: Listing of Active Channels
      operationId: getMailerChannelList
      x-api-path-slug: mailerchannellist-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: format
        description: csv or xml
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - Channel
      - List
  mailer/list/bounced:
    get:
      summary: Bounced
      description: This api will return you the list of email addresses which are
        currently in your block list.
      operationId: getMailerListBounced
      x-api-path-slug: mailerlistbounced-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - List
      - Bounced
  mailer/list/complaint:
    get:
      summary: Complaint
      description: This api will return you the list of email addresses which are
        currently in your block list.
      operationId: getMailerListComplaint
      x-api-path-slug: mailerlistcomplaint-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - List
      - Complaint
  mailer/lists/unsubscribed:
    get:
      summary: Unsubscribed
      description: This api will return you the list of email addresses which are
        currently in your block list.
      operationId: getMailerListsUnsubscribed
      x-api-path-slug: mailerlistsunsubscribed-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - Lists
      - Unsubscribed
  mailer/send/:
    get:
      summary: Send Email
      description: api.elasticemail.com
      operationId: getMailerSend
      x-api-path-slug: mailersend-get
      parameters:
      - in: query
        name: api_key
        description: your api key
      - in: query
        name: body_html
        description: html email body
      - in: query
        name: body_text
        description: text email body
      - in: query
        name: channel
        description: an id field (max 60 chars) that can be used for reporting
      - in: query
        name: charset
        description: 'text value of encoding for example: iso-8859-1, windows-1251,
          utf-8, us-ascii, windows-1250'
      - in: query
        name: encodingtype
        description: 0 for None, 1 for Raw7Bit, 2 for Raw8Bit, 3 for QuotedPrintable,
          4 for Base64 (Default), 5 for Uue  note that you can also provide the text
          version such as Raw7Bit for value 1
      - in: query
        name: from
        description: from email address
      - in: query
        name: from_name
        description: display name for from email address
      - in: query
        name: lists
        description: the name of a contact list you would like to send to
      - in: query
        name: merge_firstname
        description: if sending to a template you can send merge_ fields to merge
          data with the template
      - in: query
        name: merge_lastname
        description: if sending to a template you can send merge_ fields to merge
          data with the template
      - in: query
        name: reply_to
        description: email address to reply to
      - in: query
        name: reply_to_name
        description: display name of the reply to address
      - in: query
        name: sender
        description: email address of the sender
      - in: query
        name: sender_name
        description: display name sender
      - in: query
        name: subject
        description: email subject
      - in: query
        name: template
        description: the name of an email template you have created in your account
      - in: query
        name: time_offset_minutes
        description: number of minutes in the future this email should be sent
      - in: query
        name: total
        description: semi colon separated list of email recipients (each email is
          treated separately, like a BCC)
      - in: query
        name: username
        description: your account email address
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - Send
  mailer/status/log:
    get:
      summary: Log Activity
      description: The detailed activity log api allows you to get detailed information
        from your activity log on the emails that you have sent. Information can be
        narrowed by email status, channel and datetime.
      operationId: getMailerStatusLog
      x-api-path-slug: mailerstatuslog-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: channel
        description: If you included a channel name when submitting your requests
          you can filter here
      - in: query
        name: compress
        description: True if you want the results returned as a compressed zip file
      - in: query
        name: format
        description: xml or csv
      - in: query
        name: from
        description: 'Server time in the format: 5/19/2011 10:54:20 PM'
      - in: query
        name: status
        description: 'One of the following status values: 0 or all, 1 for ReadyToSend,
          2 for InProgress, 4 for Bounced, 5 for Sent, 6 for Opened, 7 for Clicked,
          8 for Unsubscribed, 9 for Abuse Report'
      - in: query
        name: to
        description: 'Server time in the format: 5/19/2011 10:54:20 PM'
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - Status
      - Log
  mailer/status/{message_id}:
    get:
      summary: Get Status
      description: Get the status of an email message
      operationId: getMailerStatusMessage
      x-api-path-slug: mailerstatusmessage-id-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: path
        name: message_id
        description: The ID of the email message
      - in: query
        name: showdelivered
        description: true - This will return all the recipients who succeeded
      - in: query
        name: showdetails
        description: true  - This will return all recipients for each status
      - in: query
        name: showerrors
        description: true - This will return all the recipients who bounced with details
          on why
      - in: query
        name: showfailed
        description: true - This will return all the recipients who bounced
      - in: query
        name: showpending
        description: true - This will return all the recipients still in progress
      - in: query
        name: showstats
        description: Show stats
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - Status
      - Message
      - Id