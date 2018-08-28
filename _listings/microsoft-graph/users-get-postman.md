{
  "info": {
    "name": "Microsoft Graph API List Users",
    "_postman_id": "8036deec-eae1-4033-ad22-f9de427be7d1",
    "description": "List users Retrieve a list of user objects.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "83f8f198-f8c1-4296-9d72-5730bf466e1f",
          "name": "ListUsers",
          "request": {
            "url": "http://graph.microsoft.com/users",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "application/json",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List users Retrieve a list of user objects"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "fd7656db-b6bc-4e79-819e-b70a45657190"
            }
          ]
        }
      ]
    }
  ]
}