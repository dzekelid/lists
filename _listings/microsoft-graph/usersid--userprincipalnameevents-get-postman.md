{
  "info": {
    "name": "Microsoft Graph API List Events",
    "_postman_id": "77f60b0d-c892-4594-a89f-80e2974cc19b",
    "description": "List events Get a list of event objects in the user's mailbox. The list contains single instance meetings and series masters.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "f2c01e93-aa10-4d39-a8ac-b5fd9d11a7fe",
          "name": "ListEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/events"
              ],
              "variable": [
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
              },
              {
                "key": "Prefer: outlook.timezone",
                "value": "Prefer: outlook.timezone",
                "description": "The default time zone for events in the response",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List events Get a list of event objects in the user's mailbox"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "26c144e1-7aef-47f7-8a12-72f2b4a3a0aa"
            }
          ]
        }
      ]
    }
  ]
}