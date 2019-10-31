{
  "info": {
    "name": "Xibo API Add a Web page Widget",
    "_postman_id": "21fe2beb-38de-4a23-8769-cde5deb01636",
    "description": "Add a new Web page Widget to the specified playlist",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Web",
      "item": [
        {
          "id": "5abda59b-8a3b-40f7-9fcb-fba14eb3ecc6",
          "name": "WidgetWebpageAdd",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "playlist/widget/webpage/:playlistId"
              ],
              "variable": [
                {
                  "id": "playlistId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "duration",
                  "value": "{}",
                  "disabled": false,
                  "description": "The Web page Duration"
                },
                {
                  "key": "modeId",
                  "value": "{}",
                  "disabled": false,
                  "description": "The mode option for Web page, 1- Open Natively, 2- Manual Position, 3- Best Ft"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Optional Widget Name"
                },
                {
                  "key": "offsetLeft",
                  "value": "{}",
                  "disabled": false,
                  "description": "For Manual position, the starting point from the left in pixels"
                },
                {
                  "key": "offsetTop",
                  "value": "{}",
                  "disabled": false,
                  "description": "For Manual position, the starting point from the Top in pixels"
                },
                {
                  "key": "pageHeight",
                  "value": "{}",
                  "disabled": false,
                  "description": "For Manual Position and Best Fit, The height of the page - if empty it will use region height"
                },
                {
                  "key": "pageWidth",
                  "value": "{}",
                  "disabled": false,
                  "description": "For Manual Position and Best Fit, The width of the page - if empty it will use region width"
                },
                {
                  "key": "scaling",
                  "value": "{}",
                  "disabled": false,
                  "description": "For Manual position the percentage to scale the Web page (0-100)"
                },
                {
                  "key": "transparency",
                  "value": "{}",
                  "disabled": false,
                  "description": "flag (0,1) should the HTML be shown with a transparent background?"
                },
                {
                  "key": "uri",
                  "value": "{}",
                  "disabled": false,
                  "description": "string containing the location (URL) of the web page"
                },
                {
                  "key": "useDuration",
                  "value": "{}",
                  "disabled": false,
                  "description": "(0, 1) Select 1 only if you will provide duration parameter as well"
                }
              ]
            },
            "description": "Add a new Web page Widget to the specified playlist"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec52cb30-3435-4fce-bbb0-9c59e7fab2c9"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/api"
    }
  ]
}