{
  "info": {
    "name": "OpenDNS Delete Domain",
    "_postman_id": "a66b48a7-7fda-4465-8d72-9d4353df36d4",
    "description": "To delete a domain from the shared customer???s domain list, run a DELETE request against the domains endpoint of the API.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Network Devices",
      "item": [
        {
          "id": "05c1ff09-6784-4308-ae5d-bc399969d0d2",
          "name": "networkDevices",
          "request": {
            "url": "http://example.com/api/networkdevices?macAddress=macAddress&label=label&model=model&serialNumber=serialNumber&tag=tag",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "The Network Device Registration API provides a way for networking hardware vendors to integrate their network devices with the OpenDNS Umbrella Dashboard."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bab7fc67-92ac-420e-a328-a48c5af79c3b"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "b2418da6-8459-45d3-92f2-4f29181c6768",
          "name": "domainStatus",
          "request": {
            "url": "http://example.com/api/domains/categories/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API method returns the domain status, which the quickest and easiest way to know whether a domain has been flagged as malicious by the OpenDNS Security Labs team (score of -1 for status), if it is believed to be safe (score of 1), or if it has yet to be given a status (score of 0)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4066ad4e-478a-4522-8370-0bd3eadacf42"
            }
          ]
        },
        {
          "id": "a0e5b4ba-5ca8-4aa6-9512-8c87efc7f7c6",
          "name": "coOccurrencesDomain",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "recommendations/:name/"
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "name",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API method returns a list of co-occurences for the specified domain. A co-occurrence is when two or more domains are being accessed by the same users within a small window of time. Being a co-occurrence isn't necessarily a bad thing, legitimate sites co-occur with each other as a part of normal web activity. However, unusual or suspicious co-occurence can provide additional information regarding attacks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9247c78f-ab2e-44f6-b5de-2e78d9186cc7"
            }
          ]
        },
        {
          "id": "c09eadc9-6a82-494c-9a85-5be2bfd9a00a",
          "name": "getDomains",
          "request": {
            "url": "http://example.com/api/domains",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To gather the lists of domains already added to the shared customer???s domain list, run a GET request against the domains endpoint of the API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5da7c7ea-3b8f-4add-b689-3e6058ef0db8"
            }
          ]
        },
        {
          "id": "23787f5e-d875-41e6-9cff-4f439cff7698",
          "name": "deleteDomain",
          "request": {
            "url": "http://example.com/api/domains",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "To delete a domain from the shared customer???s domain list, run a DELETE request against the domains endpoint of the API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b6f4f83-3d8d-4dcb-a8e7-ef425ab02230"
            }
          ]
        }
      ]
    },
    {
      "name": "Domain Score",
      "item": [
        {
          "id": "b839f554-7a9f-4db6-a3de-9b3cd2d99240",
          "name": "domainScore",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "domains/score/:domain"
              ],
              "variable": [
                {
                  "id": "domain",
                  "value": "domain",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API method is the quickest and easiest way to know whether a domain has been flagged as malicious by the OpenDNS security team (score of -1), if it is believed to be safe (score of 1), or if it hasn't been categorized yet (score of 0)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cedf89a7-906b-43a8-af40-e8ee9bc0a137"
            }
          ]
        }
      ]
    },
    {
      "name": "Pattern Search",
      "item": [
        {
          "id": "e31cec77-677c-4b88-a466-5debc752dfcf",
          "name": "patternSearch",
          "request": {
            "url": "http://example.com/api/search/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To perform a pattern search in the API, use the /search/ endpoint, append a RegEx pattern search to the API query and a start time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a04004f-e182-46e1-acbe-3b81b3861ee6"
            }
          ]
        }
      ]
    },
    {
      "name": "Related Domains",
      "item": [
        {
          "id": "2ec86288-de82-4746-8a98-40f4c5a7b969",
          "name": "relatedDomains",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "links/:name/"
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "name",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API method returns a list of domain names that have been frequently seen requested b around the same time (up to 60 seconds before or after) as the given domain name, but that are not frequently associated with other domain names."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d87376d4-7e5c-4fda-a6aa-e38a99991705"
            }
          ]
        }
      ]
    },
    {
      "name": "Security",
      "item": [
        {
          "id": "c49b5a0c-c349-4cbf-a7c0-191e3ba9f59d",
          "name": "securityInformation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "security/:name/"
              ],
              "query": [
                {
                  "key": "Domain Name",
                  "value": "Domain%20Name",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "name",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The security information API method contains multiple scores or security features, each of which can be used to determine relevant datapoints to build insight on the reputation or security risk posed by the site. No one security information feature is conclusive, instead these features should be looked at in conjunction with one another as part of your security research."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21e0075d-fe84-4ccd-b3ad-c00fa637ecae"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "7127910b-5200-4a85-89c1-e10509e8f249",
          "name": "domainTagging",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "domains/:name/latest_tags"
              ],
              "query": [
                {
                  "key": "Domain Name",
                  "value": "Domain%20Name",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "name",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint returns the date range when the domain being queried was a part of the OpenDNS block list. A common use case is to find how long a domain has been in the block list for domains being blocked currently. However it will also show a record of the history of the domain in the OpenDNS blocklis"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87338a13-8df0-4251-9df9-6f420b59d91f"
            }
          ]
        }
      ]
    },
    {
      "name": "History",
      "item": [
        {
          "id": "cae700ac-6b66-4649-85c6-6a248a915f9f",
          "name": "rrHistory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "dnsdb/:name/a/"
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "name",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The DNS database can be used to query the history that OpenDNS has seen for a given domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a552ebb-9b8c-4a93-95ab-6dff340f59d1"
            }
          ]
        }
      ]
    },
    {
      "name": "IP Address",
      "item": [
        {
          "id": "8ffec600-e814-409c-ae3a-2fda98b3bea0",
          "name": "ipAddressHistory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "bgp_routes/ip/:ip/"
              ],
              "variable": [
                {
                  "id": "ip",
                  "value": "ip",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "To help better understand how IP addresses are related to each other and to the regional registries, the API can provide data about ASN and IP relationships. You can also find out more about the IP space associated with an AS with this endpoint and correlate BGP routing information between AS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c471cef-a548-4a91-9eec-0754f2eb2723"
            }
          ]
        }
      ]
    },
    {
      "name": "Whois",
      "item": [
        {
          "id": "4a274e68-effd-4b93-9794-0b55dad3d79b",
          "name": "whois",
          "request": {
            "url": "http://example.com/api/whois/emails/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This API method returns the WHOIS information for the specified email address(es), nameserver(s) and domains. You can also search by multiple email addresses or multiple nameservers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf1f65ae-672d-48b7-8ff2-9d924fbcfc66"
            }
          ]
        }
      ]
    },
    {
      "name": "Malicious Domains",
      "item": [
        {
          "id": "60bd5747-afdc-45f1-81f2-ead1433a3cd2",
          "name": "latestMaliciousDomains",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "api",
                "ips/:ip/latest_domains"
              ],
              "variable": [
                {
                  "id": "ip",
                  "value": "ip",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The latest_domains endpoint shows whether the IP address you???ve entered as input has any known malicious domains associated with it."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "540ea72f-cf50-440a-8c8c-54ff3d6afdae"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "063a1441-c7f3-432d-9eca-de4c22ed94ec",
          "name": "postEvent",
          "request": {
            "url": "http://example.com/api/events",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Posts a Malware event to the API for processing and optionally adding to a customer's domain lists."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68b91e03-31a7-488f-b0ea-f6e95b75adc7"
            }
          ]
        }
      ]
    }
  ]
}