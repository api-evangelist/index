swagger: "2.0"
x-collection-name: Regulations.gov
x-complete: 1
info:
  title: Regulations.gov
  description: provides-public-users-access-to-federal-regulatory-content-
  version: 1.0.0
host: api.data.gov
basePath: /regulations/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /docket.{response_format}:
    get:
      summary: Returns Docket information
      description: Returns Docket information
      operationId: getDocket.ResponseFormat
      x-api-path-slug: docket-response-format-get
      parameters:
      - in: query
        name: docketId
        description: Docket ID
      - in: path
        name: response_format
        description: Format
      responses:
        200:
          description: OK
      tags:
      - Regulations
      - Dockets
  /document.{response_format}:
    get:
      summary: Returns Document information
      description: Returns Document information
      operationId: getDocument.ResponseFormat
      x-api-path-slug: document-response-format-get
      parameters:
      - in: query
        name: documentId
        description: FDMS Document ID
      - in: query
        name: federalRegisterNumber
        description: Federal Register Document Number
      - in: path
        name: response_format
        description: Format
      responses:
        200:
          description: OK
      tags:
      - Regulations
      - Documents
  /documents.{response_format}:
    get:
      summary: Search for Documents
      description: This API allows users to build a query based on any of the parameters
        below.  If you have trouble building queries, you may wish to try them through
        the Advanced Search page on the Regulations.gov website.
      operationId: getDocuments.ResponseFormat
      x-api-path-slug: documents-response-format-get
      parameters:
      - in: query
        name: a
        description: 'Federal Agency: List of accepted Federal Agency values'
      - in: query
        name: cat
        description: 'Document Category: AD (Aerospace and Transportation) AEP (Agriculture,
          Environment, and Public Lands) BFS (Banking and Financial) CT (Commerce
          and International) LES (Defense, Law Enforcement, and Security) EELS (Education,
          Labor, Presidential, and Government Services) EUMM (Energy, Natural Resources,
          and Utilities) HCFP (Food Safety, Health, and Pharmaceutical) PRE (Housing,
          Development, and Real Estate) ITT (Technology and Telecommunications)'
      - in: query
        name: cmd
        description: 'Comment Period End Date: Enter a date in the form of MM/DD/YY'
      - in: query
        name: cmsd
        description: 'Comment Period Start Date: Enter a date in the form of MM/DD/YY'
      - in: query
        name: countsOnly
        description: 'Counts Only: 1 (will return only the document count for a search
          query)0 (will return documents as well)'
      - in: query
        name: cp
        description: 'Comment Period: O: OpenC: Closed'
      - in: query
        name: crd
        description: 'Creation Date: Enter a date in the form of MM/DD/YY'
      - in: query
        name: cs
        description: 'Comment Period Closing Soon: 0 (closing today)3 (closing within
          3 days)15 (closing within 15 days)30 (closing within 30 days)90 (closing
          within 90 days)'
      - in: query
        name: dct
        description: 'Document Type: N: NoticePR: Proposed RuleFR: RuleO: OtherSR:
          Supporting & Related MaterialPS: Public Submission'
      - in: query
        name: dkt
        description: 'Docket Type: R: RulemakingN: NonrulemakingA Docket Type is either
          Rulemaking or Nonrulemaking'
      - in: query
        name: dktid
        description: Valid Docket ID (ex
      - in: query
        name: dktst
        description: 'Docket Subtype: Only one docket subtype at a time may be selected'
      - in: query
        name: dktst2
        description: 'Docket Sub-subtype: Only one docket sub-subtype at a time may
          be selected'
      - in: query
        name: docst
        description: 'Document Subtype: Single or multiple document subtypes may be
          included'
      - in: query
        name: encoded
        description: 'Encoded: 1 (will accept Regulations'
      - in: query
        name: np
        description: 'Newly Posted: 0 (posted today)3 (posted within last 3 days)15
          (posted within last 15 days)30 (posted within last 30 days)90 (posted within
          last 90 days)  For periods of time beyond 90-days, please use a date range
          with the Posted Date parameter'
      - in: query
        name: pd
        description: 'Posted Date: Enter a date in the form of MM/DD/YY'
      - in: query
        name: po
        description: Enter the page offset (always starts with 0)
      - in: query
        name: rd
        description: 'Received Date: Enter a date in the form of MM/DD/YY'
      - in: path
        name: response_format
        description: Format
      - in: query
        name: rpp
        description: Results Per Page 10, 25, 100, 500, 1,000
      - in: query
        name: s
        description: Keyword(s)
      - in: query
        name: sb
        description: 'Sort By: docketId (Docket ID)docId (Document ID)title (Title)postedDate
          (Posted Date)agency (Agency)documentType (Document Type)submitterName (Submitter
          Name)organization (Organization) Sort Order is REQUIRED if this parameter
          is included'
      - in: query
        name: so
        description: 'Sort Order: ASC: AscendingDESC: Descending'
      responses:
        200:
          description: OK
      tags:
      - Regulations
      - Documents