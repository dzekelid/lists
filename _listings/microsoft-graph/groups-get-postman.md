{
  "info": {
    "name": "Microsoft Graph API List Groups",
    "_postman_id": "ee00a60d-6e14-4f89-9ae6-75afd996cabf",
    "description": "List groups List all the groups available in an organization, including but not limited to Office 365 Groups. The default properties of each group are returned.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "915c9074-e84a-414f-9df3-abd6e3704a0e",
          "name": "ListGroups",
          "request": {
            "url": "http://graph.microsoft.com/groups",
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
            "description": "List groups List all the groups available in an organization, including but not limited to Office 365 Groups"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "2d3a3c3f-a319-4a06-8108-ed50c52769b2"
            }
          ]
        }
      ]
    }
  ]
}