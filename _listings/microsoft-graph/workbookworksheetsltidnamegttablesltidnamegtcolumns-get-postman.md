{
  "info": {
    "name": "Microsoft Graph API List Columns",
    "_postman_id": "456a16c7-a90a-4ee5-8136-3f61bdaf5d1c",
    "description": "List columns Retrieve a list of tablecolumn objects.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "565f2416-4e47-4ca4-94eb-c9d4ce7993a3",
          "name": "ListColumns",
          "request": {
            "url": "http://graph.microsoft.com/workbook/worksheets(&lt;id|name&gt;)/tables(&lt;id|name&gt;)/columns",
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
              "id": "27f0d16a-6c04-4b3d-a8e8-83f40e9ced9d"
            }
          ]
        }
      ]
    }
  ]
}