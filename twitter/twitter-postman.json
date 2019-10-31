{
  "info": {
    "name": "Twitter Get Rate Limit Sttaus",
    "_postman_id": "990a6b86-d6ac-4330-8ccf-7c1cd0e547c8",
    "description": "Returns the current rate limits for methods belonging to the specified resource families",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Social",
      "item": [
        {
          "id": "d7f4dd0c-f59b-4372-9790-21e5829ce6a1",
          "name": "returns-the-20-most-recent-mentions-for-the-authenticating-user",
          "request": {
            "url": "http://api.twitter.com/1.1/statuses/mentions_timeline?contributor_details=%7B%7D&count=%7B%7D&include_entities=%7B%7D&max_id=%7B%7D&since_id=%7B%7D&trim_user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the 20 most recent mentions for the authenticating user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd57664b-0707-4cd6-86b3-3fc14dd174c7"
            }
          ]
        },
        {
          "id": "8aec52f2-7b18-4717-86a6-480581bc5ce5",
          "name": "returns-a-collection-of-the-most-recent-tweets-posted-by-the-user",
          "request": {
            "url": "http://api.twitter.com/1.1/statuses/user_timeline.json?contributor_details=%7B%7D&count=%7B%7D&exclude_replies=%7B%7D&include_rts=%7B%7D&max_id=%7B%7D&screen_name=screen_name&since_id=%7B%7D&trim_user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a collection of the most recent Tweets posted by the User"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fcd2c85c-4342-45ae-a735-bbf3f7606aea"
            }
          ]
        },
        {
          "id": "516dad99-29e7-4083-a315-83c361f061a6",
          "name": "returns-a-collection-of-the-most-recent-tweets",
          "request": {
            "url": "http://api.twitter.com/1.1/statuses/home_timeline?contributor_details=%7B%7D&exclude_replies=%7B%7D&max_id=%7B%7D&since_id=%7B%7D&trim_user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a collection of the most recent Tweets"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08aaa713-243c-4f60-8afa-914088e7585d"
            }
          ]
        },
        {
          "id": "a8b7e03b-1c55-4253-bd72-ef0518eae5fb",
          "name": "retweens-a-tweet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twitter.com",
              "path": [
                "1.1",
                "statuses/retweets/:id"
              ],
              "query": [
                {
                  "key": "trim_user",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Retweens a tweet"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a31c6b0-d60b-45ae-8d19-91da5e2e94ce"
            }
          ]
        },
        {
          "id": "a8345f36-33f7-4a38-b98c-db81a5a88a10",
          "name": "retruns-a-single-tweet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twitter.com",
              "path": [
                "1.1",
                "statuses/show/:id"
              ],
              "query": [
                {
                  "key": "include_entities",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_my_retweet",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "trim_user",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retruns a single Tweet"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78b16284-74f6-42ac-9eb2-4e70eda6dbcb"
            }
          ]
        },
        {
          "id": "376bf706-c182-4009-94ce-03bad8485671",
          "name": "destroys-the-status-specified-by-the-required-id-parameter",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twitter.com",
              "path": [
                "1.1",
                "statuses/destroy/:id"
              ],
              "query": [
                {
                  "key": "trim_user",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Destroys the status specified by the required ID parameter"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15bbe249-7153-47ba-b579-925aff7617ed"
            }
          ]
        },
        {
          "id": "5b0c9355-30d4-4e2b-a126-d04f67b5045b",
          "name": "updates-the-authenticating-users-status",
          "request": {
            "url": "http://api.twitter.com/1.1/statuses/update?display_coordinates=%7B%7D&in_reply_to_status_id=%7B%7D&lat=%7B%7D&long=%7B%7D&place_id=%7B%7D&status=%7B%7D&trim_user=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the authenticating user's status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39f40351-7370-43f3-bd85-91acdab4223d"
            }
          ]
        },
        {
          "id": "1394ac7f-1b86-4c41-acde-5546808625f1",
          "name": "returns-information-allowing-the-creation-of-an-embedded-representation",
          "request": {
            "url": "http://api.twitter.com/1.1/statuses/oembed?align=%7B%7D&hide_media=%7B%7D&hide_thread=%7B%7D&id=%7B%7D&lang=%7B%7D&maxwidth=%7B%7D&related=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information allowing the creation of an embedded representation"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b59b8d1-cbaf-4438-a5b7-0e4d7c50d99d"
            }
          ]
        },
        {
          "id": "2dd4ec14-999c-4424-baa9-895087db69f3",
          "name": "return-all-lists-the-authenticating-or-specified-user-subscribes-to-including-their-own",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/list?screen_name=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return all lists the authenticating or specified user subscribes to, including their own."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b3f9c0d-d4b8-455c-95ae-80aacc1c3322"
            }
          ]
        },
        {
          "id": "8bfc7fcc-860d-46fe-a292-1a8324000bcb",
          "name": "returns-a-timeline-of-tweets-authored-by-memebers-of-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/statuses.json?count=%7B%7D&include_entities=%7B%7D&include_rts=%7B%7D&list_id=%7B%7D&max_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&since_id=%7B%7D&slug=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a timeline of tweets authored by memebers of the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b0f0ca1-1937-4070-8df2-0e2f251c8285"
            }
          ]
        },
        {
          "id": "12a279cc-539b-4b67-bc91-bd86d4059c9e",
          "name": "returns-the-list-of-memebers-destroy",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/members/destroy?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&slug=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of memebers destroy"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d25c9a98-72de-4551-99ac-1ab3cbf82ff2"
            }
          ]
        },
        {
          "id": "a1b9f686-0fab-44d3-a989-87247ef3f6e3",
          "name": "returns-the-lists-of-the-specified-user-has-been-added-to",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/memberships?cursor=%7B%7D&filter_to_owned_lists=%7B%7D&screen_name=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the lists of the specified user has been added to"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9582f962-4e2b-4585-a0a9-ea31d3bee2a5"
            }
          ]
        },
        {
          "id": "c85a6d95-1c8d-4282-afbe-34d147205ce2",
          "name": "returns-the-subscribers-of-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/subscribers?cursor=%7B%7D&include_entities=%7B%7D&list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&skip_status=%7B%7D&slug=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the subscribers of the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f481a41f-2350-4259-98a6-2e609dbb3d40"
            }
          ]
        },
        {
          "id": "2e949b87-8f39-4c2b-9113-c35403f0d7cc",
          "name": "subscribes-the-authenticated-user-to-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/subscribers/create?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&slug=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Subscribes the authenticated user to the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c8d29ac-6829-447d-821f-a67c38515f71"
            }
          ]
        },
        {
          "id": "6b34daaa-fd1c-486b-b479-a7a927e33054",
          "name": "check-if-the-specified-user-is-a-subscriber-of-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/subscribers/show?include_entities=%7B%7D&list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&skip_status=%7B%7D&slug=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Check if the specified user is a subscriber of the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "632947fe-c7c1-4f6d-877a-76f985b4aaec"
            }
          ]
        },
        {
          "id": "1e702c15-29e9-472a-a7f9-45c8db530224",
          "name": "returns-list-of-subscribers-destroy",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/subscribers/destroy?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&slug=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of subscribers destroy"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c3b2222-1978-42b6-b014-f14ca2d59776"
            }
          ]
        },
        {
          "id": "1796788a-669c-4921-811d-d0b6d6e68931",
          "name": "returns-lists-of-members-create-all",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/members/create_all?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&slug=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns lists of members create_all"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "895478fe-b2f6-44f4-b10f-232083d8a776"
            }
          ]
        },
        {
          "id": "399976de-8d34-4820-8b21-908314f4fd69",
          "name": "check-if-the-specified-user-is-a-member-of-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/list/members/show?include_entities=%7B%7D&list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&skip_status=%7B%7D&slug=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Check if the specified user is a member of the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79fbe94f-cb41-496a-ba67-1313551ff241"
            }
          ]
        },
        {
          "id": "3452ae2f-cff0-438e-b0be-0ef06617dd81",
          "name": "returns-the-members-of-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/list/members?cursor=%7B%7D&include_entities=%7B%7D&list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&skip_status=%7B%7D&slug=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the members of the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b5d2dd6-ea79-4079-8434-8481adc64e3f"
            }
          ]
        },
        {
          "id": "92b8a1d6-c967-42a6-9910-7ef72bb56867",
          "name": "returns-list-of-members-create",
          "request": {
            "url": "http://api.twitter.com/1.1/list/members/create?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&slug=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of members create"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b79f011-df1c-4e0e-963d-9eac68887b2a"
            }
          ]
        },
        {
          "id": "da470e33-1171-4fb3-89d7-aa5213bb0e66",
          "name": "returns-list-of-destroy",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/destroy?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&slug=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of destroy"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64c65ce6-1e25-44dc-87ba-486c13a94b20"
            }
          ]
        },
        {
          "id": "b89a595b-14f7-4d2e-a40b-989bf0ea921b",
          "name": "returns-lists-of-updates",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/update?description=%7B%7D&list_id=%7B%7D&mode=%7B%7D&name=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&slug=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Returns lists of updates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1267636b-588e-4a42-9033-433a876f2ad6"
            }
          ]
        },
        {
          "id": "013759f5-c66a-4e7b-8e71-53d6017db12d",
          "name": "returns-list-of-create",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/create?description=%7B%7D&mode=%7B%7D&name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of create"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd2ebfad-b428-4146-9486-2c5140a8142e"
            }
          ]
        },
        {
          "id": "ca1e54d4-3a6f-4d35-9931-0d81cc09e1a5",
          "name": "returns-list-of-show",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/show?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&slug=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of show"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a50c89a-bbcc-4c3c-9403-a86ea9668aab"
            }
          ]
        },
        {
          "id": "8d2accb4-f290-4aa9-b190-9ce6932c1ee0",
          "name": "returns-list-of-subscriptions",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/subscriptions?count=%7B%7D&cursor=%7B%7D&screen_name=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of subscriptions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8345f3e8-f1e1-4f3e-b299-8dd8ca1afbfa"
            }
          ]
        },
        {
          "id": "020f1055-cd99-4c26-b03a-67e5e64fa8d9",
          "name": "returns-lists-of-destroy-all",
          "request": {
            "url": "http://api.twitter.com/1.1/list/members/destroy_all?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&slug=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns lists of destroy all"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4cd0e45-6274-4a14-b7ce-4c03633fa8e3"
            }
          ]
        },
        {
          "id": "c5f6c1f0-343f-4d7f-821f-d859306a0280",
          "name": "return-20-most-recent-direct-messages-sent",
          "request": {
            "url": "http://api.twitter.com/1.1/direct_messages/sent?count=%7B%7D&include_entities=%7B%7D&max_id=%7B%7D&page=%7B%7D&since_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "return 20 most recent direct messages sent"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b146445-7418-4ad9-ad27-2bf6ed520584"
            }
          ]
        },
        {
          "id": "6478edf9-0ba9-4d36-ae5b-351d86ef0f5f",
          "name": "returns-a-single-direct-message-specified-by-an-id",
          "request": {
            "url": "http://api.twitter.com/1.1/direct_messages/show?id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns a single direct message specified by an id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f88f836-add1-496e-ad53-1c05e529c110"
            }
          ]
        },
        {
          "id": "68220c68-6477-45a4-a7fd-d37bdd296a2e",
          "name": "returns-collection-of-relevant-tweets-matching-query",
          "request": {
            "url": "http://api.twitter.com/1.1/search/tweets.json?callback=%7B%7D&count=%7B%7D&geocode=%7B%7D&include_entities=%7B%7D&lang=%7B%7D&locale=%7B%7D&max_id=%7B%7D&q=%7B%7D&result_type=%7B%7D&since_id=%7B%7D&until=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns collection of relevant Tweets matching query"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60df727e-c0ed-4f8c-bc76-84ebe93f6166"
            }
          ]
        },
        {
          "id": "14b3d9e0-5381-484e-a034-18552c3f33db",
          "name": "returns-the-authenticated-users-saved-search-queries",
          "request": {
            "url": "http://api.twitter.com/1.1/saved_searches/list",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the authenticated user's saved search queries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66186c2e-3dee-448e-9772-e69a0bb58e8a"
            }
          ]
        },
        {
          "id": "71cc9d5f-3521-4e06-947f-f9ad78d9a50a",
          "name": "retrieve-the-information-for-the-saved-search-represented-by-the-given-id",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twitter.com",
              "path": [
                "1.1",
                "saved_searches/show/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the information for the saved search represented by the given id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4fca5b5d-b8dc-4038-a047-e822aaab0ca8"
            }
          ]
        },
        {
          "id": "148a2599-9a5e-4b94-803f-1913944b36f0",
          "name": "create-a-new-saved-search-for-the-authenticated-user",
          "request": {
            "url": "http://api.twitter.com/1.1/saved_searches/create?query=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new saved search for the authenticated user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e636e4eb-fe80-43aa-8574-ef943f780cb4"
            }
          ]
        },
        {
          "id": "4f7a0e99-c611-4e27-924e-5c42aa359657",
          "name": "destroy-a-saved-search-for-the-authenticating-user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twitter.com",
              "path": [
                "1.1",
                "saved_searches/destroy/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Destroy a saved search for the authenticating user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed298171-0452-44a8-a8d9-afcf30ea17bc"
            }
          ]
        },
        {
          "id": "b69ef54d-ee65-4714-a90c-fefa7c3826ca",
          "name": "return-20-most-recent-direct-messages-sent-to-user",
          "request": {
            "url": "http://api.twitter.com/1.1/direct_messages?include_entities=%7B%7D&max_id=%7B%7D&since_id=%7B%7D&skip_status=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "return 20 most recent direct messages sent to user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "741378c7-d5db-4d7c-b3e6-758003068e0a"
            }
          ]
        },
        {
          "id": "f213a00b-0135-4d0a-a283-806bb4dc8958",
          "name": "destroys-direct-messages-specified-in-required-id",
          "request": {
            "url": "http://api.twitter.com/1.1/direct_messages/destroy?id=%7B%7D&include_entities=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "destroys direct messages specified in required ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a6f6194-5314-458e-9064-f6659b83f106"
            }
          ]
        },
        {
          "id": "d5ccf9be-c8bf-477a-ac92-c724cb52ac67",
          "name": "sends-a-new-direct-message-to-specified-user",
          "request": {
            "url": "http://api.twitter.com/1.1/direct_messages/new?screen_name=%7B%7D&text=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "sends a new direct message to specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6efaf95-731f-42c5-9960-4f682544eb68"
            }
          ]
        },
        {
          "id": "5ab8a281-7fd7-4617-a04f-94a92823245c",
          "name": "returns-a-cursored-collection-of-user-ids-followed-by-user",
          "request": {
            "url": "http://api.twitter.com/1.1/friends/ids?count=%7B%7D&cursor=%7B%7D&screen_name=%7B%7D&stringify_ids=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns a cursored collection of user IDs followed by user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c801c49b-611e-4f0a-8abd-caa736a50883"
            }
          ]
        },
        {
          "id": "5fa265d4-acbe-4b8b-a08e-24a80b593b3c",
          "name": "returns-a-cursored-collection-of-user-ids-following-the-user",
          "request": {
            "url": "http://api.twitter.com/1.1/followers/ids?count=%7B%7D&cursor=%7B%7D&screen_name=%7B%7D&stringify_ids=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns a cursored collection of user IDs following the user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3edf8e9-4f25-4642-92a8-f7f6029a70c4"
            }
          ]
        },
        {
          "id": "4368acd2-b22d-4c30-b884-7d3369688a5b",
          "name": "returns-collection-of-ids-of-users-with-pending-follow-request",
          "request": {
            "url": "http://api.twitter.com/1.1/friendships/incoming?cursor=%7B%7D&stringify_ids=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns collection of IDs of users with pending follow request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ae78f48-2761-4f82-8934-b55d5764fe62"
            }
          ]
        },
        {
          "id": "204548ab-30ee-462c-8c61-546ee0c684c6",
          "name": "returns-collection-of-ids-of-users-with-pending-follow-request-from-the-user",
          "request": {
            "url": "http://api.twitter.com/1.1/friendships/outgoing?cursor=%7B%7D&stringify_ids=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns collection of IDs of users with pending follow request from the user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e5b55f7-7d68-44a5-a9e3-10dd2f8c3314"
            }
          ]
        },
        {
          "id": "8c608446-ef61-4d6b-ad5b-94813cf80ab0",
          "name": "allows-users-to-follow-user-sepcified-by-id",
          "request": {
            "url": "http://api.twitter.com/1.1/friendships/create?follow=%7B%7D&screen_name=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "allows users to follow user sepcified by ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82b181fe-306f-4be5-bcdc-0af3a85be066"
            }
          ]
        },
        {
          "id": "ef06382e-f7f3-4d91-b3fd-052b32892d00",
          "name": "allows-user-to-unfollow-user-psecified-by-id",
          "request": {
            "url": "http://api.twitter.com/1.1/friendships/destroy?screen_name=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "allows user to unfollow user psecified by ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e700257-4ea0-42c5-83f8-a2d2a1c072da"
            }
          ]
        },
        {
          "id": "832e7187-8b78-470a-ad16-707dcae4e6b3",
          "name": "allows-one-to-enable-or-disable-settings-for-specified-user",
          "request": {
            "url": "http://api.twitter.com/1.1/friendships/update?device=%7B%7D&retweets=%7B%7D&screen_name=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Allows one to enable or disable settings for specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "813b5c4c-67c2-4370-88e9-fa12b5f43179"
            }
          ]
        },
        {
          "id": "b3ca461e-204d-44c9-8b67-0dded7b49163",
          "name": "returns-detailed-info-about-relationship-between-two-users",
          "request": {
            "url": "http://api.twitter.com/1.1/friendships/show?source_id=%7B%7D&source_screen_name=%7B%7D&target_id=%7B%7D&target_screen_name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns detailed info about relationship between two users"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42071ef2-8b95-43b2-b771-c72b2e72be38"
            }
          ]
        },
        {
          "id": "e1788f04-f113-4147-878f-e73da2a1df4d",
          "name": "returns-settings-for-user",
          "request": {
            "url": "http://api.twitter.com/1.1/account/settings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns settings for user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8cd7bc8d-aa1e-4f34-89f2-9cecdcd4a81c"
            }
          ]
        },
        {
          "id": "401b4940-97c1-48b8-8f5a-ecf2112fbd32",
          "name": "updates-users-settings",
          "request": {
            "url": "http://api.twitter.com/1.1/account/settings?end_sleep_time=%7B%7D&lang=%7B%7D&sleep_time_enabled=%7B%7D&start_sleep_time=%7B%7D&time_zone=%7B%7D&trend_location_woeid=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "updates user's settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a6ffe45-3d87-45e8-bd55-37180be131aa"
            }
          ]
        },
        {
          "id": "7c5d375b-ad82-411e-a7dc-850c0c855c15",
          "name": "sets-which-device-twitter-delivers-updates-to-for-user",
          "request": {
            "url": "http://api.twitter.com/1.1/account/update_delivery_device?device=%7B%7D&include_entities=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "sets which device Twitter delivers updates to for user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f79beed2-4946-4a06-aa44-a07e70f088ec"
            }
          ]
        },
        {
          "id": "884577d0-d92e-4bcb-967b-793ad8c7c223",
          "name": "sets-values-that-users-ar-eable-to-set-under-account-tab",
          "request": {
            "url": "http://api.twitter.com/1.1/account/update_profile?description=%7B%7D&include_entities=%7B%7D&location=%7B%7D&name=%7B%7D&skip_status=%7B%7D&url=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "sets values that users ar eable to set under Account tab"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52c255bc-3f8b-4183-8577-77a9c44809ed"
            }
          ]
        },
        {
          "id": "4cdbca71-6878-4849-8d6a-4993810bbc67",
          "name": "updates-users-profile-background-image",
          "request": {
            "url": "http://api.twitter.com/1.1/account/update_profile_background_image?include_entities=%7B%7D&skip_status=%7B%7D&tile=%7B%7D&use=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "file",
                  "value": "{}",
                  "disabled": false,
                  "description": "image to replace background image of profile"
                }
              ]
            },
            "description": "updates user's profile background image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0fb2d872-977b-44c0-b285-391e9ebd5d67"
            }
          ]
        },
        {
          "id": "ec2e56b5-8495-4f84-9dbb-856740689aac",
          "name": "sets-one-or-more-hex-values-that-controls-color-scheme",
          "request": {
            "url": "http://api.twitter.com/1.1/account/update_profile_colors?include_entities=%7B%7D&profile_background_color=%7B%7D&profile_link_color=%7B%7D&profile_sidebar_border_color=%7B%7D&profile_sidebar_fill_color=%7B%7D&profile_text_color=%7B%7D&skip_status=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "sets one or more hex values that controls color scheme"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7f3213f-a0bc-4868-a11a-f7bd16f8dc1b"
            }
          ]
        },
        {
          "id": "876c741f-4a13-4dd3-9408-3652d094dddf",
          "name": "updates-users-profile-image",
          "request": {
            "url": "http://api.twitter.com/1.1/account/update_profile_image?skip_status=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "image",
                  "value": "{}",
                  "disabled": false,
                  "description": "image to be set as profile image"
                }
              ]
            },
            "description": "updates user's profile image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3918001-14fa-43c9-bc1d-e43c2b428a38"
            }
          ]
        },
        {
          "id": "889d16d5-75f0-45af-a670-3170a5007838",
          "name": "disallows-retweets-and-device-notifications-from-a-user",
          "request": {
            "url": "http://api.twitter.com/1.1/blocks/list?cursor=%7B%7D&include_entities=%7B%7D&skip_status=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "disallows retweets and device notifications from a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bf5f0a2-7b60-40db-8839-6b21cc6002b8"
            }
          ]
        },
        {
          "id": "75742779-fb8d-4437-8d62-3578601638c3",
          "name": "returns-array-of-numeric-user-ids-of-blocked-users",
          "request": {
            "url": "http://api.twitter.com/1.1/blocks/ids?cursor=%7B%7D&stringify_ids=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns array of numeric user ids of blocked users"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b05bbefd-33e3-4089-bbd9-71c4c34dd9cf"
            }
          ]
        },
        {
          "id": "1b393b29-e251-4bc1-91c5-196c1ff253ce",
          "name": "blocks-the-specified-user",
          "request": {
            "url": "http://api.twitter.com/1.1/blocks/create?include_entities=%7B%7D&screen_name=%7B%7D&skip_status=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "blocks the specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb718b42-f4fd-465a-9949-d5a82cac48ec"
            }
          ]
        },
        {
          "id": "dd9133c0-c5d5-4530-b3fe-91babefa2be1",
          "name": "unblocks-the-specified-user",
          "request": {
            "url": "http://api.twitter.com/1.1/blocks/destroy?include_entities=%7B%7D&screen_name=%7B%7D&skip_status=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "un-blocks the specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88684d30-b808-4051-8fa6-d7dc7c0cd566"
            }
          ]
        },
        {
          "id": "3436b581-65e9-459c-a988-96b488223e90",
          "name": "returns-fullyhydrated-user-objects-up-to-100",
          "request": {
            "url": "http://api.twitter.com/1.1/users/lookup?include_entities=%7B%7D&screen_name=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns fully-hydrated user objects up to 100"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "311ec990-e48d-4180-bc9a-b15318e76f76"
            }
          ]
        },
        {
          "id": "6acfd35d-3537-48e6-8adc-389a552d045b",
          "name": "returns-a-variety-of-info-about-specified-user",
          "request": {
            "url": "http://api.twitter.com/1.1/users/show?include_entities=%7B%7D&screen_name=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns a variety of info about specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb999c77-85ce-431f-adb6-035f34e36d6a"
            }
          ]
        },
        {
          "id": "7d5e32bb-b6c7-47ea-af0b-2072f6753430",
          "name": "simple-relevancebased-user-search",
          "request": {
            "url": "http://api.twitter.com/1.1/users/search.json?count=%7B%7D&include_entities=%7B%7D&page=%7B%7D&q=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "simple relevance-based user search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf140e35-f976-4615-873e-e20efec6ce87"
            }
          ]
        },
        {
          "id": "e7d8c563-e01d-4978-8cff-8820dafb1fbe",
          "name": "collection-of-users-specified-user-can-contribute-to",
          "request": {
            "url": "http://api.twitter.com/1.1/users/contributees?include_entities=%7B%7D&screen_name=%7B%7D&skip_status=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "collection of users specified user can contribute to"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68a17838-0076-4a0f-80e2-e9796fea0155"
            }
          ]
        },
        {
          "id": "a8b71cd8-62e0-4c19-88f9-0517211c187a",
          "name": "collection-of-users-that-can-contribute-to-specified-account",
          "request": {
            "url": "http://api.twitter.com/1.1/users/contributors?include_entities=%7B%7D&screen_name=%7B%7D&skip_status=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "collection of users that can contribute to specified account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6058cfac-6875-499f-9e23-7c12a51a5051"
            }
          ]
        },
        {
          "id": "883e0a5f-6e56-4e28-b680-55ea20e3028d",
          "name": "returns-the-top-10-trending-topics-for-a-specific-woeid",
          "request": {
            "url": "http://api.twitter.com/1.1/trends/place.json?exclude=%7B%7D&id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the top 10 trending topics for a specific WOEID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3aba63d-854b-4c07-b22d-04297e71097e"
            }
          ]
        },
        {
          "id": "744d1501-5ba7-4ea3-8343-125a77f61eee",
          "name": "returns-the-availability",
          "request": {
            "url": "http://api.twitter.com/1.1/trends/available.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the availability"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49c478f8-bb51-4fba-ae86-069e7005e795"
            }
          ]
        },
        {
          "id": "77acc9cb-950f-4061-863b-211a10b84da8",
          "name": "returns-the-location-that-twitter-has-trending-topic-information-for",
          "request": {
            "url": "http://api.twitter.com/1.1/trends/closest.json?lat=%7B%7D&long=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the location that Twitter has trending topic information for"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d54eece6-73b4-4670-914d-405ddff998a5"
            }
          ]
        },
        {
          "id": "08b7056f-55f1-4994-a5d3-25cc239421da",
          "name": "returna-users-report-spam",
          "request": {
            "url": "http://api.twitter.com/1.1/users/report_spam?screen_name=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Returna users report spam"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d456e503-f0dd-4650-a852-4eff37df46af"
            }
          ]
        },
        {
          "id": "fe47c4c7-59ff-4b82-ba21-bcc1e8217e2a",
          "name": "returns-the-twitter-terms-of-service",
          "request": {
            "url": "http://api.twitter.com/1.1/help/tos",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the Twitter Terms of Service"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5dc751f9-fbb0-42e4-84ba-f31b959277a0"
            }
          ]
        }
      ]
    },
    {
      "name": "Places",
      "item": [
        {
          "id": "201629d8-3fc8-4890-8e9b-1107d8535e63",
          "name": "returns-all-the-information-about-a-know-place",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twitter.com",
              "path": [
                "1.1",
                "geo/id/:place_id"
              ],
              "variable": [
                {
                  "id": "place_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all the information about a know place"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc23ecab-4b0d-4df8-982d-987d8388fa37"
            }
          ]
        },
        {
          "id": "9f416b3c-c1c8-41c3-b358-4d63413c6e6b",
          "name": "given-a-latitude-and-a-longitude-searches-for-up-to-20-places-that-can-be-used-as-a-place-id-when-up",
          "request": {
            "url": "http://api.twitter.com/1.1/geo/reverse_geoncode?accuracy=%7B%7D&callback=%7B%7D&granularity=%7B%7D&lat=%7B%7D&long=%7B%7D&max_results=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a latitude and a longitude, searches for up to 20 places that can be used as a place_id when updatting a status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ccfcbdda-02e2-4a38-b882-6bbc13309c9d"
            }
          ]
        },
        {
          "id": "fcbca1fc-d057-4c97-80ab-30ac76ba2515",
          "name": "search-for-places-that-can-be-attached-to-a-statusesupdates",
          "request": {
            "url": "http://api.twitter.com/1.1/geo/search?accuracy=%7B%7D&attribute:street_address=%7B%7D&callback=%7B%7D&contained_within=%7B%7D&granularity=%7B%7D&ip=%7B%7D&lat=%7B%7D&long=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search for places that can be attached to a statuses/updates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf58e792-aac2-4708-8805-9e8986121036"
            }
          ]
        },
        {
          "id": "2e1a3540-a670-477c-b983-fbbd255fa954",
          "name": "locates-places-near-the-given-coordinates-which-are-similar-in-name",
          "request": {
            "url": "http://api.twitter.com/1.1/geo/similar_places?attribute:street_address=%7B%7D&callback=%7B%7D&contained_within=%7B%7D&lat=%7B%7D&long=%7B%7D&name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Locates places near the given coordinates which are similar in name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57f8c6cd-f182-4894-985a-95d1edbbbdb8"
            }
          ]
        },
        {
          "id": "c5e7031d-bff4-4c21-9abe-935ab8077156",
          "name": "create-a-new-place-object-at-the-given-latitude-and-logitude",
          "request": {
            "url": "http://api.twitter.com/1.1/geo/places?attribute:street_address=%7B%7D&callback=%7B%7D&contained_within=%7B%7D&lat=%7B%7D&long=%7B%7D&name=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new place object at the given latitude and logitude"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b44b2d7a-a127-4c6a-a1f7-c525411002df"
            }
          ]
        }
      ]
    },
    {
      "name": "Help",
      "item": [
        {
          "id": "893deb0d-71f7-42af-9ed4-5f72d365c92e",
          "name": "returns-the-current-configuration-used-by-twitter-including-twittercom-slugs-which-are-not-usernames",
          "request": {
            "url": "http://api.twitter.com/1.1/help/configuration",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the current configuration used by Twitter including twitter.com slugs which are not usernames"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fd9298ff-4da7-4d2a-870e-88eaddec4950"
            }
          ]
        }
      ]
    },
    {
      "name": "Languages",
      "item": [
        {
          "id": "fbd8e671-1c34-4fe3-bbdc-d016ff8a9f7d",
          "name": "returns-the-list-of-languages-supported-by-twitter-along-with-the-language-code-supported-by-twitter",
          "request": {
            "url": "http://api.twitter.com/1.1/help/languages",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of languages supported by Twitter along with the language code supported by Twitter"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e2dccac-1d6b-44d4-9882-93b68138557e"
            }
          ]
        }
      ]
    },
    {
      "name": "Terms of Service",
      "item": [
        {
          "id": "84a6ff0e-ed0c-4bb6-b526-ac4dad1f5c24",
          "name": "returns-twitters-privacy-policy",
          "request": {
            "url": "http://api.twitter.com/1.1/help/privacy",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns Twitter's privacy policy"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a2b5643-f178-425a-996b-db08a73bf232"
            }
          ]
        }
      ]
    },
    {
      "name": "Rate Limit",
      "item": [
        {
          "id": "8f7ed2fc-9300-4b53-a3e5-f32f6b737dd8",
          "name": "returns-the-current-rate-limits-for-methods-belonging-to-the-specified-resource-families",
          "request": {
            "url": "http://api.twitter.com/1.1/application/rate_limit_status?resources=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the current rate limits for methods belonging to the specified resource families"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "425d8600-aaf7-434b-8a36-2f030a5f3fa2"
            }
          ]
        }
      ]
    }
  ]
}