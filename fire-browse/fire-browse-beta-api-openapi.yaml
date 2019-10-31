swagger: "2.0"
x-collection-name: Fire Browse
x-complete: 1
info:
  title: Fire Browse Beta API
  description: a-simple-and-elegant-way-to-explore-cancer-data
  version: 1.1.35 (2016-09-27 10:12:23 6a47e74011281b2aa
host: firebrowse.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Analyses/CopyNumber/Genes/All:
    get:
      summary: Retrieve all data by genes Gistic2 results.
      description: 'This service provides access to the Gistic2 all_data_by_genes.txt
        output data. This data is a gene-level table of copy number values for all
        samples. The returned copy number values are in units (copy number - 2) so
        that no amplification or deletion is 0, genes with amplifications have positive
        values, and genes with deletions are negative values. The data are converted
        from marker level to gene level using the extreme method: a gene is assigned
        the greatest amplification or the least deletion value among the markers it
        covers. Results may be filtered by cohort, gene, or barcode, but at least
        one gene or barcode must be supplied.'
      operationId: getAnalysesCopynumberGenesAll
      x-api-path-slug: analysescopynumbergenesall-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: gene
        description: Comma separated list of gene name(s)
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: tcga_participant_barcode
        description: Comma separated list of TCGA participant barcodes (e
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - CopyNumber
      - Genes
  /Analyses/CopyNumber/Genes/Amplified:
    get:
      summary: Retrieve Gistic2 significantly amplified genes results.
      description: This service provides access to the Gistic2 amp_genes.conf_99.txt
        output data.  At least 1 gene or cohort must be supplied.
      operationId: getAnalysesCopynumberGenesAmplified
      x-api-path-slug: analysescopynumbergenesamplified-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: gene
        description: Comma separated list of gene name(s)
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: q
        description: Only return results with Q-value
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - CopyNumber
      - Genes
      - Amplified
  /Analyses/CopyNumber/Genes/Deleted:
    get:
      summary: Retrieve Gistic2 significantly deleted genes results.
      description: This service provides access to the Gistic2 del_genes.conf_99.txt
        output data.  At least 1 gene or cohort must be supplied.
      operationId: getAnalysesCopynumberGenesDeleted
      x-api-path-slug: analysescopynumbergenesdeleted-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: gene
        description: Comma separated list of gene name(s)
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: q
        description: Only return results with Q-value
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - CopyNumber
      - Genes
      - D
  /Analyses/CopyNumber/Genes/Focal:
    get:
      summary: Retrieve focal data by genes Gistic2 results.
      description: 'This service provides access to the Gistic2 focal_data_by_genes.txt
        output data. This output is similar to the all_data_by_genes.txt output, but
        using only focal events with lengths greater than the  focal length cutoff.
        This data is a gene-level table of copy number values for all samples. The
        returned copy number values are in units (copy number - 2) so that no amplification
        or deletion is 0, genes with amplifications have positive values, and genes
        with deletions are negative values. The data are converted from marker level
        to gene level using the extreme method: a gene is assigned the greatest amplification
        or the least deletion value among the markers it covers. Results may be filtered
        by cohort, gene, and/or barcode, but at least one gene or barcode must be
        supplied.'
      operationId: getAnalysesCopynumberGenesFocal
      x-api-path-slug: analysescopynumbergenesfocal-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: gene
        description: Comma separated list of gene name(s)
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: tcga_participant_barcode
        description: Comma separated list of TCGA participant barcodes (e
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - CopyNumber
      - Genes
      - Focal
  /Analyses/CopyNumber/Genes/Thresholded:
    get:
      summary: Retrieve all thresholded by genes Gistic2 results.
      description: 'This service provides access to the Gistic2 all_thresholded_by_genes.txt
        output data. A gene-level table of discrete amplification and deletion indicators
        for all samples. A table value of 0 means no amplification or deletion above
        the threshold. Amplifications are positive numbers: 1 means amplification
        above the amplification threshold; 2 means amplifications larger to the arm
        level amplifications observed for the sample. Deletions are represented by
        negative table values: -1 represents deletion beyond the threshold; -2 means
        deletions greater than the minimum arm-level deletion observed for the sample.
        Results maybe filtered by cohort, gene or barcode, but at least one gene or
        barcode must be supplied.'
      operationId: getAnalysesCopynumberGenesThresholded
      x-api-path-slug: analysescopynumbergenesthresholded-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: gene
        description: Comma separated list of gene name(s)
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: tcga_participant_barcode
        description: Comma separated list of TCGA participant barcodes (e
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - CopyNumber
      - Genes
      - Thresholded
  /Analyses/FeatureTable:
    get:
      summary: Retrieve aggregated analysis features table.
      description: This service returns part or all of the so-called feature table;
        which aggregates the most important findings across ALL pipelines in the GDAC
        Firehose analysis workflow into a single table for simple access.  One feature
        table is created per disease cohort.  Results may be filtered by date or cohort,
        but at least 1 cohort must be specified here. For more details please visit
        the online documentation.  Please note that the service is still undergoing
        experimental evaluation and does not return JSON format.
      operationId: getAnalysesFeaturetable
      x-api-path-slug: analysesfeaturetable-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: column
        description: Comma separated list of which data columns/fields to return
      - in: query
        name: date
        description: Select one or more date stamps
      - in: query
        name: format
        description: Format of result
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - FeatureTable
  /Analyses/Mutation/MAF:
    get:
      summary: Retrieve MutSig final analysis MAF.
      description: This service returns columns from the MAF generated by MutSig.
        Results may be filtered by gene, cohort, tool, or barcode, but at least one
        gene OR barcode OR cohort must be given.  By default a subset consisting of
        the most commonly used columns will be returned, but that can be modified
        with the column parameter. Specifying 'all' in this parameter is a convenient
        way to return every column of the respective MAF, and has precedence over
        any any other column selection expression.  The complete list of column names
        that may be specified is given here.  For more information on the mutation
        data, and how it is processed by Firehose, please consult the pipeline documentation.
      operationId: getAnalysesMutationMaf
      x-api-path-slug: analysesmutationmaf-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: column
        description: Comma separated list of which data columns/fields to return
      - in: query
        name: format
        description: Format of result
      - in: query
        name: gene
        description: Comma separated list of gene name(s)
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: tcga_participant_barcode
        description: Comma separated list of TCGA participant barcodes (e
      - in: query
        name: tool
        description: Narrow search to include only data/results produced by the selected
          Firehose tool
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Mutation
      - MAF
  /Analyses/Mutation/SMG:
    get:
      summary: Retrieve Significantly Mutated Genes (SMG).
      description: This service provides a list of significantly mutated genes, as
        scored by MutSig.  It may be filtered by cohort, rank, gene, tool and/or Q-value
        threshold, but at least one cohort or gene must be supplied.
      operationId: getAnalysesMutationSmg
      x-api-path-slug: analysesmutationsmg-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: gene
        description: Comma separated list of gene name(s)
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: q
        description: Only return results with Q-value
      - in: query
        name: rank
        description: Number of significant genes to return
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: tool
        description: Narrow search to include only data/results produced by the selected
          Firehose tool
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Mutation
      - SMG
  /Analyses/Reports:
    get:
      summary: Retrieve links to summary reports from Firehose analysis runs.
      description: This service returns URLs to the analysis result reports for runs
        of the Broad Institute GDAC Firehose analysis pipeline. At least one year
        of run reports are maintained in the database, but the reports from the latest
        run will be returned by default. The set of Nozzle reports returned may be
        filtered by disease cohort, report type and report name.
      operationId: getAnalysesReports
      x-api-path-slug: analysesreports-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: date
        description: Select one or more date stamps
      - in: query
        name: format
        description: Format of result
      - in: query
        name: name
        description: Narrow search to one or more report names
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: type
        description: Narrow search to one or more report types
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - Reports
  /Analyses/mRNASeq/Quartiles:
    get:
      summary: Returns RNASeq expression quartiles, e.g. suitable for drawing a boxplot.
      description: For a given gene compute quartiles and extrema, suitable e.g. for
        drawing a boxplot (Tukey 1977).  Results may be filtered by cohort, sample
        type, patient barcode  or characterization protocol, and are returned sorted
        by cohort.  Note that samples for which no expression value was recorded (e.g.
        the melanoma sample TCGA-GN-262) are removed prior to calculation.
      operationId: getAnalysesMrnaseqQuartiles
      x-api-path-slug: analysesmrnaseqquartiles-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: Exclude
        description: Comma separated list of TCGA participants, identified by barcodes
          such as TCGA-GF-A4EO, denoting samples to exclude from computation
      - in: query
        name: format
        description: Format of result
      - in: query
        name: gene
        description: Enter a single gene name
      - in: query
        name: protocol
        description: Narrow search to one or more sample characterization protocols
          from the scrollable list
      - in: query
        name: sample_type
        description: For which type of sample(s) should quartiles be computed?
      responses:
        200:
          description: OK
      tags:
      - Analyses
      - MRNASeq
      - Quartiles
  /Archives/StandardData:
    get:
      summary: Retrieve standard data archives.
      description: This service returns the archive URLs for our Firehose standard
        data runs, providing a RESTful interface similar in spirit to the command
        line firehose_get tool. The archives can be filtered based on date, cohort,
        data type, platform, center, data level, and protocol.
      operationId: getArchivesStandarddata
      x-api-path-slug: archivesstandarddata-get
      parameters:
      - in: query
        name: center
        description: Narrow search to one or more TCGA centers from the scrollable
          list
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: data_type
        description: Narrow search to one or more TCGA data types from the scrollable
          list
      - in: query
        name: date
        description: Select one or more date stamps
      - in: query
        name: format
        description: Format of result
      - in: query
        name: level
        description: Narrow search to one or more TCGA data levels
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: platform
        description: Narrow search to one or more TCGA data generation platforms from
          the scrollable list
      - in: query
        name: protocol
        description: Narrow search to one or more sample characterization protocols
          from the scrollable list
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: tool
        description: Narrow search to include only data/results produced by the selected
          Firehose tool
      responses:
        200:
          description: OK
      tags:
      - Archives
      - StandardData
  /Metadata/Centers:
    get:
      summary: Obtain identities of TCGA consortium member centers.
      description: By default this function returns a table of all consortium members
        in TCGA, aka centers; it provides both the HTTP domain and full organizational
        name of each center.  A subset of this table may be obtained by explicitly
        specifying one or more domain names.
      operationId: getMetadataCenters
      x-api-path-slug: metadatacenters-get
      parameters:
      - in: query
        name: center
        description: Narrow search to one or more TCGA centers from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Centers
  /Metadata/ClinicalNames:
    get:
      summary: Retrieve names of all TCGA clinical data elements (CDEs).
      description: Retrieve names of all patient-level clinical data elements (CDES)
        available in TCGA, unioned across all disease cohorts. A CDE will be listed
        here only when it has a value other than NA for at least 1 patient case in
        any disease cohort. For more information on how these CDEs are processed see
        our pipeline documentation.
      operationId: getMetadataClinicalnames
      x-api-path-slug: metadataclinicalnames-get
      parameters:
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - ClinicalNames
  /Metadata/ClinicalNames_FH:
    get:
      summary: Retrieve names of CDEs normalized by Firehose and selected for analyses.
      description: This service returns the names of patient-level clinical data elements
        (CDEs) that have been normalized by Firehose for use in analyses, unioned
        across all disease cohorts. For more information on how these CDEs are processed,
        see our pipeline documentation.
      operationId: getMetadataClinicalnamesFh
      x-api-path-slug: metadataclinicalnames-fh-get
      parameters:
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - ClinicalNames
      - FH
  /Metadata/Cohorts:
    get:
      summary: Translate TCGA cohort abbreviations to full disease names.
      description: By default this function returns a table containing all TCGA cohort
        abbreviations and their corresponding disease names.  A subset of that table
        may be obtained by explicitly specifying one or more cohort abbreviations.
      operationId: getMetadataCohorts
      x-api-path-slug: metadatacohorts-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Cohorts
  /Metadata/Counts:
    get:
      summary: Retrieve sample counts.
      description: |-
        Returns the aliquot counts for each disease cohort, per sample
        type and data type.  The sample type designation of "Tumor"
        may be used to aggregate the count of all tumor aliquots into
        a single number per disease and data type. See the SampleTypes
        function for a complete description of sample types.
      operationId: getMetadataCounts
      x-api-path-slug: metadatacounts-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: data_type
        description: Narrow search to one or more TCGA data types from the scrollable
          list
      - in: query
        name: date
        description: Select one or more date stamps
      - in: query
        name: format
        description: Format of result
      - in: query
        name: sample_type
        description: Narrow search to one or more TCGA sample types from the scrollable
          list
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: totals
        description: Output an entry providing the totals for each data type
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Counts
  /Metadata/Dates:
    get:
      summary: Retrieve datestamps of all GDAC Firehose standard data and analyses
        runs that have been ingested into FireBrowse.
      description: Retrieve datestamps of all gdac firehose standard data and analyses
        runs that have been ingested into firebrowse..
      operationId: getMetadataDates
      x-api-path-slug: metadatadates-get
      parameters:
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Dates
  /Metadata/HeartBeat:
    get:
      summary: Simple way to discern whether API server is up and running
      description: Returns a message to indicate that API (server) is up and running,
        or times out if not.
      operationId: getMetadataHeartbeat
      x-api-path-slug: metadataheartbeat-get
      parameters:
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - HeartBeat
  /Metadata/MAFColNames:
    get:
      summary: Retrieve names of all columns in the mutation annotation files (MAFs)
        served by FireBrowse.
      description: Retrieve the names of all columns in the mutation annotation files
        (MAFs) hosted by FireBrowse.  For more information on the mutation data, and
        how it is processed by Firehose, please consult the pipeline documentation.
      operationId: getMetadataMafcolnames
      x-api-path-slug: metadatamafcolnames-get
      parameters:
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - MAFColNames
  /Metadata/Patients:
    get:
      summary: Retrieve list of all TCGA patients.
      description: This service returns a list of all TCGA patient barcodes in FireBrowse,
        optionally filtered by disease cohort.  The barcodes are obtained directy
        from the clinical data.
      operationId: getMetadataPatients
      x-api-path-slug: metadatapatients-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Patients
  /Metadata/Platforms:
    get:
      summary: Translate TCGA platform codes to full platform names.
      description: By default this function returns a table of all of the technology
        platforms used to sequence or characterize samples in TCGA--both their short
        platform codes and full names.  A subset of this table may be obtained by
        explicitly specifying one or more platform codes.
      operationId: getMetadataPlatforms
      x-api-path-slug: metadataplatforms-get
      parameters:
      - in: query
        name: format
        description: Format of result
      - in: query
        name: platform
        description: Narrow search to one or more TCGA data generation platforms from
          the scrollable list
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - Platforms
  /Metadata/SampleType/Barcode/{TCGA_Barcode}:
    get:
      summary: Given a TCGA barcode, return its short letter sample type code.
      description: Given a tcga barcode, return its short letter sample type code..
      operationId: getMetadataSampletypeBarcodeTcgaBarcode
      x-api-path-slug: metadatasampletypebarcodetcga-barcode-get
      parameters:
      - in: query
        name: format
        description: Format of result
      - in: path
        name: TCGA_Barcode
        description: 'Enter a single TCGA barcode, of any form: e'
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - SampleType
      - Barcode
      - TCGA
      - Barcode
  /Metadata/SampleType/Code/{code}:
    get:
      summary: Translate from numeric to symbolic TCGA sample codes.
      description: Convert a TCGA numeric sample type code (e.g. 01, 02) to its corresponding
        symbolic (short letter) code (e.g. TP, TR).
      operationId: getMetadataSampletypeCodeCode
      x-api-path-slug: metadatasampletypecodecode-get
      parameters:
      - in: path
        name: code
        description: Narrow search to one or more TCGA sample type codes
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - SampleType
      - Code
      - Code
  /Metadata/SampleType/ShortLetterCode/{short_letter_code}:
    get:
      summary: Translate from symbolic to numeric TCGA sample codes.
      description: Convert a TCGA sample type code in symbolic form (or 'short letter
        code' like TP, TR) to its corresponding numeric form (e.g. 01, 02).
      operationId: getMetadataSampletypeShortlettercodeShortLetterCode
      x-api-path-slug: metadatasampletypeshortlettercodeshort-letter-code-get
      parameters:
      - in: query
        name: format
        description: Format of result
      - in: path
        name: short_letter_code
        description: TCGA sample type short letter code(s) (e
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - SampleType
      - ShortLetterCode
      - Short
      - Letter
      - Code
  /Metadata/SampleTypes:
    get:
      summary: Return all TCGA sample type codes, both numeric and symbolic.
      description: Return all tcga sample type codes, both numeric and symbolic..
      operationId: getMetadataSampletypes
      x-api-path-slug: metadatasampletypes-get
      parameters:
      - in: query
        name: format
        description: Format of result
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - SampleTypes
  /Metadata/TSSites:
    get:
      summary: Obtain identities of tissue source sites in TCGA.
      description: By default this function returns a table of all sites which contributed
        source tissue to TCGA, aka TSS's. A subset of this table may be obtained by
        explicitly specifying one or more sites.
      operationId: getMetadataTssites
      x-api-path-slug: metadatatssites-get
      parameters:
      - in: query
        name: format
        description: Format of result
      - in: query
        name: tss_code
        description: Narrow search to one or more TSS codes
      responses:
        200:
          description: OK
      tags:
      - Metadata
      - TSSites
  /Samples/Clinical:
    get:
      summary: Retrieve TCGA CDEs verbatim, i.e. not normalized by Firehose.
      description: This service returns patient clinical data from TCGA, verbatim.
        It differs from the Samples/Clinical_FH method by providing access to all
        TCGA CDEs in their original form, not merely the subset of CDEs normalized
        by Firehose for analyses.  Results may be selected by disease cohort, patient
        barcode or CDE name, but at least one cohort, barcode, or CDE must be provided.
        When filtering by CDE note that only when a patient record contains one or
        more of the selected CDEs will it be returned. Visit the Metadata/ClinicalNames
        api function to see the entire list of TCGA CDEs that may be queried via this
        method. For more information on how clinical data are processed, see our pipeline
        documentation.
      operationId: getSamplesClinical
      x-api-path-slug: samplesclinical-get
      parameters:
      - in: query
        name: cde_name
        description: Retrieve results only for specified CDEs, per the Metadata/ClinicalNames
          function
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: tcga_participant_barcode
        description: Comma separated list of TCGA participant barcodes (e
      responses:
        200:
          description: OK
      tags:
      - Samples
      - Clinical
  /Samples/Clinical_FH:
    get:
      summary: Retrieve CDEs normalized by Firehose and selected for analyses.
      description: This service returns patient-level clinical data elements (CDEs)
        that have been normalized by Firehose for use in analyses. Results may be
        selected by disease cohort, patient barcode or CDE name, but at least one
        cohort, barcode or CDE must be provided. When filtering by CDE note that only
        when a  patient record contains one or more of the selected CDEs will it be
        returned. Visit this table of CDEs to see what's available for every disase
        cohort; for more information on how these CDEs are processed see our pipeline
        documentation.
      operationId: getSamplesClinicalFh
      x-api-path-slug: samplesclinical-fh-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: fh_cde_name
        description: Retrieve results only for the CDEs specified from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: tcga_participant_barcode
        description: Comma separated list of TCGA participant barcodes (e
      responses:
        200:
          description: OK
      tags:
      - Samples
      - Clinical
      - FH
  /Samples/mRNASeq:
    get:
      summary: Retrieve mRNASeq data.
      description: This service returns sample-level log2 mRNASeq expression values.
        Results may be filtered by gene, cohort, barcode, sample type or characterization
        protocol, but at least one gene must be supplied.
      operationId: getSamplesMrnaseq
      x-api-path-slug: samplesmrnaseq-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: gene
        description: Comma separated list of gene name(s)
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: protocol
        description: Narrow search to one or more sample characterization protocols
          from the scrollable list
      - in: query
        name: sample_type
        description: Narrow search to one or more TCGA sample types from the scrollable
          list
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: tcga_participant_barcode
        description: Comma separated list of TCGA participant barcodes (e
      responses:
        200:
          description: OK
      tags:
      - Samples
      - MRNASeq
  /Samples/miRSeq:
    get:
      summary: Retrieve miRSeq data.
      description: This service returns sample-level log2 miRSeq expression values.
        Results may be filtered by miR, cohort, barcode, sample type or Firehose preprocessing
        tool, but at least one miR must be supplied.
      operationId: getSamplesMirseq
      x-api-path-slug: samplesmirseq-get
      parameters:
      - in: query
        name: cohort
        description: Narrow search to one or more TCGA disease cohorts from the scrollable
          list
      - in: query
        name: format
        description: Format of result
      - in: query
        name: mir
        description: Comma separated list of miR names (e
      - in: query
        name: page
        description: Which page (slice) of entire results set should be returned
      - in: query
        name: page_size
        description: Number of records per page of results
      - in: query
        name: sample_type
        description: Narrow search to one or more TCGA sample types from the scrollable
          list
      - in: query
        name: sort_by
        description: Which column in the results should be used for sorting paginated
          results?
      - in: query
        name: tcga_participant_barcode
        description: Comma separated list of TCGA participant barcodes (e
      - in: query
        name: tool
        description: Narrow search to include only data/results produced by the selected
          Firehose tool
      responses:
        200:
          description: OK
      tags:
      - Samples
      - MiRSeq