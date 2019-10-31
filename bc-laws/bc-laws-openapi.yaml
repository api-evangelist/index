swagger: "2.0"
x-collection-name: BC Laws
x-complete: 1
info:
  title: BC Laws
  description: bc-laws-is-an-electronic-library-providing-free-public-access-to-the-laws-of-british-columbia--bc-laws-is-hosted-by-the-queens-printer-of-british-columbia-and-published-in-partnership-with-the-ministry-of-justice-and-the-law-clerk-of-the-legislative-assembly-bc-laws-contains-a-comprehensive-collection-of-bc-legislation-and-related-materials--it-is-available-on-the-internet-in-two-formsfirst-the-library-is-available-as-a-web-site-in-which-users-can-browse-and-search-the-laws-of-british-columbia-second-the-library-is-available-as-a-portal-to-legislation-in-raw-xml-data-format-accessible-via-the-bc-laws-api2--this-direct-access-to-raw-data-is-intended-to-enable-third-parties-to-build-or-add-their-own-custom-applications-based-on-the-structure-of-the-data-and-all-the-associated-search-functionality-inherent-in-that-structure--the-bc-laws-website-itself-is-an-example-of-one-such-application-
  termsOfService: http://www.data.gov.bc.ca/local/dbc/docs/license/API_Terms_of_Use.pdf
  version: 1.0.0
host: www.bclaws.ca
basePath: /civix
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /content/{aspectId}:
    get:
      summary: Describes the documents and directories available within a specific
        'aspect' (content group) of the BCLaws library
      description: Describes the documents and directories available within a specific
        'aspect' (content group) of the BCLaws library
      operationId: getContentAspect
      x-api-path-slug: contentaspectid-get
      parameters:
      - in: path
        name: aspectId
        description: The identifier of the aspect (content group) to search
      responses:
        200:
          description: OK
      tags:
      - Content
      - AspectId
  /content/{aspectId}/{civixDocumentId}:
    get:
      summary: Lists the metadata available for the specified index or directory from
        the BCLaws legislative respository
      description: Lists the metadata available for the specified index or directory
        from the BCLaws legislative respository
      operationId: getContentAspectCivixdocument
      x-api-path-slug: contentaspectidcivixdocumentid-get
      parameters:
      - in: path
        name: aspectId
        description: The identifier of the aspect (content group) to search
      - in: path
        name: civixDocumentId
        description: The document identification code for an index or directory
      responses:
        200:
          description: OK
      tags:
      - Content
      - AspectId
      - CivixDocumentId
  /document/id/{aspectId}/{civixIndexId}/{civixDocumentId}:
    get:
      summary: Retrieves a specific document from the BCLaws legislative repository
        (HTML format)
      description: 'The /document API allows you to retrieve actual documents from
        the BCLaws legislative repository. To retrieve a document from the repository
        you need the aspect identifier and two other specific pieces of information
        about the document: the index identifier and the document identifier. These
        unique identifiers can be retrieved from the /content API.'
      operationId: getDocumentAspectCivixindexCivixdocument
      x-api-path-slug: documentidaspectidcivixindexidcivixdocumentid-get
      parameters:
      - in: path
        name: aspectId
        description: The identifier of the aspect (content group) to search
      - in: path
        name: civixDocumentId
        description: The document identification code for an index or directory
      - in: path
        name: civixIndexId
        description: Index identification code
      responses:
        200:
          description: OK
      tags:
      - Document
      - Id
      - AspectId
      - CivixIndexId
      - CivixDocumentId
  /document/id/{aspectId}/{civixIndexId}/{civixDocumentId}/search/{searchString}:
    get:
      summary: Retrieves a specific document from the BCLaws legislative repository
        with search text highlighted (HTML format)
      description: 'The /document API allows you to retrieve actual documents from
        the BCLaws legislative repository. To retrieve a document from the repository
        you need the aspect identifier and two other specific pieces of information
        about the document: the index identifier and the document identifier. These
        unique identifiers can be retrieved from the /content API.'
      operationId: getDocumentAspectCivixindexCivixdocumentSearchSearchstring
      x-api-path-slug: documentidaspectidcivixindexidcivixdocumentidsearchsearchstring-get
      parameters:
      - in: path
        name: aspectId
        description: The identifier of the aspect (content group) to search
      - in: path
        name: civixDocumentId
        description: The document identification code for an index or directory
      - in: path
        name: civixIndexId
        description: Index identification code
      - in: path
        name: searchString
        description: The text to search for within the document
      responses:
        200:
          description: OK
      tags:
      - Document
      - Id
      - AspectId
      - CivixIndexId
      - CivixDocumentId
      - Search
      - SearchString
  /document/id/{aspectId}/{civixIndexId}/{civixDocumentId}/xml:
    get:
      summary: Retrieves a specific document from the BCLaws legislative repository
        (XML format)
      description: 'The /document API allows you to retrieve actual documents from
        the BCLaws legislative repository. To retrieve a document from the repository
        you need the aspect identifier and two other specific pieces of information
        about the document: the index identifier and the document identifier. These
        unique identifiers can be retrieved from the /content API.'
      operationId: getDocumentAspectCivixindexCivixdocumentXml
      x-api-path-slug: documentidaspectidcivixindexidcivixdocumentidxml-get
      parameters:
      - in: path
        name: aspectId
        description: The identifier of the aspect (content group) to search
      - in: path
        name: civixDocumentId
        description: The document identification code for an index or directory
      - in: path
        name: civixIndexId
        description: Index identification code
      responses:
        200:
          description: OK
      tags:
      - Document
      - Id
      - AspectId
      - CivixIndexId
      - CivixDocumentId
      - Xml
  /document/id/{aspectId}/{civixIndexId}/{civixDocumentId}/xml/search/{searchString}:
    get:
      summary: Retrieves a specific document from the BCLaws legislative repository
        with search text highlighted (XML format)
      description: 'The /document API allows you to retrieve actual documents from
        the BCLaws legislative repository. To retrieve a document from the repository
        you need the aspect identifier and two other specific pieces of information
        about the document: the index identifier and the document identifier. These
        unique identifiers can be retrieved from the /content API.'
      operationId: getDocumentAspectCivixindexCivixdocumentXmlSearchSearchstring
      x-api-path-slug: documentidaspectidcivixindexidcivixdocumentidxmlsearchsearchstring-get
      parameters:
      - in: path
        name: aspectId
        description: The identifier of the aspect (content group) to search
      - in: path
        name: civixDocumentId
        description: The document identification code for an index or directory
      - in: path
        name: civixIndexId
        description: Index identification code
      - in: path
        name: searchString
        description: The text to search for within the document
      responses:
        200:
          description: OK
      tags:
      - Document
      - Id
      - AspectId
      - CivixIndexId
      - CivixDocumentId
      - Xml
      - Search
      - SearchString
  /search/{aspectId}/fullsearch:
    get:
      summary: A listing of metadata available for the specified aspect and search
        term from the BCLaws legislative repository
      description: A listing of metadata available for the specified aspect and search
        term from the BCLaws legislative repository
      operationId: getSearchAspectFullsearch
      x-api-path-slug: searchaspectidfullsearch-get
      parameters:
      - in: path
        name: aspectId
        description: The identifier of the aspect (content group) to search
      - in: query
        name: e
        description: last hit (end index)
      - in: query
        name: lFrag
        description: length of fragment snippets (< 200)
      - in: query
        name: nFrag
        description: number of fragment snippets to return (< 10)
      - in: query
        name: q
        description: query term
      - in: query
        name: s
        description: first hit (start index)
      responses:
        200:
          description: OK
      tags:
      - Search
      - AspectId
      - Fullsearch