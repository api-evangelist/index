swagger: "2.0"
x-collection-name: Wordnik
x-complete: 1
info:
  title: Wordnik
  description: wordnik-is-the-worlds-biggest-online-english-dictionary-by-number-of-words
  version: "4.0"
host: api.wordnik.com
basePath: /v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account.json/apiTokenStatus:
    get:
      summary: Returns usage statistics for the API account.
      description: Returns usage statistics for the api account..
      operationId: getApiTokenStatus
      x-api-path-slug: account-jsonapitokenstatus-get
      parameters:
      - in: header
        name: api_key
        description: Wordnik authentication token
      responses:
        200:
          description: OK
      tags:
      - Account
      - ApiTokenStatus
  /account.json/authenticate/{username}:
    get:
      summary: Authenticates a User
      description: Authenticates a user.
      operationId: authenticate
      x-api-path-slug: account-jsonauthenticateusername-get
      parameters:
      - in: query
        name: password
        description: The users password
      - in: path
        name: username
        description: A confirmed Wordnik username
      responses:
        200:
          description: OK
      tags:
      - Account
      - Authenticate
      - Username
    post:
      summary: Authenticates a user
      description: Authenticates a user.
      operationId: authenticatePost
      x-api-path-slug: account-jsonauthenticateusername-post
      parameters:
      - in: body
        name: body
        description: The users password
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: username
        description: A confirmed Wordnik username
      responses:
        200:
          description: OK
      tags:
      - Account
      - Authenticate
      - Username
  /account.json/user:
    get:
      summary: Returns the logged-in User
      description: Requires a valid auth_token to be set.
      operationId: getLoggedInUser
      x-api-path-slug: account-jsonuser-get
      parameters:
      - in: header
        name: auth_token
        description: The auth token of the logged-in user, obtained by calling /account
      responses:
        200:
          description: OK
      tags:
      - Account
      - User
  /account.json/wordLists:
    get:
      summary: Fetches WordList objects for the logged-in user.
      description: Fetches wordlist objects for the logged-in user..
      operationId: getWordListsForLoggedInUser
      x-api-path-slug: account-jsonwordlists-get
      parameters:
      - in: header
        name: auth_token
        description: auth_token of logged-in user
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: skip
        description: Results to skip
      responses:
        200:
          description: OK
      tags:
      - Account
      - Words
      - Lists
  /word.json/{word}:
    get:
      summary: Given a word as a string, returns the WordObject that represents it
      description: Given a word as a string, returns the wordobject that represents
        it.
      operationId: getWord
      x-api-path-slug: word-jsonword-get
      parameters:
      - in: query
        name: includeSuggestions
        description: Return suggestions (for correct spelling, case variants, etc
      - in: query
        name: useCanonical
        description: If true will try to return the correct word root (cats -> cat)
      - in: path
        name: word
        description: String value of WordObject to return
      responses:
        200:
          description: OK
      tags:
      - Words
  /word.json/{word}/audio:
    get:
      summary: Fetches audio metadata for a word.
      description: The metadata includes a time-expiring fileUrl which allows reading
        the audio file directly from the API.  Currently only audio pronunciations
        from the American Heritage Dictionary in mp3 format are supported.
      operationId: getAudio
      x-api-path-slug: word-jsonwordaudio-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: useCanonical
        description: Use the canonical form of the word
      - in: path
        name: word
        description: Word to get audio for
      responses:
        200:
          description: OK
      tags:
      - Words
      - Audio
  /word.json/{word}/definitions:
    get:
      summary: Return definitions for a word
      description: Return definitions for a word.
      operationId: getDefinitions
      x-api-path-slug: word-jsonworddefinitions-get
      parameters:
      - in: query
        name: includeRelated
        description: Return related words with definitions
      - in: query
        name: includeTags
        description: Return a closed set of XML tags in response
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: partOfSpeech
        description: CSV list of part-of-speech types
      - in: query
        name: sourceDictionaries
        description: Source dictionary to return definitions from
      - in: query
        name: useCanonical
        description: If true will try to return the correct word root (cats -> cat)
      - in: path
        name: word
        description: Word to return definitions for
      responses:
        200:
          description: OK
      tags:
      - Words
      - Definitions
  /word.json/{word}/etymologies:
    get:
      summary: Fetches etymology data
      description: Fetches etymology data.
      operationId: getEtymologies
      x-api-path-slug: word-jsonwordetymologies-get
      parameters:
      - in: query
        name: useCanonical
        description: If true will try to return the correct word root (cats -> cat)
      - in: path
        name: word
        description: Word to return
      responses:
        200:
          description: OK
      tags:
      - Words
      - Etymologies
  /word.json/{word}/examples:
    get:
      summary: Returns examples for a word
      description: Returns examples for a word.
      operationId: getExamples
      x-api-path-slug: word-jsonwordexamples-get
      parameters:
      - in: query
        name: includeDuplicates
        description: Show duplicate examples from different sources
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: skip
        description: Results to skip
      - in: query
        name: useCanonical
        description: If true will try to return the correct word root (cats -> cat)
      - in: path
        name: word
        description: Word to return examples for
      responses:
        200:
          description: OK
      tags:
      - Words
      - Examples
  /word.json/{word}/frequency:
    get:
      summary: Returns word usage over time
      description: Returns word usage over time.
      operationId: getWordFrequency
      x-api-path-slug: word-jsonwordfrequency-get
      parameters:
      - in: query
        name: endYear
        description: Ending Year
      - in: query
        name: startYear
        description: Starting Year
      - in: query
        name: useCanonical
        description: If true will try to return the correct word root (cats -> cat)
      - in: path
        name: word
        description: Word to return
      responses:
        200:
          description: OK
      tags:
      - Words
      - Frequency
  /word.json/{word}/hyphenation:
    get:
      summary: Returns syllable information for a word
      description: Returns syllable information for a word.
      operationId: getHyphenation
      x-api-path-slug: word-jsonwordhyphenation-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: sourceDictionary
        description: Get from a single dictionary
      - in: query
        name: useCanonical
        description: If true will try to return a correct word root (cats -> cat)
      - in: path
        name: word
        description: Word to get syllables for
      responses:
        200:
          description: OK
      tags:
      - Words
      - Hyphenation
  /word.json/{word}/phrases:
    get:
      summary: Fetches bi-gram phrases for a word
      description: Fetches bi-gram phrases for a word.
      operationId: getPhrases
      x-api-path-slug: word-jsonwordphrases-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: useCanonical
        description: If true will try to return the correct word root (cats -> cat)
      - in: query
        name: wlmi
        description: Minimum WLMI for the phrase
      - in: path
        name: word
        description: Word to fetch phrases for
      responses:
        200:
          description: OK
      tags:
      - Words
      - Phrases
  /word.json/{word}/pronunciations:
    get:
      summary: Returns text pronunciations for a given word
      description: Returns text pronunciations for a given word.
      operationId: getTextPronunciations
      x-api-path-slug: word-jsonwordpronunciations-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: sourceDictionary
        description: Get from a single dictionary
      - in: query
        name: typeFormat
        description: Text pronunciation type
      - in: query
        name: useCanonical
        description: If true will try to return a correct word root (cats -> cat)
      - in: path
        name: word
        description: Word to get pronunciations for
      responses:
        200:
          description: OK
      tags:
      - Words
      - Pronunciations
  /word.json/{word}/relatedWords:
    get:
      summary: Given a word as a string, returns relationships from the Word Graph
      description: Given a word as a string, returns relationships from the word graph.
      operationId: getRelatedWords
      x-api-path-slug: word-jsonwordrelatedwords-get
      parameters:
      - in: query
        name: limitPerRelationshipType
        description: Restrict to the supplied relationship types
      - in: query
        name: relationshipTypes
        description: Limits the total results per type of relationship type
      - in: query
        name: useCanonical
        description: If true will try to return the correct word root (cats -> cat)
      - in: path
        name: word
        description: Word to fetch relationships for
      responses:
        200:
          description: OK
      tags:
      - Words
      - RelatedWords
  /word.json/{word}/topExample:
    get:
      summary: Returns a top example for a word
      description: Returns a top example for a word.
      operationId: getTopExample
      x-api-path-slug: word-jsonwordtopexample-get
      parameters:
      - in: query
        name: useCanonical
        description: If true will try to return the correct word root (cats -> cat)
      - in: path
        name: word
        description: Word to fetch examples for
      responses:
        200:
          description: OK
      tags:
      - Words
      - TopExample
  /wordList.json/{permalink}:
    delete:
      summary: Deletes an existing WordList
      description: Deletes an existing wordlist.
      operationId: deleteWordList
      x-api-path-slug: wordlist-jsonpermalink-delete
      parameters:
      - in: header
        name: auth_token
        description: The auth token of the logged-in user, obtained by calling /account
      - in: path
        name: permalink
        description: ID of WordList to delete
      responses:
        200:
          description: OK
      tags:
      - WordList
      - Permalink
    get:
      summary: Fetches a WordList by ID
      description: Fetches a wordlist by id.
      operationId: getWordListByPermalink
      x-api-path-slug: wordlist-jsonpermalink-get
      parameters:
      - in: header
        name: auth_token
        description: The auth token of the logged-in user, obtained by calling /account
      - in: path
        name: permalink
        description: permalink of WordList to fetch
      responses:
        200:
          description: OK
      tags:
      - WordList
      - Permalink
    put:
      summary: Updates an existing WordList
      description: Updates an existing wordlist.
      operationId: updateWordList
      x-api-path-slug: wordlist-jsonpermalink-put
      parameters:
      - in: header
        name: auth_token
        description: The auth token of the logged-in user, obtained by calling /account
      - in: body
        name: body
        description: Updated WordList
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: permalink
        description: permalink of WordList to update
      responses:
        200:
          description: OK
      tags:
      - WordList
      - Permalink
  /wordList.json/{permalink}/deleteWords:
    post:
      summary: Removes words from a WordList
      description: Removes words from a wordlist.
      operationId: deleteWordsFromWordList
      x-api-path-slug: wordlist-jsonpermalinkdeletewords-post
      parameters:
      - in: header
        name: auth_token
        description: The auth token of the logged-in user, obtained by calling /account
      - in: body
        name: body
        description: Words to remove from WordList
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: permalink
        description: permalink of WordList to use
      responses:
        200:
          description: OK
      tags:
      - WordList
      - Permalink
      - DeleteWords
  /wordList.json/{permalink}/words:
    get:
      summary: Fetches words in a WordList
      description: Fetches words in a wordlist.
      operationId: getWordListWords
      x-api-path-slug: wordlist-jsonpermalinkwords-get
      parameters:
      - in: header
        name: auth_token
        description: The auth token of the logged-in user, obtained by calling /account
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: path
        name: permalink
        description: ID of WordList to use
      - in: query
        name: skip
        description: Results to skip
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortOrder
        description: Direction to sort
      responses:
        200:
          description: OK
      tags:
      - WordList
      - Permalink
      - Words
    post:
      summary: Adds words to a WordList
      description: Adds words to a wordlist.
      operationId: addWordsToWordList
      x-api-path-slug: wordlist-jsonpermalinkwords-post
      parameters:
      - in: header
        name: auth_token
        description: The auth token of the logged-in user, obtained by calling /account
      - in: body
        name: body
        description: Array of words to add to WordList
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: permalink
        description: permalink of WordList to user
      responses:
        200:
          description: OK
      tags:
      - WordList
      - Permalink
      - Words
  /wordLists.json:
    post:
      summary: Creates a WordList.
      description: Creates a wordlist..
      operationId: createWordList
      x-api-path-slug: wordlists-json-post
      parameters:
      - in: header
        name: auth_token
        description: The auth token of the logged-in user, obtained by calling /account
      - in: body
        name: body
        description: WordList to create
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Words
      - Lists
  /words.json/randomWord:
    get:
      summary: Returns a single random WordObject
      description: Returns a single random wordobject.
      operationId: getRandomWord
      x-api-path-slug: words-jsonrandomword-get
      parameters:
      - in: query
        name: excludePartOfSpeech
        description: CSV part-of-speech values to exclude
      - in: query
        name: hasDictionaryDef
        description: Only return words with dictionary definitions
      - in: query
        name: includePartOfSpeech
        description: CSV part-of-speech values to include
      - in: query
        name: maxCorpusCount
        description: Maximum corpus frequency for terms
      - in: query
        name: maxDictionaryCount
        description: Maximum dictionary count
      - in: query
        name: maxLength
        description: Maximum word length
      - in: query
        name: minCorpusCount
        description: Minimum corpus frequency for terms
      - in: query
        name: minDictionaryCount
        description: Minimum dictionary count
      - in: query
        name: minLength
        description: Minimum word length
      responses:
        200:
          description: OK
      tags:
      - Words
      - RandomWord
  /words.json/randomWords:
    get:
      summary: Returns an array of random WordObjects
      description: Returns an array of random wordobjects.
      operationId: getRandomWords
      x-api-path-slug: words-jsonrandomwords-get
      parameters:
      - in: query
        name: excludePartOfSpeech
        description: CSV part-of-speech values to exclude
      - in: query
        name: hasDictionaryDef
        description: Only return words with dictionary definitions
      - in: query
        name: includePartOfSpeech
        description: CSV part-of-speech values to include
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: maxCorpusCount
        description: Maximum corpus frequency for terms
      - in: query
        name: maxDictionaryCount
        description: Maximum dictionary count
      - in: query
        name: maxLength
        description: Maximum word length
      - in: query
        name: minCorpusCount
        description: Minimum corpus frequency for terms
      - in: query
        name: minDictionaryCount
        description: Minimum dictionary count
      - in: query
        name: minLength
        description: Minimum word length
      - in: query
        name: sortBy
        description: Attribute to sort by
      - in: query
        name: sortOrder
        description: Sort direction
      responses:
        200:
          description: OK
      tags:
      - Words
      - RandomWords
  /words.json/reverseDictionary:
    get:
      summary: Reverse dictionary search
      description: Reverse dictionary search.
      operationId: reverseDictionary
      x-api-path-slug: words-jsonreversedictionary-get
      parameters:
      - in: query
        name: excludePartOfSpeech
        description: Exclude these comma-delimited parts of speech
      - in: query
        name: excludeSourceDictionaries
        description: Exclude these comma-delimited source dictionaries
      - in: query
        name: expandTerms
        description: Expand terms
      - in: query
        name: findSenseForWord
        description: Restricts words and finds closest sense
      - in: query
        name: includePartOfSpeech
        description: Only include these comma-delimited parts of speech
      - in: query
        name: includeSourceDictionaries
        description: Only include these comma-delimited source dictionaries
      - in: query
        name: includeTags
        description: Return a closed set of XML tags in response
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: maxCorpusCount
        description: Maximum corpus frequency for terms
      - in: query
        name: maxLength
        description: Maximum word length
      - in: query
        name: minCorpusCount
        description: Minimum corpus frequency for terms
      - in: query
        name: minLength
        description: Minimum word length
      - in: query
        name: query
        description: Search term
      - in: query
        name: skip
        description: Results to skip
      - in: query
        name: sortBy
        description: Attribute to sort by
      - in: query
        name: sortOrder
        description: Sort direction
      responses:
        200:
          description: OK
      tags:
      - Words
      - ReverseDictionary
  /words.json/search/{query}:
    get:
      summary: Searches words
      description: Searches words.
      operationId: searchWords
      x-api-path-slug: words-jsonsearchquery-get
      parameters:
      - in: query
        name: caseSensitive
        description: Search case sensitive
      - in: query
        name: excludePartOfSpeech
        description: Exclude these comma-delimited parts of speech
      - in: query
        name: includePartOfSpeech
        description: Only include these comma-delimited parts of speech
      - in: query
        name: limit
        description: Maximum number of results to return
      - in: query
        name: maxCorpusCount
        description: Maximum corpus frequency for terms
      - in: query
        name: maxDictionaryCount
        description: Maximum dictionary definition count
      - in: query
        name: maxLength
        description: Maximum word length
      - in: query
        name: minCorpusCount
        description: Minimum corpus frequency for terms
      - in: query
        name: minDictionaryCount
        description: Minimum number of dictionary entries for words returned
      - in: query
        name: minLength
        description: Minimum word length
      - in: path
        name: query
        description: Search query
      - in: query
        name: skip
        description: Results to skip
      responses:
        200:
          description: OK
      tags:
      - Words
      - Search
      - Query
  /words.json/wordOfTheDay:
    get:
      summary: Returns a specific WordOfTheDay
      description: Returns a specific wordoftheday.
      operationId: getWordOfTheDay
      x-api-path-slug: words-jsonwordoftheday-get
      parameters:
      - in: query
        name: date
        description: Fetches by date in yyyy-MM-dd
      responses:
        200:
          description: OK
      tags:
      - Words
      - WordOfTheDay