{
  "info": {
    "name": "Microsoft Graph API List Attachments",
    "_postman_id": "fd015f24-be12-42d6-9be3-f01261fbfab1",
    "description": "List attachments Retrieve a list of attachment objects attached to a message.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "a332a6dd-e726-44c4-b672-269b2786fb06",
          "name": "ListAttachments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/mailFolders/:id/childFolders/:id/messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
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
              "id": "85ce11d0-7d5e-4537-bf78-765273c27faa"
            }
          ]
        }
      ]
    }
  ]
}