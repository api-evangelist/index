swagger: "2.0"
x-collection-name: Data2CRM
x-complete: 1
info:
  title: Data2CRM.API
  description: pmake-use-of-our-indepth-documentation-to-get-more-information-about-the-various-functions-of-the-service--those-willing-to-explore-the-mechanics-of-data2crm-api-can-test-it-in-live-regime-using-the-short-code-samples-ppselect-crm-span-iddocsselectcrm-stylefontweight-boldloading----please-waitspanpphere-are-the-api-access-keysbrbxapi2crmuserkeyb-span-iddocsuserkeye2a6379ab878ae7e58119d4ec842bf9c926e05b5spanbrbxapi2crmcrmkeyb-span-iddocscrmkey7ae5b17008fb414d84981191cf3b66a476ef8befspanpp-iddocscrmaccessthe-crm-access-details-arebrburlb-a-iddocscrmurl-hrefhttpslogin-salesforce-com-target-blankhttpslogin-salesforce-comabrbemail--usernameb-span-iddocscrmusernamedevelopers-data2crm-api1magneticone-comspanbrbpasswordb-span-iddocscrmpassworddata2crmapi123spanp
  version: "1"
host: api.data2crm.com:80
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account:
    get:
      summary: GET for Account
      description: Returns all accounts from the system
      operationId: getAccountCollection
      x-api-path-slug: account-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Accounts
    post:
      summary: POST for Account
      description: Add account into the system
      operationId: createAccountEntity
      x-api-path-slug: account-post
      parameters:
      - in: body
        name: body
        description: Add account into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /account/count:
    get:
      summary: COUNT for Account
      description: Count all accounts from the system
      operationId: getAccountCountCollection
      x-api-path-slug: accountcount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Count
  /account/describe:
    get:
      summary: DESCRIBE for Account
      description: Returns describe for accounts
      operationId: getAccountDescribe
      x-api-path-slug: accountdescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Describe
  /account/{account_id}:
    delete:
      summary: DELETE for Account
      description: Delete account information
      operationId: deleteAccountEntity
      x-api-path-slug: accountaccount-id-delete
      parameters:
      - in: path
        name: account_id
        description: Account Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Accounts
    get:
      summary: GET for Account
      description: Return account information
      operationId: getAccountEntity
      x-api-path-slug: accountaccount-id-get
      parameters:
      - in: path
        name: account_id
        description: Account Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Accounts
    put:
      summary: PUT for Account
      description: Update account information
      operationId: updateAccountEntity
      x-api-path-slug: accountaccount-id-put
      parameters:
      - in: path
        name: account_id
        description: Account Identifier
      - in: body
        name: body
        description: Update account information
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /attachment:
    get:
      summary: GET for Attachment
      description: Returns all attachments from the system
      operationId: getAttachmentCollection
      x-api-path-slug: attachment-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: query
        name: parent_id
        description: Parent Identifier
      - in: query
        name: parent_type
        description: Parent Type
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Attachments
    post:
      summary: POST for Attachment
      description: Add attachment into the system
      operationId: createAttachmentEntity
      x-api-path-slug: attachment-post
      parameters:
      - in: body
        name: body
        description: Add attachment into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Attachments
  /attachment/count:
    get:
      summary: COUNT for Attachment
      description: Count all attachments from the system
      operationId: getAttachmentCountCollection
      x-api-path-slug: attachmentcount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Attachments
      - Count
  /attachment/describe:
    get:
      summary: DESCRIBE for Attachment
      description: Returns describe for attachments
      operationId: getAttachmentDescribe
      x-api-path-slug: attachmentdescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Attachments
      - Describe
  /attachment/{attachment_id}:
    delete:
      summary: DELETE for Attachment
      description: Delete attachment information
      operationId: deleteAttachmentEntity
      x-api-path-slug: attachmentattachment-id-delete
      parameters:
      - in: path
        name: attachment_id
        description: Attachment Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Attachments
    get:
      summary: GET for Attachment
      description: Return attachment information
      operationId: getAttachmentEntity
      x-api-path-slug: attachmentattachment-id-get
      parameters:
      - in: path
        name: attachment_id
        description: Attachment Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Attachments
    put:
      summary: PUT for Attachment
      description: Update attachment information
      operationId: updateAttachmentEntity
      x-api-path-slug: attachmentattachment-id-put
      parameters:
      - in: path
        name: attachment_id
        description: Attachment Identifier
      - in: body
        name: body
        description: Update attachment information
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Attachments
  /call:
    get:
      summary: GET for Call
      description: Returns all calls from the system
      operationId: getCallCollection
      x-api-path-slug: call-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: query
        name: parent_id
        description: Parent Identifier
      - in: query
        name: parent_type
        description: Parent Type
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Calls
    post:
      summary: POST for Call
      description: Add call into the system
      operationId: createCallEntity
      x-api-path-slug: call-post
      parameters:
      - in: body
        name: body
        description: Add call into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Calls
  /call/count:
    get:
      summary: COUNT for Call
      description: Count all calls from the system
      operationId: getCallCountCollection
      x-api-path-slug: callcount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Count
  /call/describe:
    get:
      summary: DESCRIBE for Call
      description: Returns describe for calls
      operationId: getCallDescribe
      x-api-path-slug: calldescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Describe
  /call/{call_id}:
    delete:
      summary: DELETE for Call
      description: Delete call information
      operationId: deleteCallEntity
      x-api-path-slug: callcall-id-delete
      parameters:
      - in: path
        name: call_id
        description: Call Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Calls
    get:
      summary: GET for Call
      description: Return call information
      operationId: getCallEntity
      x-api-path-slug: callcall-id-get
      parameters:
      - in: path
        name: call_id
        description: Call Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Calls
    put:
      summary: PUT for Call
      description: Update call information
      operationId: updateCallEntity
      x-api-path-slug: callcall-id-put
      parameters:
      - in: body
        name: body
        description: Update call information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: call_id
        description: Call Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Calls
  /contact:
    get:
      summary: GET for Contact
      description: Returns all contacts from the system
      operationId: getContactCollection
      x-api-path-slug: contact-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Contacts
    post:
      summary: POST for Contact
      description: Add contact into the system
      operationId: createContactEntity
      x-api-path-slug: contact-post
      parameters:
      - in: body
        name: body
        description: Add contact into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Contacts
  /contact/count:
    get:
      summary: COUNT for Contact
      description: Count all contacts from the system
      operationId: getContactCountCollection
      x-api-path-slug: contactcount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Count
  /contact/describe:
    get:
      summary: DESCRIBE for Contact
      description: Returns describe for contacts
      operationId: getContactDescribe
      x-api-path-slug: contactdescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Describe
  /contact/{contact_id}:
    delete:
      summary: DELETE for Contact
      description: Delete contact information
      operationId: deleteContactEntity
      x-api-path-slug: contactcontact-id-delete
      parameters:
      - in: path
        name: contact_id
        description: Contact Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Contacts
    get:
      summary: GET for Contact
      description: Return contact information
      operationId: getContactEntity
      x-api-path-slug: contactcontact-id-get
      parameters:
      - in: path
        name: contact_id
        description: Contact Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Contacts
    put:
      summary: PUT for Contact
      description: Update contact information
      operationId: updateContactEntity
      x-api-path-slug: contactcontact-id-put
      parameters:
      - in: body
        name: body
        description: Update contact information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contact_id
        description: Contact Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Contacts
  /crm:
    get:
      summary: GET for Crm
      description: Returns all CRMs from the system
      operationId: getCrmCollection
      x-api-path-slug: crm-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: query
        name: type
        description: Type
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - CRM
    post:
      summary: POST for Crm
      description: Add CRM into the systemWhat do I need to connect a CRM to Data2CRM.API?
      operationId: createCrmEntity
      x-api-path-slug: crm-post
      parameters:
      - in: body
        name: body
        description: Add CRM into the systemWhat do I need to connect a CRM to Data2CRM
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - CRM
  /crm/count:
    get:
      summary: COUNT for Crm
      description: Count all CRMs from the system
      operationId: getCrmCountCollection
      x-api-path-slug: crmcount-get
      parameters:
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Crm
      - Count
  /crm/{crm_id}:
    delete:
      summary: DELETE for Crm
      description: Delete CRM information
      operationId: deleteCrmEntity
      x-api-path-slug: crmcrm-id-delete
      parameters:
      - in: path
        name: crm_id
        description: CRM Identifier
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - CRM
    get:
      summary: GET for Crm
      description: Return CRM information
      operationId: getCrmEntity
      x-api-path-slug: crmcrm-id-get
      parameters:
      - in: path
        name: crm_id
        description: CRM Identifier
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - CRM
    put:
      summary: PUT for Crm
      description: Update CRM informationWhat do I need to connect a CRM to Data2CRM.API?
      operationId: updateCrmEntity
      x-api-path-slug: crmcrm-id-put
      parameters:
      - in: body
        name: body
        description: Update CRM informationWhat do I need to connect a CRM to Data2CRM
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: crm_id
        description: CRM Identifier
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - CRM
  /customField:
    get:
      summary: GET for CustomField
      description: Returns all custom field from the system
      operationId: getCustomFieldCollection
      x-api-path-slug: customfield-get
      parameters:
      - in: query
        name: entity
        description: Entity
      - in: query
        name: filter
        description: Filter
      - in: query
        name: label
        description: Label
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: name
        description: Name
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Fields
    post:
      summary: POST for CustomField
      description: Add custom field into the system
      operationId: createCustomFieldEntity
      x-api-path-slug: customfield-post
      parameters:
      - in: body
        name: body
        description: Add custom field into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Fields
  /customField/{custom_field_id}:
    delete:
      summary: DELETE for CustomField
      description: Delete custom field information
      operationId: deleteCustomFieldEntity
      x-api-path-slug: customfieldcustom-field-id-delete
      parameters:
      - in: path
        name: custom_field_id
        description: Custom Field Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Fields
      - Custom
      - Field
    get:
      summary: GET for CustomField
      description: Return custom field information
      operationId: getCustomFieldEntity
      x-api-path-slug: customfieldcustom-field-id-get
      parameters:
      - in: path
        name: custom_field_id
        description: Custom Field Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Fields
      - Custom
      - Field
    put:
      summary: PUT for CustomField
      description: Update custom field information
      operationId: updateCustomFieldEntity
      x-api-path-slug: customfieldcustom-field-id-put
      parameters:
      - in: body
        name: body
        description: Update custom field information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: custom_field_id
        description: Custom Field Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Fields
      - Custom
      - Field
  /email:
    get:
      summary: GET for Email
      description: Returns all emails from the system
      operationId: getEmailCollection
      x-api-path-slug: email-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: query
        name: parent_id
        description: Parent Identifier
      - in: query
        name: parent_type
        description: Parent Type
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Emails
    post:
      summary: POST for Email
      description: Add email into the system
      operationId: createEmailEntity
      x-api-path-slug: email-post
      parameters:
      - in: body
        name: body
        description: Add email into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Emails
  /email/count:
    get:
      summary: COUNT for Email
      description: Count all emails from the system
      operationId: getEmailCountCollection
      x-api-path-slug: emailcount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Emails
      - Count
  /email/describe:
    get:
      summary: DESCRIBE for Email
      description: Returns describe for emails
      operationId: getEmailDescribe
      x-api-path-slug: emaildescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Emails
      - Describe
  /email/{email_id}:
    delete:
      summary: DELETE for Email
      description: Delete email information
      operationId: deleteEmailEntity
      x-api-path-slug: emailemail-id-delete
      parameters:
      - in: path
        name: email_id
        description: Email Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Emails
    get:
      summary: GET for Email
      description: Return email information
      operationId: getEmailEntity
      x-api-path-slug: emailemail-id-get
      parameters:
      - in: path
        name: email_id
        description: Email Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Emails
    put:
      summary: PUT for Email
      description: Update email information
      operationId: updateEmailEntity
      x-api-path-slug: emailemail-id-put
      parameters:
      - in: body
        name: body
        description: Update email information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: email_id
        description: Email Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Emails
  /event:
    get:
      summary: GET for Event
      description: Returns all events from the system
      operationId: getEventCollection
      x-api-path-slug: event-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: query
        name: parent_id
        description: Parent Identifier
      - in: query
        name: parent_type
        description: Parent Type
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Events
    post:
      summary: POST for Event
      description: Add event into the system
      operationId: createEventEntity
      x-api-path-slug: event-post
      parameters:
      - in: body
        name: body
        description: Add event into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Events
  /event/count:
    get:
      summary: COUNT for Event
      description: Count all events from the system
      operationId: getEventCountCollection
      x-api-path-slug: eventcount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Events
      - Count
  /event/describe:
    get:
      summary: DESCRIBE for Event
      description: Returns describe for events
      operationId: getEventDescribe
      x-api-path-slug: eventdescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Events
      - Describe
  /event/{event_id}:
    delete:
      summary: DELETE for Event
      description: Delete event information
      operationId: deleteEventEntity
      x-api-path-slug: eventevent-id-delete
      parameters:
      - in: path
        name: event_id
        description: Event Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Events
    get:
      summary: GET for Event
      description: Return event information
      operationId: getEventEntity
      x-api-path-slug: eventevent-id-get
      parameters:
      - in: path
        name: event_id
        description: Event Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Events
    put:
      summary: PUT for Event
      description: Update event information
      operationId: updateEventEntity
      x-api-path-slug: eventevent-id-put
      parameters:
      - in: body
        name: body
        description: Update event information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: event_id
        description: Event Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Events
  /lead:
    get:
      summary: GET for Lead
      description: Returns all leads from the system
      operationId: getLeadCollection
      x-api-path-slug: lead-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Leads
    post:
      summary: POST for Lead
      description: Add lead into the system
      operationId: createLeadEntity
      x-api-path-slug: lead-post
      parameters:
      - in: body
        name: body
        description: Add lead into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Leads
  /lead/count:
    get:
      summary: COUNT for Lead
      description: Count all leads from the system
      operationId: getLeadCountCollection
      x-api-path-slug: leadcount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Count
  /lead/describe:
    get:
      summary: DESCRIBE for Lead
      description: Returns describe for leads
      operationId: getLeadDescribe
      x-api-path-slug: leaddescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Leads
      - Describe
  /lead/{lead_id}:
    delete:
      summary: DELETE for Lead
      description: Delete lead information
      operationId: deleteLeadEntity
      x-api-path-slug: leadlead-id-delete
      parameters:
      - in: path
        name: lead_id
        description: Lead Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Leads
    get:
      summary: GET for Lead
      description: Return lead information
      operationId: getLeadEntity
      x-api-path-slug: leadlead-id-get
      parameters:
      - in: path
        name: lead_id
        description: Lead Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Leads
    put:
      summary: PUT for Lead
      description: Update lead information
      operationId: updateLeadEntity
      x-api-path-slug: leadlead-id-put
      parameters:
      - in: body
        name: body
        description: Update lead information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lead_id
        description: Lead Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Leads
  /meeting:
    get:
      summary: GET for Meeting
      description: Returns all meetings from the system
      operationId: getMeetingCollection
      x-api-path-slug: meeting-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: query
        name: parent_id
        description: Parent Identifier
      - in: query
        name: parent_type
        description: Parent Type
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Meeting
    post:
      summary: POST for Meeting
      description: Add meeting into the system
      operationId: createMeetingEntity
      x-api-path-slug: meeting-post
      parameters:
      - in: body
        name: body
        description: Add meeting into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Meeting
  /meeting/count:
    get:
      summary: COUNT for Meeting
      description: Count all meetings from the system
      operationId: getMeetingCountCollection
      x-api-path-slug: meetingcount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Meeting
      - Count
  /meeting/describe:
    get:
      summary: DESCRIBE for Meeting
      description: Returns describe for meetings
      operationId: getMeetingDescribe
      x-api-path-slug: meetingdescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Meeting
      - Describe
  /meeting/{meeting_id}:
    delete:
      summary: DELETE for Meeting
      description: Delete meeting information
      operationId: deleteMeetingEntity
      x-api-path-slug: meetingmeeting-id-delete
      parameters:
      - in: path
        name: meeting_id
        description: Meeting Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Meetings
    get:
      summary: GET for Meeting
      description: Return meeting information
      operationId: getMeetingEntity
      x-api-path-slug: meetingmeeting-id-get
      parameters:
      - in: path
        name: meeting_id
        description: Meeting Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Meetings
    put:
      summary: PUT for Meeting
      description: Update meeting information
      operationId: updateMeetingEntity
      x-api-path-slug: meetingmeeting-id-put
      parameters:
      - in: body
        name: body
        description: Update meeting information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: meeting_id
        description: Meeting Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Meetings
  /note:
    get:
      summary: GET for Note
      description: Returns all notes from the system
      operationId: getNoteCollection
      x-api-path-slug: note-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: query
        name: parent_id
        description: Parent Identifier
      - in: query
        name: parent_type
        description: Parent Type
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Note
    post:
      summary: POST for Note
      description: Add note into the system
      operationId: createNoteEntity
      x-api-path-slug: note-post
      parameters:
      - in: body
        name: body
        description: Add note into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Note
  /note/count:
    get:
      summary: COUNT for Note
      description: Count all notes from the system
      operationId: getNoteCountCollection
      x-api-path-slug: notecount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Note
      - Count
  /note/describe:
    get:
      summary: DESCRIBE for Note
      description: Returns describe for notes
      operationId: getNoteDescribe
      x-api-path-slug: notedescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Note
      - Describe
  /note/{note_id}:
    delete:
      summary: DELETE for Note
      description: Delete note information
      operationId: deleteNoteEntity
      x-api-path-slug: notenote-id-delete
      parameters:
      - in: path
        name: note_id
        description: Note Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Notes
    get:
      summary: GET for Note
      description: Return note information
      operationId: getNoteEntity
      x-api-path-slug: notenote-id-get
      parameters:
      - in: path
        name: note_id
        description: Note Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Notes
    put:
      summary: PUT for Note
      description: Update note information
      operationId: updateNoteEntity
      x-api-path-slug: notenote-id-put
      parameters:
      - in: body
        name: body
        description: Update note information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: note_id
        description: Note Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Notes
  /opportunity:
    get:
      summary: GET for Opportunity
      description: Returns all opportunities from the system
      operationId: getOpportunityCollection
      x-api-path-slug: opportunity-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Opportunities
    post:
      summary: POST for Opportunity
      description: Add opportunity into the system
      operationId: createOpportunityEntity
      x-api-path-slug: opportunity-post
      parameters:
      - in: body
        name: body
        description: Add opportunity into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Opportunities
  /opportunity/count:
    get:
      summary: COUNT for Opportunity
      description: Count all opportunities from the system
      operationId: getOpportunityCountCollection
      x-api-path-slug: opportunitycount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Opportunities
      - Count
  /opportunity/describe:
    get:
      summary: DESCRIBE for Opportunity
      description: Returns describe for opportunities
      operationId: getOpportunityDescribe
      x-api-path-slug: opportunitydescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Opportunities
      - Describe
  /opportunity/{opportunity_id}:
    delete:
      summary: DELETE for Opportunity
      description: Delete opportunity information
      operationId: deleteOpportunityEntity
      x-api-path-slug: opportunityopportunity-id-delete
      parameters:
      - in: path
        name: opportunity_id
        description: Opportunity Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Opportunities
    get:
      summary: GET for Opportunity
      description: Return opportunity information
      operationId: getOpportunityEntity
      x-api-path-slug: opportunityopportunity-id-get
      parameters:
      - in: path
        name: opportunity_id
        description: Opportunity Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Opportunities
    put:
      summary: PUT for Opportunity
      description: Update opportunity information
      operationId: updateOpportunityEntity
      x-api-path-slug: opportunityopportunity-id-put
      parameters:
      - in: body
        name: body
        description: Update opportunity information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: opportunity_id
        description: Opportunity Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Opportunities
  /task:
    get:
      summary: GET for Task
      description: Returns all tasks from the system
      operationId: getTaskCollection
      x-api-path-slug: task-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Tasks
    post:
      summary: POST for Task
      description: Add task into the system
      operationId: createTaskEntity
      x-api-path-slug: task-post
      parameters:
      - in: body
        name: body
        description: Add task into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /task/count:
    get:
      summary: COUNT for Task
      description: Count all tasks from the system
      operationId: getTaskCountCollection
      x-api-path-slug: taskcount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Tasks
      - Count
  /task/describe:
    get:
      summary: DESCRIBE for Task
      description: Returns describe for tasks
      operationId: getTaskDescribe
      x-api-path-slug: taskdescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Tasks
      - Describe
  /task/{task_id}:
    delete:
      summary: DELETE for Task
      description: Delete task information
      operationId: deleteTaskEntity
      x-api-path-slug: tasktask-id-delete
      parameters:
      - in: path
        name: task_id
        description: Task Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Tasks
    get:
      summary: GET for Task
      description: Return task information
      operationId: getTaskEntity
      x-api-path-slug: tasktask-id-get
      parameters:
      - in: path
        name: task_id
        description: Task Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Tasks
    put:
      summary: PUT for Task
      description: Update task information
      operationId: updateTaskEntity
      x-api-path-slug: tasktask-id-put
      parameters:
      - in: body
        name: body
        description: Update task information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: task_id
        description: Task Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /user:
    get:
      summary: GET for User
      description: Returns all users from the system
      operationId: getUserCollection
      x-api-path-slug: user-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Users
    post:
      summary: POST for User
      description: Add user into the system
      operationId: createUserEntity
      x-api-path-slug: user-post
      parameters:
      - in: body
        name: body
        description: Add user into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Users
  /user/count:
    get:
      summary: COUNT for User
      description: Count all users from the system
      operationId: getUserCountCollection
      x-api-path-slug: usercount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Count
  /user/describe:
    get:
      summary: DESCRIBE for User
      description: Returns describe for users
      operationId: getUserDescribe
      x-api-path-slug: userdescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Describe
  /user/{user_id}:
    delete:
      summary: DELETE for User
      description: Delete user information
      operationId: deleteUserEntity
      x-api-path-slug: useruser-id-delete
      parameters:
      - in: path
        name: user_id
        description: User Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Users
    get:
      summary: GET for User
      description: Return user information
      operationId: getUserEntity
      x-api-path-slug: useruser-id-get
      parameters:
      - in: path
        name: user_id
        description: User Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Users
    put:
      summary: PUT for User
      description: Update user information
      operationId: updateUserEntity
      x-api-path-slug: useruser-id-put
      parameters:
      - in: body
        name: body
        description: Update user information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: User Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Users