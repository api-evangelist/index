{
  "info": {
    "name": "Dyn Update Email X-Headers",
    "_postman_id": "473a2b2b-cd0b-4cbd-8a58-aa1f01f5a229",
    "description": "Updating the custom x-headers of an Email account",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "eda86ce2-1bef-4cc4-adfc-5a67e5b62b27",
          "name": "getAccounts",
          "request": {
            "url": "http://example.com/api/accounts?apikey=%7B%7D&startindex=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a list of up to 25 Email Sub-Accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6035f71-38bd-465e-bde2-83c862127de3"
            }
          ]
        },
        {
          "id": "715f26b6-03cf-45b6-b540-fdb371846511",
          "name": "getRecipientsStatus",
          "request": {
            "url": "http://example.com/api/recipients/status?apikey=%7B%7D&emailaddress=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Recipient(s) Status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7aaf03ae-3966-4ea4-b5cf-f6e650eea8d7"
            }
          ]
        },
        {
          "id": "f61023e0-4df4-427b-afcb-416ecb49d58e",
          "name": "getReportsBounces",
          "request": {
            "url": "http://example.com/api/reports/bounces?apikey=%7B%7D&bounce_code - Indicates the code associated with the bounced Email.=%7B%7D&bounce_code_id - The numeric code determined by the bounce processor.=%7B%7D&bounce_rule - Indicates the rule that caused this email to bounce.=%7B%7D&bounce_type=%7B%7D&bounce_type_id - Indicates whether the bounce type is a hard or soft bounce.nValid Values:n1 - Hard Bouncen2 - Soft Bounce=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&noheaders=%7B%7D&sender=%7B%7D&sender_id=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving the Email SPAM Complaints"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20185a9b-f654-4796-a6b7-632036f75107"
            }
          ]
        },
        {
          "id": "a133b831-aceb-4701-9239-d1143296c394",
          "name": "getReportsBouncesCount",
          "request": {
            "url": "http://example.com/api/reports/bounces/count?apikey=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a total count of Email bounces using the API requires specific syntax for the REST API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09dd476c-232c-48e1-b5e7-e179d21ad35c"
            }
          ]
        },
        {
          "id": "47546a1b-2b09-4399-b466-6d31bb30ec4a",
          "name": "getReportsClicksCount",
          "request": {
            "url": "http://example.com/api/reports/clicks/count?apikey=%7B%7D&domainu00a0=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a total of Email links clicked"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd79477f-cd3f-4268-a27d-c3a630334b5b"
            }
          ]
        },
        {
          "id": "9db3799b-e23e-445b-adaa-2847bce75b14",
          "name": "getReportsClicksCountUnique",
          "request": {
            "url": "http://example.com/api/reports/clicks/count/unique?apikey=%7B%7D&domainu00a0=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a total of Email links clicked"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f883321-d5dc-407e-9afb-d418d0522bdf"
            }
          ]
        },
        {
          "id": "dfbf4897-8352-4cba-8309-2aec4ae34ed3",
          "name": "getReportsComplaints",
          "request": {
            "url": "http://example.com/api/reports/complaints?apikey=%7B%7D&endtime=%7B%7D&sender=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Email SPAM Complaints"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ff231c8-914c-4af7-9ee9-109f2c601622"
            }
          ]
        },
        {
          "id": "7d875fb7-1e95-4105-aff6-732b5ed66adc",
          "name": "getReportsComplaintsCount",
          "request": {
            "url": "http://example.com/api/reports/complaints/count?apikey=%7B%7D&endtime=%7B%7D&starttime=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a total count of Email complaints"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b450eac0-d566-4806-905a-ee68d31aae35"
            }
          ]
        },
        {
          "id": "36b5029f-accc-48a7-ae2c-0dfdea52acce",
          "name": "getReportsDelivered",
          "request": {
            "url": "http://example.com/api/reports/delivered?apikey=%7B%7D&endtime=%7B%7D&sender=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Emails Delivered"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6cd8681-a1f6-499f-9793-f00f26b84e40"
            }
          ]
        },
        {
          "id": "ee6f8724-10da-4c1e-baf8-3b8940f8aecb",
          "name": "getReportsDeliveredCount",
          "request": {
            "url": "http://example.com/api/reports/delivered/count?apikey=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Count of Emails Delivered"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6dc333a7-c603-456e-b930-ec3dea43e21e"
            }
          ]
        },
        {
          "id": "2e926c02-60eb-4226-a8e9-2b39172041dc",
          "name": "getReportsIssues",
          "request": {
            "url": "http://example.com/api/reports/issues?apikey=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&sender_id=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Email Issues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8289fd3-84a1-415a-a4a1-d349c75e454b"
            }
          ]
        },
        {
          "id": "96f5bf91-7028-4385-b4a3-8677f6704179",
          "name": "getReportsIssuesCount",
          "request": {
            "url": "http://example.com/api/reports/issues/count?apikey=%7B%7D&endtime=%7B%7D&starttime=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a total count of Email issues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c48fb70-e691-4004-908e-653fa639afb5"
            }
          ]
        },
        {
          "id": "77f1d4b1-bba6-48dc-8b79-c6fbea05c2e4",
          "name": "getReportsOpensCountUnique",
          "request": {
            "url": "http://example.com/api/reports/opens/count/unique?apikey=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns total number of unique opens for the specified account for the specified date range. Including a date range is highly recommended."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7830f6e0-7684-4b5c-8e89-4fa05062f695"
            }
          ]
        },
        {
          "id": "1b1586d1-0e00-44dc-ba2a-38d8c601d05f",
          "name": "getReportsSent",
          "request": {
            "url": "http://example.com/api/reports/sent?apikey=%7B%7D&endtime=%7B%7D&sender=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Emails Sent"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "941fe869-253b-4d6c-9102-d8e968d7da11"
            }
          ]
        },
        {
          "id": "0c3281a7-28ab-4e9d-a393-18342f12daaa",
          "name": "getReportsSentCount",
          "request": {
            "url": "http://example.com/api/reports/sent/count?apikey=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Count of Emails Sent"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66f6f868-e1f0-4bf9-a7d1-59ebdc48c667"
            }
          ]
        },
        {
          "id": "6489544e-9f61-4056-b9ce-3538cdc0977b",
          "name": "getSuppressions",
          "request": {
            "url": "http://example.com/api/suppressions?apikey=%7B%7D&startdate=%7B%7D&startindex=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a list of Email addresses on the suppression list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61728a9f-0658-49c3-a39e-a36e9b491825"
            }
          ]
        },
        {
          "id": "37da70fd-2039-4455-8219-5f81bfecf31e",
          "name": "getSuppressionsCount",
          "request": {
            "url": "http://example.com/api/suppressions/count?apikey=%7B%7D&enddate=%7B%7D&startdate=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving the count of Email addresses on the suppression list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1391330-9e5f-479b-a314-ad8d5fec8cf8"
            }
          ]
        }
      ]
    },
    {
      "name": "Updating.Email",
      "item": [
        {
          "id": "a1e850e7-0958-4e2c-a4f9-6c82422cc040",
          "name": "putAccounts",
          "request": {
            "url": "http://example.com/api/accounts?address=%7B%7D&apikey=%7B%7D&bounceurl=%7B%7D&city=%7B%7D&companyname=%7B%7D&country=%7B%7D&generatenewapikey=%7B%7D&password=%7B%7D&phone=%7B%7D&spamurl=%7B%7D&state=%7B%7D&timezone=%7B%7D&tracklinks=%7B%7D&trackopens=%7B%7D&trackunsubscribes=%7B%7D&unsubscribeurl=%7B%7D&username=%7B%7D&zipcode=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updating an Email Sub-Account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b14833e-2648-4f01-a3d8-7d90c5d7a465"
            }
          ]
        }
      ]
    },
    {
      "name": "Create.Email",
      "item": [
        {
          "id": "7739f1f9-95c4-4654-b9ea-74a9aae5af35",
          "name": "postAccounts",
          "request": {
            "url": "http://example.com/api/accounts?address=%7B%7D&apikey=%7B%7D&bounceurl=%7B%7D&city=%7B%7D&companyname=%7B%7D&country=%7B%7D&generatenewapikey=%7B%7D&password=%7B%7D&phone=%7B%7D&spamurl=%7B%7D&state=%7B%7D&timezone=%7B%7D&tracklinks=%7B%7D&trackopens=%7B%7D&trackunsubscribes=%7B%7D&username=%7B%7D&zipcode=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creating an Email Sub-Account using the API requires specific syntax for the REST API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af42d7a4-5e19-4bd7-a45d-62cd2d218c3b"
            }
          ]
        }
      ]
    },
    {
      "name": "Deleting.Email",
      "item": [
        {
          "id": "474ef90b-d883-4986-805e-c07e4b1c988b",
          "name": "postAccountsDelete",
          "request": {
            "url": "http://example.com/api/accounts/delete?apikey=%7B%7D&username=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Deleting an Email Sub-Account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c057fd0-aa79-458a-8812-6ea38ef1e1f0"
            }
          ]
        }
      ]
    },
    {
      "name": ".Email",
      "item": [
        {
          "id": "c7360ffc-d4fd-47be-bd5d-ed8d21a30db7",
          "name": "getOpensCount",
          "request": {
            "url": "http://example.com/api/opens/count?apikey=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns total number of opens for the specified account for the specified date range. Including a date range is highly recommended."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "327cb2f6-55bd-44ce-99a7-1a8581d8657e"
            }
          ]
        },
        {
          "id": "e49cf767-3227-4ba9-be10-53e3b27172b3",
          "name": "postSuppressions",
          "request": {
            "url": "http://example.com/api/suppressions?apikey=%7B%7D&emailaddress=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Adding one or more recipients to the suppression list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6ce91b7-3dd7-483a-b425-dc4499d3a3a2"
            }
          ]
        },
        {
          "id": "717f3610-4e1c-4684-93c5-794b80ee1460",
          "name": "postXheaders",
          "request": {
            "url": "http://example.com/api/xheaders?apikey=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updating the custom x-headers of an Email account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55011964-3516-4883-be04-9ee9d6e4d4ad"
            }
          ]
        }
      ]
    },
    {
      "name": "Activate",
      "item": [
        {
          "id": "7af55262-7178-426f-99e8-212e26558dca",
          "name": "postRecipientsActivate",
          "request": {
            "url": "http://example.com/api/recipients/activate?apikey=%7B%7D&emailaddress=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Activating a specified Recipientu2019s status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a07893eb-7599-4688-96f8-cd3a43e0962d"
            }
          ]
        }
      ]
    },
    {
      "name": "Reports",
      "item": [
        {
          "id": "ceed14c5-a461-4ef5-a32e-c6d7212bf5c3",
          "name": "getReportsClicks",
          "request": {
            "url": "http://example.com/api/reports/clicks?apikey=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of links clicked for the specified account during the specified date range. Including a date range is highly recommended."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ffdcc2de-51b6-4969-805a-ae1f8b411b42"
            }
          ]
        }
      ]
    },
    {
      "name": "Unique",
      "item": [
        {
          "id": "091af105-5fad-434f-9d02-15beda64feda",
          "name": "getReportsClicksUnique",
          "request": {
            "url": "http://example.com/api/reports/clicks/unique?apikey=%7B%7D&emailaddress=%7B%7D&endtime=%7B%7D&sender=%7B%7D&startindex=%7B%7D&starttime=%7B%7D&[X-HeaderName]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of unique links clicked for the specified account during the specified date range. Including a date range is highly recommended."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90c33582-61ca-4386-9f37-1d91b3277362"
            }
          ]
        }
      ]
    },
    {
      "name": "Send",
      "item": [
        {
          "id": "81c9c3e6-ce4e-4b51-aa97-ae1192242e5c",
          "name": "postSend",
          "request": {
            "url": "http://example.com/api/send?apikey=%7B%7D&bcc=%7B%7D&bodyhtml=%7B%7D&bodytext=%7B%7D&cc=%7B%7D&comments=%7B%7D&from=%7B%7D&importance=%7B%7D&inreplyto=%7B%7D&keywords=%7B%7D&messageid=%7B%7D&priority=%7B%7D&references=%7B%7D&replyby=%7B%7D&replyto=%7B%7D&resent-date=%7B%7D&resent-from=%7B%7D&resent-messageid=%7B%7D&resent-replyto=%7B%7D&resent-sender=%7B%7D&sender=%7B%7D&sensitivity=%7B%7D&subject=%7B%7D&to=%7B%7D&xheaders=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sending Email"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f97f7f78-0ac0-4dd6-b153-08e6bd924b8e"
            }
          ]
        }
      ]
    },
    {
      "name": "Retrievinglist",
      "item": [
        {
          "id": "3cb528ca-b393-4bfa-aef1-007b4c54403d",
          "name": "getXheaders",
          "request": {
            "url": "http://example.com/api/xheaders?apikey=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieving a list of custom X-header field names"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b9cbe69-998b-4216-989c-03b870d8f2c6"
            }
          ]
        }
      ]
    }
  ]
}