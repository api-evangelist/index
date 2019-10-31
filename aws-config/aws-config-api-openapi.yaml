swagger: "2.0"
x-collection-name: AWS Config
x-complete: 1
info:
  title: AWS Config API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteConfigRule:
    get:
      summary: Delete Config Rule
      description: Deletes the specified AWS Config rule and all of its evaluation
        results.
      operationId: deleteConfigRule
      x-api-path-slug: actiondeleteconfigrule-get
      parameters:
      - in: query
        name: ConfigRuleName
        description: The name of the AWS Config rule that you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Rules
  /?Action=DeleteConfigurationRecorder:
    get:
      summary: Delete Configuration Recorder
      description: Deletes the configuration recorder.
      operationId: deleteConfigurationRecorder
      x-api-path-slug: actiondeleteconfigurationrecorder-get
      parameters:
      - in: query
        name: ConfigurationRecorderName
        description: The name of the configuration recorder to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Recorders
  /?Action=DeleteDeliveryChannel:
    get:
      summary: Delete Delivery Channel
      description: Deletes the delivery channel.
      operationId: deleteDeliveryChannel
      x-api-path-slug: actiondeletedeliverychannel-get
      parameters:
      - in: query
        name: DeliveryChannelName
        description: The name of the delivery channel to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Channels
  /?Action=DeleteEvaluationResults:
    get:
      summary: Delete Evaluation Results
      description: Deletes the evaluation results for the specified Config rule.
      operationId: deleteEvaluationResults
      x-api-path-slug: actiondeleteevaluationresults-get
      parameters:
      - in: query
        name: ConfigRuleName
        description: The name of the Config rule for which you want to delete the
          evaluation results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Evaluations
  /?Action=DeliverConfigSnapshot:
    get:
      summary: Deliver Config Snapshot
      description: Schedules delivery of a configuration snapshot to the Amazon S3
        bucket in the specified delivery channel.
      operationId: deliverConfigSnapshot
      x-api-path-slug: actiondeliverconfigsnapshot-get
      parameters:
      - in: query
        name: deliveryChannelName
        description: The name of the delivery channel through which the snapshot is
          delivered
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Snapshot
  /?Action=DescribeComplianceByConfigRule:
    get:
      summary: Describe Compliance By Config Rule
      description: Indicates whether the specified AWS Config rules are compliant.
      operationId: describeComplianceByConfigRule
      x-api-path-slug: actiondescribecompliancebyconfigrule-get
      parameters:
      - in: query
        name: ComplianceTypes
        description: Filters the results by compliance
        type: string
      - in: query
        name: ConfigRuleNames
        description: Specify one or more AWS Config rule names to filter the results
          by rule
        type: string
      - in: query
        name: NextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Compliance
  /?Action=DescribeComplianceByResource:
    get:
      summary: Describe Compliance By Resource
      description: Indicates whether the specified AWS resources are compliant.
      operationId: describeComplianceByResource
      x-api-path-slug: actiondescribecompliancebyresource-get
      parameters:
      - in: query
        name: ComplianceTypes
        description: Filters the results by compliance
        type: string
      - in: query
        name: Limit
        description: The maximum number of evaluation results returned on each page
        type: string
      - in: query
        name: NextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      - in: query
        name: ResourceId
        description: The ID of the AWS resource for which you want compliance information
        type: string
      - in: query
        name: ResourceType
        description: The types of AWS resources for which you want compliance information;for
          example, AWS::EC2::Instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Compliance
  /?Action=DescribeConfigRuleEvaluationStatus:
    get:
      summary: Describe Config Rule Evaluation Status
      description: Returns status information for each of your AWS managed Config
        rules.
      operationId: describeConfigRuleEvaluationStatus
      x-api-path-slug: actiondescribeconfigruleevaluationstatus-get
      parameters:
      - in: query
        name: ConfigRuleNames
        description: The name of the AWS managed Config rules for which you want status
          information
        type: string
      - in: query
        name: Limit
        description: The number of rule evaluation results that you want returned
        type: string
      - in: query
        name: NextToken
        description: The NextToken string returned on a previous page that you use
          to get the next page of results in a paginated response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Evaluations
  /?Action=DescribeConfigRules:
    get:
      summary: Describe Config Rules
      description: Returns details about your AWS Config rules.
      operationId: describeConfigRules
      x-api-path-slug: actiondescribeconfigrules-get
      parameters:
      - in: query
        name: ConfigRuleNames
        description: The names of the AWS Config rules for which you want details
        type: string
      - in: query
        name: NextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Rules
  /?Action=DescribeConfigurationRecorders:
    get:
      summary: Describe Configuration Recorders
      description: Returns the details for the specified configuration recorders.
      operationId: describeConfigurationRecorders
      x-api-path-slug: actiondescribeconfigurationrecorders-get
      parameters:
      - in: query
        name: ConfigurationRecorderNames
        description: A list of configuration recorder names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Rules
  /?Action=DescribeConfigurationRecorderStatus:
    get:
      summary: Describe Configuration Recorder Status
      description: Returns the current status of the specified configuration recorder.
      operationId: describeConfigurationRecorderStatus
      x-api-path-slug: actiondescribeconfigurationrecorderstatus-get
      parameters:
      - in: query
        name: ConfigurationRecorderNames
        description: The name(s) of the configuration recorder
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Rules
  /?Action=DescribeDeliveryChannels:
    get:
      summary: Describe Delivery Channels
      description: Returns details about the specified delivery channel.
      operationId: describeDeliveryChannels
      x-api-path-slug: actiondescribedeliverychannels-get
      parameters:
      - in: query
        name: DeliveryChannelNames
        description: A list of delivery channel names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Channels
  /?Action=DescribeDeliveryChannelStatus:
    get:
      summary: Describe Delivery Channel Status
      description: Returns the current status of the specified delivery channel.
      operationId: describeDeliveryChannelStatus
      x-api-path-slug: actiondescribedeliverychannelstatus-get
      parameters:
      - in: query
        name: DeliveryChannelNames
        description: A list of delivery channel names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Channels
  /?Action=GetComplianceDetailsByConfigRule:
    get:
      summary: Get Compliance Details By Config Rule
      description: Returns the evaluation results for the specified AWS Config rule.
      operationId: getComplianceDetailsByConfigRule
      x-api-path-slug: actiongetcompliancedetailsbyconfigrule-get
      parameters:
      - in: query
        name: ComplianceTypes
        description: Filters the results by compliance
        type: string
      - in: query
        name: ConfigRuleName
        description: The name of the AWS Config rule for which you want compliance
          information
        type: string
      - in: query
        name: Limit
        description: The maximum number of evaluation results returned on each page
        type: string
      - in: query
        name: NextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Compliance
  /?Action=GetComplianceDetailsByResource:
    get:
      summary: Get Compliance Details By Resource
      description: Returns the evaluation results for the specified AWS resource.
      operationId: getComplianceDetailsByResource
      x-api-path-slug: actiongetcompliancedetailsbyresource-get
      parameters:
      - in: query
        name: ComplianceTypes
        description: Filters the results by compliance
        type: string
      - in: query
        name: NextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      - in: query
        name: ResourceId
        description: The ID of the AWS resource for which you want compliance information
        type: string
      - in: query
        name: ResourceType
        description: The type of the AWS resource for which you want compliance information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Compliance
  /?Action=GetComplianceSummaryByConfigRule:
    get:
      summary: Get Compliance Summary By Config Rule
      description: "Returns the number of AWS Config rules that are compliant and
        noncompliant, up to a\n\t\t\tmaximum of 25 for each."
      operationId: getComplianceSummaryByConfigRule
      x-api-path-slug: actiongetcompliancesummarybyconfigrule-get
      parameters:
      - in: query
        name: ComplianceSummary
        description: The number of AWS Config rules that are compliant and the number
          that arenoncompliant, up to a maximum of 25 for each
        type: string
      responses:
        200:
          description: OK
      tags:
      - Compliance
  /?Action=GetComplianceSummaryByResourceType:
    get:
      summary: Get Compliance Summary By Resource Type
      description: Returns the number of resources that are compliant and the number
        that are noncompliant.
      operationId: getComplianceSummaryByResourceType
      x-api-path-slug: actiongetcompliancesummarybyresourcetype-get
      parameters:
      - in: query
        name: ResourceTypes
        description: Specify one or more resource types to get the number of resources
          that are compliant and the number that are noncompliant for each resource
          type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Compliance
  /?Action=GetResourceConfigHistory:
    get:
      summary: Get Resource Config History
      description: Returns a list of configuration items for the specified resource.
      operationId: getResourceConfigHistory
      x-api-path-slug: actiongetresourceconfighistory-get
      parameters:
      - in: query
        name: chronologicalOrder
        description: The chronological order for configuration items listed
        type: string
      - in: query
        name: earlierTime
        description: The time stamp that indicates an earlier time
        type: string
      - in: query
        name: laterTime
        description: The time stamp that indicates a later time
        type: string
      - in: query
        name: limit
        description: The maximum number of configuration items returned on each page
        type: string
      - in: query
        name: nextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      - in: query
        name: resourceId
        description: The ID of the resource (for example
        type: string
      - in: query
        name: resourceType
        description: The resource type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Configurations
  /?Action=ListDiscoveredResources:
    get:
      summary: List Discovered Resources
      description: Accepts a resource type and returns a list of resource identifiers
        for the resources of that type.
      operationId: listDiscoveredResources
      x-api-path-slug: actionlistdiscoveredresources-get
      parameters:
      - in: query
        name: includeDeletedResources
        description: Specifies whether AWS Config includes deleted resources in the
          results
        type: string
      - in: query
        name: limit
        description: The maximum number of resource identifiers returned on each page
        type: string
      - in: query
        name: nextToken
        description: The nextToken string returned on a previous page thatyou use
          to get the next page of results in a paginated response
        type: string
      - in: query
        name: resourceIds
        description: The IDs of only those resources that you want AWS Config to list
          in the response
        type: string
      - in: query
        name: resourceName
        description: The custom name of only those resources that you want AWS Config
          to list in the response
        type: string
      - in: query
        name: resourceType
        description: The type of resources that you want AWS Config to list in the
          response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Discovered Resources
  /?Action=PutConfigRule:
    get:
      summary: Put Config Rule
      description: "Adds or updates an AWS Config rule for evaluating whether your
        AWS resources comply\n\t\t\twith your desired configurations."
      operationId: putConfigRule
      x-api-path-slug: actionputconfigrule-get
      parameters:
      - in: query
        name: ConfigRule
        description: An AWS Config rule represents an AWS Lambda function that you
          create for a custom rule or a predefined function for an AWS managed rule
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Rules
  /?Action=PutConfigurationRecorder:
    get:
      summary: Put Configuration Recorder
      description: Creates a new configuration recorder to record the selected resource
        configurations.
      operationId: putConfigurationRecorder
      x-api-path-slug: actionputconfigurationrecorder-get
      parameters:
      - in: query
        name: ConfigurationRecorder
        description: The configuration recorder object that records each configuration
          change made to the resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Recorders
  /?Action=PutDeliveryChannel:
    get:
      summary: Put Delivery Channel
      description: Creates a delivery channel object to deliver configuration information
        to an Amazon S3 bucket and Amazon SNS topic.
      operationId: putDeliveryChannel
      x-api-path-slug: actionputdeliverychannel-get
      parameters:
      - in: query
        name: DeliveryChannel
        description: The configuration delivery channel object that delivers the configuration
          information to an Amazon S3 bucket, and to an Amazon SNS topic
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Channels
  /?Action=PutEvaluations:
    get:
      summary: Put Evaluations
      description: Used by an AWS Lambda function to deliver evaluation results to
        AWS Config.
      operationId: putEvaluations
      x-api-path-slug: actionputevaluations-get
      parameters:
      - in: query
        name: Evaluations
        description: The assessments that the AWS Lambda function performs
        type: string
      - in: query
        name: ResultToken
        description: An encrypted token that associates an evaluation with an AWS
          Config rule
        type: string
      responses:
        200:
          description: OK
      tags:
      - Evaluations
  /?Action=StartConfigRulesEvaluation:
    get:
      summary: Start Config Rules Evaluation
      description: Runs an on-demand evaluation for the specified Config rules against
        the last known configuration state of the resources.
      operationId: startConfigRulesEvaluation
      x-api-path-slug: actionstartconfigrulesevaluation-get
      parameters:
      - in: query
        name: ConfigRuleNames
        description: The list of names of Config rules that you want to run evaluations
          for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Evaluations
  /?Action=StartConfigurationRecorder:
    get:
      summary: Start Configuration Recorder
      description: Starts recording configurations of the AWS resources you have selected
        to record in your AWS account.
      operationId: startConfigurationRecorder
      x-api-path-slug: actionstartconfigurationrecorder-get
      parameters:
      - in: query
        name: ConfigurationRecorderName
        description: The name of the recorder object that records each configuration
          change made to the resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Recorders
  /?Action=StopConfigurationRecorder:
    get:
      summary: Stop Configuration Recorder
      description: Stops recording configurations of the AWS resources you have selected
        to record in your AWS account.
      operationId: stopConfigurationRecorder
      x-api-path-slug: actionstopconfigurationrecorder-get
      parameters:
      - in: query
        name: ConfigurationRecorderName
        description: The name of the recorder object that records each configuration
          change made to the resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Recorders