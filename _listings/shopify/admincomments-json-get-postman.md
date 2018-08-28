{
  "info": {
    "name": "Shopify Get a list of all comments",
    "_postman_id": "7aa14dba-5205-43e2-8d22-08366128aa4e",
    "description": "Get a list of all comments.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "0ef2299a-fe11-4aaf-8498-5bb3045f0a62",
          "name": "getAdminComments.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/comments.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of all comments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1326292a-f651-42c3-b86c-9843fffdec19"
            }
          ]
        }
      ]
    }
  ]
}