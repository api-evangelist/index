swagger: "2.0"
x-collection-name: Paylocity
x-complete: 1
info:
  title: Paylocity
  description: for-general-questions-and-support-of-the-api-contact-vendorrelationspaylocity-com-overviewpaylocity-web-services-api-is-an-externally-facing-restful-internet-protocol--the-paylocity-api-uses-http-verbs-and-a-restful-endpoint-structure--oauth-2-0-is-used-as-the-api-authorization-framework--request-and-response-payloads-are-formatted-as-json-paylocity-supports-v1-and-v2-versions-of-its-api-endpoints--v1-while-supported-wont-be-enhanced-with-additional-functionality--for-direct-link-to-v1-documentation-please-click-herehttpsdocs-paylocity-comweblinkguidespaylocity-web-services-apiv1paylocity-web-services-api-htm--for-additional-resources-regarding-v1v2-differences-and-conversion-path-please-contact-vendorrelationspaylocity-com--setuppaylocity-will-provide-the-secure-client-credentials-and-set-up-the-scope-type-of-requests-and-allowed-company-numbers--you-will-receive-the-unique-client-id-secret-and-paylocity-public-key-for-the-data-encryption--the-secret-will-expire-in-365-days---paylocity-will-send-you-an-email-10-days-prior-to-the-expiration-date-for-the-current-secret--if-not-renewed-the-second-email-notification-will-be-sent-5-days-prior-to-secrets-expiration--each-email-will-contain-the-code-necessary-to-renew-the-client-secret---you-can-obtain-the-new-secret-by-calling-api-endpoint-using-your-current-not-yet-expired-credentials-and-the-code-that-was-sent-with-the-notification-email--for-details-on-api-endpoint-please-see-client-credentials-section---both-the-current-secret-value-and-the-new-secret-value-will-be-recognized-during-the-transition-period--after-the-current-secret-expires-you-must-use-the-new-secret---if-you-were-unable-to-renew-the-secret-via-api-endpoint-you-can-still-contact-service-and-they-will-email-you-new-secret-via-secure-email-when-validating-the-request-paylocity-api-will-honor-the-defaults-and-required-fields-set-up-for-the-company-default-new-hire-template-as-defined-in-web-pay--authorizationpaylocity-web-services-api-uses-oauth2-0-authentication-with-json-message-format-all-requests-of-the-paylocity-web-services-api-require-a-bearer-token-which-can-be-obtained-by-authenticating-the-client-with-the-paylocity-web-services-api-via-oauth-2-0-the-client-must-request-a-bearer-token-from-the-authorization-endpointauthserver-for-production-httpsapi-paylocity-comidentityserverconnecttokenauthserver-for-testing-httpsapisandbox-paylocity-comidentityserverconnecttoken-authorization-headerthe-request-is-expected-to-be-in-the-form-of-a-basic-authentication-request-with-the-authorization-header-containing-the-clientid-and-clientsecret--this-means-the-standard-base64-encoded-userpassword-prefixed-with-basic-as-the-value-for-the-authorization-header-where-user-is-the-clientid-and-password-is-the-clientsecret--contenttype-headerthe-contenttype-header-is-required-to-be-applicationxwwwformurlencoded--additional-valuesthe-request-must-post-the-following-form-encoded-values-within-the-request-body----grant-type--client-credentials----scope--weblinkapi-responsessuccess-will-return-http-200-ok-with-json-content----------access-token-xxx------expires-in-3600------token-type-bearer-----encryptionpaylocity-uses-a-combination-of-rsa-and-aes-cryptography--as-part-of-the-setup-each-client-is-issued-a-public-rsa-key-paylocity-recommends-the-encryption-of-the-incoming-requests-as-additional-protection-of-the-sensitive-data--clients-can-optout-of-the-encryption-during-the-initial-setup-process--optout-will-allow-paylocity-to-process-unencrypted-requests-the-paylocity-public-key-has-the-following-properties-2048-bit-key-size-pkcs1-key-format-pem-encoding-properties-key-base-64-encoded-the-aes-symmetric-key-encrypted-with-the-paylocity-public-key--it-is-the-key-used-to-encrypt-the-content--paylocity-will-decrypt-the-aes-key-using-rsa-decryption-and-use-it-to-decrypt-the-content--iv-base-64-encoded-the-aes-iv-initialization-vector-used-when-encrypting-the-content--content-base-64-encoded-the-aes-encrypted-request--the-key-and-iv-provided-in-the-securecontent-request-are-used-by-paylocity-for-decryption-of-the-content-we-suggest-using-the-following-for-the-aes-cbc-cipher-mode-pkcs7-padding-128-bit-block-size-256-bit-key-size-sample-example----------securecontent---------key-es3aw6hqzhmj00gsi6gq3xa08dpmazk8bfy96pd99oda--------iv-nlyxmgq9svw0xo5ai9bzww--------content-gaeoiqlto1wlzguoik8fiybu42hug94eassl7nq1w-----------sample-c-code----using-newtonsoft-json----using-system----using-system-io----using-system-security-cryptography----using-system-text----public-class-securedcontent----------jsonpropertykey------public-string-key--get-set-------jsonpropertyiv------public-string-iv--get-set-------jsonpropertycontent------public-string-content--get-set---------public-class-endusersecurerequestexample----------public-string-createsecuredrequestfileinfo-paylocitypublickey-string-unsecuredjsonrequest--------------string-publickeyxml--file-readalltextpaylocitypublickey-fullname-encoding-utf8--------securedcontent-securecontent--this-createsecuredcontentpublickeyxml-unsecuredjsonrequest--------string-securerequest--jsonconvert-serializeobjectnew--securecontent---------return-securerequest------------private-securedcontent-createsecuredcontentstring-publickeyxml-string-request--------------using-aescryptoserviceprovider-aescsp--new-aescryptoserviceprovider------------------aescsp-mode--ciphermode-cbc----------aescsp-padding--paddingmode-pkcs7----------aescsp-blocksize--128----------aescsp-keysize--256----------using-icryptotransform-crt--aescsp-createencryptoraescsp-key-aescsp-iv----------------------using-memorystream-outputstream--new-memorystream--------------------------using-cryptostream-encryptstream--new-cryptostreamoutputstream-crt-cryptostreammode-write------------------------------byte-encodedrequest--encoding-utf8-getbytesrequest----------------encryptstream-writeencodedrequest-0-encodedrequest-length----------------encryptstream-flushfinalblock----------------byte-encryptedrequest--outputstream-toarray----------------using-rsacryptoserviceprovider-crp--new-rsacryptoserviceprovider----------------------------------crp-fromxmlstringpublickeyxml------------------byte-encryptedkey--crp-encryptaescsp-key-false------------------return-new-securedcontent--------------------------------------key--convert-tobase64stringencryptedkey--------------------iv--convert-tobase64stringaescsp-iv--------------------content--convert-tobase64stringencryptedrequest-----------------------------------------------------------------------------------------supportquestions-about-using-the-paylocity-api-please-contact-vendorrelationspaylocity-com--deductions-v1deductions-api-provides-endpoints-to-retrieve-add-update-and-delete-deductions-for-a-companys-employees--for-schema-details-click-a-hrefhttpsdocs-paylocity-comweblinkguidespaylocity-web-services-apiv1paylocity-web-services-api-htm-target-blankherea--onboarding-v1onboarding-api-sends-employee-data-into-paylocity-onboarding-to-help-ensure-an-easy-and-accurate-hiring-process-for-subsequent-completion-into-web-pay--for-schema-details-click-a-hrefhttpsdocs-paylocity-comweblinkguidespaylocity-web-services-apiv1paylocity-web-services-api-htm-target-blankherea-
  termsOfService: WebLink.OpenApiDoc.TermsOfService
  version: "2"
host: api.paylocity.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/companies/{companyId}/customfields/{category}:
    get:
      summary: Get All Custom Fields
      description: Get All Custom Fields for the selected company
      operationId: v2.companies.companyId.customfields.category.get
      x-api-path-slug: v2companiescompanyidcustomfieldscategory-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: category
        description: Custom Fields Category
      - in: path
        name: companyId
        description: Company Id
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Customfields
      - Category
  /v2/companies/{companyId}/employees:
    post:
      summary: Add new employee
      description: New Employee API sends new employee data directly to Web Pay. Companies
        who use the New Hire Template in Web Pay may require additional fields when
        hiring employees. New Employee API Requests will honor these required fields.
      operationId: v2.companies.companyId.employees.post
      x-api-path-slug: v2companiescompanyidemployees-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: body
        name: json
        description: Employee Model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
  /v2/companies/{companyId}/employees/{employeeId}:
    get:
      summary: Get employee
      description: Get Employee API will return employee data currently available
        in Web Pay.
      operationId: v2.companies.companyId.employees.employeeId.get
      x-api-path-slug: v2companiescompanyidemployeesemployeeid-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
    patch:
      summary: Update employee
      description: Update Employee API will update existing employee data in WebPay.
      operationId: v2.companies.companyId.employees.employeeId.patch
      x-api-path-slug: v2companiescompanyidemployeesemployeeid-patch
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      - in: body
        name: json
        description: Employee Model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
  /v2/companies/{companyId}/employees/{employeeId}/benefitSetup:
    put:
      summary: Add/update employee's benefit setup
      description: Sends new or updated employee benefit setup information directly
        to Web Pay.
      operationId: v2.companies.companyId.employees.employeeId.benefitSetup.put
      x-api-path-slug: v2companiescompanyidemployeesemployeeidbenefitsetup-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      - in: body
        name: json
        description: BenefitSetup Model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - BenefitSetup
  /v2/companies/{companyId}/employees/{employeeId}/earnings:
    get:
      summary: Get All Earnings
      description: Get All Earnings returns all earnings for the selected employee.
      operationId: v2.companies.companyId.employees.employeeId.earnings.get
      x-api-path-slug: v2companiescompanyidemployeesemployeeidearnings-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - Earnings
    put:
      summary: Add/Update Earning
      description: Add/Update Earning API sends new or updated employee earnings information
        directly to Web Pay.
      operationId: v2.companies.companyId.employees.employeeId.earnings.put
      x-api-path-slug: v2companiescompanyidemployeesemployeeidearnings-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      - in: body
        name: json
        description: Earning Model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - Earnings
  /v2/companies/{companyId}/employees/{employeeId}/earnings/{earningCode}:
    get:
      summary: Get Earnings by Earning Code
      description: Get Earnings returns all earnings with the provided earning code
        for the selected employee.
      operationId: v2.companies.companyId.employees.employeeId.earnings.earningCode.get
      x-api-path-slug: v2companiescompanyidemployeesemployeeidearningsearningcode-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: earningCode
        description: Earning Code
      - in: path
        name: employeeId
        description: Employee Id
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - Earnings
      - EarningCode
  /v2/companies/{companyId}/employees/{employeeId}/earnings/{earningCode}/{startDate}:
    delete:
      summary: Delete Earning by Earning Code and Start Date
      description: Delete Earning by Earning Code and Start Date
      operationId: v2.companies.companyId.employees.employeeId.earnings.earningCode.startDate.delete
      x-api-path-slug: v2companiescompanyidemployeesemployeeidearningsearningcodestartdate-delete
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: earningCode
        description: Earning Code
      - in: path
        name: employeeId
        description: Employee Id
      - in: path
        name: startDate
        description: Start Date
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - Earnings
      - EarningCode
      - StartDate
    get:
      summary: Get Earning by Earning Code and Start Date
      description: Get Earnings returns the single earning with the provided earning
        code and start date for the selected employee.
      operationId: v2.companies.companyId.employees.employeeId.earnings.earningCode.startDate.get
      x-api-path-slug: v2companiescompanyidemployeesemployeeidearningsearningcodestartdate-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: earningCode
        description: Earning Code
      - in: path
        name: employeeId
        description: Employee Id
      - in: path
        name: startDate
        description: Start Date
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - Earnings
      - EarningCode
      - StartDate
  /v2/companies/{companyId}/employees/{employeeId}/localTaxes:
    get:
      summary: Get all local taxes
      description: Returns all local taxes for the selected employee.
      operationId: v2.companies.companyId.employees.employeeId.localTaxes.get
      x-api-path-slug: v2companiescompanyidemployeesemployeeidlocaltaxes-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - LocalTaxes
    post:
      summary: Add new local tax
      description: Sends new employee local tax information directly to Web Pay.
      operationId: v2.companies.companyId.employees.employeeId.localTaxes.post
      x-api-path-slug: v2companiescompanyidemployeesemployeeidlocaltaxes-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      - in: body
        name: json
        description: LocalTax Model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - LocalTaxes
  /v2/companies/{companyId}/employees/{employeeId}/localTaxes/{taxCode}:
    delete:
      summary: Delete local tax by tax code
      description: Delete local tax by tax code
      operationId: v2.companies.companyId.employees.employeeId.localTaxes.taxCode.delete
      x-api-path-slug: v2companiescompanyidemployeesemployeeidlocaltaxestaxcode-delete
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      - in: path
        name: taxCode
        description: Tax Code
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - LocalTaxes
      - TaxCode
    get:
      summary: Get local taxes by tax code
      description: Returns all local taxes with the provided tax code for the selected
        employee.
      operationId: v2.companies.companyId.employees.employeeId.localTaxes.taxCode.get
      x-api-path-slug: v2companiescompanyidemployeesemployeeidlocaltaxestaxcode-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      - in: path
        name: taxCode
        description: Tax Code
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - LocalTaxes
      - TaxCode
  /v2/companies/{companyId}/employees/{employeeId}/nonprimaryStateTax:
    put:
      summary: Add/update non-primary state tax
      description: Sends new or updated employee non-primary state tax information
        directly to Web Pay.
      operationId: v2.companies.companyId.employees.employeeId.nonprimaryStateTax.put
      x-api-path-slug: v2companiescompanyidemployeesemployeeidnonprimarystatetax-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      - in: body
        name: json
        description: Non-Primary State Tax Model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - NonprimaryStateTax
  /v2/companies/{companyId}/employees/{employeeId}/primaryStateTax:
    put:
      summary: Add/update primary state tax
      description: Sends new or updated employee primary state tax information directly
        to Web Pay.
      operationId: v2.companies.companyId.employees.employeeId.primaryStateTax.put
      x-api-path-slug: v2companiescompanyidemployeesemployeeidprimarystatetax-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      - in: body
        name: json
        description: Primary State Tax Model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - PrimaryStateTax
  /v2/companies/{companyId}/openapi:
    get:
      summary: Get Company-Specific Open API Documentation
      description: The company-specific Open API endpoint allows the client to GET
        an Open API document for the Paylocity API that is customized with company-specific
        resource schemas. These customized resource schemas define certain properties
        as enumerations of pre-defined values that correspond to the company's setup
        with Web Pay. The customized schemas also indicate which properties are required
        by the company within Web Pay.<br  />To learn more about Open API, click [here](https://www.openapis.org/)
      operationId: v2.companies.companyId.openapi.get
      x-api-path-slug: v2companiescompanyidopenapi-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Openapi
  /v2/credentials/secrets:
    post:
      summary: Obtain new client secret.
      description: Obtain new client secret for Paylocity-issued client id. See Setup
        section for details.
      operationId: v2.credentials.secrets.post
      x-api-path-slug: v2credentialssecrets-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: body
        name: json
        description: Add Client Secret Model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - V2
      - Credentials
      - Secrets
  /v2/weblinkstaging/companies/{companyId}/employees/newemployees:
    post:
      summary: Add new employee to Web Link
      description: Add new employee to Web Link will send partially completed or potentially
        erroneous new hire record to Web Link, where it can be corrected and competed
        by company administrator or authorized Paylocity Service Bureau employee.
      operationId: v2.weblinkstaging.companies.companyId.employees.newemployees.post
      x-api-path-slug: v2weblinkstagingcompaniescompanyidemployeesnewemployees-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: body
        name: json
        description: StagedEmployee Model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - V2
      - Weblinkstaging
      - Companies
      - CompanyId
      - Employees
      - Newemployees