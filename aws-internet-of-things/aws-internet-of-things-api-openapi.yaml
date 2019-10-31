swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 1
info:
  title: AWS Internet of Things API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AcceptCertificateTransfer:
    get:
      summary: Accept Certificate Transfer
      description: Accepts a pending certificate transfer.
      operationId: acceptCertificateTransfer
      x-api-path-slug: actionacceptcertificatetransfer-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate
        type: string
      - in: query
        name: setAsActive
        description: Specifies whether the certificate is active
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificate Transfers
  /?Action=AttachPrincipalPolicy:
    get:
      summary: Attach Principal Policy
      description: Attaches the specified policy to the specified principal (certificate
        or other credential).
      operationId: attachPrincipalPolicy
      x-api-path-slug: actionattachprincipalpolicy-get
      parameters:
      - in: query
        name: policyName
        description: The policy name
        type: string
      - in: query
        name: principal
        description: The principal, which can be a certificate ARN (as returned from
          the CreateCertificate operation) or an Amazon Cognito ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Principal Policies
  /?Action=AttachThingPrincipal:
    get:
      summary: Attach Thing Principal
      description: Attaches the specified principal to the specified thing.
      operationId: attachThingPrincipal
      x-api-path-slug: actionattachthingprincipal-get
      parameters:
      - in: query
        name: principal
        description: The principal, such as a certificate or other credential
        type: string
      - in: query
        name: thingName
        description: The name of the thing
        type: string
      responses:
        200:
          description: OK
      tags:
      - Thing Principals
  /?Action=CancelCertificateTransfer:
    get:
      summary: Cancel Certificate Transfer
      description: Cancels a pending transfer for the specified certificate.
      operationId: cancelCertificateTransfer
      x-api-path-slug: actioncancelcertificatetransfer-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificate Transfers
  /?Action=CreateCertificateFromCsr:
    get:
      summary: Create Certificate From Csr
      description: Creates an X.
      operationId: createCertificateFromCsr
      x-api-path-slug: actioncreatecertificatefromcsr-get
      parameters:
      - in: query
        name: certificateSigningRequest
        description: The certificate signing request (CSR)
        type: string
      - in: query
        name: setAsActive
        description: Specifies whether the certificate is active
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=CreateKeysAndCertificate:
    get:
      summary: Create Keys And Certificate
      description: Creates a 2048-bit RSA key pair and issues an X.
      operationId: createKeysAndCertificate
      x-api-path-slug: actioncreatekeysandcertificate-get
      parameters:
      - in: query
        name: setAsActive
        description: Specifies whether the certificate is active
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys And Certificates
  /?Action=CreatePolicy:
    get:
      summary: Create Policy
      description: Creates an AWS IoT policy.
      operationId: createPolicy
      x-api-path-slug: actioncreatepolicy-get
      parameters:
      - in: query
        name: policyDocument
        description: The JSON document that describes the policy
        type: string
      - in: query
        name: policyName
        description: The policy name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=CreatePolicyVersion:
    get:
      summary: Create Policy Version
      description: Creates a new version of the specified AWS IoT policy.
      operationId: createPolicyVersion
      x-api-path-slug: actioncreatepolicyversion-get
      parameters:
      - in: query
        name: policyDocument
        description: The JSON document that describes the policy
        type: string
      - in: query
        name: policyName
        description: The policy name
        type: string
      - in: query
        name: setAsDefault
        description: Specifies whether the policy version is set as the default
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=CreateThing:
    get:
      summary: Create Thing
      description: Creates a thing record in the thing registry.
      operationId: createThing
      x-api-path-slug: actioncreatething-get
      parameters:
      - in: query
        name: attributePayload
        description: The attribute payload, which consists of up to three name/value
          pairs in a JSON document
        type: string
      - in: query
        name: thingName
        description: The name of the thing to create
        type: string
      - in: query
        name: thingTypeName
        description: The name of the thing type associated with the new thing
        type: string
      responses:
        200:
          description: OK
      tags:
      - Things
  /?Action=CreateThingType:
    get:
      summary: Create Thing Type
      description: Creates a new thing type.
      operationId: createThingType
      x-api-path-slug: actioncreatethingtype-get
      parameters:
      - in: query
        name: thingTypeName
        description: The name of the thing type
        type: string
      - in: query
        name: thingTypeProperties
        description: The ThingTypeProperties for the thing type to create
        type: string
      responses:
        200:
          description: OK
      tags:
      - Thing Types
  /?Action=CreateTopicRule:
    get:
      summary: Create Topic Rule
      description: Creates a rule.
      operationId: createTopicRule
      x-api-path-slug: actioncreatetopicrule-get
      parameters:
      - in: query
        name: ruleName
        description: The name of the rule
        type: string
      - in: query
        name: topicRulePayload
        description: The rule payload
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topic Rules
  /?Action=DeleteCACertificate:
    get:
      summary: Delete C A Certificate
      description: Deletes a registered CA certificate.
      operationId: deleteCACertificate
      x-api-path-slug: actiondeletecacertificate-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - CA Certificates
  /?Action=DeleteCertificate:
    get:
      summary: Delete Certificate
      description: Deletes the specified certificate.
      operationId: deleteCertificate
      x-api-path-slug: actiondeletecertificate-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=DeletePolicy:
    get:
      summary: Delete Policy
      description: Deletes the specified policy.
      operationId: deletePolicy
      x-api-path-slug: actiondeletepolicy-get
      parameters:
      - in: query
        name: policyName
        description: The name of the policy to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=DeletePolicyVersion:
    get:
      summary: Delete Policy Version
      description: Deletes the specified version of the specified policy.
      operationId: deletePolicyVersion
      x-api-path-slug: actiondeletepolicyversion-get
      parameters:
      - in: query
        name: policyName
        description: The name of the policy
        type: string
      - in: query
        name: policyVersionId
        description: The policy version ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=DeleteRegistrationCode:
    get:
      summary: Delete Registration Code
      description: Deletes a CA certificate registration code.
      operationId: deleteRegistrationCode
      x-api-path-slug: actiondeleteregistrationcode-get
      responses:
        200:
          description: OK
      tags:
      - Registration Codes
  /?Action=DeleteThing:
    get:
      summary: Delete Thing
      description: Deletes the specified thing.
      operationId: deleteThing
      x-api-path-slug: actiondeletething-get
      parameters:
      - in: query
        name: expectedVersion
        description: The expected version of the thing record in the registry
        type: string
      - in: query
        name: thingName
        description: The name of the thing to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Things
  /?Action=DeleteThingType:
    get:
      summary: Delete Thing Type
      description: Deletes the specified thing type.
      operationId: deleteThingType
      x-api-path-slug: actiondeletethingtype-get
      parameters:
      - in: query
        name: thingTypeName
        description: The name of the thing type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Thing Types
  /?Action=DeleteTopicRule:
    get:
      summary: Delete Topic Rule
      description: Deletes the specified rule.
      operationId: deleteTopicRule
      x-api-path-slug: actiondeletetopicrule-get
      parameters:
      - in: query
        name: ruleName
        description: The name of the rule
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topic Rules
  /?Action=DeprecateThingType:
    get:
      summary: Deprecate Thing Type
      description: Deprecates a thing type.
      operationId: deprecateThingType
      x-api-path-slug: actiondeprecatethingtype-get
      parameters:
      - in: query
        name: thingTypeName
        description: The name of the thing type to deprecate
        type: string
      - in: query
        name: undoDeprecate
        description: Whether to undeprecate a deprecated thing type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Thing Types
  /?Action=DescribeCACertificate:
    get:
      summary: Describe C A Certificate
      description: Describes a registered CA certificate.
      operationId: describeCACertificate
      x-api-path-slug: actiondescribecacertificate-get
      parameters:
      - in: query
        name: certificateId
        description: The CA certificate identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - CA Certificates
  /?Action=DescribeCertificate:
    get:
      summary: Describe Certificate
      description: Gets information about the specified certificate.
      operationId: describeCertificate
      x-api-path-slug: actiondescribecertificate-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=DescribeEndpoint:
    get:
      summary: Describe Endpoint
      description: Returns a unique endpoint specific to the AWS account making the
        call.
      operationId: describeEndpoint
      x-api-path-slug: actiondescribeendpoint-get
      parameters:
      - in: query
        name: endpointAddress
        description: The endpoint
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /?Action=DescribeThing:
    get:
      summary: Describe Thing
      description: Gets information about the specified thing.
      operationId: describeThing
      x-api-path-slug: actiondescribething-get
      parameters:
      - in: query
        name: thingName
        description: The name of the thing
        type: string
      responses:
        200:
          description: OK
      tags:
      - Things
  /?Action=DescribeThingType:
    get:
      summary: Describe Thing Type
      description: Gets information about the specified thing type.
      operationId: describeThingType
      x-api-path-slug: actiondescribethingtype-get
      parameters:
      - in: query
        name: thingTypeName
        description: The name of the thing type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Thing Types
  /?Action=DetachPrincipalPolicy:
    get:
      summary: Detach Principal Policy
      description: Removes the specified policy from the specified certificate.
      operationId: detachPrincipalPolicy
      x-api-path-slug: actiondetachprincipalpolicy-get
      parameters:
      - in: query
        name: policyName
        description: The name of the policy to detach
        type: string
      - in: query
        name: principal
        description: The principal
        type: string
      responses:
        200:
          description: OK
      tags:
      - Principal Policies
  /?Action=DetachThingPrincipal:
    get:
      summary: Detach Thing Principal
      description: Detaches the specified principal from the specified thing.
      operationId: detachThingPrincipal
      x-api-path-slug: actiondetachthingprincipal-get
      parameters:
      - in: query
        name: principal
        description: If the principal is a certificate, this value must be ARN of
          the certificate
        type: string
      - in: query
        name: thingName
        description: The name of the thing
        type: string
      responses:
        200:
          description: OK
      tags:
      - Thing Principals
  /?Action=DisableTopicRule:
    get:
      summary: Disable Topic Rule
      description: Disables the specified rule.
      operationId: disableTopicRule
      x-api-path-slug: actiondisabletopicrule-get
      parameters:
      - in: query
        name: ruleName
        description: The name of the rule to disable
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topic Rules
  /?Action=EnableTopicRule:
    get:
      summary: Enable Topic Rule
      description: Enables the specified rule.
      operationId: enableTopicRule
      x-api-path-slug: actionenabletopicrule-get
      parameters:
      - in: query
        name: ruleName
        description: The name of the topic rule to enable
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topic Rules
  /?Action=GetLoggingOptions:
    get:
      summary: Get Logging Options
      description: Gets the logging options.
      operationId: getLoggingOptions
      x-api-path-slug: actiongetloggingoptions-get
      parameters:
      - in: query
        name: logLevel
        description: The logging level
        type: string
      - in: query
        name: roleArn
        description: The ARN of the IAM role that grants access
        type: string
      responses:
        200:
          description: OK
      tags:
      - Logging Options
  /?Action=GetPolicy:
    get:
      summary: Get Policy
      description: Gets information about the specified policy with the policy document
        of the default version.
      operationId: getPolicy
      x-api-path-slug: actiongetpolicy-get
      parameters:
      - in: query
        name: policyName
        description: The name of the policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=GetPolicyVersion:
    get:
      summary: Get Policy Version
      description: Gets information about the specified policy version.
      operationId: getPolicyVersion
      x-api-path-slug: actiongetpolicyversion-get
      parameters:
      - in: query
        name: policyName
        description: The name of the policy
        type: string
      - in: query
        name: policyVersionId
        description: The policy version ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=GetRegistrationCode:
    get:
      summary: Get Registration Code
      description: Gets a registration code used to register a CA certificate with
        AWS IoT.
      operationId: getRegistrationCode
      x-api-path-slug: actiongetregistrationcode-get
      parameters:
      - in: query
        name: registrationCode
        description: The CA certificate registration code
        type: string
      responses:
        200:
          description: OK
      tags:
      - Registration Codes
  /?Action=GetTopicRule:
    get:
      summary: Get Topic Rule
      description: Gets information about the specified rule.
      operationId: getTopicRule
      x-api-path-slug: actiongettopicrule-get
      parameters:
      - in: query
        name: ruleName
        description: The name of the rule
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topic Rules
  /?Action=ListCACertificates:
    get:
      summary: List C A Certificates
      description: Lists the CA certificates registered for your AWS account.
      operationId: listCACertificates
      x-api-path-slug: actionlistcacertificates-get
      parameters:
      - in: query
        name: ascendingOrder
        description: Determines the order of the results
        type: string
      - in: query
        name: marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: pageSize
        description: The result page size
        type: string
      responses:
        200:
          description: OK
      tags:
      - CA Certificates
  /?Action=ListCertificates:
    get:
      summary: List Certificates
      description: Lists the certificates registered in your AWS account.
      operationId: listCertificates
      x-api-path-slug: actionlistcertificates-get
      parameters:
      - in: query
        name: ascendingOrder
        description: Specifies the order for results
        type: string
      - in: query
        name: marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: pageSize
        description: The result page size
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=ListCertificatesByCA:
    get:
      summary: List Certificates By C A
      description: List the device certificates signed by the specified CA certificate.
      operationId: listCertificatesByCA
      x-api-path-slug: actionlistcertificatesbyca-get
      parameters:
      - in: query
        name: ascendingOrder
        description: Specifies the order for results
        type: string
      - in: query
        name: caCertificateId
        description: The ID of the CA certificate
        type: string
      - in: query
        name: marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: pageSize
        description: The result page size
        type: string
      responses:
        200:
          description: OK
      tags:
      - CA Certificates
  /?Action=ListOutgoingCertificates:
    get:
      summary: List Outgoing Certificates
      description: Lists certificates that are being transfered but not yet accepted.
      operationId: listOutgoingCertificates
      x-api-path-slug: actionlistoutgoingcertificates-get
      parameters:
      - in: query
        name: ascendingOrder
        description: Specifies the order for results
        type: string
      - in: query
        name: marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: pageSize
        description: The result page size
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=ListPolicies:
    get:
      summary: List Policies
      description: Lists your policies.
      operationId: listPolicies
      x-api-path-slug: actionlistpolicies-get
      parameters:
      - in: query
        name: ascendingOrder
        description: Specifies the order for results
        type: string
      - in: query
        name: marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: pageSize
        description: The result page size
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=ListPolicyPrincipals:
    get:
      summary: List Policy Principals
      description: Lists the principals associated with the specified policy.
      operationId: listPolicyPrincipals
      x-api-path-slug: actionlistpolicyprincipals-get
      parameters:
      - in: query
        name: ascendingOrder
        description: Specifies the order for results
        type: string
      - in: query
        name: marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: pageSize
        description: The result page size
        type: string
      - in: query
        name: policyName
        description: The policy name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policy Principals
  /?Action=ListPolicyVersions:
    get:
      summary: List Policy Versions
      description: Lists the versions of the specified policy and identifies the default
        version.
      operationId: listPolicyVersions
      x-api-path-slug: actionlistpolicyversions-get
      parameters:
      - in: query
        name: policyName
        description: The policy name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policy Versions
  /?Action=ListPrincipalPolicies:
    get:
      summary: List Principal Policies
      description: Lists the policies attached to the specified principal.
      operationId: listPrincipalPolicies
      x-api-path-slug: actionlistprincipalpolicies-get
      parameters:
      - in: query
        name: ascendingOrder
        description: Specifies the order for results
        type: string
      - in: query
        name: marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: pageSize
        description: The result page size
        type: string
      - in: query
        name: principal
        description: The principal
        type: string
      responses:
        200:
          description: OK
      tags:
      - Principal Policies
  /?Action=ListPrincipalThings:
    get:
      summary: List Principal Things
      description: Lists the things associated with the specified principal.
      operationId: listPrincipalThings
      x-api-path-slug: actionlistprincipalthings-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of results to return in this operation
        type: string
      - in: query
        name: nextToken
        description: The token for the next set of results, or null if there are no
          additional results
        type: string
      - in: query
        name: principal
        description: The principal
        type: string
      responses:
        200:
          description: OK
      tags:
      - Principal Things
  /?Action=ListThingPrincipals:
    get:
      summary: List Thing Principals
      description: Lists the principals associated with the specified thing.
      operationId: listThingPrincipals
      x-api-path-slug: actionlistthingprincipals-get
      parameters:
      - in: query
        name: thingName
        description: The name of the thing
        type: string
      responses:
        200:
          description: OK
      tags:
      - Thing Principals
  /?Action=ListThings:
    get:
      summary: List Things
      description: Lists your things.
      operationId: listThings
      x-api-path-slug: actionlistthings-get
      parameters:
      - in: query
        name: attributeName
        description: The attribute name used to search for things
        type: string
      - in: query
        name: attributeValue
        description: The attribute value used to search for things
        type: string
      - in: query
        name: maxResults
        description: The maximum number of results to return in this operation
        type: string
      - in: query
        name: nextToken
        description: The token for the next set of results, or null if there are no
          additional results
        type: string
      - in: query
        name: thingTypeName
        description: The name of the thing type used to search for things
        type: string
      responses:
        200:
          description: OK
      tags:
      - Things
  /?Action=ListThingTypes:
    get:
      summary: List Thing Types
      description: Lists the existing thing types.
      operationId: listThingTypes
      x-api-path-slug: actionlistthingtypes-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of results to return in this operation
        type: string
      - in: query
        name: nextToken
        description: The token for the next set of results, or null if there are no
          additional results
        type: string
      - in: query
        name: thingTypeName
        description: The name of the thing type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Thing Types
  /?Action=ListTopicRules:
    get:
      summary: List Topic Rules
      description: Lists the rules for the specific topic.
      operationId: listTopicRules
      x-api-path-slug: actionlisttopicrules-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of results to return
        type: string
      - in: query
        name: nextToken
        description: A token used to retrieve the next value
        type: string
      - in: query
        name: ruleDisabled
        description: Specifies whether the rule is disabled
        type: string
      - in: query
        name: topic
        description: The topic
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topic Rules
  /?Action=RegisterCACertificate:
    get:
      summary: Register C A Certificate
      description: Registers a CA certificate with AWS IoT.
      operationId: registerCACertificate
      x-api-path-slug: actionregistercacertificate-get
      parameters:
      - in: query
        name: allowAutoRegistration
        description: Allows this CA certificate to be used for auto registration of
          device certificates
        type: string
      - in: query
        name: caCertificate
        description: The CA certificate
        type: string
      - in: query
        name: setAsActive
        description: A boolean value that specifies if the CA certificate is set to
          active
        type: string
      - in: query
        name: verificationCertificate
        description: The private key verification certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - CA Certificates
  /?Action=RegisterCertificate:
    get:
      summary: Register Certificate
      description: Registers a device certificate with AWS IoT.
      operationId: registerCertificate
      x-api-path-slug: actionregistercertificate-get
      parameters:
      - in: query
        name: caCertificatePem
        description: The CA certificate used to sign the device certificate being
          registered
        type: string
      - in: query
        name: certificatePem
        description: The certificate data, in PEM format
        type: string
      - in: query
        name: setAsActive
        description: A boolean value that specifies if the CA certificate is set to
          active
        type: string
      - in: query
        name: status
        description: The status of the register certificate request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=RejectCertificateTransfer:
    get:
      summary: Reject Certificate Transfer
      description: Rejects a pending certificate transfer.
      operationId: rejectCertificateTransfer
      x-api-path-slug: actionrejectcertificatetransfer-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate
        type: string
      - in: query
        name: rejectReason
        description: The reason the certificate transfer was rejected
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificate Transfers
  /?Action=ReplaceTopicRule:
    get:
      summary: Replace Topic Rule
      description: Replaces the specified rule.
      operationId: replaceTopicRule
      x-api-path-slug: actionreplacetopicrule-get
      parameters:
      - in: query
        name: ruleName
        description: The name of the rule
        type: string
      - in: query
        name: topicRulePayload
        description: The rule payload
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topic Rules
  /?Action=SetDefaultPolicyVersion:
    get:
      summary: Set Default Policy Version
      description: Sets the specified version of the specified policy as the policy's
        default (operative) version.
      operationId: setDefaultPolicyVersion
      x-api-path-slug: actionsetdefaultpolicyversion-get
      parameters:
      - in: query
        name: policyName
        description: The policy name
        type: string
      - in: query
        name: policyVersionId
        description: The policy version ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=SetLoggingOptions:
    get:
      summary: Set Logging Options
      description: Sets the logging options.
      operationId: setLoggingOptions
      x-api-path-slug: actionsetloggingoptions-get
      parameters:
      - in: query
        name: loggingOptionsPayload
        description: The logging options payload
        type: string
      responses:
        200:
          description: OK
      tags:
      - Logging
  /?Action=TransferCertificate:
    get:
      summary: Transfer Certificate
      description: Transfers the specified certificate to the specified AWS account.
      operationId: transferCertificate
      x-api-path-slug: actiontransfercertificate-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate
        type: string
      - in: query
        name: targetAwsAccount
        description: The AWS account
        type: string
      - in: query
        name: transferMessage
        description: The transfer message
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=UpdateCACertificate:
    get:
      summary: Update C A Certificate
      description: Updates a registered CA certificate.
      operationId: updateCACertificate
      x-api-path-slug: actionupdatecacertificate-get
      parameters:
      - in: query
        name: certificateId
        description: The CA certificate identifier
        type: string
      - in: query
        name: newAutoRegistrationStatus
        description: The new value for the auto registration status
        type: string
      - in: query
        name: newStatus
        description: The updated status of the CA certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - CA Certificates
  /?Action=UpdateCertificate:
    get:
      summary: Update Certificate
      description: Updates the status of the specified certificate.
      operationId: updateCertificate
      x-api-path-slug: actionupdatecertificate-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate
        type: string
      - in: query
        name: newStatus
        description: The new status
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=UpdateThing:
    get:
      summary: Update Thing
      description: Updates the data for a thing.
      operationId: updateThing
      x-api-path-slug: actionupdatething-get
      parameters:
      - in: query
        name: attributePayload
        description: A list of thing attributes, a JSON string containing name-value
          pairs
        type: string
      - in: query
        name: expectedVersion
        description: The expected version of the thing record in the registry
        type: string
      - in: query
        name: removeThingType
        description: Remove a thing type association
        type: string
      - in: query
        name: thingName
        description: The name of the thing to update
        type: string
      - in: query
        name: thingTypeName
        description: The name of the thing type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Things