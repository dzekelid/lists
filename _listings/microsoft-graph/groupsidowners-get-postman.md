{
  "info": {
    "name": "Microsoft Graph API List Owners",
    "_postman_id": "88c3e430-edbf-4e8e-b0b2-2c7192d48531",
    "description": "List owners Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "3534cbe6-a4b6-470f-ad83-17d9c688b492",
          "name": "ListOwners",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/owners"
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
            "description": "List owners Retrieve a list of the group's owners"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "1d3841d1-3109-42f1-a4ab-20ae16c12df4"
            }
          ]
        }
      ]
    }
  ]
}