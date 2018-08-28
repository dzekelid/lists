{
  "info": {
    "name": "Microsoft Graph API List Worksheets",
    "_postman_id": "176d5dab-1399-4fb8-a59e-a73db949fe91",
    "description": "List worksheets Retrieve a list of worksheet objects.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "6f91cbdd-383f-4f11-b002-973152e99bf2",
          "name": "ListWorksheets",
          "request": {
            "url": "http://graph.microsoft.com/workbook/worksheets",
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
            "description": "List worksheets Retrieve a list of worksheet objects"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "5cc4cb6e-0814-4247-8b3b-3ac56cddd217"
            }
          ]
        }
      ]
    }
  ]
}