{
  "info": {
    "name": "Microsoft Graph API List Columns",
    "_postman_id": "e97bce50-bf1c-4fdc-aaf6-04d778ff19db",
    "description": "List columns Retrieve a list of tablecolumn objects.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "54aa8ea0-b2c0-4205-885b-c4bea341dc16",
          "name": "ListColumns",
          "request": {
            "url": "http://graph.microsoft.com/workbook/tables(&lt;id|name&gt;)/columns",
            "method": "GET",
            "header": [
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
            "description": "List columns Retrieve a list of tablecolumn objects"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "e6cb27b8-38b2-479d-910e-ba0b3d57b415"
            }
          ]
        }
      ]
    }
  ]
}