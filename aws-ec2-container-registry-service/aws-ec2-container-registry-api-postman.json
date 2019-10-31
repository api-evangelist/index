{
  "info": {
    "name": "AWS EC2 Container Registry API Upload Layer Part",
    "_postman_id": "c5281463-13d2-4314-8ac8-11d6b8109765",
    "description": "Uploads an image layer part to Amazon ECR.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Layer Availability",
      "item": [
        {
          "id": "fefd241a-6bba-4de4-9af1-32bb94e52e26",
          "name": "batchCheckLayerAvailability",
          "request": {
            "url": "http://example.com/api/?Action=BatchCheckLayerAvailability?layerDigests=layerDigests&registryId=registryId&repositoryName=repositoryName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Check the availability of multiple image layers in a specified registry and repository."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "405a320f-1795-4dc0-bf2c-8a5588982d39"
            }
          ]
        }
      ]
    },
    {
      "name": "Image",
      "item": [
        {
          "id": "acc9ecdf-c686-4ddb-a9f2-d846b599a9f2",
          "name": "batchDeleteImage",
          "request": {
            "url": "http://example.com/api/?Action=BatchDeleteImage?imageIds=imageIds&registryId=registryId&repositoryName=repositoryName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a list of specified images within a specified repository."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15341e17-dbc1-4bd3-8fe9-08cff9af945a"
            }
          ]
        },
        {
          "id": "f2074abf-c5b6-4eca-8730-49a944cf32e8",
          "name": "batchGetImage",
          "request": {
            "url": "http://example.com/api/?Action=BatchGetImage?acceptedMediaTypes=acceptedMediaTypes&imageIds=imageIds&registryId=registryId&repositoryName=repositoryName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets detailed information for specified images within a specified repository."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf7ff5cf-a6e0-482b-8592-65eadd9b375d"
            }
          ]
        }
      ]
    },
    {
      "name": "Layer Upload",
      "item": [
        {
          "id": "e4d85555-dbe3-4ccf-963f-1774947c51c1",
          "name": "completeLayerUpload",
          "request": {
            "url": "http://example.com/api/?Action=CompleteLayerUpload",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Inform Amazon ECR that the image layer upload for a specified registry, repository name, and upload ID, has completed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c3fec6a-1854-4592-b061-158adc7a00cb"
            }
          ]
        },
        {
          "id": "e4b35e3c-32d9-495e-aa81-6ad23a9a165f",
          "name": "initiateLayerUpload",
          "request": {
            "url": "http://example.com/api/?Action=InitiateLayerUpload",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Notify Amazon ECR that you intend to upload an image layer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a605f8a3-de01-4724-85ec-d93ea94ba054"
            }
          ]
        }
      ]
    },
    {
      "name": "Repositories",
      "item": [
        {
          "id": "d432947d-33ca-47fd-a4b8-581cfeb81f17",
          "name": "createRepository",
          "request": {
            "url": "http://example.com/api/?Action=CreateRepository?repositoryName=repositoryName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an image repository."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86ce5233-c42d-449c-b985-153ac2031e6d"
            }
          ]
        },
        {
          "id": "acd8ab22-5fc0-4352-9a5d-8f929c8edfab",
          "name": "deleteRepository",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRepository?force=force&registryId=registryId&repositoryName=repositoryName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an existing image repository."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa9842d3-a2d0-4c82-a359-6f9ff65cfe5a"
            }
          ]
        },
        {
          "id": "e6c626a5-71b2-4cad-b86f-716c7a12560b",
          "name": "describeRepositories",
          "request": {
            "url": "http://example.com/api/?Action=DescribeRepositories?maxResults=maxResults&nextToken=nextToken&registryId=registryId&repositoryNames=repositoryNames",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes image repositories in a registry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cdda114e-4d78-4e58-b2d1-2001ad2e11d3"
            }
          ]
        }
      ]
    },
    {
      "name": "Repository Policies",
      "item": [
        {
          "id": "e09f0a28-8e59-4ffd-b5cb-1cadf8643f44",
          "name": "deleteRepositoryPolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRepositoryPolicy?registryId=registryId&repositoryName=repositoryName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the repository policy from a specified repository."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "652508ab-1968-4870-89f2-483a6a05c926"
            }
          ]
        },
        {
          "id": "887a4580-1d9e-42c1-a1e5-b81bf7ef374b",
          "name": "getRepositoryPolicy",
          "request": {
            "url": "http://example.com/api/?Action=GetRepositoryPolicy?registryId=registryId&repositoryName=repositoryName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the repository policy for a specified repository."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b05ef986-558b-466d-8244-11435e25ed99"
            }
          ]
        },
        {
          "id": "bcd2d328-5a41-4979-bbbd-661ae4f04617",
          "name": "setRepositoryPolicy",
          "request": {
            "url": "http://example.com/api/?Action=SetRepositoryPolicy?force=force&policyText=policyText&registryId=registryId&repositoryName=repositoryName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Applies a repository policy on a specified repository to control access permissions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc2cc097-0098-4a83-b315-cad03a4bf39f"
            }
          ]
        }
      ]
    },
    {
      "name": "Images",
      "item": [
        {
          "id": "3da73c4d-3539-414a-af4f-dd2a9ed918ac",
          "name": "describeImages",
          "request": {
            "url": "http://example.com/api/?Action=DescribeImages?filter=filter&imageIds=imageIds&maxResults=maxResults&nextToken=nextToken&registryId=registryId&repositoryName=repositoryName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metadata about the images in a repository, including image size, image\n            tags, and creation date."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa0c57bb-9d1f-4b2f-9100-7ca13c29bd9e"
            }
          ]
        },
        {
          "id": "26f3b03b-5488-4d70-8048-9bd023821aaa",
          "name": "listImages",
          "request": {
            "url": "http://example.com/api/?Action=ListImages?filter=filter&maxResults=maxResults&nextToken=nextToken&registryId=registryId&repositoryName=repositoryName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the image IDs for a given repository."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3266ddb-a89a-438c-9f7c-acec4d90aa66"
            }
          ]
        },
        {
          "id": "a35366fb-a461-41c8-81e8-43e088baba9f",
          "name": "putImage",
          "request": {
            "url": "http://example.com/api/?Action=PutImage?imageManifest=imageManifest&imageTag=imageTag&registryId=registryId&repositoryName=repositoryName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates or updates the image manifest and tags associated with an image."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90948f0f-2954-4d2a-b2a0-2ebdb078c1ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Authorization Tokens",
      "item": [
        {
          "id": "9b036cd4-a9ff-4528-832d-70028a4097d1",
          "name": "getAuthorizationToken",
          "request": {
            "url": "http://example.com/api/?Action=GetAuthorizationToken?registryIds=registryIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a token that is valid for a specified registry for 12 hours."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a5e9e3c-efee-4593-98a1-c05353f25566"
            }
          ]
        }
      ]
    },
    {
      "name": "Layers",
      "item": [
        {
          "id": "d6d36e3d-3fe4-48e6-a11f-1cd396cc190d",
          "name": "getDownloadUrlForLayer",
          "request": {
            "url": "http://example.com/api/?Action=GetDownloadUrlForLayer",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": ".Retrieves the pre-signed Amazon S3 download URL corresponding to an image layer. You can only get URLs for image layers that are referenced in an image."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c07d2aa9-ac34-4f1a-b48f-5837b630d9c3"
            }
          ]
        }
      ]
    },
    {
      "name": "Layer Parts",
      "item": [
        {
          "id": "e9a1e78b-71ff-4d50-b0bd-6a39ec20b045",
          "name": "uploadLayerPart",
          "request": {
            "url": "http://example.com/api/?Action=UploadLayerPart",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Uploads an image layer part to Amazon ECR."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba20e423-a4fe-4eff-b488-c3cc08c0c3db"
            }
          ]
        }
      ]
    }
  ]
}