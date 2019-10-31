{
  "info": {
    "name": "Browshot Retrieve a thumbnail image",
    "_postman_id": "42dda585-1b32-431c-be72-cba522663edf",
    "description": "Unlike the other API calls, this API sends back the thumbnail as a PNG file, not JSON. The HTTP response code indicates whether the screenshot was successful (200), or incomplete (404) or failed (404). If the screenshot failed or is not finished, a default image \"Not found\" is sent.\n\nYou can crop your screenshots. The crop is done first, then the thumbnail. You can take a 1024x768 screenshot, crop it to 768x768, and get it scaled down to 300x300.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "6633806c-0d7c-4e07-a628-ee8a18a3292a",
          "name": "GetAccountInfo",
          "request": {
            "url": "http://api.browshot.com/api/v1/account/info?details=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18993512-dd07-44a1-8455-f800ba373f22"
            }
          ]
        }
      ]
    },
    {
      "name": "Batch",
      "item": [
        {
          "id": "a8824d6a-9162-40be-b1f0-8cbe3baeaaf0",
          "name": "CreateBatch",
          "request": {
            "url": "http://api.browshot.com/api/v1/batch/ceate?hosting=%7B%7D&hosting_bucket=%7B%7D&hosting_file=%7B%7D&hosting_headers=%7B%7D&hosting_height=%7B%7D&hosting_scale=%7B%7D&hosting_width=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "cookie",
                  "value": "{}",
                  "disabled": false,
                  "description": "set a cookie for the URL requested (see Custom POST Data, Referer and Cookie) Cookies should be separated by a ; - paid screenshots only"
                },
                {
                  "key": "delay",
                  "value": "{}",
                  "disabled": false,
                  "description": "number of seconds to wait after the page has loaded"
                },
                {
                  "key": "details",
                  "value": "{}",
                  "disabled": false,
                  "description": "level of information available with screenshot/info"
                },
                {
                  "key": "file",
                  "value": "{}",
                  "disabled": false,
                  "description": "text file to use"
                },
                {
                  "key": "flash_delay",
                  "value": "{}",
                  "disabled": false,
                  "description": "number of seconds to wait after the page has loaded if Flash elements are present"
                },
                {
                  "key": "format",
                  "value": "{}",
                  "disabled": false,
                  "description": "image as PNG or JPEG"
                },
                {
                  "key": "headers",
                  "value": "{}",
                  "disabled": false,
                  "description": "any custom HTTP headers"
                },
                {
                  "key": "height",
                  "value": "{}",
                  "disabled": false,
                  "description": "thumbnail height"
                },
                {
                  "key": "html",
                  "value": "{}",
                  "disabled": false,
                  "description": "saves the HTML of the rendered page which can be retrieved by the API call screenshot/html"
                },
                {
                  "key": "instance_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "instance ID to use"
                },
                {
                  "key": "max_wait",
                  "value": "{}",
                  "disabled": false,
                  "description": "maximum number of seconds to wait before triggering the PageLoad event"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "name of the batch"
                },
                {
                  "key": "post_data",
                  "value": "{}",
                  "disabled": false,
                  "description": "send a POST requests with post_data, useful for filling out forms - paid screenshots only"
                },
                {
                  "key": "priority",
                  "value": "{}",
                  "disabled": false,
                  "description": "assign priority to the screenshot (for private instances only)"
                },
                {
                  "key": "referer",
                  "value": "{}",
                  "disabled": false,
                  "description": "use a custom referrer header - paid screenshots only"
                },
                {
                  "key": "screen_height",
                  "value": "{}",
                  "disabled": false,
                  "description": "height of the browser window"
                },
                {
                  "key": "screen_width",
                  "value": "{}",
                  "disabled": false,
                  "description": "width of the browser window"
                },
                {
                  "key": "script",
                  "value": "{}",
                  "disabled": false,
                  "description": "URL of javascript file to execute after the page load event"
                },
                {
                  "key": "size",
                  "value": "{}",
                  "disabled": false,
                  "description": "screenshots size - screen (default) or page"
                },
                {
                  "key": "width",
                  "value": "{}",
                  "disabled": false,
                  "description": "thumbnail width"
                }
              ]
            },
            "description": "Get hundreds or thousands of screenshots from a text file. You can use this API call or the dashboard. Unlike the other API calls, you must issue a POST request with the Content-Type \"multipart/form-data\" in order to upload the text file. The text file must contain the list of URLs to request, 1 URL per line. Failed screenshots will be tried up to 3 times before giving up."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f97bc5e-97cc-4cf5-98cd-8d0d788b0c76"
            }
          ]
        },
        {
          "id": "fb46be25-1fb2-4778-8e13-aacadf10be01",
          "name": "GetBatchInfo",
          "request": {
            "url": "http://api.browshot.com/api/v1/batch/info?id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the status of a batch requested through the API or through the dashboard."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0ab13e1-8d58-4d5d-ad98-8392dcd5f7b2"
            }
          ]
        }
      ]
    },
    {
      "name": "Browser",
      "item": [
        {
          "id": "5885268c-49ce-4dbb-b0ff-a49d3f21bebc",
          "name": "GetBrowserInfo",
          "request": {
            "url": "http://api.browshot.com/api/v1/browser/info?id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a browser."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd51d1b7-748b-4165-8d3b-71bdda6dbfbf"
            }
          ]
        },
        {
          "id": "df4359f3-a49a-431a-9da0-667205985eb2",
          "name": "GetBrowsersInfo",
          "request": {
            "url": "http://api.browshot.com/api/v1/browser/list",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all browsers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82face8d-1c9f-4ec6-8630-b863f2495ae9"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance",
      "item": [
        {
          "id": "32aa4af1-40dd-4274-adf6-e0c53305cee7",
          "name": "GetInstanceInfo",
          "request": {
            "url": "http://api.browshot.com/api/v1/instance/info?id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about an instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97c1db01-c34d-44dc-b82a-7a0400292078"
            }
          ]
        },
        {
          "id": "141c61a6-1075-403c-bd6e-12ed4069cf84",
          "name": "GetInstancesInfo",
          "request": {
            "url": "http://api.browshot.com/api/v1/instance/list",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a9538c2-feb2-4561-bec4-d3146fff32c8"
            }
          ]
        }
      ]
    },
    {
      "name": "Screenshot",
      "item": [
        {
          "id": "1a4e2c33-a89b-47bd-8f3a-44db377256a4",
          "name": "CreateScreenshot",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/create?cache=%7B%7D&cookie=%7B%7D&delay=%7B%7D&details=%7B%7D&flash_delay=%7B%7D&headers=%7B%7D&hosting=%7B%7D&hosting_bucket=%7B%7D&hosting_file=%7B%7D&hosting_headers=%7B%7D&hosting_height=%7B%7D&hosting_scale=%7B%7D&hosting_width=%7B%7D&html=%7B%7D&instance_id=%7B%7D&max_wait=%7B%7D&post_data=%7B%7D&priority=%7B%7D&referer=%7B%7D&screen_height=%7B%7D&screen_width=%7B%7D&script=%7B%7D&shots=%7B%7D&shot_interval=%7B%7D&size=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Screenshots requests to private and shared instances require a positive balance.\n\n*IMPORTANT*: Remember that you can only do 100 free screenshots per month. To used a premium instance, use instance_id=65 for example."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36c3cdaa-5a5c-452e-99e3-92144d39ab1b"
            }
          ]
        },
        {
          "id": "78e0b823-608a-4a50-aa2d-0742e3647660",
          "name": "DeleteScreenshot",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/delete?data=%7B%7D&id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can delete details of your screenshots to remove any confidential information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "897e2784-4c5c-42e9-9b38-5dbfdd7ae3c9"
            }
          ]
        },
        {
          "id": "2c2b9385-c2b7-4e84-8885-d635948eda10",
          "name": "HostScreenshot",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/host?bucket=%7B%7D&file=%7B%7D&headers=%7B%7D&height=%7B%7D&hosting=%7B%7D&id=%7B%7D&scale=%7B%7D&width=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can host screenshots and thumbnails on your own S3 account or on Browshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37d92f1d-3bb1-45f8-9e3f-6d5337e15169"
            }
          ]
        },
        {
          "id": "a5167d86-204b-483c-9931-dca9b29eb12a",
          "name": "GetHTML",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/html?id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the HTML code of the rendered page. This API call should be used when html=1 was specified in the screenshot request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96990722-0814-4bda-814f-1010d66b1973"
            }
          ]
        },
        {
          "id": "6e877376-663a-46f5-9703-b5985037638d",
          "name": "GetScreenshotInfo",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/info?details=%7B%7D&id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Once a screenshot has been requested, its status must be checked until it is either \"error\" or \"finished\"."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71aa25f2-a57e-45fc-8d92-7c3c72db707a"
            }
          ]
        },
        {
          "id": "38663043-c535-4590-9f12-8c6f578423c9",
          "name": "GetMultipleScreenshotsInfo",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/list?limit=%7B%7D&status=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about the last 100 screenshots requested."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37cea0f0-8c42-4db8-a20d-0d7048acf74a"
            }
          ]
        },
        {
          "id": "a9bdfac5-3027-44ee-8c49-6d7df70c847e",
          "name": "CreateMultipleScreenshots",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/multiple?cache=%7B%7D&cookie=%7B%7D&delay=%7B%7D&details=%7B%7D&flash_delay=%7B%7D&headers=%7B%7D&hosting=%7B%7D&hosting_bucket=%7B%7D&hosting_file=%7B%7D&hosting_headers=%7B%7D&hosting_height=%7B%7D&hosting_scale=%7B%7D&hosting_width=%7B%7D&html=%7B%7D&instance_id=%7B%7D&max_wait=%7B%7D&post_data=%7B%7D&priority=%7B%7D&referer=%7B%7D&screen_height=%7B%7D&screen_width=%7B%7D&script=%7B%7D&size=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Request multiple screenshots in one API call. The API call accepts all the parameters supported by screenshot/create.\nYou can specify up to 10 URLs and 10 instances for a total of 100 screenshots in one API call."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c1b5a35-4047-44ad-ac47-c0c3c10003d7"
            }
          ]
        },
        {
          "id": "0993c963-beb1-4b1f-aa0a-aca0264d39b3",
          "name": "SearchScreenshot",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/search?limit=%7B%7D&status=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search for screenshots of a specific URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8eb829ec-5557-4512-b312-9d57a35e1759"
            }
          ]
        },
        {
          "id": "174473ea-5171-46ab-920c-28d16d680f43",
          "name": "ShareScreenshot",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/share?id=%7B%7D&note=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can make your screenshots public, add notes, and share it with your friends and colleagues. Only screenshots which are successfully completed can be shared.n the thumbnail. You can take a 1024x768 screenshot, crop it to 768x768, and get it scaled down to 300x300."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "029c1b93-9a86-40ea-9bcd-7d199d698dc1"
            }
          ]
        },
        {
          "id": "cc438bb0-a87e-4b35-b8ed-6405a3864617",
          "name": "GetThumbnail",
          "request": {
            "url": "http://api.browshot.com/api/v1/screenshot/thumbnail?bottom=%7B%7D&format=%7B%7D&height=%7B%7D&id=%7B%7D&left=%7B%7D&quality=%7B%7D&ratio=%7B%7D&right=%7B%7D&scale=%7B%7D&shot=%7B%7D&top=%7B%7D&width=%7B%7D&zoom=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Unlike the other API calls, this API sends back the thumbnail as a PNG file, not JSON. The HTTP response code indicates whether the screenshot was successful (200), or incomplete (404) or failed (404). If the screenshot failed or is not finished, a default image \"Not found\" is sent.\n\nYou can crop your screenshots. The crop is done first, then the thumbnail. You can take a 1024x768 screenshot, crop it to 768x768, and get it scaled down to 300x300."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b556b7e6-68db-4d93-84e9-1260457def41"
            }
          ]
        }
      ]
    }
  ]
}