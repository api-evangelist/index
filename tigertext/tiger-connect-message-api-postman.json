{
  "info": {
    "name": "Tiger Connect Message API Forward the message to the following User or Group.",
    "_postman_id": "c3aaeeec-2dd1-4d81-a373-a79f1b6dda2f",
    "description": "Forward the message to the following User or Group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Message",
      "item": [
        {
          "id": "220bcd6a-a836-4a71-9459-0a4272b33d95",
          "name": "forwardMessage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "developer.tigertext.me",
              "path": [
                "v2",
                "message/:message_token/forward/"
              ],
              "variable": [
                {
                  "id": "message_token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "recipient_organization",
                  "value": "{}",
                  "disabled": false,
                  "description": "The recipient organization token"
                },
                {
                  "key": "recipient_token",
                  "value": "{}",
                  "disabled": false,
                  "description": "The recipient User or Group token based on address encoding"
                },
                {
                  "key": "sender_organization",
                  "value": "{}",
                  "disabled": false,
                  "description": "The sender User organization token"
                }
              ]
            },
            "description": "Forward the message to the following User or Group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ed3085d-25ba-4087-af79-914055a4e7dc"
            }
          ]
        }
      ]
    }
  ]
}