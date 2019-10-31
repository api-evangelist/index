swagger: "2.0"
x-collection-name: Google Cloud Billing
x-complete: 1
info:
  title: Google Cloud Billing
  description: allows-developers-to-manage-billing-for-their-google-cloud-platform-projects----programmatically-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: cloudbilling.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/billingAccounts:
    get:
      summary: Get Billing Accounts
      description: |-
        Lists the billing accounts that the current authenticated user
        [owns](https://support.google.com/cloud/answer/4430947).
      operationId: cloudbilling.billingAccounts.list
      x-api-path-slug: v1billingaccounts-get
      parameters:
      - in: query
        name: pageSize
        description: Requested page size
      - in: query
        name: pageToken
        description: A token identifying a page of results to return
      responses:
        200:
          description: OK
      tags:
      - Account
  /v1/{name}:
    get:
      summary: Get Billing Account
      description: |-
        Gets information about a billing account. The current authenticated user
        must be an [owner of the billing
        account](https://support.google.com/cloud/answer/4430947).
      operationId: cloudbilling.billingAccounts.get
      x-api-path-slug: v1name-get
      parameters:
      - in: path
        name: name
        description: The resource name of the billing account to retrieve
      responses:
        200:
          description: OK
      tags:
      - Account
  /v1/{name}/billingInfo:
    get:
      summary: Get Billing Information
      description: |-
        Gets the billing information for a project. The current authenticated user
        must have [permission to view the
        project](https://cloud.google.com/docs/permissions-overview#h.bgs0oxofvnoo
        ).
      operationId: cloudbilling.projects.getBillingInfo
      x-api-path-slug: v1namebillinginfo-get
      parameters:
      - in: path
        name: name
        description: The resource name of the project for which billing information
          isretrieved
      responses:
        200:
          description: OK
      tags:
      - Billing
    put:
      summary: Update Billing Information
      description: |-
        Sets or updates the billing account associated with a project. You specify
        the new billing account by setting the `billing_account_name` in the
        `ProjectBillingInfo` resource to the resource name of a billing account.
        Associating a project with an open billing account enables billing on the
        project and allows charges for resource usage. If the project already had a
        billing account, this method changes the billing account used for resource
        usage charges.

        *Note:* Incurred charges that have not yet been reported in the transaction
        history of the Google Cloud Console may be billed to the new billing
        account, even if the charge occurred before the new billing account was
        assigned to the project.

        The current authenticated user must have ownership privileges for both the
        [project](https://cloud.google.com/docs/permissions-overview#h.bgs0oxofvnoo
        ) and the [billing
        account](https://support.google.com/cloud/answer/4430947).

        You can disable billing on the project by setting the
        `billing_account_name` field to empty. This action disassociates the
        current billing account from the project. Any billable activity of your
        in-use services will stop, and your application could stop functioning as
        expected. Any unbilled charges to date will be billed to the previously
        associated account. The current authenticated user must be either an owner
        of the project or an owner of the billing account for the project.

        Note that associating a project with a *closed* billing account will have
        much the same effect as disabling billing on the project: any paid
        resources used by the project will be shut down. Thus, unless you wish to
        disable billing, you should always call this method with the name of an
        *open* billing account.
      operationId: cloudbilling.projects.updateBillingInfo
      x-api-path-slug: v1namebillinginfo-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: The resource name of the project associated with the billing
          informationthat you want to update
      responses:
        200:
          description: OK
      tags:
      - Billing
  /v1/{name}/projects:
    get:
      summary: Get Projects
      description: |-
        Lists the projects associated with a billing account. The current
        authenticated user must be an [owner of the billing
        account](https://support.google.com/cloud/answer/4430947).
      operationId: cloudbilling.billingAccounts.projects.list
      x-api-path-slug: v1nameprojects-get
      parameters:
      - in: path
        name: name
        description: The resource name of the billing account associated with the
          projects thatyou want to list
      - in: query
        name: pageSize
        description: Requested page size
      - in: query
        name: pageToken
        description: A token identifying a page of results to be returned
      responses:
        200:
          description: OK
      tags:
      - Project