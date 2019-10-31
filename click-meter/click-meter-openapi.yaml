swagger: "2.0"
x-collection-name: Click Meter
x-complete: 1
info:
  title: Click Meter
  description: api-dashboard-for-clickmeter-api
  contact:
    name: Api Support
    url: http://www.clickmeter.com/api
    email: api@clickmeter.com
  version: v2
host: apiv2.clickmeter.com:80
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account:
    get:
      summary: Retrieve current account data
      description: Retrieve current account data.
      operationId: getAccount
      x-api-path-slug: account-get
      responses:
        200:
          description: OK
      tags:
      - Account
    post:
      summary: Update current account data
      description: Update current account data.
      operationId: postAccount
      x-api-path-slug: account-post
      parameters:
      - in: body
        name: value
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
  /account/domainwhitelist:
    get:
      summary: Retrieve list of a domains allowed to redirect in DDU mode
      description: Retrieve list of a domains allowed to redirect in ddu mode.
      operationId: getAccountDomainwhitelist
      x-api-path-slug: accountdomainwhitelist-get
      parameters:
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      responses:
        200:
          description: OK
      tags:
      - Account
      - Domainwhitelist
    post:
      summary: Create an domain entry
      description: Create an domain entry.
      operationId: postAccountDomainwhitelist
      x-api-path-slug: accountdomainwhitelist-post
      parameters:
      - in: body
        name: value
        description: The entry to add
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Domainwhitelist
  /account/domainwhitelist/{whitelistId}:
    delete:
      summary: Delete an domain entry
      description: Delete an domain entry.
      operationId: deleteAccountDomainwhitelistWhitelist
      x-api-path-slug: accountdomainwhitelistwhitelistid-delete
      parameters:
      - in: path
        name: whitelistId
        description: The id of the domain to delete
      responses:
        200:
          description: OK
      tags:
      - Account
      - Domainwhitelist
      - WhitelistId
  /account/guests:
    get:
      summary: Retrieve list of a guest
      description: Retrieve list of a guest.
      operationId: getAccountGuests
      x-api-path-slug: accountguests-get
      parameters:
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortDirection
        description: Direction of sort asc or desc
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      responses:
        200:
          description: OK
      tags:
      - Account
      - Guests
    post:
      summary: Create a guest
      description: Create a guest.
      operationId: postAccountGuests
      x-api-path-slug: accountguests-post
      parameters:
      - in: body
        name: value
        description: Guest object to create
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Guests
  /account/guests/count:
    get:
      summary: Retrieve count of guests
      description: Retrieve count of guests.
      operationId: getAccountGuestsCount
      x-api-path-slug: accountguestscount-get
      parameters:
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      responses:
        200:
          description: OK
      tags:
      - Account
      - Guests
      - Count
  /account/guests/{guestId}:
    delete:
      summary: Delete a guest
      description: Delete a guest.
      operationId: deleteAccountGuestsGuest
      x-api-path-slug: accountguestsguestid-delete
      parameters:
      - in: path
        name: guestId
        description: Id of the guest
      responses:
        200:
          description: OK
      tags:
      - Account
      - Guests
      - GuestId
    get:
      summary: Retrieve a guest
      description: Retrieve a guest.
      operationId: getAccountGuestsGuest
      x-api-path-slug: accountguestsguestid-get
      parameters:
      - in: path
        name: guestId
        description: Id of the guest
      responses:
        200:
          description: OK
      tags:
      - Account
      - Guests
      - GuestId
    post:
      summary: Update a guest
      description: Update a guest.
      operationId: postAccountGuestsGuest
      x-api-path-slug: accountguestsguestid-post
      parameters:
      - in: path
        name: guestId
        description: Id of the guest
      - in: body
        name: value
        description: Guest object with field updated
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Guests
      - GuestId
  /account/guests/{guestId}/permissions:
    get:
      summary: Retrieve permissions for a guest
      description: Retrieve permissions for a guest.
      operationId: getAccountGuestsGuestPermissions
      x-api-path-slug: accountguestsguestidpermissions-get
      parameters:
      - in: query
        name: entityId
        description: Optional id of the datapoint/group entity to filter by
      - in: query
        name: entityType
        description: Can be datapoint or group
      - in: path
        name: guestId
        description: Id of the guest
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: type
        description: Can be w or r
      responses:
        200:
          description: OK
      tags:
      - Account
      - Guests
      - GuestId
      - Permissions
  /account/guests/{guestId}/permissions/count:
    get:
      summary: Retrieve count of the permissions for a guest
      description: Retrieve count of the permissions for a guest.
      operationId: getAccountGuestsGuestPermissionsCount
      x-api-path-slug: accountguestsguestidpermissionscount-get
      parameters:
      - in: query
        name: entityId
        description: Optional id of the datapoint/group entity to filter by
      - in: query
        name: entityType
        description: Can be datapoint or group
      - in: path
        name: guestId
        description: Id of the guest
      - in: query
        name: type
        description: Can be w or r
      responses:
        200:
          description: OK
      tags:
      - Account
      - Guests
      - GuestId
      - Permissions
      - Count
  /account/guests/{guestId}/{type}/permissions/patch:
    post:
      summary: Change the permission on a shared object
      description: Change the permission on a shared object.
      operationId: postAccountGuestsGuestTypePermissionsPatch
      x-api-path-slug: accountguestsguestidtypepermissionspatch-post
      parameters:
      - in: body
        name: body
        description: The patch permission request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: guestId
        description: Id of the guest
      - in: path
        name: type
        description: Can be datapoint or group
      responses:
        200:
          description: OK
      tags:
      - Account
      - Guests
      - GuestId
      - Type
      - Permissions
      - Patch
    put:
      summary: Change the permission on a shared object
      description: Change the permission on a shared object.
      operationId: putAccountGuestsGuestTypePermissionsPatch
      x-api-path-slug: accountguestsguestidtypepermissionspatch-put
      parameters:
      - in: body
        name: body
        description: The patch permission request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: guestId
        description: Id of the guest
      - in: path
        name: type
        description: Can be datapoint or group
      responses:
        200:
          description: OK
      tags:
      - Account
      - Guests
      - GuestId
      - Type
      - Permissions
      - Patch
  /account/ipblacklist:
    get:
      summary: Retrieve list of a ip to exclude from event tracking
      description: Retrieve list of a ip to exclude from event tracking.
      operationId: getAccountIpblacklist
      x-api-path-slug: accountipblacklist-get
      parameters:
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      responses:
        200:
          description: OK
      tags:
      - Account
      - Ipblacklist
    post:
      summary: Create an ip blacklist entry
      description: Create an ip blacklist entry.
      operationId: postAccountIpblacklist
      x-api-path-slug: accountipblacklist-post
      parameters:
      - in: body
        name: value
        description: The entry to add
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Ipblacklist
  /account/ipblacklist/{blacklistId}:
    delete:
      summary: Delete an ip blacklist entry
      description: Delete an ip blacklist entry.
      operationId: deleteAccountIpblacklistBlacklist
      x-api-path-slug: accountipblacklistblacklistid-delete
      parameters:
      - in: path
        name: blacklistId
        description: The id of the ip to delete
      responses:
        200:
          description: OK
      tags:
      - Account
      - Ipblacklist
      - BlacklistId
  /account/plan:
    get:
      summary: Retrieve current account plan
      description: Retrieve current account plan.
      operationId: getAccountPlan
      x-api-path-slug: accountplan-get
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
  /aggregated:
    get:
      summary: Retrieve statistics about this customer for a timeframe
      description: Retrieve statistics about this customer for a timeframe.
      operationId: getAggregated
      x-api-path-slug: aggregated-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hourly
        description: If using yesterday or today timeframe you can ask for the hourly
          detail
      - in: query
        name: onlyFavorites
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Aggregated
  /aggregated/list:
    get:
      summary: Retrieve statistics about this customer for a timeframe grouped by
        some temporal entity (day/week/month)
      description: Retrieve statistics about this customer for a timeframe grouped
        by some temporal entity (day/week/month).
      operationId: getAggregatedList
      x-api-path-slug: aggregatedlist-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Aggregated
      - List
  /aggregated/summary/conversions:
    get:
      summary: Retrieve statistics about a subset of conversions for a timeframe with
        conversions data
      description: Retrieve statistics about a subset of conversions for a timeframe
        with conversions data.
      operationId: getAggregatedSummaryConversions
      x-api-path-slug: aggregatedsummaryconversions-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortDirection
        description: Direction of sort asc or desc
      - in: query
        name: status
        description: Status of conversion (deleted/active)
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Aggregated
      - Summary
      - Conversions
  /aggregated/summary/datapoints:
    get:
      summary: Retrieve statistics about a subset of datapoints for a timeframe with
        datapoints data
      description: Retrieve statistics about a subset of datapoints for a timeframe
        with datapoints data.
      operationId: getAggregatedSummaryDatapoints
      x-api-path-slug: aggregatedsummarydatapoints-get
      parameters:
      - in: query
        name: favourite
        description: Is the datapoint marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupId
        description: Filter by this group id
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortDirection
        description: Direction of sort asc or desc
      - in: query
        name: status
        description: Status of datapoint (deleted/active/paused/spam)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of datapoint (tl/tp)
      responses:
        200:
          description: OK
      tags:
      - Aggregated
      - Summary
      - Datapoints
  /aggregated/summary/groups:
    get:
      summary: Retrieve statistics about a subset of groups for a timeframe with groups
        data
      description: Retrieve statistics about a subset of groups for a timeframe with
        groups data.
      operationId: getAggregatedSummaryGroups
      x-api-path-slug: aggregatedsummarygroups-get
      parameters:
      - in: query
        name: favourite
        description: Is the group marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortDirection
        description: Direction of sort asc or desc
      - in: query
        name: status
        description: Status of group (deleted/active)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Aggregated
      - Summary
      - Groups
  /clickstream:
    get:
      summary: Retrieve the latest list of events of this account. Limited to last
        100.
      description: Retrieve the latest list of events of this account. limited to
        last 100..
      operationId: getClickstream
      x-api-path-slug: clickstream-get
      parameters:
      - in: query
        name: conversion
        description: Filter by this conversion id (mutually exclusive with datapoint
          and group)
      - in: query
        name: datapoint
        description: Filter by this datapoint id (mutually exclusive with group and
          conversion)
      - in: query
        name: filter
        description: Filter event type (spiders/uniques/nonuniques/conversions)
      - in: query
        name: group
        description: Filter by this group id (mutually exclusive with datapoint and
          conversion)
      - in: query
        name: pageSize
        description: Limit results to this number
      responses:
        200:
          description: OK
      tags:
      - Clickstream
  /conversions:
    get:
      summary: Retrieve a list of conversions
      description: Retrieve a list of conversions.
      operationId: getConversions
      x-api-path-slug: conversions-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude conversions created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude conversions created after this date (YYYYMMDD)
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: status
        description: Status of conversion (deleted/active)
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      responses:
        200:
          description: OK
      tags:
      - Conversions
    post:
      summary: Create a conversion
      description: Create a conversion.
      operationId: postConversions
      x-api-path-slug: conversions-post
      parameters:
      - in: body
        name: value
        description: The body of the conversion
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Conversions
  /conversions/aggregated/list:
    get:
      summary: Retrieve statistics about this customer for a timeframe related to
        a subset of conversions grouped by some temporal entity (day/week/month)
      description: Retrieve statistics about this customer for a timeframe related
        to a subset of conversions grouped by some temporal entity (day/week/month).
      operationId: getConversionsAggregatedList
      x-api-path-slug: conversionsaggregatedlist-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: status
        description: Status of conversion (deleted/active)
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - Aggregated
      - List
  /conversions/count:
    get:
      summary: Retrieve a count of conversions
      description: Retrieve a count of conversions.
      operationId: getConversionsCount
      x-api-path-slug: conversionscount-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude conversions created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude conversions created after this date (YYYYMMDD)
      - in: query
        name: status
        description: Status of conversion (deleted/active)
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - Count
  /conversions/{conversionId}:
    delete:
      summary: Delete conversion specified by id
      description: Delete conversion specified by id.
      operationId: deleteConversionsConversion
      x-api-path-slug: conversionsconversionid-delete
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
    get:
      summary: Retrieve conversion specified by id
      description: Retrieve conversion specified by id.
      operationId: getConversionsConversion
      x-api-path-slug: conversionsconversionid-get
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
    post:
      summary: Update conversion specified by id
      description: Update conversion specified by id.
      operationId: postConversionsConversion
      x-api-path-slug: conversionsconversionid-post
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      - in: body
        name: value
        description: Updated body of the conversion
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
  /conversions/{conversionId}/aggregated:
    get:
      summary: Retrieve statistics about this conversion for a timeframe
      description: Retrieve statistics about this conversion for a timeframe.
      operationId: getConversionsConversionAggregated
      x-api-path-slug: conversionsconversionidaggregated-get
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      - in: query
        name: favourite
        description: Is the datapoint marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hourly
        description: If using yesterday or today timeframe you can ask for the hourly
          detail
      - in: query
        name: tag
        description: Filter by this tag name
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
      - Aggregated
  /conversions/{conversionId}/aggregated/list:
    get:
      summary: Retrieve statistics about this conversion for a timeframe grouped by
        some temporal entity (day/week/month)
      description: Retrieve statistics about this conversion for a timeframe grouped
        by some temporal entity (day/week/month).
      operationId: getConversionsConversionAggregatedList
      x-api-path-slug: conversionsconversionidaggregatedlist-get
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
      - Aggregated
      - List
  /conversions/{conversionId}/datapoints:
    get:
      summary: Retrieve a list of datapoints connected to this conversion
      description: Retrieve a list of datapoints connected to this conversion.
      operationId: getConversionsConversionDatapoints
      x-api-path-slug: conversionsconversioniddatapoints-get
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      - in: query
        name: createdAfter
        description: Exclude datapoints created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude datapoints created after this date (YYYYMMDD)
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: status
        description: Status of datapoint (deleted/active/paused/spam)
      - in: query
        name: tags
        description: Filter by this tag name
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: type
        description: Type of datapoint (tl/tp)
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
      - Datapoints
  /conversions/{conversionId}/datapoints/batch/patch:
    put:
      summary: Modify the association between a conversion and multiple datapoints
      description: Modify the association between a conversion and multiple datapoints.
      operationId: putConversionsConversionDatapointsBatchPatch
      x-api-path-slug: conversionsconversioniddatapointsbatchpatch-put
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      - in: body
        name: data
        description: Patch requests
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
      - Datapoints
      - Batch
      - Patch
  /conversions/{conversionId}/datapoints/count:
    get:
      summary: Retrieve a count of datapoints connected to this conversion
      description: Retrieve a count of datapoints connected to this conversion.
      operationId: getConversionsConversionDatapointsCount
      x-api-path-slug: conversionsconversioniddatapointscount-get
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      - in: query
        name: createdAfter
        description: Exclude datapoints created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude datapoints created after this date (YYYYMMDD)
      - in: query
        name: status
        description: Status of datapoint (deleted/active/paused/spam)
      - in: query
        name: tags
        description: Filter by this tag name
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: type
        description: Type of datapoint (tl/tp)
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
      - Datapoints
      - Count
  /conversions/{conversionId}/datapoints/patch:
    put:
      summary: Modify the association between a conversion and a datapoint
      description: Modify the association between a conversion and a datapoint.
      operationId: putConversionsConversionDatapointsPatch
      x-api-path-slug: conversionsconversioniddatapointspatch-put
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      - in: body
        name: data
        description: Patch request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
      - Datapoints
      - Patch
  /conversions/{conversionId}/hits:
    get:
      summary: Retrieve the list of events related to this conversion.
      description: Retrieve the list of events related to this conversion..
      operationId: getConversionsConversionHits
      x-api-path-slug: conversionsconversionidhits-get
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      - in: query
        name: filter
        description: Filter event type (spiders/uniques/nonuniques/conversions)
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from (its the lastKey field in the response
          object)
      - in: query
        name: timeframe
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
      - Hits
  /conversions/{conversionId}/notes:
    put:
      summary: Fast patch the "notes" field of a conversion
      description: Fast patch the "notes" field of a conversion.
      operationId: putConversionsConversionNotes
      x-api-path-slug: conversionsconversionidnotes-put
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      - in: body
        name: note
        description: Patch requests
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
      - Notes
  /conversions/{conversionId}/reports:
    get:
      summary: Retrieve a top report connected to this conversion
      description: Retrieve a top report connected to this conversion.
      operationId: getConversionsConversionReports
      x-api-path-slug: conversionsconversionidreports-get
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hittype
        description: Type of the event you want to filter this report with
      - in: query
        name: timeframe
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of the report
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
      - Reports
  /datapoints:
    get:
      summary: List of all the datapoints associated to the user
      description: List of all the datapoints associated to the user.
      operationId: getDatapoints
      x-api-path-slug: datapoints-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude datapoints created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude datapoints created after this date (YYYYMMDD)
      - in: query
        name: limit
        description: Maximum elements to retrieve
      - in: query
        name: offset
        description: Where to start when retrieving elements
      - in: query
        name: onlyFavorites
        description: Filter fields by favourite status
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortDirection
        description: Direction of sort asc or desc
      - in: query
        name: status
        description: Status of the datapoint
      - in: query
        name: tags
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: type
        description: Type of the datapoint (tp/tl)
      responses:
        200:
          description: OK
      tags:
      - Datapoints
    post:
      summary: Create a datapoint
      description: Create a datapoint.
      operationId: postDatapoints
      x-api-path-slug: datapoints-post
      parameters:
      - in: body
        name: value
        description: The body of the datapoint
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datapoints
  /datapoints/aggregated:
    get:
      summary: Retrieve statistics about this customer for a timeframe by groups
      description: Retrieve statistics about this customer for a timeframe by groups.
      operationId: getDatapointsAggregated
      x-api-path-slug: datapointsaggregated-get
      parameters:
      - in: query
        name: favourite
        description: Is the datapoint is marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hourly
        description: If using yesterday or today timeframe you can ask for the hourly
          detail
      - in: query
        name: status
        description: Status of datapoint (deleted/active/paused/spam)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of datapoint (tl/tp)
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Aggregated
  /datapoints/aggregated/list:
    get:
      summary: Retrieve statistics about all datapoints of this customer for a timeframe
        grouped by some temporal entity (day/week/month)
      description: Retrieve statistics about all datapoints of this customer for a
        timeframe grouped by some temporal entity (day/week/month).
      operationId: getDatapointsAggregatedList
      x-api-path-slug: datapointsaggregatedlist-get
      parameters:
      - in: query
        name: favourite
        description: Is the datapoint is marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: status
        description: Status of datapoint (deleted/active/paused/spam)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of datapoint (tl/tp)
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Aggregated
      - List
  /datapoints/batch:
    delete:
      summary: Delete multiple datapoints
      description: Delete multiple datapoints.
      operationId: deleteDatapointsBatch
      x-api-path-slug: datapointsbatch-delete
      parameters:
      - in: body
        name: batch
        description: A json containing the datapoints to delete
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Batch
    post:
      summary: Update multiple datapoints
      description: Update multiple datapoints.
      operationId: postDatapointsBatch
      x-api-path-slug: datapointsbatch-post
      parameters:
      - in: body
        name: batch
        description: A json containing the datapoints to update
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Batch
    put:
      summary: Create multiple datapoints
      description: Create multiple datapoints.
      operationId: putDatapointsBatch
      x-api-path-slug: datapointsbatch-put
      parameters:
      - in: body
        name: batch
        description: A json containing the datapoints to create
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Batch
  /datapoints/count:
    get:
      summary: Count the datapoints associated to the user
      description: Count the datapoints associated to the user.
      operationId: getDatapointsCount
      x-api-path-slug: datapointscount-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude datapoints created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude datapoints created after this date (YYYYMMDD)
      - in: query
        name: onlyFavorites
        description: Filter fields by favourite status
      - in: query
        name: status
        description: Status of the datapoint
      - in: query
        name: tags
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: type
        description: Type of the datapoint (tp/tl)
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Count
  /datapoints/{id}:
    delete:
      summary: Delete a datapoint
      description: Delete a datapoint.
      operationId: deleteDatapoints
      x-api-path-slug: datapointsid-delete
      parameters:
      - in: path
        name: id
        description: The id of the datapoint
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Id
    get:
      summary: Get a datapoint
      description: Get a datapoint.
      operationId: getDatapoints
      x-api-path-slug: datapointsid-get
      parameters:
      - in: path
        name: id
        description: The id of the datapoint
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Id
    post:
      summary: Update a datapoint
      description: Update a datapoint.
      operationId: postDatapoints
      x-api-path-slug: datapointsid-post
      parameters:
      - in: path
        name: id
        description: The id of the datapoint
      - in: body
        name: value
        description: The body of the datapoint
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Id
  /datapoints/{id}/aggregated:
    get:
      summary: Retrieve statistics about this datapoint for a timeframe
      description: Retrieve statistics about this datapoint for a timeframe.
      operationId: getDatapointsAggregated
      x-api-path-slug: datapointsidaggregated-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hourly
        description: If using yesterday or today timeframe you can ask for the hourly
          detail
      - in: path
        name: id
        description: Id of the datapoint
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Id
      - Aggregated
  /datapoints/{id}/aggregated/list:
    get:
      summary: Retrieve statistics about this datapoint for a timeframe grouped by
        some temporal entity (day/week/month)
      description: Retrieve statistics about this datapoint for a timeframe grouped
        by some temporal entity (day/week/month).
      operationId: getDatapointsAggregatedList
      x-api-path-slug: datapointsidaggregatedlist-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: path
        name: id
        description: Id of the datapoint
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Id
      - Aggregated
      - List
  /datapoints/{id}/favourite:
    put:
      summary: Fast switch the "favourite" field of a datapoint
      description: Fast switch the "favourite" field of a datapoint.
      operationId: putDatapointsFavourite
      x-api-path-slug: datapointsidfavourite-put
      parameters:
      - in: path
        name: id
        description: Id of the datapoint
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Id
      - Favourite
  /datapoints/{id}/hits:
    get:
      summary: Retrieve the list of events related to this datapoint.
      description: Retrieve the list of events related to this datapoint..
      operationId: getDatapointsHits
      x-api-path-slug: datapointsidhits-get
      parameters:
      - in: query
        name: filter
        description: Filter event type (spiders/uniques/nonuniques/conversions)
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: path
        name: id
        description: Id of the datapoint
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from (its the lastKey field in the response
          object)
      - in: query
        name: timeframe
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Id
      - Hits
  /datapoints/{id}/notes:
    put:
      summary: Fast patch the "notes" field of a datapoint
      description: Fast patch the "notes" field of a datapoint.
      operationId: putDatapointsNotes
      x-api-path-slug: datapointsidnotes-put
      parameters:
      - in: path
        name: id
        description: Id of the datapoint
      - in: body
        name: note
        description: Patch requests
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Id
      - Notes
  /datapoints/{id}/reports:
    get:
      summary: Retrieve a top report connected to this datapoint
      description: Retrieve a top report connected to this datapoint.
      operationId: getDatapointsReports
      x-api-path-slug: datapointsidreports-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: path
        name: id
        description: Id of the datapoint
      - in: query
        name: timeframe
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of the report
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Id
      - Reports
  /domains:
    get:
      summary: Retrieve a list of domains
      description: Retrieve a list of domains.
      operationId: getDomains
      x-api-path-slug: domains-get
      parameters:
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: name
        description: Filter domains with this anmen
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: type
        description: Type of domain (system/go/personal/dedicated)
      responses:
        200:
          description: OK
      tags:
      - Domains
    post:
      summary: Create a domain
      description: Create a domain.
      operationId: postDomains
      x-api-path-slug: domains-post
      parameters:
      - in: body
        name: value
        description: The domain to create
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Domains
  /domains/count:
    get:
      summary: Retrieve count of domains
      description: Retrieve count of domains.
      operationId: getDomainsCount
      x-api-path-slug: domainscount-get
      parameters:
      - in: query
        name: name
        description: Filter domains with this anmen
      - in: query
        name: type
        description: Type of domain (system/go/personal/dedicated)
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Count
  /domains/{id}:
    delete:
      summary: Delete a domain
      description: Delete a domain.
      operationId: deleteDomains
      x-api-path-slug: domainsid-delete
      parameters:
      - in: path
        name: id
        description: Id of domain
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Id
    get:
      summary: Get a domain
      description: Get a domain.
      operationId: getDomains
      x-api-path-slug: domainsid-get
      parameters:
      - in: path
        name: id
        description: Id of domain
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Id
    post:
      summary: Update a domain
      description: Update a domain.
      operationId: postDomains
      x-api-path-slug: domainsid-post
      parameters:
      - in: path
        name: id
        description: Id of domain
      - in: body
        name: value
        description: The domain to update
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Id
  /groups:
    get:
      summary: List of all the groups associated to the user.
      description: List of all the groups associated to the user..
      operationId: getGroups
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude groups created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude groups created after this date (YYYYMMDD)
      - in: query
        name: limit
        description: Maximum elements to retrieve
      - in: query
        name: offset
        description: Where to start when retrieving elements
      - in: query
        name: status
        description: Status of the group
      - in: query
        name: tags
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: write
        description: Write permission
      responses:
        200:
          description: OK
      tags:
      - Groups
    post:
      summary: Create a group
      description: Create a group.
      operationId: postGroups
      x-api-path-slug: groups-post
      parameters:
      - in: body
        name: value
        description: The body of the group
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Groups
  /groups/aggregated:
    get:
      summary: Retrieve statistics about this customer for a timeframe by groups
      description: Retrieve statistics about this customer for a timeframe by groups.
      operationId: getGroupsAggregated
      x-api-path-slug: groupsaggregated-get
      parameters:
      - in: query
        name: favourite
        description: Is the group is marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hourly
        description: If using yesterday or today timeframe you can ask for the hourly
          detail
      - in: query
        name: status
        description: Status of group (deleted/active)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Aggregated
  /groups/aggregated/list:
    get:
      summary: Retrieve statistics about all groups of this customer for a timeframe
        grouped by some temporal entity (day/week/month)
      description: Retrieve statistics about all groups of this customer for a timeframe
        grouped by some temporal entity (day/week/month).
      operationId: getGroupsAggregatedList
      x-api-path-slug: groupsaggregatedlist-get
      parameters:
      - in: query
        name: favourite
        description: Is the group is marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: status
        description: Status of group (deleted/active)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Aggregated
      - List
  /groups/count:
    get:
      summary: Count the groups associated to the user.
      description: Count the groups associated to the user..
      operationId: getGroupsCount
      x-api-path-slug: groupscount-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude groups created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude groups created after this date (YYYYMMDD)
      - in: query
        name: status
        description: Status of the datapoint
      - in: query
        name: tags
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: write
        description: Write permission
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Count
  /groups/{id}:
    delete:
      summary: Delete group specified by id
      description: Delete group specified by id.
      operationId: deleteGroups
      x-api-path-slug: groupsid-delete
      parameters:
      - in: path
        name: id
        description: Id of the group
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
    get:
      summary: Get a group
      description: Get a group.
      operationId: getGroups
      x-api-path-slug: groupsid-get
      parameters:
      - in: path
        name: id
        description: The id of the group
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
    post:
      summary: Update a group
      description: Update a group.
      operationId: postGroups
      x-api-path-slug: groupsid-post
      parameters:
      - in: path
        name: id
        description: The id of the group
      - in: body
        name: value
        description: The body of the group
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
  /groups/{id}/aggregated:
    get:
      summary: Retrieve statistics about this group for a timeframe
      description: Retrieve statistics about this group for a timeframe.
      operationId: getGroupsAggregated
      x-api-path-slug: groupsidaggregated-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hourly
        description: If using yesterday or today timeframe you can ask for the hourly
          detail
      - in: path
        name: id
        description: Id of the group
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Aggregated
  /groups/{id}/aggregated/list:
    get:
      summary: Retrieve statistics about this group for a timeframe grouped by some
        temporal entity (day/week/month)
      description: Retrieve statistics about this group for a timeframe grouped by
        some temporal entity (day/week/month).
      operationId: getGroupsAggregatedList
      x-api-path-slug: groupsidaggregatedlist-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: path
        name: id
        description: Id of the group
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Aggregated
      - List
  /groups/{id}/aggregated/summary:
    get:
      summary: Retrieve statistics about a subset of datapoints for a timeframe with
        datapoints data
      description: Retrieve statistics about a subset of datapoints for a timeframe
        with datapoints data.
      operationId: getGroupsAggregatedSummary
      x-api-path-slug: groupsidaggregatedsummary-get
      parameters:
      - in: query
        name: favourite
        description: Is the datapoint marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: path
        name: id
        description: Filter by this group id
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortDirection
        description: Direction of sort asc or desc
      - in: query
        name: status
        description: Status of datapoint (deleted/active/paused/spam)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of datapoint (tl/tp)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Aggregated
      - Summary
  /groups/{id}/datapoints:
    get:
      summary: List of all the datapoints associated to the user in this group.
      description: List of all the datapoints associated to the user in this group..
      operationId: getGroupsDatapoints
      x-api-path-slug: groupsiddatapoints-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude datapoints created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude datapoints created after this date (YYYYMMDD)
      - in: path
        name: id
        description: Id of the group
      - in: query
        name: limit
        description: Maximum elements to retrieve
      - in: query
        name: offset
        description: Where to start when retrieving elements
      - in: query
        name: onlyFavorites
        description: Filter fields by favourite status
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortDirection
        description: Direction of sort asc or desc
      - in: query
        name: status
        description: Status of the datapoint
      - in: query
        name: tags
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: type
        description: Type of the datapoint (tp/tl)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Datapoints
    post:
      summary: Create a datapoint in this group
      description: Create a datapoint in this group.
      operationId: postGroupsDatapoints
      x-api-path-slug: groupsiddatapoints-post
      parameters:
      - in: path
        name: id
        description: The id of the group
      - in: body
        name: value
        description: The body of the datapoint
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Datapoints
  /groups/{id}/datapoints/count:
    get:
      summary: Count the datapoints associated to the user in this group.
      description: Count the datapoints associated to the user in this group..
      operationId: getGroupsDatapointsCount
      x-api-path-slug: groupsiddatapointscount-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude datapoints created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude datapoints created after this date (YYYYMMDD)
      - in: path
        name: id
        description: Id of the group
      - in: query
        name: onlyFavorites
        description: Filter fields by favourite status
      - in: query
        name: status
        description: Status of the datapoint
      - in: query
        name: tags
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: type
        description: Type of the datapoint (tp/tl)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Datapoints
      - Count
  /groups/{id}/favourite:
    put:
      summary: Fast switch the "favourite" field of a group
      description: Fast switch the "favourite" field of a group.
      operationId: putGroupsFavourite
      x-api-path-slug: groupsidfavourite-put
      parameters:
      - in: path
        name: id
        description: Id of the group
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Favourite
  /groups/{id}/hits:
    get:
      summary: Retrieve the list of events related to this group.
      description: Retrieve the list of events related to this group..
      operationId: getGroupsHits
      x-api-path-slug: groupsidhits-get
      parameters:
      - in: query
        name: filter
        description: Filter event type (spiders/uniques/nonuniques/conversions)
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: path
        name: id
        description: Id of the group
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from (its the lastKey field in the response
          object)
      - in: query
        name: timeframe
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Hits
  /groups/{id}/notes:
    put:
      summary: Fast patch the "notes" field of a group
      description: Fast patch the "notes" field of a group.
      operationId: putGroupsNotes
      x-api-path-slug: groupsidnotes-put
      parameters:
      - in: path
        name: id
        description: Id of the group
      - in: body
        name: note
        description: Patch requests
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Notes
  /groups/{id}/reports:
    get:
      summary: Retrieve a top report connected to this group
      description: Retrieve a top report connected to this group.
      operationId: getGroupsReports
      x-api-path-slug: groupsidreports-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hittype
        description: Type of the event you want to filter this report with
      - in: path
        name: id
        description: Id of the group
      - in: query
        name: timeframe
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of the report
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Reports
  /hits:
    get:
      summary: Retrieve the list of events related to this account.
      description: Retrieve the list of events related to this account..
      operationId: getHits
      x-api-path-slug: hits-get
      parameters:
      - in: query
        name: filter
        description: Filter event type (spiders/uniques/nonuniques/conversions)
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from (its the lastKey field in the response
          object)
      - in: query
        name: timeframe
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Hits
  /me:
    get:
      summary: Retrieve current account data
      description: Retrieve current account data.
      operationId: getMe
      x-api-path-slug: me-get
      responses:
        200:
          description: OK
      tags:
      - Me
  /me/plan:
    get:
      summary: Retrieve current account plan
      description: Retrieve current account plan.
      operationId: getMePlan
      x-api-path-slug: meplan-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Plan
  /reports:
    get:
      summary: Retrieve a top report
      description: Retrieve a top report.
      operationId: getReports
      x-api-path-slug: reports-get
      parameters:
      - in: query
        name: conversion
        description: Filter by this conversion id (mutually exclusive with datapoint
          and group)
      - in: query
        name: datapoint
        description: Filter by this datapoint id (mutually exclusive with group and
          conversion)
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: group
        description: Filter by this group id (mutually exclusive with datapoint and
          conversion)
      - in: query
        name: hittype
        description: Type of the event you want to filter this report with
      - in: query
        name: timeframe
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of the report
      responses:
        200:
          description: OK
      tags:
      - Reports
  /retargeting:
    get:
      summary: List of all the retargeting scripts associated to the user
      description: List of all the retargeting scripts associated to the user.
      operationId: getRetargeting
      x-api-path-slug: retargeting-get
      parameters:
      - in: query
        name: limit
        description: Maximum elements to retrieve
      - in: query
        name: offset
        description: Where to start when retrieving elements
      responses:
        200:
          description: OK
      tags:
      - Retargeting
    post:
      summary: Creates a retargeting script
      description: Creates a retargeting script.
      operationId: postRetargeting
      x-api-path-slug: retargeting-post
      parameters:
      - in: body
        name: value
        description: The body of the retargeting script
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Retargeting
  /retargeting/count:
    get:
      summary: Retrieve count of retargeting scripts
      description: Retrieve count of retargeting scripts.
      operationId: getRetargetingCount
      x-api-path-slug: retargetingcount-get
      responses:
        200:
          description: OK
      tags:
      - Retargeting
      - Count
  /retargeting/{id}:
    delete:
      summary: Deletes a retargeting script (and remove associations)
      description: Deletes a retargeting script (and remove associations).
      operationId: deleteRetargeting
      x-api-path-slug: retargetingid-delete
      parameters:
      - in: path
        name: id
        description: The id of the retargeting script
      responses:
        200:
          description: OK
      tags:
      - Retargeting
      - Id
    get:
      summary: Get a retargeting script object
      description: Get a retargeting script object.
      operationId: getRetargeting
      x-api-path-slug: retargetingid-get
      parameters:
      - in: path
        name: id
        description: The id of the retargeting script
      responses:
        200:
          description: OK
      tags:
      - Retargeting
      - Id
    post:
      summary: Updates a retargeting script
      description: Updates a retargeting script.
      operationId: postRetargeting
      x-api-path-slug: retargetingid-post
      parameters:
      - in: path
        name: id
        description: The id of the retargeting script
      - in: body
        name: value
        description: The body of the retargeting script
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Retargeting
      - Id
  /retargeting/{id}/datapoints:
    get:
      summary: List of all the datapoints associated to the retargeting script.
      description: List of all the datapoints associated to the retargeting script..
      operationId: getRetargetingDatapoints
      x-api-path-slug: retargetingiddatapoints-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude datapoints created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude datapoints created after this date (YYYYMMDD)
      - in: path
        name: id
        description: Id of the retargeting script
      - in: query
        name: limit
        description: Maximum elements to retrieve
      - in: query
        name: offset
        description: Where to start when retrieving elements
      - in: query
        name: onlyFavorites
        description: Filter fields by favourite status
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortDirection
        description: Direction of sort asc or desc
      - in: query
        name: status
        description: Status of the datapoint
      - in: query
        name: tags
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      responses:
        200:
          description: OK
      tags:
      - Retargeting
      - Id
      - Datapoints
  /retargeting/{id}/datapoints/count:
    get:
      summary: Count the datapoints associated to the retargeting script.
      description: Count the datapoints associated to the retargeting script..
      operationId: getRetargetingDatapointsCount
      x-api-path-slug: retargetingiddatapointscount-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude datapoints created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude datapoints created after this date (YYYYMMDD)
      - in: path
        name: id
        description: Id of the group
      - in: query
        name: onlyFavorites
        description: Filter fields by favourite status
      - in: query
        name: status
        description: Status of the datapoint
      - in: query
        name: tags
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      responses:
        200:
          description: OK
      tags:
      - Retargeting
      - Id
      - Datapoints
      - Count
  /tags:
    get:
      summary: List of all the groups associated to the user filtered by this tag.
      description: List of all the groups associated to the user filtered by this
        tag..
      operationId: getTags
      x-api-path-slug: tags-get
      parameters:
      - in: query
        name: datapoints
        description: Comma separated list of datapoints id to filter by
      - in: query
        name: groups
        description: Comma separated list of groups id to filter by
      - in: query
        name: limit
        description: Maximum elements to retrieve
      - in: query
        name: name
        description: Name of the tag
      - in: query
        name: offset
        description: Where to start when retrieving elements
      - in: query
        name: type
        description: Type of entity related to the tag
      responses:
        200:
          description: OK
      tags:
      - Tags
    post:
      summary: Create a tag
      description: Create a tag.
      operationId: postTags
      x-api-path-slug: tags-post
      parameters:
      - in: body
        name: value
        description: The body of the tag
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/count:
    get:
      summary: List of all the groups associated to the user filtered by this tag.
      description: List of all the groups associated to the user filtered by this
        tag..
      operationId: getTagsCount
      x-api-path-slug: tagscount-get
      parameters:
      - in: query
        name: datapoints
        description: Comma separated list of datapoints id to filter by
      - in: query
        name: groups
        description: Comma separated list of groups id to filter by
      - in: query
        name: name
        description: Name of the tag
      - in: query
        name: type
        description: Type of entity related to the tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Count
  /tags/{tagId}:
    delete:
      summary: Delete a tag
      description: Delete a tag.
      operationId: deleteTagsTag
      x-api-path-slug: tagstagid-delete
      parameters:
      - in: path
        name: tagId
        description: Id of the tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - TagId
    get:
      summary: Retrieve a tag
      description: Retrieve a tag.
      operationId: getTagsTag
      x-api-path-slug: tagstagid-get
      parameters:
      - in: path
        name: tagId
        description: Id of the tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - TagId
  /tags/{tagId}/datapoints:
    delete:
      summary: Delete the association of this tag with all datapoints
      description: Delete the association of this tag with all datapoints.
      operationId: deleteTagsTagDatapoints
      x-api-path-slug: tagstagiddatapoints-delete
      parameters:
      - in: path
        name: tagId
        description: Id of the tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - TagId
      - Datapoints
    get:
      summary: List of all the datapoints associated to the user filtered by this
        tag
      description: List of all the datapoints associated to the user filtered by this
        tag.
      operationId: getTagsTagDatapoints
      x-api-path-slug: tagstagiddatapoints-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude datapoints created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude datapoints created after this date (YYYYMMDD)
      - in: query
        name: limit
        description: Maximum elements to retrieve
      - in: query
        name: offset
        description: Where to start when retrieving elements
      - in: query
        name: status
        description: Status of the datapoint
      - in: path
        name: tagId
        description: Id of the tag
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: type
        description: Type of the datapoint (tp/tl)
      responses:
        200:
          description: OK
      tags:
      - Tags
      - TagId
      - Datapoints
  /tags/{tagId}/datapoints/count:
    get:
      summary: Count the datapoints associated to the user filtered by this tag
      description: Count the datapoints associated to the user filtered by this tag.
      operationId: getTagsTagDatapointsCount
      x-api-path-slug: tagstagiddatapointscount-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude datapoints created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude datapoints created after this date (YYYYMMDD)
      - in: query
        name: status
        description: Status of the datapoint
      - in: path
        name: tagId
        description: Id of the tag
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: type
        description: Type of the datapoint (tp/tl)
      responses:
        200:
          description: OK
      tags:
      - Tags
      - TagId
      - Datapoints
      - Count
  /tags/{tagId}/datapoints/patch:
    put:
      summary: Associate/Deassociate a tag with a datapoint
      description: Associate/deassociate a tag with a datapoint.
      operationId: putTagsTagDatapointsPatch
      x-api-path-slug: tagstagiddatapointspatch-put
      parameters:
      - in: body
        name: data
        description: The body patch
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tagId
        description: Id of the tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - TagId
      - Datapoints
      - Patch
  /tags/{tagId}/groups:
    delete:
      summary: Delete the association of this tag with all groups
      description: Delete the association of this tag with all groups.
      operationId: deleteTagsTagGroups
      x-api-path-slug: tagstagidgroups-delete
      parameters:
      - in: path
        name: tagId
        description: Id of the tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - TagId
      - Groups
    get:
      summary: List of all the groups associated to the user filtered by this tag.
      description: List of all the groups associated to the user filtered by this
        tag..
      operationId: getTagsTagGroups
      x-api-path-slug: tagstagidgroups-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude groups created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude groups created after this date (YYYYMMDD)
      - in: query
        name: limit
        description: Maximum elements to retrieve
      - in: query
        name: offset
        description: Where to start when retrieving elements
      - in: query
        name: status
        description: Status of the datapoint
      - in: path
        name: tagId
        description: Id of the tag
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      responses:
        200:
          description: OK
      tags:
      - Tags
      - TagId
      - Groups
  /tags/{tagId}/groups/count:
    get:
      summary: Count the groups associated to the user filtered by this tag
      description: Count the groups associated to the user filtered by this tag.
      operationId: getTagsTagGroupsCount
      x-api-path-slug: tagstagidgroupscount-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude groups created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude groups created after this date (YYYYMMDD)
      - in: query
        name: status
        description: Status of the datapoint
      - in: path
        name: tagId
        description: Id of the tag
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      responses:
        200:
          description: OK
      tags:
      - Tags
      - TagId
      - Groups
      - Count
  /tags/{tagId}/groups/patch:
    put:
      summary: Associate/Deassociate a tag with a group
      description: Associate/deassociate a tag with a group.
      operationId: putTagsTagGroupsPatch
      x-api-path-slug: tagstagidgroupspatch-put
      parameters:
      - in: body
        name: data
        description: The body patch
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tagId
        description: Id of the tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - TagId
      - Groups
      - Patch
  /tags/{tagId}/name:
    put:
      summary: Fast patch a tag name
      description: Fast patch a tag name.
      operationId: putTagsTagName
      x-api-path-slug: tagstagidname-put
      parameters:
      - in: body
        name: data
        description: The body patch
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tagId
        description: Id of the tag
      responses:
        200:
          description: OK
      tags:
      - Tags
      - TagId
      - Name