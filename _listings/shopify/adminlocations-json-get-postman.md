{
  "info": {
    "name": "Shopify Get a list of all locations for a shop",
    "_postman_id": "3ef65632-e6fd-4f5c-9255-c974623308e7",
    "description": "Get a list of all locations for a shop.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "84d5dcf5-925d-4f87-9828-77c0c2dda269",
          "name": "getAdminLocations8790723.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/locations/8790723.json",
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
            "description": "Get a single location."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5395737-ba95-4eea-bf28-4ef336379dac"
            }
          ]
        },
        {
          "id": "51f90d21-80ee-48dc-b6c0-a977ede9e5e9",
          "name": "getAdminLocations.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/locations.json",
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
            "description": "Get a list of all locations for a shop."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1b57853-bc0a-4db0-ba9a-2709de727cf0"
            }
          ]
        }
      ]
    }
  ]
}