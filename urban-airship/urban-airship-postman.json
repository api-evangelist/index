{
  "info": {
    "name": "Urban Airship Put Partner Apps App",
    "_postman_id": "9efafd78-07a3-4256-8824-736ab8a381cb",
    "description": "Updates an application.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device",
      "item": [
        {
          "id": "74b4e68a-9a42-49a0-80ab-8c12c7a57fc7",
          "name": "device_tokens.token.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:token"
              ],
              "variable": [
                {
                  "id": "token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a device token???s alias."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b3037d2-8080-485f-bd62-720cf0999ff5"
            }
          ]
        },
        {
          "id": "05b0890f-689e-43c6-aec2-de562c92af4a",
          "name": "device_tokens.token.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:token"
              ],
              "variable": [
                {
                  "id": "token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Registers a device token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0426c6ac-38e0-4bd1-b791-b048a81b334c"
            }
          ]
        },
        {
          "id": "a6530889-d7a1-4387-a3cd-93379ef3114c",
          "name": "device_tokens.token.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:token"
              ],
              "variable": [
                {
                  "id": "token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Marks the device token as inactive. No notifications will be delivered to it until a PUT is executed again. The DELETE returns HTTP 204 No Content, and needs no payload. When a token is deleted in this manner, any alias or tags will be cleared."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f347cd64-c29d-4af3-aa8f-967abba5f2e8"
            }
          ]
        },
        {
          "id": "e6dcdb8c-3ee6-4672-a1a4-a7d8d145bae1",
          "name": "device_tokens.get",
          "request": {
            "url": "http://go.urbanairship.com/api/device_tokens?limit=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about all of your device tokens. If your application has a large number of device tokens, we???ll paginate the request for you. By default, we paginate at 5000 device tokens. You can receive the next page simply by retrieving the URL from \"next_page\" - in this way it is easy to export all of your device tokens and all their data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "824172a1-04b7-4b9c-8f34-4972845e24f7"
            }
          ]
        },
        {
          "id": "339a4991-21ec-416f-87f7-0ca858312a81",
          "name": "device_tokens.count.get",
          "request": {
            "url": "http://go.urbanairship.com/api/device_tokens/count?limit=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the number of device tokens you have registered."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c24573b-f978-4b0e-8274-c882e0175135"
            }
          ]
        },
        {
          "id": "209d1739-7c81-4545-bc29-c3804c9aa77a",
          "name": "device_tokens.feedback.get",
          "request": {
            "url": "http://go.urbanairship.com/api/device_tokens/feedback?since=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets what device tokens are now invalid. Apple informs us when a push notification is sent to a device that can???t receive it because the application has been uninstalled. We mark the device token as inactive and immediately stop sending notifications to that device. Once a day is a good interval for querying the feedback service, but you can do it more often to save on bandwidth from unnecessary notifications. In the response, what does marked_inactive_on mean? Apple sends a timestamp for each device token returned via the feedback service. Since a device can be off the network for a while, this can be a point in the recent past. In order to make this API work smoothly for you, we record the timestamp we marked as inactive. This means you only need to query for data since the last time you queried. Once a day is a good timeframe, or once a week for very small or infrequently used applications. A few times a day is good for applications with heavy use."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66d63900-9f56-4e87-8119-ba49610875ab"
            }
          ]
        },
        {
          "id": "b44ae0be-d361-45e5-878c-9935ab361255",
          "name": "device_pins.pin.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_pins/:pin"
              ],
              "variable": [
                {
                  "id": "pin",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets Device PIN information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f46bd8a-30c3-41e7-83be-b53592227000"
            }
          ]
        },
        {
          "id": "eb987f6a-1742-415c-80fb-3e21b61b8f11",
          "name": "device_pins.pin.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_pins/:pin"
              ],
              "variable": [
                {
                  "id": "pin",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Registers a BlackBerry PIN. This is optional, but recommended, for BlackBerry push messages. This returns HTTP 201 Created for the first registration and 200 OK for any updates. If you wish to include additional information about a device pin, for instance an alias or tags, include a JSON payload along with this request. Not including one of these keys removes it from the device pin."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4617c2c4-f3c6-4027-814f-d0f4b0b0b3c5"
            }
          ]
        },
        {
          "id": "c070d852-9bf3-43cf-a77a-1c667a32530d",
          "name": "device_pins.pin.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_pins/:pin"
              ],
              "variable": [
                {
                  "id": "pin",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Marks a PIN as inactive. No notifications will be delivered to it until a PUT is executed again."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17e8b2c8-b169-49c2-aff8-cedc8b3cc395"
            }
          ]
        },
        {
          "id": "2c4786a5-40df-4cb3-bc61-8c4d3b2d0dc7",
          "name": "device_tokens.device_token.tags.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:device_token/tags"
              ],
              "variable": [
                {
                  "id": "device_token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets tags for a specific device token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "585c4434-e5df-4565-ae48-538863097fbc"
            }
          ]
        },
        {
          "id": "f7b698bf-aa5d-4366-b3fb-e002cc3eb89f",
          "name": "device_tokens.device_token.tags.tag.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:device_token/tags/:tag"
              ],
              "variable": [
                {
                  "id": "device_token",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "tag",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a tag and associate it with the specific device token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "721dd7e8-8d93-40fe-8cd6-8845594aa10d"
            }
          ]
        },
        {
          "id": "8e131342-2b70-43e7-8d9b-206c0cce854c",
          "name": "device_tokens.device_token.tags.tag.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:device_token/tags/:tag"
              ],
              "variable": [
                {
                  "id": "device_token",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "tag",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a single tag from a device token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f235f61d-290d-4fe5-868f-1793a5da6e38"
            }
          ]
        }
      ]
    },
    {
      "name": "Push",
      "item": [
        {
          "id": "69019161-0bf9-4c4d-90a7-79c3858c2fcd",
          "name": "push.post",
          "request": {
            "url": "http://go.urbanairship.com/api/push?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sends a push message to one or more users. Only one of aliases, tags, or device_pins is required, but they can be mixed and matched as much as you???d like."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0bcf32e2-160a-4f6f-b67e-7b52a6928c67"
            }
          ]
        },
        {
          "id": "231df184-3eb8-4849-838e-c03ba04c0d69",
          "name": "push.scheduled.notification.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "push/scheduled/:notification"
              ],
              "variable": [
                {
                  "id": "notification",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels a scheduled notification.  A successful delete will have an HTTP status code of 204. If the scheduled notification does not exist, has already been successfully deleted, or was sent, the status code will be 404."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2468704f-420c-4792-a320-742f857999b7"
            }
          ]
        },
        {
          "id": "133f82d5-41ef-4da2-ba1d-67be2cbbe6bd",
          "name": "push.scheduled.post",
          "request": {
            "url": "http://go.urbanairship.com/api/push/scheduled?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Bulk deletes scheduled notifications. If you include URLs or aliases for scheduled notifications that don???t exist or have already been sent, they will be ignored. Any device token in the cancel_device_tokens payload will have every notification that is sent to it removed. This will not prevent it from receiving scheduled notifications to tags or broadcast messages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8dc82419-5405-4d7c-a308-74f9a12970a8"
            }
          ]
        },
        {
          "id": "23259c7e-6a2d-476e-91d4-5f2665eea295",
          "name": "push.scheduled.alias.alias.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "push/scheduled/alias/:alias"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "alias",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Changes a scheduled notification alias. Aliases for scheduled notifications are unique per Urban Airship application, so you might want to hash the aliases with a device ID or use some other mechanism to ensure uniqueness. The only other limit is that they must be 255 characters or less."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4878a050-cdba-4011-91f4-ef9beb168f1c"
            }
          ]
        },
        {
          "id": "66fff81a-d8d3-4592-b003-b57c9028473b",
          "name": "push.scheduled.alias.alias.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "push/scheduled/alias/:alias"
              ],
              "variable": [
                {
                  "id": "alias",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a scheduled notification alias.  If you attempt to schedule an aliased scheduled notification with an alias that already exists for your application, it will overwrite the existing one."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e88116f8-659b-4cc9-b373-65ecc12f9fbf"
            }
          ]
        },
        {
          "id": "650e8023-057e-43a3-8910-a7397a3bdf1f",
          "name": "push.batch.post",
          "request": {
            "url": "http://go.urbanairship.com/api/push/batch?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sends a push message to all the listed PINs. Each item in the list can contain 0 or many device_pins and 0 or many aliases or tags, and the blackberry payload is in the same format as for individual pushes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f06063a5-1939-460a-b2d5-d5e62cd6facb"
            }
          ]
        },
        {
          "id": "fb63d5ed-c418-4de9-9c0b-38e983f40343",
          "name": "push.broadcast.post",
          "request": {
            "url": "http://go.urbanairship.com/api/push/broadcast?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sends a push message to all active APIDs (Broadcast). Important: The maximum message size is 1024 bytes. This is calculated as the UTF-8 lengths of alert and extra fields together."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3230ba4-3a16-4740-93a7-b83b2448ae03"
            }
          ]
        },
        {
          "id": "6b6b68e3-56d8-48e1-935d-34551eb1dc39",
          "name": "push.stats.get",
          "request": {
            "url": "http://go.urbanairship.com/api/push/stats?end=%7B%7D&format=%7B%7D&start=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns hourly message counts for your application. By default, results are returned in JSON. For CSV, either add the header:Accept:text/csv or append &format=csv to the query string. Times are in UTC, and data is provided for each push platform (currently: iOS, BlackBerry, Android, and C2DM, in that order). The statistics system is updated every 15 minutes, so the final count for an hour will be done at the latest 15 minutes after the hour is done."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7949f811-3e1c-41e4-9190-6ab6d0304d1c"
            }
          ]
        }
      ]
    },
    {
      "name": "Apids",
      "item": [
        {
          "id": "1d4bf7b8-c673-41c6-8abc-9ce8a27004cc",
          "name": "apids.apid.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "apids/:apid"
              ],
              "variable": [
                {
                  "id": "apid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets APID information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f71fa439-c12b-4809-afe3-4c2435138ead"
            }
          ]
        },
        {
          "id": "1695e216-7a1a-4788-8514-ac829356d483",
          "name": "apids.apid.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "apids/:apid"
              ],
              "variable": [
                {
                  "id": "apid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Registers an APID. Unlike registration for iOS and BlackBerry applications, basic registration tying an APID to your application happens automatically. The registration API can be used to set aliases or tags. This returns HTTP 200 OK for any updates. Registering without any body is a no-op. Not including the alias field will clear it. To clear the list of tags, set it to the empty list []. If you are registering an APID to be used with C2DM, you will also need to include a C2DM registration ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ffcf7a1c-f7eb-42db-ae10-7594226508f5"
            }
          ]
        },
        {
          "id": "e480c812-1785-4075-b8b1-b4109fa188cc",
          "name": "apids.apid.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "apids/:apid"
              ],
              "variable": [
                {
                  "id": "apid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Marks an APID as invalid. No notifications will be delivered to it until it re-registers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5de505a-3c14-4058-ba1e-695bbe2334ed"
            }
          ]
        },
        {
          "id": "00c5367b-04fa-4628-95b1-c4afd088d765",
          "name": "apids.get",
          "request": {
            "url": "http://go.urbanairship.com/api/apids?limit=%7B%7D&start=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets APIDs. You can control how many APIDs are returned at a time by using the limit GET argument. The maximum limit is 5000."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "936426fc-e807-415e-b70b-b94d6159a9a8"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "2ce60aa3-75fc-4707-8371-06f27ec93634",
          "name": "user.post",
          "request": {
            "url": "http://go.urbanairship.com/api/user",
            "method": "POST",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new user and returns the credentials."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "499aa538-6ae4-49f4-ab18-b158f39b4bbb"
            }
          ]
        },
        {
          "id": "55ded450-dfeb-4959-abe3-902ca6fc706e",
          "name": "user.user_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves an user???s subscription information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8dac2d58-0bcb-429f-bf55-524c09152890"
            }
          ]
        },
        {
          "id": "d2253c36-4020-433a-bd67-8b15d1e790fc",
          "name": "user.user_id.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Changes properties of an user - for example, changing or adding an email address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "293c8d1e-f22d-4156-8f09-e0836e87eed3"
            }
          ]
        },
        {
          "id": "245dc200-e575-4dc0-a9f5-3761b18da6a4",
          "name": "user.user_id.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6acf80d2-a1df-4f2d-b4bb-aa56f8e183be"
            }
          ]
        },
        {
          "id": "3eae141d-34a0-47d2-a258-99aeb24ce21d",
          "name": "user.user_id.creds.reset.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/creds/reset"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Changes the password of an user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f23cb62-6a14-41eb-b13a-12545974b16e"
            }
          ]
        },
        {
          "id": "5ae6fc26-0f2a-4c05-bf61-f55a0456b416",
          "name": "user.user_id.messages.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages"
              ],
              "query": [
                {
                  "key": "full_list",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "since",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of messages and some metadata about them. It will also include some metadata about the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c80ef76-8055-4031-83fb-4bdbd2042741"
            }
          ]
        },
        {
          "id": "c17b2e1a-8ae5-4895-821b-0978d838c043",
          "name": "user.user_id.messages.unread.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/unread"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of unread message IDs and their URLs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7dba649-6c77-489a-8e52-bdf6257c74ee"
            }
          ]
        },
        {
          "id": "dba230ec-5291-445a-9f33-23888538e29b",
          "name": "user.user_id.messages.unread.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/unread"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Marks multiple messages as read at once. If a message has already been marked as read, it will be silently skipped."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b133abb-1595-49a2-b92a-d31f0e33d274"
            }
          ]
        },
        {
          "id": "7cc4f906-e078-44b1-ac35-580b83219a2e",
          "name": "user.user_id.messages.message.message_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/message/:message_id"
              ],
              "variable": [
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bca0906-c283-4217-8065-51baa87137c0"
            }
          ]
        },
        {
          "id": "3b6c0675-e6cc-4ad5-b847-79ac27b93478",
          "name": "user.user_id.messages.message.message_id.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/message/:message_id"
              ],
              "variable": [
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2bcf16e-8c66-40bb-a3fb-38070004b881"
            }
          ]
        },
        {
          "id": "10ee0435-15b1-4f10-89f2-511faf950e5f",
          "name": "user.user_id.messages.message.message_id.body.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/message/:message_id/body"
              ],
              "variable": [
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a message's body."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c783cf4-d9a4-43ac-91d6-7bd0a85fbd8b"
            }
          ]
        },
        {
          "id": "dec374df-69e2-43fc-baaf-7afe8bfc40ff",
          "name": "user.user_id.messages.message.message_id.read.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/message/:message_id/read"
              ],
              "variable": [
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Marks a message as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1c6a37b-8a10-4c3d-b6db-a6ca748109ee"
            }
          ]
        },
        {
          "id": "1bac9279-3d7a-4392-94a1-9f673aec1b9a",
          "name": "user.user_id.messages.delete.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/delete"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes multiple messages at once. If a message has already been deleted, it will be silently skipped."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "717a0fe4-202d-47dc-83c5-91979e530baa"
            }
          ]
        },
        {
          "id": "36c0e6ee-5818-4a3d-a72b-33f601d98bdb",
          "name": "user.recover.post",
          "request": {
            "url": "http://go.urbanairship.com/api/user/recover",
            "method": "POST",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Uses the user???s email address as a way to restore subscription content across devices."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31e23251-394f-475b-8a6d-35653ec76675"
            }
          ]
        },
        {
          "id": "63a037f1-b944-4b12-8be3-74f92e3e3c59",
          "name": "user.recover.id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/recover/:id"
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
            "description": "Checks the recovery status."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6aecc31d-11d7-4bb3-a366-27d1895fb650"
            }
          ]
        },
        {
          "id": "2b0711eb-bfe9-4614-a600-c93ba0d5536f",
          "name": "user.user_id.available_subscriptions.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/available_subscriptions"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves subscription options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb6473cb-7453-44db-8c83-96382e4c7cb1"
            }
          ]
        },
        {
          "id": "44d0096e-85ed-4982-9e16-7869214de20e",
          "name": "user.user_id.subscriptions.subscription_key.purchase.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/subscriptions/:subscription_key/purchase"
              ],
              "variable": [
                {
                  "id": "subscription_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8dd2fb09-f045-4864-92da-349e5025d76a"
            }
          ]
        },
        {
          "id": "670eed7d-300d-49a8-825a-f18da4e2a896",
          "name": "user.user_id.subscription_content.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/subscription_content"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of available content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bef14a07-af8f-43a1-8b9a-33a808055019"
            }
          ]
        },
        {
          "id": "639ea248-64c3-4a16-9879-623cdb90faef",
          "name": "user.user_id.subscriptions.content.content_id.download.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/subscriptions/content/:content_id/download"
              ],
              "variable": [
                {
                  "id": "content_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Downloads the content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5a148b4-13f5-4850-9a85-18b32fe84ca3"
            }
          ]
        }
      ]
    },
    {
      "name": "Airmail",
      "item": [
        {
          "id": "55caedda-935b-443e-afc2-d2da6c997496",
          "name": "airmail.send.post",
          "request": {
            "url": "http://go.urbanairship.com/api/airmail/send",
            "method": "POST",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Sends a message. All fields except message are optional, but at least one of tags, users or aliases must be specified. Much like the push API, we have a batch API call that can make sending multiple messages easier. It???s located at /api/airmail/send/batch/ and accepts a list of messages in the same format as the standard push call."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d333b27-ee14-4c86-aaf9-5961c45b1153"
            }
          ]
        },
        {
          "id": "611a17b5-fdfc-481b-9856-f62a37ba0b40",
          "name": "airmail.send.broadcast.post",
          "request": {
            "url": "http://go.urbanairship.com/api/airmail/send/broadcast?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sends a message to all users (broadcast). Only message is required. The message will be sent out to every registered user. Badge numbers will be handled automatically as long as the push key is present."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28afdd46-0d5c-4673-a2d2-667e8ed12b9f"
            }
          ]
        }
      ]
    },
    {
      "name": "App",
      "item": [
        {
          "id": "b4b84c73-cd0c-4728-9567-d3b45c69837f",
          "name": "app.content.get",
          "request": {
            "url": "http://go.urbanairship.com/api/app/content?Content-Type=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the store inventory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "347e8ec4-5d47-4c3b-8d48-582e81c05d0b"
            }
          ]
        },
        {
          "id": "24192e51-883f-4e8c-a582-412bfd8a78bb",
          "name": "app.content.product_id.download.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "app/content/:product_id/download"
              ],
              "variable": [
                {
                  "id": "product_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a temporary URL where the client can download the content. In the payload, the receipt string is the receipt data from the purchase. It should be unaltered from how Apple delivers it to your application.udid is an optional field to help identify a particular user???s purchases, which can aid debugging. It should always be a hash of the UDID, not the actual UDID, to ensure compliance with Apple???s TOS. The optional version field should be the StoreFront library version, or custom if you???re building your own."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7769332-3963-441b-977a-88eefb9669bd"
            }
          ]
        },
        {
          "id": "75c8d8cd-4860-4d24-9558-3aef6aa4446f",
          "name": "app.updates.post",
          "request": {
            "url": "http://go.urbanairship.com/api/app/updates?product_id=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Checks for updates. It can be useful on application launch to compare a list of installed updates with our server to see if there are any updates to be had for the content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "503cc327-3db3-4f31-a86e-087eb2cdfd7b"
            }
          ]
        }
      ]
    },
    {
      "name": "Feeds",
      "item": [
        {
          "id": "d3ace5bd-7825-4397-b302-caa3d1394b15",
          "name": "feeds.get",
          "request": {
            "url": "http://go.urbanairship.com/api/feeds?Content-Type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of feeds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc172f83-9603-405c-916c-b533084698b9"
            }
          ]
        },
        {
          "id": "a43c2fa9-5663-44aa-9c8d-657cfda1dc92",
          "name": "feeds.post",
          "request": {
            "url": "http://go.urbanairship.com/api/feeds",
            "method": "POST",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new feed item."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7c5409f-e0c1-4cca-9e7d-f4b4ca3d10c3"
            }
          ]
        },
        {
          "id": "9ca27571-610c-494c-956f-53a0c373dd97",
          "name": "feeds.feed_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "feeds/:feed_id"
              ],
              "variable": [
                {
                  "id": "feed_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a particular feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "464ee2ed-48b5-41b5-8533-5dd3f6d82321"
            }
          ]
        },
        {
          "id": "58bb2e59-6a80-496b-a79a-2cdf58168805",
          "name": "feeds.feed_id.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "feeds/:feed_id"
              ],
              "variable": [
                {
                  "id": "feed_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Updates a feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1f07694-22cb-4ea1-82a3-46e758f2838f"
            }
          ]
        },
        {
          "id": "def3a533-a99e-4bab-b95f-abe33c6d7656",
          "name": "feeds.feed_id.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "feeds/:feed_id"
              ],
              "variable": [
                {
                  "id": "feed_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6d6a646-1fee-4dac-ba1b-f8457a216849"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "836920c5-93fb-4f77-9c6a-6e388bd72c68",
          "name": "tags.get",
          "request": {
            "url": "http://go.urbanairship.com/api/tags?feed_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all the tags that you have created."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43497d16-4f89-492e-a722-1f0725e4d5a8"
            }
          ]
        },
        {
          "id": "68e88c2d-1716-4e80-a68d-c38455bf88d7",
          "name": "tags.tag.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "tags/:tag"
              ],
              "variable": [
                {
                  "id": "tag",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14305afa-bbea-4e6b-aa22-87c13d1aaf12"
            }
          ]
        },
        {
          "id": "95cd7a0f-f3ad-44a8-8183-441cc301a457",
          "name": "tags.tag.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "tags/:tag"
              ],
              "variable": [
                {
                  "id": "tag",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Modifies device tokens on a tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14068a43-fc1e-4c86-bbd9-3d40eb58c51a"
            }
          ]
        }
      ]
    },
    {
      "name": "Partner",
      "item": [
        {
          "id": "6ad3d8a6-1d5a-4c8e-b02c-198f2dd89213",
          "name": "partner.apps.get",
          "request": {
            "url": "http://go.urbanairship.com/api/partner/apps?device_token=%7B%7D&tag=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List applications."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5e5b4ce-ca57-417a-81be-2e723c46ce44"
            }
          ]
        },
        {
          "id": "11437a25-55f9-44ea-919b-485f51c9978f",
          "name": "partner.apps.post",
          "request": {
            "url": "http://go.urbanairship.com/api/partner/apps",
            "method": "POST",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f2e5f7e-0f44-4485-a1ab-967288142b92"
            }
          ]
        },
        {
          "id": "f1a646be-36f8-4706-8dbf-5dad4c998163",
          "name": "partner.apps.app_id.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "partner/apps/:app_id"
              ],
              "variable": [
                {
                  "id": "app_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Updates an application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9464bfea-c0db-42ef-b695-0640ac8ca13a"
            }
          ]
        }
      ]
    }
  ]
}