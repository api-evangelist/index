swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 1
info:
  title: AWS Identity and Access Management API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddClientIDToOpenIDConnectProvider:
    get:
      summary: Add Client I D To Open I D Connect Provider
      description: |-
        Adds a new client ID (also known as audience) to the list of client IDs already
              registered for the specified IAM OpenID Connect (OIDC) provider resource.
      operationId: addClientIDToOpenIDConnectProvider
      x-api-path-slug: actionaddclientidtoopenidconnectprovider-get
      parameters:
      - in: query
        name: ClientID
        description: The client ID (also known as audience) to add to the IAM OpenID
          Connect provider      resource
        type: string
      - in: query
        name: OpenIDConnectProviderArn
        description: The Amazon Resource Name (ARN) of the IAM OpenID Connect (OIDC)
          provider resource to      add the client ID to
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
  /?Action=AddRoleToInstanceProfile:
    get:
      summary: Add Role To Instance Profile
      description: Adds the specified IAM role to the specified instance profile.
      operationId: addRoleToInstanceProfile
      x-api-path-slug: actionaddroletoinstanceprofile-get
      parameters:
      - in: query
        name: InstanceProfileName
        description: The name of the instance profile to update
        type: string
      - in: query
        name: RoleName
        description: The name of the role to add
        type: string
      responses:
        200:
          description: OK
      tags:
      - Role Instance
  /?Action=AddUserToGroup:
    get:
      summary: Add User To Group
      description: Adds the specified user to the specified group.
      operationId: addUserToGroup
      x-api-path-slug: actionaddusertogroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group to update
        type: string
      - in: query
        name: UserName
        description: The name of the user to add
        type: string
      responses:
        200:
          description: OK
      tags:
      - User Groups
  /?Action=AttachGroupPolicy:
    get:
      summary: Attach Group Policy
      description: Attaches the specified managed policy to the specified IAM group.
      operationId: attachGroupPolicy
      x-api-path-slug: actionattachgrouppolicy-get
      parameters:
      - in: query
        name: GroupName
        description: The name (friendly name, not ARN) of the group to attach the
          policy to
        type: string
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy you want to
          attach
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group Policies
  /?Action=AttachRolePolicy:
    get:
      summary: Attach Role Policy
      description: Attaches the specified managed policy to the specified IAM role.
      operationId: attachRolePolicy
      x-api-path-slug: actionattachrolepolicy-get
      parameters:
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy you want to
          attach
        type: string
      - in: query
        name: RoleName
        description: The name (friendly name, not ARN) of the role to attach the policy
          to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Role Policies
  /?Action=AttachUserPolicy:
    get:
      summary: Attach User Policy
      description: Attaches the specified managed policy to the specified user.
      operationId: attachUserPolicy
      x-api-path-slug: actionattachuserpolicy-get
      parameters:
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy you want to
          attach
        type: string
      - in: query
        name: UserName
        description: The name (friendly name, not ARN) of the IAM user to attach the
          policy to
        type: string
      responses:
        200:
          description: OK
      tags:
      - User Policies
  /?Action=ChangePassword:
    get:
      summary: Change Password
      description: Changes the password of the IAM user who is calling this action.
      operationId: changePassword
      x-api-path-slug: actionchangepassword-get
      parameters:
      - in: query
        name: NewPassword
        description: The new password
        type: string
      - in: query
        name: OldPassword
        description: The IAM users current password
        type: string
      responses:
        200:
          description: OK
      tags:
      - Passwords
  /?Action=CreateAccessKey:
    get:
      summary: Create Access Key
      description: |-
        Creates a new AWS secret access key and corresponding AWS access key ID for the
              specified user.
      operationId: createAccessKey
      x-api-path-slug: actioncreateaccesskey-get
      parameters:
      - in: query
        name: UserName
        description: The name of the IAM user that the new key will belong to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Access Keys
  /?Action=CreateAccountAlias:
    get:
      summary: Create Account Alias
      description: Creates an alias for your AWS account.
      operationId: createAccountAlias
      x-api-path-slug: actioncreateaccountalias-get
      parameters:
      - in: query
        name: AccountAlias
        description: The account alias to create
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Alias
  /?Action=CreateGroup:
    get:
      summary: Create Group
      description: Creates a new group.
      operationId: createGroup
      x-api-path-slug: actioncreategroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group to create
        type: string
      - in: query
        name: Path
        description: The path to the group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=CreateInstanceProfile:
    get:
      summary: Create Instance Profile
      description: Creates a new instance profile.
      operationId: createInstanceProfile
      x-api-path-slug: actioncreateinstanceprofile-get
      parameters:
      - in: query
        name: InstanceProfileName
        description: The name of the instance profile to create
        type: string
      - in: query
        name: Path
        description: The path to the instance profile
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Profiles
  /?Action=CreateLoginProfile:
    get:
      summary: Create Login Profile
      description: |-
        Creates a password for the specified user, giving the user the ability to access AWS
              services through the AWS Management Console.
      operationId: createLoginProfile
      x-api-path-slug: actioncreateloginprofile-get
      parameters:
      - in: query
        name: Password
        description: The new password for the user
        type: string
      - in: query
        name: PasswordResetRequired
        description: Specifies whether the user is required to set a new password
          on next sign-in
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user to create a password for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Login Profiles
  /?Action=CreateOpenIDConnectProvider:
    get:
      summary: Create Open I D Connect Provider
      description: Creates an IAM entity to describe an identity provider (IdP) that
        supports.
      operationId: createOpenIDConnectProvider
      x-api-path-slug: actioncreateopenidconnectprovider-get
      parameters:
      - in: query
        name: ClientIDList.member.N
        description: A list of client IDs (also known as audiences)
        type: string
      - in: query
        name: ThumbprintList.member.N
        description: A list of server certificate thumbprints for the OpenID Connect
          (OIDC) identity      providers server certificate(s)
        type: string
      - in: query
        name: Url
        description: The URL of the identity provider
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
  /?Action=CreatePolicy:
    get:
      summary: Create Policy
      description: Creates a new managed policy for your AWS account.
      operationId: createPolicy
      x-api-path-slug: actioncreatepolicy-get
      parameters:
      - in: query
        name: Description
        description: A friendly description of the policy
        type: string
      - in: query
        name: Path
        description: The path for the policy
        type: string
      - in: query
        name: PolicyDocument
        description: The JSON policy document that you want to use as the content
          for the new      policy
        type: string
      - in: query
        name: PolicyName
        description: The friendly name of the policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=CreatePolicyVersion:
    get:
      summary: Create Policy Version
      description: Creates a new version of the specified managed policy.
      operationId: createPolicyVersion
      x-api-path-slug: actioncreatepolicyversion-get
      parameters:
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy to which you
          want to add a new      version
        type: string
      - in: query
        name: PolicyDocument
        description: The JSON policy document that you want to use as the content
          for this new version of      the policy
        type: string
      - in: query
        name: SetAsDefault
        description: Specifies whether to set this version as the policys default
          version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=CreateRole:
    get:
      summary: Create Role
      description: Creates a new role for your AWS account.
      operationId: createRole
      x-api-path-slug: actioncreaterole-get
      parameters:
      - in: query
        name: AssumeRolePolicyDocument
        description: The trust relationship policy document that grants an entity
          permission to assume the      role
        type: string
      - in: query
        name: Path
        description: The path to the role
        type: string
      - in: query
        name: RoleName
        description: The name of the role to create
        type: string
      responses:
        200:
          description: OK
      tags:
      - Roles
  /?Action=CreateSAMLProvider:
    get:
      summary: Create S A M L Provider
      description: |-
        Creates an IAM resource that describes an identity provider (IdP) that supports SAML
              2.
      operationId: createSAMLProvider
      x-api-path-slug: actioncreatesamlprovider-get
      parameters:
      - in: query
        name: Name
        description: The name of the provider to create
        type: string
      - in: query
        name: SAMLMetadataDocument
        description: An XML document generated by an identity provider (IdP) that
          supports SAML 2
        type: string
      responses:
        200:
          description: OK
      tags:
      - SAML Providers
  /?Action=CreateServiceSpecificCredential:
    get:
      summary: Create Service Specific Credential
      description: |-
        Generates a set of credentials consisting of a user name and password that can be used
              to access the service specified in the request.
      operationId: createServiceSpecificCredential
      x-api-path-slug: actioncreateservicespecificcredential-get
      parameters:
      - in: query
        name: ServiceName
        description: The name of the AWS service that is to be associated with the
          credentials
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user that is to be associated with the credentials
        type: string
      responses:
        200:
          description: OK
      tags:
      - Service Specific Credentials
  /?Action=CreateUser:
    get:
      summary: Create User
      description: Creates a new IAM user for your AWS account.
      operationId: createUser
      x-api-path-slug: actioncreateuser-get
      parameters:
      - in: query
        name: Path
        description: The path for the user name
        type: string
      - in: query
        name: UserName
        description: The name of the user to create
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=CreateVirtualMFADevice:
    get:
      summary: Create Virtual M F A Device
      description: Creates a new virtual MFA device for the AWS account.
      operationId: createVirtualMFADevice
      x-api-path-slug: actioncreatevirtualmfadevice-get
      parameters:
      - in: query
        name: Path
        description: The path for the virtual MFA device
        type: string
      - in: query
        name: VirtualMFADeviceName
        description: The name of the virtual MFA device
        type: string
      responses:
        200:
          description: OK
      tags:
      - Virtual MFA Device
  /?Action=DeactivateMFADevice:
    get:
      summary: Deactivate M F A Device
      description: |-
        Deactivates the specified MFA device and removes it from association with the user name
              for which it was originally enabled.
      operationId: deactivateMFADevice
      x-api-path-slug: actiondeactivatemfadevice-get
      parameters:
      - in: query
        name: SerialNumber
        description: The serial number that uniquely identifies the MFA device
        type: string
      - in: query
        name: UserName
        description: The name of the user whose MFA device you want to deactivate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Virtual MFA Device
  /?Action=DeleteAccessKey:
    get:
      summary: Delete Access Key
      description: Deletes the access key pair associated with the specified IAM user.
      operationId: deleteAccessKey
      x-api-path-slug: actiondeleteaccesskey-get
      parameters:
      - in: query
        name: AccessKeyId
        description: The access key ID for the access key ID and secret access key
          you want to      delete
        type: string
      - in: query
        name: UserName
        description: The name of the user whose access key pair you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Access Keys
  /?Action=DeleteAccountAlias:
    get:
      summary: Delete Account Alias
      description: Deletes the specified AWS account alias.
      operationId: deleteAccountAlias
      x-api-path-slug: actiondeleteaccountalias-get
      parameters:
      - in: query
        name: AccountAlias
        description: The name of the account alias to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Alias
  /?Action=DeleteAccountPasswordPolicy:
    get:
      summary: Delete Account Password Policy
      description: Deletes the password policy for the AWS account.
      operationId: deleteAccountPasswordPolicy
      x-api-path-slug: actiondeleteaccountpasswordpolicy-get
      parameters:
      - in: query
        name: LimitExceeded
        description: The request was rejected because it attempted to create resources
          beyond the current      AWS account limits
        type: string
      - in: query
        name: NoSuchEntity
        description: The request was rejected because it referenced an entity that
          does not exist
        type: string
      - in: query
        name: ServiceFailure
        description: The request processing has failed because of an unknown error,
          exception or      failure
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Password Policies
  /?Action=DeleteGroup:
    get:
      summary: Delete Group
      description: Deletes the specified IAM group.
      operationId: deleteGroup
      x-api-path-slug: actiondeletegroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the IAM group to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=DeleteGroupPolicy:
    get:
      summary: Delete Group Policy
      description: |-
        Deletes the specified inline policy that is embedded in the specified IAM
              group.
      operationId: deleteGroupPolicy
      x-api-path-slug: actiondeletegrouppolicy-get
      parameters:
      - in: query
        name: GroupName
        description: The name (friendly name, not ARN) identifying the group that
          the policy is embedded      in
        type: string
      - in: query
        name: PolicyName
        description: The name identifying the policy document to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group Policies
  /?Action=DeleteInstanceProfile:
    get:
      summary: Delete Instance Profile
      description: Deletes the specified instance profile.
      operationId: deleteInstanceProfile
      x-api-path-slug: actiondeleteinstanceprofile-get
      parameters:
      - in: query
        name: InstanceProfileName
        description: The name of the instance profile to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Profiles
  /?Action=DeleteLoginProfile:
    get:
      summary: Delete Login Profile
      description: |-
        Deletes the password for the specified IAM user, which terminates the user's ability
              to access AWS services through the AWS Management Console.
      operationId: deleteLoginProfile
      x-api-path-slug: actiondeleteloginprofile-get
      parameters:
      - in: query
        name: UserName
        description: The name of the user whose password you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Login Profiles
  /?Action=DeleteOpenIDConnectProvider:
    get:
      summary: Delete Open I D Connect Provider
      description: Deletes an OpenID Connect identity provider (IdP) resource object
        in IAM.
      operationId: deleteOpenIDConnectProvider
      x-api-path-slug: actiondeleteopenidconnectprovider-get
      parameters:
      - in: query
        name: OpenIDConnectProviderArn
        description: The Amazon Resource Name (ARN) of the IAM OpenID Connect provider
          resource object to      delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
  /?Action=DeletePolicy:
    get:
      summary: Delete Policy
      description: Deletes the specified managed policy.
      operationId: deletePolicy
      x-api-path-slug: actiondeletepolicy-get
      parameters:
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy you want to
          delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=DeletePolicyVersion:
    get:
      summary: Delete Policy Version
      description: Deletes the specified version from the specified managed policy.
      operationId: deletePolicyVersion
      x-api-path-slug: actiondeletepolicyversion-get
      parameters:
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy from which you
          want to delete a      version
        type: string
      - in: query
        name: VersionId
        description: The policy version to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=DeleteRole:
    get:
      summary: Delete Role
      description: Deletes the specified role.
      operationId: deleteRole
      x-api-path-slug: actiondeleterole-get
      parameters:
      - in: query
        name: RoleName
        description: The name of the role to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Roles
  /?Action=DeleteRolePolicy:
    get:
      summary: Delete Role Policy
      description: |-
        Deletes the specified inline policy that is embedded in the specified IAM
              role.
      operationId: deleteRolePolicy
      x-api-path-slug: actiondeleterolepolicy-get
      parameters:
      - in: query
        name: PolicyName
        description: The name of the inline policy to delete from the specified IAM
          role
        type: string
      - in: query
        name: RoleName
        description: The name (friendly name, not ARN) identifying the role that the
          policy is embedded      in
        type: string
      responses:
        200:
          description: OK
      tags:
      - Role Policies
  /?Action=DeleteSAMLProvider:
    get:
      summary: Delete S A M L Provider
      description: Deletes a SAML provider resource in IAM.
      operationId: deleteSAMLProvider
      x-api-path-slug: actiondeletesamlprovider-get
      parameters:
      - in: query
        name: SAMLProviderArn
        description: The Amazon Resource Name (ARN) of the SAML provider to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - SAML Providers
  /?Action=DeleteServerCertificate:
    get:
      summary: Delete Server Certificate
      description: Deletes the specified server certificate.
      operationId: deleteServerCertificate
      x-api-path-slug: actiondeleteservercertificate-get
      parameters:
      - in: query
        name: ServerCertificateName
        description: The name of the server certificate you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Certificates
  /?Action=DeleteServiceSpecificCredential:
    get:
      summary: Delete Service Specific Credential
      description: Deletes the specified service-specific credential.
      operationId: deleteServiceSpecificCredential
      x-api-path-slug: actiondeleteservicespecificcredential-get
      parameters:
      - in: query
        name: ServiceSpecificCredentialId
        description: The unique identifier of the service-specific credential
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user associated with the service-specific
          credential
        type: string
      responses:
        200:
          description: OK
      tags:
      - Service Specific Credentials
  /?Action=DeleteSigningCertificate:
    get:
      summary: Delete Signing Certificate
      description: Deletes a signing certificate associated with the specified IAM
        user.
      operationId: deleteSigningCertificate
      x-api-path-slug: actiondeletesigningcertificate-get
      parameters:
      - in: query
        name: CertificateId
        description: The ID of the signing certificate to delete
        type: string
      - in: query
        name: UserName
        description: The name of the user the signing certificate belongs to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Signing Certificates
  /?Action=DeleteSSHPublicKey:
    get:
      summary: Delete S S H Public Key
      description: Deletes the specified SSH public key.
      operationId: deleteSSHPublicKey
      x-api-path-slug: actiondeletesshpublickey-get
      parameters:
      - in: query
        name: SSHPublicKeyId
        description: The unique identifier for the SSH public key
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user associated with the SSH public key
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSH Public Key
  /?Action=DeleteUser:
    get:
      summary: Delete User
      description: Deletes the specified IAM user.
      operationId: deleteUser
      x-api-path-slug: actiondeleteuser-get
      parameters:
      - in: query
        name: UserName
        description: The name of the user to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=DeleteUserPolicy:
    get:
      summary: Delete User Policy
      description: |-
        Deletes the specified inline policy that is embedded in the specified IAM
              user.
      operationId: deleteUserPolicy
      x-api-path-slug: actiondeleteuserpolicy-get
      parameters:
      - in: query
        name: PolicyName
        description: The name identifying the policy document to delete
        type: string
      - in: query
        name: UserName
        description: The name (friendly name, not ARN) identifying the user that the
          policy is embedded      in
        type: string
      responses:
        200:
          description: OK
      tags:
      - User Policies
  /?Action=DeleteVirtualMFADevice:
    get:
      summary: Delete Virtual M F A Device
      description: Deletes a virtual MFA device.
      operationId: deleteVirtualMFADevice
      x-api-path-slug: actiondeletevirtualmfadevice-get
      parameters:
      - in: query
        name: SerialNumber
        description: The serial number that uniquely identifies the MFA device
        type: string
      responses:
        200:
          description: OK
      tags:
      - Virtual MFA Devices
  /?Action=DetachGroupPolicy:
    get:
      summary: Detach Group Policy
      description: Removes the specified managed policy from the specified IAM group.
      operationId: detachGroupPolicy
      x-api-path-slug: actiondetachgrouppolicy-get
      parameters:
      - in: query
        name: GroupName
        description: The name (friendly name, not ARN) of the IAM group to detach
          the policy      from
        type: string
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy you want to
          detach
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group Policies
  /?Action=DetachRolePolicy:
    get:
      summary: Detach Role Policy
      description: Removes the specified managed policy from the specified role.
      operationId: detachRolePolicy
      x-api-path-slug: actiondetachrolepolicy-get
      parameters:
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy you want to
          detach
        type: string
      - in: query
        name: RoleName
        description: The name (friendly name, not ARN) of the IAM role to detach the
          policy      from
        type: string
      responses:
        200:
          description: OK
      tags:
      - Role Policies
  /?Action=DetachUserPolicy:
    get:
      summary: Detach User Policy
      description: Removes the specified managed policy from the specified user.
      operationId: detachUserPolicy
      x-api-path-slug: actiondetachuserpolicy-get
      parameters:
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy you want to
          detach
        type: string
      - in: query
        name: UserName
        description: The name (friendly name, not ARN) of the IAM user to detach the
          policy      from
        type: string
      responses:
        200:
          description: OK
      tags:
      - User Policies
  /?Action=EnableMFADevice:
    get:
      summary: Enable M F A Device
      description: Enables the specified MFA device and associates it with the specified
        IAM user.
      operationId: enableMFADevice
      x-api-path-slug: actionenablemfadevice-get
      parameters:
      - in: query
        name: AuthenticationCode1
        description: An authentication code emitted by the device
        type: string
      - in: query
        name: AuthenticationCode2
        description: A subsequent authentication code emitted by the device
        type: string
      - in: query
        name: SerialNumber
        description: The serial number that uniquely identifies the MFA device
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user for whom you want to enable the MFA
          device
        type: string
      responses:
        200:
          description: OK
      tags:
      - MFA Devices
  /?Action=GenerateCredentialReport:
    get:
      summary: Generate Credential Report
      description: Generates a credential report for the AWS account.
      operationId: generateCredentialReport
      x-api-path-slug: actiongeneratecredentialreport-get
      parameters:
      - in: query
        name: Description
        description: Information about the credential report
        type: string
      - in: query
        name: State
        description: Information about the state of the credential report
        type: string
      responses:
        200:
          description: OK
      tags:
      - Credential Reports
  /?Action=GetAccessKeyLastUsed:
    get:
      summary: Get Access Key Last Used
      description: Retrieves information about when the specified access key was last
        used.
      operationId: getAccessKeyLastUsed
      x-api-path-slug: actiongetaccesskeylastused-get
      parameters:
      - in: query
        name: AccessKeyId
        description: The identifier of an access key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Access Keys
  /?Action=GetAccountAuthorizationDetails:
    get:
      summary: Get Account Authorization Details
      description: |-
        Retrieves information about all IAM users, groups, roles, and policies in your AWS
              account, including their relationships to one another.
      operationId: getAccountAuthorizationDetails
      x-api-path-slug: actiongetaccountauthorizationdetails-get
      parameters:
      - in: query
        name: Filter.member.N
        description: A list of entity types used to filter the results
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /?Action=GetAccountPasswordPolicy:
    get:
      summary: Get Account Password Policy
      description: Retrieves the password policy for the AWS account.
      operationId: getAccountPasswordPolicy
      x-api-path-slug: actiongetaccountpasswordpolicy-get
      parameters:
      - in: query
        name: PasswordPolicy
        description: Contains information about the account password policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /?Action=GetAccountSummary:
    get:
      summary: Get Account Summary
      description: |-
        Retrieves information about IAM entity usage and IAM quotas in the AWS
              account.
      operationId: getAccountSummary
      x-api-path-slug: actiongetaccountsummary-get
      parameters:
      - in: query
        name: |-
          SummaryMap
                      , SummaryMap.entry.N.key (key), SummaryMapentry.N.value (value)
        description: A set of key value pairs containing information about IAM entity
          usage and IAM      quotas
        type: string
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /?Action=GetContextKeysForCustomPolicy:
    get:
      summary: Get Context Keys For Custom Policy
      description: Gets a list of all of the context keys referenced in the input
        policies.
      operationId: getContextKeysForCustomPolicy
      x-api-path-slug: actiongetcontextkeysforcustompolicy-get
      parameters:
      - in: query
        name: PolicyInputList.member.N
        description: A list of policies for which you want the list of context keys
          referenced in those      policies
        type: string
      responses:
        200:
          description: OK
      tags:
      - Context Keys For Custom Policies
  /?Action=GetContextKeysForPrincipalPolicy:
    get:
      summary: Get Context Keys For Principal Policy
      description: |-
        Gets a list of all of the context keys referenced in all of the IAM policies attached
              to the specified IAM entity.
      operationId: getContextKeysForPrincipalPolicy
      x-api-path-slug: actiongetcontextkeysforprincipalpolicy-get
      parameters:
      - in: query
        name: PolicyInputList.member.N
        description: An optional list of additional policies for which you want the
          list of context keys      that are referenced
        type: string
      - in: query
        name: PolicySourceArn
        description: The ARN of a user, group, or role whose policies contain the
          context keys that you want      listed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Context Keys For Principal Policies
  /?Action=GetCredentialReport:
    get:
      summary: Get Credential Report
      description: Retrieves a credential report for the AWS account.
      operationId: getCredentialReport
      x-api-path-slug: actiongetcredentialreport-get
      parameters:
      - in: query
        name: Content
        description: Contains the credential report
        type: string
      - in: query
        name: GeneratedTime
        description: The date and time when the credential report was created, in
          ISO 8601 date-time format
        type: string
      - in: query
        name: ReportFormat
        description: The format (MIME type) of the credential report
        type: string
      responses:
        200:
          description: OK
      tags:
      - Credential Reports
  /?Action=GetGroup:
    get:
      summary: Get Group
      description: Returns a list of IAM users that are in the specified IAM group.
      operationId: getGroup
      x-api-path-slug: actiongetgroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=GetGroupPolicy:
    get:
      summary: Get Group Policy
      description: |-
        Retrieves the specified inline policy document that is embedded in the specified IAM
              group.
      operationId: getGroupPolicy
      x-api-path-slug: actiongetgrouppolicy-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group the policy is associated with
        type: string
      - in: query
        name: PolicyName
        description: The name of the policy document to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group Policies
  /?Action=GetInstanceProfile:
    get:
      summary: Get Instance Profile
      description: |-
        Retrieves information about the specified instance profile, including the instance
              profile's path, GUID, ARN, and role.
      operationId: getInstanceProfile
      x-api-path-slug: actiongetinstanceprofile-get
      parameters:
      - in: query
        name: InstanceProfileName
        description: The name of the instance profile to get information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Profiles
  /?Action=GetLoginProfile:
    get:
      summary: Get Login Profile
      description: Retrieves the user name and password-creation date for the specified
        IAM user.
      operationId: getLoginProfile
      x-api-path-slug: actiongetloginprofile-get
      parameters:
      - in: query
        name: UserName
        description: The name of the user whose login profile you want to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Login Profiles
  /?Action=GetOpenIDConnectProvider:
    get:
      summary: Get Open I D Connect Provider
      description: |-
        Returns information about the specified OpenID Connect (OIDC) provider resource object
              in IAM.
      operationId: getOpenIDConnectProvider
      x-api-path-slug: actiongetopenidconnectprovider-get
      parameters:
      - in: query
        name: OpenIDConnectProviderArn
        description: The Amazon Resource Name (ARN) of the OIDC provider resource
          object in IAM to get      information for
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
  /?Action=GetPolicy:
    get:
      summary: Get Policy
      description: |-
        Retrieves information about the specified managed policy, including the policy's
              default version and the total number of IAM users, groups, and roles to which the policy is
              attached.
      operationId: getPolicy
      x-api-path-slug: actiongetpolicy-get
      parameters:
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the managed policy that you
          want information      about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=GetPolicyVersion:
    get:
      summary: Get Policy Version
      description: |-
        Retrieves information about the specified version of the specified managed policy,
              including the policy document.
      operationId: getPolicyVersion
      x-api-path-slug: actiongetpolicyversion-get
      parameters:
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the managed policy that you
          want information      about
        type: string
      - in: query
        name: VersionId
        description: Identifies the policy version to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policies
  /?Action=GetRole:
    get:
      summary: Get Role
      description: |-
        Retrieves information about the specified role, including the role's path, GUID, ARN,
              and the role's trust policy that grants permission to assume the role.
      operationId: getRole
      x-api-path-slug: actiongetrole-get
      parameters:
      - in: query
        name: RoleName
        description: The name of the IAM role to get information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Roles
  /?Action=GetRolePolicy:
    get:
      summary: Get Role Policy
      description: |-
        Retrieves the specified inline policy document that is embedded with the specified
              IAM role.
      operationId: getRolePolicy
      x-api-path-slug: actiongetrolepolicy-get
      parameters:
      - in: query
        name: PolicyName
        description: The name of the policy document to get
        type: string
      - in: query
        name: RoleName
        description: The name of the role associated with the policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Role Policies
  /?Action=GetSAMLProvider:
    get:
      summary: Get S A M L Provider
      description: |-
        Returns the SAML provider metadocument that was uploaded when the IAM SAML provider
              resource object was created or updated.
      operationId: getSAMLProvider
      x-api-path-slug: actiongetsamlprovider-get
      parameters:
      - in: query
        name: SAMLProviderArn
        description: The Amazon Resource Name (ARN) of the SAML provider resource
          object in IAM to get      information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - SAML Providers
  /?Action=GetServerCertificate:
    get:
      summary: Get Server Certificate
      description: Retrieves information about the specified server certificate stored
        in IAM.
      operationId: getServerCertificate
      x-api-path-slug: actiongetservercertificate-get
      parameters:
      - in: query
        name: ServerCertificateName
        description: The name of the server certificate you want to retrieve information
          about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Certificates
  /?Action=GetSSHPublicKey:
    get:
      summary: Get S S H Public Key
      description: Retrieves the specified SSH public key, including metadata about
        the key.
      operationId: getSSHPublicKey
      x-api-path-slug: actiongetsshpublickey-get
      parameters:
      - in: query
        name: Encoding
        description: Specifies the public key encoding format to use in the response
        type: string
      - in: query
        name: SSHPublicKeyId
        description: The unique identifier for the SSH public key
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user associated with the SSH public key
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSH Public Key
  /?Action=GetUser:
    get:
      summary: Get User
      description: |-
        Retrieves information about the specified IAM user, including the user's creation
              date, path, unique ID, and ARN.
      operationId: getUser
      x-api-path-slug: actiongetuser-get
      parameters:
      - in: query
        name: UserName
        description: The name of the user to get information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=GetUserPolicy:
    get:
      summary: Get User Policy
      description: |-
        Retrieves the specified inline policy document that is embedded in the specified IAM
              user.
      operationId: getUserPolicy
      x-api-path-slug: actiongetuserpolicy-get
      parameters:
      - in: query
        name: PolicyName
        description: The name of the policy document to get
        type: string
      - in: query
        name: UserName
        description: The name of the user who the policy is associated with
        type: string
      responses:
        200:
          description: OK
      tags:
      - User Policies
  /?Action=ListAccessKeys:
    get:
      summary: List Access Keys
      description: Returns information about the access key IDs associated with the
        specified IAM user.
      operationId: listAccessKeys
      x-api-path-slug: actionlistaccesskeys-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: UserName
        description: The name of the user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Access Keys
  /?Action=ListAccountAliases:
    get:
      summary: List Account Aliases
      description: |-
        Lists the account alias associated with the AWS account (Note: you can have only
              one).
      operationId: listAccountAliases
      x-api-path-slug: actionlistaccountaliases-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Aliases
  /?Action=ListAttachedGroupPolicies:
    get:
      summary: List Attached Group Policies
      description: Lists all managed policies that are attached to the specified IAM
        group.
      operationId: listAttachedGroupPolicies
      x-api-path-slug: actionlistattachedgrouppolicies-get
      parameters:
      - in: query
        name: GroupName
        description: The name (friendly name, not ARN) of the group to list attached
          policies for
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attached Group Policies
  /?Action=ListAttachedRolePolicies:
    get:
      summary: List Attached Role Policies
      description: Lists all managed policies that are attached to the specified IAM
        role.
      operationId: listAttachedRolePolicies
      x-api-path-slug: actionlistattachedrolepolicies-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      - in: query
        name: RoleName
        description: The name (friendly name, not ARN) of the role to list attached
          policies for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attached Role Policies
  /?Action=ListAttachedUserPolicies:
    get:
      summary: List Attached User Policies
      description: Lists all managed policies that are attached to the specified IAM
        user.
      operationId: listAttachedUserPolicies
      x-api-path-slug: actionlistattacheduserpolicies-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      - in: query
        name: UserName
        description: The name (friendly name, not ARN) of the user to list attached
          policies for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attached Use rPolicies
  /?Action=ListEntitiesForPolicy:
    get:
      summary: List Entities For Policy
      description: |-
        Lists all IAM users, groups, and roles that the specified managed policy is attached
              to.
      operationId: listEntitiesForPolicy
      x-api-path-slug: actionlistentitiesforpolicy-get
      parameters:
      - in: query
        name: EntityFilter
        description: The entity type to use for filtering the results
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy for which you
          want the      versions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Entities For Policies
  /?Action=ListGroupPolicies:
    get:
      summary: List Group Policies
      description: |-
        Lists the names of the inline policies that are embedded in the specified IAM
              group.
      operationId: listGroupPolicies
      x-api-path-slug: actionlistgrouppolicies-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group to list policies for
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group Policies
  /?Action=ListGroups:
    get:
      summary: List Groups
      description: Lists the IAM groups that have the specified path prefix.
      operationId: listGroups
      x-api-path-slug: actionlistgroups-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=ListGroupsForUser:
    get:
      summary: List Groups For User
      description: Lists the IAM groups that the specified IAM user belongs to.
      operationId: listGroupsForUser
      x-api-path-slug: actionlistgroupsforuser-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: UserName
        description: The name of the user to list groups for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups For User
  /?Action=ListInstanceProfiles:
    get:
      summary: List Instance Profiles
      description: Lists the instance profiles that have the specified path prefix.
      operationId: listInstanceProfiles
      x-api-path-slug: actionlistinstanceprofiles-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Profiles
  /?Action=ListInstanceProfilesForRole:
    get:
      summary: List Instance Profiles For Role
      description: Lists the instance profiles that have the specified associated
        IAM role.
      operationId: listInstanceProfilesForRole
      x-api-path-slug: actionlistinstanceprofilesforrole-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: RoleName
        description: The name of the role to list instance profiles for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Profiles For Role
  /?Action=ListMFADevices:
    get:
      summary: List M F A Devices
      description: Lists the MFA devices for an IAM user.
      operationId: listMFADevices
      x-api-path-slug: actionlistmfadevices-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: UserName
        description: The name of the user whose MFA devices you want to list
        type: string
      responses:
        200:
          description: OK
      tags:
      - MFA Devices
  /?Action=ListOpenIDConnectProviders:
    get:
      summary: List Open I D Connect Providers
      description: |-
        Lists information about the IAM OpenID Connect (OIDC) provider resource objects
              defined in the AWS account.
      operationId: listOpenIDConnectProviders
      x-api-path-slug: actionlistopenidconnectproviders-get
      parameters:
      - in: query
        name: OpenIDConnectProviderList.member.N
        description: The list of IAM OIDC provider resource objects defined in the
          AWS      account
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
  /?Action=ListPolicies:
    get:
      summary: List Policies
      description: |-
        Lists all the managed policies that are available in your AWS account, including your
              own customer-defined managed policies and all AWS managed policies.
      operationId: listPolicies
      x-api-path-slug: actionlistpolicies-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: OnlyAttached
        description: A flag to filter the results to only the attached policies
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      - in: query
        name: Scope
        description: The scope to use for filtering the results
        type: string
      responses:
        200:
          description: OK
      tags:
      - listPolicies
  /?Action=ListPolicyVersions:
    get:
      summary: List Policy Versions
      description: |-
        Lists information about the versions of the specified managed policy, including the
              version that is currently set as the policy's default version.
      operationId: listPolicyVersions
      x-api-path-slug: actionlistpolicyversions-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy for which you
          want the      versions
        type: string
      responses:
        200:
          description: OK
      tags:
      - Policy Versions
  /?Action=ListRolePolicies:
    get:
      summary: List Role Policies
      description: |-
        Lists the names of the inline policies that are embedded in the specified IAM
              role.
      operationId: listRolePolicies
      x-api-path-slug: actionlistrolepolicies-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: RoleName
        description: The name of the role to list policies for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Role Policies
  /?Action=ListRoles:
    get:
      summary: List Roles
      description: Lists the IAM roles that have the specified path prefix.
      operationId: listRoles
      x-api-path-slug: actionlistroles-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Roles
  /?Action=ListSAMLProviders:
    get:
      summary: List S A M L Providers
      description: Lists the SAML provider resource objects defined in IAM in the
        account.
      operationId: listSAMLProviders
      x-api-path-slug: actionlistsamlproviders-get
      parameters:
      - in: query
        name: SAMLProviderList.member.N
        description: The list of SAML provider resource objects defined in IAM for
          this AWS      account
        type: string
      responses:
        200:
          description: OK
      tags:
      - SAML Providers
  /?Action=ListServerCertificates:
    get:
      summary: List Server Certificates
      description: Lists the server certificates stored in IAM that have the specified
        path prefix.
      operationId: listServerCertificates
      x-api-path-slug: actionlistservercertificates-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Serve rCertificates
  /?Action=ListServiceSpecificCredentials:
    get:
      summary: List Service Specific Credentials
      description: |-
        Returns information about the service-specific credentials associated with the
              specified IAM user.
      operationId: listServiceSpecificCredentials
      x-api-path-slug: actionlistservicespecificcredentials-get
      parameters:
      - in: query
        name: ServiceName
        description: Filters the returned results to only those for the specified
          AWS service
        type: string
      - in: query
        name: UserName
        description: The name of the user whose service-specific credentials you want
          information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Service Specific Credentials
  /?Action=ListSigningCertificates:
    get:
      summary: List Signing Certificates
      description: |-
        Returns information about the signing certificates associated with the specified IAM
              user.
      operationId: listSigningCertificates
      x-api-path-slug: actionlistsigningcertificates-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user whose signing certificates you want
          to examine
        type: string
      responses:
        200:
          description: OK
      tags:
      - Signing Certificates
  /?Action=ListSSHPublicKeys:
    get:
      summary: List S S H Public Keys
      description: Returns information about the SSH public keys associated with the
        specified IAM user.
      operationId: listSSHPublicKeys
      x-api-path-slug: actionlistsshpublickeys-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user to list SSH public keys for
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSH Public Keys
  /?Action=ListUserPolicies:
    get:
      summary: List User Policies
      description: Lists the names of the inline policies embedded in the specified
        IAM user.
      operationId: listUserPolicies
      x-api-path-slug: actionlistuserpolicies-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: UserName
        description: The name of the user to list policies for
        type: string
      responses:
        200:
          description: OK
      tags:
      - User Policies
  /?Action=ListUsers:
    get:
      summary: List Users
      description: Lists the IAM users that have the specified path prefix.
      operationId: listUsers
      x-api-path-slug: actionlistusers-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=ListVirtualMFADevices:
    get:
      summary: List Virtual M F A Devices
      description: Lists the virtual MFA devices defined in the AWS account by assignment
        status.
      operationId: listVirtualMFADevices
      x-api-path-slug: actionlistvirtualmfadevices-get
      parameters:
      - in: query
        name: AssignmentStatus
        description: The status (Unassigned or Assigned) of the devices to list
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Virtual MFA Devices
  /?Action=PutGroupPolicy:
    get:
      summary: Put Group Policy
      description: |-
        Adds or updates an inline policy document that is embedded in the specified IAM
              group.
      operationId: putGroupPolicy
      x-api-path-slug: actionputgrouppolicy-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group to associate the policy with
        type: string
      - in: query
        name: PolicyDocument
        description: The policy document
        type: string
      - in: query
        name: PolicyName
        description: The name of the policy document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group Policies
  /?Action=PutRolePolicy:
    get:
      summary: Put Role Policy
      description: |-
        Adds or updates an inline policy document that is embedded in the specified IAM
              role.
      operationId: putRolePolicy
      x-api-path-slug: actionputrolepolicy-get
      parameters:
      - in: query
        name: PolicyDocument
        description: The policy document
        type: string
      - in: query
        name: PolicyName
        description: The name of the policy document
        type: string
      - in: query
        name: RoleName
        description: The name of the role to associate the policy with
        type: string
      responses:
        200:
          description: OK
      tags:
      - Role Policies
  /?Action=PutUserPolicy:
    get:
      summary: Put User Policy
      description: |-
        Adds or updates an inline policy document that is embedded in the specified IAM
              user.
      operationId: putUserPolicy
      x-api-path-slug: actionputuserpolicy-get
      parameters:
      - in: query
        name: PolicyDocument
        description: The policy document
        type: string
      - in: query
        name: PolicyName
        description: The name of the policy document
        type: string
      - in: query
        name: UserName
        description: The name of the user to associate the policy with
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users Policies
  /?Action=RemoveClientIDFromOpenIDConnectProvider:
    get:
      summary: Remove Client I D From Open I D Connect Provider
      description: |-
        Removes the specified client ID (also known as audience) from the list of client IDs
              registered for the specified IAM OpenID Connect (OIDC) provider resource object.
      operationId: removeClientIDFromOpenIDConnectProvider
      x-api-path-slug: actionremoveclientidfromopenidconnectprovider-get
      parameters:
      - in: query
        name: ClientID
        description: The client ID (also known as audience) to remove from the IAM
          OIDC provider resource
        type: string
      - in: query
        name: OpenIDConnectProviderArn
        description: The Amazon Resource Name (ARN) of the IAM OIDC provider resource
          to remove the client      ID from
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
  /?Action=RemoveRoleFromInstanceProfile:
    get:
      summary: Remove Role From Instance Profile
      description: Removes the specified IAM role from the specified EC2 instance
        profile.
      operationId: removeRoleFromInstanceProfile
      x-api-path-slug: actionremoverolefrominstanceprofile-get
      parameters:
      - in: query
        name: InstanceProfileName
        description: The name of the instance profile to update
        type: string
      - in: query
        name: RoleName
        description: The name of the role to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - Role From Instance Profiles
  /?Action=RemoveUserFromGroup:
    get:
      summary: Remove User From Group
      description: Removes the specified user from the specified group.
      operationId: removeUserFromGroup
      x-api-path-slug: actionremoveuserfromgroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group to update
        type: string
      - in: query
        name: UserName
        description: The name of the user to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - User From Groups
  /?Action=ResetServiceSpecificCredential:
    get:
      summary: Reset Service Specific Credential
      description: Resets the password for a service-specific credential.
      operationId: resetServiceSpecificCredential
      x-api-path-slug: actionresetservicespecificcredential-get
      parameters:
      - in: query
        name: ServiceSpecificCredentialId
        description: The unique identifier of the service-specific credential
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user associated with the service-specific
          credential
        type: string
      responses:
        200:
          description: OK
      tags:
      - Service Specific Credentials
  /?Action=ResyncMFADevice:
    get:
      summary: Resync M F A Device
      description: |-
        Synchronizes the specified MFA device with its IAM resource object on the AWS
              servers.
      operationId: resyncMFADevice
      x-api-path-slug: actionresyncmfadevice-get
      parameters:
      - in: query
        name: AuthenticationCode1
        description: An authentication code emitted by the device
        type: string
      - in: query
        name: AuthenticationCode2
        description: A subsequent authentication code emitted by the device
        type: string
      - in: query
        name: SerialNumber
        description: Serial number that uniquely identifies the MFA device
        type: string
      - in: query
        name: UserName
        description: The name of the user whose MFA device you want to resynchronize
        type: string
      responses:
        200:
          description: OK
      tags:
      - MFA Devices
  /?Action=SetDefaultPolicyVersion:
    get:
      summary: Set Default Policy Version
      description: |-
        Sets the specified version of the specified policy as the policy's default (operative)
              version.
      operationId: setDefaultPolicyVersion
      x-api-path-slug: actionsetdefaultpolicyversion-get
      parameters:
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy whose default
          version you want to      set
        type: string
      - in: query
        name: VersionId
        description: The version of the policy to set as the default (operative) version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Default Policy Versions
  /?Action=SimulateCustomPolicy:
    get:
      summary: Simulate Custom Policy
      description: |-
        Simulate how a set of IAM policies and optionally a resource-based policy works with
              a list of API actions and AWS resources to determine the policies' effective permissions.
      operationId: simulateCustomPolicy
      x-api-path-slug: actionsimulatecustompolicy-get
      parameters:
      - in: query
        name: ActionNames.member.N
        description: A list of names of API actions to evaluate in the simulation
        type: string
      - in: query
        name: CallerArn
        description: The ARN of the IAM user that you want to use as the simulated
          caller of the APIs
        type: string
      - in: query
        name: ContextEntries.member.N
        description: A list of context keys and corresponding values for the simulation
          to use
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PolicyInputList.member.N
        description: A list of policy documents to include in the simulation
        type: string
      - in: query
        name: ResourceArns.member.N
        description: A list of ARNs of AWS resources to include in the simulation
        type: string
      - in: query
        name: ResourceHandlingOption
        description: Specifies the type of simulation to run
        type: string
      - in: query
        name: ResourceOwner
        description: An AWS account ID that specifies the owner of any simulated resource
          that does not      identify its owner in the resource ARN, such as an S3
          bucket or object
        type: string
      - in: query
        name: ResourcePolicy
        description: A resource-based policy to include in the simulation provided
          as a string
        type: string
      responses:
        200:
          description: OK
      tags:
      - Custom Policies
  /?Action=SimulatePrincipalPolicy:
    get:
      summary: Simulate Principal Policy
      description: |-
        Simulate how a set of IAM policies attached to an IAM entity works with a list of
              API actions and AWS resources to determine the policies' effective permissions.
      operationId: simulatePrincipalPolicy
      x-api-path-slug: actionsimulateprincipalpolicy-get
      parameters:
      - in: query
        name: ActionNames.member.N
        description: A list of names of API actions to evaluate in the simulation
        type: string
      - in: query
        name: CallerArn
        description: The ARN of the IAM user that you want to specify as the simulated
          caller of the APIs
        type: string
      - in: query
        name: ContextEntries.member.N
        description: A list of context keys and corresponding values for the simulation
          to use
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PolicyInputList.member.N
        description: An optional list of additional policy documents to include in
          the simulation
        type: string
      - in: query
        name: PolicySourceArn
        description: The Amazon Resource Name (ARN) of a user, group, or role whose
          policies you want to      include in the simulation
        type: string
      - in: query
        name: ResourceArns.member.N
        description: A list of ARNs of AWS resources to include in the simulation
        type: string
      - in: query
        name: ResourceHandlingOption
        description: Specifies the type of simulation to run
        type: string
      - in: query
        name: ResourceOwner
        description: An AWS account ID that specifies the owner of any simulated resource
          that does not      identify its owner in the resource ARN, such as an S3
          bucket or object
        type: string
      - in: query
        name: ResourcePolicy
        description: A resource-based policy to include in the simulation provided
          as a string
        type: string
      responses:
        200:
          description: OK
      tags:
      - Principal Policies
  /?Action=UpdateAccessKey:
    get:
      summary: Update Access Key
      description: Changes the status of the specified access key from Active to Inactive,
        or vice versa.
      operationId: updateAccessKey
      x-api-path-slug: actionupdateaccesskey-get
      parameters:
      - in: query
        name: AccessKeyId
        description: The access key ID of the secret access key you want to update
        type: string
      - in: query
        name: Status
        description: The status you want to assign to the secret access key
        type: string
      - in: query
        name: UserName
        description: The name of the user whose key you want to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Access Keys
  /?Action=UpdateAccountPasswordPolicy:
    get:
      summary: Update Account Password Policy
      description: Updates the password policy settings for the AWS account.
      operationId: updateAccountPasswordPolicy
      x-api-path-slug: actionupdateaccountpasswordpolicy-get
      parameters:
      - in: query
        name: AllowUsersToChangePassword
        description: Allows all IAM users in your account to use the AWS Management
          Console to change their own      passwords
        type: string
      - in: query
        name: HardExpiry
        description: Prevents IAM users from setting a new password after their password
          has      expired
        type: string
      - in: query
        name: MaxPasswordAge
        description: The number of days that an IAM user password is valid
        type: string
      - in: query
        name: MinimumPasswordLength
        description: The minimum number of characters allowed in an IAM user password
        type: string
      - in: query
        name: PasswordReusePrevention
        description: Specifies the number of previous passwords that IAM users are
          prevented from reusing
        type: string
      - in: query
        name: RequireLowercaseCharacters
        description: Specifies whether IAM user passwords must contain at least one
          lowercase character      from the ISO basic Latin alphabet (a to z)
        type: string
      - in: query
        name: RequireNumbers
        description: Specifies whether IAM user passwords must contain at least one
          numeric character (0      to 9)
        type: string
      - in: query
        name: RequireSymbols
        description: 'Specifies whether IAM user passwords must contain at least one
          of the following      non-alphanumeric characters:'
        type: string
      - in: query
        name: RequireUppercaseCharacters
        description: Specifies whether IAM user passwords must contain at least one
          uppercase character      from the ISO basic Latin alphabet (A to Z)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Password Policy
  /?Action=UpdateAssumeRolePolicy:
    get:
      summary: Update Assume Role Policy
      description: Updates the policy that grants an IAM entity permission to assume
        a role.
      operationId: updateAssumeRolePolicy
      x-api-path-slug: actionupdateassumerolepolicy-get
      parameters:
      - in: query
        name: PolicyDocument
        description: The policy that grants an entity permission to assume the role
        type: string
      - in: query
        name: RoleName
        description: The name of the role to update with the new policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Assume Role Policy
  /?Action=UpdateGroup:
    get:
      summary: Update Group
      description: Updates the name and/or the path of the specified IAM group.
      operationId: updateGroup
      x-api-path-slug: actionupdategroup-get
      parameters:
      - in: query
        name: GroupName
        description: Name of the IAM group to update
        type: string
      - in: query
        name: NewGroupName
        description: New name for the IAM group
        type: string
      - in: query
        name: NewPath
        description: New path for the IAM group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=UpdateLoginProfile:
    get:
      summary: Update Login Profile
      description: Changes the password for the specified IAM user.
      operationId: updateLoginProfile
      x-api-path-slug: actionupdateloginprofile-get
      parameters:
      - in: query
        name: Password
        description: The new password for the specified IAM user
        type: string
      - in: query
        name: PasswordResetRequired
        description: Allows this new password to be used only once by requiring the
          specified IAM user to      set a new password on next sign-in
        type: string
      - in: query
        name: UserName
        description: The name of the user whose password you want to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Login Profiles
  /?Action=UpdateOpenIDConnectProviderThumbprint:
    get:
      summary: Update Open I D Connect Provider Thumbprint
      description: |-
        Replaces the existing list of server certificate thumbprints associated with an OpenID
              Connect (OIDC) provider resource object with a new list of thumbprints.
      operationId: updateOpenIDConnectProviderThumbprint
      x-api-path-slug: actionupdateopenidconnectproviderthumbprint-get
      parameters:
      - in: query
        name: OpenIDConnectProviderArn
        description: The Amazon Resource Name (ARN) of the IAM OIDC provider resource
          object for which you      want to update the thumbprint
        type: string
      - in: query
        name: ThumbprintList.member.N
        description: A list of certificate thumbprints that are associated with the
          specified IAM OpenID      Connect provider
        type: string
      responses:
        200:
          description: OK
      tags:
      - OpenID Connect Providers
  /?Action=UpdateSAMLProvider:
    get:
      summary: Update S A M L Provider
      description: Updates the metadata document for an existing SAML provider resource
        object.
      operationId: updateSAMLProvider
      x-api-path-slug: actionupdatesamlprovider-get
      parameters:
      - in: query
        name: SAMLMetadataDocument
        description: An XML document generated by an identity provider (IdP) that
          supports SAML 2
        type: string
      - in: query
        name: SAMLProviderArn
        description: The Amazon Resource Name (ARN) of the SAML provider to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - SAML Provider
  /?Action=UpdateServerCertificate:
    get:
      summary: Update Server Certificate
      description: |-
        Updates the name and/or the path of the specified server certificate stored in
              IAM.
      operationId: updateServerCertificate
      x-api-path-slug: actionupdateservercertificate-get
      parameters:
      - in: query
        name: NewPath
        description: The new path for the server certificate
        type: string
      - in: query
        name: NewServerCertificateName
        description: The new name for the server certificate
        type: string
      - in: query
        name: ServerCertificateName
        description: The name of the server certificate that you want to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Certificates
  /?Action=UpdateServiceSpecificCredential:
    get:
      summary: Update Service Specific Credential
      description: |-
        Sets the status of a service-specific credential to Active or
                Inactive.
      operationId: updateServiceSpecificCredential
      x-api-path-slug: actionupdateservicespecificcredential-get
      parameters:
      - in: query
        name: ServiceSpecificCredentialId
        description: The unique identifier of the service-specific credential
        type: string
      - in: query
        name: Status
        description: The status to be assigned to the service-specific credential
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user associated with the service-specific
          credential
        type: string
      responses:
        200:
          description: OK
      tags:
      - Service Specific Credentials
  /?Action=UpdateSigningCertificate:
    get:
      summary: Update Signing Certificate
      description: |-
        Changes the status of the specified user signing certificate from active to disabled,
              or vice versa.
      operationId: updateSigningCertificate
      x-api-path-slug: actionupdatesigningcertificate-get
      parameters:
      - in: query
        name: CertificateId
        description: The ID of the signing certificate you want to update
        type: string
      - in: query
        name: Status
        description: The status you want to assign to the certificate
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user the signing certificate belongs to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Signing Certificates
  /?Action=UpdateSSHPublicKey:
    get:
      summary: Update S S H Public Key
      description: Sets the status of an IAM user's SSH public key to active or inactive.
      operationId: updateSSHPublicKey
      x-api-path-slug: actionupdatesshpublickey-get
      parameters:
      - in: query
        name: SSHPublicKeyId
        description: The unique identifier for the SSH public key
        type: string
      - in: query
        name: Status
        description: The status to assign to the SSH public key
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user associated with the SSH public key
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSH Public Keys
  /?Action=UpdateUser:
    get:
      summary: Update User
      description: Updates the name and/or the path of the specified IAM user.
      operationId: updateUser
      x-api-path-slug: actionupdateuser-get
      parameters:
      - in: query
        name: NewPath
        description: New path for the IAM user
        type: string
      - in: query
        name: NewUserName
        description: New name for the user
        type: string
      - in: query
        name: UserName
        description: Name of the user to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=UploadServerCertificate:
    get:
      summary: Upload Server Certificate
      description: Uploads a server certificate entity for the AWS account.
      operationId: uploadServerCertificate
      x-api-path-slug: actionuploadservercertificate-get
      parameters:
      - in: query
        name: CertificateBody
        description: The contents of the public key certificate in PEM-encoded format
        type: string
      - in: query
        name: CertificateChain
        description: The contents of the certificate chain
        type: string
      - in: query
        name: Path
        description: The path for the server certificate
        type: string
      - in: query
        name: PrivateKey
        description: The contents of the private key in PEM-encoded format
        type: string
      - in: query
        name: ServerCertificateName
        description: The name for the server certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Certificates
  /?Action=UploadSigningCertificate:
    get:
      summary: Upload Signing Certificate
      description: Uploads an X.
      operationId: uploadSigningCertificate
      x-api-path-slug: actionuploadsigningcertificate-get
      parameters:
      - in: query
        name: CertificateBody
        description: The contents of the signing certificate
        type: string
      - in: query
        name: UserName
        description: The name of the user the signing certificate is for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Signing Certificates
  /?Action=UploadSSHPublicKey:
    get:
      summary: Upload S S H Public Key
      description: Uploads an SSH public key and associates it with the specified
        IAM user.
      operationId: uploadSSHPublicKey
      x-api-path-slug: actionuploadsshpublickey-get
      parameters:
      - in: query
        name: SSHPublicKeyBody
        description: The SSH public key
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user to associate the SSH public key with
        type: string
      responses:
        200:
          description: OK
      tags:
      - SSH Public Key