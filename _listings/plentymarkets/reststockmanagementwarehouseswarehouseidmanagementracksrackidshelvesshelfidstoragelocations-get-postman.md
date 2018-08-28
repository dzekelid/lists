{
  "info": {
    "name": "Plentymarkets List storage locations",
    "_postman_id": "e013eaa4-6405-499b-87a9-ecc6c783e57f",
    "description": "Lists storage locations. The id of the warehouse, the id of the rack and the id of the shelf must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "f56e0f46-2ccb-44fb-9940-bfa3337ce601",
          "name": "getRestAccountingStoresLocations",
          "request": {
            "url": "http://example.com/rest/accounting/stores/locations",
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
            "description": "List all accounting locations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e60bcaf5-8a4a-4115-a1af-134b24e114f5"
            }
          ]
        },
        {
          "id": "8fa0a156-aa02-4cfb-bf59-a769b92338df",
          "name": "getRestAccountingStoresPlentyLocations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/stores/:plentyId/locations"
              ],
              "query": [
                {
                  "key": "locationId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "plentyId",
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
            "description": "Lists accounting locations of a client. The plenty ID of the client must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fd512a8e-4b20-4805-b67d-ded916202e85"
            }
          ]
        },
        {
          "id": "90b86e0f-c604-474d-9130-3b00f3837c96",
          "name": "getRestItemsVariationsVariationStockStoragelocations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/stock/storageLocations"
              ],
              "query": [
                {
                  "key": "columns",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "itemsPerPage",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Lists stock of a variation per storage location. The ID of the item and the ID of the variation must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dfba9c80-468f-40f2-81ed-65c86615a1e4"
            }
          ]
        },
        {
          "id": "eea3c473-8b8a-46f5-94ab-d81c2dd0d023",
          "name": "getRestStockmanagementWarehousesWarehouseManagementRacksRackShelvesShelfStoragelocations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/stockmanagement/warehouses/:warehouseId/management/racks/:rackId/shelves/:shelfId/storageLocations"
              ],
              "query": [
                {
                  "key": "columns",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "itemsPerPage",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "with",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "rackId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "shelfId",
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
            "description": "Lists storage locations. The id of the warehouse, the id of the rack and the id of the shelf must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6313689-e64c-4023-8355-65c9b42f5496"
            }
          ]
        }
      ]
    }
  ]
}