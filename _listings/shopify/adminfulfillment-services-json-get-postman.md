{
  "info": {
    "name": "Shopify List your app's fulfillment services",
    "_postman_id": "b3c37ad3-6ed3-49a6-826c-54f1ab666caa",
    "description": "List your app's fulfillment services.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "bf390209-8322-4d0e-a308-1996bdab92d2",
          "name": "getAdminFulfillmentServices.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/fulfillment_services.json",
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
            "description": "List your app's fulfillment services."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c51ff91e-93be-4224-9196-288ab702e64a"
            }
          ]
        }
      ]
    }
  ]
}