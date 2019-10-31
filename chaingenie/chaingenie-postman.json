{
  "info": {
    "name": "ChainGenie Retrieve document from IPFS",
    "_postman_id": "2bda42ac-70a3-4bbe-b0a7-21969855e271",
    "description": "Retrieve the document stream from IPFS node",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blockchain",
      "item": [
        {
          "id": "f52419e4-5c6a-449d-928f-0c90b943b32f",
          "name": "EthbankDepositPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethbank/deposit",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "value",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Deposit crypto currency into the bank.  In sandbox mode, the account used is the demo account on the blockchain server."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5644c8df-cfcc-4412-b8e7-96acfedc5d8a"
            }
          ]
        },
        {
          "id": "5080e17c-66ae-4ede-bc45-464855cf1d7a",
          "name": "EthbankWithdrawPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethbank/withdraw",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "value",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Withdraw crypto currency into the bank.  In sandbox mode, the account used is the demo account on the blockchain server. Of course, you can only withdraw if there is money in the account!"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bef9166b-4540-4ea5-bd46-429db6264aaa"
            }
          ]
        },
        {
          "id": "e7ef8a4d-7a80-4e56-94ef-d7cd17031883",
          "name": "EthbankPassbookGet",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethbank/passbook",
            "method": "GET",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Displays all transactions made by the user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a504ddb-15ef-4d21-b320-0c538fd00aa1"
            }
          ]
        },
        {
          "id": "13807ee7-c29b-4414-99cb-79b05b34cbc2",
          "name": "EthbankBalanceGet",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethbank/balance",
            "method": "GET",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Displays user bank balance information"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb5096b0-96eb-49e0-abe3-73642c9a2eb5"
            }
          ]
        },
        {
          "id": "f1ae2fad-2e44-4ee6-adb6-a95a6284f2c2",
          "name": "EthledgerInvokecontractPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/invokecontract",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "attribs",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "file",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "This API is the generic version of the \"Generate document from template\" API. Any template file can be uploaded (sample available as link for testing).  If you just want to see how this would work - use the other call and just run it without any uploaded certificate. \nUpload a templated pdf with editable / filable fields and generate a document with automated sign and routing to a recipient.  Every attribute that needs to be filled will need to be passed in the format - ex. course field to be substituted - field = attrib; value = [\"course\",\"course value\"] or date field to be substituted - field = attrib; value = [\"date\",\"12/12/2016\"].  If your fillable form has the field named \"today\", current time will be used for filling the value of that field.\nYou will need to upload for the file attribute a real template file with fillable fields. For the sample values as configured, you can use the demo template available at http://chaingenie.com/cert.pdf.  Download this certificate and add it as your input file\nTo route the document to recipient (optional) add field recipient with \"key\" of the recipient - available recipient in the system - 0xb3A214341df9560a3e09E256BfacefD6648f5Ca9 for your testing\nUse case - Upload an invoice template with fillable fields, add attrib values for all the fields that needs to be filled, add the recipient field - your invoice will be created, signed with your key (in production / in test it will be signed with the local admin key) and will be routed to the recipient (in production you can add your recipient / in sandbox - use recipient 0xb3A214341df9560a3e09E256BfacefD6648f5Ca9)\nResponse will contain the document name, signatories, timestamps, recipient, IPFS hash (handle to retrieve the actual document)\nThe document hash will be posted on blockchain and the actual document will be added to IPFS.  Want to retrieve your document? Check out the API - Write & Retrieve - Docs (IPFS)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e77eea9d-bb60-4534-b68b-36e03dc13ad4"
            }
          ]
        },
        {
          "id": "e2166e06-65f0-416b-94b2-ff667ff4a30b",
          "name": "EthledgerDocertPost2",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/docert",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "course",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "date",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "students",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "This is an over simplified version for testing this API for its powers a template - uses an inbuilt into ChainGenie template and values are preconfigured - just running this will work and provide you an IPFS handle to retrieve the document you generated with your variables / values from the template.\nUse an existing document on our server and generate a document with automated sign and routing to a recipient.  Ex. this configured api will generate a certificate for a student name (name) with the completed certificate course (course) and dated (date). \nThe document hash will be posted on blockchain and the actual document will be added to IPFS.  Want to retrieve your document? Check out the API - Write & Retrieve - Docs (IPFS)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca8d6cfd-011d-41b5-8212-74850d36a3ad"
            }
          ]
        },
        {
          "id": "d95a398d-bb13-4936-8412-7b341fd1be75",
          "name": "EthledgerSendforsignPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/sendforsign",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "files",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "recipient",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Route the document for signature.  The document history and status is updated for querying."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db617b47-c291-4560-a1b1-00676c3897ee"
            }
          ]
        },
        {
          "id": "a0aa38b6-ca9c-4de8-820c-d33775ccc44b",
          "name": "EthledgerSignPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/sign",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "files",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Cryptographically sign the document and add the record to blockchain.  The document history and status is updated for querying."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a3741f7-d637-431f-b451-a8ab8f75ade4"
            }
          ]
        },
        {
          "id": "9a74a595-0d07-488e-a3dc-c692d9f6d3ed",
          "name": "EthledgerDocstatusPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/docstatus",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "files",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Review the document status - existence, hash, block info, signatories, routing to users and details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a89891e7-b406-4b55-b71f-8a6a8c90e6e6"
            }
          ]
        },
        {
          "id": "f3d1eec8-00b3-41ce-b40b-6d1ba88369c7",
          "name": "EthledgerExistsdocPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/existsdoc",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "files",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Check if your documents exists in the eth blockchain"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a55244d5-b79f-4c50-9237-a5c4649b4910"
            }
          ]
        },
        {
          "id": "d977fa35-f998-4aaf-a3f9-e7d736c9255b",
          "name": "EthledgerPostdocPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/postdoc",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "files",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "filetypes",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Post document hash into eth chain for POE (proof of existence) and post the document into ipfs for safekeep!"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b04d2e2b-dfbf-482e-a230-b49e1b38a73c"
            }
          ]
        },
        {
          "id": "b02d1c75-a3c3-49cf-881d-b177625de9c4",
          "name": "EthledgerSendcertPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/sendcert",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "recipient",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "strHash",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Route the document to a recipient.  The document history and status is updated for querying.  The API call does not return any document properties.  This is a <b>minimalistic function</b> for stringing with other functions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8c9d900-a486-4476-9dac-3b96aac4809b"
            }
          ]
        },
        {
          "id": "087a7d9b-3136-41df-9957-7ebc204d6234",
          "name": "EthledgerSigncertPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/signcert",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "strHash",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Cryptographically sign the document and add the record to blockchain.  The document history and status is updated for querying.  The API call does not return any document properties.  This is a <b>minimalistic function</b> for stringing with other functions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3eb82ef0-48a0-4b2d-a4fb-79e2cec7e677"
            }
          ]
        },
        {
          "id": "66bcc616-34a5-413b-89bc-89705c5f3666",
          "name": "EthledgerGetdocstatePost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/getdocstate",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "strHash",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Review the document status - existence, hash, block info, signatories, routing to users and details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf272631-386e-46d3-a4d8-6172450544b3"
            }
          ]
        },
        {
          "id": "e5727ec4-4e0e-475f-af6f-2dbe39d5b20d",
          "name": "EthledgerPosthashPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/posthash",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "hash",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Post string hash into eth chain for POE (proof of existence)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c33b89bc-c1da-4e10-863f-c370ff706da1"
            }
          ]
        },
        {
          "id": "ff55fa90-c78f-4eab-9b76-2957b7e5d4ab",
          "name": "EthledgerExistshashPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/existshash",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "hash",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Check if your hash exists in the eth blockchain"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1cc2fa9-46cf-4d4e-9a14-1598822b8f2c"
            }
          ]
        },
        {
          "id": "7d6ad7f7-cd92-4d31-b498-0a1c21e61041",
          "name": "EthledgerPoststrPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/poststr",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "str",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Post string hash into eth chain for POE (proof of existence)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e31ed1e1-c9ab-4dcb-8514-ca57c897a9d0"
            }
          ]
        },
        {
          "id": "2a1210f6-d51a-4cb0-85aa-c12f2200d4a2",
          "name": "EthledgerExistsstrPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/existsstr",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "str",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Check if your string exists in the eth blockchain"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4d45cc6-58a3-4a41-881b-9f2c2cc049d4"
            }
          ]
        },
        {
          "id": "e234b979-1698-430e-9ad3-9837b93f6942",
          "name": "EthledgerGettransGet",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/gettrans",
            "method": "GET",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Displays all transactions connected to this project / smart contract"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dbaf0dd5-3416-476e-92c0-53a67503b725"
            }
          ]
        },
        {
          "id": "220a2a14-a7f4-45a9-b341-9cabea48631e",
          "name": "TradechainCreateTradeContractPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/tradechain/CreateTradeContract",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "itemName",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "itemPartNum",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "itemSellerName",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "itemValidUntil",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "itemValue",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "List product on marketplace: <br/>\r\n- Seller initiates sale - CreateTradeContract<br/>\r\n- Escrow from seller added for value of contract<br/>\r\n- End transaction state = Smart Contract Created<br/>"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95dfd855-e80e-4c81-b170-2eb951393e5e"
            }
          ]
        },
        {
          "id": "058934e6-36b8-4699-a026-3645081341e5",
          "name": "TradechainConfirmAbortPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/tradechain/ConfirmAbort",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "itemContractId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "itemSellerName",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Remove Listing (by Seller)<br/>\r\n- Seller cancels the market trade after listing but before bid/buy<br/>\r\n- Escrow from seller is returned back to the seller<br/>\r\n- End transaction state = Smart contract is rendered inactive<br/>"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0760698f-3932-4cf7-9e3c-1d7228873952"
            }
          ]
        },
        {
          "id": "5867eb9f-37a6-4cc3-967e-c34585fad48c",
          "name": "TradechainConfirmPurchasePost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/tradechain/ConfirmPurchase",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "itemBuyerName",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "itemContractId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Bid / buy the item listed on the marketplace: <br/>\r\n- Buyer confirms interest in buying<br/>\r\n- Escrow from buyer added to value of contract<br/>\r\n- Invoice document is created with all details using invoice template<br/>\r\n- Invoice is added IPFS and invoice hash into blockchain<br/>\r\n- End transaction state = Trade is actively locked between the seller and buyer<br/>"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bfb96197-3655-4883-a748-cd7d91a0716d"
            }
          ]
        },
        {
          "id": "0b3d5892-499d-4a78-832a-5ebde8ac76c9",
          "name": "TradechainConfirmRefundPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/tradechain/ConfirmRefund",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "itemContractId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "itemSellerName",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Seller can cancel the market trade after bid/buy by refunding the seller<br/>\r\nEscrow from buyer is returned back to the buyer<br/>\r\nEscrow from seller is returned back to the seller (optional: penalties can be imposed)<br/>\r\nEnd transaction state = Escrow returned, smart contract cancelled and become inactive<br/>"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a8bbbcc-9a51-4b95-93ef-ae567e24b78c"
            }
          ]
        },
        {
          "id": "78ce0263-6781-4987-95e9-96c7804e0c44",
          "name": "TradechainConfirmReceivedPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/tradechain/ConfirmReceived",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "itemBuyerName",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "itemContractId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Delivery of item confirmed by the buyer \r\n-Escrow is fully sent to seller\r\n- End transaction state = TRANSACTION COMPLETE"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c5b813c-592c-4df6-95a5-16ce59109d77"
            }
          ]
        },
        {
          "id": "e145d581-63d4-4cdc-90df-267b5c67268c",
          "name": "TradechainGetStateOfContractPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/tradechain/GetStateOfContract",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "itemContractId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Get contract details & state\n- Provide full information including\n - Escrow amount in contract\n - Contract state \n - Buyer & Seller information\n - Links to contract / invoice documents\n - and other contract / sale specific information"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e615bce-206e-49a6-a2fc-4d62428931b9"
            }
          ]
        },
        {
          "id": "ef11de9b-c923-4430-ad8e-801cc33bbdf9",
          "name": "TradechainGetFundsLockedInContractPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/tradechain/GetFundsLockedInContract",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "itemContractId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Get contract escrow details -\n- Retrieves full information including but not limited to\n - Escrow amount in contract\n - Contract state \n - Buyer & Seller information\n - Links to contract / invoice documents\n - and other contract / sale specific information"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d899973-74cf-47b2-b8c5-8384869762f7"
            }
          ]
        },
        {
          "id": "b5fb7578-82c3-4bd1-bb40-e1bff68377a7",
          "name": "TradechainWhoIsSellerPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/tradechain/WhoIsSeller",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "itemContractId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Get full information about the seller by providing the contract id.  Response will also include some contract details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d41e1a6-0203-43ca-bd33-c0876a115d91"
            }
          ]
        },
        {
          "id": "99a3f3d2-9c07-4d75-9fc4-711f26b41b4a",
          "name": "TradechainWhoIsBuyerPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/tradechain/WhoIsBuyer",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "itemContractId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Get full information about the seller by providing the contract id.  Response will also include some contract details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2be53edf-673d-4a3f-b3b7-a67b78b236cd"
            }
          ]
        },
        {
          "id": "460a8070-25da-40ed-bdcb-b2af3958f6e2",
          "name": "TradechainGetItemsFilterSortPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/tradechain/GetItemsFilterSort",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "filterField",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "filterValue",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "maxPrice",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "onSaleOnly",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "sortField",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "sortOrder",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Use a combination of fields to get any type of report.  Ex. send specific seller name or id to get active for sale items by seller; send specific filehash to get status of a particular item/invoice; send itemPartNum to get a list of all products of that partnumber and send sort order as itemValue ascending to cheapest top list) . . . \r\n-\tfilterField (accepted items below, default – none)\r\no\titemSellerId\r\no\titemSellerName\r\no\titemBuyerId\r\no\titemBuyerName\r\no\titemId\r\no\titemName\r\no\titemPartNum\r\no\tfileHash\r\no\tFileHash\r\n-\tsortField (accepted items below, default – itemValidUntil)\r\no\titemSellerId\r\no\titemSellerName\r\no\titemBuyerId\r\no\titemBuyerName\r\no\titemId\r\no\titemName\r\no\titemValue\r\no\titemPartNum\r\no\titemValidUntil\r\n-\tsortOrder (default – desc)\r\no\tasc\r\no\tdesc\r\n-\tonSaleOnly (default – true, only if not “Inactive”)\r\no\ttrue\r\no\tfalse\r\n-\tmaxPrice (double; default - 0)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39f6814c-ff10-4222-b051-d1bf47550a26"
            }
          ]
        },
        {
          "id": "3fa479e0-1f8e-4ac2-b14b-694a39934a8c",
          "name": "BasicfnsGetAccountBalancePost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/basicfns/GetAccountBalance",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "accountId",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Get information about an user's account balance.  The call is restricted to the unlocked user's account / query only. <br/>* In this sandbox, you can query any user's account balance for testing purposes.  All accounts are test accounts and no actual value or account is exposed in the sandbox."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "722c4041-f745-4920-be37-ebc4156043c1"
            }
          ]
        },
        {
          "id": "9f0e9558-89df-475e-a4bc-c0c7e073aa57",
          "name": "EthledgerIpfsaddPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/ipfsadd",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "files",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Post the document into ipfs for safekeep!"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "feac058f-1215-40a0-9b10-9190e5deb85c"
            }
          ]
        },
        {
          "id": "5339d15b-2a45-4132-ad99-1b064db410ff",
          "name": "EthledgerIpfsgetPost",
          "request": {
            "url": "http://api.chaingenie.com/api/v1/ethledger/ipfsget",
            "method": "POST",
            "header": [
              {
                "key": "ApiKey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "hash",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Retrieve the document stream from IPFS node"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58ad62cf-5a3c-400e-af3f-c5299760ebe4"
            }
          ]
        }
      ]
    }
  ]
}