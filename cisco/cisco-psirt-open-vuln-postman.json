{
  "info": {
    "name": "Cisco PSIRT open Vuln Get Security Advisories Oval Severity Severity Lastpublished",
    "_postman_id": "0d9f4d65-f472-4c60-95cd-ccc4929d48bc",
    "description": "Used to obtain all security advisories for a given security impact rating (critical, high, medium, or low) in OVAL format.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Security",
      "item": [
        {
          "id": "d39d6c9c-111e-44cd-a3ef-9df0aadf16d5",
          "name": "used-to-obtain-an-advisory-in-cvrf-format-for-a-given-advisory-id-advisory-id-i-e--ciscosa20150819pc",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/cvrf/advisory/:advisory_id"
              ],
              "variable": [
                {
                  "id": "advisory_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain an advisory in CVRF format for a given advisory ID `advisory_id` (i.e., cisco-sa-20150819-pcp)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1542ce3-809d-41e8-b563-20275a1e3597"
            }
          ]
        },
        {
          "id": "712bdf58-8ecf-4132-b90b-f182b721aa3c",
          "name": "used-to-obtain-all-advisories-in-common-vulnerability-reporting-format-cvrf--for-more-information-ab",
          "request": {
            "url": "http://api.cisco.com/security/advisories/cvrf/all",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all advisories in Common Vulnerability Reporting Format (CVRF). For more information about CVRF go to https://communities.cisco.com/docs/DOC-63156 . By default the output is in JSON. To obtain the output in XML use the .xml extension. For example, /advisories/cvrf/all.xml"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a55b8edc-5b9c-4c1f-b52b-bbe343729b9f"
            }
          ]
        },
        {
          "id": "ab8a3b3e-7eaa-46fb-ba96-cdccafd4f8b4",
          "name": "used-to-obtain-an-advisory-in-cvrf-format-for-a-given-common-vulnerability-enumerator-cve--the-cve-i",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/cvrf/cve/:cve_id"
              ],
              "variable": [
                {
                  "id": "cve_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain an advisory in CVRF format for a given Common Vulnerability Enumerator (CVE). The `cve_id` format is CVE-YYYY-NNNN. For more information about CVE visit http://cve.mitre.org/"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d24c3d96-a5cd-4c9e-be35-3e9ed0c145a4"
            }
          ]
        },
        {
          "id": "c66ac3a0-b7c9-46e3-92e5-8b9ce12f4ebb",
          "name": "used-to-obtain-all-the-latest-security-advisories-in-cvrf-format-given-an-absolute-number--for-insta",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/cvrf/latest/:number"
              ],
              "variable": [
                {
                  "id": "number",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all the latest security advisories in CVRF format given an absolute number. For instance, the latest 10 or latest 5."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2edc76f6-a1e4-4872-962e-654f8fea5875"
            }
          ]
        },
        {
          "id": "f2c1542d-b93d-47fc-8c48-781046f18584",
          "name": "used-to-obtain-all-the-advisories-that-affects-the-given-product-name-",
          "request": {
            "url": "http://api.cisco.com/security/advisories/cvrf/product?product=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all the advisories that affects the given product name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7fe38b3a-62c3-4ced-91dd-bf07bc190930"
            }
          ]
        },
        {
          "id": "c77d4515-d98f-4e9c-9e1d-185160cf3b2d",
          "name": "used-to-obtain-all-security-advisories-for-a-given-security-impact-rating-critical-high-medium-or-lo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/cvrf/severity/:severity"
              ],
              "variable": [
                {
                  "id": "severity",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all security advisories for a given security impact rating (critical, high, medium, or low) in CVRF format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f388d682-67c6-4d79-bb55-8c93d832cabc"
            }
          ]
        },
        {
          "id": "844d5653-ebff-45e0-94ef-a5d735c7c6f3",
          "name": "used-to-obtain-all-security-advisories-for-a-given-security-impact-rating-critical-high-medium-or-lo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/cvrf/severity/:severity/firstpublished"
              ],
              "query": [
                {
                  "key": "endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startDate",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "severity",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all security advisories for a given security impact rating (critical, high, medium, or low) in CVRF format and additionally filter based of firstpublished start date and enddate"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed0e0614-51e5-4a00-b849-52b354b03f20"
            }
          ]
        },
        {
          "id": "2427ad9e-62d9-4f00-b4f4-28d330f5993c",
          "name": "used-to-obtain-all-security-advisories-for-a-given-security-impact-rating-critical-high-medium-or-lo1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/cvrf/severity/:severity/lastpublished"
              ],
              "query": [
                {
                  "key": "endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startDate",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "severity",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all security advisories for a given security impact rating (critical, high, medium, or low) in CVRF format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9cab575e-00f1-4ff9-884d-b74ec4996284"
            }
          ]
        },
        {
          "id": "4538712e-c438-4509-abd5-fb7682b35a80",
          "name": "used-to-obtain-all-security-advisories-that-have-were-orginally-published-in-a-specific-year-yyyy-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/cvrf/year/:year"
              ],
              "variable": [
                {
                  "id": "year",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all security advisories that have were orginally published in a specific year `YYYY`."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00a96daf-ffce-466c-8da8-bbfc1f8c2ac7"
            }
          ]
        },
        {
          "id": "25be99b5-c5be-4b3a-8c4c-e77c54a763c2",
          "name": "used-to-obtain-all-advisories-that-affects-the-given-ios-version",
          "request": {
            "url": "http://api.cisco.com/security/advisories/ios?version=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all advisories that affects the given ios version"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a4d8703-302c-428a-9dd3-0054a8279273"
            }
          ]
        },
        {
          "id": "9319bfda-0bde-4eda-b3a9-7f27f9780ca4",
          "name": "used-to-obtain-all-advisories-that-affects-the-given-ios-version1",
          "request": {
            "url": "http://api.cisco.com/security/advisories/iosxe?version=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all advisories that affects the given ios version"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f581301-8f58-4979-83b3-afc45b6c209c"
            }
          ]
        },
        {
          "id": "7a26f3ac-a497-4661-b9e0-2ae9792b050e",
          "name": "used-to-obtain-oval-definitions-for-a-given-advisory-id-advisory-id-i-e--ciscosa20150819pcp",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/oval/advisory/:advisory_id"
              ],
              "variable": [
                {
                  "id": "advisory_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain OVAL definitions for a given advisory ID `advisory_id` (i.e., cisco-sa-20150819-pcp)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22091b94-c5a7-4de1-aff7-535e0a6de73c"
            }
          ]
        },
        {
          "id": "85221f94-8a58-4220-854d-5fb638c9b6b7",
          "name": "used-to-obtain-all-open-vulnerability-and-assessment-language-oval-definitions-available-for-cisco-s",
          "request": {
            "url": "http://api.cisco.com/security/advisories/oval/all",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all Open Vulnerability and Assessment Language (OVAL) definitions available for Cisco security vulnerabilities. For more information about OVAL go to https://communities.cisco.com/docs/DOC-63158 . By default the output is in JSON. To obtain the output in XML use the .xml extension. For example, /advisories/oval/all.xml"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "174c19a8-5c0a-4b78-9675-cb6f1632c543"
            }
          ]
        },
        {
          "id": "2aef4980-0d92-480c-ab7a-264a75ad4cbf",
          "name": "used-to-obtain-oval-definitions-for-a-given-cve-identifier--the-cve-id-format-is-cveyyyynnnn-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/oval/cve/:cve_id"
              ],
              "variable": [
                {
                  "id": "cve_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain OVAL definitions for a given CVE Identifier. The `cve_id` format is CVE-YYYY-NNNN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f5c1b24-ebfb-426d-9aac-3c50db6d6cf0"
            }
          ]
        },
        {
          "id": "6acd3671-dcc7-46d8-a9f9-70193d692ed6",
          "name": "used-to-obtain-all-the-latest-oval-definitions-given-an-absolute-number--for-instance-the-latest-10-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/oval/latest/:number"
              ],
              "variable": [
                {
                  "id": "number",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all the latest OVAL definitions given an absolute number. For instance, the latest 10 or latest 5."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac43a01c-1964-4b8f-a66d-2e11ea8c6c2f"
            }
          ]
        },
        {
          "id": "90b32c8c-dd26-4648-b4e6-5ab59ace5fd6",
          "name": "used-to-obtain-all-the-oval-advisories-that-affects-the-given-product-name-",
          "request": {
            "url": "http://api.cisco.com/security/advisories/oval/product?product=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all the oval advisories that affects the given product name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa1de2ed-881c-4cb8-a03a-0e9f2fa6b6d0"
            }
          ]
        },
        {
          "id": "23990031-60cc-416a-91b6-c96c95152b1c",
          "name": "used-to-obtain-all-oval-definitions-for-a-given-security-impact-rating-critical-high-medium-or-low-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/oval/severity/:severity"
              ],
              "variable": [
                {
                  "id": "severity",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all OVAL definitions for a given security impact rating (critical, high, medium, or low)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06f659a9-c067-4f7a-8074-bfb8548e4978"
            }
          ]
        },
        {
          "id": "616d6a91-1a2d-40ca-bd67-8dee83f5687a",
          "name": "used-to-obtain-all-security-advisories-for-a-given-security-impact-rating-critical-high-medium-or-lo2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/oval/severity/:severity/firstpublished"
              ],
              "query": [
                {
                  "key": "endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startDate",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "severity",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all security advisories for a given security impact rating (critical, high, medium, or low) in OVAL format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a81be8f-15f2-47ee-aed3-be78128e0116"
            }
          ]
        },
        {
          "id": "ee5d617c-ab62-4c6f-b419-abba791bf20b",
          "name": "used-to-obtain-all-security-advisories-for-a-given-security-impact-rating-critical-high-medium-or-lo3",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.cisco.com",
              "path": [
                "security/advisories/oval/severity/:severity/lastpublished"
              ],
              "query": [
                {
                  "key": "endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startDate",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "severity",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Used to obtain all security advisories for a given security impact rating (critical, high, medium, or low) in OVAL format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1ddb3e3-f5c0-4256-b4a8-994771e8957f"
            }
          ]
        }
      ]
    }
  ]
}