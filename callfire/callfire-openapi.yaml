swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calls:
    get:
      summary: Find calls
      description: To search for all calls sent or received by the user. Use "id=0"
        for the campaignId parameter to query for all calls sent through the POST
        /calls API. See [call states and results](https://developers.callfire.com/results-responses-errors.html)
      operationId: findCalls
      x-api-path-slug: calls-get
      parameters:
      - in: query
        name: batchId
        description: An id of a contact batch, queries for calls of a particular contact
          batch
      - in: query
        name: campaignId
        description: An id of a campaign, queries for calls included to a particular
          campaign
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: fromNumber
        description: Phone number in E
      - in: query
        name: id
        description: Lists the Call ids to search for
      - in: query
        name: inbound
        description: Filters inbound calls for true value and outbound calls for false
          value
      - in: query
        name: intervalBegin
        description: Start of the find time interval, formatted in unix time milliseconds
      - in: query
        name: intervalEnd
        description: End of the find time interval, formatted in unix time milliseconds
      - in: query
        name: label
        description: A label for a specific call
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      - in: query
        name: results
        description: Searches for all calls with statuses listed in a comma separated
          string
      - in: query
        name: states
        description: Searches for all calls which correspond to statuses listed in
          a comma separated string
      - in: query
        name: toNumber
        description: Phone number in E
      responses:
        200:
          description: OK
      tags:
      - Calls
    post:
      summary: Send calls
      description: Use the /calls API to send individual calls quickly. A verified
        Caller ID and sufficient credits are required to make a call. CallRecipient
        represents a single recipient identified by phone number or contact id in
        CallFire system. You can attach user-defined attributes to a Call action via
        CallRecipient.attributes property, attributes are available in Call action
        response
      operationId: sendCalls
      x-api-path-slug: calls-post
      parameters:
      - in: body
        name: body
        description: An array of CallRecipient objects
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: campaignId
        description: Specifies a campaignId to send calls quickly on a previously
          created campaign
      - in: query
        name: defaultLiveMessage
        description: Text to be turned into a sound, this text will be played when
          the phone is answered
      - in: query
        name: defaultLiveMessageSoundId
        description: Id of sound file to play if phone is answered
      - in: query
        name: defaultMachineMessage
        description: Text to be turned into a sound, this text will be played when
          answering machine is detected
      - in: query
        name: defaultMachineMessageSoundId
        description: An id of a sound file to play if answering machine is detected
      - in: query
        name: defaultVoice
        description: The voice set by default for all text-to-speech messages defined
          in CallRecipient objects or as default *Message properties
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Calls
  /calls/broadcasts:
    get:
      summary: Find call broadcasts
      description: Searches for all voice broadcasts created by user. Can query on
        label, name, and the current running status of the campaign. Returns a paged
        list of voice broadcasts
      operationId: findCallBroadcasts
      x-api-path-slug: callsbroadcasts-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: label
        description: A label of a voice broadcast
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: name
        description: A name of voice broadcast
      - in: query
        name: offset
        description: Offset to the start of a given page
      - in: query
        name: running
        description: Specify whether the campaigns should be running or not
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
    post:
      summary: Create a call broadcast
      description: Creates a call broadcast campaign using the Call Broadcast API.
        Send a CallBroadcast in the message body to add details in a voice broadcast
        campaign. The campaign can be created without contacts and bare minimum configuration,
        but contacts will have to be added further on to use the campaign
      operationId: createCallBroadcast
      x-api-path-slug: callsbroadcasts-post
      parameters:
      - in: body
        name: body
        description: A CallBroadcast object
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: start
        description: Specify whether to immediately start this campaign (not required)
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
  /calls/broadcasts/{id}:
    get:
      summary: Find a specific call broadcast
      description: Returns a single CallBroadcast instance for a given call broadcast
        campaign id
      operationId: getCallBroadcast
      x-api-path-slug: callsbroadcastsid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a CallBroadcast
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
    put:
      summary: Update a call broadcast
      description: This operation lets the user modify the configuration of a voice
        broadcast campaign after call broadcast campaign is created. See CallBroadcast
        for more information on what can/can't be updated on this API
      operationId: updateCallBroadcast
      x-api-path-slug: callsbroadcastsid-put
      parameters:
      - in: body
        name: body
        description: A CallBroadcast object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: An id of a voice broadcast
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
  /calls/broadcasts/{id}/archive:
    post:
      summary: Archive voice broadcast
      description: Archives a voice broadcast (voice broadcast will be hidden in search
        results)
      operationId: archiveVoiceBroadcast
      x-api-path-slug: callsbroadcastsidarchive-post
      parameters:
      - in: path
        name: id
        description: An id of a voice broadcast to archive
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Archive
  /calls/broadcasts/{id}/batches:
    get:
      summary: Find batches in a call broadcast
      description: This endpoint will enable the user to page through all of the batches
        for a particular voice broadcast campaign
      operationId: getCallBroadcastBatches
      x-api-path-slug: callsbroadcastsidbatches-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a call broadcast
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Batches
    post:
      summary: Add batches to a call broadcast
      description: The 'add batch' API allows user to add additional batches to an
        already created voice broadcast campaign. The added batch will go through
        the CallFire validation process, unlike in the recipients version of this
        API. That is why you can use the scrubDuplicates flag to remove duplicates
        from your batch. Batches may be added as a contact list id, a list of contact
        ids, or a list of numbers
      operationId: addCallBroadcastBatch
      x-api-path-slug: callsbroadcastsidbatches-post
      parameters:
      - in: body
        name: body
        description: A request object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: An id of a call broadcast
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Batches
  /calls/broadcasts/{id}/calls:
    get:
      summary: Find calls in a call broadcast
      description: This endpoint will enable the user to page through all calls for
        a particular call broadcast campaign
      operationId: getCallBroadcastCalls
      x-api-path-slug: callsbroadcastsidcalls-get
      parameters:
      - in: query
        name: batchId
        description: An id of a particular batch associated with broadcast
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An Id of a call broadcast
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Calls
  /calls/broadcasts/{id}/recipients:
    post:
      summary: Add recipients to a call broadcast
      description: Use this API to add the recipients to an existing voice broadcast.
        Post a list of Recipient objects to be added to the voice broadcast campaign.
        These contacts will not go through validation process, and will be acted upon
        as they are added. Recipients may be added as a list of contact ids, or list
        of numbers
      operationId: addCallBroadcastRecipients
      x-api-path-slug: callsbroadcastsidrecipients-post
      parameters:
      - in: body
        name: body
        description: A list of CallRecipient objects
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a call broadcast
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Recipients
  /calls/broadcasts/{id}/start:
    post:
      summary: Start voice broadcast
      description: Start a voice broadcast
      operationId: startVoiceBroadcast
      x-api-path-slug: callsbroadcastsidstart-post
      parameters:
      - in: path
        name: id
        description: An id of voice broadcast to start
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Start
  /calls/broadcasts/{id}/stats:
    get:
      summary: Get statistics on call broadcast
      description: Returns broadcast statistics like total number of sent/received
        actions, total cost, number of remaining outbound actions, error count, etc
      operationId: getCallBroadcastStats
      x-api-path-slug: callsbroadcastsidstats-get
      parameters:
      - in: query
        name: begin
        description: Start of the search time interval, formatted in unix time milliseconds
      - in: query
        name: end
        description: End of the search time interval, formatted in unix time milliseconds
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a call broadcast
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Stats
  /calls/broadcasts/{id}/stop:
    post:
      summary: Stop voice broadcast
      description: Stop a voice broadcast
      operationId: stopVoiceBroadcast
      x-api-path-slug: callsbroadcastsidstop-post
      parameters:
      - in: path
        name: id
        description: An id of voice broadcast to stop
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Stop
  /calls/recordings/{id}:
    get:
      summary: Get call recording by id
      description: Returns metadata of recording of a particular call. Metadata contains
        a link to a MP3 recording
      operationId: getCallRecording
      x-api-path-slug: callsrecordingsid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: "~"
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Recordings
  /calls/recordings/{id}.mp3:
    get:
      summary: Get call recording in mp3 format
      description: Returns an MP3 recording of particular call, response contains
        binary data, content type is 'audio/mpeg'
      operationId: getCallRecordingMp3
      x-api-path-slug: callsrecordingsid-mp3-get
      parameters:
      - in: path
        name: id
        description: An id of a call
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Recordings.mp3
  /calls/{id}:
    get:
      summary: Find a specific call
      description: Returns a single Call instance for a given call id.
      operationId: getCall
      x-api-path-slug: callsid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a call
      responses:
        200:
          description: OK
      tags:
      - Calls
  /calls/{id}/recordings:
    get:
      summary: Get call recordings for a call
      description: Returns a list of recordings metadata of particular call. Metadata
        contains link to a MP3 recording
      operationId: getCallRecordings
      x-api-path-slug: callsidrecordings-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a call
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Recordings
  /calls/{id}/recordings/{name}:
    get:
      summary: Get call recording by name
      description: Returns recording metadata of particular call. Metadata contains
        link to a MP3 recording
      operationId: getCallRecordingByName
      x-api-path-slug: callsidrecordingsname-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a call
      - in: path
        name: name
        description: A name of a recording
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Recordings
      - Name
  /calls/{id}/recordings/{name}.mp3:
    get:
      summary: Get call mp3 recording by name
      description: Returns a MP3 recording of a particular call, response contains
        binary data, content type is 'audio/mpeg'
      operationId: getCallRecordingMp3ByName
      x-api-path-slug: callsidrecordingsname-mp3-get
      parameters:
      - in: path
        name: id
        description: An id of a call
      - in: path
        name: name
        description: A name of a recording
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Recordings
      - Name.mp3
  /campaigns/batches/{id}:
    get:
      summary: Find a specific batch
      description: Returns a single Batch instance for a given batch id. This API
        is useful for determining the state of a validating batch
      operationId: getCampaignBatch
      x-api-path-slug: campaignsbatchesid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a batch
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Batches
    put:
      summary: Update a batch
      description: Updates a single Batch instance, currently batch can only be turned
        "on/off"
      operationId: updateCampaignBatch
      x-api-path-slug: campaignsbatchesid-put
      parameters:
      - in: body
        name: body
        description: A batch instance
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: An id of a batch to update
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Batches
  /campaigns/sounds:
    get:
      summary: Find sounds
      description: To find all campaign sounds which were created by user. Returns
        all sounds available to be used in campaigns
      operationId: findCampaignSounds
      x-api-path-slug: campaignssounds-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: filter
        description: Name of a file to search for
      - in: query
        name: includeArchived
        description: Includes ARCHIVED sounds for true value
      - in: query
        name: includePending
        description: Includes UPLOAD/RECORDING sounds for true value
      - in: query
        name: includeScrubbed
        description: Includes SCRUBBED sounds for true value
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Sounds
  /campaigns/sounds/calls:
    post:
      summary: Add sound via call
      description: Use this API to create a sound via a phone call. Provide the required
        phone number in the CallCreateSound object inside the request, and user will
        receive a call shortly after with instructions on how to record a sound over
        the phone.
      operationId: postCallCampaignSound
      x-api-path-slug: campaignssoundscalls-post
      parameters:
      - in: body
        name: body
        description: Request object containing the name of a new campaign sound and
          phone number to call up
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Limit fields received in response
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Sounds
      - Calls
  /campaigns/sounds/files:
    post:
      summary: Add sound via file
      description: Create a campaign sound file via a supplied .mp3 or .wav file
      operationId: postFileCampaignSound
      x-api-path-slug: campaignssoundsfiles-post
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: formData
        name: file
        description: A sound file encoded in binary form
      - in: formData
        name: name
        description: Optional name of a sound file, if the name is empty than it will
          be taken from a file
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Sounds
      - Files
  /campaigns/sounds/tts:
    post:
      summary: Add sound via text-to-speech
      description: 'Use this API to create a sound file via a supplied string of text.
        Add a text in the TextToSpeech.message field, and pick a voice in the TextToSpeech.voice
        field. Available voices are: MALE1, FEMALE1, FEMALE2, SPANISH1, FRENCHCANADIAN1'
      operationId: postTTSCampaignSound
      x-api-path-slug: campaignssoundstts-post
      parameters:
      - in: body
        name: body
        description: textToSpeech
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Limit fields received in response
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Sounds
      - Tts
  /campaigns/sounds/{id}:
    delete:
      summary: Delete a specific sound
      description: Deletes a single campaign sound instance for a specific campaign
        sound id, this operation does not delete sound completely, it sets sound status
        to ARCHIVED which means that sound will no longer appear in 'find' operation
        results, but still accessible via 'get' operation
      operationId: deleteCampaignSound
      x-api-path-slug: campaignssoundsid-delete
      parameters:
      - in: path
        name: id
        description: An id of a campaign sound
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Sounds
    get:
      summary: Find a specific sound
      description: Returns a single CampaignSound instance for a given sound id in
        campaign. This is a meta data to the sounds. No audio data is returned from
        this API
      operationId: getCampaignSound
      x-api-path-slug: campaignssoundsid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a sound campaign
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Sounds
  /campaigns/sounds/{id}.mp3:
    get:
      summary: Download a MP3 sound
      description: Download the MP3 version of a hosted file. This is an audio data
        endpoint. Returns binary response of the 'audio/mpeg' content type
      operationId: getCampaignSoundDataMp3
      x-api-path-slug: campaignssoundsid-mp3-get
      parameters:
      - in: path
        name: id
        description: An id of a campaign sound
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Sounds.mp3
  /campaigns/sounds/{id}.wav:
    get:
      summary: Download a WAV sound
      description: Download the WAV version of the hosted file. This is an audio data
        endpoint. Returns binary response of the 'audio/mpeg' content type
      operationId: getCampaignSoundDataWav
      x-api-path-slug: campaignssoundsid-wav-get
      parameters:
      - in: path
        name: id
        description: An id of a campaign sound
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - Sounds.wav
  /contacts:
    get:
      summary: Find contacts
      description: Find user's contacts by id, contact list, or on any property name.
        Returns a paged list of contacts
      operationId: findContacts
      x-api-path-slug: contacts-get
      parameters:
      - in: query
        name: contactListId
        description: Filters contacts by a particular contact list
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: id
        description: A list of contact IDs
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: number
        description: Multiple contact numbers can be specified
      - in: query
        name: offset
        description: Offset to the start of a given page
      - in: query
        name: propertyName
        description: Name of a contact property to search by
      - in: query
        name: propertyValue
        description: Value of a contact property to search by
      responses:
        200:
          description: OK
      tags:
      - Contacts
    post:
      summary: Create contacts
      description: Creates contacts in CallFire system. These contacts are not validated
        on creation. They will be validated upon being added to a campaign
      operationId: createContacts
      x-api-path-slug: contacts-post
      parameters:
      - in: body
        name: body
        description: A list of a contact objects
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contacts
  /contacts/dncs:
    get:
      summary: Find do not contact (dnc) items
      description: Searches for all Do Not Contact (DNC) objects created by user.
        These DoNotContact entries only affect calls/texts/campaigns on this account.
        Returns a paged list of DoNotContact objects
      operationId: findDoNotContacts
      x-api-path-slug: contactsdncs-get
      parameters:
      - in: query
        name: call
        description: Show only Do-Not-Call numbers
      - in: query
        name: campaignId
        description: A campaign id which was used to send a message to a DNC number
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: number
        description: "~"
      - in: query
        name: offset
        description: Offset to the start of a given page
      - in: query
        name: prefix
        description: Prefix (1-10 digits) of phone numbers
      - in: query
        name: source
        description: A DNC source name to search for DNCs
      - in: query
        name: text
        description: Show only Do-Not-Text numbers
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Dncs
    post:
      summary: Add or update do not contact (dnc) numbers
      description: Add or update a list of Do Not Contact (DNC) contact entries. Can
        toggle whether the DNCs are enabled for calls/texts.
      operationId: addDoNotContacts
      x-api-path-slug: contactsdncs-post
      parameters:
      - in: body
        name: body
        description: AddDoNotContactsRequest object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Dncs
  /contacts/dncs/sources/{source}:
    delete:
      summary: Delete do not contact (dnc) numbers contained in source.
      description: Delete Do Not Contact (DNC) contact entries contained in source.
      operationId: deleteDoNotContactsBySource
      x-api-path-slug: contactsdncssourcessource-delete
      parameters:
      - in: path
        name: source
        description: Source associated with Do Not Contact (DNC) entry
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Dncs
      - Sources
      - Source
  /contacts/dncs/universals/{toNumber}:
    get:
      summary: Find universal do not contacts (udnc) associated with toNumber
      description: Searches for a UniversalDoNotContact object for a given phone number.
        Shows whether inbound/outbound actions are allowed for a given number
      operationId: getUniversalDoNotContacts
      x-api-path-slug: contactsdncsuniversalstonumber-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: fromNumber
        description: An optional destination/source number for DNC, specified in E
      - in: path
        name: toNumber
        description: A required destination phone number in E
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Dncs
      - Universals
      - ToNumber
  /contacts/dncs/{number}:
    delete:
      summary: Delete do not contact (dnc) number. If number contains commas treat
        as list of numbers
      description: Delete a Do Not Contact (DNC) contact entry.
      operationId: deleteDoNotContact
      x-api-path-slug: contactsdncsnumber-delete
      parameters:
      - in: path
        name: number
        description: Number associated with Do Not Contact (DNC) entry
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Dncs
      - Number
    get:
      summary: Get do not contact (dnc)
      description: Get Do Not Contact (DNC) object create by user. This DoNotContact
        entry only affects calls/texts/campaigns on this account.
      operationId: getDoNotContact
      x-api-path-slug: contactsdncsnumber-get
      parameters:
      - in: path
        name: number
        description: Number associated with Do Not Contact (DNC) entry
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Dncs
      - Number
    put:
      summary: Update an individual do not contact (dnc) number
      description: Update a Do Not Contact (DNC) contact entry. Can toggle whether
        the DNC is enabled for calls/texts.
      operationId: updateDoNotContact
      x-api-path-slug: contactsdncsnumber-put
      parameters:
      - in: body
        name: body
        description: DoNotContact object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: number
        description: "~"
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Dncs
      - Number
  /contacts/lists:
    get:
      summary: Find contact lists
      description: Searches for all contact lists which are available for the current
        user. Returns a paged list of contact lists
      operationId: findContactLists
      x-api-path-slug: contactslists-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: name
        description: A name or a partial name of a contact list
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
    post:
      summary: Create contact lists
      description: Creates a contact list for use with campaigns using 1 of 3 inputs.
        A List of Contact objects, a list of String E.164 numbers, or a list of CallFire
        contactIds can be used as the data source for the created contact list. After
        contact list is added into the CallFire system, contact lists goes through
        seven system safeguards that check the accuracy and consistency of the data.
        For example, our system checks that contact number is formatted correctly,
        is valid, is not duplicated in another contact list, or is not added on a
        specific DNC list. You can configure to keep/merge or remove contacts which
        do not complies these rules. If contacts were not added to a contact list
        after the validation, this means the data needs to be properly formatted and
        corrected before calling this API
      operationId: createContactList
      x-api-path-slug: contactslists-post
      parameters:
      - in: body
        name: body
        description: A request object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
  /contacts/lists/upload:
    post:
      summary: Create contact list from file
      description: Creates a contact list to be used with campaigns through uploading
        a .csv file. Returns the id of created list
      operationId: createContactListFromFile
      x-api-path-slug: contactslistsupload-post
      parameters:
      - in: formData
        name: file
        description: CSV file to be uploaded
      - in: formData
        name: name
        description: A name of a contact list
      - in: formData
        name: useCustomFields
        description: A flag to indicate how to define property names for contacts
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
      - Upload
  /contacts/lists/{id}:
    delete:
      summary: Delete a contact list
      description: Deletes a contact list, included contacts will not be deleted.
      operationId: deleteContactList
      x-api-path-slug: contactslistsid-delete
      parameters:
      - in: path
        name: id
        description: An id of the contact list to be deleted
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
    get:
      summary: Find a specific contact list
      description: Returns a single ContactList instance for a given contact list
        id
      operationId: getContactList
      x-api-path-slug: contactslistsid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a contact list to return
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
    put:
      summary: Update a contact list
      description: Updates contact list instance.
      operationId: updateContactList
      x-api-path-slug: contactslistsid-put
      parameters:
      - in: body
        name: body
        description: A request object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: An id of contact list to update
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
  /contacts/lists/{id}/items:
    delete:
      summary: Delete contacts from a contact list
      description: Deletes contacts from a contact list. List the contact ids in request
        to delete multiple contacts with one request.
      operationId: removeContactListItems
      x-api-path-slug: contactslistsiditems-delete
      parameters:
      - in: query
        name: contactId
        description: An id of a contact entity in the CallFire system
      - in: path
        name: id
        description: A id of a contact list
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
      - Items
    get:
      summary: Find contacts in a contact list
      description: Searches for all entries in a contact list with specified id. Returns
        a paged list of contact entries
      operationId: getContactListItems
      x-api-path-slug: contactslistsiditems-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a contact list
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
      - Items
    post:
      summary: Add contacts to a contact list
      description: 'Adds contacts to a contact list. Available contact sources are:
        list of the contact entities, list of ids of existing contacts in user''s
        account, list of phone numbers in E.164 format (11-digits)'
      operationId: addContactListItems
      x-api-path-slug: contactslistsiditems-post
      parameters:
      - in: body
        name: body
        description: A request object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: An id of a contact list
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
      - Items
  /contacts/lists/{id}/items/{contactId}:
    delete:
      summary: Delete a contact from a contact list
      description: Deletes a single contact from a contact list
      operationId: removeContactListItem
      x-api-path-slug: contactslistsiditemscontactid-delete
      parameters:
      - in: path
        name: contactId
        description: An id of a contact
      - in: path
        name: id
        description: An id of a contact list
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
      - Items
      - ContactId
  /contacts/{id}:
    delete:
      summary: Delete a contact
      description: Deletes a contact instance from account
      operationId: deleteContact
      x-api-path-slug: contactsid-delete
      parameters:
      - in: path
        name: id
        description: An Id of a contact
      responses:
        200:
          description: OK
      tags:
      - Contacts
    get:
      summary: Find a specific contact
      description: Returns a Contact instance for a given contact id. Deleted contacts
        can be still retrieved but will be marked as deleted. Deleted contacts will
        not be shown in search request.
      operationId: getContact
      x-api-path-slug: contactsid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a contact
      responses:
        200:
          description: OK
      tags:
      - Contacts
    put:
      summary: Update a contact
      description: Updates a single contact instance with id specified
      operationId: updateContact
      x-api-path-slug: contactsid-put
      parameters:
      - in: body
        name: body
        description: A contact object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: An id of a contact
      responses:
        200:
          description: OK
      tags:
      - Contacts
  /contacts/{id}/history:
    get:
      summary: Find a contact's history
      description: Searches for all texts and calls attributed to a contact. Returns
        a list of calls and texts a contact has been involved with
      operationId: getContactHistory
      x-api-path-slug: contactsidhistory-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An Id of a contact
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - History
  /keywords:
    get:
      summary: Find keywords
      description: Searches for all keywords available for purchase on the CallFire
        platform. If a keyword appears in the response, it is available for purchase.
        List the 'keywords' in a query parameter to search for multiple keywords (at
        least one keyword should be sent in request)
      operationId: findKeywords
      x-api-path-slug: keywords-get
      parameters:
      - in: query
        name: keywords
        description: A keyword to search for
      responses:
        200:
          description: OK
      tags:
      - Keywords
  /keywords/leases:
    get:
      summary: Find keyword leases
      description: Searches for all keywords owned by user. A keyword lease is the
        ownership information involving a keyword
      operationId: findKeywordLeases
      x-api-path-slug: keywordsleases-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Keywords
      - Leases
  /keywords/leases/{keyword}:
    get:
      summary: Find a specific lease
      description: Searches for all keywords owned by user
      operationId: getKeywordLease
      x-api-path-slug: keywordsleaseskeyword-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: keyword
        description: Keyword text that a lease is desired for
      responses:
        200:
          description: OK
      tags:
      - Keywords
      - Leases
      - Keyword
    put:
      summary: Update a lease
      description: Updates a keyword lease. Turns the autoRenew on/off.
      operationId: updateKeywordLease
      x-api-path-slug: keywordsleaseskeyword-put
      parameters:
      - in: body
        name: body
        description: A keyword lease object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: keyword
        description: To update a keyword lease
      responses:
        200:
          description: OK
      tags:
      - Keywords
      - Leases
      - Keyword
  /keywords/{keyword}/available:
    get:
      summary: Check for a specific keyword
      description: Searches for the specific keyword to purchase on the CallFire platform.
        Returns 'true' if keyword is available.
      operationId: isKeywordAvailable
      x-api-path-slug: keywordskeywordavailable-get
      parameters:
      - in: path
        name: keyword
        description: To specify a keyword to search for
      responses:
        200:
          description: OK
      tags:
      - Keywords
      - Keyword
      - Available
  /me/account:
    get:
      summary: Find account details
      description: Searches for the user account details. Details include name, email,
        and basic account permissions
      operationId: getAccount
      x-api-path-slug: meaccount-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Account
  /me/api/credentials:
    get:
      summary: Find api credentials
      description: Searches for all credentials generated by user. Returns a paged
        list of the API credentials. Only ACCOUNT_HOLDER can invoke this API
      operationId: findApiCredentials
      x-api-path-slug: meapicredentials-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Me
      - Api
      - Credentials
    post:
      summary: Create api credentials
      description: Creates an API credentials for the CallFire API. This endpoint
        requires full CallFire account credentials to be used, authenticated using
        Basic Authentication. At the moment user provides only the name for the credentials.
        The generated credentials can be used to access any CallFire APIs
      operationId: createApiCredential
      x-api-path-slug: meapicredentials-post
      parameters:
      - in: body
        name: body
        description: To create the API credentials
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Me
      - Api
      - Credentials
  /me/api/credentials/{id}:
    delete:
      summary: Delete api credentials
      description: Deletes a specified API credential. Currently, removes the ability
        to access the API. Only ACCOUNT_HOLDER can invoke this API
      operationId: deleteApiCredential
      x-api-path-slug: meapicredentialsid-delete
      parameters:
      - in: path
        name: id
        description: An id of an API credential
      responses:
        200:
          description: OK
      tags:
      - Me
      - Api
      - Credentials
    get:
      summary: Find a specific api credential
      description: Returns an API credential instance for a given api credential id.
        Only ACCOUNT_HOLDER can invoke this API
      operationId: getApiCredential
      x-api-path-slug: meapicredentialsid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of an API credential
      responses:
        200:
          description: OK
      tags:
      - Me
      - Api
      - Credentials
  /me/billing/credit-usage:
    get:
      summary: Find credit usage
      description: Find credit usage for the user. Returns credits usage for time
        period specified or if unspecified then total for all time.
      operationId: getCreditUsage
      x-api-path-slug: mebillingcreditusage-get
      parameters:
      - in: query
        name: intervalBegin
        description: Beginning of usage period formatted in unix time milliseconds
      - in: query
        name: intervalEnd
        description: End of usage period formatted in unix time milliseconds
      responses:
        200:
          description: OK
      tags:
      - Me
      - Billing
      - Credit-usage
  /me/billing/plan-usage:
    get:
      summary: Find plan usage
      description: Searches for the data of a billing plan usage for the user. Returns
        the data of a billing plan usage for the current month
      operationId: getBillingPlanUsage
      x-api-path-slug: mebillingplanusage-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Billing
      - Plan-usage
  /me/callerids:
    get:
      summary: Find caller ids
      description: Returns a list of verified caller ids. If the number is not shown
        in the list, then it is not verified. In this case sending of a verification
        code is required.
      operationId: getCallerIds
      x-api-path-slug: mecallerids-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Callerids
  /me/callerids/{callerid}:
    post:
      summary: Create a caller id
      description: Generates and sends a verification code to the phone number provided
        in the path. The verification code is delivered via a phone call. This code
        needs to be submitted to the verify caller id API endpoint to complete verification.
      operationId: sendVerificationCodeToCallerId
      x-api-path-slug: mecalleridscallerid-post
      parameters:
      - in: path
        name: callerid
        description: A phone number in E
      responses:
        200:
          description: OK
      tags:
      - Me
      - Callerids
      - Callerid
  /me/callerids/{callerid}/verification-code:
    post:
      summary: Verify a caller id
      description: With the verification code received from the Create caller id endpoint,
        a call to this endpoint is required to finish verification
      operationId: verifyCallerId
      x-api-path-slug: mecalleridscalleridverificationcode-post
      parameters:
      - in: body
        name: body
        description: request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: callerid
        description: A phone number in E
      responses:
        200:
          description: OK
      tags:
      - Me
      - Callerids
      - Callerid
      - Verification-code
  /media:
    post:
      summary: Create media
      description: 'Uploads media file to account, acceptable media formats: bmp,
        gif, jpg, m4a, mp3, mp4, png, wav'
      operationId: createMedia
      x-api-path-slug: media-post
      parameters:
      - in: formData
        name: file
        description: Binary media file
      - in: formData
        name: name
        description: A name of a media file
      responses:
        200:
          description: OK
      tags:
      - Media
  /media/public/{key}.{extension}:
    get:
      summary: Download media by extension
      description: 'Download a media file. Available types of files: bmp, gif, jpg,
        m4a, mp3, mp4, png, wav. Content type in response depends on ''extension''
        parameter, e.g. image/jpeg, image/png, audio/mp3, etc'
      operationId: getMediaDataByKey
      x-api-path-slug: mediapublickey-extension-get
      parameters:
      - in: path
        name: extension
        description: 'Media file type, available types: bmp, gif, jpg, m4a, mp3, mp4,
          png, wav'
      - in: path
        name: key
        description: A hash-key of a media resource
      responses:
        200:
          description: OK
      tags:
      - Media
      - Public
      - Key.extension
  /media/{id}:
    get:
      summary: Get a specific media
      description: Get media resource by id
      operationId: getMedia
      x-api-path-slug: mediaid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a media resource
      responses:
        200:
          description: OK
      tags:
      - Media
  /media/{id}.{extension}:
    get:
      summary: Download media by extension
      description: 'Download a media file. Available types of files: bmp, gif, jpg,
        m4a, mp3, mp4, png, wav. Content type in response depends on ''extension''
        parameter, e.g. image/jpeg, image/png, audio/mp3, etc'
      operationId: getMediaData
      x-api-path-slug: mediaid-extension-get
      parameters:
      - in: path
        name: extension
        description: Media file type
      - in: path
        name: id
        description: An id of a media resource
      responses:
        200:
          description: OK
      tags:
      - Media
      - Extensions
  /media/{id}/file:
    get:
      summary: Download a MP3 media
      description: Download a MP3 media, endpoint returns application/binary content-type
      operationId: getMediaDataBinary
      x-api-path-slug: mediaidfile-get
      parameters:
      - in: path
        name: id
        description: An id of a media resource
      responses:
        200:
          description: OK
      tags:
      - Media
      - File
  /numbers/leases:
    get:
      summary: Find leases
      description: Searches for all numbers leased by account user. This API is useful
        for finding all numbers currently owned by the user. Returns a paged list
        of number leases.
      operationId: findNumberLeases
      x-api-path-slug: numbersleases-get
      parameters:
      - in: query
        name: city
        description: A city name
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: labelName
        description: A label name
      - in: query
        name: lata
        description: A local access and transport area (LATA)
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      - in: query
        name: prefix
        description: A 4-7 digit prefix
      - in: query
        name: rateCenter
        description: A rate center
      - in: query
        name: state
        description: A two-letter state code
      - in: query
        name: zipcode
        description: A five-digit Zipcode
      responses:
        200:
          description: OK
      tags:
      - Numbers
      - Leases
  /numbers/leases/configs:
    get:
      summary: Find lease configs
      description: Searches for all number lease configs for the user. Returns a paged
        list of NumberConfig
      operationId: findNumberLeaseConfigs
      x-api-path-slug: numbersleasesconfigs-get
      parameters:
      - in: query
        name: city
        description: A city name
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: labelName
        description: A label name
      - in: query
        name: lata
        description: A local access and transport area (LATA)
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      - in: query
        name: prefix
        description: A 4-7 digit prefix
      - in: query
        name: rateCenter
        description: A rate center
      - in: query
        name: state
        description: A two-letter state code
      - in: query
        name: zipcode
        description: A five-digit Zipcode
      responses:
        200:
          description: OK
      tags:
      - Numbers
      - Leases
      - Configs
  /numbers/leases/configs/{number}:
    get:
      summary: Find a specific lease config
      description: Returns a single NumberConfig instance for a given number lease
      operationId: getNumberLeaseConfig
      x-api-path-slug: numbersleasesconfigsnumber-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: number
        description: A phone number in E
      responses:
        200:
          description: OK
      tags:
      - Numbers
      - Leases
      - Configs
      - Number
    put:
      summary: Update a lease config
      description: Updates a phone number lease configuration. Use this API endpoint
        to add an Inbound IVR or Call Tracking feature to a CallFire phone number.
        Call tracking configuration allows you to track the incoming calls, to analyze
        and to respond customers using sms or voice replies. For more information
        see [call tracking page](https://www.callfire.com/products/call-tracking)
      operationId: updateNumberLeaseConfig
      x-api-path-slug: numbersleasesconfigsnumber-put
      parameters:
      - in: body
        name: body
        description: The configuration of a number lease object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: number
        description: A phone number in E
      responses:
        200:
          description: OK
      tags:
      - Numbers
      - Leases
      - Configs
      - Number
  /numbers/leases/{number}:
    get:
      summary: Find a specific lease
      description: Returns a single NumberLease instance for a given number
      operationId: getNumberLease
      x-api-path-slug: numbersleasesnumber-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: number
        description: A phone number in E
      responses:
        200:
          description: OK
      tags:
      - Numbers
      - Leases
      - Number
    put:
      summary: Update a lease
      description: Updates a number lease instance. Ability to turn on/off autoRenew
        and toggle call/text features for a particular number
      operationId: updateNumberLease
      x-api-path-slug: numbersleasesnumber-put
      parameters:
      - in: body
        name: body
        description: A NumberLease object to update
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: number
        description: A phone number in E
      responses:
        200:
          description: OK
      tags:
      - Numbers
      - Leases
      - Number
  /numbers/local:
    get:
      summary: Find local numbers
      description: Searches for numbers available for purchase in CallFire local numbers
        catalog . At least one additional parameter is required. User may filter local
        numbers by their region information.
      operationId: findNumbersLocal
      x-api-path-slug: numberslocal-get
      parameters:
      - in: query
        name: city
        description: A city name
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: lata
        description: A local access and transport area (LATA)
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: prefix
        description: A 4-7 digit prefix
      - in: query
        name: rateCenter
        description: A rate center
      - in: query
        name: state
        description: A two-letter state code
      - in: query
        name: zipcode
        description: A five-digit Zipcode
      responses:
        200:
          description: OK
      tags:
      - Numbers
      - Local
  /numbers/regions:
    get:
      summary: Find number regions
      description: Searches for region information. Use this API to obtain detailed
        region information that can be used to query for more specific phone numbers
        than a general query.
      operationId: findNumberRegions
      x-api-path-slug: numbersregions-get
      parameters:
      - in: query
        name: city
        description: A city name
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: lata
        description: A local access and transport area (LATA)
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      - in: query
        name: prefix
        description: A 4-7 digit prefix
      - in: query
        name: rateCenter
        description: A rate center
      - in: query
        name: state
        description: A two-letter state code
      - in: query
        name: zipcode
        description: A five-digit Zipcode
      responses:
        200:
          description: OK
      tags:
      - Numbers
      - Regions
  /numbers/tollfree:
    get:
      summary: Find tollfree numbers
      description: Searches for the toll free numbers which are available for purchase
        in the CallFire catalog
      operationId: findNumbersTollfree
      x-api-path-slug: numberstollfree-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: pattern
        description: Filter toll free numbers by prefix, pattern must be 3 char long
          and should end with *
      responses:
        200:
          description: OK
      tags:
      - Numbers
      - Tollfree
  /orders/keywords:
    post:
      summary: Purchase keywords
      description: Purchase keywords. Send a list of available keywords into this
        API to purchase them using CallFire credits. Make sure the account has enough
        credits before trying to purchase the keywords
      operationId: orderKeywords
      x-api-path-slug: orderskeywords-post
      parameters:
      - in: body
        name: body
        description: Request object which contains a list of keywords to buy
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Keywords
  /orders/numbers:
    post:
      summary: Purchase numbers
      description: Purchase numbers. There are many ways to purchase a number. Set
        either 'tollFreeCount' or 'localCount' along with some querying fields to
        purchase numbers by bulk query. Set the list of numbers to purchase by list.
        Available numbers will be purchased using CallFire credits owned by the user.
        Make sure the account has enough credits before trying to purchase
      operationId: orderNumbers
      x-api-path-slug: ordersnumbers-post
      parameters:
      - in: body
        name: body
        description: 'Request object contains a list of numbers to buy, you can filter
          the numbers by their region information: city, state, zipcode, LATA, etc'
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Numbers
  /orders/{id}:
    get:
      summary: Find a specific order
      description: Returns a single NumberOrder instance for a given order id. Order
        contains information about purchased keywords, local, toll-free numbers
      operationId: getOrder
      x-api-path-slug: ordersid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of an order
      responses:
        200:
          description: OK
      tags:
      - Orders
  /texts:
    get:
      summary: Find texts
      description: Searches for texts sent or received by user. Use "campaignId=0"
        parameter to query for all texts sent through the POST /texts API. See [call
        states and results](https://developers.callfire.com/results-responses-errors.html)
      operationId: findTexts
      x-api-path-slug: texts-get
      parameters:
      - in: query
        name: batchId
        description: An Id of a contact batch, queries for texts which are used in
          the particular contact batch
      - in: query
        name: campaignId
        description: An id of a campaign, queries for texts inside a particular campaign
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: fromNumber
        description: A phone number in E
      - in: query
        name: id
        description: List of Text ids to search for, if ids specified other query
          params ignored
      - in: query
        name: inbound
        description: Specify true for inbound or false for outbounds
      - in: query
        name: intervalBegin
        description: Start of the find time interval, formatted in unix time milliseconds
      - in: query
        name: intervalEnd
        description: End of the find time interval, formatted in unix time milliseconds
      - in: query
        name: label
        description: A label of a text message
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      - in: query
        name: results
        description: 'Expected text results in comma separated string, available values:
          SENT, RECEIVED, DNT, TOO_BIG, INTERNAL_ERROR, CARRIER_ERROR, CARRIER_TEMP_ERROR,
          UNDIALED'
      - in: query
        name: states
        description: 'Expected text statuses in comma separated string, available
          values: READY, SELECTED, CALLBACK, FINISHED, DISABLED, DNC, DUP, INVALID,
          TIMEOUT, PERIOD_LIMIT'
      - in: query
        name: toNumber
        description: A phone number in E
      responses:
        200:
          description: OK
      tags:
      - Texts
    post:
      summary: Send texts
      description: Use the /texts API to send individual texts quickly. By default
        all texts are going out from CallFire's dedicated short code 67076
      operationId: sendTexts
      x-api-path-slug: texts-post
      parameters:
      - in: body
        name: body
        description: List of TextRecipient objects
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: campaignId
        description: Specifies a campaignId to send texts through a previously created
          campaign
      - in: query
        name: defaultMessage
        description: Text message can be overridden by TextRecipient
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Texts
  /texts/auto-replys:
    get:
      summary: Find auto replies
      description: Find all text autoreplies created by user. Returns a paged list
        of TextAutoReply
      operationId: findTextAutoReplys
      x-api-path-slug: textsautoreplys-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: number
        description: Phone number in E
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Auto-replys
    post:
      summary: Create an auto reply
      description: CallFire gives you possibility to set up auto reply messages for
        your numbers and keywords. You can set a general auto reply for anyone who
        texts your number, keyword, and/or include a text to match, so that the auto
        reply would be sent only to those who text the matched text
      operationId: createTextAutoReply
      x-api-path-slug: textsautoreplys-post
      parameters:
      - in: body
        name: body
        description: TextAutoReply object, keyword or number should be specified with
          response message and text to match if needed
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Auto-replys
  /texts/auto-replys/{id}:
    delete:
      summary: Delete an auto reply
      description: Deletes a text auto reply and removes the configuration. Can not
        delete a TextAutoReply which is currently active for a campaign
      operationId: deleteTextAutoReply
      x-api-path-slug: textsautoreplysid-delete
      parameters:
      - in: path
        name: id
        description: An id of a text auto reply
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Auto-replys
    get:
      summary: Find a specific auto reply
      description: Returns a single TextAutoReply instance for a given text auto reply
        id
      operationId: getTextAutoReply
      x-api-path-slug: textsautoreplysid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a text auto reply
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Auto-replys
  /texts/broadcasts:
    get:
      summary: Find text broadcasts
      description: Searches for all text broadcasts created by user. Can query on
        label, name, and the current running status of the campaign. Returns a paged
        list of text broadcasts
      operationId: findTextBroadcasts
      x-api-path-slug: textsbroadcasts-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: label
        description: A label of a text broadcast
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: name
        description: A name of text broadcast
      - in: query
        name: offset
        description: Offset to the start of a given page
      - in: query
        name: running
        description: Returns broadcasts only in running state
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
    post:
      summary: Create a text broadcast
      description: Creates a text broadcast campaign using the Text Broadcast API.
        Send a TextBroadcast object in the message body to detail a text broadcast
        campaign. A campaign can be created without contacts and with bare minimum
        configuration, but contacts have to be added further on to use the campaign.
        It supports scheduling, retry logic, pattern-based messages.
      operationId: createTextBroadcast
      x-api-path-slug: textsbroadcasts-post
      parameters:
      - in: body
        name: body
        description: A TextBroadcast object
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: start
        description: If true then starts the campaign immediately (not required)
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
  /texts/broadcasts/{id}:
    get:
      summary: Find a specific text broadcast
      description: Returns a single TextBroadcast instance for a given text broadcast
        id
      operationId: getTextBroadcast
      x-api-path-slug: textsbroadcastsid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a text broadcast
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
    put:
      summary: Update a text broadcast
      description: Allows modifying the configuration of existing text broadcast campaign.
        See TextBroadcast for more information on what can/can't be updated on this
        API
      operationId: updateTextBroadcast
      x-api-path-slug: textsbroadcastsid-put
      parameters:
      - in: body
        name: body
        description: A TextBroadcast object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: An id of a text broadcast
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
  /texts/broadcasts/{id}/archive:
    post:
      summary: Archive text broadcast
      description: Archives a text broadcast (and hides it in the search results)
      operationId: archiveTextBroadcast
      x-api-path-slug: textsbroadcastsidarchive-post
      parameters:
      - in: path
        name: id
        description: An id of a text broadcast to archive
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
      - Archive
  /texts/broadcasts/{id}/batches:
    get:
      summary: Find batches in a text broadcast
      description: This endpoint will enable the user to page through all of the batches
        for a particular text broadcast campaign
      operationId: getTextBroadcastBatches
      x-api-path-slug: textsbroadcastsidbatches-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a text broadcast
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
      - Batches
    post:
      summary: Add batches to a text broadcast
      description: Allows adding an extra batches to an already created text broadcast
        campaign. The batches which being  added pass the CallFire validation process
        (unlike in the recipients version of this API). That is why using of a scrubDuplicates
        flag remove duplicates from your batch. Batches may be added as a contact
        list id, a list of contact ids, or a list of numbers
      operationId: addTextBroadcastBatch
      x-api-path-slug: textsbroadcastsidbatches-post
      parameters:
      - in: body
        name: body
        description: A request object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: An id of a text broadcast
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
      - Batches
  /texts/broadcasts/{id}/recipients:
    post:
      summary: Add recipients to a text broadcast
      description: Use this API to add recipients to a text broadcast which is already
        created. Post a list of Recipient objects to be immediately added to the text
        broadcast campaign. These contacts will not go through validation process,
        and will be acted upon as they are added. Recipients may be added as a list
        of contact ids, or list of numbers
      operationId: addTextBroadcastRecipients
      x-api-path-slug: textsbroadcastsidrecipients-post
      parameters:
      - in: body
        name: body
        description: A list of the TextRecipient objects
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a text broadcast
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
      - Recipients
  /texts/broadcasts/{id}/start:
    post:
      summary: Start text broadcast
      description: Starts a text broadcast
      operationId: startTextBroadcast
      x-api-path-slug: textsbroadcastsidstart-post
      parameters:
      - in: path
        name: id
        description: An id of a text broadcast to start
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
      - Start
  /texts/broadcasts/{id}/stats:
    get:
      summary: Get statistics on text broadcast
      description: 'Returns the broadcast statistics. Example: total number of the
        sent/received actions, total cost, number of remaining outbound actions, error
        count, etc'
      operationId: getTextBroadcastStats
      x-api-path-slug: textsbroadcastsidstats-get
      parameters:
      - in: query
        name: begin
        description: Start of a search find time interval, formatted in unix time
          milliseconds
      - in: query
        name: end
        description: End of a search time interval, formatted in unix time milliseconds
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a text broadcast
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
      - Stats
  /texts/broadcasts/{id}/stop:
    post:
      summary: Stop text broadcast
      description: Stops a text broadcast
      operationId: stopTextBroadcast
      x-api-path-slug: textsbroadcastsidstop-post
      parameters:
      - in: path
        name: id
        description: An Id of a text broadcast
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
      - Stop
  /texts/broadcasts/{id}/texts:
    get:
      summary: Find texts in a text broadcast
      description: This endpoint will enable the user to page through all of the texts
        for a particular text broadcast campaign
      operationId: getTextBroadcastTexts
      x-api-path-slug: textsbroadcastsidtexts-get
      parameters:
      - in: query
        name: batchId
        description: "~"
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a text broadcast
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
      - Texts
  /texts/{id}:
    get:
      summary: Find a specific text
      description: Returns a single Text instance for a given text id
      operationId: getText
      x-api-path-slug: textsid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a text
      responses:
        200:
          description: OK
      tags:
      - Texts
  /webhooks:
    get:
      summary: Find webhooks
      description: Searches all webhooks available for a current user. Searches by
        name, resource, event, callback URL, or whether they are enabled. Returns
        a paged list of Webhooks
      operationId: findWebhooks
      x-api-path-slug: webhooks-get
      parameters:
      - in: query
        name: callback
        description: A callback URL
      - in: query
        name: enabled
        description: Specifies whether webhook is enabled
      - in: query
        name: event
        description: 'A name of event, available values: started, stopped, finished'
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: name
        description: A name of a webhook
      - in: query
        name: offset
        description: Offset to the start of a given page
      - in: query
        name: resource
        description: 'A name of a resource, available values: CccCampaign, CallBroadcast,
          TextBroadcast,  OutboundCall, OutboundText, InboundCall, InboundText, ContactList'
      responses:
        200:
          description: OK
      tags:
      - Webhooks
    post:
      summary: Create a webhook
      description: 'Create a Webhook for notification in the CallFire system. Use
        the webhooks API to receive notifications of important CallFire events. Select
        the resource to listen to, and then choose the resource events to receive
        notifications on. When an event triggers, a POST will be made to the callback
        URL with a payload of notification information. Available resources and their
        events include ''CccCampaign'': [''started'', ''stopped'', ''finished''],
        ''CallBroadcast'': [''started'', ''stopped'', ''finished''], ''TextBroadcast'':
        [''started'', ''stopped'', ''finished''], ''OutboundCall'': [''finished''],
        ''InboundCall'': [''finished''], ''OutboundText'': [''finished''], ''InboundText'':
        [''finished''], ''ContactList'': [''validationFinished'', ''validationFailed''].
        Webhooks support secret token which is used as signing key to HmacSHA1 hash
        of json payload which is returned in ''X-CallFire-Signature'' header. This
        header can be used to verify callback POST is coming from CallFire. See [security
        guide](https://developers.callfire.com/security-guide.html)'
      operationId: createWebhook
      x-api-path-slug: webhooks-post
      parameters:
      - in: body
        name: body
        description: A webhook object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Webhooks
  /webhooks/resources:
    get:
      summary: Find webhook resources
      description: 'Searches for webhook resources. Available resources include ''CccCampaign'':
        [''started'', ''stopped'', ''finished''], ''CallBroadcast'': [''started'',
        ''stopped'', ''finished''], ''TextBroadcast'': [''started'', ''stopped'',
        ''finished''], ''OutboundCall'': [''finished''], ''InboundCall'': [''finished''],
        ''OutboundText'': [''finished''], ''InboundText'': [''finished''], ''ContactList'':
        [''validationFinished'', ''validationFailed'']'
      operationId: findWebhookResources
      x-api-path-slug: webhooksresources-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - Resources
  /webhooks/resources/{resource}:
    get:
      summary: Find specific webhook resource
      description: Returns information about supported events for a given webhook
        resource
      operationId: getWebhookResource
      x-api-path-slug: webhooksresourcesresource-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: resource
        description: A name of a webhook resource
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - Resources
      - Resource
  /webhooks/{id}:
    delete:
      summary: Delete a webhook
      description: Deletes a webhook instance. Will be removed permanently
      operationId: deleteWebhook
      x-api-path-slug: webhooksid-delete
      parameters:
      - in: path
        name: id
        description: An Id of a webhook
      responses:
        200:
          description: OK
      tags:
      - Webhooks
    get:
      summary: Find a specific webhook
      description: Returns a single Webhook instance for a given webhook id
      operationId: getWebhook
      x-api-path-slug: webhooksid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a webhook
      responses:
        200:
          description: OK
      tags:
      - Webhooks
    put:
      summary: Update a webhook
      description: Updates the information in existing webhook
      operationId: updateWebhook
      x-api-path-slug: webhooksid-put
      parameters:
      - in: body
        name: body
        description: A webhook object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: An id of a webhook
      responses:
        200:
          description: OK
      tags:
      - Webhooks