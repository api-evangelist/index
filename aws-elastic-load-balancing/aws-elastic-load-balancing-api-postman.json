{
  "info": {
    "name": "AWS Elastic Load Balancing API Set Subnets",
    "_postman_id": "d7781956-e0bc-4838-b1c5-5c660c359758",
    "description": "Enables the Availability Zone for the specified subnets for the specified load balancer.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "651b7d45-4a66-41bc-bde1-586ce3a54d87",
          "name": "addTags",
          "request": {
            "url": "http://example.com/api/?Action=AddTags?ResourceArns.member.N=ResourceArns.member.N&Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds the specified tags to the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd071049-1091-489d-9d6e-f7173ce017e8"
            }
          ]
        },
        {
          "id": "00ba13ad-7cd8-4c5c-a571-fa6d767c9af6",
          "name": "describeTags",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTags?ResourceArns.member.N=ResourceArns.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the tags for the specified resources."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47bc05f0-1ede-499c-a70b-3fca4152a531"
            }
          ]
        },
        {
          "id": "64f37d63-ec9b-490e-8547-5dfca62fcf1f",
          "name": "removeTags",
          "request": {
            "url": "http://example.com/api/?Action=RemoveTags?ResourceArns.member.N=ResourceArns.member.N&TagKeys.member.N=TagKeys.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the specified tags from the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3fe9419e-71fc-41cc-bee0-772099458094"
            }
          ]
        }
      ]
    },
    {
      "name": "Listeners",
      "item": [
        {
          "id": "f5ff5140-7732-44ae-ac70-ff1cbeca8575",
          "name": "createListener",
          "request": {
            "url": "http://example.com/api/?Action=CreateListener?Certificates.member.N=Certificates.member.N&DefaultActions.member.N=DefaultActions.member.N&LoadBalancerArn=LoadBalancerArn&Port=Port&Protocol=Protocol&SslPolicy=SslPolicy",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a listener for the specified Application Load Balancer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8ffcf9c-8108-407e-8b3d-60ca368c717a"
            }
          ]
        },
        {
          "id": "39c7330e-d6ef-44cd-bdad-f02502228ed5",
          "name": "deleteListener",
          "request": {
            "url": "http://example.com/api/?Action=DeleteListener?ListenerArn=ListenerArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified listener."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c943df12-b2f8-41be-b195-5cf3a4039874"
            }
          ]
        },
        {
          "id": "8f6edac6-c45e-4401-b827-5b4125a8899b",
          "name": "describeListeners",
          "request": {
            "url": "http://example.com/api/?Action=DescribeListeners?ListenerArns.member.N=ListenerArns.member.N&LoadBalancerArn=LoadBalancerArn&Marker=Marker&PageSize=PageSize",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified listeners or the listeners for the specified Application Load Balancer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c44d55a1-50f7-459c-9066-0c25175f5813"
            }
          ]
        },
        {
          "id": "90925826-1632-426a-8d1e-54ecd8a92351",
          "name": "modifyListener",
          "request": {
            "url": "http://example.com/api/?Action=ModifyListener?Certificates.member.N=Certificates.member.N&DefaultActions.member.N=DefaultActions.member.N&ListenerArn=ListenerArn&Port=Port&Protocol=Protocol&SslPolicy=SslPolicy",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the specified properties of the specified listener."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3fd70597-61d3-4c05-a761-8dde36b96745"
            }
          ]
        }
      ]
    },
    {
      "name": "Load Balancers",
      "item": [
        {
          "id": "82c40efe-9468-4806-a49a-6d5a52464675",
          "name": "createLoadBalancer",
          "request": {
            "url": "http://example.com/api/?Action=CreateLoadBalancer?Name=Name&Scheme=Scheme&SecurityGroups.member.N=SecurityGroups.member.N&Subnets.member.N=Subnets.member.N&Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an Application Load Balancer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e379fc7-b03e-4725-8845-ac3bdea4f453"
            }
          ]
        },
        {
          "id": "62b2b25f-c2ed-468b-8f60-f90c687f79a0",
          "name": "deleteLoadBalancer",
          "request": {
            "url": "http://example.com/api/?Action=DeleteLoadBalancer?LoadBalancerArn=LoadBalancerArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Application Load Balancer and its attached listeners."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c3756b8-cca4-4b0c-95b9-cf6f681fea38"
            }
          ]
        },
        {
          "id": "98622530-7839-4346-bd5e-a456187266fd",
          "name": "describeLoadBalancerAttributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLoadBalancerAttributes?LoadBalancerArn=LoadBalancerArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the attributes for the specified Application Load Balancer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41d763a0-5f4a-4e65-9c3e-b8d8a01b92fe"
            }
          ]
        },
        {
          "id": "aa766c8f-b165-4a45-82c6-5b66c4bd1d43",
          "name": "describeLoadBalancers",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLoadBalancers?LoadBalancerArns.member.N=LoadBalancerArns.member.N&Marker=Marker&Names.member.N=Names.member.N&PageSize=PageSize",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified Application Load Balancers or all of your Application Load Balancers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a40e7bf2-2cc6-4a69-ac89-4b53aae95bec"
            }
          ]
        },
        {
          "id": "323b3a96-1503-4acd-a84d-be8b1e967632",
          "name": "modifyLoadBalancerAttributes",
          "request": {
            "url": "http://example.com/api/?Action=ModifyLoadBalancerAttributes?Attributes.member.N=Attributes.member.N&LoadBalancerArn=LoadBalancerArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the specified attributes of the specified Application Load Balancer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4a4cb28-8c7a-4ca8-ab44-4fef2703ee90"
            }
          ]
        }
      ]
    },
    {
      "name": "Rules",
      "item": [
        {
          "id": "13cf4fe4-9c1e-4886-a910-d9fb80847cab",
          "name": "createRule",
          "request": {
            "url": "http://example.com/api/?Action=CreateRule?Actions.member.N=Actions.member.N&Conditions.member.N=Conditions.member.N&ListenerArn=ListenerArn&Priority=Priority",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a rule for the specified listener."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49a85da0-accb-44a9-90d1-2318fcc7e932"
            }
          ]
        },
        {
          "id": "4b35e7d8-fdac-41e5-9e22-359a3445b1c9",
          "name": "deleteRule",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRule?RuleArn=RuleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c492cd52-2368-476b-ad3f-26c6ec3b40e2"
            }
          ]
        },
        {
          "id": "12c7f522-7e61-44da-b28a-d0160f5a7096",
          "name": "describeRules",
          "request": {
            "url": "http://example.com/api/?Action=DescribeRules?ListenerArn=ListenerArn&RuleArns.member.N=RuleArns.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified rules or the rules for the specified listener."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72ea7de8-dedc-4fa5-b512-ef234e985cb5"
            }
          ]
        },
        {
          "id": "f4f4eb9f-61a6-468b-a9ca-3925ad535cd7",
          "name": "modifyRule",
          "request": {
            "url": "http://example.com/api/?Action=ModifyRule?Actions.member.N=Actions.member.N&Conditions.member.N=Conditions.member.N&RuleArn=RuleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the specified rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6abdb12b-bd98-479c-a116-80f2ff1f7362"
            }
          ]
        }
      ]
    },
    {
      "name": "Target Groups",
      "item": [
        {
          "id": "ab2582e7-ead0-4953-9dce-666800eb0e69",
          "name": "createTargetGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateTargetGroup?HealthCheckIntervalSeconds=HealthCheckIntervalSeconds&HealthCheckPath=HealthCheckPath&HealthCheckPort=HealthCheckPort&HealthCheckProtocol=HealthCheckProtocol&HealthCheckTimeoutSeconds=HealthCheckTimeoutSeconds&HealthyThresholdCount=HealthyThresholdCount&Matcher=Matcher&Name=Name&Port=Port&Protocol=Protocol&UnhealthyThresholdCount=UnhealthyThresholdCount&VpcId=VpcId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a target group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8c614fa-af54-4375-9b06-31ee6193a727"
            }
          ]
        },
        {
          "id": "5f3d19e7-2066-4dee-8e48-8807f65f4f7a",
          "name": "deleteTargetGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTargetGroup?TargetGroupArn=TargetGroupArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified target group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c28e723-ac5a-4165-9992-2450d196a7b7"
            }
          ]
        },
        {
          "id": "5032bd03-2958-4798-bf86-ed078d90511e",
          "name": "describeTargetGroupAttributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTargetGroupAttributes?TargetGroupArn=TargetGroupArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the attributes for the specified target group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b2dc5e6-d64a-4f31-ae19-e1d146fe01d5"
            }
          ]
        },
        {
          "id": "fa1eda87-12f6-449e-a6f1-d479fd583e73",
          "name": "describeTargetGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTargetGroups?LoadBalancerArn=LoadBalancerArn&Marker=Marker&Names.member.N=Names.member.N&PageSize=PageSize&TargetGroupArns.member.N=TargetGroupArns.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified target groups or all of your target groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e523c44-9291-45ff-af7f-9ef8e5bfd9d8"
            }
          ]
        },
        {
          "id": "10ae3857-29bd-44b0-8de4-a9d56491103b",
          "name": "modifyTargetGroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyTargetGroup?HealthCheckIntervalSeconds=HealthCheckIntervalSeconds&HealthCheckPath=HealthCheckPath&HealthCheckPort=HealthCheckPort&HealthCheckProtocol=HealthCheckProtocol&HealthCheckTimeoutSeconds=HealthCheckTimeoutSeconds&HealthyThresholdCount=HealthyThresholdCount&Matcher=Matcher&TargetGroupArn=TargetGroupArn&UnhealthyThresholdCount=UnhealthyThresholdCount",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the health checks used when evaluating the health state of the targets in the specified target group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25dab88c-8663-4a95-baf2-5e3d7efb5eb2"
            }
          ]
        },
        {
          "id": "a52d14bb-10c3-49af-a53c-0b0fb4860e2a",
          "name": "modifyTargetGroupAttributes",
          "request": {
            "url": "http://example.com/api/?Action=ModifyTargetGroupAttributes?Attributes.member.N=Attributes.member.N&TargetGroupArn=TargetGroupArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the specified attributes of the specified target group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a68fd36b-d5bd-4fa3-ae07-780a70905c92"
            }
          ]
        }
      ]
    },
    {
      "name": "Targets",
      "item": [
        {
          "id": "362e309b-ed6a-479e-b7df-51d0aee0cf46",
          "name": "deregisterTargets",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTargets?TargetGroupArn=TargetGroupArn&Targets.member.N=Targets.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregisters the specified targets from the specified target group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b119df05-329e-4a4e-9d98-742543665817"
            }
          ]
        },
        {
          "id": "dff6878d-9db6-4df5-ac59-c62ac6db0acb",
          "name": "registerTargets",
          "request": {
            "url": "http://example.com/api/?Action=RegisterTargets?TargetGroupArn=TargetGroupArn&Targets.member.N=Targets.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers the specified targets with the specified target group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c237bba-25db-4d43-9795-511d8fd50e5a"
            }
          ]
        }
      ]
    },
    {
      "name": "SSL Policies",
      "item": [
        {
          "id": "f7c10ff1-3220-475e-a4d5-4228eec304b3",
          "name": "describeSSLPolicies",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSSLPolicies?Marker=Marker&Names.member.N=Names.member.N&PageSize=PageSize",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified policies or all policies used for SSL negotiation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff0f0502-780d-4cb2-a33c-daccfe2d3216"
            }
          ]
        }
      ]
    },
    {
      "name": "Target Health",
      "item": [
        {
          "id": "07887588-c6ba-4b19-be6d-cc2f95551809",
          "name": "describeTargetHealth",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTargetHealth?TargetGroupArn=TargetGroupArn&Targets.member.N=Targets.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the health of the specified targets or all of your targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7eb57590-8706-42d0-a59e-2493fbec9d9c"
            }
          ]
        }
      ]
    },
    {
      "name": "Rule Priorities",
      "item": [
        {
          "id": "fffabe3a-51b0-42e8-a950-cdbeec5a8350",
          "name": "setRulePriorities",
          "request": {
            "url": "http://example.com/api/?Action=SetRulePriorities?RulePriorities.member.N=RulePriorities.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the priorities of the specified rules."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6b47cd2-0315-47af-a85b-ab865ed0b87c"
            }
          ]
        }
      ]
    },
    {
      "name": "Security Groups",
      "item": [
        {
          "id": "83f42e51-8cdc-4c0e-b054-c4e3eb111ce9",
          "name": "setSecurityGroups",
          "request": {
            "url": "http://example.com/api/?Action=SetSecurityGroups?LoadBalancerArn=LoadBalancerArn&SecurityGroups.member.N=SecurityGroups.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified security groups with the specified load balancer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b303ab4-c3a2-4be7-86ba-e166857bd9a6"
            }
          ]
        }
      ]
    },
    {
      "name": "Subnets",
      "item": [
        {
          "id": "cb19b7e1-68d8-44e3-9c79-9b37588d65f2",
          "name": "setSubnets",
          "request": {
            "url": "http://example.com/api/?Action=SetSubnets?LoadBalancerArn=LoadBalancerArn&Subnets.member.N=Subnets.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables the Availability Zone for the specified subnets for the specified load balancer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2cff0556-cb51-4a04-9054-c9a80002f8f9"
            }
          ]
        }
      ]
    }
  ]
}