{
  "info": {
    "name": "AWS Code Pipeline API Update Pipeline",
    "_postman_id": "4b13b68d-b843-4c8f-8ee5-7a4755ccd518",
    "description": "Updates a specified pipeline with edits or changes to its structure.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Acknowledge",
      "item": [
        {
          "id": "1cdcd5cf-073a-4dac-bead-fe1cfcf94795",
          "name": "acknowledgeJob",
          "request": {
            "url": "http://example.com/api/?Action=AcknowledgeJob?DryRun=DryRun&jobId=jobId&nonce=nonce&SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specified job and whether that job has been received by\n            the job worker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b77b227a-49a2-42ae-8451-86092623ac26"
            }
          ]
        },
        {
          "id": "29275e9c-3b20-4b67-a96c-e506ee658cda",
          "name": "acknowledgeThirdPartyJob",
          "request": {
            "url": "http://example.com/api/?Action=AcknowledgeThirdPartyJob?clientToken=clientToken&DryRun=DryRun&jobId=jobId&nonce=nonce&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Confirms a job worker has received the specified job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf0d9f5f-2c54-4ecb-afca-4e8ed4b55dfb"
            }
          ]
        }
      ]
    },
    {
      "name": "Custom",
      "item": [
        {
          "id": "bafb5cf1-20e3-4a86-bf75-6a1e876804a8",
          "name": "createCustomActionType",
          "request": {
            "url": "http://example.com/api/?Action=CreateCustomActionType?Attribute=Attribute&category=category&configurationProperties=configurationProperties&DryRun=DryRun&inputArtifactDetails=inputArtifactDetails&outputArtifactDetails=outputArtifactDetails&provider=provider&settings=settings&SnapshotId=SnapshotId&version=version",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new custom action that can be used in all pipelines associated with the\n            AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e26bb86-a63e-401c-b38c-aaced9cf991d"
            }
          ]
        },
        {
          "id": "ab1ffe7e-791c-432e-8914-14855de52805",
          "name": "deleteCustomActionType",
          "request": {
            "url": "http://example.com/api/?Action=DeleteCustomActionType?Attribute=Attribute&category=category&DryRun=DryRun&provider=provider&version=version&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Marks a custom action as deleted."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4877ad0c-226d-471a-b00a-04d3cddf4b75"
            }
          ]
        }
      ]
    },
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "c8a20685-309e-47f1-bb2d-efbefdcbc73f",
          "name": "createPipeline",
          "request": {
            "url": "http://example.com/api/?Action=CreatePipeline?DryRun=DryRun&Filter.N=Filter.N&MaxResults=MaxResults&NextToken=NextToken&Owner.N=Owner.N&pipeline=pipeline&RestorableBy.N=RestorableBy.N&SnapshotId.N=SnapshotId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2fe739e-53b7-41dd-bb29-07c101706618"
            }
          ]
        },
        {
          "id": "b3c4d99e-4e55-441f-8c46-4a931deded69",
          "name": "deletePipeline",
          "request": {
            "url": "http://example.com/api/?Action=DeletePipeline?DryRun=DryRun&Filter.N=Filter.N&MaxResults=MaxResults&name=name&NextToken=NextToken&VolumeId.N=VolumeId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a2ca0de-2863-47a5-9ee1-c24972774a80"
            }
          ]
        },
        {
          "id": "a8cf8e2a-f3ac-4907-a1c2-01696c975e49",
          "name": "getPipeline",
          "request": {
            "url": "http://example.com/api/?Action=GetPipeline?Attribute=Attribute&CreateVolumePermission=CreateVolumePermission&DryRun=DryRun&name=name&OperationType=OperationType&SnapshotId=SnapshotId&UserGroup.N=UserGroup.N&UserId.N=UserId.N&version=version",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the metadata, structure, stages, and actions of a pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3bed84aa-ac95-416d-9a78-2d10c5fad853"
            }
          ]
        },
        {
          "id": "0cf59e6e-e50e-4fc2-a175-d17dc8f4167c",
          "name": "getPipelineExecution",
          "request": {
            "url": "http://example.com/api/?Action=GetPipelineExecution?AutoEnableIO=AutoEnableIO&DryRun=DryRun&pipelineExecutionId=pipelineExecutionId&pipelineName=pipelineName&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about an execution of a pipeline, including details about\n            artifacts, the pipeline execution ID, and the name, version, and status of the\n            pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95cb89a6-0204-4b5c-957a-7ea3bcb88ac0"
            }
          ]
        },
        {
          "id": "dedae4cd-c3b0-4d9e-905a-87459162c8de",
          "name": "getPipelineState",
          "request": {
            "url": "http://example.com/api/?Action=GetPipelineState?Attribute=Attribute&DryRun=DryRun&name=name&SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the state of a pipeline, including the stages and\n            actions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93031be3-3a7a-48b9-b54c-e6bc1a92a824"
            }
          ]
        },
        {
          "id": "a91b8d8c-2248-497a-b146-4bea9521fc20",
          "name": "updatePipeline",
          "request": {
            "url": "http://example.com/api/?Action=UpdatePipeline?Attribute=Attribute&DryRun=DryRun&NetworkInterfaceId=NetworkInterfaceId&pipeline=pipeline",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a specified pipeline with edits or changes to its structure."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e245b420-c697-436c-8890-d345e0f7e33e"
            }
          ]
        }
      ]
    },
    {
      "name": "Disable",
      "item": [
        {
          "id": "545ccf41-fac9-49f2-aceb-2830adf39cff",
          "name": "disableStageTransition",
          "request": {
            "url": "http://example.com/api/?Action=DisableStageTransition?DryRun=DryRun&Filter.N=Filter.N&MaxResults=MaxResults&NextToken=NextToken&pipelineName=pipelineName&reason=reason&stageName=stageName&transitionType=transitionType&VolumeId.N=VolumeId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Prevents artifacts in a pipeline from transitioning to the next stage in the\n            pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70bb9a52-c5b2-4fec-a8c1-963a8218fa40"
            }
          ]
        }
      ]
    },
    {
      "name": "Enable",
      "item": [
        {
          "id": "31460bcc-a171-4c81-9965-802b83d1d0b2",
          "name": "enableStageTransition",
          "request": {
            "url": "http://example.com/api/?Action=EnableStageTransition?Device=Device&DryRun=DryRun&Force=Force&InstanceId=InstanceId&pipelineName=pipelineName&stageName=stageName&transitionType=transitionType&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables artifacts in a pipeline to transition to a stage in a pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ccf6c0f-5443-4da1-abea-3c0c82145904"
            }
          ]
        }
      ]
    },
    {
      "name": "Job",
      "item": [
        {
          "id": "3dc9f547-3816-4d85-aca6-89ad4b03a9ee",
          "name": "getJobDetails",
          "request": {
            "url": "http://example.com/api/?Action=GetJobDetails?DryRun=DryRun&jobId=jobId&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18b7fb00-7c15-4e01-9070-1d832f960232"
            }
          ]
        }
      ]
    },
    {
      "name": "Third",
      "item": [
        {
          "id": "c6d4252c-6153-4ade-9f2e-481e1f51c18d",
          "name": "getThirdPartyJobDetails",
          "request": {
            "url": "http://example.com/api/?Action=GetThirdPartyJobDetails?clientToken=clientToken&Domain=Domain&DryRun=DryRun&jobId=jobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Requests the details of a job for a third party action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3314bfc1-54e6-4802-97ab-38458bdd09eb"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "a7cb9e15-730a-4582-9321-3873a323f9bd",
          "name": "listActionTypes",
          "request": {
            "url": "http://example.com/api/?Action=ListActionTypes?actionOwnerFilter=actionOwnerFilter&AllocationId=AllocationId&AllowReassociation=AllowReassociation&DryRun=DryRun&InstanceId=InstanceId&NetworkInterfaceId=NetworkInterfaceId&nextToken=nextToken&PrivateIpAddress=PrivateIpAddress&PublicIp=PublicIp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a summary of all AWS CodePipeline action types associated with your\n            account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd2fd09d-eda0-4a74-8d17-2e9a7202427c"
            }
          ]
        },
        {
          "id": "9da8fd0a-c87a-4b59-ab7d-498a7b59c2a2",
          "name": "listPipelines",
          "request": {
            "url": "http://example.com/api/?Action=ListPipelines?AllocationId.N=AllocationId.N&DryRun=DryRun&Filter.N=Filter.N&nextToken=nextToken&PublicIp.N=PublicIp.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a summary of all of the pipelines associated with your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b462e97f-54f0-4f86-857f-60881292504c"
            }
          ]
        }
      ]
    },
    {
      "name": "PollJobs",
      "item": [
        {
          "id": "a9493143-722f-42a3-aeed-d03ebbf63048",
          "name": "pollForJobs",
          "request": {
            "url": "http://example.com/api/?Action=PollForJobs?actionTypeId=actionTypeId&DryRun=DryRun&Filter.N=Filter.N&maxBatchSize=maxBatchSize&MaxResults=MaxResults&NextToken=NextToken&PublicIp.N=PublicIp.N&queryParam=queryParam",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about any jobs for AWS CodePipeline to act upon."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc2bc385-4ccb-4e8a-8c71-ba1d90de3c05"
            }
          ]
        }
      ]
    },
    {
      "name": "PollThird",
      "item": [
        {
          "id": "76d24cea-95ae-4caa-99b9-c8ef775384a8",
          "name": "pollForThirdPartyJobs",
          "request": {
            "url": "http://example.com/api/?Action=PollForThirdPartyJobs?actionTypeId=actionTypeId&AssociationId=AssociationId&DryRun=DryRun&maxBatchSize=maxBatchSize&PublicIp=PublicIp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Determines whether there are any third party jobs for a job worker to act on."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d1e8730-b80f-4ef8-898d-9df7e4793206"
            }
          ]
        }
      ]
    },
    {
      "name": "Put",
      "item": [
        {
          "id": "288a5965-aee3-485b-ba75-572e4613d0ad",
          "name": "putActionRevision",
          "request": {
            "url": "http://example.com/api/?Action=PutActionRevision?actionName=actionName&actionRevision=actionRevision&DryRun=DryRun&pipelineName=pipelineName&PublicIp=PublicIp&stageName=stageName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides information to AWS CodePipeline about new revisions to a source."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5509518-3119-4e68-961e-78717e70cf36"
            }
          ]
        },
        {
          "id": "1797fc18-179b-4bf4-9b25-fe3733cbbce6",
          "name": "putApprovalResult",
          "request": {
            "url": "http://example.com/api/?Action=PutApprovalResult?actionName=actionName&AllocationId=AllocationId&DryRun=DryRun&pipelineName=pipelineName&PublicIp=PublicIp&result=result&stageName=stageName&token=token",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides the response to a manual approval request to AWS CodePipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24dc89a1-3682-4c4d-80c1-21a5393cf1fa"
            }
          ]
        },
        {
          "id": "2e32cf7f-7824-4641-a1d4-0370d354f088",
          "name": "putJobFailureResult",
          "request": {
            "url": "http://example.com/api/?Action=PutJobFailureResult?DryRun=DryRun&failureDetails=failureDetails&jobId=jobId&PublicIp=PublicIp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Represents the failure of a job as returned to the pipeline by a job worker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72a5a297-c9c4-4ea9-8ad7-395d0ca5c205"
            }
          ]
        },
        {
          "id": "d5486c33-42af-46f2-9867-36d13b26a243",
          "name": "putJobSuccessResult",
          "request": {
            "url": "http://example.com/api/?Action=PutJobSuccessResult?continuationToken=continuationToken&currentRevision=currentRevision&executionDetails=executionDetails&Ipv6AddressCount=Ipv6AddressCount&Ipv6Addresses.N=Ipv6Addresses.N&jobId=jobId&NetworkInterfaceId=NetworkInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Represents the success of a job as returned to the pipeline by a job worker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36ba1868-1e57-49ea-a900-95df5d64f825"
            }
          ]
        },
        {
          "id": "921645fb-63ec-464a-bd1d-320fecb0afc1",
          "name": "putThirdPartyJobFailureResult",
          "request": {
            "url": "http://example.com/api/?Action=PutThirdPartyJobFailureResult?AllowReassignment=AllowReassignment&clientToken=clientToken&failureDetails=failureDetails&jobId=jobId&NetworkInterfaceId=NetworkInterfaceId&PrivateIpAddress.N=PrivateIpAddress.N&SecondaryPrivateIpAddressCount=SecondaryPrivateIpAddressCount",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Represents the failure of a third party job as returned to the pipeline by a job\n            worker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f3d127e-d69f-45db-ae09-0a54e24a3881"
            }
          ]
        },
        {
          "id": "c1dd116a-cb9d-4736-b8d9-b291560edb7e",
          "name": "putThirdPartyJobSuccessResult",
          "request": {
            "url": "http://example.com/api/?Action=PutThirdPartyJobSuccessResult?clientToken=clientToken&continuationToken=continuationToken&currentRevision=currentRevision&DeviceIndex=DeviceIndex&DryRun=DryRun&executionDetails=executionDetails&InstanceId=InstanceId&jobId=jobId&NetworkInterfaceId=NetworkInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Represents the success of a third party job as returned to the pipeline by a job\n            worker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fde9398e-1be2-4fe4-a0a4-8d9d6dc296ed"
            }
          ]
        }
      ]
    },
    {
      "name": "Retry",
      "item": [
        {
          "id": "1db9d4b7-37ae-4707-8392-450ed3056837",
          "name": "retryStageExecution",
          "request": {
            "url": "http://example.com/api/?Action=RetryStageExecution?Description=Description&DryRun=DryRun&Ipv6AddressCount=Ipv6AddressCount&Ipv6Addresses.N=Ipv6Addresses.N&pipelineExecutionId=pipelineExecutionId&pipelineName=pipelineName&PrivateIpAddress=PrivateIpAddress&PrivateIpAddresses.N=PrivateIpAddresses.N&retryMode=retryMode&SecondaryPrivateIpAddressCount=SecondaryPrivateIpAddressCount&SecurityGroupId.N=SecurityGroupId.N&stageName=stageName&SubnetId=SubnetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Resumes the pipeline execution by retrying the last failed actions in a\n            stage."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3a7c15c-8239-4fd1-9361-a255cb5fe6b3"
            }
          ]
        }
      ]
    },
    {
      "name": "Start",
      "item": [
        {
          "id": "15964292-c28b-41f5-8b32-4cff1ac7ee74",
          "name": "startPipelineExecution",
          "request": {
            "url": "http://example.com/api/?Action=StartPipelineExecution?DryRun=DryRun&name=name&NetworkInterfaceId=NetworkInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts the specified pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10d8aa03-16bd-4485-9854-08efa7697440"
            }
          ]
        }
      ]
    }
  ]
}