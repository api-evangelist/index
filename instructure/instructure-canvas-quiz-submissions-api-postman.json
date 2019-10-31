{
  "info": {
    "name": "Instructure Canvas Quiz Submissions API Unflagging a question.",
    "_postman_id": "a9b4182b-8f6e-4c6b-8c62-bc8817a235fa",
    "description": "Unflagging a question..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Quiz",
      "item": [
        {
          "id": "a15dcd76-d389-4288-8736-cb19cca79b7d",
          "name": "get-all-quiz-submission-questions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "quiz_submissions/:quiz_submission_id/questions"
              ],
              "query": [
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "quiz_submission_id",
                  "value": "quiz_submission_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all quiz submission questions.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0c22a68-87aa-4d72-8667-08bce1d0d106"
            }
          ]
        },
        {
          "id": "3fee9150-aa35-479d-b356-b75713d20700",
          "name": "answering-questions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "quiz_submissions/:quiz_submission_id/questions"
              ],
              "query": [
                {
                  "key": "access_code",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "attempt",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "quiz_questions",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "validation_token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "quiz_submission_id",
                  "value": "quiz_submission_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Answering questions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85e41e66-e4ac-4876-bd00-3a49a6b0904f"
            }
          ]
        },
        {
          "id": "6c132391-56ce-4c85-a507-311f56f5b100",
          "name": "flagging-a-question",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "quiz_submissions/:quiz_submission_id/questions/id/flag"
              ],
              "query": [
                {
                  "key": "access_code",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "attempt",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "validation_token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "quiz_submission_id",
                  "value": "quiz_submission_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Flagging a question.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d81bbc7-8112-4a5c-8ada-b3e5af030bce"
            }
          ]
        },
        {
          "id": "31d9c196-04a1-4ca5-96a7-8d80168de2cc",
          "name": "unflagging-a-question",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "quiz_submissions/:quiz_submission_id/questions/id/unflag"
              ],
              "query": [
                {
                  "key": "access_code",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "attempt",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "validation_token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "quiz_submission_id",
                  "value": "quiz_submission_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Unflagging a question.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "185dd510-0616-4791-a238-389b0946d468"
            }
          ]
        }
      ]
    }
  ]
}