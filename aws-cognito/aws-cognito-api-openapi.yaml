swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddCustomAttributes:
    get:
      summary: Add Custom Attributes
      description: Adds additional user attributes to the user pool schema.
      operationId: addCustomAttributes
      x-api-path-slug: actionaddcustomattributes-get
      parameters:
      - in: query
        name: CustomAttributes
        description: An array of custom attributes, such as Mutable and Name
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to add custom            attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attributes
  /?Action=AdminAddUserToGroup:
    get:
      summary: Admin Add User To Group
      description: Adds the specified user to the specified group.
      operationId: adminAddUserToGroup
      x-api-path-slug: actionadminaddusertogroup-get
      parameters:
      - in: query
        name: GroupName
        description: The group name
        type: string
      - in: query
        name: Username
        description: The username for the user
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /?Action=AdminConfirmSignUp:
    get:
      summary: Admin Confirm Sign Up
      description: Confirms user registration as an admin without using a confirmation
        code.
      operationId: adminConfirmSignUp
      x-api-path-slug: actionadminconfirmsignup-get
      parameters:
      - in: query
        name: Username
        description: The user name for which you want to confirm user registration
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for which you want to confirm user registration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Sign Up
  /?Action=AdminCreateUser:
    get:
      summary: Admin Create User
      description: |-
        Creates a new user in the specified user pool and sends a welcome message via email
                    or phone (SMS).
      operationId: adminCreateUser
      x-api-path-slug: actionadmincreateuser-get
      parameters:
      - in: query
        name: DesiredDeliveryMediums
        description: Specify EMAIL if email will be used to send the welcome message
        type: string
      - in: query
        name: ForceAliasCreation
        description: This parameter is only used if the phone_number_verified or email_verified            attribute
          is set to True
        type: string
      - in: query
        name: MessageAction
        description: Set to RESEND to resend the invitation message to a user that
          already exists and            reset the expiration limit on the users account
        type: string
      - in: query
        name: TemporaryPassword
        description: The users temporary password
        type: string
      - in: query
        name: UserAttributes
        description: An array of name-value pairs that contain user attributes and
          attribute values to            be set for the user to be created
        type: string
      - in: query
        name: Username
        description: The username for the user
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where the user will be created
        type: string
      - in: query
        name: ValidationData
        description: The users validation data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminDeleteUser:
    get:
      summary: Admin Delete User
      description: Deletes a user as an administrator.
      operationId: adminDeleteUser
      x-api-path-slug: actionadmindeleteuser-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user you wish to delete
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to delete the
          user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminDeleteUserAttributes:
    get:
      summary: Admin Delete User Attributes
      description: Deletes the user attributes in a user pool as an administrator.
      operationId: adminDeleteUserAttributes
      x-api-path-slug: actionadmindeleteuserattributes-get
      parameters:
      - in: query
        name: UserAttributeNames
        description: An array of strings representing the user attribute names you
          wish to            delete
        type: string
      - in: query
        name: Username
        description: The user name of the user from which you would like to delete
          attributes
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to delete user            attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminDisableUser:
    get:
      summary: Admin Disable User
      description: Disables the specified user as an administrator.
      operationId: adminDisableUser
      x-api-path-slug: actionadmindisableuser-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user you wish to disable
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to disable
          the user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminEnableUser:
    get:
      summary: Admin Enable User
      description: Enables the specified user as an administrator.
      operationId: adminEnableUser
      x-api-path-slug: actionadminenableuser-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user you wish to enable
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to enable the
          user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminForgetDevice:
    get:
      summary: Admin Forget Device
      description: Forgets the device, as an administrator.
      operationId: adminForgetDevice
      x-api-path-slug: actionadminforgetdevice-get
      parameters:
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      - in: query
        name: Username
        description: The user name
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Devices
  /?Action=AdminGetDevice:
    get:
      summary: Admin Get Device
      description: Gets the device, as an administrator.
      operationId: adminGetDevice
      x-api-path-slug: actionadmingetdevice-get
      parameters:
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      - in: query
        name: Username
        description: The user name
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - http://laneworks.net/api-stack/pull/pull-amazon-cognito-sync.php
  /?Action=AdminGetUser:
    get:
      summary: Admin Get User
      description: Gets the specified user by user name in a user pool as an administrator.
      operationId: adminGetUser
      x-api-path-slug: actionadmingetuser-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user you wish to retrieve
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to get information
          about the            user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminInitiateAuth:
    get:
      summary: Admin Initiate Auth
      description: Initiates the authentication flow, as an administrator.
      operationId: adminInitiateAuth
      x-api-path-slug: actionadmininitiateauth-get
      parameters:
      - in: query
        name: AuthFlow
        description: The authentication flow
        type: string
      - in: query
        name: AuthParameters
        description: The authentication parameters
        type: string
      - in: query
        name: ClientId
        description: The client app ID
        type: string
      - in: query
        name: ClientMetadata
        description: The client app metadata
        type: string
      - in: query
        name: UserPoolId
        description: The ID of the Amazon Cognito user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Authnetication
  /?Action=AdminListDevices:
    get:
      summary: Admin List Devices
      description: Lists devices, as an administrator.
      operationId: adminListDevices
      x-api-path-slug: actionadminlistdevices-get
      parameters:
      - in: query
        name: Limit
        description: The limit of the devices request
        type: string
      - in: query
        name: PaginationToken
        description: The pagination token
        type: string
      - in: query
        name: Username
        description: The user name
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - http://laneworks.net/api-stack/pull/pull-amazon-cognito-sync.php
  /?Action=AdminListGroupsForUser:
    get:
      summary: Admin List Groups For User
      description: Lists the groups that the user belongs to.
      operationId: adminListGroupsForUser
      x-api-path-slug: actionadminlistgroupsforuser-get
      parameters:
      - in: query
        name: Limit
        description: The limit of the request to list groups
        type: string
      - in: query
        name: NextToken
        description: An identifier that was returned from the previous call to this
          operation, which can            be used to return the next set of items
          in the list
        type: string
      - in: query
        name: Username
        description: The username for the user
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /?Action=AdminRemoveUserFromGroup:
    get:
      summary: Admin Remove User From Group
      description: Removes the specified user from the specified group.
      operationId: adminRemoveUserFromGroup
      x-api-path-slug: actionadminremoveuserfromgroup-get
      parameters:
      - in: query
        name: GroupName
        description: The group name
        type: string
      - in: query
        name: Username
        description: The username for the user
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /?Action=AdminResetUserPassword:
    get:
      summary: Admin Reset User Password
      description: Resets the specified user's password in a user pool as an administrator.
      operationId: adminResetUserPassword
      x-api-path-slug: actionadminresetuserpassword-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user whose password you wish to reset
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to reset the
          users            password
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Passwords
  /?Action=AdminRespondToAuthChallenge:
    get:
      summary: Admin Respond To Auth Challenge
      description: Responds to an authentication challenge, as an administrator.
      operationId: adminRespondToAuthChallenge
      x-api-path-slug: actionadminrespondtoauthchallenge-get
      parameters:
      - in: query
        name: ChallengeName
        description: The name of the challenge
        type: string
      - in: query
        name: ChallengeResponses
        description: The challenge response
        type: string
      - in: query
        name: ClientId
        description: The client ID
        type: string
      - in: query
        name: Session
        description: The session
        type: string
      - in: query
        name: UserPoolId
        description: The ID of the Amazon Cognito user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Authentication Challenge
  /?Action=AdminSetUserSettings:
    get:
      summary: Admin Set User Settings
      description: Sets all the user settings for a specified user name.
      operationId: adminSetUserSettings
      x-api-path-slug: actionadminsetusersettings-get
      parameters:
      - in: query
        name: MFAOptions
        description: Specifies the options for MFA (e
        type: string
      - in: query
        name: Username
        description: The user name of the user for whom you wish to set user settings
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to set the
          users settings, such            as MFA options
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminUpdateDeviceStatus:
    get:
      summary: Admin Update Device Status
      description: Updates the device status as an administrator.
      operationId: adminUpdateDeviceStatus
      x-api-path-slug: actionadminupdatedevicestatus-get
      parameters:
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      - in: query
        name: DeviceRememberedStatus
        description: The status indicating whether a device has been remembered or
          not
        type: string
      - in: query
        name: Username
        description: The user name
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID&gt;
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminUpdateUserAttributes:
    get:
      summary: Admin Update User Attributes
      description: |-
        Updates the specified user's attributes, including developer attributes, as an
                    administrator.
      operationId: adminUpdateUserAttributes
      x-api-path-slug: actionadminupdateuserattributes-get
      parameters:
      - in: query
        name: UserAttributes
        description: An array of name-value pairs representing user attributes
        type: string
      - in: query
        name: Username
        description: The user name of the user for whom you want to update user attributes
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to update user            attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminUserGlobalSignOut:
    get:
      summary: Admin User Global Sign Out
      description: Signs out users from all devices, as an administrator.
      operationId: adminUserGlobalSignOut
      x-api-path-slug: actionadminuserglobalsignout-get
      parameters:
      - in: query
        name: Username
        description: The user name
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Global Sign Out
  /?Action=ChangePassword:
    get:
      summary: Change Password
      description: Changes the password for a specified user in a user pool.
      operationId: changePassword
      x-api-path-slug: actionchangepassword-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token in the change password request
        type: string
      - in: query
        name: PreviousPassword
        description: The old password in the change password request
        type: string
      - in: query
        name: ProposedPassword
        description: The new password in the change password request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Password
  /?Action=ConfirmDevice:
    get:
      summary: Confirm Device
      description: Confirms tracking of the device.
      operationId: confirmDevice
      x-api-path-slug: actionconfirmdevice-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token
        type: string
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      - in: query
        name: DeviceName
        description: The device name
        type: string
      - in: query
        name: DeviceSecretVerifierConfig
        description: The configuration of the device secret verifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Devices
  /?Action=ConfirmForgotPassword:
    get:
      summary: Confirm Forgot Password
      description: |-
        Allows a user to enter a code provided when they reset their password to update
                    their password.
      operationId: confirmForgotPassword
      x-api-path-slug: actionconfirmforgotpassword-get
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: ConfirmationCode
        description: The confirmation code sent by a users request to retrieve a forgotten            password
        type: string
      - in: query
        name: Password
        description: The password sent by sent by a users request to retrieve a forgotten            password
        type: string
      - in: query
        name: SecretHash
        description: A keyed-hash message authentication code (HMAC) calculated using
          the secret key of            a user pool client and username plus the client
          ID in the message
        type: string
      - in: query
        name: Username
        description: The user name of the user for whom you want to enter a code to
          retrieve a forgotten            password
        type: string
      responses:
        200:
          description: OK
      tags:
      - Passwords
  /?Action=ConfirmSignUp:
    get:
      summary: Confirm Sign Up
      description: |-
        Confirms registration of a user and handles the existing alias from a previous
                    user.
      operationId: confirmSignUp
      x-api-path-slug: actionconfirmsignup-get
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: ConfirmationCode
        description: The confirmation code sent by a users request to confirm registration
        type: string
      - in: query
        name: ForceAliasCreation
        description: Boolean to be specified to force user confirmation irrespective
          of existing alias
        type: string
      - in: query
        name: SecretHash
        description: A keyed-hash message authentication code (HMAC) calculated using
          the secret key of            a user pool client and username plus the client
          ID in the message
        type: string
      - in: query
        name: Username
        description: The user name of the user whose registration you wish to confirm
        type: string
      responses:
        200:
          description: OK
      tags:
      - Sign Ups
  /?Action=CreateGroup:
    get:
      summary: Create Group
      description: Creates a new group in the specified user pool.
      operationId: createGroup
      x-api-path-slug: actioncreategroup-get
      parameters:
      - in: query
        name: Description
        description: A string containing the description of the group
        type: string
      - in: query
        name: GroupName
        description: The name of the group
        type: string
      - in: query
        name: Precedence
        description: A nonnegative integer value that specifies the precedence of
          this group relative to            the other groups that a user can belong
          to in the user pool
        type: string
      - in: query
        name: RoleArn
        description: The role ARN for the group
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=CreateUserImportJob:
    get:
      summary: Create User Import Job
      description: Creates the user import job.
      operationId: createUserImportJob
      x-api-path-slug: actioncreateuserimportjob-get
      parameters:
      - in: query
        name: CloudWatchLogsRoleArn
        description: The role ARN for the Amazon CloudWatch Logging role for the user
          import            job
        type: string
      - in: query
        name: JobName
        description: The job name for the user import job
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are being imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Imports
  /?Action=CreateUserPool:
    get:
      summary: Create User Pool
      description: |-
        Creates a new Amazon Cognito user pool and sets the password policy for the
                    pool.
      operationId: createUserPool
      x-api-path-slug: actioncreateuserpool-get
      parameters:
      - in: query
        name: AdminCreateUserConfig
        description: The configuration for AdminCreateUser requests
        type: string
      - in: query
        name: AliasAttributes
        description: Attributes supported as an alias for this user pool
        type: string
      - in: query
        name: AutoVerifiedAttributes
        description: The attributes to be auto-verified
        type: string
      - in: query
        name: DeviceConfiguration
        description: The device configuration
        type: string
      - in: query
        name: EmailConfiguration
        description: The email configuration
        type: string
      - in: query
        name: EmailVerificationMessage
        description: A string representing the email verification message
        type: string
      - in: query
        name: EmailVerificationSubject
        description: A string representing the email verification subject
        type: string
      - in: query
        name: LambdaConfig
        description: The Lambda trigger configuration information for the new user
          pool
        type: string
      - in: query
        name: MfaConfiguration
        description: Specifies MFA configuration details
        type: string
      - in: query
        name: Policies
        description: The policies associated with the new user pool
        type: string
      - in: query
        name: PoolName
        description: A string used to name the user pool
        type: string
      - in: query
        name: Schema
        description: An array of schema attributes for the new user pool
        type: string
      - in: query
        name: SmsAuthenticationMessage
        description: A string representing the SMS authentication message
        type: string
      - in: query
        name: SmsConfiguration
        description: The SMS configuration
        type: string
      - in: query
        name: SmsVerificationMessage
        description: A string representing the SMS verification message
        type: string
      - in: query
        name: UserPoolTags
        description: The cost allocation tags for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pools
  /?Action=CreateUserPoolClient:
    get:
      summary: Create User Pool Client
      description: Creates the user pool client.
      operationId: createUserPoolClient
      x-api-path-slug: actioncreateuserpoolclient-get
      parameters:
      - in: query
        name: ClientName
        description: The client name for the user pool client you would like to create
        type: string
      - in: query
        name: ExplicitAuthFlows
        description: The explicit authentication flows
        type: string
      - in: query
        name: GenerateSecret
        description: Boolean to specify whether you want to generate a secret for
          the user pool client            being created
        type: string
      - in: query
        name: ReadAttributes
        description: The read attributes
        type: string
      - in: query
        name: RefreshTokenValidity
        description: The validity of the refresh token, in days
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to create a
          user pool            client
        type: string
      - in: query
        name: WriteAttributes
        description: The write attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pool Clients
  /?Action=DeleteGroup:
    get:
      summary: Delete Group
      description: Deletes a group.
      operationId: deleteGroup
      x-api-path-slug: actiondeletegroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=DeleteUser:
    get:
      summary: Delete User
      description: Allows a user to delete one's self.
      operationId: deleteUser
      x-api-path-slug: actiondeleteuser-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token from a request to delete a user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=DeleteUserAttributes:
    get:
      summary: Delete User Attributes
      description: Deletes the attributes for a user.
      operationId: deleteUserAttributes
      x-api-path-slug: actiondeleteuserattributes-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token used in the request to delete user attributes
        type: string
      - in: query
        name: UserAttributeNames
        description: An array of strings representing the user attribute names you
          wish to            delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=DeleteUserPool:
    get:
      summary: Delete User Pool
      description: Deletes the specified Amazon Cognito user pool.
      operationId: deleteUserPool
      x-api-path-slug: actiondeleteuserpool-get
      parameters:
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pools
  /?Action=DeleteUserPoolClient:
    get:
      summary: Delete User Pool Client
      description: Allows the developer to delete the user pool client.
      operationId: deleteUserPoolClient
      x-api-path-slug: actiondeleteuserpoolclient-get
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to delete the
          client
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pools
  /?Action=DescribeUserImportJob:
    get:
      summary: Describe User Import Job
      description: Describes the user import job.
      operationId: describeUserImportJob
      x-api-path-slug: actiondescribeuserimportjob-get
      parameters:
      - in: query
        name: JobId
        description: The job ID for the user import job
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are being imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Imports
  /?Action=DescribeUserPool:
    get:
      summary: Describe User Pool
      description: |-
        Returns the configuration information and metadata of the specified user
                    pool.
      operationId: describeUserPool
      x-api-path-slug: actiondescribeuserpool-get
      parameters:
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pools
  /?Action=DescribeUserPoolClient:
    get:
      summary: Describe User Pool Client
      description: |-
        Client method for returning the configuration information and metadata of the
                    specified user pool client.
      operationId: describeUserPoolClient
      x-api-path-slug: actiondescribeuserpoolclient-get
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pool Clients
  /?Action=ForgetDevice:
    get:
      summary: Forget Device
      description: Forgets the specified device.
      operationId: forgetDevice
      x-api-path-slug: actionforgetdevice-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token for the forgotten device request
        type: string
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Devices
  /?Action=ForgotPassword:
    get:
      summary: Forgot Password
      description: Retrieves the password for the specified client ID or username.
      operationId: forgotPassword
      x-api-path-slug: actionforgotpassword-get
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: SecretHash
        description: A keyed-hash message authentication code (HMAC) calculated using
          the secret key of            a user pool client and username plus the client
          ID in the message
        type: string
      - in: query
        name: Username
        description: The user name of the user for whom you want to enter a code to
          reset a forgotten            password
        type: string
      responses:
        200:
          description: OK
      tags:
      - Passwords
  /?Action=GetCSVHeader:
    get:
      summary: Get C S V Header
      description: Gets the header information for the.
      operationId: getCSVHeader
      x-api-path-slug: actiongetcsvheader-get
      parameters:
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are to be imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - CSV Header
  /?Action=GetDevice:
    get:
      summary: Get Device
      description: Gets the device.
      operationId: getDevice
      x-api-path-slug: actiongetdevice-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token
        type: string
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pools
  /?Action=GetGroup:
    get:
      summary: Get Group
      description: Gets a group.
      operationId: getGroup
      x-api-path-slug: actiongetgroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=GetUser:
    get:
      summary: Get User
      description: Gets the user attributes and metadata for a user.
      operationId: getUser
      x-api-path-slug: actiongetuser-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token returned by the server response to get information
          about the            user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=GetUserAttributeVerificationCode:
    get:
      summary: Get User Attribute Verification Code
      description: |-
        Gets the user attribute verification code for the specified attribute
                    name.
      operationId: getUserAttributeVerificationCode
      x-api-path-slug: actiongetuserattributeverificationcode-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token returned by the server response to get the user
          attribute            verification code
        type: string
      - in: query
        name: AttributeName
        description: The attribute name returned by the server response to get the
          user attribute            verification code
        type: string
      responses:
        200:
          description: OK
      tags:
      - Verification Codes
  /?Action=GlobalSignOut:
    get:
      summary: Global Sign Out
      description: Signs out users from all devices.
      operationId: globalSignOut
      x-api-path-slug: actionglobalsignout-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token
        type: string
      responses:
        200:
          description: OK
      tags:
      - Sign Out
  /?Action=InitiateAuth:
    get:
      summary: Initiate Auth
      description: Initiates the authentication flow.
      operationId: initiateAuth
      x-api-path-slug: actioninitiateauth-get
      parameters:
      - in: query
        name: AuthFlow
        description: The authentication flow
        type: string
      - in: query
        name: AuthParameters
        description: The authentication parameters
        type: string
      - in: query
        name: ClientId
        description: The client ID
        type: string
      - in: query
        name: ClientMetadata
        description: The client apps metadata
        type: string
      responses:
        200:
          description: OK
      tags:
      - Authentication
  /?Action=ListDevices:
    get:
      summary: List Devices
      description: Lists the devices.
      operationId: listDevices
      x-api-path-slug: actionlistdevices-get
      parameters:
      - in: query
        name: AccessToken
        description: The access tokens for the request to list devices
        type: string
      - in: query
        name: Limit
        description: The limit of the device request
        type: string
      - in: query
        name: PaginationToken
        description: The pagination token for the list request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Devices
  /?Action=ListGroups:
    get:
      summary: List Groups
      description: Lists the groups associated with a user pool.
      operationId: listGroups
      x-api-path-slug: actionlistgroups-get
      parameters:
      - in: query
        name: Limit
        description: The limit of the request to list groups
        type: string
      - in: query
        name: NextToken
        description: An identifier that was returned from the previous call to this
          operation, which can            be used to return the next set of items
          in the list
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=ListUserImportJobs:
    get:
      summary: List User Import Jobs
      description: Lists the user import jobs.
      operationId: listUserImportJobs
      x-api-path-slug: actionlistuserimportjobs-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of import jobs you want the request to return
        type: string
      - in: query
        name: PaginationToken
        description: An identifier that was returned from the previous call to ListUserImportJobs,
          which            can be used to return the next set of import jobs in the
          list
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are being imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Imports
  /?Action=ListUserPoolClients:
    get:
      summary: List User Pool Clients
      description: Lists the clients that have been created for the specified user
        pool.
      operationId: listUserPoolClients
      x-api-path-slug: actionlistuserpoolclients-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of results you want the request to return
          when listing the user            pool clients
        type: string
      - in: query
        name: NextToken
        description: An identifier that was returned from the previous call to this
          operation, which can            be used to return the next set of items
          in the list
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to list user
          pool            clients
        type: string
      responses:
        200:
          description: OK
      tags:
      - user Pool Clients
  /?Action=ListUserPools:
    get:
      summary: List User Pools
      description: Lists the user pools associated with an AWS account.
      operationId: listUserPools
      x-api-path-slug: actionlistuserpools-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of results you want the request to return
          when listing the user            pools
        type: string
      - in: query
        name: NextToken
        description: An identifier that was returned from the previous call to this
          operation, which can            be used to return the next set of items
          in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - user Pools
  /?Action=ListUsers:
    get:
      summary: List Users
      description: Lists the users in the Amazon Cognito user pool.
      operationId: listUsers
      x-api-path-slug: actionlistusers-get
      parameters:
      - in: query
        name: AttributesToGet
        description: The attributes to get from the request to list users
        type: string
      - in: query
        name: Filter
        description: The filter for the list users request
        type: string
      - in: query
        name: Limit
        description: The limit of the request to list users
        type: string
      - in: query
        name: PaginationToken
        description: An identifier that was returned from the previous call to this
          operation, which can            be used to return the next set of items
          in the list
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for which you want to list users
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=ListUsersInGroup:
    get:
      summary: List Users In Group
      description: Lists the users in the specified group.
      operationId: listUsersInGroup
      x-api-path-slug: actionlistusersingroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group
        type: string
      - in: query
        name: Limit
        description: The limit of the request to list users
        type: string
      - in: query
        name: NextToken
        description: An identifier that was returned from the previous call to this
          operation, which can            be used to return the next set of items
          in the list
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /?Action=ResendConfirmationCode:
    get:
      summary: Resend Confirmation Code
      description: |-
        Resends the confirmation (for confirmation of registration) to a specific user in
                    the user pool.
      operationId: resendConfirmationCode
      x-api-path-slug: actionresendconfirmationcode-get
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: SecretHash
        description: A keyed-hash message authentication code (HMAC) calculated using
          the secret key of            a user pool client and username plus the client
          ID in the message
        type: string
      - in: query
        name: Username
        description: The user name of the user to whom you wish to resend a confirmation
          code
        type: string
      responses:
        200:
          description: OK
      tags:
      - Confirmation Code
  /?Action=RespondToAuthChallenge:
    get:
      summary: Respond To Auth Challenge
      description: Responds to the authentication challenge.
      operationId: respondToAuthChallenge
      x-api-path-slug: actionrespondtoauthchallenge-get
      parameters:
      - in: query
        name: ChallengeName
        description: The name of the challenge
        type: string
      - in: query
        name: ChallengeResponses
        description: The responses to the authentication challenge
        type: string
      - in: query
        name: ClientId
        description: The client ID
        type: string
      - in: query
        name: Session
        description: The session
        type: string
      responses:
        200:
          description: OK
      tags:
      - Authentication Challenges
  /?Action=SetUserSettings:
    get:
      summary: Set User Settings
      description: Sets the user settings like multi-factor authentication (MFA).
      operationId: setUserSettings
      x-api-path-slug: actionsetusersettings-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token for the set user settings request
        type: string
      - in: query
        name: MFAOptions
        description: Specifies the options for MFA (e
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=SignUp:
    get:
      summary: Sign Up
      description: |-
        Registers the user in the specified user pool and creates a user name, password,
                    and user attributes.
      operationId: signUp
      x-api-path-slug: actionsignup-get
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: Password
        description: The password of the user you wish to register
        type: string
      - in: query
        name: SecretHash
        description: A keyed-hash message authentication code (HMAC) calculated using
          the secret key of            a user pool client and username plus the client
          ID in the message
        type: string
      - in: query
        name: UserAttributes
        description: An array of name-value pairs representing user attributes
        type: string
      - in: query
        name: Username
        description: The user name of the user you wish to register
        type: string
      - in: query
        name: ValidationData
        description: The validation data in the request to register a user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Sign Up
  /?Action=StartUserImportJob:
    get:
      summary: Start User Import Job
      description: Starts the user import.
      operationId: startUserImportJob
      x-api-path-slug: actionstartuserimportjob-get
      parameters:
      - in: query
        name: JobId
        description: The job ID for the user import job
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are being imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Imports
  /?Action=StopUserImportJob:
    get:
      summary: Stop User Import Job
      description: Stops the user import job.
      operationId: stopUserImportJob
      x-api-path-slug: actionstopuserimportjob-get
      parameters:
      - in: query
        name: JobId
        description: The job ID for the user import job
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are being imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Iimport
  /?Action=UpdateDeviceStatus:
    get:
      summary: Update Device Status
      description: Updates the device status.
      operationId: updateDeviceStatus
      x-api-path-slug: actionupdatedevicestatus-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token
        type: string
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      - in: query
        name: DeviceRememberedStatus
        description: The status of whether a device is remembered
        type: string
      responses:
        200:
          description: OK
      tags:
      - Devices
  /?Action=UpdateGroup:
    get:
      summary: Update Group
      description: Updates the specified group with the specified attributes.
      operationId: updateGroup
      x-api-path-slug: actionupdategroup-get
      parameters:
      - in: query
        name: Description
        description: A string containing the new description of the group
        type: string
      - in: query
        name: GroupName
        description: The name of the group
        type: string
      - in: query
        name: Precedence
        description: The new precedence value for the group
        type: string
      - in: query
        name: RoleArn
        description: The new role ARN for the group
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=UpdateUserAttributes:
    get:
      summary: Update User Attributes
      description: Allows a user to update a specific attribute (one at a time).
      operationId: updateUserAttributes
      x-api-path-slug: actionupdateuserattributes-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token for the request to update user attributes
        type: string
      - in: query
        name: UserAttributes
        description: An array of name-value pairs representing user attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=UpdateUserPool:
    get:
      summary: Update User Pool
      description: Updates the specified user pool with the specified attributes.
      operationId: updateUserPool
      x-api-path-slug: actionupdateuserpool-get
      parameters:
      - in: query
        name: AdminCreateUserConfig
        description: The configuration for AdminCreateUser requests
        type: string
      - in: query
        name: AutoVerifiedAttributes
        description: The attributes that are automatically verified when the Amazon
          Cognito service            makes a request to update user pools
        type: string
      - in: query
        name: DeviceConfiguration
        description: Device configuration
        type: string
      - in: query
        name: EmailConfiguration
        description: Email configuration
        type: string
      - in: query
        name: EmailVerificationMessage
        description: The contents of the email verification message
        type: string
      - in: query
        name: EmailVerificationSubject
        description: The subject of the email verification message
        type: string
      - in: query
        name: LambdaConfig
        description: The AWS Lambda configuration information from the request to
          update the user            pool
        type: string
      - in: query
        name: MfaConfiguration
        description: 'Can be one of the following values:'
        type: string
      - in: query
        name: Policies
        description: A container with the policies you wish to update in a user pool
        type: string
      - in: query
        name: SmsAuthenticationMessage
        description: The contents of the SMS authentication message
        type: string
      - in: query
        name: SmsConfiguration
        description: SMS configuration
        type: string
      - in: query
        name: SmsVerificationMessage
        description: A container with information about the SMS verification message
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool you want to update
        type: string
      - in: query
        name: UserPoolTags
        description: The cost allocation tags for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pools
  /?Action=UpdateUserPoolClient:
    get:
      summary: Update User Pool Client
      description: |-
        Allows the developer to update the specified user pool client and password
                    policy.
      operationId: updateUserPoolClient
      x-api-path-slug: actionupdateuserpoolclient-get
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: ClientName
        description: The client name from the update user pool client request
        type: string
      - in: query
        name: ExplicitAuthFlows
        description: Explicit authentication flows
        type: string
      - in: query
        name: ReadAttributes
        description: The read-only attributes of the user pool
        type: string
      - in: query
        name: RefreshTokenValidity
        description: The validity of the refresh token, in days
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to update the
          user pool            client
        type: string
      - in: query
        name: WriteAttributes
        description: The writeable attributes of the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pool Clients
  /?Action=VerifyUserAttribute:
    get:
      summary: Verify User Attribute
      description: Verifies the specified user attributes in the user pool.
      operationId: verifyUserAttribute
      x-api-path-slug: actionverifyuserattribute-get
      parameters:
      - in: query
        name: AccessToken
        description: Represents the access token of the request to verify user attributes
        type: string
      - in: query
        name: AttributeName
        description: The attribute name in the request to verify user attributes
        type: string
      - in: query
        name: Code
        description: The verification code in the request to verify user attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=CreateIdentityPool:
    get:
      summary: Create Identity Pool
      description: Creates a new identity pool.
      operationId: createIdentityPool
      x-api-path-slug: actioncreateidentitypool-get
      parameters:
      - in: query
        name: AllowUnauthenticatedIdentities
        description: TRUE if the identity pool supports unauthenticated logins
        type: string
      - in: query
        name: CognitoIdentityProviders
        description: An array of Amazon Cognito Identity user pools and their client
          IDs
        type: string
      - in: query
        name: DeveloperProviderName
        description: The domain by which Cognito will refer to your users
        type: string
      - in: query
        name: IdentityPoolName
        description: A string that you provide
        type: string
      - in: query
        name: OpenIdConnectProviderARNs
        description: A list of OpendID Connect provider ARNs
        type: string
      - in: query
        name: SamlProviderARNs
        description: An array of Amazon Resource Names (ARNs) of the SAML provider
          for your identity         pool
        type: string
      - in: query
        name: SupportedLoginProviders
        description: Optional key:value pairs mapping provider names to provider app
          IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pool
  /?Action=DeleteIdentities:
    get:
      summary: Delete Identities
      description: Deletes identities from an identity pool.
      operationId: deleteIdentities
      x-api-path-slug: actiondeleteidentities-get
      parameters:
      - in: query
        name: IdentityIdsToDelete
        description: A list of 1-60 identities that you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identities
  /?Action=DeleteIdentityPool:
    get:
      summary: Delete Identity Pool
      description: Deletes a user pool.
      operationId: deleteIdentityPool
      x-api-path-slug: actiondeleteidentitypool-get
      parameters:
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pool
  /?Action=DescribeIdentity:
    get:
      summary: Describe Identity
      description: |-
        Returns metadata related to the given identity, including when the identity was
                 created and any associated linked logins.
      operationId: describeIdentity
      x-api-path-slug: actiondescribeidentity-get
      parameters:
      - in: query
        name: IdentityId
        description: A unique identifier in the format REGION:GUID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identities
  /?Action=DescribeIdentityPool:
    get:
      summary: Describe Identity Pool
      description: |-
        Gets details about a particular identity pool, including the pool name, ID
                 description, creation date, and current number of users.
      operationId: describeIdentityPool
      x-api-path-slug: actiondescribeidentitypool-get
      parameters:
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pool
  /?Action=GetCredentialsForIdentity:
    get:
      summary: Get Credentials For Identity
      description: Returns credentials for the provided identity ID.
      operationId: getCredentialsForIdentity
      x-api-path-slug: actiongetcredentialsforidentity-get
      parameters:
      - in: query
        name: CustomRoleArn
        description: The Amazon Resource Name (ARN) of the role to be assumed when
          multiple roles were         received in the token from the identity provider
        type: string
      - in: query
        name: IdentityId
        description: A unique identifier in the format REGION:GUID
        type: string
      - in: query
        name: Logins
        description: A set of optional name-value pairs that map provider names to
          provider         tokens
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identities
  /?Action=GetId:
    get:
      summary: Get Id
      description: Generates (or retrieves) a Cognito ID.
      operationId: getId
      x-api-path-slug: actiongetid-get
      parameters:
      - in: query
        name: AccountId
        description: A standard AWS account ID (9+ digits)
        type: string
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      - in: query
        name: Logins
        description: A set of optional name-value pairs that map provider names to
          provider tokens
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identities
  /?Action=GetIdentityPoolRoles:
    get:
      summary: Get Identity Pool Roles
      description: Gets the roles for an identity pool.
      operationId: getIdentityPoolRoles
      x-api-path-slug: actiongetidentitypoolroles-get
      parameters:
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pool Roles
  /?Action=GetOpenIdToken:
    get:
      summary: Get Open Id Token
      description: Gets an OpenID token, using a known Cognito ID.
      operationId: getOpenIdToken
      x-api-path-slug: actiongetopenidtoken-get
      parameters:
      - in: query
        name: IdentityId
        description: A unique identifier in the format REGION:GUID
        type: string
      - in: query
        name: Logins
        description: A set of optional name-value pairs that map provider names to
          provider tokens
        type: string
      responses:
        200:
          description: OK
      tags:
      - Open ID Token
  /?Action=GetOpenIdTokenForDeveloperIdentity:
    get:
      summary: Get Open Id Token For Developer Identity
      description: |-
        Registers (or retrieves) a Cognito IdentityId and an OpenID Connect
                 token for a user authenticated by your backend authentication process.
      operationId: getOpenIdTokenForDeveloperIdentity
      x-api-path-slug: actiongetopenidtokenfordeveloperidentity-get
      parameters:
      - in: query
        name: IdentityId
        description: A unique identifier in the format REGION:GUID
        type: string
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      - in: query
        name: Logins
        description: A set of optional name-value pairs that map provider names to
          provider tokens
        type: string
      - in: query
        name: TokenDuration
        description: The expiration time of the token, in seconds
        type: string
      responses:
        200:
          description: OK
      tags:
      - Open ID Token for Developer Identities
  /?Action=ListIdentities:
    get:
      summary: List Identities
      description: Lists the identities in a pool.
      operationId: listIdentities
      x-api-path-slug: actionlistidentities-get
      parameters:
      - in: query
        name: HideDisabled
        description: An optional boolean parameter that allows you to hide disabled
          identities
        type: string
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of identities to return
        type: string
      - in: query
        name: NextToken
        description: A pagination token
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identities
  /?Action=ListIdentityPools:
    get:
      summary: List Identity Pools
      description: Lists all of the Cognito identity pools registered for your account.
      operationId: listIdentityPools
      x-api-path-slug: actionlistidentitypools-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of identities to return
        type: string
      - in: query
        name: NextToken
        description: A pagination token
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pool
  /?Action=LookupDeveloperIdentity:
    get:
      summary: Lookup Developer Identity
      description: |-
        Retrieves the IdentityID associated with a
                    DeveloperUserIdentifier or the list of
                 DeveloperUserIdentifiers associated with an IdentityId for an
                 existing identity.
      operationId: lookupDeveloperIdentity
      x-api-path-slug: actionlookupdeveloperidentity-get
      parameters:
      - in: query
        name: DeveloperUserIdentifier
        description: A unique ID used by your backend authentication process to identify
          a user
        type: string
      - in: query
        name: IdentityId
        description: A unique identifier in the format REGION:GUID
        type: string
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of identities to return
        type: string
      - in: query
        name: NextToken
        description: A pagination token
        type: string
      responses:
        200:
          description: OK
      tags:
      - Developer Identities
  /?Action=MergeDeveloperIdentities:
    get:
      summary: Merge Developer Identities
      description: |-
        Merges two users having different IdentityIds, existing in the same
                 identity pool, and identified by the same developer provider.
      operationId: mergeDeveloperIdentities
      x-api-path-slug: actionmergedeveloperidentities-get
      parameters:
      - in: query
        name: DestinationUserIdentifier
        description: User identifier for the destination user
        type: string
      - in: query
        name: DeveloperProviderName
        description: The domain by which Cognito will refer to your users
        type: string
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      - in: query
        name: SourceUserIdentifier
        description: User identifier for the source user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Developer Identities
  /?Action=SetIdentityPoolRoles:
    get:
      summary: Set Identity Pool Roles
      description: Sets the roles for an identity pool.
      operationId: setIdentityPoolRoles
      x-api-path-slug: actionsetidentitypoolroles-get
      parameters:
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      - in: query
        name: RoleMappings
        description: How users for a specific identity provider are to mapped to roles
        type: string
      - in: query
        name: Roles
        description: The map of roles associated with this pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pool
  /?Action=UnlinkDeveloperIdentity:
    get:
      summary: Unlink Developer Identity
      description: Unlinks a DeveloperUserIdentifier from an existing identity.
      operationId: unlinkDeveloperIdentity
      x-api-path-slug: actionunlinkdeveloperidentity-get
      parameters:
      - in: query
        name: DeveloperProviderName
        description: The domain by which Cognito will refer to your users
        type: string
      - in: query
        name: DeveloperUserIdentifier
        description: A unique ID used by your backend authentication process to identify
          a user
        type: string
      - in: query
        name: IdentityId
        description: A unique identifier in the format REGION:GUID
        type: string
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Developer Identities
  /?Action=UnlinkIdentity:
    get:
      summary: Unlink Identity
      description: Unlinks a federated identity from an existing account.
      operationId: unlinkIdentity
      x-api-path-slug: actionunlinkidentity-get
      parameters:
      - in: query
        name: IdentityId
        description: A unique identifier in the format REGION:GUID
        type: string
      - in: query
        name: Logins
        description: A set of optional name-value pairs that map provider names to
          provider         tokens
        type: string
      - in: query
        name: LoginsToRemove
        description: Provider names to unlink from this identity
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identities
  /?Action=UpdateIdentityPool:
    get:
      summary: Update Identity Pool
      description: Updates a user pool.
      operationId: updateIdentityPool
      x-api-path-slug: actionupdateidentitypool-get
      parameters:
      - in: query
        name: AllowUnauthenticatedIdentities
        description: TRUE if the identity pool supports unauthenticated logins
        type: string
      - in: query
        name: CognitoIdentityProviders
        description: A list representing an Amazon Cognito Identity User Pool and
          its client ID
        type: string
      - in: query
        name: DeveloperProviderName
        description: The domain by which Cognito will refer to your users
        type: string
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      - in: query
        name: IdentityPoolName
        description: A string that you provide
        type: string
      - in: query
        name: OpenIdConnectProviderARNs
        description: A list of OpendID Connect provider ARNs
        type: string
      - in: query
        name: SamlProviderARNs
        description: An array of Amazon Resource Names (ARNs) of the SAML provider
          for your identity         pool
        type: string
      - in: query
        name: SupportedLoginProviders
        description: Optional key:value pairs mapping provider names to provider app
          IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pool
  /?Action=BulkPublish:
    get:
      summary: Bulk Publish
      description: Initiates a bulk publish of all existing datasets for an Identity
        Pool to the configured stream.
      operationId: bulkPublish
      x-api-path-slug: actionbulkpublish-get
      parameters:
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Publish
  /?Action=DeleteDataset:
    get:
      summary: Delete Dataset
      description: Deletes the specific dataset.
      operationId: deleteDataset
      x-api-path-slug: actiondeletedataset-get
      parameters:
      - in: query
        name: DatasetName
        description: A string of up to 128 characters
        type: string
      - in: query
        name: IdentityId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)       created
          by Amazon Cognito
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)       created
          by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Dataset
  /?Action=DescribeDataset:
    get:
      summary: Describe Dataset
      description: Gets meta data about a dataset by identity and dataset name.
      operationId: describeDataset
      x-api-path-slug: actiondescribedataset-get
      parameters:
      - in: query
        name: DatasetName
        description: A string of up to 128 characters
        type: string
      - in: query
        name: IdentityId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)       created
          by Amazon Cognito
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)       created
          by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Dataset
  /?Action=DescribeIdentityPoolUsage:
    get:
      summary: Describe Identity Pool Usage
      description: Gets usage details (for example, data storage) about a particular
        identity pool.
      operationId: describeIdentityPoolUsage
      x-api-path-slug: actiondescribeidentitypoolusage-get
      parameters:
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)       created
          by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pool Usage
  /?Action=DescribeIdentityUsage:
    get:
      summary: Describe Identity Usage
      description: Gets usage information for an identity, including number of datasets
        and data usage.
      operationId: describeIdentityUsage
      x-api-path-slug: actiondescribeidentityusage-get
      parameters:
      - in: query
        name: IdentityId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)       created
          by Amazon Cognito
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)       created
          by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pool Usage
  /?Action=GetBulkPublishDetails:
    get:
      summary: Get Bulk Publish Details
      description: Get the status of the last BulkPublish operation for an identity
        pool.
      operationId: getBulkPublishDetails
      x-api-path-slug: actiongetbulkpublishdetails-get
      parameters:
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Publish
  /?Action=GetCognitoEvents:
    get:
      summary: Get Cognito Events
      description: Gets the events and the corresponding Lambda functions associated
        with an identity pool.
      operationId: getCognitoEvents
      x-api-path-slug: actiongetcognitoevents-get
      parameters:
      - in: query
        name: IdentityPoolId
        description: The Cognito Identity Pool ID for the request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
  /?Action=GetIdentityPoolConfiguration:
    get:
      summary: Get Identity Pool Configuration
      description: Gets the configuration settings of an identity pool.
      operationId: getIdentityPoolConfiguration
      x-api-path-slug: actiongetidentitypoolconfiguration-get
      parameters:
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pools
  /?Action=ListDatasets:
    get:
      summary: List Datasets
      description: Lists datasets for an identity.
      operationId: listDatasets
      x-api-path-slug: actionlistdatasets-get
      parameters:
      - in: query
        name: IdentityId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to be returned
        type: string
      - in: query
        name: NextToken
        description: A pagination token for obtaining the next page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Dataset
  /?Action=ListIdentityPoolUsage:
    get:
      summary: List Identity Pool Usage
      description: Gets a list of identity pools registered with Cognito.
      operationId: listIdentityPoolUsage
      x-api-path-slug: actionlistidentitypoolusage-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of results to be returned
        type: string
      - in: query
        name: NextToken
        description: A pagination token for obtaining the next page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pools
  /?Action=ListRecords:
    get:
      summary: List Records
      description: Gets paginated records, optionally changed after a particular sync
        count for a dataset and identity.
      operationId: listRecords
      x-api-path-slug: actionlistrecords-get
      parameters:
      - in: query
        name: DatasetName
        description: A string of up to 128 characters
        type: string
      - in: query
        name: IdentityId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      - in: query
        name: LastSyncCount
        description: The last server sync count for this record
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to be returned
        type: string
      - in: query
        name: NextToken
        description: A pagination token for obtaining the next page of results
        type: string
      - in: query
        name: SyncSessionToken
        description: A token containing a session ID, identity ID, and expiration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Records
  /?Action=RegisterDevice:
    get:
      summary: Register Device
      description: Registers a device to receive push sync notifications.
      operationId: registerDevice
      x-api-path-slug: actionregisterdevice-get
      parameters:
      - in: query
        name: IdentityId
        description: The unique ID for this identity
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Devices
  /?Action=SetCognitoEvents:
    get:
      summary: Set Cognito Events
      description: Sets the AWS Lambda function for a given event type for an identity
        pool.
      operationId: setCognitoEvents
      x-api-path-slug: actionsetcognitoevents-get
      parameters:
      - in: query
        name: IdentityPoolId
        description: The Cognito Identity Pool to use when configuring Cognito Events
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
  /?Action=SetIdentityPoolConfiguration:
    get:
      summary: Set Identity Pool Configuration
      description: Sets the necessary configuration for push sync.
      operationId: setIdentityPoolConfiguration
      x-api-path-slug: actionsetidentitypoolconfiguration-get
      parameters:
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Identity Pools
  /?Action=SubscribeToDataset:
    get:
      summary: Subscribe To Dataset
      description: Subscribes to receive notifications when a dataset is modified
        by another device.
      operationId: subscribeToDataset
      x-api-path-slug: actionsubscribetodataset-get
      parameters:
      - in: query
        name: DatasetName
        description: The name of the dataset to subcribe to
        type: string
      - in: query
        name: DeviceId
        description: The unique ID generated for this device by Cognito
        type: string
      - in: query
        name: IdentityId
        description: Unique ID for this identity
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Dataset
  /?Action=UnsubscribeFromDataset:
    get:
      summary: Unsubscribe From Dataset
      description: Unsubscribes from receiving notifications when a dataset is modified
        by another device.
      operationId: unsubscribeFromDataset
      x-api-path-slug: actionunsubscribefromdataset-get
      parameters:
      - in: query
        name: DatasetName
        description: The name of the dataset from which to unsubcribe
        type: string
      - in: query
        name: DeviceId
        description: The unique ID generated for this device by Cognito
        type: string
      - in: query
        name: IdentityId
        description: Unique ID for this identity
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Dataset
  /?Action=UpdateRecords:
    get:
      summary: Update Records
      description: Posts updates to records and adds and deletes records for a dataset
        and user.
      operationId: updateRecords
      x-api-path-slug: actionupdaterecords-get
      parameters:
      - in: query
        name: ClientContext
        description: Intended to supply a device ID that will populate the lastModifiedBy
          field referenced in other methods
        type: string
      - in: query
        name: DatasetName
        description: A string of up to 128 characters
        type: string
      - in: query
        name: IdentityId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Records