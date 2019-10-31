swagger: "2.0"
x-collection-name: AWS WAF
x-complete: 1
info:
  title: AWS WAF API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AssociateWebACL:
    get:
      summary: Associate Web ACL
      description: 'Service: AWS WAF RegionalAssociates a web ACL with a resource.'
      operationId: associateWebACL
      x-api-path-slug: actionassociatewebacl-get
      parameters:
      - in: query
        name: ResourceArn
        description: The ARN (Amazon Resource Name) of the resource to be protected
        type: string
      - in: query
        name: WebACLId
        description: A unique identifier (ID) for the web ACL
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
  /?Action=CreateByteMatchSet:
    get:
      summary: Create Byte Match Set
      description: 'Service: AWS WAFCreates a ByteMatchSet.'
      operationId: createByteMatchSet
      x-api-path-slug: actioncreatebytematchset-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: Name
        description: A friendly name or description of the ByteMatchSet
        type: string
      responses:
        200:
          description: OK
      tags:
      - Byte Match Set
  /?Action=CreateIPSet:
    get:
      summary: Create IP Set
      description: 'Service: AWS WAFCreates an.'
      operationId: createIPSet
      x-api-path-slug: actioncreateipset-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: Name
        description: A friendly name or description of the IPSet
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Sets
  /?Action=CreateRule:
    get:
      summary: Create Rule
      description: "Service: AWS WAFCreates a Rule, which contains the IPSet objects,
        ByteMatchSet objects, and \n\t\t\tother predicates that identify the requests
        that you want to block."
      operationId: createRule
      x-api-path-slug: actioncreaterule-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: MetricName
        description: A friendly name or description for the metrics for this Rule
        type: string
      - in: query
        name: Name
        description: A friendly name or description of the Rule
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rules
  /?Action=CreateSizeConstraintSet:
    get:
      summary: Create Size Constraint Set
      description: 'Service: AWS WAFCreates a SizeConstraintSet.'
      operationId: createSizeConstraintSet
      x-api-path-slug: actioncreatesizeconstraintset-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: Name
        description: A friendly name or description of the SizeConstraintSet
        type: string
      responses:
        200:
          description: OK
      tags:
      - Size Constraint Set
  /?Action=CreateSqlInjectionMatchSet:
    get:
      summary: Create Sql Injection Match Set
      description: 'Service: AWS WAFCreates a.'
      operationId: createSqlInjectionMatchSet
      x-api-path-slug: actioncreatesqlinjectionmatchset-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: Name
        description: A friendly name or description for the SqlInjectionMatchSet that
          youre creating
        type: string
      responses:
        200:
          description: OK
      tags:
      - SQL Injection Match Set
  /?Action=CreateWebACL:
    get:
      summary: Create Web ACL
      description: 'Service: AWS WAFCreates a WebACL, which contains the Rules that
        identify the CloudFront web requests that you want to allow, block, or count.'
      operationId: createWebACL
      x-api-path-slug: actioncreatewebacl-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: DefaultAction
        description: The action that you want  AWS WAF to take when a request doesnt
          match the criteria specified in any of the Rule objects that are associated
          with the WebACL
        type: string
      - in: query
        name: MetricName
        description: A friendly name or description for the metrics for this WebACL
        type: string
      - in: query
        name: Name
        description: A friendly name or description of the WebACL
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
  /?Action=CreateXssMatchSet:
    get:
      summary: Create XSS Match Set
      description: 'Service: AWS WAFCreates an.'
      operationId: createXssMatchSet
      x-api-path-slug: actioncreatexssmatchset-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: Name
        description: A friendly name or description for the XssMatchSet that youre
          creating
        type: string
      responses:
        200:
          description: OK
      tags:
      - XSS Match Set
  /?Action=DeleteByteMatchSet:
    get:
      summary: Delete Byte Match Set
      description: 'Service: AWS WAFPermanently deletes a.'
      operationId: deleteByteMatchSet
      x-api-path-slug: actiondeletebytematchset-get
      parameters:
      - in: query
        name: ByteMatchSetId
        description: The ByteMatchSetId of the ByteMatchSet that you want to delete
        type: string
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      responses:
        200:
          description: OK
      tags:
      - Byte Match Set
  /?Action=DeleteIPSet:
    get:
      summary: Delete IP Set
      description: 'Service: AWS WAFPermanently deletes an.'
      operationId: deleteIPSet
      x-api-path-slug: actiondeleteipset-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: IPSetId
        description: The IPSetId of the IPSet that you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Sets
  /?Action=DeleteRule:
    get:
      summary: Delete Rule
      description: 'Service: AWS WAFPermanently deletes a.'
      operationId: deleteRule
      x-api-path-slug: actiondeleterule-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: RuleId
        description: The RuleId of the Rule that you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rules
  /?Action=DeleteSizeConstraintSet:
    get:
      summary: Delete Size Constraint Set
      description: 'Service: AWS WAFPermanently deletes a.'
      operationId: deleteSizeConstraintSet
      x-api-path-slug: actiondeletesizeconstraintset-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: SizeConstraintSetId
        description: The SizeConstraintSetId of the SizeConstraintSet that you want
          to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Size Constraint Set
  /?Action=DeleteSqlInjectionMatchSet:
    get:
      summary: Delete Sql Injection Match Set
      description: 'Service: AWS WAFPermanently deletes a.'
      operationId: deleteSqlInjectionMatchSet
      x-api-path-slug: actiondeletesqlinjectionmatchset-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: SqlInjectionMatchSetId
        description: The SqlInjectionMatchSetId of the SqlInjectionMatchSet that you
          want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - SQL Injection Match Set
  /?Action=DeleteWebACL:
    get:
      summary: Delete Web ACL
      description: 'Service: AWS WAFPermanently deletes a.'
      operationId: deleteWebACL
      x-api-path-slug: actiondeletewebacl-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: WebACLId
        description: The WebACLId of the WebACL that you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
  /?Action=DeleteXssMatchSet:
    get:
      summary: Delete Xss Match Set
      description: 'Service: AWS WAFPermanently deletes an.'
      operationId: deleteXssMatchSet
      x-api-path-slug: actiondeletexssmatchset-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: XssMatchSetId
        description: The XssMatchSetId of the XssMatchSet that you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - XSS Match Set
  /?Action=DisassociateWebACL:
    get:
      summary: Disassociate Web ACL
      description: 'Service: AWS WAF RegionalRemoves a web ACL from the specified
        resource.'
      operationId: disassociateWebACL
      x-api-path-slug: actiondisassociatewebacl-get
      parameters:
      - in: query
        name: ResourceArn
        description: The ARN (Amazon Resource Name) of the resource from which the
          web ACL is being removed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
  /?Action=GetByteMatchSet:
    get:
      summary: Get Byte Match Set
      description: 'Service: AWS WAFReturns the.'
      operationId: getByteMatchSet
      x-api-path-slug: actiongetbytematchset-get
      parameters:
      - in: query
        name: ByteMatchSetId
        description: The ByteMatchSetId of the ByteMatchSet that you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Byte Match Set
  /?Action=GetChangeToken:
    get:
      summary: Get Change Token
      description: 'Service: AWS WAFWhen you want to create, update, or delete AWS
        WAF objects, get a change token and include the change token in the create,
        update, or delete request.'
      operationId: getChangeToken
      x-api-path-slug: actiongetchangetoken-get
      parameters:
      - in: query
        name: ChangeToken
        description: The ChangeToken that you used in the request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Change Token
  /?Action=GetChangeTokenStatus:
    get:
      summary: Get Change Token Status
      description: 'Service: AWS WAFReturns the status of a ChangeToken that you got
        by calling.'
      operationId: getChangeTokenStatus
      x-api-path-slug: actiongetchangetokenstatus-get
      parameters:
      - in: query
        name: ChangeToken
        description: The change token for which you want to get the status
        type: string
      responses:
        200:
          description: OK
      tags:
      - Change Token
  /?Action=GetIPSet:
    get:
      summary: Get IP Set
      description: 'Service: AWS WAFReturns the.'
      operationId: getIPSet
      x-api-path-slug: actiongetipset-get
      parameters:
      - in: query
        name: IPSetId
        description: The IPSetId of the IPSet that you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Sets
  /?Action=GetRule:
    get:
      summary: Get Rule
      description: 'Service: AWS WAFReturns the.'
      operationId: getRule
      x-api-path-slug: actiongetrule-get
      parameters:
      - in: query
        name: RuleId
        description: The RuleId of the Rule that you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rules
  /?Action=GetSampledRequests:
    get:
      summary: Get Sampled Requests
      description: 'Service: AWS WAFGets detailed information about a specified number
        of requests--a sample--that AWS WAF randomly selects from among the first
        5,000 requests that your AWS resource received during a time range that you
        choose.'
      operationId: getSampledRequests
      x-api-path-slug: actiongetsampledrequests-get
      parameters:
      - in: query
        name: MaxItems
        description: The number of requests that you want AWS WAF to return from among
          the first 5,000 requests that your AWS resource receivedduring the time
          range
        type: string
      - in: query
        name: RuleId
        description: 'RuleId is one of two values:'
        type: string
      - in: query
        name: TimeWindow
        description: The start date and time and the end date and time of the range
          for which you want GetSampledRequests to return a     sample of requests
        type: string
      - in: query
        name: WebAclId
        description: The WebACLId of the WebACL for which you want GetSampledRequests
          to return a sample of requests
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""
  /?Action=GetSizeConstraintSet:
    get:
      summary: Get Size Constraint Set
      description: 'Service: AWS WAFReturns the.'
      operationId: getSizeConstraintSet
      x-api-path-slug: actiongetsizeconstraintset-get
      parameters:
      - in: query
        name: SizeConstraintSetId
        description: The SizeConstraintSetId of the SizeConstraintSet that you want
          to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Size Constraint Set
  /?Action=GetSqlInjectionMatchSet:
    get:
      summary: Get Sql Injection Match Set
      description: 'Service: AWS WAFReturns the.'
      operationId: getSqlInjectionMatchSet
      x-api-path-slug: actiongetsqlinjectionmatchset-get
      parameters:
      - in: query
        name: SqlInjectionMatchSetId
        description: The SqlInjectionMatchSetId of the SqlInjectionMatchSet that you
          want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - SQL Injection Match Set
  /?Action=GetWebACL:
    get:
      summary: Get Web ACL
      description: 'Service: AWS WAFReturns the.'
      operationId: getWebACL
      x-api-path-slug: actiongetwebacl-get
      parameters:
      - in: query
        name: WebACLId
        description: The WebACLId of the WebACL that you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
  /?Action=GetWebACLForResource:
    get:
      summary: Get Web ACLFor Resource
      description: 'Service: AWS WAF RegionalReturns the web ACL for the specified
        resource.'
      operationId: getWebACLForResource
      x-api-path-slug: actiongetwebaclforresource-get
      parameters:
      - in: query
        name: ResourceArn
        description: The ARN (Amazon Resource Name) of the resource for which to get
          the web ACL
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
  /?Action=GetXssMatchSet:
    get:
      summary: Get Xss Match Set
      description: 'Service: AWS WAFReturns the.'
      operationId: getXssMatchSet
      x-api-path-slug: actiongetxssmatchset-get
      parameters:
      - in: query
        name: XssMatchSetId
        description: The XssMatchSetId of the XssMatchSet that you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - XSS Match Set
  /?Action=ListByteMatchSets:
    get:
      summary: List Byte Match Sets
      description: 'Service: AWS WAFReturns an array of.'
      operationId: listByteMatchSets
      x-api-path-slug: actionlistbytematchsets-get
      parameters:
      - in: query
        name: Limit
        description: Specifies the number of ByteMatchSet objects that you want AWS
          WAF to return for this request
        type: string
      - in: query
        name: NextMarker
        description: If you specify a value for Limit and you have more ByteMatchSets
          than the value of Limit, AWS WAF returns a NextMarker value in the response
          that allows you to list another group of ByteMatchSets
        type: string
      responses:
        200:
          description: OK
      tags:
      - Byte Match Sets
  /?Action=ListIPSets:
    get:
      summary: List IP Sets
      description: 'Service: AWS WAFReturns an array of.'
      operationId: listIPSets
      x-api-path-slug: actionlistipsets-get
      parameters:
      - in: query
        name: Limit
        description: Specifies the number of IPSet objects that you want AWS WAF to
          return for this request
        type: string
      - in: query
        name: NextMarker
        description: If you specify a value for Limit and you have more IPSets than
          the value of Limit, AWS WAF returns a NextMarker value in the response that
          allows you to list another group of IPSets
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Sets
  /?Action=ListResourcesForWebACL:
    get:
      summary: List Resources For Web ACL
      description: 'Service: AWS WAF RegionalReturns an array of resources associated
        with the specified web ACL.'
      operationId: listResourcesForWebACL
      x-api-path-slug: actionlistresourcesforwebacl-get
      parameters:
      - in: query
        name: WebACLId
        description: The unique identifier (ID) of the web ACL for which to list the
          associated resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
  /?Action=ListRules:
    get:
      summary: List Rules
      description: 'Service: AWS WAFReturns an array of.'
      operationId: listRules
      x-api-path-slug: actionlistrules-get
      parameters:
      - in: query
        name: Limit
        description: Specifies the number of Rules that you want AWS WAF to return
          for this request
        type: string
      - in: query
        name: NextMarker
        description: If you specify a value for Limit and you have more Rules than
          the value of Limit, AWS WAF returns a NextMarker value in the response that
          allows you to list another group of Rules
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rules
  /?Action=ListSizeConstraintSets:
    get:
      summary: List Size Constraint Sets
      description: 'Service: AWS WAFReturns an array of.'
      operationId: listSizeConstraintSets
      x-api-path-slug: actionlistsizeconstraintsets-get
      parameters:
      - in: query
        name: Limit
        description: Specifies the number of SizeConstraintSet objects that you want
          AWS WAF to return for this request
        type: string
      - in: query
        name: NextMarker
        description: If you specify a value for Limit and you have more SizeConstraintSets
          than the value of Limit, AWS WAF returns a NextMarker value in the response
          that allows you to list another group of SizeConstraintSets
        type: string
      responses:
        200:
          description: OK
      tags:
      - Size Constraint Sets
  /?Action=ListSqlInjectionMatchSets:
    get:
      summary: List SQL Injection Match Sets
      description: 'Service: AWS WAFReturns an array of.'
      operationId: listSqlInjectionMatchSets
      x-api-path-slug: actionlistsqlinjectionmatchsets-get
      parameters:
      - in: query
        name: Limit
        description: Specifies the number of SqlInjectionMatchSet objects that you
          want AWS WAF to return for this request
        type: string
      - in: query
        name: NextMarker
        description: If you specify a value for Limit and you have more SqlInjectionMatchSet
          objects than the value of Limit, AWS WAF returns a NextMarker value in the
          response that allows you to list another group of SqlInjectionMatchSets
        type: string
      responses:
        200:
          description: OK
      tags:
      - SQL Injection Match Sets
  /?Action=ListWebACLs:
    get:
      summary: List Web ACLs
      description: 'Service: AWS WAFReturns an array of.'
      operationId: listWebACLs
      x-api-path-slug: actionlistwebacls-get
      parameters:
      - in: query
        name: Limit
        description: Specifies the number of WebACL objects that you want AWS WAF
          to return for this request
        type: string
      - in: query
        name: NextMarker
        description: If you specify a value for Limit and you have more WebACL objects
          than the number that you specify for Limit, AWS WAF returns a NextMarker
          value in the response that allows you to list another group of WebACL objects
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
  /?Action=ListXssMatchSets:
    get:
      summary: List Xss Match Sets
      description: 'Service: AWS WAFReturns an array of.'
      operationId: listXssMatchSets
      x-api-path-slug: actionlistxssmatchsets-get
      parameters:
      - in: query
        name: Limit
        description: Specifies the number of XssMatchSet objects that you want AWS
          WAF to return for this request
        type: string
      - in: query
        name: NextMarker
        description: If you specify a value for Limit and you have more XssMatchSet
          objects than the value of Limit, AWS WAF returns a NextMarker value in the
          response that allows you to list another group of XssMatchSets
        type: string
      responses:
        200:
          description: OK
      tags:
      - XSS Match Set
  /?Action=UpdateByteMatchSet:
    get:
      summary: Update Byte Match Set
      description: 'Service: AWS WAFInserts or deletes.'
      operationId: updateByteMatchSet
      x-api-path-slug: actionupdatebytematchset-get
      parameters:
      - in: query
        name: ByteMatchSetId
        description: The ByteMatchSetId of the ByteMatchSet that you want to update
        type: string
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: Updates
        description: An array of ByteMatchSetUpdate objects that you want to insert
          into or delete from a ByteMatchSet
        type: string
      responses:
        200:
          description: OK
      tags:
      - Byte Match Set
  /?Action=UpdateIPSet:
    get:
      summary: Update IP Set
      description: 'Service: AWS WAFInserts or deletes.'
      operationId: updateIPSet
      x-api-path-slug: actionupdateipset-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: IPSetId
        description: The IPSetId of the IPSet that you want to update
        type: string
      - in: query
        name: Updates
        description: An array of IPSetUpdate objects that you want to insert into
          or delete from an IPSet
        type: string
      responses:
        200:
          description: OK
      tags:
      - IP Sets
  /?Action=UpdateRule:
    get:
      summary: Update Rule
      description: 'Service: AWS WAFInserts or deletes.'
      operationId: updateRule
      x-api-path-slug: actionupdaterule-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: RuleId
        description: The RuleId of the Rule that you want to update
        type: string
      - in: query
        name: Updates
        description: An array of RuleUpdate objects that you want to insert into or
          delete from a Rule
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rules
  /?Action=UpdateSizeConstraintSet:
    get:
      summary: Update Size Constraint Set
      description: 'Service: AWS WAFInserts or deletes.'
      operationId: updateSizeConstraintSet
      x-api-path-slug: actionupdatesizeconstraintset-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: SizeConstraintSetId
        description: The SizeConstraintSetId of the SizeConstraintSet that you want
          to update
        type: string
      - in: query
        name: Updates
        description: An array of SizeConstraintSetUpdate objects that you want to
          insert into or delete from a SizeConstraintSet
        type: string
      responses:
        200:
          description: OK
      tags:
      - Size Constraint Set
  /?Action=UpdateSqlInjectionMatchSet:
    get:
      summary: Update SQL Injection Match Set
      description: 'Service: AWS WAFInserts or deletes.'
      operationId: updateSqlInjectionMatchSet
      x-api-path-slug: actionupdatesqlinjectionmatchset-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: SqlInjectionMatchSetId
        description: The SqlInjectionMatchSetId of the SqlInjectionMatchSet that you
          want to update
        type: string
      - in: query
        name: Updates
        description: An array of SqlInjectionMatchSetUpdate objects that you want
          to insert into or delete from a SqlInjectionMatchSet
        type: string
      responses:
        200:
          description: OK
      tags:
      - SQL Injection Match Sets
  /?Action=UpdateWebACL:
    get:
      summary: Update Web ACL
      description: 'Service: AWS WAFInserts or deletes.'
      operationId: updateWebACL
      x-api-path-slug: actionupdatewebacl-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: DefaultAction
        description: A default action for the web ACL, either ALLOW or BLOCK
        type: string
      - in: query
        name: Updates
        description: An array of updates to make to the WebACL
        type: string
      - in: query
        name: WebACLId
        description: The WebACLId of the WebACL that you want to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Web ACL
  /?Action=UpdateXssMatchSet:
    get:
      summary: Update Xss Match Set
      description: 'Service: AWS WAFInserts or deletes.'
      operationId: updateXssMatchSet
      x-api-path-slug: actionupdatexssmatchset-get
      parameters:
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: Updates
        description: An array of XssMatchSetUpdate objects that you want to insert
          into or delete from a XssMatchSet
        type: string
      - in: query
        name: XssMatchSetId
        description: The XssMatchSetId of the XssMatchSet that you want to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - XSS Match Set