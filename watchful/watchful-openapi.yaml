swagger: "2.0"
x-collection-name: Watchful
x-complete: 1
info:
  title: Watchful
  description: watchful-resulted-from-the-need-for-a-single-unified-dashboard-to-easily-monitor-all-of-the-web-sites-in-our-portfolios--after-years-of-evolution-our-solution-has-matured-into-a-simple-complete-and-professional-service--
  version: 1.0.0
host: watchful.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /audits:
    get:
      summary: Get A List Of Audits
      description: Returns a list of audits
      operationId: getAudits
      x-api-path-slug: audits-get
      parameters:
      - in: query
        name: limit
        description: Number of object to return (max 100, default 25)
      - in: query
        name: limitstart
        description: Start of the return (default 0)
      - in: query
        name: order
        description: ORDER by this field separete by comas
      responses:
        200:
          description: OK
      tags:
      - Audits
    post:
      summary: Create A Audit
      description: Create a audit.
      operationId: CreateAudits
      x-api-path-slug: audits-post
      parameters:
      - in: body
        name: body
        description: JSON object Audit
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Audits
  /audits/metadata:
    get:
      summary: Get The List Of Fields
      description: Returns a list of fields
      operationId: getFieldsAudits
      x-api-path-slug: auditsmetadata-get
      responses:
        200:
          description: OK
      tags:
      - Audits
      - Metadata
  /audits/{id}:
    delete:
      summary: Delete A Specific Audit
      description: Delete a specific audit.
      operationId: deleteAuditById
      x-api-path-slug: auditsid-delete
      parameters:
      - in: path
        name: id
        description: ID of audit that needs to be deleted
      responses:
        200:
          description: OK
      tags:
      - Audits
      - Id
    get:
      summary: Find Audit By ID
      description: Returns a audit based on ID
      operationId: getAuditById
      x-api-path-slug: auditsid-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: path
        name: id
        description: ID of audit that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Audits
      - Id
  /extensions:
    get:
      summary: Get A List Extensions
      description: Returns a list Extensions
      operationId: getExtensions
      x-api-path-slug: extensions-get
      parameters:
      - in: query
        name: ext_name
        description: Do a LIKE search, you can also use %
      - in: query
        name: ext_prefix
        description: Do a LIKE search, you can also use %
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: query
        name: limit
        description: Number of object to return (max 100, default 25)
      - in: query
        name: limitstart
        description: Start of the return (default 0)
      - in: query
        name: order
        description: ORDER by this field separete by comas
      - in: query
        name: siteids
        description: List of sites id separated by comma
      - in: query
        name: version
        description: Do a LIKE search, you can also use %
      - in: query
        name: vUpdate
        description: update available for this extension
      responses:
        200:
          description: OK
      tags:
      - Extensions
  /extensions/metadata:
    get:
      summary: Get The List Of Fields
      description: Returns a list of fields
      operationId: getFieldsExtensions
      x-api-path-slug: extensionsmetadata-get
      responses:
        200:
          description: OK
      tags:
      - Extensions
      - Metadata
  /extensions/{id}/ignore:
    post:
      summary: Set 'ignore Updates' For A Given Extension / Site_id
      description: Set 'ignore updates' for a given extension / site_id
      operationId: ignoreExtensionUpdate
      x-api-path-slug: extensionsidignore-post
      parameters:
      - in: path
        name: id
        description: ID of the extension
      responses:
        200:
          description: OK
      tags:
      - Extensions
      - Id
      - Ignore
  /extensions/{id}/unignore:
    post:
      summary: Remove 'ignore Updates' For A Given Extension
      description: Remove 'ignore updates' for a given extension
      operationId: unignoreExtensionUpdate
      x-api-path-slug: extensionsidunignore-post
      parameters:
      - in: path
        name: id
        description: ID of the extension
      responses:
        200:
          description: OK
      tags:
      - Extensions
      - Id
      - Unignore
  /extensions/{id}/update:
    post:
      summary: Update The Extension On The Remote Site
      description: Update the extension on the remote site
      operationId: updateExtension
      x-api-path-slug: extensionsidupdate-post
      parameters:
      - in: path
        name: id
        description: ID of the extension
      responses:
        200:
          description: OK
      tags:
      - Extensions
      - Id
      - Update
  /feedbacks:
    get:
      summary: Get Feedbacks
      description: Returns a list of feedbacks
      operationId: getFeedbacks
      x-api-path-slug: feedbacks-get
      parameters:
      - in: query
        name: fields
        description: Fields to return separate by comas (es
      responses:
        200:
          description: OK
      tags:
      - Feedbacks
    post:
      summary: Create A Feedback
      description: Create a feedback
      operationId: createFeedbacks
      x-api-path-slug: feedbacks-post
      parameters:
      - in: body
        name: body
        description: JSON object Feedback
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Feedbacks
  /feedbacks/metadata:
    get:
      summary: Get The List Of Fields
      description: Returns a list of fields
      operationId: getFieldsFeedbacks
      x-api-path-slug: feedbacksmetadata-get
      responses:
        200:
          description: OK
      tags:
      - Feedbacks
      - Metadata
  /logs:
    get:
      summary: Get A List Of Logs
      description: Returns a list of logs
      operationId: logs.get
      x-api-path-slug: logs-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: query
        name: from
        description: Logs after this date, format YYYY-MM-DD HH:MM:SS
      - in: query
        name: limit
        description: Number of object to return (max 100, default 25)
      - in: query
        name: limitstart
        description: Start of the return (default 0)
      - in: query
        name: log_entry
        description: Do a LIKE search, you can also use %
      - in: query
        name: log_type
        description: Type of the log
      - in: query
        name: order
        description: ORDER by this field separete by comas
      - in: query
        name: to
        description: Logs before this date, format YYYY-MM-DD HH:MM:SS
      responses:
        200:
          description: OK
      tags:
      - Logs
  /logs/export:
    get:
      summary: Get A CSV Or PDF File Contain The List Of Logs
      description: Returns a file contain the list of logs
      operationId: getExportLogs
      x-api-path-slug: logsexport-get
      parameters:
      - in: query
        name: enddate
        description: Logs before this date, format YYYY-MM-DD HH:MM:SS
      - in: query
        name: filter_type
        description: Type of the log
      - in: query
        name: format
        description: Format of exported file (PDF or CSV)
      - in: query
        name: limit
        description: Number of object to return (max 100, default 25)
      - in: query
        name: search
        description: Do a LIKE search, you can also use %
      - in: query
        name: site
        description: Site id of the log
      - in: query
        name: startdate
        description: Logs after this date, format YYYY-MM-DD HH:MM:SS
      - in: query
        name: startid
        description: Start of the return (default 0)
      responses:
        200:
          description: OK
      tags:
      - Logs
      - Export
  /logs/metadata:
    get:
      summary: Get The List Of Fields
      description: Returns a list of fields
      operationId: getFieldsLogs
      x-api-path-slug: logsmetadata-get
      responses:
        200:
          description: OK
      tags:
      - Logs
      - Metadata
  /logs/types:
    get:
      summary: Get The List Of Log Types
      description: Returns a list of log types
      operationId: getTypesLogs
      x-api-path-slug: logstypes-get
      responses:
        200:
          description: OK
      tags:
      - Logs
      - Types
  /logs/{id}:
    delete:
      summary: Delete A Specific Log
      description: Delete a specific log
      operationId: deleteLogById
      x-api-path-slug: logsid-delete
      parameters:
      - in: path
        name: id
        description: ID of log that needs to be deleted
      responses:
        200:
          description: OK
      tags:
      - Logs
      - Id
  /packages:
    post:
      summary: ""
      description: ""
      operationId: packages.post
      x-api-path-slug: packages-post
      parameters:
      - in: formData
        name: file
        description: ZIP package
      responses:
        200:
          description: OK
      tags:
      - Packages
  /reports/sites/{id}:
    get:
      summary: Returns A PDF Report For A Specific Site
      description: Returns a PDF report based on a site ID
      operationId: reports.sites.id.get
      x-api-path-slug: reportssitesid-get
      parameters:
      - in: query
        name: compare
        description: Define if you want show previous values in Google Analytics graph
      - in: query
        name: from
        description: Start of the report, format YYYY-MM-DD, default today-30day
      - in: path
        name: id
        description: ID that needs to be fetched
      - in: query
        name: log_type
        description: Type of the log to show in the report
      - in: query
        name: reports
        description: 'Type of reports separate by comas: Ga,Logs,Uptime'
      - in: query
        name: to
        description: End of the report, format YYYY-MM-DD, default today
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Sites
      - Id
  /reports/tags/{id}:
    get:
      summary: Find Sites By ID
      description: Returns a report based on a site ID
      operationId: reports.tags.id.get
      x-api-path-slug: reportstagsid-get
      parameters:
      - in: query
        name: compare
        description: Define if you want show previous values in Google Analytics graph
      - in: query
        name: from
        description: Start of the report, format YYYY-MM-DD, default today-30day
      - in: path
        name: id
        description: ID that needs to be fetched
      - in: query
        name: log_type
        description: Type of the log to show in the report
      - in: query
        name: reports
        description: 'Type of reports separate by comas: Ga,Logs,Uptime'
      - in: query
        name: to
        description: End of the report, format YYYY-MM-DD, default today
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Tags
      - Id
  /sites:
    get:
      summary: Get A List Of Sites
      description: Returns a list of Sites
      operationId: getSites
      x-api-path-slug: sites-get
      parameters:
      - in: query
        name: access_url
        description: Access URL
      - in: query
        name: canUpdate
        description: canUpdate
      - in: query
        name: error
        description: Has errors
      - in: query
        name: fields
        description: Fields to return separated by commas (e
      - in: query
        name: ip
        description: Ip address
      - in: query
        name: jUpdate
        description: 'Joomla core update status (1: update required, 0: update not
          required)'
      - in: query
        name: j_version
        description: Joomla version
      - in: query
        name: limit
        description: Number of objects to return (max 100, default 25)
      - in: query
        name: limitstart
        description: Start of the return (default 0)
      - in: query
        name: name
        description: Site name
      - in: query
        name: nbUpdates
      - in: query
        name: order
        description: ORDER by this field separete by comas
      - in: query
        name: published
        description: Is published
      - in: query
        name: siteids
        description: List of sites id separated by comma
      - in: query
        name: up
        description: Is online
      responses:
        200:
          description: OK
      tags:
      - Sites
    post:
      summary: Create A Site
      description: Create a site
      operationId: createSite
      x-api-path-slug: sites-post
      parameters:
      - in: body
        name: body
        description: JSON object Site
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sites
  /sites/metadata:
    get:
      summary: Get The List Of Fields
      description: Returns a list of fields
      operationId: sites.metadata.get
      x-api-path-slug: sitesmetadata-get
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Metadata
  /sites/{id}:
    delete:
      summary: Delete A Specific Site
      description: Delete a specific Site
      operationId: sites.id.delete
      x-api-path-slug: sitesid-delete
      parameters:
      - in: path
        name: id
        description: ID of Site that needs to be deleted
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
    get:
      summary: Find Sites By ID
      description: Return a site based on ID
      operationId: getSiteById
      x-api-path-slug: sitesid-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: path
        name: id
        description: ID that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
    put:
      summary: Update A Site
      description: Update a site
      operationId: sites.id.put
      x-api-path-slug: sitesid-put
      parameters:
      - in: body
        name: body
        description: JSON object Site
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of the website that needs to be update
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
  /sites/{id}/audits:
    get:
      summary: Return Audits For A Specific Website
      description: Return audits for a specific website
      operationId: getSiteAudits
      x-api-path-slug: sitesidaudits-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: path
        name: id
        description: ID of the website
      - in: query
        name: limit
        description: Number of object to return (max 100, default 25)
      - in: query
        name: limitstart
        description: Start of the return (default 0)
      - in: query
        name: order
        description: ORDER by this field
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Audits
    post:
      summary: Create An Audit For The Site
      description: Create an audit for the site
      operationId: createAudits
      x-api-path-slug: sitesidaudits-post
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Audits
  /sites/{id}/backupnow:
    post:
      summary: Add The Site To The Backup Queue
      description: Add the site to the backup queue
      operationId: addSiteToBackupQueue
      x-api-path-slug: sitesidbackupnow-post
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Backupnow
  /sites/{id}/backupprofiles:
    get:
      summary: Return Backup Profile
      description: Return backup profile
      operationId: getBackupProfiles
      x-api-path-slug: sitesidbackupprofiles-get
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Backupprofiles
  /sites/{id}/backups:
    get:
      summary: List Of Latest Backups
      description: List of latest backups
      operationId: getListBackups
      x-api-path-slug: sitesidbackups-get
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Backups
  /sites/{id}/backupstart:
    post:
      summary: Start A Remote Backup For The Site
      description: Start a remote backup for the site
      operationId: startSiteBackup
      x-api-path-slug: sitesidbackupstart-post
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Backupstart
  /sites/{id}/backupstep:
    post:
      summary: Step (continue) A Remote Backup For The Site
      description: Step (continue) a remote backup for the site
      operationId: stepSiteBackup
      x-api-path-slug: sitesidbackupstep-post
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Backupstep
  /sites/{id}/extensions:
    get:
      summary: Get Extensions For A Site
      description: Get extensions for a site
      operationId: sites.id.extensions.get
      x-api-path-slug: sitesidextensions-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: path
        name: id
        description: ID of the website
      - in: query
        name: limit
        description: Number of object to return (max 100, default 25)
      - in: query
        name: limitstart
        description: Start of the return (default 0)
      - in: query
        name: order
        description: ORDER by this field
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Extensions
    post:
      summary: Install Extension
      description: ""
      operationId: installExtension
      x-api-path-slug: sitesidextensions-post
      parameters:
      - in: path
        name: id
        description: ID of the website
      - in: query
        name: url
        description: URL to install the extension from
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Extensions
  /sites/{id}/logs:
    get:
      summary: Return Logs For A Specific Website
      description: Return logs for a specific website
      operationId: sites.id.logs.get
      x-api-path-slug: sitesidlogs-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: query
        name: from
        description: Logs after this date, format YYYY-MM-DD HH:MM:SS
      - in: path
        name: id
        description: ID of the website
      - in: query
        name: limit
        description: Number of object to return (max 100, default 25)
      - in: query
        name: limitstart
        description: Start of the return (default 0)
      - in: query
        name: log_entry
        description: Do a LIKE search, you can also use %
      - in: query
        name: log_type
        description: Type of the log
      - in: query
        name: order
        description: ORDER by this field separete by comas
      - in: query
        name: to
        description: Logs before this date, format YYYY-MM-DD HH:MM:SS
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Logs
    post:
      summary: Create A Custom Log For A Specific Website
      description: Create a custom log for a specific website
      operationId: CreateLog
      x-api-path-slug: sitesidlogs-post
      parameters:
      - in: body
        name: body
        description: JSON object Log (only type custom)
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Logs
  /sites/{id}/monitor:
    delete:
      summary: Delete Uptime Monitor
      description: Return boolean
      operationId: deleteMonitor
      x-api-path-slug: sitesidmonitor-delete
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Monitor
    post:
      summary: Post Uptime Monitor
      description: Return boolean
      operationId: postMonitor
      x-api-path-slug: sitesidmonitor-post
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Monitor
  /sites/{id}/scanner:
    get:
      summary: Scan The Site For Malware
      description: Scan the site for malware
      operationId: scanner
      x-api-path-slug: sitesidscanner-get
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Scanner
  /sites/{id}/seo:
    get:
      summary: SEO Analyze For A Page
      description: SEO analyze for a page
      operationId: seoAnalyze
      x-api-path-slug: sitesidseo-get
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Seo
  /sites/{id}/tags:
    get:
      summary: Return Tags For A Specific Website
      description: Return tags for a specific website
      operationId: sites.id.tags.get
      x-api-path-slug: sitesidtags-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: path
        name: id
        description: ID of the website
      - in: query
        name: limit
        description: Number of object to return (max 100, default 25)
      - in: query
        name: limitstart
        description: Start of the return (default 0)
      - in: query
        name: name
        description: Do a LIKE search, you can also use %
      - in: query
        name: order
        description: ORDER by this field
      - in: query
        name: type
        description: Bootstrap color of the tag
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Tags
    post:
      summary: Add Tags For A Specific Website
      description: Add tags for a specific website
      operationId: postTags
      x-api-path-slug: sitesidtags-post
      parameters:
      - in: body
        name: body
        description: JSON object Tag
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Tags
  /sites/{id}/updatejoomla:
    post:
      summary: Update Joomla Core On The Remote Site
      description: Update Joomla core on the remote site
      operationId: updateJoomla
      x-api-path-slug: sitesidupdatejoomla-post
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Updatejoomla
  /sites/{id}/uptime:
    get:
      summary: Return Uptime Data
      description: Return uptime data
      operationId: getUptime
      x-api-path-slug: sitesiduptime-get
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Uptime
  /sites/{id}/validate:
    get:
      summary: Validate The Site, Return The New Logs
      description: validate the site
      operationId: validateSite
      x-api-path-slug: sitesidvalidate-get
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Validate
  /sites/{id}/validatedebug:
    get:
      summary: Validate The Site, Return The Debug Information
      description: ""
      operationId: validateDebugSite
      x-api-path-slug: sitesidvalidatedebug-get
      parameters:
      - in: path
        name: id
        description: ID of the website
      responses:
        200:
          description: OK
      tags:
      - Sites
      - Id
      - Validatedebug
  /ssousers:
    get:
      summary: Get A List Of SSO Users
      description: Returns a list of SSO Users
      operationId: getSsoUsers
      x-api-path-slug: ssousers-get
      responses:
        200:
          description: OK
      tags:
      - Ssousers
    post:
      summary: Create A SSO User
      description: Create a SSO User
      operationId: CreateSsoUsers
      x-api-path-slug: ssousers-post
      parameters:
      - in: body
        name: body
        description: JSON object SsoUsers
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Ssousers
  /ssousers/{id}:
    delete:
      summary: Delete A Specific SSO User
      description: Delete a specific SSO User
      operationId: deleteSsoUserById
      x-api-path-slug: ssousersid-delete
      parameters:
      - in: path
        name: id
        description: ID of SSO User that needs to be deleted
      responses:
        200:
          description: OK
      tags:
      - Ssousers
      - Id
    get:
      summary: Find SSO User By ID
      description: Returns a SSO User based on ID
      operationId: getSsoUsersById
      x-api-path-slug: ssousersid-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: path
        name: id
        description: ID of SSO User that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Ssousers
      - Id
    put:
      summary: Update A SSO User
      description: Update a SSO User
      operationId: UpdateSsoUsers
      x-api-path-slug: ssousersid-put
      parameters:
      - in: body
        name: body
        description: JSON object SsoUsers
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of SSO User that needs to be updated
      responses:
        200:
          description: OK
      tags:
      - Ssousers
      - Id
  /tags:
    get:
      summary: Get A List Of Tags
      description: Returns a list of tags
      operationId: tags.get
      x-api-path-slug: tags-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: query
        name: limit
        description: Number of object to return (max 100, default 25)
      - in: query
        name: limitstart
        description: Start of the return (default 0)
      - in: query
        name: name
        description: Do a LIKE search, you can also use %
      - in: query
        name: order
        description: ORDER by this field separete by comas
      - in: query
        name: type
        description: Bootstrap color of the tag
      responses:
        200:
          description: OK
      tags:
      - Tags
    post:
      summary: Create A Tag
      description: Create a tag
      operationId: CreateTags
      x-api-path-slug: tags-post
      parameters:
      - in: body
        name: body
        description: JSON object Tag
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/metadata:
    get:
      summary: Get The List Of Fields
      description: Returns a list of fields
      operationId: tags.metadata.get
      x-api-path-slug: tagsmetadata-get
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Metadata
  /tags/{id}:
    delete:
      summary: Delete A Specific Tag
      description: Delete a specific tag
      operationId: tags.id.delete
      x-api-path-slug: tagsid-delete
      parameters:
      - in: path
        name: id
        description: ID of tag that needs to be deleted
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Id
    get:
      summary: Find Tag By ID
      description: Returns a tag based on ID
      operationId: getTagById
      x-api-path-slug: tagsid-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: path
        name: id
        description: ID of tag that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Id
    put:
      summary: Update A Tag
      description: Update a tag
      operationId: UpdateTag
      x-api-path-slug: tagsid-put
      parameters:
      - in: body
        name: body
        description: JSON object of the updated tag
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Id
  /tags/{id}/sites:
    get:
      summary: Find Sites By Tag ID
      description: Returns a list of sites based with a specific tag id
      operationId: getSitesByTags
      x-api-path-slug: tagsidsites-get
      parameters:
      - in: query
        name: access_url
        description: Do a LIKE search, you can also use %
      - in: query
        name: error
        description: have errors
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      - in: path
        name: id
        description: ID of tag that needs to be fetched
      - in: query
        name: ip
        description: Do a LIKE search, you can also use %
      - in: query
        name: jUpdate
        description: Joomla core update
      - in: query
        name: j_version
        description: Do a LIKE search, you can also use %
      - in: query
        name: limit
        description: Number of object to return (max 100, default 25)
      - in: query
        name: limitstart
        description: Start of the return (default 0)
      - in: query
        name: name
        description: Do a LIKE search, you can also use %
      - in: query
        name: nbUpdates
      - in: query
        name: order
        description: ORDER by this field separete by comas
      - in: query
        name: published
        description: is published
      - in: query
        name: up
        description: is the website online
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Id
      - Sites
  /versions:
    get:
      summary: Get List Of Versions
      description: ""
      operationId: getVersions
      x-api-path-slug: versions-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by comas: name,id'
      responses:
        200:
          description: OK
      tags:
      - Versions
  /versions/{id}:
    get:
      summary: Find A Version By ID
      description: ""
      operationId: getVersion
      x-api-path-slug: versionsid-get
      parameters:
      - in: query
        name: fields
        description: 'Fields to return separate by commas: name,id'
      - in: path
        name: id
        description: ID of version that needs to be fetched
      responses:
        200:
          description: OK
      tags:
      - Versions
      - Id