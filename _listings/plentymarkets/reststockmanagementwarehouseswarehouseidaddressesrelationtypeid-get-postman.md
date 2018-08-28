{
  "info": {
    "name": "Plentymarkets List warehouse addresses",
    "_postman_id": "fed1b796-6c5d-4434-bb2b-128b8ff219f0",
    "description": "List warehouse addresses. The ID of the warehouse must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "403fa1dc-ae6d-45e3-8134-22f94e4816c1",
          "name": "getRestAccountsContactsContactAddressesAddresstype",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/contacts/:contactId/addresses/:addressTypeId?"
              ],
              "variable": [
                {
                  "id": "addressTypeId?",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "contactId",
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
            "description": "Lists addresses of the contact. The ID of the contact must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96a34030-edd5-49b9-a8aa-fda60bcf4c13"
            }
          ]
        },
        {
          "id": "27febfd3-fe25-4ae5-9e45-0ef45a58e6a2",
          "name": "getRestOrdersOrderAddressesRelationtype",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/:orderId/addresses/:relationTypeId?"
              ],
              "variable": [
                {
                  "id": "orderId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "relationTypeId?",
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
            "description": "Lists order addresses. The ID of the order must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30e7face-88a7-4c54-84f4-23df425d6a70"
            }
          ]
        },
        {
          "id": "118642eb-0865-44d4-99c1-c5318140c52d",
          "name": "getRestStockmanagementWarehousesWarehouseAddressesRelationtype",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/stockmanagement/warehouses/:warehouseId/addresses/:relationTypeId?"
              ],
              "variable": [
                {
                  "id": "relationTypeId?",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "warehouseId",
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
            "description": "List warehouse addresses. The ID of the warehouse must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1dd3d29-4218-4a31-a88c-f3862153c74d"
            }
          ]
        }
      ]
    }
  ]
}