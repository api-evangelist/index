swagger: "2.0"
x-collection-name: AWS Certificate Manager
x-complete: 1
info:
  title: AWS Certificate Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddTagsToCertificate:
    get:
      summary: Add Tags To Certificate
      description: Adds one or more tags to an ACM Certificate.
      operationId: AddTagsToCertificate
      x-api-path-slug: actionaddtagstocertificate-get
      parameters:
      - in: query
        name: CertificateArn
        description: String that contains the ARN of the ACM Certificate to which
          the tag is to be applied
        type: string
      - in: query
        name: Tags
        description: The key-value pair that defines the tag
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificate Tags
  /?Action=DeleteCertificate:
    get:
      summary: Delete Certificate
      description: Deletes an ACM Certificate and its associated private key.
      operationId: DeleteCertificate
      x-api-path-slug: actiondeletecertificate-get
      parameters:
      - in: query
        name: CertificateArn
        description: String that contains the ARN of the ACM Certificate to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=DescribeCertificate:
    get:
      summary: Describe Certificate
      description: Returns a list of the fields contained in the specified ACM Certificate.
      operationId: DescribeCertificate
      x-api-path-slug: actiondescribecertificate-get
      parameters:
      - in: query
        name: CertificateArn
        description: String that contains an ACM Certificate ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=GetCertificate:
    get:
      summary: Get Certificate
      description: |-
        Retrieves an ACM Certificate and certificate chain for the certificate specified by an
              ARN.
      operationId: GetCertificate
      x-api-path-slug: actiongetcertificate-get
      parameters:
      - in: query
        name: CertificateArn
        description: 'String that contains a certificate ARN in the following format:'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=ImportCertificate:
    get:
      summary: Import Certificate
      description: Imports an SSL/TLS certificate into AWS Certificate Manager (ACM)
        to use with.
      operationId: ImportCertificate
      x-api-path-slug: actionimportcertificate-get
      parameters:
      - in: query
        name: Certificate
        description: The certificate to import
        type: string
      - in: query
        name: CertificateArn
        description: The Amazon Resource Name        (ARN) of an imported certificate
          to replace
        type: string
      - in: query
        name: CertificateChain
        description: The certificate chain
        type: string
      - in: query
        name: PrivateKey
        description: The private key that matches the public key in the certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=ListCertificates:
    get:
      summary: List Certificates
      description: Retrieves a list of ACM Certificates and the domain name for each.
      operationId: ListCertificates
      x-api-path-slug: actionlistcertificates-get
      parameters:
      - in: query
        name: CertificateStatuses
        description: The status or statuses on which to filter the list of ACM Certificates
        type: string
      - in: query
        name: MaxItems
        description: Use this parameter when paginating results to specify the maximum
          number of items to      return in the response
        type: string
      - in: query
        name: NextToken
        description: Use this parameter only when paginating results and only in a
          subsequent request after      you receive a response with truncated results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=ListTagsForCertificate:
    get:
      summary: List Tags For Certificate
      description: Lists the tags that have been applied to the ACM Certificate.
      operationId: ListTagsForCertificate
      x-api-path-slug: actionlisttagsforcertificate-get
      parameters:
      - in: query
        name: CertificateArn
        description: String that contains the ARN of the ACM Certificate for which
          you want to list the      tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificate Tags
  /?Action=RemoveTagsFromCertificate:
    get:
      summary: Remove Tags From Certificate
      description: Remove one or more tags from an ACM Certificate.
      operationId: RemoveTagsFromCertificate
      x-api-path-slug: actionremovetagsfromcertificate-get
      parameters:
      - in: query
        name: CertificateArn
        description: String that contains the ARN of the ACM Certificate with one
          or more tags that you want      to remove
        type: string
      - in: query
        name: Tags
        description: The key-value pair that defines the tag to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificate Tags
  /?Action=RequestCertificate:
    get:
      summary: Request Certificate
      description: Requests an ACM Certificate for use with other AWS services.
      operationId: RequestCertificate
      x-api-path-slug: actionrequestcertificate-get
      parameters:
      - in: query
        name: DomainName
        description: Fully qualified domain name (FQDN), such as www
        type: string
      - in: query
        name: DomainValidationOptions
        description: The base validation domain that will act as the suffix of the
          email addresses that are      used to send the emails
        type: string
      - in: query
        name: IdempotencyToken
        description: Customer chosen string that can be used to distinguish between
          calls to        RequestCertificate
        type: string
      - in: query
        name: SubjectAlternativeNames
        description: Additional FQDNs to be included in the Subject Alternative Name
          extension of the ACM      Certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=ResendValidationEmail:
    get:
      summary: Resend Validation Email
      description: Resends the email that requests domain ownership validation.
      operationId: ResendValidationEmail
      x-api-path-slug: actionresendvalidationemail-get
      parameters:
      - in: query
        name: CertificateArn
        description: String that contains the ARN of the requested certificate
        type: string
      - in: query
        name: Domain
        description: The Fully Qualified Domain Name (FQDN) of the certificate that
          needs to be      validated
        type: string
      - in: query
        name: ValidationDomain
        description: The base validation domain that will act as the suffix of the
          email addresses that are      used to send the emails
        type: string
      responses:
        200:
          description: OK
      tags:
      - Validation Email