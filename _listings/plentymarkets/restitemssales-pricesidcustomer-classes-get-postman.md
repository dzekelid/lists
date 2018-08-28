{
  "info": {
    "name": "Plentymarkets List activated customer classes",
    "_postman_id": "4021572d-1358-4485-b6e3-9b6490892464",
    "description": "Lists the activated customer classes for a sales price. The ID of the sales price must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "2a7a239e-c502-4c34-8626-2e8146300088",
          "name": "getRestAccountsContactsClasses",
          "request": {
            "url": "http://example.com/rest/accounts/contacts/classes",
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
            "description": "List contact classes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9554165-7502-47de-9db8-6f34e7b6a90b"
            }
          ]
        },
        {
          "id": "f1aba94c-4658-48e5-8743-09dc3de2cc6d",
          "name": "getRestItemsSalesPricesCustomerClasses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/customer_classes"
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
            "description": "Lists the activated customer classes for a sales price. The ID of the sales price must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14dfb8c2-4d5e-4e85-8250-85793a7995c2"
            }
          ]
        }
      ]
    }
  ]
}