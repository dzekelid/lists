{
  "info": {
    "name": "Microsoft Graph API List Owned Devices",
    "_postman_id": "5ddd9f4a-f878-4225-aca9-c053d85ed819",
    "description": "List ownedDevices Get the list of devices that are owned by the user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "ea26a548-b232-437b-b775-7b16ca4d9796",
          "name": "ListOwnedDevices",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/ownedDevices"
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
                "key": "Accept",
                "value": "{}",
                "description": "application/json",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List ownedDevices Get the list of devices that are owned by the user"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "aeff0888-5d4d-4fda-95a5-77a28ddab0ec"
            }
          ]
        }
      ]
    }
  ]
}