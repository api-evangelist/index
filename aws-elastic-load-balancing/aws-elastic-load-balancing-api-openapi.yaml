swagger: "2.0"
x-collection-name: AWS Elastic Load Balancing
x-complete: 1
info:
  title: AWS Elastic Load Balancing API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddTags:
    get:
      summary: Add Tags
      description: Adds the specified tags to the specified resource.
      operationId: addTags
      x-api-path-slug: actionaddtags-get
      parameters:
      - in: query
        name: ResourceArns.member.N
        description: The Amazon Resource Name (ARN) of the resource
        type: string
      - in: query
        name: Tags.member.N
        description: The tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=CreateListener:
    get:
      summary: Create Listener
      description: Creates a listener for the specified Application Load Balancer.
      operationId: createListener
      x-api-path-slug: actioncreatelistener-get
      parameters:
      - in: query
        name: Certificates.member.N
        description: The SSL server certificate
        type: string
      - in: query
        name: DefaultActions.member.N
        description: The default action for the listener
        type: string
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      - in: query
        name: Port
        description: The port on which the load balancer is listening
        type: string
      - in: query
        name: Protocol
        description: The protocol for connections from clients to the load balancer
        type: string
      - in: query
        name: SslPolicy
        description: The security policy that defines which ciphers and protocols
          are supported
        type: string
      responses:
        200:
          description: OK
      tags:
      - Listeners
  /?Action=CreateLoadBalancer:
    get:
      summary: Create Load Balancer
      description: Creates an Application Load Balancer.
      operationId: createLoadBalancer
      x-api-path-slug: actioncreateloadbalancer-get
      parameters:
      - in: query
        name: Name
        description: The name of the load balancer
        type: string
      - in: query
        name: Scheme
        description: The nodes of an Internet-facing load balancer have public IP
          addresses
        type: string
      - in: query
        name: SecurityGroups.member.N
        description: The IDs of the security groups to assign to the load balancer
        type: string
      - in: query
        name: Subnets.member.N
        description: The IDs of the subnets to attach to the load balancer
        type: string
      - in: query
        name: Tags.member.N
        description: One or more tags to assign to the load balancer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=CreateRule:
    get:
      summary: Create Rule
      description: Creates a rule for the specified listener.
      operationId: createRule
      x-api-path-slug: actioncreaterule-get
      parameters:
      - in: query
        name: Actions.member.N
        description: An action
        type: string
      - in: query
        name: Conditions.member.N
        description: A condition
        type: string
      - in: query
        name: ListenerArn
        description: The Amazon Resource Name (ARN) of the listener
        type: string
      - in: query
        name: Priority
        description: The priority for the rule
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rules
  /?Action=CreateTargetGroup:
    get:
      summary: Create Target Group
      description: Creates a target group.
      operationId: createTargetGroup
      x-api-path-slug: actioncreatetargetgroup-get
      parameters:
      - in: query
        name: HealthCheckIntervalSeconds
        description: The approximate amount of time, in seconds, between health checks
          of an individual target
        type: string
      - in: query
        name: HealthCheckPath
        description: The ping path that is the destination on the targets for health
          checks
        type: string
      - in: query
        name: HealthCheckPort
        description: The port the load balancer uses when performing health checks
          on targets
        type: string
      - in: query
        name: HealthCheckProtocol
        description: The protocol the load balancer uses when performing health checks
          on targets
        type: string
      - in: query
        name: HealthCheckTimeoutSeconds
        description: The amount of time, in seconds, during which no response from
          a target means a failed health check
        type: string
      - in: query
        name: HealthyThresholdCount
        description: The number of consecutive health checks successes required before
          considering an unhealthy target healthy
        type: string
      - in: query
        name: Matcher
        description: The HTTP codes to use when checking for a successful response
          from a target
        type: string
      - in: query
        name: Name
        description: The name of the target group
        type: string
      - in: query
        name: Port
        description: The port on which the targets receive traffic
        type: string
      - in: query
        name: Protocol
        description: The protocol to use for routing traffic to the targets
        type: string
      - in: query
        name: UnhealthyThresholdCount
        description: The number of consecutive health check failures required before
          considering a target unhealthy
        type: string
      - in: query
        name: VpcId
        description: The identifier of the virtual private cloud (VPC)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Target Groups
  /?Action=DeleteListener:
    get:
      summary: Delete Listener
      description: Deletes the specified listener.
      operationId: deleteListener
      x-api-path-slug: actiondeletelistener-get
      parameters:
      - in: query
        name: ListenerArn
        description: The Amazon Resource Name (ARN) of the listener
        type: string
      responses:
        200:
          description: OK
      tags:
      - Listeners
  /?Action=DeleteLoadBalancer:
    get:
      summary: Delete Load Balancer
      description: Deletes the specified Application Load Balancer and its attached
        listeners.
      operationId: deleteLoadBalancer
      x-api-path-slug: actiondeleteloadbalancer-get
      parameters:
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=DeleteRule:
    get:
      summary: Delete Rule
      description: Deletes the specified rule.
      operationId: deleteRule
      x-api-path-slug: actiondeleterule-get
      parameters:
      - in: query
        name: RuleArn
        description: The Amazon Resource Name (ARN) of the rule
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rules
  /?Action=DeleteTargetGroup:
    get:
      summary: Delete Target Group
      description: Deletes the specified target group.
      operationId: deleteTargetGroup
      x-api-path-slug: actiondeletetargetgroup-get
      parameters:
      - in: query
        name: TargetGroupArn
        description: The Amazon Resource Name (ARN) of the target group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Target Groups
  /?Action=DeregisterTargets:
    get:
      summary: Deregister Targets
      description: Deregisters the specified targets from the specified target group.
      operationId: deregisterTargets
      x-api-path-slug: actionderegistertargets-get
      parameters:
      - in: query
        name: TargetGroupArn
        description: The Amazon Resource Name (ARN) of the target group
        type: string
      - in: query
        name: Targets.member.N
        description: The targets
        type: string
      responses:
        200:
          description: OK
      tags:
      - Targets
  /?Action=DescribeListeners:
    get:
      summary: Describe Listeners
      description: Describes the specified listeners or the listeners for the specified
        Application Load Balancer.
      operationId: describeListeners
      x-api-path-slug: actiondescribelisteners-get
      parameters:
      - in: query
        name: ListenerArns.member.N
        description: The Amazon Resource Names (ARN) of the listeners
        type: string
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      - in: query
        name: Marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: PageSize
        description: The maximum number of results to return with this call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Listeners
  /?Action=DescribeLoadBalancerAttributes:
    get:
      summary: Describe Load Balancer Attributes
      description: Describes the attributes for the specified Application Load Balancer.
      operationId: describeLoadBalancerAttributes
      x-api-path-slug: actiondescribeloadbalancerattributes-get
      parameters:
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=DescribeLoadBalancers:
    get:
      summary: Describe Load Balancers
      description: Describes the specified Application Load Balancers or all of your
        Application Load Balancers.
      operationId: describeLoadBalancers
      x-api-path-slug: actiondescribeloadbalancers-get
      parameters:
      - in: query
        name: LoadBalancerArns.member.N
        description: The Amazon Resource Names (ARN) of the load balancers
        type: string
      - in: query
        name: Marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: Names.member.N
        description: The names of the load balancers
        type: string
      - in: query
        name: PageSize
        description: The maximum number of results to return with this call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=DescribeRules:
    get:
      summary: Describe Rules
      description: Describes the specified rules or the rules for the specified listener.
      operationId: describeRules
      x-api-path-slug: actiondescriberules-get
      parameters:
      - in: query
        name: ListenerArn
        description: The Amazon Resource Name (ARN) of the listener
        type: string
      - in: query
        name: RuleArns.member.N
        description: The Amazon Resource Names (ARN) of the rules
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rules
  /?Action=DescribeSSLPolicies:
    get:
      summary: Describe S S L Policies
      description: Describes the specified policies or all policies used for SSL negotiation.
      operationId: describeSSLPolicies
      x-api-path-slug: actiondescribesslpolicies-get
      parameters:
      - in: query
        name: Marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: Names.member.N
        description: The names of the policies
        type: string
      - in: query
        name: PageSize
        description: The maximum number of results to return with this call
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSL Policies
  /?Action=DescribeTags:
    get:
      summary: Describe Tags
      description: Describes the tags for the specified resources.
      operationId: describeTags
      x-api-path-slug: actiondescribetags-get
      parameters:
      - in: query
        name: ResourceArns.member.N
        description: The Amazon Resource Names (ARN) of the resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=DescribeTargetGroupAttributes:
    get:
      summary: Describe Target Group Attributes
      description: Describes the attributes for the specified target group.
      operationId: describeTargetGroupAttributes
      x-api-path-slug: actiondescribetargetgroupattributes-get
      parameters:
      - in: query
        name: TargetGroupArn
        description: The Amazon Resource Name (ARN) of the target group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Target Groups
  /?Action=DescribeTargetGroups:
    get:
      summary: Describe Target Groups
      description: Describes the specified target groups or all of your target groups.
      operationId: describeTargetGroups
      x-api-path-slug: actiondescribetargetgroups-get
      parameters:
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      - in: query
        name: Marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: Names.member.N
        description: The names of the target groups
        type: string
      - in: query
        name: PageSize
        description: The maximum number of results to return with this call
        type: string
      - in: query
        name: TargetGroupArns.member.N
        description: The Amazon Resource Names (ARN) of the target groups
        type: string
      responses:
        200:
          description: OK
      tags:
      - Target Groups
  /?Action=DescribeTargetHealth:
    get:
      summary: Describe Target Health
      description: Describes the health of the specified targets or all of your targets.
      operationId: describeTargetHealth
      x-api-path-slug: actiondescribetargethealth-get
      parameters:
      - in: query
        name: TargetGroupArn
        description: The Amazon Resource Name (ARN) of the target group
        type: string
      - in: query
        name: Targets.member.N
        description: The targets
        type: string
      responses:
        200:
          description: OK
      tags:
      - Target Health
  /?Action=ModifyListener:
    get:
      summary: Modify Listener
      description: Modifies the specified properties of the specified listener.
      operationId: modifyListener
      x-api-path-slug: actionmodifylistener-get
      parameters:
      - in: query
        name: Certificates.member.N
        description: The SSL server certificate
        type: string
      - in: query
        name: DefaultActions.member.N
        description: The default actions
        type: string
      - in: query
        name: ListenerArn
        description: The Amazon Resource Name (ARN) of the listener
        type: string
      - in: query
        name: Port
        description: The port for connections from clients to the load balancer
        type: string
      - in: query
        name: Protocol
        description: The protocol for connections from clients to the load balancer
        type: string
      - in: query
        name: SslPolicy
        description: The security policy that defines which ciphers and protocols
          are supported
        type: string
      responses:
        200:
          description: OK
      tags:
      - Listeners
  /?Action=ModifyLoadBalancerAttributes:
    get:
      summary: Modify Load Balancer Attributes
      description: Modifies the specified attributes of the specified Application
        Load Balancer.
      operationId: modifyLoadBalancerAttributes
      x-api-path-slug: actionmodifyloadbalancerattributes-get
      parameters:
      - in: query
        name: Attributes.member.N
        description: The load balancer attributes
        type: string
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=ModifyRule:
    get:
      summary: Modify Rule
      description: Modifies the specified rule.
      operationId: modifyRule
      x-api-path-slug: actionmodifyrule-get
      parameters:
      - in: query
        name: Actions.member.N
        description: The actions
        type: string
      - in: query
        name: Conditions.member.N
        description: The conditions
        type: string
      - in: query
        name: RuleArn
        description: The Amazon Resource Name (ARN) of the rule
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rules
  /?Action=ModifyTargetGroup:
    get:
      summary: Modify Target Group
      description: Modifies the health checks used when evaluating the health state
        of the targets in the specified target group.
      operationId: modifyTargetGroup
      x-api-path-slug: actionmodifytargetgroup-get
      parameters:
      - in: query
        name: HealthCheckIntervalSeconds
        description: The approximate amount of time, in seconds, between health checks
          of an individual target
        type: string
      - in: query
        name: HealthCheckPath
        description: The ping path that is the destination for the health check request
        type: string
      - in: query
        name: HealthCheckPort
        description: The port to use to connect with the target
        type: string
      - in: query
        name: HealthCheckProtocol
        description: The protocol to use to connect with the target
        type: string
      - in: query
        name: HealthCheckTimeoutSeconds
        description: The amount of time, in seconds, during which no response means
          a failed health check
        type: string
      - in: query
        name: HealthyThresholdCount
        description: The number of consecutive health checks successes required before
          considering an unhealthy target healthy
        type: string
      - in: query
        name: Matcher
        description: The HTTP codes to use when checking for a successful response
          from a target
        type: string
      - in: query
        name: TargetGroupArn
        description: The Amazon Resource Name (ARN) of the target group
        type: string
      - in: query
        name: UnhealthyThresholdCount
        description: The number of consecutive health check failures required before
          considering the target unhealthy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Target Groups
  /?Action=ModifyTargetGroupAttributes:
    get:
      summary: Modify Target Group Attributes
      description: Modifies the specified attributes of the specified target group.
      operationId: modifyTargetGroupAttributes
      x-api-path-slug: actionmodifytargetgroupattributes-get
      parameters:
      - in: query
        name: Attributes.member.N
        description: The attributes
        type: string
      - in: query
        name: TargetGroupArn
        description: The Amazon Resource Name (ARN) of the target group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Target Groups
  /?Action=RegisterTargets:
    get:
      summary: Register Targets
      description: Registers the specified targets with the specified target group.
      operationId: registerTargets
      x-api-path-slug: actionregistertargets-get
      parameters:
      - in: query
        name: TargetGroupArn
        description: The Amazon Resource Name (ARN) of the target group
        type: string
      - in: query
        name: Targets.member.N
        description: The targets
        type: string
      responses:
        200:
          description: OK
      tags:
      - Targets
  /?Action=RemoveTags:
    get:
      summary: Remove Tags
      description: Removes the specified tags from the specified resource.
      operationId: removeTags
      x-api-path-slug: actionremovetags-get
      parameters:
      - in: query
        name: ResourceArns.member.N
        description: The Amazon Resource Name (ARN) of the resource
        type: string
      - in: query
        name: TagKeys.member.N
        description: The tag keys for the tags to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=SetRulePriorities:
    get:
      summary: Set Rule Priorities
      description: Sets the priorities of the specified rules.
      operationId: setRulePriorities
      x-api-path-slug: actionsetrulepriorities-get
      parameters:
      - in: query
        name: RulePriorities.member.N
        description: The rule priorities
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rule Priorities
  /?Action=SetSecurityGroups:
    get:
      summary: Set Security Groups
      description: Associates the specified security groups with the specified load
        balancer.
      operationId: setSecurityGroups
      x-api-path-slug: actionsetsecuritygroups-get
      parameters:
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      - in: query
        name: SecurityGroups.member.N
        description: The IDs of the security groups
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Groups
  /?Action=SetSubnets:
    get:
      summary: Set Subnets
      description: Enables the Availability Zone for the specified subnets for the
        specified load balancer.
      operationId: setSubnets
      x-api-path-slug: actionsetsubnets-get
      parameters:
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      - in: query
        name: Subnets.member.N
        description: The IDs of the subnets
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnets