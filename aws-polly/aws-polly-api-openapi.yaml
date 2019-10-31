swagger: "2.0"
x-collection-name: AWS Polly
x-complete: 1
info:
  title: AWS Polly API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteLexicon:
    get:
      summary: Delete Lexicon
      description: Deletes the specified pronunciation lexicon stored in an AWS Region.
      operationId: deleteLexicon
      x-api-path-slug: actiondeletelexicon-get
      parameters:
      - in: query
        name: Name
        description: The name of the lexicon to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Lexicons
  /?Action=DescribeVoices:
    get:
      summary: Describe Voices
      description: Returns the list of voices that are available for use when requesting
        speech synthesis.
      operationId: describeVoices
      x-api-path-slug: actiondescribevoices-get
      parameters:
      - in: query
        name: LanguageCode
        description: The language identification tag (ISO 639 code for the language
          name-ISO 3166 country code)       for filtering the list of voices returned
        type: string
      - in: query
        name: NextToken
        description: An opaque pagination token returned from the previous     DescribeVoices
          operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - voices
  /?Action=GetLexicon:
    get:
      summary: Get Lexicon
      description: Returns the content of the specified pronunciation lexicon stored
        in an AWS Region.
      operationId: getLexicon
      x-api-path-slug: actiongetlexicon-get
      parameters:
      - in: query
        name: Name
        description: Name of the lexicon
        type: string
      responses:
        200:
          description: OK
      tags:
      - Lexicons
  /?Action=ListLexicons:
    get:
      summary: List Lexicons
      description: Returns a list of pronunciation lexicons stored in an AWS Region.
      operationId: listLexicons
      x-api-path-slug: actionlistlexicons-get
      parameters:
      - in: query
        name: NextToken
        description: An opaque pagination token returned from previous       ListLexicons
          operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Lexicons
  /?Action=PutLexicon:
    get:
      summary: Put Lexicon
      description: Stores a pronunciation lexicon in an AWS Region.
      operationId: putLexicon
      x-api-path-slug: actionputlexicon-get
      parameters:
      - in: query
        name: Name
        description: Name of the lexicon
        type: string
      responses:
        200:
          description: OK
      tags:
      - Lexicons
  /?Action=SynthesizeSpeech:
    get:
      summary: Synthesize Speech
      description: Synthesizes UTF-8 input, plain text or SSML, to a stream of bytes.
      operationId: synthesizeSpeech
      x-api-path-slug: actionsynthesizespeech-get
      parameters:
      - in: query
        name: LexiconNames
        description: List of one or more pronunciation lexicon names you want the
          service to apply      during synthesis
        type: string
      - in: query
        name: OutputFormat
        description: The audio format in which the resulting stream will be encoded
        type: string
      - in: query
        name: SampleRate
        description: The audio frequency specified in Hz
        type: string
      - in: query
        name: Text
        description: Input text to synthesize
        type: string
      - in: query
        name: TextType
        description: Specifies whether the input text is plain text or SSML
        type: string
      - in: query
        name: VoiceId
        description: Voice ID to use for the synthesis
        type: string
      responses:
        200:
          description: OK
      tags:
      - Speech