{
  "info": {
    "name": "GoToAssist Remote Support Mark Recordings as Archived",
    "_postman_id": "44b0cf80-f29d-4ccc-95dd-4eadaad5c68a",
    "description": "This method marks a list of recordings as archived by setting their archived flag to “true.” No more than 500 recordings can be marked as archived once.\n\nNote: Session recording must be enabled on the account in order to use this API method. To enable session recording, log in at https://app.gotoassist.com (link is external) and go to Configure > GoToAssist Settings > Enable Session Recording check box.\n\n  Request Parameters                    \n                      \n    field        data type      description    \n    recordingIds        array      A list of recordingIDs for the recordings to be archived    \n\n\nStatus Codes                \n                \n    Staus Code        description    \n    204 No Content        Recordings have been archived    \n    400 Bad Request        Request may be malformed or property may be missing or invalid    \n    403 Forbidden        Invalid authorization header or invalid recordingIDs    \n    500 Internal Server Error        Unexpected server error",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Mark",
      "item": [
        {
          "id": "7de2bffe-c341-4d6a-bbf8-5f983177f88b",
          "name": "ArchiveRecordingsArchivedByRecordingIDsPut",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.getgo.com",
              "path": [
                "G2A",
                "rest",
                "v1",
                "archive/recordings/archived/:recordingIDs"
              ],
              "variable": [
                {
                  "id": "recordingIDs",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This method marks a list of recordings as archived by setting their archived flag to “true.” No more than 500 recordings can be marked as archived once.\n\nNote: Session recording must be enabled on the account in order to use this API method. To enable session recording, log in at https://app.gotoassist.com (link is external) and go to Configure > GoToAssist Settings > Enable Session Recording check box.\n\n  Request Parameters                    \n                      \n    field        data type      description    \n    recordingIds        array      A list of recordingIDs for the recordings to be archived    \n\n\nStatus Codes                \n                \n    Staus Code        description    \n    204 No Content        Recordings have been archived    \n    400 Bad Request        Request may be malformed or property may be missing or invalid    \n    403 Forbidden        Invalid authorization header or invalid recordingIDs    \n    500 Internal Server Error        Unexpected server error"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f41f1129-9b3d-424f-bc70-02047b6afdaf"
            }
          ]
        }
      ]
    }
  ]
}