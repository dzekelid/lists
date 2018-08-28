{
  "info": {
    "name": "Plentymarkets List activated clients (stores)",
    "_postman_id": "df748943-cb9a-4543-ba4e-11085ceddf2e",
    "description": "Lists all activated clients (stores) for a sales price. The ID of the sales price must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "0a8921ca-ea68-416f-94d0-88125bbc2fbb",
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
              "id": "83ea9aa3-b9bb-41af-9e9c-b105ba251406"
            }
          ]
        }
      ]
    }
  ]
}