{
  "info": {
    "name": "Fire Browse Beta API Retrieve miRSeq data.",
    "_postman_id": "3e64aa95-2931-499e-9f74-89c1fa2e3d75",
    "description": "This service returns sample-level log2 miRSeq expression values. Results may be filtered by miR, cohort, barcode, sample type or Firehose preprocessing tool, but at least one miR must be supplied.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Analyses",
      "item": [
        {
          "id": "7d1bba05-5160-4315-baa8-c2fb09b8d51c",
          "name": "getAnalysesCopynumberGenesAll",
          "request": {
            "url": "http://firebrowse.org/api/v1/Analyses/CopyNumber/Genes/All?cohort=%7B%7D&format=%7B%7D&gene=%7B%7D&page=%7B%7D&page_size=%7B%7D&sort_by=%7B%7D&tcga_participant_barcode=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service provides access to the Gistic2 all_data_by_genes.txt output data. This data is a gene-level table of copy number values for all samples. The returned copy number values are in units (copy number - 2) so that no amplification or deletion is 0, genes with amplifications have positive values, and genes with deletions are negative values. The data are converted from marker level to gene level using the extreme method: a gene is assigned the greatest amplification or the least deletion value among the markers it covers. Results may be filtered by cohort, gene, or barcode, but at least one gene or barcode must be supplied."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d066e59-b261-4799-9c49-a9079869e0de"
            }
          ]
        },
        {
          "id": "2edb33a8-62d0-46fa-b52f-b8ddebdf355a",
          "name": "getAnalysesCopynumberGenesAmplified",
          "request": {
            "url": "http://firebrowse.org/api/v1/Analyses/CopyNumber/Genes/Amplified?cohort=%7B%7D&format=%7B%7D&gene=%7B%7D&page=%7B%7D&page_size=%7B%7D&q=%7B%7D&sort_by=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service provides access to the Gistic2 amp_genes.conf_99.txt output data.  At least 1 gene or cohort must be supplied."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa25d441-cc6e-4fe9-9fad-c4fec8b34c1a"
            }
          ]
        },
        {
          "id": "f37e880c-2ad4-447c-806a-efaf8ce564d2",
          "name": "getAnalysesCopynumberGenesDeleted",
          "request": {
            "url": "http://firebrowse.org/api/v1/Analyses/CopyNumber/Genes/Deleted?cohort=%7B%7D&format=%7B%7D&gene=%7B%7D&page=%7B%7D&page_size=%7B%7D&q=%7B%7D&sort_by=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service provides access to the Gistic2 del_genes.conf_99.txt output data.  At least 1 gene or cohort must be supplied."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51f160f1-d6de-42e0-815e-4d3e76528c5e"
            }
          ]
        },
        {
          "id": "f96b8faf-6403-438c-a409-2ebabc8092a5",
          "name": "getAnalysesCopynumberGenesFocal",
          "request": {
            "url": "http://firebrowse.org/api/v1/Analyses/CopyNumber/Genes/Focal?cohort=%7B%7D&format=%7B%7D&gene=%7B%7D&page=%7B%7D&page_size=%7B%7D&sort_by=%7B%7D&tcga_participant_barcode=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service provides access to the Gistic2 focal_data_by_genes.txt output data. This output is similar to the all_data_by_genes.txt output, but using only focal events with lengths greater than the  focal length cutoff. This data is a gene-level table of copy number values for all samples. The returned copy number values are in units (copy number - 2) so that no amplification or deletion is 0, genes with amplifications have positive values, and genes with deletions are negative values. The data are converted from marker level to gene level using the extreme method: a gene is assigned the greatest amplification or the least deletion value among the markers it covers. Results may be filtered by cohort, gene, and/or barcode, but at least one gene or barcode must be supplied."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0100eba4-2481-4f62-b13b-4ea7246273ef"
            }
          ]
        },
        {
          "id": "d7fc6565-0793-41c6-9f1e-6740e5801e5d",
          "name": "getAnalysesCopynumberGenesThresholded",
          "request": {
            "url": "http://firebrowse.org/api/v1/Analyses/CopyNumber/Genes/Thresholded?cohort=%7B%7D&format=%7B%7D&gene=%7B%7D&page=%7B%7D&page_size=%7B%7D&sort_by=%7B%7D&tcga_participant_barcode=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service provides access to the Gistic2 all_thresholded_by_genes.txt output data. A gene-level table of discrete amplification and deletion indicators for all samples. A table value of 0 means no amplification or deletion above the threshold. Amplifications are positive numbers: 1 means amplification above the amplification threshold; 2 means amplifications larger to the arm level amplifications observed for the sample. Deletions are represented by negative table values: -1 represents deletion beyond the threshold; -2 means deletions greater than the minimum arm-level deletion observed for the sample. Results maybe filtered by cohort, gene or barcode, but at least one gene or barcode must be supplied."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66f282c6-b285-476b-82a4-f9df8400ffa7"
            }
          ]
        },
        {
          "id": "ecc64cf5-eda2-4426-8bbb-c035c0fedb15",
          "name": "getAnalysesFeaturetable",
          "request": {
            "url": "http://firebrowse.org/api/v1/Analyses/FeatureTable?cohort=%7B%7D&column=%7B%7D&date=%7B%7D&format=%7B%7D&page=%7B%7D&page_size=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service returns part or all of the so-called feature table; which aggregates the most important findings across ALL pipelines in the GDAC Firehose analysis workflow into a single table for simple access.  One feature table is created per disease cohort.  Results may be filtered by date or cohort, but at least 1 cohort must be specified here. For more details please visit the online documentation.  Please note that the service is still undergoing experimental evaluation and does not return JSON format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37741910-72ca-4aea-b25b-e288e247550f"
            }
          ]
        },
        {
          "id": "7643b39f-2873-4f6c-adf0-a522601c9012",
          "name": "getAnalysesMutationMaf",
          "request": {
            "url": "http://firebrowse.org/api/v1/Analyses/Mutation/MAF?cohort=%7B%7D&column=%7B%7D&format=%7B%7D&gene=%7B%7D&page=%7B%7D&page_size=%7B%7D&sort_by=%7B%7D&tcga_participant_barcode=%7B%7D&tool=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service returns columns from the MAF generated by MutSig. Results may be filtered by gene, cohort, tool, or barcode, but at least one gene OR barcode OR cohort must be given.  By default a subset consisting of the most commonly used columns will be returned, but that can be modified with the column parameter. Specifying 'all' in this parameter is a convenient way to return every column of the respective MAF, and has precedence over any any other column selection expression.  The complete list of column names that may be specified is given here.  For more information on the mutation data, and how it is processed by Firehose, please consult the pipeline documentation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4864204f-00a3-488b-8348-b61f3f6ca658"
            }
          ]
        },
        {
          "id": "41840fc5-8ed9-4b97-9b20-750c263b1b61",
          "name": "getAnalysesMutationSmg",
          "request": {
            "url": "http://firebrowse.org/api/v1/Analyses/Mutation/SMG?cohort=%7B%7D&format=%7B%7D&gene=%7B%7D&page=%7B%7D&page_size=%7B%7D&q=%7B%7D&rank=%7B%7D&sort_by=%7B%7D&tool=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service provides a list of significantly mutated genes, as scored by MutSig.  It may be filtered by cohort, rank, gene, tool and/or Q-value threshold, but at least one cohort or gene must be supplied."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1a15525-6412-4e89-bd27-171c07629cc4"
            }
          ]
        },
        {
          "id": "575bba01-4d0f-412a-9eed-ac0ba33b7e09",
          "name": "getAnalysesReports",
          "request": {
            "url": "http://firebrowse.org/api/v1/Analyses/Reports?cohort=%7B%7D&date=%7B%7D&format=%7B%7D&name=%7B%7D&page=%7B%7D&page_size=%7B%7D&sort_by=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service returns URLs to the analysis result reports for runs of the Broad Institute GDAC Firehose analysis pipeline. At least one year of run reports are maintained in the database, but the reports from the latest run will be returned by default. The set of Nozzle reports returned may be filtered by disease cohort, report type and report name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73b6a10b-3dc1-415c-a38e-b508e16ae19c"
            }
          ]
        },
        {
          "id": "af10a798-9ad2-474b-9a48-750c53fd00c9",
          "name": "getAnalysesMrnaseqQuartiles",
          "request": {
            "url": "http://firebrowse.org/api/v1/Analyses/mRNASeq/Quartiles?cohort=%7B%7D&Exclude=%7B%7D&format=%7B%7D&gene=%7B%7D&protocol=%7B%7D&sample_type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "For a given gene compute quartiles and extrema, suitable e.g. for drawing a boxplot (Tukey 1977).  Results may be filtered by cohort, sample type, patient barcode  or characterization protocol, and are returned sorted by cohort.  Note that samples for which no expression value was recorded (e.g. the melanoma sample TCGA-GN-262) are removed prior to calculation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ea2218c-f494-4a18-9fc4-e3d653b701d2"
            }
          ]
        }
      ]
    },
    {
      "name": "Archives",
      "item": [
        {
          "id": "162ef0d7-10a2-4f5b-bbb7-db1c1e972bad",
          "name": "getArchivesStandarddata",
          "request": {
            "url": "http://firebrowse.org/api/v1/Archives/StandardData?center=%7B%7D&cohort=%7B%7D&data_type=%7B%7D&date=%7B%7D&format=%7B%7D&level=%7B%7D&page=%7B%7D&page_size=%7B%7D&platform=%7B%7D&protocol=%7B%7D&sort_by=%7B%7D&tool=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service returns the archive URLs for our Firehose standard data runs, providing a RESTful interface similar in spirit to the command line firehose_get tool. The archives can be filtered based on date, cohort, data type, platform, center, data level, and protocol."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07e243e6-9923-43c3-9f98-dd4496ed4fd4"
            }
          ]
        }
      ]
    },
    {
      "name": "Metadata",
      "item": [
        {
          "id": "09b08fe7-8fea-4b4a-b8c4-796bb43dabce",
          "name": "getMetadataCenters",
          "request": {
            "url": "http://firebrowse.org/api/v1/Metadata/Centers?center=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "By default this function returns a table of all consortium members in TCGA, aka centers; it provides both the HTTP domain and full organizational name of each center.  A subset of this table may be obtained by explicitly specifying one or more domain names."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28e03702-a46d-4cc7-8b75-b606124daecf"
            }
          ]
        },
        {
          "id": "01cdf21d-928b-4b24-9ce0-3668500185d4",
          "name": "getMetadataClinicalnames",
          "request": {
            "url": "http://firebrowse.org/api/v1/Metadata/ClinicalNames?format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve names of all patient-level clinical data elements (CDES) available in TCGA, unioned across all disease cohorts. A CDE will be listed here only when it has a value other than NA for at least 1 patient case in any disease cohort. For more information on how these CDEs are processed see our pipeline documentation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c638f5cb-fcff-4c43-8d16-af6c58c0010c"
            }
          ]
        },
        {
          "id": "a610b892-d3ad-4c89-b4ca-427077c79e8b",
          "name": "getMetadataClinicalnamesFh",
          "request": {
            "url": "http://firebrowse.org/api/v1/Metadata/ClinicalNames_FH?format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service returns the names of patient-level clinical data elements (CDEs) that have been normalized by Firehose for use in analyses, unioned across all disease cohorts. For more information on how these CDEs are processed, see our pipeline documentation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5075d9cc-2d3f-48eb-a92c-a598b32814c2"
            }
          ]
        },
        {
          "id": "5b95e3bf-8851-42d8-a6ae-915a45694439",
          "name": "getMetadataCohorts",
          "request": {
            "url": "http://firebrowse.org/api/v1/Metadata/Cohorts?cohort=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "By default this function returns a table containing all TCGA cohort abbreviations and their corresponding disease names.  A subset of that table may be obtained by explicitly specifying one or more cohort abbreviations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7cabe9d-70d0-40e8-ade8-1526731fc025"
            }
          ]
        },
        {
          "id": "fabff168-5d33-4edd-96b6-174b91272537",
          "name": "getMetadataCounts",
          "request": {
            "url": "http://firebrowse.org/api/v1/Metadata/Counts?cohort=%7B%7D&data_type=%7B%7D&date=%7B%7D&format=%7B%7D&sample_type=%7B%7D&sort_by=%7B%7D&totals=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the aliquot counts for each disease cohort, per sample\ntype and data type.  The sample type designation of \"Tumor\"\nmay be used to aggregate the count of all tumor aliquots into\na single number per disease and data type. See the SampleTypes\nfunction for a complete description of sample types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7a7f54f-935a-4413-93d4-6c969a23fa73"
            }
          ]
        },
        {
          "id": "05fc3123-8fee-4f0d-bf41-3e9d0096dbd9",
          "name": "getMetadataDates",
          "request": {
            "url": "http://firebrowse.org/api/v1/Metadata/Dates?format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve datestamps of all gdac firehose standard data and analyses runs that have been ingested into firebrowse.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a408843d-84c8-43a7-9489-524bb12c5bd5"
            }
          ]
        },
        {
          "id": "4037fac2-d2ee-4d39-91dc-b55f5406eac1",
          "name": "getMetadataHeartbeat",
          "request": {
            "url": "http://firebrowse.org/api/v1/Metadata/HeartBeat?format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a message to indicate that API (server) is up and running, or times out if not."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "771569ce-4b1b-45f7-bbaa-3db1b4092641"
            }
          ]
        },
        {
          "id": "77c501f9-6457-4b6d-b76a-49eec093b195",
          "name": "getMetadataMafcolnames",
          "request": {
            "url": "http://firebrowse.org/api/v1/Metadata/MAFColNames?format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the names of all columns in the mutation annotation files (MAFs) hosted by FireBrowse.  For more information on the mutation data, and how it is processed by Firehose, please consult the pipeline documentation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "276c5138-fc74-4fbc-b3db-33ed9969cb05"
            }
          ]
        },
        {
          "id": "b4dfcb5f-a769-4af1-a0a5-92db0aed99b9",
          "name": "getMetadataPatients",
          "request": {
            "url": "http://firebrowse.org/api/v1/Metadata/Patients?cohort=%7B%7D&format=%7B%7D&page=%7B%7D&page_size=%7B%7D&sort_by=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service returns a list of all TCGA patient barcodes in FireBrowse, optionally filtered by disease cohort.  The barcodes are obtained directy from the clinical data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6feba5b-9f07-4905-957f-a42b8ce1121c"
            }
          ]
        },
        {
          "id": "6a53674a-0273-4a52-82d4-4c347e1d0e0b",
          "name": "getMetadataPlatforms",
          "request": {
            "url": "http://firebrowse.org/api/v1/Metadata/Platforms?format=%7B%7D&platform=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "By default this function returns a table of all of the technology platforms used to sequence or characterize samples in TCGA--both their short platform codes and full names.  A subset of this table may be obtained by explicitly specifying one or more platform codes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b46e45f0-c00c-4dbd-961a-c85a016485c1"
            }
          ]
        },
        {
          "id": "f2d1b7f9-3588-4cfe-b15b-b09c001221c4",
          "name": "getMetadataSampletypeBarcodeTcgaBarcode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "firebrowse.org",
              "path": [
                "api",
                "v1",
                "Metadata/SampleType/Barcode/:TCGA_Barcode"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "TCGA_Barcode",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a tcga barcode, return its short letter sample type code.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55c8c864-9bef-4b79-bdf2-611b3a023939"
            }
          ]
        },
        {
          "id": "a0b491a2-7cff-4902-b8ed-16386d86b01a",
          "name": "getMetadataSampletypeCodeCode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "firebrowse.org",
              "path": [
                "api",
                "v1",
                "Metadata/SampleType/Code/:code"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Convert a TCGA numeric sample type code (e.g. 01, 02) to its corresponding symbolic (short letter) code (e.g. TP, TR)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c7a3cf7-daa3-421b-9ed3-52869eeb8eab"
            }
          ]
        },
        {
          "id": "58eda2a8-ca2c-49aa-a378-dcf6c1653363",
          "name": "getMetadataSampletypeShortlettercodeShortLetterCode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "firebrowse.org",
              "path": [
                "api",
                "v1",
                "Metadata/SampleType/ShortLetterCode/:short_letter_code"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "short_letter_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Convert a TCGA sample type code in symbolic form (or 'short letter code' like TP, TR) to its corresponding numeric form (e.g. 01, 02)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a418abc1-f614-4247-9c38-c0a6832280a7"
            }
          ]
        },
        {
          "id": "9124c288-2cae-449e-aa15-bdc82d820ece",
          "name": "getMetadataSampletypes",
          "request": {
            "url": "http://firebrowse.org/api/v1/Metadata/SampleTypes?format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return all tcga sample type codes, both numeric and symbolic.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15001858-2868-4792-8bbf-fd13c7fd3124"
            }
          ]
        },
        {
          "id": "93751df6-9a40-4e6d-b0cb-352297a38b78",
          "name": "getMetadataTssites",
          "request": {
            "url": "http://firebrowse.org/api/v1/Metadata/TSSites?format=%7B%7D&tss_code=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "By default this function returns a table of all sites which contributed source tissue to TCGA, aka TSS's. A subset of this table may be obtained by explicitly specifying one or more sites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd577783-3c74-4293-94de-205785f3190c"
            }
          ]
        }
      ]
    },
    {
      "name": "Samples",
      "item": [
        {
          "id": "c3d739bc-f4aa-4d13-bba1-44bf34d9f784",
          "name": "getSamplesClinical",
          "request": {
            "url": "http://firebrowse.org/api/v1/Samples/Clinical?cde_name=%7B%7D&cohort=%7B%7D&format=%7B%7D&page=%7B%7D&page_size=%7B%7D&sort_by=%7B%7D&tcga_participant_barcode=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service returns patient clinical data from TCGA, verbatim. It differs from the Samples/Clinical_FH method by providing access to all TCGA CDEs in their original form, not merely the subset of CDEs normalized by Firehose for analyses.  Results may be selected by disease cohort, patient barcode or CDE name, but at least one cohort, barcode, or CDE must be provided. When filtering by CDE note that only when a patient record contains one or more of the selected CDEs will it be returned. Visit the Metadata/ClinicalNames api function to see the entire list of TCGA CDEs that may be queried via this method. For more information on how clinical data are processed, see our pipeline documentation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bae4e792-7a44-454a-8c68-d4f7664f5636"
            }
          ]
        },
        {
          "id": "55c08ba9-6921-4a35-a8e4-f3c325bb807c",
          "name": "getSamplesClinicalFh",
          "request": {
            "url": "http://firebrowse.org/api/v1/Samples/Clinical_FH?cohort=%7B%7D&fh_cde_name=%7B%7D&format=%7B%7D&page=%7B%7D&page_size=%7B%7D&sort_by=%7B%7D&tcga_participant_barcode=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service returns patient-level clinical data elements (CDEs) that have been normalized by Firehose for use in analyses. Results may be selected by disease cohort, patient barcode or CDE name, but at least one cohort, barcode or CDE must be provided. When filtering by CDE note that only when a  patient record contains one or more of the selected CDEs will it be returned. Visit this table of CDEs to see what's available for every disase cohort; for more information on how these CDEs are processed see our pipeline documentation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb0baec5-1aef-4fcd-b8f8-be81d7a7aa3d"
            }
          ]
        },
        {
          "id": "c8786422-aa33-42fd-8a46-0907bc95db5c",
          "name": "getSamplesMrnaseq",
          "request": {
            "url": "http://firebrowse.org/api/v1/Samples/mRNASeq?cohort=%7B%7D&format=%7B%7D&gene=%7B%7D&page=%7B%7D&page_size=%7B%7D&protocol=%7B%7D&sample_type=%7B%7D&sort_by=%7B%7D&tcga_participant_barcode=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service returns sample-level log2 mRNASeq expression values. Results may be filtered by gene, cohort, barcode, sample type or characterization protocol, but at least one gene must be supplied."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59bfd64d-127f-4880-bfc9-6b3bc07c02e7"
            }
          ]
        },
        {
          "id": "21192b91-2173-4ece-956b-7b738af69aab",
          "name": "getSamplesMirseq",
          "request": {
            "url": "http://firebrowse.org/api/v1/Samples/miRSeq?cohort=%7B%7D&format=%7B%7D&mir=%7B%7D&page=%7B%7D&page_size=%7B%7D&sample_type=%7B%7D&sort_by=%7B%7D&tcga_participant_barcode=%7B%7D&tool=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This service returns sample-level log2 miRSeq expression values. Results may be filtered by miR, cohort, barcode, sample type or Firehose preprocessing tool, but at least one miR must be supplied."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7d490d5-069c-4708-9c16-b07b3db82cfe"
            }
          ]
        }
      ]
    }
  ]
}