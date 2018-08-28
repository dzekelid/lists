{
  "info": {
    "name": "Plentymarkets Lists suppliers for a variation",
    "_postman_id": "2b8e13c4-66a9-48e0-9f96-7aa57b2353ee",
    "description": "Lists all supplier data linked to a variation. The ID of the variation must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Lists",
      "item": [
        {
          "id": "ba6e8ebf-53ba-48e5-85b5-d3b5eabf059f",
          "name": "getRestItemsVariationsVariationVariationSuppliers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_suppliers"
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
            "description": "Lists all supplier data linked to a variation. The ID of the variation must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a39a2ff0-401c-409a-86b6-ba99671e9ccf"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "598e2f34-9636-4ed0-90cb-76ed2692ea84",
          "name": "postRestItemsVariationsVariationVariationSuppliers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_suppliers"
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
            "method": "POST",
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
            "description": "Creates a link between a variation and a supplier and adds supplier data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "808a6c7d-62d4-4b96-844a-dfd11fdd81bc"
            }
          ]
        },
        {
          "id": "ff83f91d-a4a2-4ff9-81bf-e4a0fff5ba25",
          "name": "deleteRestItemsVariationsVariationVariationSuppliersVariationsupplier",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_suppliers/:variationSupplierId"
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
                },
                {
                  "id": "variationSupplierId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Deletes a link between a variation and a supplier. The ID of the variation and the ID of the link between the variation and the supplier must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d64a0fb-3e53-4cb6-8073-7e94cbd0be56"
            }
          ]
        }
      ]
    },
    {
      "name": "Supplier",
      "item": [
        {
          "id": "c47c5e9a-c6a4-40ec-8c46-4815bd60592d",
          "name": "getRestItemsVariationsVariationVariationSuppliersVariationsupplier",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_suppliers/:variationSupplierId"
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
                },
                {
                  "id": "variationSupplierId",
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
            "description": "Gets the data for a supplier linked to a variation. The ID of the variation and the ID of the link between the variation and the supplier must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab566fe5-5e2f-4312-8fb8-b115d24751bb"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "3b894f3a-3fa6-4aae-a914-e2607b65b857",
          "name": "putRestItemsVariationsVariationVariationSuppliersVariationsupplier",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_suppliers/:variationSupplierId"
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
                },
                {
                  "id": "variationSupplierId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
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
            "description": "Updates the data of a supplier linked to a variation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "410715ee-b272-450d-9348-6686c23de947"
            }
          ]
        }
      ]
    }
  ]
}