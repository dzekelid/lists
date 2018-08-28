{
  "info": {
    "name": "Plentymarkets List clients (stores)",
    "_postman_id": "9a34a848-f230-4081-a7be-3edb1eb9db32",
    "description": "List clients (stores).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "9c01a6c2-e42c-4cd6-bbff-945eecec146b",
          "name": "getRestItemsSalesPricesOnlineStores",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/online_stores"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists all activated clients (stores) for a sales price. The ID of the sales price must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "757575b5-716e-4582-8733-85a537e8f689"
            }
          ]
        },
        {
          "id": "141ce4c1-b69f-470c-a8d4-5ca483367032",
          "name": "getRestItemsVariationsVariationVariationClients",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_clients"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists all clients (stores) linked to a variation. The ID of the variation must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef8aea90-0f8f-4840-933d-a89b2a5aba4a"
            }
          ]
        },
        {
          "id": "7b373e88-f9e8-4c5e-b095-26b8efe3420d",
          "name": "getRestWebstores",
          "request": {
            "url": "http://example.com/rest/webstores",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List clients (stores)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58ffde15-d0d3-4c2c-8558-6f67505a4a70"
            }
          ]
        }
      ]
    }
  ]
}