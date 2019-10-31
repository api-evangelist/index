swagger: "2.0"
x-collection-name: AWS Shield
x-complete: 1
info:
  title: AWS Shield API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateProtection:
    get:
      summary: Create Protection
      description: Enables AWS Shield Advanced for a specific AWS resource.
      operationId: createProtection
      x-api-path-slug: actioncreateprotection-get
      parameters:
      - in: query
        name: Name
        description: Friendly name for the Protection you are creating
        type: string
      - in: query
        name: ResourceArn
        description: The ARN (Amazon Resource Name) of the resource to be protected
        type: string
      responses:
        200:
          description: OK
      tags:
      - Protection
  /?Action=CreateSubscription:
    get:
      summary: Create Subscription
      description: Activates AWS Shield Advanced for an account.
      operationId: createSubscription
      x-api-path-slug: actioncreatesubscription-get
      responses:
        200:
          description: OK
      tags:
      - Protection
  /?Action=DeleteProtection:
    get:
      summary: Delete Protection
      description: Deletes an AWS Shield Advanced.
      operationId: deleteProtection
      x-api-path-slug: actiondeleteprotection-get
      parameters:
      - in: query
        name: ProtectionId
        description: The unique identifier (ID) for the Protection object to be         deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Protection
  /?Action=DeleteSubscription:
    get:
      summary: Delete Subscription
      description: Removes AWS Shield Advanced from an account.
      operationId: deleteSubscription
      x-api-path-slug: actiondeletesubscription-get
      responses:
        200:
          description: OK
      tags:
      - Protection
  /?Action=DescribeAttack:
    get:
      summary: Describe Attack
      description: Describes the details of a DDoS attack.
      operationId: describeAttack
      x-api-path-slug: actiondescribeattack-get
      parameters:
      - in: query
        name: AttackId
        description: The unique identifier (ID) for the attack that to be described
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attacks
  /?Action=DescribeProtection:
    get:
      summary: Describe Protection
      description: Lists the details of a.
      operationId: describeProtection
      x-api-path-slug: actiondescribeprotection-get
      parameters:
      - in: query
        name: ProtectionId
        description: The unique identifier (ID) for the Protection object that is         described
        type: string
      responses:
        200:
          description: OK
      tags:
      - Protection
  /?Action=DescribeSubscription:
    get:
      summary: Describe Subscription
      description: Provides details about the AWS Shield Advanced subscription for
        an account.
      operationId: describeSubscription
      x-api-path-slug: actiondescribesubscription-get
      parameters:
      - in: query
        name: Subscription
        description: The AWS Shield Advanced subscription details for an account
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=ListAttacks:
    get:
      summary: List Attacks
      description: |-
        Returns all ongoing DDoS attacks or all DDoS attacks during a specified time
                 period.
      operationId: listAttacks
      x-api-path-slug: actionlistattacks-get
      parameters:
      - in: query
        name: EndTime
        description: The end of the time period for the attacks
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of AttackSummary objects to be returned
        type: string
      - in: query
        name: NextToken
        description: The ListAttacksRequest
        type: string
      - in: query
        name: ResourceArns
        description: The ARN (Amazon Resource Name) of the resource that was attacked
        type: string
      - in: query
        name: StartTime
        description: The time period for the attacks
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attacks
  /?Action=ListProtections:
    get:
      summary: List Protections
      description: Lists all protections.
      operationId: listProtections
      x-api-path-slug: actionlistprotections-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of Protection objects to be returned
        type: string
      - in: query
        name: NextToken
        description: The ListProtectionsRequest
        type: string
      responses:
        200:
          description: OK
      tags:
      - Protection