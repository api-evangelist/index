swagger: "2.0"
x-collection-name: AWS Security Token Service
x-complete: 1
info:
  title: AWS Security Token Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AssumeRole:
    get:
      summary: Assume Role
      description: |-
        Returns a set of temporary security credentials (consisting of an access key ID, a
              secret access key, and a security token) that you can use to access AWS resources that you
              might not normally have access to.
      operationId: assumeRole
      x-api-path-slug: actionassumerole-get
      parameters:
      - in: query
        name: DurationSeconds
        description: The duration, in seconds, of the role session
        type: string
      - in: query
        name: ExternalId
        description: A unique identifier that is used by third parties when assuming
          roles in their      customers accounts
        type: string
      - in: query
        name: Policy
        description: An IAM policy in JSON format
        type: string
      - in: query
        name: RoleArn
        description: The Amazon Resource Name (ARN) of the role to assume
        type: string
      - in: query
        name: RoleSessionName
        description: An identifier for the assumed role session
        type: string
      - in: query
        name: SerialNumber
        description: The identification number of the MFA device that is associated
          with the user who is      making the AssumeRole call
        type: string
      - in: query
        name: TokenCode
        description: The value provided by the MFA device, if the trust policy of
          the role being assumed      requires MFA (that is, if the policy includes
          a condition that tests for MFA)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Roles
  /?Action=AssumeRoleWithSAML:
    get:
      summary: Assume Role With S A M L
      description: |-
        Returns a set of temporary security credentials for users who have been authenticated
              via a SAML authentication response.
      operationId: assumeRoleWithSAML
      x-api-path-slug: actionassumerolewithsaml-get
      parameters:
      - in: query
        name: DurationSeconds
        description: The duration, in seconds, of the role session
        type: string
      - in: query
        name: Policy
        description: An IAM policy in JSON format
        type: string
      - in: query
        name: PrincipalArn
        description: The Amazon Resource Name (ARN) of the SAML provider in IAM that
          describes the      IdP
        type: string
      - in: query
        name: RoleArn
        description: The Amazon Resource Name (ARN) of the role that the caller is
          assuming
        type: string
      - in: query
        name: SAMLAssertion
        description: The base-64 encoded SAML authentication response provided by
          the IdP
        type: string
      responses:
        200:
          description: OK
      tags:
      - Roles
  /?Action=AssumeRoleWithWebIdentity:
    get:
      summary: Assume Role With Web Identity
      description: |-
        Returns a set of temporary security credentials for users who have been authenticated
              in a mobile or web application with a web identity provider, such as Amazon Cognito, Login with Amazon,
              Facebook, Google, or any OpenID Connect-compatible identity provider.
      operationId: assumeRoleWithWebIdentity
      x-api-path-slug: actionassumerolewithwebidentity-get
      parameters:
      - in: query
        name: DurationSeconds
        description: The duration, in seconds, of the role session
        type: string
      - in: query
        name: Policy
        description: An IAM policy in JSON format
        type: string
      - in: query
        name: ProviderId
        description: The fully qualified host component of the domain name of the
          identity      provider
        type: string
      - in: query
        name: RoleArn
        description: The Amazon Resource Name (ARN) of the role that the caller is
          assuming
        type: string
      - in: query
        name: RoleSessionName
        description: An identifier for the assumed role session
        type: string
      - in: query
        name: WebIdentityToken
        description: The OAuth 2
        type: string
      responses:
        200:
          description: OK
      tags:
      - Roles
  /?Action=DecodeAuthorizationMessage:
    get:
      summary: Decode Authorization Message
      description: |-
        Decodes additional information about the authorization status of a request from an
              encoded message returned in response to an AWS request.
      operationId: decodeAuthorizationMessage
      x-api-path-slug: actiondecodeauthorizationmessage-get
      parameters:
      - in: query
        name: EncodedMessage
        description: The encoded message that was returned with the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Roles
  /?Action=GetCallerIdentity:
    get:
      summary: Get Caller Identity
      description: |-
        Returns details about the IAM identity whose credentials are used to call the
              API.
      operationId: getCallerIdentity
      x-api-path-slug: actiongetcalleridentity-get
      parameters:
      - in: query
        name: Account
        description: The AWS account ID number of the account that owns or contains
          the calling      entity
        type: string
      - in: query
        name: Arn
        description: The AWS ARN associated with the calling entity
        type: string
      - in: query
        name: UserId
        description: The unique identifier of the calling entity
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity
  /?Action=GetFederationToken:
    get:
      summary: Get Federation Token
      description: |-
        Returns a set of temporary security credentials (consisting of an access key ID, a
              secret access key, and a security token) for a federated user.
      operationId: getFederationToken
      x-api-path-slug: actiongetfederationtoken-get
      parameters:
      - in: query
        name: DurationSeconds
        description: The duration, in seconds, that the session should last
        type: string
      - in: query
        name: Name
        description: The name of the federated user
        type: string
      - in: query
        name: Policy
        description: An IAM policy in JSON format that is passed with the GetFederationToken      call
          and evaluated along with the policy or policies that are attached to the
          IAM user whose      credentials are used to call GetFederationToken
        type: string
      responses:
        200:
          description: OK
      tags:
      - Federation Token
  /?Action=GetSessionToken:
    get:
      summary: Get Session Token
      description: Returns a set of temporary credentials for an AWS account or IAM
        user.
      operationId: getSessionToken
      x-api-path-slug: actiongetsessiontoken-get
      parameters:
      - in: query
        name: DurationSeconds
        description: The duration, in seconds, that the credentials should remain
          valid
        type: string
      - in: query
        name: SerialNumber
        description: The identification number of the MFA device that is associated
          with the IAM user who      is making the GetSessionToken call
        type: string
      - in: query
        name: TokenCode
        description: The value provided by the MFA device, if MFA is required
        type: string
      responses:
        200:
          description: OK
      tags:
      - Session Token