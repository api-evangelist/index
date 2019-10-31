swagger: "2.0"
x-collection-name: Google Genomics
x-complete: 1
info:
  title: Genomics
  description: upload-process-query-and-search-genomics-data-in-the-cloud-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: genomics.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/annotations:
    post:
      summary: Create Annotation
      description: |-
        Creates a new annotation. Caller must have WRITE permission
        for the associated annotation set.

        The following fields are required:

        * annotationSetId
        * referenceName or
          referenceId

        ### Transcripts

        For annotations of type TRANSCRIPT, the following fields of
        transcript must be provided:

        * exons.start
        * exons.end

        All other fields may be optionally specified, unless documented as being
        server-generated (for example, the `id` field). The annotated
        range must be no longer than 100Mbp (mega base pairs). See the
        Annotation resource
        for additional restrictions on each field.
      operationId: genomics.annotations.create
      x-api-path-slug: v1annotations-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Annotation
  /v1/annotations/search:
    post:
      summary: Search Annotations
      description: |-
        Searches for annotations that match the given criteria. Results are
        ordered by genomic coordinate (by reference sequence, then position).
        Annotations with equivalent genomic coordinates are returned in an
        unspecified order. This order is consistent, such that two queries for the
        same content (regardless of page size) yield annotations in the same order
        across their respective streams of paginated responses. Caller must have
        READ permission for the queried annotation sets.
      operationId: genomics.annotations.search
      x-api-path-slug: v1annotationssearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Annotation
  /v1/annotations/{annotationId}:
    delete:
      summary: Delete Annotation
      description: |-
        Deletes an annotation. Caller must have WRITE permission for
        the associated annotation set.
      operationId: genomics.annotations.delete
      x-api-path-slug: v1annotationsannotationid-delete
      parameters:
      - in: path
        name: annotationId
        description: The ID of the annotation to be deleted
      responses:
        200:
          description: OK
      tags:
      - Annotation
    get:
      summary: Get Annotation
      description: |-
        Gets an annotation. Caller must have READ permission
        for the associated annotation set.
      operationId: genomics.annotations.get
      x-api-path-slug: v1annotationsannotationid-get
      parameters:
      - in: path
        name: annotationId
        description: The ID of the annotation to be retrieved
      responses:
        200:
          description: OK
      tags:
      - Annotation
    put:
      summary: Update Annotation
      description: |-
        Updates an annotation. Caller must have
        WRITE permission for the associated dataset.
      operationId: genomics.annotations.update
      x-api-path-slug: v1annotationsannotationid-put
      parameters:
      - in: path
        name: annotationId
        description: The ID of the annotation to be updated
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: updateMask
        description: An optional mask specifying which fields to update
      responses:
        200:
          description: OK
      tags:
      - Annotation
  /v1/annotations:batchCreate:
    post:
      summary: Create Batch Annotation
      description: |-
        Creates one or more new annotations atomically. All annotations must
        belong to the same annotation set. Caller must have WRITE
        permission for this annotation set. For optimal performance, batch
        positionally adjacent annotations together.

        If the request has a systemic issue, such as an attempt to write to
        an inaccessible annotation set, the entire RPC will fail accordingly. For
        lesser data issues, when possible an error will be isolated to the
        corresponding batch entry in the response; the remaining well formed
        annotations will be created normally.

        For details on the requirements for each individual annotation resource,
        see
        CreateAnnotation.
      operationId: genomics.annotations.batchCreate
      x-api-path-slug: v1annotationsbatchcreate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Annotation
  /v1/annotationsets:
    post:
      summary: Create Annotation Set
      description: |-
        Creates a new annotation set. Caller must have WRITE permission for the
        associated dataset.

        The following fields are required:

          * datasetId
          * referenceSetId

        All other fields may be optionally specified, unless documented as being
        server-generated (for example, the `id` field).
      operationId: genomics.annotationsets.create
      x-api-path-slug: v1annotationsets-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Annotation Set
  /v1/annotationsets/search:
    post:
      summary: Search Annotation Sets
      description: |-
        Searches for annotation sets that match the given criteria. Annotation sets
        are returned in an unspecified order. This order is consistent, such that
        two queries for the same content (regardless of page size) yield annotation
        sets in the same order across their respective streams of paginated
        responses. Caller must have READ permission for the queried datasets.
      operationId: genomics.annotationsets.search
      x-api-path-slug: v1annotationsetssearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Annotation Set
  /v1/annotationsets/{annotationSetId}:
    delete:
      summary: Delete Annotation Set
      description: |-
        Deletes an annotation set. Caller must have WRITE permission
        for the associated annotation set.
      operationId: genomics.annotationsets.delete
      x-api-path-slug: v1annotationsetsannotationsetid-delete
      parameters:
      - in: path
        name: annotationSetId
        description: The ID of the annotation set to be deleted
      responses:
        200:
          description: OK
      tags:
      - Annotation Set
    get:
      summary: Get Annotation Set
      description: |-
        Gets an annotation set. Caller must have READ permission for
        the associated dataset.
      operationId: genomics.annotationsets.get
      x-api-path-slug: v1annotationsetsannotationsetid-get
      parameters:
      - in: path
        name: annotationSetId
        description: The ID of the annotation set to be retrieved
      responses:
        200:
          description: OK
      tags:
      - Annotation Set
    put:
      summary: Update Annotation Set
      description: |-
        Updates an annotation set. The update must respect all mutability
        restrictions and other invariants described on the annotation set resource.
        Caller must have WRITE permission for the associated dataset.
      operationId: genomics.annotationsets.update
      x-api-path-slug: v1annotationsetsannotationsetid-put
      parameters:
      - in: path
        name: annotationSetId
        description: The ID of the annotation set to be updated
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: updateMask
        description: An optional mask specifying which fields to update
      responses:
        200:
          description: OK
      tags:
      - Annotation Set
  /v1/callsets:
    post:
      summary: Create Call Set
      description: |-
        Creates a new call set.

        For the definitions of call sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.callsets.create
      x-api-path-slug: v1callsets-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Call Set
  /v1/callsets/search:
    post:
      summary: Search Call Sets
      description: |-
        Gets a list of call sets matching the criteria.

        For the definitions of call sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Implements
        [GlobalAllianceApi.searchCallSets](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/variantmethods.avdl#L178).
      operationId: genomics.callsets.search
      x-api-path-slug: v1callsetssearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Call Set
  /v1/callsets/{callSetId}:
    delete:
      summary: Delete Call Set
      description: |-
        Deletes a call set.

        For the definitions of call sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.callsets.delete
      x-api-path-slug: v1callsetscallsetid-delete
      parameters:
      - in: path
        name: callSetId
        description: The ID of the call set to be deleted
      responses:
        200:
          description: OK
      tags:
      - Call Set
    get:
      summary: Get Call Set
      description: |-
        Gets a call set by ID.

        For the definitions of call sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.callsets.get
      x-api-path-slug: v1callsetscallsetid-get
      parameters:
      - in: path
        name: callSetId
        description: The ID of the call set
      responses:
        200:
          description: OK
      tags:
      - Call Set
    patch:
      summary: Update Call Set
      description: |-
        Updates a call set.

        For the definitions of call sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        This method supports patch semantics.
      operationId: genomics.callsets.patch
      x-api-path-slug: v1callsetscallsetid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: callSetId
        description: The ID of the call set to be updated
      - in: query
        name: updateMask
        description: An optional mask specifying which fields to update
      responses:
        200:
          description: OK
      tags:
      - Call Set
  /v1/datasets:
    get:
      summary: Get Datasets
      description: |-
        Lists datasets within a project.

        For the definitions of datasets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.datasets.list
      x-api-path-slug: v1datasets-get
      parameters:
      - in: query
        name: pageSize
        description: The maximum number of results to return in a single page
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: query
        name: projectId
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Dataset
    post:
      summary: Create Dataset
      description: |-
        Creates a new dataset.

        For the definitions of datasets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.datasets.create
      x-api-path-slug: v1datasets-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Dataset
  /v1/datasets/{datasetId}:
    delete:
      summary: Delete Dataset
      description: |-
        Deletes a dataset and all of its contents (all read group sets,
        reference sets, variant sets, call sets, annotation sets, etc.)
        This is reversible (up to one week after the deletion) via
        the
        datasets.undelete
        operation.

        For the definitions of datasets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.datasets.delete
      x-api-path-slug: v1datasetsdatasetid-delete
      parameters:
      - in: path
        name: datasetId
        description: The ID of the dataset to be deleted
      responses:
        200:
          description: OK
      tags:
      - Dataset
    get:
      summary: Get Dataset
      description: |-
        Gets a dataset by ID.

        For the definitions of datasets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.datasets.get
      x-api-path-slug: v1datasetsdatasetid-get
      parameters:
      - in: path
        name: datasetId
        description: The ID of the dataset
      responses:
        200:
          description: OK
      tags:
      - Dataset
    patch:
      summary: Update Dataset
      description: |-
        Updates a dataset.

        For the definitions of datasets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        This method supports patch semantics.
      operationId: genomics.datasets.patch
      x-api-path-slug: v1datasetsdatasetid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: datasetId
        description: The ID of the dataset to be updated
      - in: query
        name: updateMask
        description: An optional mask specifying which fields to update
      responses:
        200:
          description: OK
      tags:
      - Dataset
  /v1/datasets/{datasetId}:undelete:
    post:
      summary: Restore Dataset
      description: |-
        Undeletes a dataset by restoring a dataset which was deleted via this API.

        For the definitions of datasets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        This operation is only possible for a week after the deletion occurred.
      operationId: genomics.datasets.undelete
      x-api-path-slug: v1datasetsdatasetidundelete-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: datasetId
        description: The ID of the dataset to be undeleted
      responses:
        200:
          description: OK
      tags:
      - Dataset
  /v1/readgroupsets/search:
    post:
      summary: Search Read Group Sets
      description: |-
        Searches for read group sets matching the criteria.

        For the definitions of read group sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Implements
        [GlobalAllianceApi.searchReadGroupSets](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/readmethods.avdl#L135).
      operationId: genomics.readgroupsets.search
      x-api-path-slug: v1readgroupsetssearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Read Group Set
  /v1/readgroupsets/{readGroupSetId}:
    delete:
      summary: Delete Read Group Set
      description: |-
        Deletes a read group set.

        For the definitions of read group sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.readgroupsets.delete
      x-api-path-slug: v1readgroupsetsreadgroupsetid-delete
      parameters:
      - in: path
        name: readGroupSetId
        description: The ID of the read group set to be deleted
      responses:
        200:
          description: OK
      tags:
      - Read Group Set
    get:
      summary: Get Read Group Set
      description: |-
        Gets a read group set by ID.

        For the definitions of read group sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.readgroupsets.get
      x-api-path-slug: v1readgroupsetsreadgroupsetid-get
      parameters:
      - in: path
        name: readGroupSetId
        description: The ID of the read group set
      responses:
        200:
          description: OK
      tags:
      - Read Group Set
    patch:
      summary: Update Read Group Set
      description: |-
        Updates a read group set.

        For the definitions of read group sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        This method supports patch semantics.
      operationId: genomics.readgroupsets.patch
      x-api-path-slug: v1readgroupsetsreadgroupsetid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: readGroupSetId
        description: The ID of the read group set to be updated
      - in: query
        name: updateMask
        description: An optional mask specifying which fields to update
      responses:
        200:
          description: OK
      tags:
      - Read Group Set
  /v1/readgroupsets/{readGroupSetId}/coveragebuckets:
    get:
      summary: Get Coverage Buckets for Read Group Set
      description: |-
        Lists fixed width coverage buckets for a read group set, each of which
        correspond to a range of a reference sequence. Each bucket summarizes
        coverage information across its corresponding genomic range.

        For the definitions of read group sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Coverage is defined as the number of reads which are aligned to a given
        base in the reference sequence. Coverage buckets are available at several
        precomputed bucket widths, enabling retrieval of various coverage 'zoom
        levels'. The caller must have READ permissions for the target read group
        set.
      operationId: genomics.readgroupsets.coveragebuckets.list
      x-api-path-slug: v1readgroupsetsreadgroupsetidcoveragebuckets-get
      parameters:
      - in: query
        name: end
        description: The end position of the range on the reference, 0-based exclusive
      - in: query
        name: pageSize
        description: The maximum number of results to return in a single page
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: path
        name: readGroupSetId
        description: Required
      - in: query
        name: referenceName
        description: The name of the reference to query, within the reference set
          associatedwith this query
      - in: query
        name: start
        description: The start position of the range on the reference, 0-based inclusive
      - in: query
        name: targetBucketWidth
        description: The desired width of each reported coverage bucket in base pairs
      responses:
        200:
          description: OK
      tags:
      - Read Group Set
  /v1/readgroupsets/{readGroupSetId}:export:
    post:
      summary: Export Read Group Set
      description: |-
        Exports a read group set to a BAM file in Google Cloud Storage.

        For the definitions of read group sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Note that currently there may be some differences between exported BAM
        files and the original BAM file at the time of import. See
        ImportReadGroupSets
        for caveats.
      operationId: genomics.readgroupsets.export
      x-api-path-slug: v1readgroupsetsreadgroupsetidexport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: readGroupSetId
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Read Group Set
  /v1/readgroupsets:import:
    post:
      summary: Create Read Group Set
      description: |-
        Creates read group sets by asynchronously importing the provided
        information.

        For the definitions of read group sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        The caller must have WRITE permissions to the dataset.

        ## Notes on [BAM](https://samtools.github.io/hts-specs/SAMv1.pdf) import

        - Tags will be converted to strings - tag types are not preserved
        - Comments (`@CO`) in the input file header will not be preserved
        - Original header order of references (`@SQ`) will not be preserved
        - Any reverse stranded unmapped reads will be reverse complemented, and
        their qualities (also the "BQ" and "OQ" tags, if any) will be reversed
        - Unmapped reads will be stripped of positional information (reference name
        and position)
      operationId: genomics.readgroupsets.import
      x-api-path-slug: v1readgroupsetsimport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Read Group Set
  /v1/reads/search:
    post:
      summary: Search Reads
      description: |-
        Gets a list of reads for one or more read group sets.

        For the definitions of read group sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Reads search operates over a genomic coordinate space of reference sequence
        & position defined over the reference sequences to which the requested
        read group sets are aligned.

        If a target positional range is specified, search returns all reads whose
        alignment to the reference genome overlap the range. A query which
        specifies only read group set IDs yields all reads in those read group
        sets, including unmapped reads.

        All reads returned (including reads on subsequent pages) are ordered by
        genomic coordinate (by reference sequence, then position). Reads with
        equivalent genomic coordinates are returned in an unspecified order. This
        order is consistent, such that two queries for the same content (regardless
        of page size) yield reads in the same order across their respective streams
        of paginated responses.

        Implements
        [GlobalAllianceApi.searchReads](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/readmethods.avdl#L85).
      operationId: genomics.reads.search
      x-api-path-slug: v1readssearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Reads
  /v1/references/search:
    post:
      summary: Search References
      description: |-
        Searches for references which match the given criteria.

        For the definitions of references and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Implements
        [GlobalAllianceApi.searchReferences](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/referencemethods.avdl#L146).
      operationId: genomics.references.search
      x-api-path-slug: v1referencessearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Reference
  /v1/references/{referenceId}:
    get:
      summary: Get Reference
      description: |-
        Gets a reference.

        For the definitions of references and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Implements
        [GlobalAllianceApi.getReference](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/referencemethods.avdl#L158).
      operationId: genomics.references.get
      x-api-path-slug: v1referencesreferenceid-get
      parameters:
      - in: path
        name: referenceId
        description: The ID of the reference
      responses:
        200:
          description: OK
      tags:
      - Reference
  /v1/references/{referenceId}/bases:
    get:
      summary: Get Reference Base
      description: |-
        Lists the bases in a reference, optionally restricted to a range.

        For the definitions of references and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Implements
        [GlobalAllianceApi.getReferenceBases](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/referencemethods.avdl#L221).
      operationId: genomics.references.bases.list
      x-api-path-slug: v1referencesreferenceidbases-get
      parameters:
      - in: query
        name: end
        description: The end position (0-based, exclusive) of this query
      - in: query
        name: pageSize
        description: The maximum number of bases to return in a single page
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: path
        name: referenceId
        description: The ID of the reference
      - in: query
        name: start
        description: The start position (0-based) of this query
      responses:
        200:
          description: OK
      tags:
      - Reference
  /v1/referencesets/search:
    post:
      summary: Search Reference Set
      description: |-
        Searches for reference sets which match the given criteria.

        For the definitions of references and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Implements
        [GlobalAllianceApi.searchReferenceSets](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/referencemethods.avdl#L71)
      operationId: genomics.referencesets.search
      x-api-path-slug: v1referencesetssearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Reference Set
  /v1/referencesets/{referenceSetId}:
    get:
      summary: Get Reference Set
      description: |-
        Gets a reference set.

        For the definitions of references and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Implements
        [GlobalAllianceApi.getReferenceSet](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/referencemethods.avdl#L83).
      operationId: genomics.referencesets.get
      x-api-path-slug: v1referencesetsreferencesetid-get
      parameters:
      - in: path
        name: referenceSetId
        description: The ID of the reference set
      responses:
        200:
          description: OK
      tags:
      - Reference Set
  /v1/variants:
    post:
      summary: Create Variant
      description: |-
        Creates a new variant.

        For the definitions of variants and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.variants.create
      x-api-path-slug: v1variants-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Variant
  /v1/variants/search:
    post:
      summary: Get Variants
      description: |-
        Gets a list of variants matching the criteria.

        For the definitions of variants and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Implements
        [GlobalAllianceApi.searchVariants](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/variantmethods.avdl#L126).
      operationId: genomics.variants.search
      x-api-path-slug: v1variantssearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Variant
  /v1/variants/{variantId}:
    delete:
      summary: Delete Variant
      description: |-
        Deletes a variant.

        For the definitions of variants and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.variants.delete
      x-api-path-slug: v1variantsvariantid-delete
      parameters:
      - in: path
        name: variantId
        description: The ID of the variant to be deleted
      responses:
        200:
          description: OK
      tags:
      - Variant
    get:
      summary: Get Variant
      description: |-
        Gets a variant by ID.

        For the definitions of variants and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.variants.get
      x-api-path-slug: v1variantsvariantid-get
      parameters:
      - in: path
        name: variantId
        description: The ID of the variant
      responses:
        200:
          description: OK
      tags:
      - Variant
    patch:
      summary: Update Variant
      description: |-
        Updates a variant.

        For the definitions of variants and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        This method supports patch semantics. Returns the modified variant without
        its calls.
      operationId: genomics.variants.patch
      x-api-path-slug: v1variantsvariantid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: updateMask
        description: An optional mask specifying which fields to update
      - in: path
        name: variantId
        description: The ID of the variant to be updated
      responses:
        200:
          description: OK
      tags:
      - Variant
  /v1/variants:import:
    post:
      summary: Create Variant
      description: |-
        Creates variant data by asynchronously importing the provided information.

        For the definitions of variant sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        The variants for import will be merged with any existing variant that
        matches its reference sequence, start, end, reference bases, and
        alternative bases. If no such variant exists, a new one will be created.

        When variants are merged, the call information from the new variant
        is added to the existing variant, and Variant info fields are merged
        as specified in
        infoMergeConfig.
        As a special case, for single-sample VCF files, QUAL and FILTER fields will
        be moved to the call level; these are sometimes interpreted in a
        call-specific context.
        Imported VCF headers are appended to the metadata already in a variant set.
      operationId: genomics.variants.import
      x-api-path-slug: v1variantsimport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Variant
  /v1/variants:merge:
    post:
      summary: Merge Variants
      description: |-
        Merges the given variants with existing variants.

        For the definitions of variants and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Each variant will be
        merged with an existing variant that matches its reference sequence,
        start, end, reference bases, and alternative bases. If no such variant
        exists, a new one will be created.

        When variants are merged, the call information from the new variant
        is added to the existing variant. Variant info fields are merged as
        specified in the
        infoMergeConfig
        field of the MergeVariantsRequest.

        Please exercise caution when using this method!  It is easy to introduce
        mistakes in existing variants and difficult to back out of them.  For
        example,
        suppose you were trying to merge a new variant with an existing one and
        both
        variants contain calls that belong to callsets with the same callset ID.

            // Existing variant - irrelevant fields trimmed for clarity
            {
                "variantSetId": "10473108253681171589",
                "referenceName": "1",
                "start": "10582",
                "referenceBases": "G",
                "alternateBases": [
                    "A"
                ],
                "calls": [
                    {
                        "callSetId": "10473108253681171589-0",
                        "callSetName": "CALLSET0",
                        "genotype": [
                            0,
                            1
                        ],
                    }
                ]
            }

            // New variant with conflicting call information
            {
                "variantSetId": "10473108253681171589",
                "referenceName": "1",
                "start": "10582",
                "referenceBases": "G",
                "alternateBases": [
                    "A"
                ],
                "calls": [
                    {
                        "callSetId": "10473108253681171589-0",
                        "callSetName": "CALLSET0",
                        "genotype": [
                            1,
                            1
                        ],
                    }
                ]
            }

        The resulting merged variant would overwrite the existing calls with those
        from the new variant:

            {
                "variantSetId": "10473108253681171589",
                "referenceName": "1",
                "start": "10582",
                "referenceBases": "G",
                "alternateBases": [
                    "A"
                ],
                "calls": [
                    {
                        "callSetId": "10473108253681171589-0",
                        "callSetName": "CALLSET0",
                        "genotype": [
                            1,
                            1
                        ],
                    }
                ]
            }

        This may be the desired outcome, but it is up to the user to determine if
        if that is indeed the case.
      operationId: genomics.variants.merge
      x-api-path-slug: v1variantsmerge-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Variant
  /v1/variantsets:
    post:
      summary: Create Variant Set
      description: |-
        Creates a new variant set.

        For the definitions of variant sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        The provided variant set must have a valid `datasetId` set - all other
        fields are optional. Note that the `id` field will be ignored, as this is
        assigned by the server.
      operationId: genomics.variantsets.create
      x-api-path-slug: v1variantsets-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Variant Set
  /v1/variantsets/search:
    post:
      summary: Get Variant Sets
      description: |-
        Returns a list of all variant sets matching search criteria.

        For the definitions of variant sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Implements
        [GlobalAllianceApi.searchVariantSets](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/variantmethods.avdl#L49).
      operationId: genomics.variantsets.search
      x-api-path-slug: v1variantsetssearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Variant Set
  /v1/variantsets/{variantSetId}:
    delete:
      summary: Delete Variant Set
      description: |-
        Deletes a variant set including all variants, call sets, and calls within.
        This is not reversible.

        For the definitions of variant sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.variantsets.delete
      x-api-path-slug: v1variantsetsvariantsetid-delete
      parameters:
      - in: path
        name: variantSetId
        description: The ID of the variant set to be deleted
      responses:
        200:
          description: OK
      tags:
      - Variant Set
    get:
      summary: Get Variant Set
      description: |-
        Gets a variant set by ID.

        For the definitions of variant sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.variantsets.get
      x-api-path-slug: v1variantsetsvariantsetid-get
      parameters:
      - in: path
        name: variantSetId
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Variant Set
    patch:
      summary: Update Variant Set
      description: |-
        Updates a variant set using patch semantics.

        For the definitions of variant sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.variantsets.patch
      x-api-path-slug: v1variantsetsvariantsetid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: updateMask
        description: An optional mask specifying which fields to update
      - in: path
        name: variantSetId
        description: The ID of the variant to be updated (must already exist)
      responses:
        200:
          description: OK
      tags:
      - Variant Set
  /v1/variantsets/{variantSetId}:export:
    post:
      summary: Export Variant Set
      description: |-
        Exports variant set data to an external destination.

        For the definitions of variant sets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.variantsets.export
      x-api-path-slug: v1variantsetsvariantsetidexport-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: variantSetId
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Variant Set
  /v1/{name}:
    get:
      summary: Get Operation
      description: |-
        Gets the latest state of a long-running operation.  Clients can use this
        method to poll the operation result at intervals as recommended by the API
        service.
      operationId: genomics.operations.get
      x-api-path-slug: v1name-get
      parameters:
      - in: path
        name: name
        description: The name of the operation resource
      responses:
        200:
          description: OK
      tags:
      - Operation
  /v1/{name}:cancel:
    post:
      summary: Cancel Operation
      description: Starts asynchronous cancellation on a long-running operation. The
        server makes a best effort to cancel the operation, but success is not guaranteed.
        Clients may use Operations.GetOperation or Operations.ListOperations to check
        whether the cancellation succeeded or the operation completed despite cancellation.
      operationId: genomics.operations.cancel
      x-api-path-slug: v1namecancel-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The name of the operation resource to be cancelled
      responses:
        200:
          description: OK
      tags:
      - Operation
  /v1/{resource}:getIamPolicy:
    post:
      summary: Get IAM Policy
      description: |-
        Gets the access control policy for the dataset. This is empty if the
        policy or resource does not exist.

        See <a href="/iam/docs/managing-policies#getting_a_policy">Getting a
        Policy</a> for more information.

        For the definitions of datasets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.datasets.getIamPolicy
      x-api-path-slug: v1resourcegetiampolicy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which policy is being specified'
      responses:
        200:
          description: OK
      tags:
      - IAM
  /v1/{resource}:setIamPolicy:
    post:
      summary: Set IAM Policy
      description: |-
        Sets the access control policy on the specified dataset. Replaces any
        existing policy.

        For the definitions of datasets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        See <a href="/iam/docs/managing-policies#setting_a_policy">Setting a
        Policy</a> for more information.
      operationId: genomics.datasets.setIamPolicy
      x-api-path-slug: v1resourcesetiampolicy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which policy is being specified'
      responses:
        200:
          description: OK
      tags:
      - IAM
  /v1/{resource}:testIamPermissions:
    post:
      summary: Test IAM Permissions
      description: |-
        Returns permissions that a caller has on the specified resource.
        See <a href="/iam/docs/managing-policies#testing_permissions">Testing
        Permissions</a> for more information.

        For the definitions of datasets and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)
      operationId: genomics.datasets.testIamPermissions
      x-api-path-slug: v1resourcetestiampermissions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which policy is being specified'
      responses:
        200:
          description: OK
      tags:
      - IAM