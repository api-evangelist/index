{
  "info": {
    "name": "Charity Navigator Get Advisory",
    "_postman_id": "84563487-7274-4588-8dca-f77b186a3f7b",
    "description": "Retrieve the full set of Charity Navigator advisories for a specified\norganization. An advisory is a cautionary communication from Charity Navigator,\nadvising of unusual events or behavior related to a known organization.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "2d30a063-ea08-4b58-8d9e-8bc1b82a3394",
          "name": "searchOrganizations",
          "request": {
            "url": "http://api.data.charitynavigator.org/v2/Organizations?app_id=%7B%7D&app_key=%7B%7D&categoryID=%7B%7D&causeID=%7B%7D&cfcCharities=%7B%7D&city=%7B%7D&donorPrivacy=%7B%7D&fundraisingOrgs=%7B%7D&maxRating=%7B%7D&minRating=%7B%7D&noGovSupport=%7B%7D&pageNum=%7B%7D&pageSize=%7B%7D&rated=%7B%7D&scopeOfWork=%7B%7D&search=%7B%7D&searchType=%7B%7D&sizeRange=%7B%7D&sort=%7B%7D&state=%7B%7D&zip=%7B%7D",
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
            "description": "Retrieve a list of the organizations available in the Charity Navigator Data\nStore. Allows paged retrieval, simple and advanced searching."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e912bac-781e-4635-995e-9fd9f8b173d6"
            }
          ]
        },
        {
          "id": "96a08fad-1d86-4b63-ac5c-528777d5ff92",
          "name": "getOrganization",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.charitynavigator.org",
              "path": [
                "v2",
                "Organizations/:ein"
              ],
              "query": [
                {
                  "key": "app_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "app_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ein",
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
            "description": "Retrieve full detail of a single Organization. This is a composite set of\ninformation describing an organization that may engage in charitable work.\nNormally the Organization data structure includes a single legal entity, though\nlegal entity information may be excluded in exceptional cases."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88423ff8-358d-46fe-9aec-4f89921a8451"
            }
          ]
        },
        {
          "id": "21402842-0ed7-484d-834d-1806e770e27c",
          "name": "getRatings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.charitynavigator.org",
              "path": [
                "v2",
                "Organizations/:ein/Ratings"
              ],
              "query": [
                {
                  "key": "app_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "app_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageNum",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageSize",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ein",
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
            "description": "Retrieve all Charity Navigator ratings for a single organization. <br/>\n![Content\nSubscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png\n\"Included with the paid Content Subscription.\")"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22e1e362-85c5-4e5b-89a8-99ccf9c83e75"
            }
          ]
        },
        {
          "id": "ff908f23-ccae-4ee0-9c14-008c3e86484b",
          "name": "getRating",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.charitynavigator.org",
              "path": [
                "v2",
                "Organizations/:ein/Ratings/:RatingID"
              ],
              "query": [
                {
                  "key": "app_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "app_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ein",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "RatingID",
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
            "description": "Retrieve a single Rating object for an Organization. Each rating is listed\nonce, under its primary `referenceOrganization`. Note that the rating may apply\nto other organizations, and this is represented by `includedOrganizations`,\nwhich is a collection of hyperlinks to all of the organizations to which the\nrating applies.\nThe rating is a point-in-time assessment provided by Charity Navigator, along\nwith related metrics and ratios taken from financial statements for a fiscal\nyear, on which the rating is based. <br/> ![Content\nSubscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png\n\"Included with the paid Content Subscription.\")"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f003529c-e79b-4388-b286-ec54c531ee40"
            }
          ]
        },
        {
          "id": "5e0f8fc4-3fd0-487a-a177-0ecda02e5d67",
          "name": "getAdvisories",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.charitynavigator.org",
              "path": [
                "v2",
                "Organizations/:ein/Advisories"
              ],
              "query": [
                {
                  "key": "app_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "app_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageNum",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageSize",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "status",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ein",
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
            "description": "Retrieve the full set of Charity Navigator advisories for a specified\norganization. An advisory is a cautionary communication from Charity Navigator,\nadvising of unusual events or behavior related to a known organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7233344a-d44d-4e7e-93e0-93f69da1e822"
            }
          ]
        },
        {
          "id": "01627d4d-8c1d-4fd4-ba12-22b2406babfc",
          "name": "getAdvisory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.charitynavigator.org",
              "path": [
                "v2",
                "Organizations/:ein/Advisories/:AdvisoryID"
              ],
              "query": [
                {
                  "key": "app_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "app_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AdvisoryID",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "ein",
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
            "description": "Retrieve full details of a single Advisory, under a given organization. An\nadvisory is a cautionary communication from Charity Navigator, advising of\nunusual events or behavior related to a known organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b50ca04-863a-44ba-bf47-fc42085f4713"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "be214db0-9529-4f8c-820e-5905358c2691",
          "name": "getLists",
          "request": {
            "url": "http://api.data.charitynavigator.org/v2/Lists?app_id=%7B%7D&app_key=%7B%7D&pageNum=%7B%7D&pageSize=%7B%7D",
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
            "description": "Retrieve a set of Lists defined in Charity Navigator. Each entry in this\ncollection is a curated or generated list of organizations, published by Charity\nNavigator. <br/> ![Content\nSubscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png\n\"Included with the paid Content Subscription.\")"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d6fa936-73b0-4009-96b7-41771632e6d2"
            }
          ]
        },
        {
          "id": "b78b26ec-75b0-4916-8401-3c1000220e59",
          "name": "getList",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.charitynavigator.org",
              "path": [
                "v2",
                "Lists/:ListID"
              ],
              "query": [
                {
                  "key": "app_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "app_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ListID",
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
            "description": "Retrieve a curated or generated list of organizations, published by Charity\nNavigator. <br/> ![Content\nSubscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png\n\"Included with the paid Content Subscription.\")"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb37cc6c-3ab7-4770-95ab-68393964534b"
            }
          ]
        }
      ]
    },
    {
      "name": "Categories",
      "item": [
        {
          "id": "82fe16fd-ff22-408c-adf0-2015d6587ceb",
          "name": "getCategories",
          "request": {
            "url": "http://api.data.charitynavigator.org/v2/Categories?app_id=%7B%7D&app_key=%7B%7D",
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
            "description": "Returns metadata for Charity Navigator's classification hierarchy for\ncharitable Organizations. Category is the top-level classifier, and each\ncategory may contain a number of Causes. <br/> ![Content\nSubscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png\n\"Included with the paid Content Subscription.\")"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78aadfbc-04eb-4755-a14c-4e345ac3153f"
            }
          ]
        }
      ]
    },
    {
      "name": "Advisory",
      "item": [
        {
          "id": "f9683e63-bf13-4fb5-8a67-1ba711b90a23",
          "name": "getAllActiveAdvisories",
          "request": {
            "url": "http://api.data.charitynavigator.org/v2/Advisory?app_id=%7B%7D&app_key=%7B%7D&pageNum=%7B%7D&pageSize=%7B%7D",
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
            "description": "Retrieve the full set of Charity Navigator advisories for a specified\norganization. An advisory is a cautionary communication from Charity Navigator,\nadvising of unusual events or behavior related to a known organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac30e149-e705-41c4-8724-de186859da46"
            }
          ]
        }
      ]
    }
  ]
}