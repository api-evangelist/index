{
  "info": {
    "name": "AWS Directory Service API Verify Trust",
    "_postman_id": "a99b2113-a864-4de5-b2a6-241ae5ff1bd7",
    "description": "AWS Directory Service for Microsoft Active Directory allows you to configure and verify trust relationships.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "IP Address Routes",
      "item": [
        {
          "id": "38ff7e36-8d8c-4d47-a60c-fe94eea8ac0d",
          "name": "addIpRoutes",
          "request": {
            "url": "http://example.com/api/?Action=AddIpRoutes?DirectoryId=DirectoryId&IpRoutes=IpRoutes&UpdateSecurityGroupForDirectoryControllers=UpdateSecurityGroupForDirectoryControllers",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "If the DNS server for your on-premises domain uses a publicly addressable IP address, you must add a CIDR address block to correctly route traffic to and from your Microsoft AD on Amazon Web Services."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "300288c6-eb0e-4702-ab15-615674ba301b"
            }
          ]
        },
        {
          "id": "e1e528e1-6db6-400d-92f0-da4c2ad2f281",
          "name": "listIpRoutes",
          "request": {
            "url": "http://example.com/api/?Action=ListIpRoutes?DirectoryId=DirectoryId&Limit=Limit&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the address blocks that you have added to a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8a38b12-b127-40fc-9984-96b4bc7d70e4"
            }
          ]
        },
        {
          "id": "6bf8fb50-7b2f-4783-ab0a-836ea64f12db",
          "name": "removeIpRoutes",
          "request": {
            "url": "http://example.com/api/?Action=RemoveIpRoutes?CidrIps=CidrIps&DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes IP address blocks from a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4815851b-d29e-40ba-be2f-31913383d559"
            }
          ]
        }
      ]
    },
    {
      "name": "Resource Tags",
      "item": [
        {
          "id": "e0798c39-200f-490e-be5e-9b450effb2e4",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceId=ResourceId&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or overwrites one or more tags for the specified directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db5c1d01-2318-427e-bb35-114cc1e1dc94"
            }
          ]
        },
        {
          "id": "8228dc4d-0d1b-4dff-b823-83cadaebe40f",
          "name": "listTagsForResource",
          "request": {
            "url": "http://example.com/api/?Action=ListTagsForResource?Limit=Limit&NextToken=NextToken&ResourceId=ResourceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all tags on a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd25f5d9-34bf-45a9-89b1-1d89b1e809a5"
            }
          ]
        },
        {
          "id": "508e653c-b022-42ac-81a8-b1eac9f088c6",
          "name": "removeTagsFromResource",
          "request": {
            "url": "http://example.com/api/?Action=RemoveTagsFromResource?ResourceId=ResourceId&TagKeys=TagKeys",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes tags from a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b905514-6f12-41e7-9d41-1d67b998bedf"
            }
          ]
        }
      ]
    },
    {
      "name": "Schemas",
      "item": [
        {
          "id": "d9e1daf3-9015-4ed1-8f81-be9d5a45a915",
          "name": "cancelSchemaExtension",
          "request": {
            "url": "http://example.com/api/?Action=CancelSchemaExtension?DirectoryId=DirectoryId&SchemaExtensionId=SchemaExtensionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels an in-progress schema extension to a Microsoft AD directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2ed62e2-bf59-4559-9142-5cf444c72cce"
            }
          ]
        }
      ]
    },
    {
      "name": "Directories",
      "item": [
        {
          "id": "4598ee71-cfcd-4984-ad30-b6d7648ab77c",
          "name": "connectDirectory",
          "request": {
            "url": "http://example.com/api/?Action=ConnectDirectory?ConnectSettings=ConnectSettings&Description=Description&Name=Name&Password=Password&ShortName=ShortName&Size=Size",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an AD Connector to connect to an on-premises directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "acc0e355-b464-4451-bc5b-22eb5bb1ed19"
            }
          ]
        },
        {
          "id": "b52633b3-d67f-412e-8008-1999e9ed4489",
          "name": "createDirectory",
          "request": {
            "url": "http://example.com/api/?Action=CreateDirectory?Description=Description&Name=Name&Password=Password&ShortName=ShortName&Size=Size&VpcSettings=VpcSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a Simple AD directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f38acbe0-29b3-492d-8608-167fdc96da01"
            }
          ]
        },
        {
          "id": "4083b0c4-1358-4dbb-a32f-a87e34725d1a",
          "name": "deleteDirectory",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDirectory?DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an AWS Directory Service directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc9b061d-b632-48d9-8f4b-da3cc7780ffa"
            }
          ]
        },
        {
          "id": "da3991f1-d772-4328-b8df-8b9a8d176ec3",
          "name": "describeDirectories",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDirectories?DirectoryIds=DirectoryIds&Limit=Limit&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about the directories that belong to this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "455e6e17-9199-4841-873d-cb781eebe2e0"
            }
          ]
        },
        {
          "id": "19f4b8e1-7272-45bd-b0ba-edf2a5c6d3bb",
          "name": "getDirectoryLimits",
          "request": {
            "url": "http://example.com/api/?Action=GetDirectoryLimits?DirectoryLimits=DirectoryLimits",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains directory limit information for the current region."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "680e98ab-9964-4fcf-a19f-563fa1ba7c4b"
            }
          ]
        }
      ]
    },
    {
      "name": "Alias",
      "item": [
        {
          "id": "aec36372-cce5-400f-8d4c-236a36a2e378",
          "name": "createAlias",
          "request": {
            "url": "http://example.com/api/?Action=CreateAlias?Alias=Alias&DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an alias for a directory and assigns the alias to the directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7de45e9-31a4-4b6f-97cb-be623af2352c"
            }
          ]
        }
      ]
    },
    {
      "name": "Computer",
      "item": [
        {
          "id": "04f45b68-e329-4ad7-b482-92c4aa8d1a35",
          "name": "createComputer",
          "request": {
            "url": "http://example.com/api/?Action=CreateComputer?ComputerAttributes=ComputerAttributes&ComputerName=ComputerName&DirectoryId=DirectoryId&OrganizationalUnitDistinguishedName=OrganizationalUnitDistinguishedName&Password=Password",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a computer account in the specified directory, and joins the computer to the directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6be1e5d-252a-4254-8428-0d631022c3a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Conditional Forwarder",
      "item": [
        {
          "id": "746f5469-66f9-481b-81aa-1ab8240b3174",
          "name": "createConditionalForwarder",
          "request": {
            "url": "http://example.com/api/?Action=CreateConditionalForwarder?DirectoryId=DirectoryId&DnsIpAddrs=DnsIpAddrs&RemoteDomainName=RemoteDomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a conditional forwarder associated with your AWS directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98d5d093-0518-4314-af65-d23c7a6dc26c"
            }
          ]
        },
        {
          "id": "30c260ad-3b97-4e91-b2be-72e016827cf2",
          "name": "deleteConditionalForwarder",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConditionalForwarder?DirectoryId=DirectoryId&RemoteDomainName=RemoteDomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a conditional forwarder that has been set up for your AWS directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58069274-80c8-4dff-88e7-4799d728cb3c"
            }
          ]
        },
        {
          "id": "11e12892-4e6d-4e71-80a6-79fc3b948fc6",
          "name": "describeConditionalForwarders",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConditionalForwarders?DirectoryId=DirectoryId&RemoteDomainNames=RemoteDomainNames",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about the conditional forwarders for this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e2a4495-a927-4c06-bb24-f1017ac0b4f2"
            }
          ]
        },
        {
          "id": "62b1abc9-2d28-4678-8678-84b6191ba0f7",
          "name": "updateConditionalForwarder",
          "request": {
            "url": "http://example.com/api/?Action=UpdateConditionalForwarder?DirectoryId=DirectoryId&DnsIpAddrs=DnsIpAddrs&RemoteDomainName=RemoteDomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a conditional forwarder that has been set up for your AWS directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "458bf09d-ad9c-4afa-84f2-8100f890d62e"
            }
          ]
        }
      ]
    },
    {
      "name": "Microsoft AD",
      "item": [
        {
          "id": "c2f8e82b-456a-44bf-8de5-7608fdf20ec8",
          "name": "createMicrosoftAD",
          "request": {
            "url": "http://example.com/api/?Action=CreateMicrosoftAD?Description=Description&Name=Name&Password=Password&ShortName=ShortName&VpcSettings=VpcSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a Microsoft AD in the AWS cloud."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3c54711-7466-417a-8cb7-4aada47a0961"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshot",
      "item": [
        {
          "id": "e91990a2-e586-4812-b799-8993d42ee88d",
          "name": "createSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateSnapshot?DirectoryId=DirectoryId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a Simple AD or Microsoft AD directory in the AWS cloud."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2bb68a25-7ea2-4e20-a38b-7da76015f38c"
            }
          ]
        }
      ]
    },
    {
      "name": "Trust",
      "item": [
        {
          "id": "2c0e69e1-2125-4715-9a70-50bdc821b8be",
          "name": "createTrust",
          "request": {
            "url": "http://example.com/api/?Action=CreateTrust?ConditionalForwarderIpAddrs=ConditionalForwarderIpAddrs&DirectoryId=DirectoryId&RemoteDomainName=RemoteDomainName&TrustDirection=TrustDirection&TrustPassword=TrustPassword&TrustType=TrustType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "AWS Directory Service for Microsoft Active Directory allows you to configure trust relationships."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d43b6f1a-1f55-4f25-b831-650a5b89234b"
            }
          ]
        },
        {
          "id": "e3805beb-3000-4621-9cc3-18c13a3869d0",
          "name": "deleteTrust",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTrust?DeleteAssociatedConditionalForwarder=DeleteAssociatedConditionalForwarder&TrustId=TrustId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an existing trust relationship between your Microsoft AD in the AWS cloud and an external domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cffb3fa-8197-4bf8-b497-33054cb2a3e5"
            }
          ]
        },
        {
          "id": "e222cd49-4475-4431-b47c-aa73e4136944",
          "name": "describeTrusts",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTrusts?DirectoryId=DirectoryId&Limit=Limit&NextToken=NextToken&TrustIds=TrustIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about the trust relationships for this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e1bcc5b-9de5-4b78-a720-a953b6b52b01"
            }
          ]
        },
        {
          "id": "9ee51331-c51c-47d0-bde7-b78d088471a2",
          "name": "verifyTrust",
          "request": {
            "url": "http://example.com/api/?Action=VerifyTrust?TrustId=TrustId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "AWS Directory Service for Microsoft Active Directory allows you to configure and verify trust relationships."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c13fcf2-81f6-4857-bd04-413483a52c19"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "3a4befa3-d51f-4ee3-b6ed-f426507a812d",
          "name": "deleteSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSnapshot?SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a directory snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1228a80f-a734-4a12-ab59-2de9b25fda1b"
            }
          ]
        },
        {
          "id": "b8348a82-c537-4ff9-80d7-4c4a765a895b",
          "name": "describeSnapshots",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSnapshots?DirectoryId=DirectoryId&Limit=Limit&NextToken=NextToken&SnapshotIds=SnapshotIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about the directory snapshots that belong to this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "027e6c54-ce7c-46a8-bb04-52586a0e36cc"
            }
          ]
        },
        {
          "id": "2ccf64b8-6b6d-457e-bb9b-f865a8f39b73",
          "name": "getSnapshotLimits",
          "request": {
            "url": "http://example.com/api/?Action=GetSnapshotLimits?DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains the manual snapshot limits for a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c032191c-963f-410b-bb83-34642f379dfb"
            }
          ]
        },
        {
          "id": "1f541ee8-cc5f-42eb-afb8-31e429f62213",
          "name": "restoreFromSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=RestoreFromSnapshot?SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Restores a directory using an existing directory snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "671926ee-e367-4d97-9c83-d43f74bbe998"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "ff3e10a7-f33a-48a4-824c-1f233689c1ec",
          "name": "deregisterEventTopic",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterEventTopic?DirectoryId=DirectoryId&TopicName=TopicName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the specified directory as a publisher to the specified SNS topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "107bb89d-7a03-458c-bc54-636100b5bbe4"
            }
          ]
        },
        {
          "id": "cb59441f-9da0-45cd-be75-18e4f1646fb2",
          "name": "describeEventTopics",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEventTopics?DirectoryId=DirectoryId&TopicNames=TopicNames",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about which SNS topics receive status messages from the specified directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b0e6527-2a4a-4db7-91b4-95c3848833a9"
            }
          ]
        },
        {
          "id": "428fdf5c-faa1-4106-ad0b-7fa6f99af50b",
          "name": "registerEventTopic",
          "request": {
            "url": "http://example.com/api/?Action=RegisterEventTopic?DirectoryId=DirectoryId&TopicName=TopicName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates a directory with an SNS topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00dc7f03-d30f-433b-9611-f53fd93a6c0e"
            }
          ]
        }
      ]
    },
    {
      "name": "Radius",
      "item": [
        {
          "id": "edd7815b-dd95-4fa7-a0b3-331c7562a7f0",
          "name": "disableRadius",
          "request": {
            "url": "http://example.com/api/?Action=DisableRadius?DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables multi-factor authentication (MFA) with the Remote Authentication Dial In User Service (RADIUS) server for an AD Connector directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "790fe120-5364-4257-a0cb-f934c8df255e"
            }
          ]
        },
        {
          "id": "80379d9e-c924-439e-af2a-d71bb03d3d89",
          "name": "enableRadius",
          "request": {
            "url": "http://example.com/api/?Action=EnableRadius?DirectoryId=DirectoryId&RadiusSettings=RadiusSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables multi-factor authentication (MFA) with the Remote Authentication Dial In User Service (RADIUS) server for an AD Connector directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59acc8de-0d38-40a8-a212-db32b21e1510"
            }
          ]
        },
        {
          "id": "b7addce3-278b-494f-a47c-3161f48103b1",
          "name": "updateRadius",
          "request": {
            "url": "http://example.com/api/?Action=UpdateRadius?DirectoryId=DirectoryId&RadiusSettings=RadiusSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the Remote Authentication Dial In User Service (RADIUS) server information for an AD Connector directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba7653a8-1f39-434c-8cd0-734a59ad65a8"
            }
          ]
        }
      ]
    },
    {
      "name": "SSO",
      "item": [
        {
          "id": "55c4a987-4d85-443d-ae5f-2923bfdf3711",
          "name": "disableSso",
          "request": {
            "url": "http://example.com/api/?Action=DisableSso?DirectoryId=DirectoryId&Password=Password&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables single-sign on for a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "473abe8b-52a1-42ab-ba75-2915cf93a6d8"
            }
          ]
        },
        {
          "id": "27cdf447-12ab-4c5e-9a09-cb02c4c307eb",
          "name": "enableSso",
          "request": {
            "url": "http://example.com/api/?Action=EnableSso?DirectoryId=DirectoryId&Password=Password&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables single sign-on for a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f70f57b0-b524-4735-8b19-39662b02a35a"
            }
          ]
        }
      ]
    },
    {
      "name": "Schema Extension",
      "item": [
        {
          "id": "51242127-604a-4478-81fa-ca59627bde85",
          "name": "listSchemaExtensions",
          "request": {
            "url": "http://example.com/api/?Action=ListSchemaExtensions?DirectoryId=DirectoryId&Limit=Limit&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all schema extensions applied to a Microsoft AD Directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6badc4f-fe5d-4f07-af12-613127673189"
            }
          ]
        },
        {
          "id": "202c3ef2-85cd-41f9-8ff2-20743636f260",
          "name": "startSchemaExtension",
          "request": {
            "url": "http://example.com/api/?Action=StartSchemaExtension?CreateSnapshotBeforeSchemaExtension=CreateSnapshotBeforeSchemaExtension&Description=Description&DirectoryId=DirectoryId&LdifContent=LdifContent",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Applies a schema extension to a Microsoft AD directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ae9793b-81ee-43c8-a2c7-c515c0ebd263"
            }
          ]
        }
      ]
    }
  ]
}