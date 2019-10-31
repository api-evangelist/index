{
  "info": {
    "name": "Oxford Dictionaries Find translation results for search query.",
    "_postman_id": "9058ff6d-5f80-4fd7-bdac-cb008804d9bc",
    "description": "Find available translation results  for a search query and language.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Domains",
      "item": [
        {
          "id": "753ea213-de8c-4704-876d-41e44be664c7",
          "name": "getDomainsSourceDomainsLanguageTargetDomainsLanguage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "domains/:source_domains_language/:target_domains_language"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_domains_language",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "target_domains_language",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the available [domains](documentation/glossary?term=domain) for a given bilingual language dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00457fd3-45e4-4edf-8473-8ac625922304"
            }
          ]
        },
        {
          "id": "5911ff47-f452-4f1f-a5d4-1b9918d6f3d8",
          "name": "getDomainsSourceLanguage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "domains/:source_language"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_language",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the available [domains](documentation/glossary?term=domain) for a given monolingual language dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39cd4146-4710-4242-8a1c-9d7b732c09ec"
            }
          ]
        },
        {
          "id": "4b860855-acbc-4e7c-bc7b-c90521913693",
          "name": "getDomainsSourceLanguageTargetLanguage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "domains/:source_language/:target_language"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_language",
                  "value": "source_language",
                  "type": "string"
                },
                {
                  "id": "target_language",
                  "value": "target_language",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the available [domains](/glossary?tag=#domains&expand) for a given bilingual language dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50696b2d-b332-4521-9887-f1a3e20faf04"
            }
          ]
        }
      ]
    },
    {
      "name": "Entries",
      "item": [
        {
          "id": "1a88d77f-76c5-4f52-9e05-8c13f64b3d75",
          "name": "getEntriesSourceLanguageWordSentences",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "entries/:source_language/:word_id/sentences"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_language",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "word_id",
                  "value": "word_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Use this to retrieve sentences extracted from  corpora which show how a word is used in the language. This is available for English and Spanish. For English, the sentences are linked to the correct [sense](documentation/glossary?term=sense) of the word in the dictionary. In Spanish, they are linked at the [headword](documentation/glossary?term=headword) level."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55be362d-1d19-4db1-84a6-b8a792c4a72d"
            }
          ]
        },
        {
          "id": "d0e2decc-ec33-4e9b-a780-66c9fe27d1af",
          "name": "getEntriesSourceLangWord",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "entries/:source_lang/:word_id"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_lang",
                  "value": "source_lang",
                  "type": "string"
                },
                {
                  "id": "word_id",
                  "value": "word_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Use this to retrieve definitions, [pronunciations](documentation/glossary?term=pronunciation), example sentences, [grammatical information](documentation/glossary?term=grammaticalfeatures) and [word origins](documentation/glossary?term=etymology). It only works for dictionary [headwords](documentation/glossary?term=headword), so you may need to use the [Lemmatron](documentation/glossary?term=lemma) first if your input is likely to be an [inflected](documentation/glossary?term=inflection) form (e.g., 'swimming'). This would return the linked [headword](documentation/glossary?term=headword) (e.g., 'swim') which you can then use in the Entries endpoint. Unless specified using a region filter, the default lookup will be the Oxford Dictionary of English (GB)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "211eeef4-a4d4-426d-a2ce-dd795c418840"
            }
          ]
        },
        {
          "id": "7d0e7efd-27c8-45f8-910f-e9fa905d53a6",
          "name": "getEntriesSourceLangWordAntonyms",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "entries/:source_lang/:word_id/antonyms"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_lang",
                  "value": "source_lang",
                  "type": "string"
                },
                {
                  "id": "word_id",
                  "value": "word_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve words that are opposite in meaning to the input word ([antonym](documentation/glossary?term=thesaurus))."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31a09f12-f542-4696-acf1-fe76fb3b2f32"
            }
          ]
        },
        {
          "id": "ba448b1f-ba3d-4fdd-ae22-df5fb641ee79",
          "name": "getEntriesSourceLangWordRegionsRegion",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "entries/:source_lang/:word_id/regions=:region"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "region",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "source_lang",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "word_id",
                  "value": "word_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "USe this filter to restrict the lookup to either our Oxford Dictionary of English (GB) or New Oxford American Dictionary (US)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ff6ab52-11d6-4c6c-bb4b-21f571e39595"
            }
          ]
        },
        {
          "id": "bf4a1293-2a23-4df8-ac97-93cf13fc30da",
          "name": "getEntriesSourceLangWordSynonyms",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "entries/:source_lang/:word_id/synonyms"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_lang",
                  "value": "source_lang",
                  "type": "string"
                },
                {
                  "id": "word_id",
                  "value": "word_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Use this to retrieve words that are similar in meaning to the input word ([synonym](documentation/glossary?term=synonym))."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3b0d657-c17e-41df-a994-7ea937351da8"
            }
          ]
        },
        {
          "id": "07825980-2c5f-4eff-b9f8-586fa20d0249",
          "name": "getEntriesSourceLangWordSynonyms;antonyms",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "entries/:source_lang/:word_id/synonyms;antonyms"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_lang",
                  "value": "source_lang",
                  "type": "string"
                },
                {
                  "id": "word_id",
                  "value": "word_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve available [synonyms](documentation/glossary?term=thesaurus) and [antonyms](documentation/glossary?term=thesaurus) for a given word and language."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54d77829-ed71-4a39-9146-05ac18f38e9c"
            }
          ]
        },
        {
          "id": "542fee08-b007-40d0-938c-7fd9da48cb72",
          "name": "getEntriesSourceLangWordFilters",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "entries/:source_lang/:word_id/:filters"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_lang",
                  "value": "source_lang",
                  "type": "string"
                },
                {
                  "id": "word_id",
                  "value": "word_id",
                  "type": "string"
                },
                {
                  "id": "filters",
                  "value": "filters",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Use filters to limit the [entry](documentation/glossary?term=entry) information that is returned. For example, you may only require definitions and not everything else, or just [pronunciations](documentation/glossary?term=pronunciation). The full list of filters can be retrieved from the filters Utility endpoint. You can also specify values within the filter using '='. For example 'grammaticalFeatures=singular'. Filters can also be combined using a semicolon."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f531c5b2-0d34-4e83-a8dc-2f8ee532f0f8"
            }
          ]
        },
        {
          "id": "b598e6ff-4cb6-4a65-996e-1a903ac29c26",
          "name": "getEntriesSourceTranslationLanguageWordTranslationsTargetTranslationLanguage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "entries/:source_translation_language/:word_id/translations=:target_translation_language"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_translation_language",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "target_translation_language",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "word_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Use this to return translations for a given word. In the event that a word in the dataset does not have a direct translation, the response will be a [definition](documentation/glossary?term=entry) in the target language."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f03708c5-007b-4f47-92c8-4e6670cf85ef"
            }
          ]
        },
        {
          "id": "26185508-dabb-4bb5-bf91-da57c08cb655",
          "name": "getEntriesSourceLangWordDefinitions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "entries/:source_lang/:word_id/definitions"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_lang",
                  "value": "source_lang",
                  "type": "string"
                },
                {
                  "id": "word_id",
                  "value": "word_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Find available [dictionary entries](/glossary?tag=#entry&expand) for given word and language. Filter results by categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5019cf44-3dae-4676-955b-dddfe2f4bebc"
            }
          ]
        },
        {
          "id": "56118a3d-ae50-4774-b1da-579f9787502f",
          "name": "getEntriesSourceLangWordExamples",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "entries/:source_lang/:word_id/examples"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_lang",
                  "value": "source_lang",
                  "type": "string"
                },
                {
                  "id": "word_id",
                  "value": "word_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Find available [dictionary entries](/glossary?tag=#entry&expand) for given word and language. Filter results by categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c744900-ef3a-4878-bf01-b805449af93d"
            }
          ]
        },
        {
          "id": "81225541-b8eb-4102-b924-84e151bcedd5",
          "name": "getEntriesSourceLangWordPronunciations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "entries/:source_lang/:word_id/pronunciations"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_lang",
                  "value": "source_lang",
                  "type": "string"
                },
                {
                  "id": "word_id",
                  "value": "word_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Find available [dictionary entries](/glossary?tag=#entry&expand) for given word and language. Filter results by categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb20d3fc-51f6-4b8d-8c42-c3f280562845"
            }
          ]
        },
        {
          "id": "4771e266-f0e9-4d95-8a1b-191140c90a44",
          "name": "getEntriesSourceLangWordTranslationsTargetLang",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "entries/:source_lang/:word_id/translations=:target_lang"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "word_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "source_lang",
                  "value": "source_lang",
                  "type": "string"
                },
                {
                  "id": "target_lang",
                  "value": "target_lang",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns target language translations for a given word ID and source language. \nIn the event that a word in the dataset does not have a direct translation, the response will be a [definition](/glossary?tag=#entry&expand) in the target language."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37f0dc01-8b9f-4a74-b759-b0f909c52fbd"
            }
          ]
        }
      ]
    },
    {
      "name": "Filters",
      "item": [
        {
          "id": "e1a55cf0-4259-41b8-a3be-1d0bb8b70eaa",
          "name": "getFilters",
          "request": {
            "url": "http://od-api-demo.oxforddictionaries.com:443/api/v1/filters?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all the valid filters to construct API calls."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8cfc3f9d-a9d2-4534-93ed-9350300bbdd5"
            }
          ]
        },
        {
          "id": "bf582f3c-75b0-4493-bd2d-d6b8ea637dbe",
          "name": "getFiltersEndpoint",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "filters/:endpoint"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "endpoint",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all the valid filters for a given endpoint to construct API calls."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08bf1617-c1a0-4fd2-9277-50370561d819"
            }
          ]
        }
      ]
    },
    {
      "name": "GrammaticalFeatures",
      "item": [
        {
          "id": "1dc6fa1e-6d58-48b9-9d9c-d3aa78a16901",
          "name": "getGrammaticalfeaturesSourceLanguage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "grammaticalFeatures/:source_language"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_language",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the available [grammatical features](documentation/glossary?term=grammaticalfeatures) for a given language dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79f04706-1bba-48d3-9a6e-e80a1a649130"
            }
          ]
        }
      ]
    },
    {
      "name": "Inflections",
      "item": [
        {
          "id": "b95004eb-d0ef-4720-b76d-027e2115337b",
          "name": "getInflectionsSourceLangWord",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "inflections/:source_lang/:word_id"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "word_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "source_lang",
                  "value": "source_lang",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Use this to check if a word exists in the dictionary, or what 'root' form it links to (e.g., swimming > swim). The response tells you the possible [lemmas](documentation/glossary?term=lemma) for a given [inflected](documentation/glossary?term=inflection) word. This can then be combined with other endpoints to retrieve more information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d406d550-3f9d-4142-be9c-86f36467c8fe"
            }
          ]
        },
        {
          "id": "4d924ed5-00a0-48d1-91c9-c62fba9528d8",
          "name": "getInflectionsSourceLangWordFilters",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "inflections/:source_lang/:word_id/:filters"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "word_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "source_lang",
                  "value": "source_lang",
                  "type": "string"
                },
                {
                  "id": "filters",
                  "value": "filters",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve available [lemmas](documentation/glossary?term=lemma) for a given [inflected](documentation/glossary?term=inflection) wordform. Filter results by categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00482f42-fc85-4bc5-b81c-87df4df7b4b4"
            }
          ]
        }
      ]
    },
    {
      "name": "Languages",
      "item": [
        {
          "id": "865d0f3b-4c5b-473c-87ba-a9242b9c0cb3",
          "name": "getLanguages",
          "request": {
            "url": "http://od-api-demo.oxforddictionaries.com:443/api/v1/languages?No Name=%7B%7D&sourceLanguage=%7B%7D&targetLanguage=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of monolingual and bilingual language datasets available in the API"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90c70063-1010-4f63-b3e9-42caf2c83545"
            }
          ]
        }
      ]
    },
    {
      "name": "Lexicalcategories",
      "item": [
        {
          "id": "8ed6826f-d7fd-4442-92aa-1cb1f0700b87",
          "name": "getLexicalcategoriesLanguage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "lexicalcategories/:language"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "language",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of available [lexical categories](documentation/glossary?term=lexicalcategory) for a given language dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea7748f6-8cc6-4301-9224-fc73f7793342"
            }
          ]
        }
      ]
    },
    {
      "name": "Regions",
      "item": [
        {
          "id": "8ce8c1e8-5ea9-4d28-b9c2-f8a54b0b4786",
          "name": "getRegionsSourceLanguage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "regions/:source_language"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_language",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the available [regions](documentation/glossary?term=regions) for a given monolingual language dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2811b022-7b28-4b36-ac5f-4934a2e4fb9b"
            }
          ]
        }
      ]
    },
    {
      "name": "Registers",
      "item": [
        {
          "id": "51c48d1b-e49c-44c1-be28-eae011c42d33",
          "name": "getRegistersSourceLanguage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "registers/:source_language"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_language",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the available [registers](documentation/glossary?term=registers) for a given monolingual language dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4afc683d-a87d-4feb-a52d-49efe641ef11"
            }
          ]
        },
        {
          "id": "0d6a3813-79b3-44dc-9e1d-0dc486eff4d8",
          "name": "getRegistersSourceRegisterLanguageTargetRegisterLanguage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "registers/:source_register_language/:target_register_language"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_register_language",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "target_register_language",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the available [registers](documentation/glossary?term=registers) for a given bilingual language dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4c0092c-bad6-45d2-8e9c-50b8ad0eb657"
            }
          ]
        },
        {
          "id": "ae55ff94-a3a4-4e92-b6a7-6c5cbbd99a52",
          "name": "getRegistersSourceLanguageTargetLanguage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "registers/:source_language/:target_language"
              ],
              "port": "443",
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_language",
                  "value": "source_language",
                  "type": "string"
                },
                {
                  "id": "target_language",
                  "value": "target_language",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the available [registers](/glossary?tag=#registers&expand) for a given bilingual language dataset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5756aaf8-ca92-4d89-85cd-006d3ecc67ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "3653e546-ece8-4429-8c16-cb2578cd45b6",
          "name": "getSearchSourceLang",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "search/:source_lang"
              ],
              "port": "443",
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "prefix",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "q",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "regions",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_lang",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Use this to retrieve possible [headword](documentation/glossary?term=headword) matches for a given string of text. The results are culculated using headword matching, fuzzy matching, and [lemmatization](documentation/glossary?term=lemma)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aeacbad2-d1b6-4b07-8b4c-c91db4c30841"
            }
          ]
        },
        {
          "id": "d715af2c-b18d-442c-87e6-9dc3a915e8b1",
          "name": "getSearchSourceSearchLanguageTranslationsTargetSearchLanguage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "search/:source_search_language/translations=:target_search_language"
              ],
              "port": "443",
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "prefix",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "q",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "regions",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_search_language",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "target_search_language",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Use this to find matches in our translation dictionaries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc1e036d-ade3-433e-bad0-8b10e2cf1a98"
            }
          ]
        },
        {
          "id": "17728e24-01ab-461c-8bee-9c0611c02942",
          "name": "getSearchSourceLangTranslationsTargetLang",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "search/:source_lang/translations=:target_lang"
              ],
              "port": "443",
              "query": [
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "prefix",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "q",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "regions",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_lang",
                  "value": "source_lang",
                  "type": "string"
                },
                {
                  "id": "target_lang",
                  "value": "target_lang",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Find available translation results  for a search query and language."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df4e8749-0327-4058-89cc-7194538658b2"
            }
          ]
        }
      ]
    },
    {
      "name": "Stats",
      "item": [
        {
          "id": "3c4ed651-0c94-4616-a858-b9b173b438fe",
          "name": "getStatsFrequencyNgramsSourceLangCorpusNgramSize",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "stats/frequency/ngrams/:source_lang/:corpus/:ngram-size/"
              ],
              "port": "443",
              "query": [
                {
                  "key": "contains",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxDocumentFrequency",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxFrequency",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "minDocumentFrequency",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "minFrequency",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "punctuation",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tokens",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "corpus",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "ngram-size",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "source_lang",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint returns frequencies of ngrams of size 1-4. That is the number of times a word (ngram size = 1) or words (ngram size > 1) appear in the corpus. Ngrams are case sensitive (\"I AM\" and \"I am\" will have different frequency) and frequencies are calculated per word (true case) so \"the book\" and \"the books\" are two different ngrams. The results can be filtered based on query parameters.   Parameters can be provided in PATH, GET or POST (form or json). The parameters in PATH are overriden by parameters in GET, POST and json (in that order). In PATH, individual options are separated by semicolon and values are separated by commas (where multiple values can be used).   Example for bigrams (ngram of size 2):\n* PATH: /tokens=a word,another word\n* GET: /?tokens=a word&tokens=another word\n* POST (json):\n\n  ```javascript\n    {\n        \"tokens\": [\"a word\", \"another word\"]\n    }\n  ```"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60df4c40-6563-4bac-8e87-5970aba12259"
            }
          ]
        },
        {
          "id": "4ffa96e9-c75e-4e9f-b855-f01f2bf1405d",
          "name": "getStatsFrequencyWordSourceLang",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "stats/frequency/word/:source_lang/"
              ],
              "port": "443",
              "query": [
                {
                  "key": "corpus",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lemma",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lexicalCategory",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "trueCase",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "wordform",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_lang",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint provides the frequency of a given word. When multiple database records match the query parameters, the returned frequency is the sum of the individual frequencies. For example, if the query parameters are lemma=test, the returned frequency will include the verb \"test\", the noun \"test\" and the adjective \"test\" in all forms (Test, tested, testing, etc.)   If you are interested in the frequency of the word \"test\" but want to exclude other forms (e.g., tested) use the option trueCase=test. Normally, the word \"test\" will be spelt with a capital letter at the beginning of a sentence. The option trueCase will ignore this and it will count \"Test\" and \"test\" as the same token. If you are interested in frequencies of \"Test\" and \"test\", use the option wordform=test or wordform=Test. Note that trueCase is not just a lower case of the word as some words are genuinely spelt with a capital letter such as the word \"press\" in Oxford University Press.   Parameters can be provided in PATH, GET or POST (form or json). The parameters in PATH are overriden by parameters in GET, POST and json (in that order). In PATH, individual options are separated by semicolon and values are separated by commas (where multiple values can be used). Examples:\n* PATH: /lemma=test;lexicalCategory=noun\n* GET: /?lemma=test&lexicalCategory=noun\n* POST (json):\n\n  ```javascript\n    {\n      \"lemma\": \"test\",\n      \"lexicalCategory\": \"noun\"\n    }\n  ```\n\n One of the options wordform/trueCase/lemma/lexicalCategory has to be provided."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9fb4e648-a85c-459a-aea1-9c793fd98cdc"
            }
          ]
        },
        {
          "id": "5b31dff5-168f-4f75-9a22-0bd51609b8b1",
          "name": "getStatsFrequencyWordsSourceLang",
          "request": {
            "url": {
              "protocol": "http",
              "host": "od-api-demo.oxforddictionaries.com",
              "path": [
                "api",
                "v1",
                "stats/frequency/words/:source_lang/"
              ],
              "port": "443",
              "query": [
                {
                  "key": "corpus",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "grammaticalFeatures",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lemma",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lexicalCategory",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxFrequency",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxNormalizedFrequency",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "minFrequency",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "minNormalizedFrequency",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "trueCase",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "wordform",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "source_lang",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint provides a list of frequencies for a given word or words. Unlike the /word/ endpoint, the results are split into the smallest units.   To exclude a specific value, prepend it with the minus sign ('-'). For example, to get frequencies of the lemma 'happy' but exclude superlative forms (i.e., happiest) you could use options 'lemma=happy;grammaticalFeatures=-degreeType:superlative'.   Parameters can be provided in PATH, GET or POST (form or json). The parameters in PATH are overriden by parameters in GET, POST and json (in that order). In PATH, individual options are separated by semicolon and values are separated by commas (where multiple values can be used).   The parameters wordform/trueCase/lemma/lexicalCategory also exist in a plural form, taking a lists of items. Examples:\n* PATH: /wordforms=happy,happier,happiest\n* GET: /?wordforms=happy&wordforms=happier&wordforms=happiest\n* POST (json):\n```javascript\n  {\n    \"wordforms\": [\"happy\", \"happier\", \"happiest\"]\n  }\n```\n Aside from individual frequency requests, users can also post a list of items for which they would like to get frequencies. The list has to be uploaded in json and the required fields are \"items\" and \"collate\".   The field \"items\" is a list of items for which you want the frequencies. The content of the items depends on the option for \"collate\". The value of \"collate\" should be a list of \"columns\" that the items contain. The list is limited to combinations of \"wordform\", \"lemma\", \"trueCase\" and \"lexicalCategory\". The fields that are listed in the \"collate\" options have to be present in each item. Here are some examples of queries:\n* ### Get frequencies of provided wordforms:\n```javascript\n  {\n      \"collate\": [\"wordform\"],\n      \"items\": [{\"wordform\": \"test\"}, {\"wordform\": \"Test\"}]\n  }\n```\n* ### Get frequencies of provided lemmas:\n```javascript\n  {\n      \"collate\": [\"lemma\"],\n      \"items\": [{\"lemma\": \"test\"}, {\"lemma\": \"Test\"}]\n  }\n```\n* ### Get frequencies of provided lemmas per lexical category:\n```javascript\n  {\n      \"collate\": [\"lemma\", \"lexicalCategory\"],\n      \"items\": [\n          {\"lemma\": \"test\", \"lexicalCategory\": \"verb\"},\n