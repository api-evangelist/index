{
  "info": {
    "name": "SYNQ Video Return embeddable url to an uploader widget",
    "_postman_id": "f5948638-37b6-4dfa-a4f5-4f4367eec62e",
    "description": "Returns an embeddable url, that contains an uploader widget that allows you to easily upload any mp4. Great way to simplify the uploading process for end users.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Video",
      "item": [
        {
          "id": "38e5bf97-c5e9-44ab-a86a-b43fa482b78e",
          "name": "create",
          "request": {
            "url": "http://api.synq.fm/v1/video/create",
            "method": "POST",
            "header": [
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
                  "key": "api_key",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "userdata",
                  "value": "{}",
                  "disabled": false,
                  "description": "Additional metadata that will be associated with the video"
                }
              ]
            },
            "description": "Create a new video, optionally setting some metadata fields. You may optionally set some of the metadata associated with the video. Only fields inside the \"userdata\" field can be set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "543dad26-67e9-45f1-83bf-5208288865f7"
            }
          ]
        },
        {
          "id": "d27d00ec-1fc7-43ea-bb9e-8f3682bce7ad",
          "name": "details",
          "request": {
            "url": "http://api.synq.fm/v1/video/details",
            "method": "POST",
            "header": [
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
                  "key": "api_key",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "video_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "ID of the video to retrieve the metadata from"
                }
              ]
            },
            "description": "Return details about a video. You may optionally request that only some of the metadata fields are returned."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0a13f19-0bb8-4c9f-b282-df5b9efe1b75"
            }
          ]
        },
        {
          "id": "d65d92db-1782-44ac-b0d9-abe3381707cb",
          "name": "query",
          "request": {
            "url": "http://api.synq.fm/v1/video/query",
            "method": "POST",
            "header": [
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
                  "key": "api_key",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "filter",
                  "value": "{}",
                  "disabled": false,
                  "description": "JavaScript code to be run over each video object, to determine what should be returend"
                }
              ]
            },
            "description": "Find videos matching any criteria, by running a JavaScript function over each video object. A detailed tutorial on how to use this functionality is available on the [documentation page](https://www.synq.fm/queries-video-api/)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3cc6211-861f-469e-b315-7ac6611a6a9d"
            }
          ]
        },
        {
          "id": "b69181b1-01b6-4fb6-88b8-b28f9b346960",
          "name": "stream",
          "request": {
            "url": "http://api.synq.fm/v1/video/stream",
            "method": "POST",
            "header": [
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
                  "key": "api_key",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "video_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of the video you want to stream to"
                }
              ]
            },
            "description": "Returns a stream url that you can stream to from your broadcasting software, and a playback url people can use to watch the stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b63c549-8c16-467b-92de-832a3de03c24"
            }
          ]
        },
        {
          "id": "c144ce82-f7d7-4097-80d4-3cde4916a7fa",
          "name": "update",
          "request": {
            "url": "http://api.synq.fm/v1/video/update",
            "method": "POST",
            "header": [
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
                  "key": "api_key",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "source",
                  "value": "{}",
                  "disabled": false,
                  "description": "JavaScript code to execute on the video object"
                },
                {
                  "key": "video_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of the video whose metadata will be updated"
                }
              ]
            },
            "description": "Update a video's metadata through JavaScript code. Only fields inside the \"userdata\" object can be set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5200142e-74b2-4a42-bcf8-064bb7fafbb3"
            }
          ]
        },
        {
          "id": "796305b7-1ac3-4b19-9305-6deb1417ddce",
          "name": "upload",
          "request": {
            "url": "http://api.synq.fm/v1/video/upload",
            "method": "POST",
            "header": [
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
                  "key": "api_key",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "video_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of the video you are going to upload into"
                }
              ]
            },
            "description": "Return parameters needed for uploading a video file to Amazon Simple Storage Service. See http://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-post-example.html as well as the language-specific code-examples.\n#### *Example request*\n```shell\ncurl -s https://api.synq.fm/v1/video/upload \\\n  -F api_key=${SYNQ_API_KEY} \\\n  -F video_id=2d81c30ce62f4dfdb501dbca96c7ae56\n```\n\n#### *Example response*\n```json\n{\n  \"action\": \"https://synqfm.s3.amazonaws.com/\",\n  \"AWSAccessKeyId\": \"AKIAIP77Y7MMX3ITZMFA\",\n  \"Content-Type\": \"video/mp4\",\n  \"Policy\": \"eyJleHBpcmF0aW9uIiA6ICIyMDE2LTA0LTIyVDE5OjAyOjI2LjE3MloiLCAiY29uZGl0aW9ucyIgOiBbeyJidWNrZXQiIDogInN5bnFmbSJ9LCB7ImFjbCIgOiAicHVibGljLXJlYWQifSwgWyJzdGFydHMtd2l0aCIsICIka2V5IiwgInByb2plY3RzLzZlLzYzLzZlNjNiNzUyYTE4NTRkZGU4ODViNWNjNDcyZWRmNTY5L3VwbG9hZHMvdmlkZW9zLzJkLzgxLzJkODFjMzBjZTYyZjRkZmRiNTAxZGJjYTk2YzdhZTU2Lm1wNCJdLCBbInN0YXJ0cy13aXRoIiwgIiRDb250ZW50LVR5cGUiLCAidmlkZW8vbXA0Il0sIFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLCAwLCAxMDk5NTExNjI3Nzc2XV19\",\n  \"Signature\": \"ysqDemlKXKr6hKzVFP0hCGgf/cs=\",\n  \"acl\": \"public-read\",\n  \"key\": \"projects/6e/63/6e63b752a1854dde885b5cc472edf569/uploads/videos/2d/81/2d81c30ce62f4dfdb501dbca96c7ae56.mp4\"\n}\n```\n\nTo upload the file, you can then make a multipart POST request to the URL in `action`, and for all the other parameters returned, set them as form parameters.\n\nGiven the parameters above, you would upload a file `test.mp4` using cURL like this:\n\n```shell\ncurl -s https://synqfm.s3.amazonaws.com/ \\\n  -F AWSAccessKeyId=\"AKIAIP77Y7MMX3ITZMFA\" \\\n  -F Content-Type=\"video/mp4\" \\\n  -F Policy=\"eyJleHBpcmF0aW9uIiA6ICIyMDE2LTA0LTIyVDE5OjAyOjI2LjE3MloiLCAiY29uZGl0aW9ucyIgOiBbeyJidWNrZXQiIDogInN5bnFmbSJ9LCB7ImFjbCIgOiAicHVibGljLXJlYWQifSwgWyJzdGFydHMtd2l0aCIsICIka2V5IiwgInByb2plY3RzLzZlLzYzLzZlNjNiNzUyYTE4NTRkZGU4ODViNWNjNDcyZWRmNTY5L3VwbG9hZHMvdmlkZW9zLzJkLzgxLzJkODFjMzBjZTYyZjRkZmRiNTAxZGJjYTk2YzdhZTU2Lm1wNCJdLCBbInN0YXJ0cy13aXRoIiwgIiRDb250ZW50LVR5cGUiLCAidmlkZW8vbXA0Il0sIFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLCAwLCAxMDk5NTExNjI3Nzc2XV19\" \\\n  -F Signature=\"ysqDemlKXKr6hKzVFP0hCGgf/cs=\" \\\n  -F acl=\"public-read\" \\\n  -F key=\"projects/6e/63/6e63b752a1854dde885b5cc472edf569/uploads/videos/2d/81/2d81c30ce62f4dfdb501dbca96c7ae56.mp4\" \\\n  -F file=\"@my_video_file.mp4\"\n```"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b15f5599-33f5-4d76-b080-a1cf845ce089"
            }
          ]
        },
        {
          "id": "eb39e5ca-70e4-468e-9e76-50cd0c780bcd",
          "name": "uploader",
          "request": {
            "url": "http://api.synq.fm/v1/video/uploader",
            "method": "POST",
            "header": [
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
                  "key": "api_key",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "timeout",
                  "value": "{}",
                  "disabled": false,
                  "description": "How long the uploader widget works for"
                },
                {
                  "key": "video_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of the video you are going to upload into"
                }
              ]
            },
            "description": "Returns an embeddable url, that contains an uploader widget that allows you to easily upload any mp4. Great way to simplify the uploading process for end users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1212f43b-4ef2-4be5-bb51-6f0819bf6506"
            }
          ]
        }
      ]
    }
  ]
}