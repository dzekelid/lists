{
  "info": {
    "name": "Microsoft Graph API List Devices",
    "_postman_id": "7532869a-b45d-4288-91a3-ea25ba025714",
    "description": "List devices Retrieve a list of device objects registered in the organization.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "df6f7e53-4563-4c95-98b1-1b25970066d8",
          "name": "ListDevices",
          "request": {
            "url": "http://graph.microsoft.com/devices",
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
            "description": "List devices Retrieve a list of device objects registered in the organization"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "b86c85ce-2b09-4314-b54a-db7fe6e1159c"
            }
          ]
        }
      ]
    }
  ]
}