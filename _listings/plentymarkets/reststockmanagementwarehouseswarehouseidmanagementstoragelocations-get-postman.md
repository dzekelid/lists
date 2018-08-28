{
  "info": {
    "name": "Plentymarkets List storage locations",
    "_postman_id": "ed8f7070-34e7-44df-879a-bab9f464d004",
    "description": "Lists storage locations that belong to a warehouse. The id of the warehouse must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "fdbdb2b7-0dd9-4714-be05-a352c17c00c3",
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
              "id": "14a91661-f444-4df0-ae75-f2278a8feed6"
            }
          ]
        },
        {
          "id": "8dd31691-4e5a-4ebf-a7e5-a968de18825b",
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
              "id": "7a2e142c-5e0e-4035-928f-2190afd0f357"
            }
          ]
        },
        {
          "id": "a8dc015e-6c06-4ac1-a177-df87394e42a1",
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
              "id": "ac5fd7b4-1fbd-43a3-b75b-570ddf323573"
            }
          ]
        },
        {
          "id": "80e9ba04-b8c5-4609-b73d-c536a96b2637",
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
              "id": "67d7ea21-f798-4817-854d-f837a0205bde"
            }
          ]
        },
        {
          "id": "82230c5f-2c08-415d-a338-5d8cdbcd217f",
          "name": "getRestStockmanagementWarehousesWarehouseManagementStoragelocations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/stockmanagement/warehouses/:warehouseId/management/storageLocations"
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
            "description": "Lists storage locations that belong to a warehouse. The id of the warehouse must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6262d621-e922-47fe-b6fe-e7a3cb56e32a"
            }
          ]
        }
      ]
    }
  ]
}