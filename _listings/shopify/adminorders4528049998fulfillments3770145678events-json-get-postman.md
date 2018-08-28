{
  "info": {
    "name": "Shopify Get a list of all fulfillment events for a fulfillment",
    "_postman_id": "6caf8372-435a-4db4-8292-28d635422b95",
    "description": "Get a list of all fulfillment events for a fulfillment.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "d8c6cf16-c3eb-440d-800e-f55de22b4acd",
          "name": "getAdminOrders4554953422Events.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/orders/4554953422/events.json",
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
            "description": "Get all the events from a particular order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0cedfbf-9f5f-4834-b9c9-5cc55d74d234"
            }
          ]
        },
        {
          "id": "17e244ea-10ed-464a-94f6-998273ad4399",
          "name": "getAdminProducts7990943555Events.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/products/7990943555/events.json",
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
            "description": "Get all the events from a particular product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb9ab569-4660-4035-a2b7-7f0aba2f85db"
            }
          ]
        },
        {
          "id": "7c800327-8132-4b2c-8086-844236feedb8",
          "name": "getAdminEventsCount.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/events/count.json",
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
            "description": "Count all the events."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b860998a-0653-40c4-a807-1983122cb57e"
            }
          ]
        },
        {
          "id": "a880487f-055d-4536-ba00-a1a322f47a2b",
          "name": "getAdminOrders4528049998Fulfillments3770145678Events.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/orders/4528049998/fulfillments/3770145678/events.json",
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
            "description": "Get a list of all fulfillment events for a fulfillment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56745d97-7ae7-4612-ba5a-540dfddfca4e"
            }
          ]
        }
      ]
    }
  ]
}