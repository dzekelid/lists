{
  "info": {
    "name": "Plentymarkets List currencies",
    "_postman_id": "cd7f9f3d-f2e7-4aa9-9733-79c11d766ec4",
    "description": "List currencies.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "5c0347bb-fab8-4575-b452-1e05a08650e9",
          "name": "getRestItemsSalesPricesCurrencies",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/currencies"
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
            "description": "List all currencies activated for a sales price. The ID of the sales price must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cacb10c1-e18a-4104-bcd2-8c40db22f349"
            }
          ]
        },
        {
          "id": "4e1544f6-a5b1-4423-a3e1-e62798b0029a",
          "name": "getRestOrdersCurrencies",
          "request": {
            "url": "http://example.com/rest/orders/currencies?columns=%7B%7D&with=%7B%7D",
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
            "description": "List currencies."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fbe57acb-bd10-4ccf-a80b-73c7b13d374c"
            }
          ]
        }
      ]
    }
  ]
}