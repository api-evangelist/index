swagger: "2.0"
x-collection-name: PayRun
x-complete: 1
info:
  title: Pay Run.IO
  description: open-scableable-transparent-payroll-api-
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Employer/{EmployerId}:
    delete:
      summary: Delete an Employer
      description: Delete the specified employer
      operationId: DeleteEmployer
      x-api-path-slug: employeremployerid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employer
    get:
      summary: Gets the employer
      description: Get the specified employer object
      operationId: GetEmployer
      x-api-path-slug: employeremployerid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employer
    patch:
      summary: Patches the employer
      description: Patches the specified employer with the supplied values
      operationId: PatchEmployer
      x-api-path-slug: employeremployerid-patch
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: Employer
        description: The employer object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Patches
      - Employer
    put:
      summary: Updates the Employer
      description: Updates the existing specified employer object
      operationId: PutEmployer
      x-api-path-slug: employeremployerid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: Employer
        description: The employer object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employer
  /Employer/{EmployerId}/DpsMessage/{DpsMessageId}:
    delete:
      summary: Deletes the DPS message
      description: Deletes the DPS message
      operationId: DeleteDpsMessage
      x-api-path-slug: employeremployeriddpsmessagedpsmessageid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: DpsMessageId
        description: The DPS message unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - DPMessage
    get:
      summary: Gets the DPS message
      description: Gets the DPS message
      operationId: GetDpsMessageFromEmployer
      x-api-path-slug: employeremployeriddpsmessagedpsmessageid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: DpsMessageId
        description: The DPS message unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - DPMessage
    patch:
      summary: Patches the DPS message
      description: Patches the specified DPS message with the supplied values
      operationId: PatchDpsMessage
      x-api-path-slug: employeremployeriddpsmessagedpsmessageid-patch
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: DpsMessageId
        description: The DPS message unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Patches
      - DPMessage
  /Employer/{EmployerId}/DpsMessages:
    get:
      summary: Gets the DPS messages
      description: Gets the DPS message links
      operationId: GetDpsMessagesFromEmployer
      x-api-path-slug: employeremployeriddpsmessages-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - DPMessages
  /Employer/{EmployerId}/Employee/{EmployeeId}:
    delete:
      summary: Delete an Employee
      description: Delete the specified employee
      operationId: DeleteEmployee
      x-api-path-slug: employeremployeridemployeeemployeeid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employee
    get:
      summary: Get employee from employer
      description: Gets the specified employee from employer by employee code.
      operationId: GetEmployeeFromEmployer
      x-api-path-slug: employeremployeridemployeeemployeeid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employee
      - From
      - Employer
    patch:
      summary: Patches the employee
      description: Patches the specified employee with the supplied values
      operationId: PatchEmployee
      x-api-path-slug: employeremployeridemployeeemployeeid-patch
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: Employee
        description: The employee object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Patches
      - Employee
    put:
      summary: Updates the Employee
      description: Updates the existing specified employee object
      operationId: PutEmployeeIntoEmployer
      x-api-path-slug: employeremployeridemployeeemployeeid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: Employee
        description: The employee object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employee
  /Employer/{EmployerId}/Employee/{EmployeeId}/AEAssessment/{AEAssessmentId}:
    delete:
      summary: Delete auto enrolment assessment
      description: Deletes an existing auto enrolment assessment for the employee.
        Used to remove historical assessments
      operationId: DeleteAEAssessment
      x-api-path-slug: employeremployeridemployeeemployeeidaeassessmentaeassessmentid-delete
      parameters:
      - in: path
        name: AEAssessmentId
        description: The auto enrolment assessment unique identifier
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Auto
      - Enrolment
      - Assessment
    get:
      summary: Get the auto enrolment assessment
      description: Gets the auto enrolment assessment from the specified employee
      operationId: GetAEAssessmentFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidaeassessmentaeassessmentid-get
      parameters:
      - in: path
        name: AEAssessmentId
        description: The auto enrolment assessment unique identifier
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Auto
      - Enrolment
      - Assessment
    put:
      summary: Insert new auto enrolment assessment
      description: Creates a new auto enrolment assessment for the employee. Used
        to insert historical assessments
      operationId: PutNewAEAssessment
      x-api-path-slug: employeremployeridemployeeemployeeidaeassessmentaeassessmentid-put
      parameters:
      - in: body
        name: AEAssessment
        description: The auto enrolment assessment object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: AEAssessmentId
        description: The auto enrolment assessment unique identifier
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Insert
      - New
      - Auto
      - Enrolment
      - Assessment
  /Employer/{EmployerId}/Employee/{EmployeeId}/AEAssessments:
    get:
      summary: Get the auto enrolment assessments
      description: Gets all auto enrolment assessments from the specified employee
      operationId: GetAEAssessmentsFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidaeassessments-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Auto
      - Enrolment
      - Assessments
    post:
      summary: Insert new auto enrolment assessment
      description: Creates a new auto enrolment assessment for the employee. Used
        to insert historical assessments
      operationId: PostNewAEAssessment
      x-api-path-slug: employeremployeridemployeeemployeeidaeassessments-post
      parameters:
      - in: body
        name: AEAssessment
        description: The auto enrolment assessment object
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Insert
      - New
      - Auto
      - Enrolment
      - Assessment
  /Employer/{EmployerId}/Employee/{EmployeeId}/Commentaries:
    get:
      summary: Get links to all commentaries for the specified employee
      description: Get links to all commentaries for the specified employee.
      operationId: GetCommentariesFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidcommentaries-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Links
      - To
      - ""
      - Commentariesthe
      - Specified
      - Employee
  /Employer/{EmployerId}/Employee/{EmployeeId}/Commentary/{CommentaryId}:
    get:
      summary: Get commentary from employee
      description: Gets the specified commentary report from the employee
      operationId: GetCommentaryFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidcommentarycommentaryid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: CommentaryId
        description: The commentary unique identifier
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Commentary
      - From
      - Employee
  /Employer/{EmployerId}/Employee/{EmployeeId}/PayInstruction/{PayInstructionId}:
    delete:
      summary: Deletes a pay instruction
      description: Delete the specified pay instruction
      operationId: DeletePayInstruction
      x-api-path-slug: employeremployeridemployeeemployeeidpayinstructionpayinstructionid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayInstructionId
        description: The pay instruction unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Instruction
    get:
      summary: Gets the specified pay instruction from the employee
      description: Returns the specified pay instruction from employee
      operationId: GetPayInstructionFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidpayinstructionpayinstructionid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayInstructionId
        description: The pay instruction unique identifier
      responses:
        200:
          description: OK
      tags:
      - Specified
      - Pay
      - Instruction
      - From
      - Employee
    patch:
      summary: Sparse Update of a Pay Instruction
      description: Patches the specified pay instruction with the supplied values
      operationId: PatchPayInstruction
      x-api-path-slug: employeremployeridemployeeemployeeidpayinstructionpayinstructionid-patch
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: body
        name: PayInstruction
        description: The pay instruction object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: PayInstructionId
        description: The pay instruction unique identifier
      responses:
        200:
          description: OK
      tags:
      - Sparse
      - ""
      - Of
      - Pay
      - Instruction
    put:
      summary: Update a Pay Instruction
      description: Updates the existing specified pay instruction object
      operationId: PutPayInstruction
      x-api-path-slug: employeremployeridemployeeemployeeidpayinstructionpayinstructionid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: body
        name: PayInstruction
        description: The pay instruction object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: PayInstructionId
        description: The pay instruction unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Instruction
  /Employer/{EmployerId}/Employee/{EmployeeId}/PayInstructions:
    get:
      summary: Gets the pay instructions from the specified employee
      description: Get links to all pay instructions for the specified employee
      operationId: GetPayInstructionsFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidpayinstructions-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Instructions
      - From
      - Specified
      - Employee
    post:
      summary: Creates a new Pay Instruction
      description: Creates a new pay instruction object
      operationId: PostPayInstruction
      x-api-path-slug: employeremployeridemployeeemployeeidpayinstructions-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: body
        name: PayInstruction
        description: The pay instruction object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Pay
      - Instruction
  /Employer/{EmployerId}/Employee/{EmployeeId}/PayLine/{PayLineId}:
    get:
      summary: Gets the specified pay line from the employee
      description: Returns the specified pay line from employee
      operationId: GetPayLineFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidpaylinepaylineid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayLineId
        description: The pay line unique identifier
      responses:
        200:
          description: OK
      tags:
      - Specified
      - Pay
      - Line
      - From
      - Employee
  /Employer/{EmployerId}/Employee/{EmployeeId}/PayLines:
    get:
      summary: Gets the pay lines from the specified employee
      description: Get links to all pay lines for the specified employee
      operationId: GetPayLinesFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidpaylines-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Lines
      - From
      - Specified
      - Employee
  /Employer/{EmployerId}/Employee/{EmployeeId}/PayRuns:
    get:
      summary: Gets the pay runs from the employee
      description: Get links to all pay runs for the specified employee.
      operationId: GetPayRunsFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidpayruns-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Runs
      - From
      - Employee
  /Employer/{EmployerId}/Employee/{EmployeeId}/Tag/{TagId}:
    delete:
      summary: Delete employee tag
      description: Deletes a tag from the employee
      operationId: DeleteEmployeeTag
      x-api-path-slug: employeremployeridemployeeemployeeidtagtagid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employee
      - Tag
    get:
      summary: Get employee tag
      description: Gets the tag from the employee
      operationId: GetTagFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidtagtagid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employee
      - Tag
    put:
      summary: Insert employee tag
      description: Inserts a new tag on the employee
      operationId: PutEmployeeTag
      x-api-path-slug: employeremployeridemployeeemployeeidtagtagid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Employee
      - Tag
  /Employer/{EmployerId}/Employee/{EmployeeId}/Tag/{TagId}/{EffectiveDate}:
    get:
      summary: Get employee revision tag
      description: Gets the tag from the employee revision
      operationId: GetTagFromEmployeeRevision
      x-api-path-slug: employeremployeridemployeeemployeeidtagtagideffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employee
      - Revision
      - Tag
  /Employer/{EmployerId}/Employee/{EmployeeId}/Tags:
    get:
      summary: Get all employee tags
      description: Gets all the tags from the employee
      operationId: GetTagsFromEmployee
      x-api-path-slug: employeremployeridemployeeemployeeidtags-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employee
      - Tags
  /Employer/{EmployerId}/Employee/{EmployeeId}/Tags/{EffectiveDate}:
    get:
      summary: Get all employee revision tags
      description: Gets all the tags from the employee revision
      operationId: GetTagsFromEmployeeRevision
      x-api-path-slug: employeremployeridemployeeemployeeidtagseffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employee
      - Revision
      - Tags
  /Employer/{EmployerId}/Employee/{EmployeeId}/{EffectiveDate}:
    delete:
      summary: Delete an Employee revision matching the specified revision date.
      description: Deletes the specified employee revision for the matching revision
        date
      operationId: DeleteEmployeeRevision
      x-api-path-slug: employeremployeridemployeeemployeeideffectivedate-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employee
      - Revision
      - Matching
      - Specified
      - Revision
      - Date
    get:
      summary: Get employee by effective date.
      description: Returns the employee's state at the specified effective date.
      operationId: GetEmployeeByEffectiveDate
      x-api-path-slug: employeremployeridemployeeemployeeideffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employee
      - By
      - Effective
      - Date
  /Employer/{EmployerId}/Employees:
    get:
      summary: Get employees from employer.
      description: Get links to all employees for the specified employer.
      operationId: GetEmployeesFromEmployer
      x-api-path-slug: employeremployeridemployees-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employees
      - From
      - Employer
    post:
      summary: Create a new Employee
      description: Create a new employee object
      operationId: PostEmployeeIntoEmployer
      x-api-path-slug: employeremployeridemployees-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: Employee
        description: The employee object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - New
      - Employee
  /Employer/{EmployerId}/Employees/Tag/{TagId}:
    get:
      summary: Get employees with tag
      description: Gets the employees with the tag
      operationId: GetEmployeesWithTag
      x-api-path-slug: employeremployeridemployeestagtagid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employees
      - Tag
  /Employer/{EmployerId}/Employees/Tags:
    get:
      summary: Get all employee tags
      description: Gets all the employee tags
      operationId: GetAllEmployeeTags
      x-api-path-slug: employeremployeridemployeestags-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employee
      - Tags
  /Employer/{EmployerId}/Employees/{EffectiveDate}:
    get:
      summary: Get employees from employer at a given effective date.
      description: Get links to all employees for the employer on specified effective
        date.
      operationId: GetEmployeesByEffectiveDate
      x-api-path-slug: employeremployeridemployeeseffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employees
      - From
      - Employer
      - At
      - Given
      - Effective
      - Date
  /Employer/{EmployerId}/NominalCode/{NominalCodeId}:
    delete:
      summary: Deletes the nominal codes
      description: Deletes the nominal code
      operationId: DeleteNominalCode
      x-api-path-slug: employeremployeridnominalcodenominalcodeid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: NominalCodeId
        description: The nominal code unique identifier
      responses:
        200:
          description: OK
      tags:
      - Nominal
      - Codes
    get:
      summary: Gets the nominal code
      description: Gets the nominal code
      operationId: GetNominalCodeFromEmployer
      x-api-path-slug: employeremployeridnominalcodenominalcodeid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: NominalCodeId
        description: The nominal code unique identifier
      responses:
        200:
          description: OK
      tags:
      - Nominal
      - Code
    put:
      summary: Insert nominal code
      description: Inserts a new nominal code at the specified resource location
      operationId: PutNominalCode
      x-api-path-slug: employeremployeridnominalcodenominalcodeid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: body
        name: NominalCode
        description: The nominal code object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: NominalCodeId
        description: The nominal code unique identifier
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Nominal
      - Code
  /Employer/{EmployerId}/NominalCodes:
    get:
      summary: Gets the nominal codes
      description: Gets the nominal code links
      operationId: GetNominalCodesFromEmployer
      x-api-path-slug: employeremployeridnominalcodes-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Nominal
      - Codes
    post:
      summary: Insert nominal code
      description: Inserts a new nominal code
      operationId: PostNominalCode
      x-api-path-slug: employeremployeridnominalcodes-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: body
        name: NominalCode
        description: The nominal code object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Nominal
      - Code
  /Employer/{EmployerId}/PayCode/{PayCodeId}:
    delete:
      summary: Deletes a pay code
      description: Delete the specified pay code
      operationId: DeletePayCode
      x-api-path-slug: employeremployeridpaycodepaycodeid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayCodeId
        description: The pay code unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Code
    get:
      summary: Gets the specified pay code from the employer
      description: Returns the specified pay code from the employer
      operationId: GetPayCodeFromEmployer
      x-api-path-slug: employeremployeridpaycodepaycodeid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayCodeId
        description: The pay code unique identifier
      responses:
        200:
          description: OK
      tags:
      - Specified
      - Pay
      - Code
      - From
      - Employer
    patch:
      summary: Patches the pay code
      description: Patches the specified pay code object with the supplied values
      operationId: PatchPayCode
      x-api-path-slug: employeremployeridpaycodepaycodeid-patch
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: body
        name: PayCode
        description: The pay code object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: PayCodeId
        description: The pay code unique identifier
      responses:
        200:
          description: OK
      tags:
      - Patches
      - Pay
      - Code
    put:
      summary: Updates a pay code
      description: Updates the existing specified pay code object
      operationId: PutPayCode
      x-api-path-slug: employeremployeridpaycodepaycodeid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: body
        name: PayCode
        description: The pay code object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: PayCodeId
        description: The pay code unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Code
  /Employer/{EmployerId}/PayCode/{PayCodeId}/Tag/{TagId}:
    delete:
      summary: Delete pay code tag
      description: Deletes a tag from the pay code
      operationId: DeletePayCodeTag
      x-api-path-slug: employeremployeridpaycodepaycodeidtagtagid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayCodeId
        description: The pay code unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Code
      - Tag
    get:
      summary: Get pay code tag
      description: Gets the tag from the pay code
      operationId: GetTagFromPayCode
      x-api-path-slug: employeremployeridpaycodepaycodeidtagtagid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayCodeId
        description: The pay code unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Code
      - Tag
    put:
      summary: Insert pay code tag
      description: Inserts a new tag on the pay code
      operationId: PutPayCodeTag
      x-api-path-slug: employeremployeridpaycodepaycodeidtagtagid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayCodeId
        description: The pay code unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Pay
      - Code
      - Tag
  /Employer/{EmployerId}/PayCode/{PayCodeId}/Tags:
    get:
      summary: Get all pay code tags
      description: Gets all the tags from the pay code
      operationId: GetTagsFromPayCode
      x-api-path-slug: employeremployeridpaycodepaycodeidtags-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayCodeId
        description: The pay code unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Code
      - Tags
  /Employer/{EmployerId}/PayCode/{PayCodeId}/{EffectiveDate}:
    delete:
      summary: Deletes a pay code revision
      description: Delete the pay code revision for the specified date
      operationId: DeletePayCodeRevision
      x-api-path-slug: employeremployeridpaycodepaycodeideffectivedate-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayCodeId
        description: The pay code unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Code
      - Revision
    get:
      summary: Gets pay code for specified date
      description: Gets the pay code revision for the specified effective date
      operationId: GetPayCodeByEffectiveDate
      x-api-path-slug: employeremployeridpaycodepaycodeideffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayCodeId
        description: The pay code unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Codespecified
      - Date
  /Employer/{EmployerId}/PayCodes:
    get:
      summary: Gets the pay codes from the employer
      description: Get links to all the pay codes for the specified employer
      operationId: GetPayCodesFromEmployer
      x-api-path-slug: employeremployeridpaycodes-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Codes
      - From
      - Employer
    post:
      summary: Create a new pay code
      description: Create a new pay code object
      operationId: PostPayCode
      x-api-path-slug: employeremployeridpaycodes-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: body
        name: PayCode
        description: The pay code object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Pay
      - Code
  /Employer/{EmployerId}/PayCodes/Tag/{TagId}:
    get:
      summary: Get pay codes with tag
      description: Gets the pay codes with the tag
      operationId: GetPayCodesWithTag
      x-api-path-slug: employeremployeridpaycodestagtagid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Codes
      - Tag
  /Employer/{EmployerId}/PayCodes/Tags:
    get:
      summary: Get all pay code tags
      description: Gets all the pay code tags
      operationId: GetAllPayCodeTags
      x-api-path-slug: employeremployeridpaycodestags-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Code
      - Tags
  /Employer/{EmployerId}/PayCodes/{EffectiveDate}:
    get:
      summary: Gets all pay codes for specified date
      description: Gets the effective pay code revision for the specified date
      operationId: GetPayCodesByEffectiveDate
      x-api-path-slug: employeremployeridpaycodeseffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - ""
      - Pay
      - Codesspecified
      - Date
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}:
    delete:
      summary: Deletes a pay schedule
      description: Delete the specified pay schedule
      operationId: DeletePaySchedule
      x-api-path-slug: employeremployeridpayschedulepayscheduleid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Schedule
    get:
      summary: Gets the specified pay schedule from the employer
      description: Returns the specified pay schedule object from employer
      operationId: GetPayScheduleFromEmployer
      x-api-path-slug: employeremployeridpayschedulepayscheduleid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Specified
      - Pay
      - Schedule
      - From
      - Employer
    put:
      summary: Updates a pay schedule
      description: Updates the existing specified pay schedule object
      operationId: PutPaySchedule
      x-api-path-slug: employeremployeridpayschedulepayscheduleid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: body
        name: PaySchedule
        description: The pay schedule object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Schedule
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/Employees:
    get:
      summary: Get employees from a pay schedule.
      description: Gets links to all employees included in the specified pay schedule.
      operationId: GetEmployeesFromPaySchedule
      x-api-path-slug: employeremployeridpayschedulepayscheduleidemployees-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employees
      - From
      - Pay
      - Schedule
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}:
    delete:
      summary: Deletes a pay run
      description: Delete the specified pay run
      operationId: DeletePayRun
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
    get:
      summary: Gets the pay run from the pay schedule
      description: Returns the pay run from the pay schedule
      operationId: GetPayRunFromPaySchedule
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - From
      - Pay
      - Schedule
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}/AEAssessments:
    get:
      summary: Get the auto enrolment assessments
      description: Gets all auto enrolment assessments from the specified pay run
      operationId: GetAEAssessmentsFromPayRun
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidaeassessments-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Auto
      - Enrolment
      - Assessments
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}/Employee/{EmployeeId}:
    delete:
      summary: Deletes a pay run employee
      description: Delete pay run results for a single employee
      operationId: DeletePayRunEmployee
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidemployeeemployeeid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Employee
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}/Employees:
    get:
      summary: Get employees from the pay run
      description: Gets links to all employees included in the specified pay run.
      operationId: GetEmployeesFromPayRun
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidemployees-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employees
      - From
      - Pay
      - Run
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}/ReportLines:
    get:
      summary: Gets the report lines from the specified pay run
      description: Returns all report lines associated with the specified pay run
      operationId: GetReportLinesFromPayRun
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidreportlines-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Report
      - Lines
      - From
      - Specified
      - Pay
      - Run
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}/Tag/{TagId}:
    delete:
      summary: Delete pay run tag
      description: Deletes a tag from the pay run
      operationId: DeletePayRunTag
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidtagtagid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Tag
    get:
      summary: Get pay run tag
      description: Gets the tag from the pay run
      operationId: GetTagFromPayRun
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidtagtagid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Tag
    put:
      summary: Insert pay run tag
      description: Inserts a new tag on the pay run
      operationId: PutPayRunTag
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidtagtagid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Pay
      - Run
      - Tag
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}/Tags:
    get:
      summary: Get all pay run tags
      description: Gets all the tags from the pay run
      operationId: GetTagsFromPayRun
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidtags-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Tags
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRuns:
    get:
      summary: Gets the pay runs from the pay schedule
      description: Get links to all pay runs for the specified pay schedule
      operationId: GetPayRunsFromPaySchedule
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayruns-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Runs
      - From
      - Pay
      - Schedule
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRuns/Tag/{TagId}:
    get:
      summary: Get pay runs with tag
      description: Gets the pay runs with the tag
      operationId: GetPayRunsWithTag
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunstagtagid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Runs
      - Tag
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRuns/Tags:
    get:
      summary: Get all pay run tags
      description: Gets all the pay run tags
      operationId: GetAllPayRunTags
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunstags-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Tags
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/Tag/{TagId}:
    delete:
      summary: Delete pay schedule tag
      description: Deletes a tag from the pay schedule
      operationId: DeletePayScheduleTag
      x-api-path-slug: employeremployeridpayschedulepayscheduleidtagtagid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Schedule
      - Tag
    get:
      summary: Get pay schedule tag
      description: Gets the tag from the pay schedule
      operationId: GetTagFromPaySchedule
      x-api-path-slug: employeremployeridpayschedulepayscheduleidtagtagid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Schedule
      - Tag
    put:
      summary: Insert pay schedule tag
      description: Inserts a new tag on the pay schedule
      operationId: PutPayScheduleTag
      x-api-path-slug: employeremployeridpayschedulepayscheduleidtagtagid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Pay
      - Schedule
      - Tag
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/Tags:
    get:
      summary: Get all pay schedule tags
      description: Gets all the tags from the pay schedule
      operationId: GetTagsFromPaySchedule
      x-api-path-slug: employeremployeridpayschedulepayscheduleidtags-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Schedule
      - Tags
  /Employer/{EmployerId}/PaySchedules:
    get:
      summary: Gets the pay schedule from the specified employer
      description: Get links to all pay schedules for the specified employer
      operationId: GetPaySchedulesFromEmployer
      x-api-path-slug: employeremployeridpayschedules-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Schedule
      - From
      - Specified
      - Employer
    post:
      summary: Create a new pay schedule
      description: Create a new pay schedule object
      operationId: PostPaySchedule
      x-api-path-slug: employeremployeridpayschedules-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: body
        name: PaySchedule
        description: The pay schedule object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Pay
      - Schedule
  /Employer/{EmployerId}/PaySchedules/Tag/{TagId}:
    get:
      summary: Get pay schedule with tag
      description: Gets the pay schedules with the tag
      operationId: GetPaySchedulesWithTag
      x-api-path-slug: employeremployeridpayschedulestagtagid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Schedule
      - Tag
  /Employer/{EmployerId}/PaySchedules/Tags:
    get:
      summary: Get all pay schedule tags
      description: Gets all the pay schedule tags
      operationId: GetAllPayScheduleTags
      x-api-path-slug: employeremployeridpayschedulestags-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Schedule
      - Tags
  /Employer/{EmployerId}/Pension/{PensionId}:
    delete:
      summary: Delete a Pension
      description: Delete the specified ppension
      operationId: DeletePension
      x-api-path-slug: employeremployeridpensionpensionid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PensionId
        description: The pensions unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pension
    get:
      summary: Get pension from employer
      description: Gets the specified pension from employer by pension code.
      operationId: GetPensionFromEmployer
      x-api-path-slug: employeremployeridpensionpensionid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PensionId
        description: The pensions unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pension
      - From
      - Employer
    patch:
      summary: Patches the pension
      description: Patches the specified pension with the supplied values
      operationId: PatchPension
      x-api-path-slug: employeremployeridpensionpensionid-patch
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: body
        name: Pension
        description: The pension object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: PensionId
        description: The pensions unique identifier
      responses:
        200:
          description: OK
      tags:
      - Patches
      - Pension
    put:
      summary: Updates the Pension
      description: Updates existing or inserts the specified pension object
      operationId: PutPensionIntoEmployer
      x-api-path-slug: employeremployeridpensionpensionid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: body
        name: Pension
        description: The pension object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: PensionId
        description: The pensions unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pension
  /Employer/{EmployerId}/Pension/{PensionId}/{EffectiveDate}:
    delete:
      summary: Delete an Pension revision matching the specified revision date.
      description: Deletes the specified pension revision for the matching revision
        date
      operationId: DeletePensionRevision
      x-api-path-slug: employeremployeridpensionpensionideffectivedate-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PensionId
        description: The pensions unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pension
      - Revision
      - Matching
      - Specified
      - Revision
      - Date
    get:
      summary: Get pension by effective date.
      description: Returns the penion's state at the specified effective date.
      operationId: GetPensionByEffectiveDate
      x-api-path-slug: employeremployeridpensionpensionideffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PensionId
        description: The pensions unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pension
      - By
      - Effective
      - Date
  /Employer/{EmployerId}/Pensions:
    get:
      summary: Get pensions from employer.
      description: Get links to all pensions for the specified employer.
      operationId: GetPensionsFromEmployer
      x-api-path-slug: employeremployeridpensions-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pensions
      - From
      - Employer
    post:
      summary: Create a new Pension
      description: Create a new pension object
      operationId: PostPensionIntoEmployer
      x-api-path-slug: employeremployeridpensions-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: body
        name: Pension
        description: The pension object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Pension
  /Employer/{EmployerId}/Pensions/{EffectiveDate}:
    get:
      summary: Get pensions from employer at a given effective date.
      description: Get links to all pensions for the employer on specified effective
        date.
      operationId: GetPensionsByEffectiveDate
      x-api-path-slug: employeremployeridpensionseffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pensions
      - From
      - Employer
      - At
      - Given
      - Effective
      - Date
  /Employer/{EmployerId}/ReportLine/{ReportLineId}:
    get:
      summary: Gets the specified report line from the employer
      description: Returns the specified pay line from employee
      operationId: GetReportLineFromEmployer
      x-api-path-slug: employeremployeridreportlinereportlineid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: ReportLineId
        description: The report line unique identifier
      responses:
        200:
          description: OK
      tags:
      - Specified
      - Report
      - Line
      - From
      - Employer
  /Employer/{EmployerId}/ReportLines:
    get:
      summary: Gets the report lines from the specified employer
      description: Get links to all report lines for the specified employee
      operationId: GetReportLinesFromEmployer
      x-api-path-slug: employeremployeridreportlines-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Report
      - Lines
      - From
      - Specified
      - Employer
  /Employer/{EmployerId}/ReportingInstruction/{ReportingInstructionId}:
    delete:
      summary: Deletes a reporting instruction
      description: Delete the specified reporting instruction
      operationId: DeleteReportingInstruction
      x-api-path-slug: employeremployeridreportinginstructionreportinginstructionid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: ReportingInstructionId
        description: The reporting instruction unique identifier
      responses:
        200:
          description: OK
      tags:
      - Reporting
      - Instruction
    get:
      summary: Gets the specified reporting instruction from the employer
      description: Returns the specified pay instruction from employee
      operationId: GetReportingInstructionFromEmployer
      x-api-path-slug: employeremployeridreportinginstructionreportinginstructionid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: ReportingInstructionId
        description: The reporting instruction unique identifier
      responses:
        200:
          description: OK
      tags:
      - Specified
      - Reporting
      - Instruction
      - From
      - Employer
    put:
      summary: Update a reporting Instruction
      description: Updates the existing specified reporting instruction object
      operationId: PutReportingInstruction
      x-api-path-slug: employeremployeridreportinginstructionreportinginstructionid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: ReportingInstructionId
        description: The reporting instruction unique identifier
      responses:
        200:
          description: OK
      tags:
      - Reporting
      - Instruction
  /Employer/{EmployerId}/ReportingInstructions:
    get:
      summary: Gets the reporting instructions from the specified employer
      description: Get links to all pay instructions for the specified employee
      operationId: GetReportingInstructionsFromEmployer
      x-api-path-slug: employeremployeridreportinginstructions-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Reporting
      - Instructions
      - From
      - Specified
      - Employer
    post:
      summary: Creates a new Reporting Instruction
      description: Creates a new reporting instruction object
      operationId: PostReportingInstruction
      x-api-path-slug: employeremployeridreportinginstructions-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Reporting
      - Instruction
  /Employer/{EmployerId}/RtiTransaction/{RtiTransactionId}:
    get:
      summary: Get the RTI transaction
      description: Returns the specified RTI transaction
      operationId: GetRtiTransactionFromEmployer
      x-api-path-slug: employeremployeridrtitransactionrtitransactionid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: RtiTransactionId
        description: The RTI transaction unique identifier
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Transaction
  /Employer/{EmployerId}/RtiTransactions:
    get:
      summary: Get all RTI transactions for the employer
      description: Get links for all RTI transactions for the specified employer
      operationId: GetRtiTransactionsFromEmployer
      x-api-path-slug: employeremployeridrtitransactions-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Transactionsthe
      - Employer
  /Employer/{EmployerId}/Tag/{TagId}:
    delete:
      summary: Delete employer tag
      description: Deletes a tag from the employer
      operationId: DeleteEmployerTag
      x-api-path-slug: employeremployeridtagtagid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employer
      - Tag
    get:
      summary: Get employer tag
      description: Gets the tag from the employer
      operationId: GetTagFromEmployer
      x-api-path-slug: employeremployeridtagtagid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employer
      - Tag
    put:
      summary: Insert employer tag
      description: Inserts a new tag on the employer
      operationId: PutEmployerTag
      x-api-path-slug: employeremployeridtagtagid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Employer
      - Tag
  /Employer/{EmployerId}/Tag/{TagId}/{EffectiveDate}:
    get:
      summary: Get employer revision tag
      description: Gets the tag from the employer revision
      operationId: GetTagFromEmployerRevision
      x-api-path-slug: employeremployeridtagtagideffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employer
      - Revision
      - Tag
  /Employer/{EmployerId}/Tags:
    get:
      summary: Get all employer tags
      description: Gets all the tags from the employer
      operationId: GetTagsFromEmployer
      x-api-path-slug: employeremployeridtags-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employer
      - Tags
  /Employer/{EmployerId}/Tags/{EffectiveDate}:
    get:
      summary: Get all employer revision tags
      description: Gets all the tags from the employer revision
      operationId: GetTagsFromEmployerRevision
      x-api-path-slug: employeremployeridtagseffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employer
      - Revision
      - Tags
  /Employer/{EmployerId}/{EffectiveDate}:
    delete:
      summary: Delete an Employer revision matching the specified revision date.
      description: Deletes the specified employer revision for the matching revision
        date
      operationId: DeleteEmployerRevision
      x-api-path-slug: employeremployerideffectivedate-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employer
      - Revision
      - Matching
      - Specified
      - Revision
      - Date
    get:
      summary: Gets the employer at the specified effective
      description: Returns the employer's state at the specified effective date.
      operationId: GetEmployerByEffectiveDate
      x-api-path-slug: employeremployerideffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employer
      - At
      - Specified
      - Effective
  /Employers:
    get:
      summary: Gets all employers
      description: Gets links to all employers contained under the authorised application
        scope
      operationId: GetEmployers
      x-api-path-slug: employers-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - ""
      - Employers
    post:
      summary: Create a new Employer
      description: Create a new employer object
      operationId: PostEmployer
      x-api-path-slug: employers-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: Employer
        description: The employer object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Employer
  /Employers/Tag/{TagId}:
    get:
      summary: Get employers with tag
      description: Gets the employers with the tag
      operationId: GetEmployersWithTag
      x-api-path-slug: employerstagtagid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employers
      - Tag
  /Employers/Tags:
    get:
      summary: Get all employer tags
      description: Gets all the employer tags
      operationId: GetAllEmployerTags
      x-api-path-slug: employerstags-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Employer
      - Tags
  /Employers/{EffectiveDate}:
    get:
      summary: Gets all employers at the specified effective date
      description: Gets links to all employers contained under the authorised application
        scope for the specified effective date.
      operationId: GetEmployersByEffectiveDate
      x-api-path-slug: employerseffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      responses:
        200:
          description: OK
      tags:
      - ""
      - Employers
      - At
      - Specified
      - Effective
      - Date
  /Healthcheck:
    get:
      summary: Get health check status
      description: Returns the health status of the application
      operationId: GetHealthCheck
      x-api-path-slug: healthcheck-get
      responses:
        200:
          description: OK
      tags:
      - Health
      - Check
      - Status
  /Jobs/Dps:
    get:
      summary: Get all DPS jobs
      description: Gets all the DPS jobs
      operationId: GetDpsJobs
      x-api-path-slug: jobsdps-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - DPJobs
    post:
      summary: Create new DPS job
      description: Creates the new DPS job to the queue and returns the job info
      operationId: PostNewDpsJob
      x-api-path-slug: jobsdps-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: DpsJobInstruction
        description: The the DPS job instruction object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - DPJob
  /Jobs/Dps/{JobId}:
    delete:
      summary: Delete the DPS job
      description: Deletes the the DPS job
      operationId: DeleteDpsJob
      x-api-path-slug: jobsdpsjobid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - DPJob
  /Jobs/Dps/{JobId}/Info:
    get:
      summary: Get the DPS job information
      description: Return the the DPS job information
      operationId: GetDpsJobInfo
      x-api-path-slug: jobsdpsjobidinfo-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - DPJob
      - Information
  /Jobs/Dps/{JobId}/Progress:
    get:
      summary: Get the DPS job progress
      description: Return the the DPS job progress
      operationId: GetDpsJobProgress
      x-api-path-slug: jobsdpsjobidprogress-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - DPJob
      - Progress
  /Jobs/Dps/{JobId}/Status:
    get:
      summary: Get the DPS job status
      description: Return the the DPS job status
      operationId: GetDpsJobStatus
      x-api-path-slug: jobsdpsjobidstatus-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - DPJob
      - Status
  /Jobs/PayRuns:
    get:
      summary: Get all PayRun jobs
      description: Gets all the pay run jobs
      operationId: GetPayRunJobs
      x-api-path-slug: jobspayruns-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - PayRun
      - Jobs
    post:
      summary: Create new PayRun job
      description: Creates the new pay run job to the queue and returns the job info
      operationId: PostNewPayRunJob
      x-api-path-slug: jobspayruns-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: PayRunJobInstruction
        description: The pay run job instruction object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - PayRun
      - Job
  /Jobs/PayRuns/{JobId}:
    delete:
      summary: Delete the pay run job
      description: Deletes the the payrun job
      operationId: DeletePayRunJob
      x-api-path-slug: jobspayrunsjobid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
  /Jobs/PayRuns/{JobId}/Info:
    get:
      summary: Get the pay run job information
      description: Return the the payrun job information
      operationId: GetPayRunJobInfo
      x-api-path-slug: jobspayrunsjobidinfo-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
      - Information
  /Jobs/PayRuns/{JobId}/Progress:
    get:
      summary: Get the pay run job progress
      description: Return the the payrun job progress
      operationId: GetPayRunJobProgress
      x-api-path-slug: jobspayrunsjobidprogress-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
      - Progress
  /Jobs/PayRuns/{JobId}/Status:
    get:
      summary: Get the pay run job status
      description: Return the the payrun job status
      operationId: GetPayRunJobStatus
      x-api-path-slug: jobspayrunsjobidstatus-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
      - Status
  /Jobs/Rti:
    get:
      summary: Get all RTI jobs
      description: Gets all the RTI jobs
      operationId: GetRtiJobs
      x-api-path-slug: jobsrti-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Jobs
    post:
      summary: Create new RTI job
      description: Creates the new RTI job to the queue and returns the job info
      operationId: PostNewRtiJob
      x-api-path-slug: jobsrti-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: RtiJobInstruction
        description: The the RTI job instruction object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - RTI
      - Job
  /Jobs/Rti/{JobId}:
    delete:
      summary: Delete the RTI job
      description: Deletes the the RTI job
      operationId: DeleteRtiJob
      x-api-path-slug: jobsrtijobid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Job
  /Jobs/Rti/{JobId}/Info:
    get:
      summary: Get the RTI job information
      description: Return the the RTI job information
      operationId: GetRtiJobInfo
      x-api-path-slug: jobsrtijobidinfo-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Job
      - Information
  /Jobs/Rti/{JobId}/Progress:
    get:
      summary: Get the RTI job progress
      description: Return the the RTI job progress
      operationId: GetRtiJobProgress
      x-api-path-slug: jobsrtijobidprogress-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Job
      - Progress
  /Jobs/Rti/{JobId}/Status:
    get:
      summary: Get the RTI job status
      description: Return the the RTI job status
      operationId: GetRtiJobStatus
      x-api-path-slug: jobsrtijobidstatus-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Job
      - Status
  /Query:
    post:
      summary: Get the query result
      description: Get the results for the specified query
      operationId: GetQueryResponse
      x-api-path-slug: query-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: Query
        description: The query object to be executed against the application data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Query
      - Result
  /Report/ACTPAYINS/run:
    get:
      summary: Runs the active pay instructions report
      description: Returns the result of the executed active pay instructions report
        for the given query parameters
      operationId: GetActivePayInstructionsReportOutput
      x-api-path-slug: reportactpayinsrun-get
      parameters:
      - in: query
        name: ActiveOn
        description: The active date to consider
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployeeKey
        description: The employee unique key
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: Type
        description: the data type to filter on
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Active
      - Pay
      - Instructions
      - Report
  /Report/DPSMSG/run:
    get:
      summary: Runs the DPS message report
      description: Returns the result of the executed DPS message report for the given
        query parameters
      operationId: GetDpsMessageReportOutput
      x-api-path-slug: reportdpsmsgrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: FromDate
        description: The lower filter date
      - in: query
        name: MessageStatuses
        description: The DPS message status as a CSV list
      - in: query
        name: MessageTypes
        description: The DPS message types as a CSV list
      - in: query
        name: ToDate
        description: The upper filter date
      responses:
        200:
          description: OK
      tags:
      - Runs
      - DPMessage
      - Report
  /Report/GRO2NET/run:
    get:
      summary: Runs the gross to net report
      description: Returns the result of the executed gross to net report for the
        given query parameters
      operationId: GetGrossToNetReportOutput
      x-api-path-slug: reportgro2netrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: PayScheduleKey
        description: The pay schedule unique key
      - in: query
        name: TaxPeriod
        description: The tax period number
      - in: query
        name: TaxYear
        description: The tax year
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Gross
      - To
      - Net
      - Report
  /Report/NETPAY/run:
    get:
      summary: Runs the net pay report
      description: Returns the result of the executed net pay report for the given
        query parameters
      operationId: GetNetPayReportOutput
      x-api-path-slug: reportnetpayrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: PayScheduleKey
        description: The pay schedule unique key
      - in: query
        name: TaxPeriod
        description: The tax period number
      - in: query
        name: TaxYear
        description: The tax year
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Net
      - Pay
      - Report
  /Report/P11SUM/run:
    get:
      summary: Runs the P11 summary report
      description: Returns the result of the executed P11 summary report for the given
        query parameters
      operationId: GetP11SummaryReportOutput
      x-api-path-slug: reportp11sumrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: PayScheduleKey
        description: The pay schedule unique key
      - in: query
        name: TaxPeriod
        description: The tax period number
      - in: query
        name: TaxYear
        description: The tax year
      responses:
        200:
          description: OK
      tags:
      - Runs
      - P11
      - Summary
      - Report
  /Report/P32/run:
    get:
      summary: Runs the P32 report
      description: Returns the result of the executed P32 report for the given query
        parameters
      operationId: GetP32NetReportOutput
      x-api-path-slug: reportp32run-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: TaxYear
        description: The tax year
      responses:
        200:
          description: OK
      tags:
      - Runs
      - P32
      - Report
  /Report/P32SUM/run:
    get:
      summary: Runs the P32 summary report
      description: Returns the result of the executed P32 summary report for the given
        query parameters
      operationId: GetP32SummaryNetReportOutput
      x-api-path-slug: reportp32sumrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: TaxYear
        description: The tax year
      responses:
        200:
          description: OK
      tags:
      - Runs
      - P32
      - Summary
      - Report
  /Report/P45/run:
    get:
      summary: Runs the P45 report
      description: Returns the result of the executed P45 report for the given query
        parameters
      operationId: GetP45ReportOutput
      x-api-path-slug: reportp45run-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployeeKey
        description: The employee unique key
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: TransformDefinitionKey
        description: The transform definition unique key
      responses:
        200:
          description: OK
      tags:
      - Runs
      - P45
      - Report
  /Report/P60/run:
    get:
      summary: Runs the P60 report
      description: Returns the result of the executed P60 report for the given query
        parameters
      operationId: GetP60ReportOutput
      x-api-path-slug: reportp60run-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployeeCodes
        description: A comma separated list of the employee codes
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: TaxYear
        description: The tax year
      - in: query
        name: TransformDefinitionKey
        description: The transform definition unique key
      responses:
        200:
          description: OK
      tags:
      - Runs
      - P60
      - Report
  /Report/PAYSLIP/run:
    get:
      summary: Runs the payslip report
      description: Returns the result of the executed payslip report for the given
        query parameters
      operationId: GetPayslipReportOutput
      x-api-path-slug: reportpaysliprun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployeeCodes
        description: A comma separated list of the employee codes
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: TaxPeriod
        description: The tax period number
      - in: query
        name: TaxYear
        description: The tax year
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Payslip
      - Report
  /Report/PENLIABILITY/run:
    get:
      summary: Runs the pension liability report
      description: Returns the result of the executed pension liability report for
        the given query parameters
      operationId: GetPensionLiabilityReportOutput
      x-api-path-slug: reportpenliabilityrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: query
        name: EmployerKey
        description: The employer unique key
      - in: query
        name: PensionKey
        description: The pension scheme unique key
      - in: query
        name: TaxYear
        description: The tax year
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Pension
      - Liability
      - Report
  /Report/{ReportDefinitionId}:
    delete:
      summary: Deletes a report definition
      description: Delete the specified report definition
      operationId: DeleteReportDefinition
      x-api-path-slug: reportreportdefinitionid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: ReportDefinitionId
        description: The report definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Report
      - Definition
    get:
      summary: Get the report definition
      description: Returns the specified report definition from the authroised application
      operationId: GetReportDefinitionFromApplication
      x-api-path-slug: reportreportdefinitionid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: ReportDefinitionId
        description: The report definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Report
      - Definition
    put:
      summary: Updates a report definition
      description: Updates the existing specified report definition object
      operationId: PutReportDefinition
      x-api-path-slug: reportreportdefinitionid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: ReportDefinition
        description: The report definition object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: ReportDefinitionId
        description: The report definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Report
      - Definition
  /Report/{ReportDefinitionId}/run:
    get:
      summary: Runs the specified report definition
      description: Returns the result of the executed report definition
      operationId: GetReportOutput
      x-api-path-slug: reportreportdefinitionidrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: ReportDefinitionId
        description: The report definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Specified
      - Report
      - Definition
  /Reports:
    get:
      summary: Gets all reports
      description: Get links to all saved report definitions under authorised application
      operationId: GetReportDefinitionsFromApplication
      x-api-path-slug: reports-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - ""
      - Reports
    post:
      summary: Create a new report definition
      description: Creates a new report defintion object
      operationId: PostReportDefinition
      x-api-path-slug: reports-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: ReportDefinition
        description: The report definition object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Report
      - Definition
  /Schemas:
    get:
      summary: Get a list of all available schemas
      description: Returns a collection of links to all the available data object
        schemas
      operationId: GetSchemas
      x-api-path-slug: schemas-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - Available
      - Schemas
  /Schemas/AbsencePayInstruction.xsd:
    get:
      summary: Get the AbsencePayInstruction schema
      description: Returns the AbsencePayInstruction schema object
      operationId: GetAbsencePayInstructionSchema
      x-api-path-slug: schemasabsencepayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - AbsencePayInstruction
      - Schema
  /Schemas/AbsenceYtdPayInstruction.xsd:
    get:
      summary: Get the AbsenceYtdPayInstruction schema
      description: Returns the AbsenceYtdPayInstruction schema object
      operationId: GetAbsenceYtdPayInstructionSchema
      x-api-path-slug: schemasabsenceytdpayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - AbsenceYtdPayInstruction
      - Schema
  /Schemas/Address.xsd:
    get:
      summary: Get the Address schema
      description: Returns the Address schema object
      operationId: GetAddressSchema
      x-api-path-slug: schemasaddress-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Ress
      - Schema
  /Schemas/ArrayOfEmployee.xsd:
    get:
      summary: Get the ArrayOfEmployee schema
      description: Returns the ArrayOfEmployee schema object
      operationId: GetArrayOfEmployeeSchema
      x-api-path-slug: schemasarrayofemployee-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - ArrayOfEmployee
      - Schema
  /Schemas/BankAccount.xsd:
    get:
      summary: Get the BankAccount schema
      description: Returns the BankAccount schema object
      operationId: GetBankAccountSchema
      x-api-path-slug: schemasbankaccount-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - BankAccount
      - Schema
  /Schemas/BenefitPayInstruction.xsd:
    get:
      summary: Get the BenefitPayInstruction schema
      description: Returns the BenefitPayInstruction schema object
      operationId: GetBenefitPayInstructionSchema
      x-api-path-slug: schemasbenefitpayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - BenefitPayInstruction
      - Schema
  /Schemas/BenefitYtdPayInstruction.xsd:
    get:
      summary: Get the BenefitYtdPayInstruction schema
      description: Returns the BenefitYtdPayInstruction schema object
      operationId: GetBenefitYtdPayInstructionSchema
      x-api-path-slug: schemasbenefitytdpayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - BenefitYtdPayInstruction
      - Schema
  /Schemas/Common.xsd:
    get:
      summary: Get the Common schema
      description: Returns the Common schema object
      operationId: GetCommonSchema
      x-api-path-slug: schemascommon-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Common
      - Schema
  /Schemas/Employee.xsd:
    get:
      summary: Get the Employee schema
      description: Returns the Employee schema object
      operationId: GetEmployeeSchema
      x-api-path-slug: schemasemployee-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Employee
      - Schema
  /Schemas/EmployeePartner.xsd:
    get:
      summary: Get the EmployeePartner schema
      description: Returns the EmployeePartner schema object
      operationId: GetEmployeePartnerSchema
      x-api-path-slug: schemasemployeepartner-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - EmployeePartner
      - Schema
  /Schemas/Employer.xsd:
    get:
      summary: Get the Employer schema
      description: Returns the Employer schema object
      operationId: GetEmployerSchema
      x-api-path-slug: schemasemployer-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Employer
      - Schema
  /Schemas/HmrcSettings.xsd:
    get:
      summary: Get the HmrcSettings schema
      description: Returns the HmrcSettings schema object
      operationId: GetHmrcSettingsSchema
      x-api-path-slug: schemashmrcsettings-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - HmrcSettings
      - Schema
  /Schemas/Link.xsd:
    get:
      summary: Get the Link schema
      description: Returns the Link schema object
      operationId: GetLinkSchema
      x-api-path-slug: schemaslink-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Link
      - Schema
  /Schemas/NiAdjustmentPayInstruction.xsd:
    get:
      summary: Get the NiAdjustmentPayInstruction schema
      description: Returns the NiAdjustmentPayInstruction schema object
      operationId: GetNiAdjustmentPayInstructionSchema
      x-api-path-slug: schemasniadjustmentpayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - NiAdjustmentPayInstruction
      - Schema
  /Schemas/NiPayInstruction.xsd:
    get:
      summary: Get the NiPayInstruction schema
      description: Returns the NiPayInstruction schema object
      operationId: GetNiPayInstructionSchema
      x-api-path-slug: schemasnipayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - NiPayInstruction
      - Schema
  /Schemas/NiYtdPayInstruction.xsd:
    get:
      summary: Get the NiYtdPayInstruction schema
      description: Returns the NiYtdPayInstruction schema object
      operationId: GetNiYtdPayInstructionSchema
      x-api-path-slug: schemasniytdpayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - NiYtdPayInstruction
      - Schema
  /Schemas/P45PayInstruction.xsd:
    get:
      summary: Get the P45PayInstruction schema
      description: Returns the P45PayInstruction schema object
      operationId: GetP45PayInstructionSchema
      x-api-path-slug: schemasp45payinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - P45PayInstruction
      - Schema
  /Schemas/PayInstruction.xsd:
    get:
      summary: Get the PayInstruction schema
      description: Returns the PayInstruction schema object
      operationId: GetPayInstructionSchema
      x-api-path-slug: schemaspayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - PayInstruction
      - Schema
  /Schemas/PayRunJobInstruction.xsd:
    get:
      summary: Get the PayRunJobInstruction schema
      description: Returns the PayRunJobInstruction schema object
      operationId: GetPayRunJobInstructionSchema
      x-api-path-slug: schemaspayrunjobinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - PayRunJobInstruction
      - Schema
  /Schemas/PaySchedule.xsd:
    get:
      summary: Get the PaySchedule schema
      description: Returns the PaySchedule schema object
      operationId: GetPayScheduleSchema
      x-api-path-slug: schemaspayschedule-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - PaySchedule
      - Schema
  /Schemas/PensionPayInstruction.xsd:
    get:
      summary: Get the PensionPayInstruction schema
      description: Returns the PensionPayInstruction schema object
      operationId: GetPensionPayInstructionSchema
      x-api-path-slug: schemaspensionpayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - PensionPayInstruction
      - Schema
  /Schemas/PensionYtdPayInstruction.xsd:
    get:
      summary: Get the PensionYtdPayInstruction schema
      description: Returns the PensionYtdPayInstruction schema object
      operationId: GetPensionYtdPayInstructionSchema
      x-api-path-slug: schemaspensionytdpayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - PensionYtdPayInstruction
      - Schema
  /Schemas/PrimitivePayInstruction.xsd:
    get:
      summary: Get the PrimitivePayInstruction schema
      description: Returns the PrimitivePayInstruction schema object
      operationId: GetPrimitivePayInstructionSchema
      x-api-path-slug: schemasprimitivepayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - PrimitivePayInstruction
      - Schema
  /Schemas/RtiJobInstruction.xsd:
    get:
      summary: Get the RtiJobInstruction schema
      description: Returns the RtiJobInstruction schema object
      operationId: GetRtiJobInstructionSchema
      x-api-path-slug: schemasrtijobinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - RtiJobInstruction
      - Schema
  /Schemas/SalaryPayInstruction.xsd:
    get:
      summary: Get the SalaryPayInstruction schema
      description: Returns the SalaryPayInstruction schema object
      operationId: GetSalaryPayInstructionSchema
      x-api-path-slug: schemassalarypayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - SalaryPayInstruction
      - Schema
  /Schemas/SapPayInstruction.xsd:
    get:
      summary: Get the SapPayInstruction schema
      description: Returns the SapPayInstruction schema object
      operationId: GetSapPayInstructionSchema
      x-api-path-slug: schemassappayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - SapPayInstruction
      - Schema
  /Schemas/SapYtdPayInstruction.xsd:
    get:
      summary: Get the SapYtdPayInstruction schema
      description: Returns the SapYtdPayInstruction schema object
      operationId: GetSapYtdPayInstructionSchema
      x-api-path-slug: schemassapytdpayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - SapYtdPayInstruction
      - Schema
  /Schemas/ShppPayInstruction.xsd:
    get:
      summary: Get the ShppPayInstruction schema
      description: Returns the ShppPayInstruction schema object
      operationId: GetShppPayInstructionSchema
      x-api-path-slug: schemasshpppayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - ShppPayInstruction
      - Schema
  /Schemas/ShppYtdPayInstruction.xsd:
    get:
      summary: Get the ShppYtdPayInstruction schema
      description: Returns the ShppYtdPayInstruction schema object
      operationId: GetShppYtdPayInstructionSchema
      x-api-path-slug: schemasshppytdpayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - ShppYtdPayInstruction
      - Schema
  /Schemas/SmpPayInstruction.xsd:
    get:
      summary: Get the SmpPayInstruction schema
      description: Returns the SmpPayInstruction schema object
      operationId: GetSmpPayInstructionSchema
      x-api-path-slug: schemassmppayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - SmpPayInstruction
      - Schema
  /Schemas/SmpYtdPayInstruction.xsd:
    get:
      summary: Get the SmpYtdPayInstruction schema
      description: Returns the SmpYtdPayInstruction schema object
      operationId: GetSmpYtdPayInstructionSchema
      x-api-path-slug: schemassmpytdpayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - SmpYtdPayInstruction
      - Schema
  /Schemas/SppPayInstruction.xsd:
    get:
      summary: Get the SppPayInstruction schema
      description: Returns the SppPayInstruction schema object
      operationId: GetSppPayInstructionSchema
      x-api-path-slug: schemasspppayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - SppPayInstruction
      - Schema
  /Schemas/SppYtdPayInstruction.xsd:
    get:
      summary: Get the SppYtdPayInstruction schema
      description: Returns the SppYtdPayInstruction schema object
      operationId: GetSppYtdPayInstructionSchema
      x-api-path-slug: schemassppytdpayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - SppYtdPayInstruction
      - Schema
  /Schemas/SspPayInstruction.xsd:
    get:
      summary: Get the SspPayInstruction schema
      description: Returns the SspPayInstruction schema object
      operationId: GetSspPayInstructionSchema
      x-api-path-slug: schemasssppayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - SspPayInstruction
      - Schema
  /Schemas/SspYtdPayInstruction.xsd:
    get:
      summary: Get the SspYtdPayInstruction schema
      description: Returns the SspYtdPayInstruction schema object
      operationId: GetSspYtdPayInstructionSchema
      x-api-path-slug: schemassspytdpayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - SspYtdPayInstruction
      - Schema
  /Schemas/StudentLoanPayInstruction.xsd:
    get:
      summary: Get the StudentLoanPayInstruction schema
      description: Returns the StudentLoanPayInstruction schema object
      operationId: GetStudentLoanPayInstructionSchema
      x-api-path-slug: schemasstudentloanpayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - StudentLoanPayInstruction
      - Schema
  /Schemas/StudentLoanYtdPayInstruction.xsd:
    get:
      summary: Get the StudentLoanYtdPayInstruction schema
      description: Returns the StudentLoanYtdPayInstruction schema object
      operationId: GetStudentLoanYtdPayInstructionSchema
      x-api-path-slug: schemasstudentloanytdpayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - StudentLoanYtdPayInstruction
      - Schema
  /Schemas/TaxPayInstruction.xsd:
    get:
      summary: Get the TaxPayInstruction schema
      description: Returns the TaxPayInstruction schema object
      operationId: GetTaxPayInstructionSchema
      x-api-path-slug: schemastaxpayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - TaxPayInstruction
      - Schema
  /Schemas/TaxYtdPayInstruction.xsd:
    get:
      summary: Get the TaxYtdPayInstruction schema
      description: Returns the TaxYtdPayInstruction schema object
      operationId: GetTaxYtdPayInstructionSchema
      x-api-path-slug: schemastaxytdpayinstruction-xsd-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - TaxYtdPayInstruction
      - Schema
  /Templates:
    get:
      summary: Get a list of all available data object tempaltes
      description: Returns a collection of links to all the available data object
        templates
      operationId: GetTemplates
      x-api-path-slug: templates-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - Available
      - Data
      - Object
      - Tempaltes
  /Templates/address:
    get:
      summary: Gets the address template
      description: Return the address data object template
      operationId: GetAddressTemplate
      x-api-path-slug: templatesaddress-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Address
      - Template
  /Templates/applicationinfo:
    get:
      summary: Gets the application info template
      description: Return the application info data object template
      operationId: GetApplicationInfoTemplate
      x-api-path-slug: templatesapplicationinfo-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Application
      - Info
      - Template
  /Templates/bankaccount:
    get:
      summary: Gets the bank account template
      description: Return the bank account data object template
      operationId: GetBankAccountTemplate
      x-api-path-slug: templatesbankaccount-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Bank
      - Account
      - Template
  /Templates/benefitpayinstruction:
    get:
      summary: Gets the benefit pay instruction template
      description: Return the benefit pay instruction data object template
      operationId: GetBenefitPayInstructionTemplate
      x-api-path-slug: templatesbenefitpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Benefit
      - Pay
      - Instruction
      - Template
  /Templates/benefitytdpayinstruction:
    get:
      summary: Gets the benefit YTD pay instruction template
      description: Return the benefit YTD pay instruction data object template
      operationId: GetBenefitYtdPayInstructionTemplate
      x-api-path-slug: templatesbenefitytdpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Benefit
      - YTD
      - Pay
      - Instruction
      - Template
  /Templates/commentary:
    get:
      summary: Gets the commentary template
      description: Return the commentary data object template
      operationId: GetCommentaryTemplate
      x-api-path-slug: templatescommentary-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Commentary
      - Template
  /Templates/employee:
    get:
      summary: Gets the employee template
      description: Return the employee data object template
      operationId: GetEmployeeTemplate
      x-api-path-slug: templatesemployee-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Employee
      - Template
  /Templates/employeepartner:
    get:
      summary: Gets the employee partner template
      description: Return the employee partner data object template
      operationId: GetEmployeePartnerTemplate
      x-api-path-slug: templatesemployeepartner-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Employee
      - Partner
      - Template
  /Templates/employer:
    get:
      summary: Gets the employer template
      description: Return the employer data object template
      operationId: GetEmployerTemplate
      x-api-path-slug: templatesemployer-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Employer
      - Template
  /Templates/errormodel:
    get:
      summary: Gets the error model template
      description: Return the error model data object template
      operationId: GetErrorModelTemplate
      x-api-path-slug: templateserrormodel-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Error
      - Model
      - Template
  /Templates/hmrcsettings:
    get:
      summary: Gets the hmrc settings template
      description: Return the hmrc settings data object template
      operationId: GetHmrcSettingsTemplate
      x-api-path-slug: templateshmrcsettings-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Hmrc
      - Settings
      - Template
  /Templates/jobinfo:
    get:
      summary: Gets the job info template
      description: Return the job info data object template
      operationId: GetJobInfoTemplate
      x-api-path-slug: templatesjobinfo-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Job
      - Info
      - Template
  /Templates/link:
    get:
      summary: Gets the link template
      description: Return the link data object template
      operationId: GetLinkTemplate
      x-api-path-slug: templateslink-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Link
      - Template
  /Templates/linkcollection:
    get:
      summary: Gets the link collection template
      description: Return the link collection data object template
      operationId: GetLinkCollectionTemplate
      x-api-path-slug: templateslinkcollection-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Link
      - Collection
      - Template
  /Templates/niadjustmentpayinstruction:
    get:
      summary: Gets the NI adjustment pay instruction template
      description: Return the NI adjustment pay instruction data object template
      operationId: GetNiAdjustmentPayInstructionTemplate
      x-api-path-slug: templatesniadjustmentpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - NI
      - Adjustment
      - Pay
      - Instruction
      - Template
  /Templates/nipayinstruction:
    get:
      summary: Gets the NI pay instruction template
      description: Return the NI pay instruction data object template
      operationId: GetNiPayInstructionTemplate
      x-api-path-slug: templatesnipayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - NI
      - Pay
      - Instruction
      - Template
  /Templates/niytdpayinstruction:
    get:
      summary: Gets the NI YTD pay instruction template
      description: Return the NI YTD pay instruction data object template
      operationId: GetNiYtdPayInstructionTemplate
      x-api-path-slug: templatesniytdpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - NI
      - YTD
      - Pay
      - Instruction
      - Template
  /Templates/p45payinstruction:
    get:
      summary: Gets the P45 pay instruction template
      description: Return the P45 pay instruction data object template
      operationId: GetP45PayInstructionTemplate
      x-api-path-slug: templatesp45payinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - P45
      - Pay
      - Instruction
      - Template
  /Templates/paycode:
    get:
      summary: Gets the pay code template
      description: Return the pay code data object template
      operationId: GetPayCodeTemplate
      x-api-path-slug: templatespaycode-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Code
      - Template
  /Templates/payinstruction:
    get:
      summary: Gets the pay instruction template
      description: Return the pay instruction data object template
      operationId: GetPayInstructionTemplate
      x-api-path-slug: templatespayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Instruction
      - Template
  /Templates/payline:
    get:
      summary: Gets the pay line template
      description: Return the pay line data object template
      operationId: GetPayLineTemplate
      x-api-path-slug: templatespayline-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Line
      - Template
  /Templates/paylinebenefit:
    get:
      summary: Gets the pay line benefit template
      description: Return the pay line benefit data object template
      operationId: GetPayLineBenefitTemplate
      x-api-path-slug: templatespaylinebenefit-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Line
      - Benefit
      - Template
  /Templates/paylineni:
    get:
      summary: Gets the pay line NI template
      description: Return the pay line NI data object template
      operationId: GetPayLineNiTemplate
      x-api-path-slug: templatespaylineni-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Line
      - NI
      - Template
  /Templates/paylinepension:
    get:
      summary: Gets the pay line pension template
      description: Return the pay line pension data object template
      operationId: GetPayLinePensionTemplate
      x-api-path-slug: templatespaylinepension-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Line
      - Pension
      - Template
  /Templates/paylinesap:
    get:
      summary: Gets the pay line sap template
      description: Return the pay line sap data object template
      operationId: GetPayLineSapTemplate
      x-api-path-slug: templatespaylinesap-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Line
      - Sap
      - Template
  /Templates/paylineshpp:
    get:
      summary: Gets the pay line shpp template
      description: Return the pay line shpp data object template
      operationId: GetPayLineShppTemplate
      x-api-path-slug: templatespaylineshpp-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Line
      - Shpp
      - Template
  /Templates/paylinesmp:
    get:
      summary: Gets the pay line smp template
      description: Return the pay line smp data object template
      operationId: GetPayLineSmpTemplate
      x-api-path-slug: templatespaylinesmp-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Line
      - Smp
      - Template
  /Templates/paylinespp:
    get:
      summary: Gets the pay line spp template
      description: Return the pay line spp data object template
      operationId: GetPayLineSppTemplate
      x-api-path-slug: templatespaylinespp-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Line
      - Spp
      - Template
  /Templates/paylinessp:
    get:
      summary: Gets the pay line ssp template
      description: Return the pay line ssp data object template
      operationId: GetPayLineSspTemplate
      x-api-path-slug: templatespaylinessp-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Line
      - Ssp
      - Template
  /Templates/paylinestudentloan:
    get:
      summary: Gets the pay line student loan template
      description: Return the pay line student loan data object template
      operationId: GetPayLineStudentLoanTemplate
      x-api-path-slug: templatespaylinestudentloan-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Line
      - Student
      - Loan
      - Template
  /Templates/paylinetax:
    get:
      summary: Gets the pay line tax template
      description: Return the pay line tax data object template
      operationId: GetPayLineTaxTemplate
      x-api-path-slug: templatespaylinetax-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Line
      - Tax
      - Template
  /Templates/payrun:
    get:
      summary: Gets the pay run template
      description: Return the pay run data object template
      operationId: GetPayRunTemplate
      x-api-path-slug: templatespayrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Template
  /Templates/payrunjob:
    get:
      summary: Gets the pay run job template
      description: Return the pay run job data object template
      operationId: GetPayRunJobTemplate
      x-api-path-slug: templatespayrunjob-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
      - Template
  /Templates/payrunjobinstruction:
    get:
      summary: Gets the pay run job instruction template
      description: Return the pay run job instruction data object template
      operationId: GetPayRunJobInstructionTemplate
      x-api-path-slug: templatespayrunjobinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
      - Instruction
      - Template
  /Templates/payschedule:
    get:
      summary: Gets the pay schedule template
      description: Return the pay schedule data object template
      operationId: GetPayScheduleTemplate
      x-api-path-slug: templatespayschedule-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Schedule
      - Template
  /Templates/pensionpayinstruction:
    get:
      summary: Gets the pension pay instruction template
      description: Return the pension pay instruction data object template
      operationId: GetPensionPayInstructionTemplate
      x-api-path-slug: templatespensionpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pension
      - Pay
      - Instruction
      - Template
  /Templates/pensionytdpayinstruction:
    get:
      summary: Gets the pension YTD pay instruction template
      description: Return the pension YTD pay instruction data object template
      operationId: GetPensionYtdPayInstructionTemplate
      x-api-path-slug: templatespensionytdpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pension
      - YTD
      - Pay
      - Instruction
      - Template
  /Templates/primitivepayinstruction:
    get:
      summary: Gets the primitive pay instruction template
      description: Return the primitive pay instruction data object template
      operationId: GetPrimitivePayInstructionTemplate
      x-api-path-slug: templatesprimitivepayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Primitive
      - Pay
      - Instruction
      - Template
  /Templates/reportdefinition:
    get:
      summary: Gets the report definition template
      description: Return the report definition data object template
      operationId: GetReportDefinitionTemplate
      x-api-path-slug: templatesreportdefinition-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Report
      - Definition
      - Template
  /Templates/rtieastransaction:
    get:
      summary: Gets the rti eas transaction template
      description: Return the rti eas transaction data object template
      operationId: GetRtiEasTransactionTemplate
      x-api-path-slug: templatesrtieastransaction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Eas
      - Transaction
      - Template
  /Templates/rtiepstransaction:
    get:
      summary: Gets the rti eps transaction template
      description: Return the rti eps transaction data object template
      operationId: GetRtiEpsTransactionTemplate
      x-api-path-slug: templatesrtiepstransaction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Eps
      - Transaction
      - Template
  /Templates/rtieyutransaction:
    get:
      summary: Gets the rti eyu transaction template
      description: Return the rti eyu transaction data object template
      operationId: GetRtiEyuTransactionTemplate
      x-api-path-slug: templatesrtieyutransaction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Eyu
      - Transaction
      - Template
  /Templates/rtifpstransaction:
    get:
      summary: Gets the rti fps transaction template
      description: Return the rti fps transaction data object template
      operationId: GetRtiFpsTransactionTemplate
      x-api-path-slug: templatesrtifpstransaction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Fps
      - Transaction
      - Template
  /Templates/rtijob:
    get:
      summary: Gets the rti job template
      description: Return the rti job data object template
      operationId: GetRtiJobTemplate
      x-api-path-slug: templatesrtijob-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Job
      - Template
  /Templates/rtijobinstruction:
    get:
      summary: Gets the rti job instruction template
      description: Return the rti job instruction data object template
      operationId: GetRtiJobInstructionTemplate
      x-api-path-slug: templatesrtijobinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Job
      - Instruction
      - Template
  /Templates/rtinvrtransaction:
    get:
      summary: Gets the rti nvr transaction template
      description: Return the rti nvr transaction data object template
      operationId: GetRtiNvrTransactionTemplate
      x-api-path-slug: templatesrtinvrtransaction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Nvr
      - Transaction
      - Template
  /Templates/rtitransactionbase:
    get:
      summary: Gets the rti transaction base template
      description: Return the rti transaction base data object template
      operationId: GetRtiTransactionBaseTemplate
      x-api-path-slug: templatesrtitransactionbase-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Rti
      - Transaction
      - Base
      - Template
  /Templates/salarypayinstruction:
    get:
      summary: Gets the salary pay instruction template
      description: Return the salary pay instruction data object template
      operationId: GetSalaryPayInstructionTemplate
      x-api-path-slug: templatessalarypayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Salary
      - Pay
      - Instruction
      - Template
  /Templates/sappayinstruction:
    get:
      summary: Gets the sap pay instruction template
      description: Return the sap pay instruction data object template
      operationId: GetSapPayInstructionTemplate
      x-api-path-slug: templatessappayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Sap
      - Pay
      - Instruction
      - Template
  /Templates/sapytdpayinstruction:
    get:
      summary: Gets the sap YTD pay instruction template
      description: Return the sap YTD pay instruction data object template
      operationId: GetSapYtdPayInstructionTemplate
      x-api-path-slug: templatessapytdpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Sap
      - YTD
      - Pay
      - Instruction
      - Template
  /Templates/shpppayinstruction:
    get:
      summary: Gets the shpp pay instruction template
      description: Return the shpp pay instruction data object template
      operationId: GetShppPayInstructionTemplate
      x-api-path-slug: templatesshpppayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Shpp
      - Pay
      - Instruction
      - Template
  /Templates/shppytdpayinstruction:
    get:
      summary: Gets the shpp YTD pay instruction template
      description: Return the shpp YTD pay instruction data object template
      operationId: GetShppYtdPayInstructionTemplate
      x-api-path-slug: templatesshppytdpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Shpp
      - YTD
      - Pay
      - Instruction
      - Template
  /Templates/smppayinstruction:
    get:
      summary: Gets the smp pay instruction template
      description: Return the smp pay instruction data object template
      operationId: GetSmpPayInstructionTemplate
      x-api-path-slug: templatessmppayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Smp
      - Pay
      - Instruction
      - Template
  /Templates/smpytdpayinstruction:
    get:
      summary: Gets the smp YTD pay instruction template
      description: Return the smp YTD pay instruction data object template
      operationId: GetSmpYtdPayInstructionTemplate
      x-api-path-slug: templatessmpytdpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Smp
      - YTD
      - Pay
      - Instruction
      - Template
  /Templates/spppayinstruction:
    get:
      summary: Gets the spp pay instruction template
      description: Return the spp pay instruction data object template
      operationId: GetSppPayInstructionTemplate
      x-api-path-slug: templatesspppayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Spp
      - Pay
      - Instruction
      - Template
  /Templates/sppytdpayinstruction:
    get:
      summary: Gets the spp YTD pay instruction template
      description: Return the spp YTD pay instruction data object template
      operationId: GetSppYtdPayInstructionTemplate
      x-api-path-slug: templatessppytdpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Spp
      - YTD
      - Pay
      - Instruction
      - Template
  /Templates/ssppayinstruction:
    get:
      summary: Gets the ssp pay instruction template
      description: Return the ssp pay instruction data object template
      operationId: GetSspPayInstructionTemplate
      x-api-path-slug: templatesssppayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Ssp
      - Pay
      - Instruction
      - Template
  /Templates/sspytdpayinstruction:
    get:
      summary: Gets the ssp YTD pay instruction template
      description: Return the ssp YTD pay instruction data object template
      operationId: GetSspYtdPayInstructionTemplate
      x-api-path-slug: templatessspytdpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Ssp
      - YTD
      - Pay
      - Instruction
      - Template
  /Templates/studentloanpayinstruction:
    get:
      summary: Gets the student loan pay instruction template
      description: Return the student loan pay instruction data object template
      operationId: GetStudentLoanPayInstructionTemplate
      x-api-path-slug: templatesstudentloanpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Student
      - Loan
      - Pay
      - Instruction
      - Template
  /Templates/studentloanytdpayinstruction:
    get:
      summary: Gets the student loan YTD pay instruction template
      description: Return the student loan YTD pay instruction data object template
      operationId: GetStudentLoanYtdPayInstructionTemplate
      x-api-path-slug: templatesstudentloanytdpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Student
      - Loan
      - YTD
      - Pay
      - Instruction
      - Template
  /Templates/taxpayinstruction:
    get:
      summary: Gets the tax pay instruction template
      description: Return the tax pay instruction data object template
      operationId: GetTaxPayInstructionTemplate
      x-api-path-slug: templatestaxpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Tax
      - Pay
      - Instruction
      - Template
  /Templates/taxytdpayinstruction:
    get:
      summary: Gets the tax YTD pay instruction template
      description: Return the tax YTD pay instruction data object template
      operationId: GetTaxYtdPayInstructionTemplate
      x-api-path-slug: templatestaxytdpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Tax
      - YTD
      - Pay
      - Instruction
      - Template
  /Transform/{TransformDefinitionId}:
    delete:
      summary: Deletes a transform definition
      description: Delete the specified transform definition
      operationId: DeleteTransformDefinition
      x-api-path-slug: transformtransformdefinitionid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: TransformDefinitionId
        description: The transform definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Transform
      - Definition
    get:
      summary: Get the transform definition
      description: Returns the specified transform definition from the authroised
        application
      operationId: GetTransformDefinitionFromApplication
      x-api-path-slug: transformtransformdefinitionid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: TransformDefinitionId
        description: The transform definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Transform
      - Definition
    put:
      summary: Updates a transform definition
      description: Updates the existing specified transform definition object
      operationId: PutTransformDefinition
      x-api-path-slug: transformtransformdefinitionid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: TransformDefinition
        description: The transform definition object to be executed against the report
          data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: TransformDefinitionId
        description: The transform definition unique identifier
      responses:
        200:
          description: OK
      tags:
      - Transform
      - Definition
  /Transforms:
    get:
      summary: Gets all transform definitions
      description: Get links to all saved transform definitions under authorised application
      operationId: GetTransformDefinitionsFromApplication
      x-api-path-slug: transforms-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - ""
      - Transform
      - Definitions
    post:
      summary: Create a new transform definition
      description: Creates a new transform defintion object
      operationId: PostTransformDefinition
      x-api-path-slug: transforms-post
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: body
        name: TransformDefinition
        description: The transform definition object to be executed against the report
          data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Transform
      - Definition