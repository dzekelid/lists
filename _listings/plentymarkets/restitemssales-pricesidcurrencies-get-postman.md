{
  "info": {
    "name": "Plentymarkets List activated currencies",
    "_postman_id": "ca39b9e9-d371-4331-8afb-3bcb0f460a6a",
    "description": "List all currencies activated for a sales price. The ID of the sales price must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "09cefee5-a2d4-4824-8dbd-d8491f6e6cfd",
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
              "id": "7015fe1d-4d1a-4ebf-817e-27c9055163cb"
            }
          ]
        }
      ]
    }
  ]
}