{
  "info": {
    "name": "Shopify List all abandoned checkouts",
    "_postman_id": "4f6f7ae0-f6b9-4598-8409-48d680fb06b0",
    "description": "List all abandoned checkouts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "e4a09369-5a8a-43d8-84fb-5820ae2ac149",
          "name": "getAdminCheckouts.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/checkouts.json",
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
            "description": "List all abandoned checkouts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9c607ec-4cea-408f-aaa3-6dd9637d3ee8"
            }
          ]
        }
      ]
    }
  ]
}