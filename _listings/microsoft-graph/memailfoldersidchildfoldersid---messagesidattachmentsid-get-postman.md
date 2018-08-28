{
  "info": {
    "name": "Microsoft Graph API List Attachments",
    "_postman_id": "159051c0-8b99-4726-9ddc-f81bcfb1e862",
    "description": "List attachments Retrieve a list of attachment objects attached to a message.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "274b6cc9-e196-4dd1-93a3-a70ee05244ec",
          "name": "ListAttachments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/mailFolders/:id/childFolders/:id/.../messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List attachments Retrieve a list of attachment objects attached to a message"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "da504c2b-df62-4306-a9c1-1c988a487ce3"
            }
          ]
        }
      ]
    }
  ]
}