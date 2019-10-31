swagger: "2.0"
x-collection-name: aWhere
x-complete: 1
info:
  title: aWhere API Platform
  description: todo-add-description
  version: 1.0.0
host: api.awhere.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/agronomics/fields/field1/agronomicvalues/2015-08-01,2015-08-03:
    get:
      summary: Agronomic Values & Accumulations
      description: "####Request\nThis API call gets calculated agronomics and accumulations
        at a field location. \n\nThe URL used here will get the values for a certain
        range of days. This is a very flexible API and so you're encouraged to review
        the [Agronomics Documentation](http://developer.awhere.com/api/reference/agronomics/values).\n\n_Tip:
        Remember to use a field ID that exists in your account. By default, this collection
        uses a default field ID of 'field1'_\n\n\n####Security\nThis API call uses
        the security Access Token that is retrieved with the \"Get a Token\" request.
        If you run that request first, it will save a token to Postman and this API
        will use it automatically. You can also see where the token should normally
        go by clicking the \"Headers\" tab below. The Authorization header holds the
        token, replacing the \"{{aWhereAccessToken}}\" part."
      operationId: V2AgronomicsFieldsField1Agronomicvalues2015080120150803Get
      x-api-path-slug: v2agronomicsfieldsfield1agronomicvalues2015080120150803-get
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Agronomic
      - Values
      - '&'
      - Accumulations
  /v2/agronomics/fields/field1/agronomicnorms/08-01,08-03/years/2010,2014:
    get:
      summary: Agronomic Norms
      description: "####Request\nThis API call gets the long term averages for agronomic
        values and accumulations at a field location. \n\nThe URL used here will get
        the values for a certain range of days over a certain range of years. This
        is a very flexible API and so you're encouraged to review the [Agronomics
        Documentation](http://developer.awhere.com/api/reference/agronomics/norms).\n\n_Tip:
        Remember to use a field ID that exists in your account. By default, this collection
        uses a default field ID of 'field1'_\n\n\n####Security\nThis API call uses
        the security Access Token that is retrieved with the \"Get a Token\" request.
        If you run that request first, it will save a token to Postman and this API
        will use it automatically. You can also see where the token should normally
        go by clicking the \"Headers\" tab below. The Authorization header holds the
        token, replacing the \"{{aWhereAccessToken}}\" part."
      operationId: V2AgronomicsFieldsField1Agronomicnorms08010803Years20102014Get
      x-api-path-slug: v2agronomicsfieldsfield1agronomicnorms08010803years20102014-get
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Agronomic
      - Norms
  /v2/fields:
    get:
      summary: Get Fields List
      description: "####Request\nThis API call retrieves the list of fields in your
        account. \n\n[Get Fields Documentation](http://developer.awhere.com/api/reference/fields/get-fields)\n\n\n####Security\nThis
        API call uses the security Access Token that is retrieved with the \"Get a
        Token\" request. If you run that request first, it will save a token to Postman
        and this API will use it automatically. You can also see where the token should
        normally go by clicking the \"Headers\" tab below. The Authorization header
        holds the token, replacing the \"{{aWhereAccessToken}}\" part."
      operationId: V2FieldsGet
      x-api-path-slug: v2fields-get
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Fields
      - List
    post:
      summary: Create a Field
      description: "####Request\nThis API call creates a field location in your account.
        Be sure to change the body payload. \n\n[Create Fields Documentation](http://developer.awhere.com/api/reference/fields/create-field)\n\n\n####Security\nThis
        API call uses the security Access Token that is retrieved with the \"Get a
        Token\" request. If you run that request first, it will save a token to Postman
        and this API will use it automatically. You can also see where the token should
        normally go by clicking the \"Headers\" tab below. The Authorization header
        holds the token, replacing the \"{{aWhereAccessToken}}\" part."
      operationId: V2FieldsPost
      x-api-path-slug: v2fields-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Field
  /v2/fields/field1:
    get:
      summary: Get a Single Field by ID
      description: |-
        ####Request
        This API call retrieves a single field by ID.

        [Get Fields Documentation](http://developer.awhere.com/api/reference/fields/get-fields)


        ####Security
        This API call uses the security Access Token that is retrieved with the "Get a Token" request. If you run that request first, it will save a token to Postman and this API will use it automatically. You can also see where the token should normally go by clicking the "Headers" tab below. The Authorization header holds the token, replacing the "{{aWhereAccessToken}}" part.
      operationId: V2FieldsField1Get
      x-api-path-slug: v2fieldsfield1-get
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Single
      - Field
      - By
      - ID
    patch:
      summary: Update Field
      description: |-
        ####Request
        This API call shows how to update the farm ID on a field location. You can also change the name.

        [Update Field Documentation](http://developer.awhere.com/api/reference/fields/update-field)


        ####Security
        This API call uses the security Access Token that is retrieved with the "Get a Token" request. If you run that request first, it will save a token to Postman and this API will use it automatically. You can also see where the token should normally go by clicking the "Headers" tab below. The Authorization header holds the token, replacing the "{{aWhereAccessToken}}" part.
      operationId: V2FieldsField1Patch
      x-api-path-slug: v2fieldsfield1-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Field
  /v2/agronomics/fields/field1/plantings:
    get:
      summary: Get Plantings List for a Field
      description: "####Request\nThis API call retrieves the list of plantings for
        a specific field in your account. \n\n[Get Plantings Documentation](http://developer.awhere.com/api/reference/plantings/get-plantings)\n\n\n####Security\nThis
        API call uses the security Access Token that is retrieved with the \"Get a
        Token\" request. If you run that request first, it will save a token to Postman
        and this API will use it automatically. You can also see where the token should
        normally go by clicking the \"Headers\" tab below. The Authorization header
        holds the token, replacing the \"{{aWhereAccessToken}}\" part."
      operationId: V2AgronomicsFieldsField1PlantingsGet
      x-api-path-slug: v2agronomicsfieldsfield1plantings-get
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Plantings
      - Lista
      - Field
    post:
      summary: Create a Planting
      description: "####Request\nThis API call creates a planting for a specific field
        in your account. \n\n__Note:__ You should at least change the dates in the
        request body.\n\n[Create Planting Documentation](http://developer.awhere.com/api/reference/plantings/create)\n\n\n####Security\nThis
        API call uses the security Access Token that is retrieved with the \"Get a
        Token\" request. If you run that request first, it will save a token to Postman
        and this API will use it automatically. You can also see where the token should
        normally go by clicking the \"Headers\" tab below. The Authorization header
        holds the token, replacing the \"{{aWhereAccessToken}}\" part."
      operationId: V2AgronomicsFieldsField1PlantingsPost
      x-api-path-slug: v2agronomicsfieldsfield1plantings-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Planting
  /v2/agronomics/fields/field1/plantings/current:
    patch:
      summary: Update Part of a Planting
      description: |-
        ####Request
        This API call shows how to update only a couple of fields in a planting instead of having to update the entire object.

        __Note:__ You probably what to change the date in the request body.

        [Update Planting Documentation](http://developer.awhere.com/api/reference/plantings/update)


        ####Security
        This API call uses the security Access Token that is retrieved with the "Get a Token" request. If you run that request first, it will save a token to Postman and this API will use it automatically. You can also see where the token should normally go by clicking the "Headers" tab below. The Authorization header holds the token, replacing the "{{aWhereAccessToken}}" part.
      operationId: V2AgronomicsFieldsField1PlantingsCurrentPatch
      x-api-path-slug: v2agronomicsfieldsfield1plantingscurrent-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Part
      - Of
      - Planting
  /v2/agronomics/crops:
    get:
      summary: Get Crops
      description: |-
        ####Request
        This API call returns the list of currently available crops in the aWhere platform.

        [Crops Documentation](http://developer.awhere.com/api/reference/crops).


        ####Security
        This API call uses the security Access Token that is retrieved with the "Get a Token" request. If you run that request first, it will save a token to Postman and this API will use it automatically. You can also see where the token should normally go by clicking the "Headers" tab below. The Authorization header holds the token, replacing the "{{aWhereAccessToken}}" part.
      operationId: V2AgronomicsCropsGet
      x-api-path-slug: v2agronomicscrops-get
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Crops
  /v2/agronomics/models:
    get:
      summary: Get Models
      description: |-
        ####Request
        This API call returns the list of currently available models in the aWhere platform.

        [Crops Documentation](http://developer.awhere.com/api/reference/models/get-models).


        ####Security
        This API call uses the security Access Token that is retrieved with the "Get a Token" request. If you run that request first, it will save a token to Postman and this API will use it automatically. You can also see where the token should normally go by clicking the "Headers" tab below. The Authorization header holds the token, replacing the "{{aWhereAccessToken}}" part.
      operationId: V2AgronomicsModelsGet
      x-api-path-slug: v2agronomicsmodels-get
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Models
  /v2/agronomics/models/BarleyGenericMSU/details:
    get:
      summary: Get Model Details
      description: "####Request\nThis API call returns the details about a particular
        model. Currently, growth stage models are available via the API, so the details
        are a list of the possible stages with GDD threshold information. \n\n[Model
        Details Documentation](http://developer.awhere.com/api/reference/models/details).\n\n\n####Security\nThis
        API call uses the security Access Token that is retrieved with the \"Get a
        Token\" request. If you run that request first, it will save a token to Postman
        and this API will use it automatically. You can also see where the token should
        normally go by clicking the \"Headers\" tab below. The Authorization header
        holds the token, replacing the \"{{aWhereAccessToken}}\" part."
      operationId: V2AgronomicsModelsBarleyGenericMSUDetailsGet
      x-api-path-slug: v2agronomicsmodelsbarleygenericmsudetails-get
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Model
      - Details
  /v2/agronomics/fields/field1/models/BarleyGenericMSU/results:
    get:
      summary: Get Model Results
      description: "####Request\nThis API call returns the current results of a model
        based on the data provided for the identified field location. \n\n[Model Results
        Documentation](http://developer.awhere.com/api/reference/models/results).\n\n\n####Security\nThis
        API call uses the security Access Token that is retrieved with the \"Get a
        Token\" request. If you run that request first, it will save a token to Postman
        and this API will use it automatically. You can also see where the token should
        normally go by clicking the \"Headers\" tab below. The Authorization header
        holds the token, replacing the \"{{aWhereAccessToken}}\" part."
      operationId: V2AgronomicsFieldsField1ModelsBarleyGenericMSUResultsGet
      x-api-path-slug: v2agronomicsfieldsfield1modelsbarleygenericmsuresults-get
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Model
      - Results
  /v2/weather/fields/field1/observations:
    get:
      summary: Daily Observations
      description: "####Request\nThis API call gets the weather at a field location.\n\nThe
        default URL will get the last seven days of actual weather observations. You
        can add dates to the end of the URL to get the weather for a specific range
        of days, like so: \n\n`/v2/weather/fields/field1/observations/2015-08-01`
        gets a single day\n`/v2/weather/fields/field1/observations/2015-08-01,2015-08-15`
        gets everything from August 1-15\n\nYou can customize the response payload
        using query string parameters. Learn more in the [Daily Observations Documentation](http://developer.awhere.com/api/reference/weather/observations).\n\n_Tip:
        Remember to use a field ID that exists in your account. By default, this collection
        uses a default field ID of 'field1'_\n\n\n####Security\nThis API call uses
        the security Access Token that is retrieved with the \"Get a Token\" request.
        If you run that request first, it will save a token to Postman and this API
        will use it automatically. You can also see where the token should normally
        go by clicking the \"Headers\" tab below. The Authorization header holds the
        token, replacing the \"{{aWhereAccessToken}}\" part."
      operationId: V2WeatherFieldsField1ObservationsGet
      x-api-path-slug: v2weatherfieldsfield1observations-get
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Daily
      - Observations
  /v2/weather/fields/field1/forecasts:
    get:
      summary: Forecasts
      description: "####Request\nThis API call gets the forecast at a field location.\n\nWith
        the default configuration you'll get the hourly forecast for today +8 days.
        Add dates to the end of the URL to request only specific days, like so: \n\n`/v2/weather/fields/field1/forecasts/YYYY-MM-DD`
        returns a single day\n`/v2/weather/fields/field1/forecasts/YYYY-MM-DD,YYYY-MM-DD`
        returns a range of days\n\nYou can also use query string parameters to customize
        the payloads. Read the [Forecast Documentation](http://developer.awhere.com/api/reference/weather/forecast)
        for details.\n\n\n_Tip: Remember to use a field ID that exists in your account.
        By default, this collection uses a default field ID of 'field1'_\n\n\n\n####Security\nThis
        API call uses the security Access Token that is retrieved with the \"Get a
        Token\" request. If you run that request first, it will save a token to Postman
        and this API will use it automatically. You can also see where the token should
        normally go by clicking the \"Headers\" tab below. The Authorization header
        holds the token, replacing the \"{{aWhereAccessToken}}\" part."
      operationId: V2WeatherFieldsField1ForecastsGet
      x-api-path-slug: v2weatherfieldsfield1forecasts-get
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Forecasts
  /v2/weather/fields/field1/norms/08-01,08-15/years/2010,2015:
    get:
      summary: Norms
      description: |-
        ####Request
        Use this API to calculate long-term averages for the weather for any set of days across any set of years (minumum 3). This is a very flexible API, and you're encouraged to review the [Weather Norms Documentation](http://developer.awhere.com/api/reference/weather/norms) for details.

        _Tip: Remember to use a field ID that exists in your account. By default, this collection uses a default field ID of 'field1'_

        ####Security
        This API call uses the security Access Token that is retrieved with the "Get a Token" request. If you run that request first, it will save a token to Postman and this API will use it automatically. You can also see where the token should normally go by clicking the "Headers" tab below. The Authorization header holds the token, replacing the "{{aWhereAccessToken}}" part.
      operationId: V2WeatherFieldsField1Norms08010815Years20102015Get
      x-api-path-slug: v2weatherfieldsfield1norms08010815years20102015-get
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Norms
  /v2/weather/fields/field1/currentconditions:
    get:
      summary: Current Conditions
      description: |-
        ####Request
        This API call provides a snapshot of recent weather using the weather station nearest to the field location.

        [Current Conditions Documentation](http://developer.awhere.com/api/reference/weather/current)

        _Tip: Remember to use a field ID that exists in your account. By default, this collection uses a default field ID of 'field1'_


        ####Security
        This API call uses the security Access Token that is retrieved with the "Get a Token" request. If you run that request first, it will save a token to Postman and this API will use it automatically. You can also see where the token should normally go by clicking the "Headers" tab below. The Authorization header holds the token, replacing the "{{aWhereAccessToken}}" part.
      operationId: V2WeatherFieldsField1CurrentconditionsGet
      x-api-path-slug: v2weatherfieldsfield1currentconditions-get
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Current
      - Conditions
  /oauth/token:
    post:
      summary: Get a Token
      description: "This is the first API call you will make any time you use the
        API \n(but you only need to use once per hour). This request will \nrequest
        a security access token and save it to Postman. Later \nAPI calls will use
        the token from Postman's saved variables. \n\n[Authentication Documentation](http://developer.awhere.com/api/authentication)\n\nPrior
        to using this API call you should load the aWhere Environment\nfile into Postman
        and change the settings to your API Key and Secret.\nYou can also see where
        the key and secret should go, or enter\nthem manually, by choosing the \"Authorization\"
        tab below, selecting\n\"Basic Auth,\" and then entering the key and secret
        as the username\nand password."
      operationId: OauthTokenPost
      x-api-path-slug: oauthtoken-post
      parameters:
      - in: formData
        name: grant_type
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Token