{
  "info": {
    "name": "Plentymarkets List warehouse locations",
    "_postman_id": "2f464f1a-d1e7-4220-9d1b-f6b5387eb134",
    "description": "Lists all warehouse locations.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "9dcb28f0-18ae-41f5-af96-5296e62189dd",
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
              "id": "43063247-ba14-48b9-829f-ebf353e8790d"
            }
          ]
        },
        {
          "id": "e805cbe6-076a-4673-a307-c332ea4dd58d",
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
              "id": "14e63149-de06-42e4-a7e0-248eba4bc34b"
            }
          ]
        },
        {
          "id": "eed5d83e-c35d-42f2-a6b3-945d7812acea",
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
              "id": "783dfc74-23ff-46f2-84e3-d95962a0c925"
            }
          ]
        },
        {
          "id": "8ca854f4-b24f-4170-8f37-d8b4733d8b48",
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
              "id": "c2a79c0e-61d1-4fbc-8807-ea3459a0f3e9"
            }
          ]
        },
        {
          "id": "5ff8a8a9-fdf2-4d9c-9807-ae5320e63d79",
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
              "id": "5a592cde-353c-4cf0-9732-d88dca71ccde"
            }
          ]
        },
        {
          "id": "6425ae6b-05f7-49f6-8d85-868ff990dbbe",
          "name": "getRestWarehousesWarehouseLocations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/warehouses/:warehouseId/locations"
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
            "description": "Lists all warehouse locations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dcaf8ffd-8142-44d6-93ce-944f9f3d740c"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "783fc199-f767-4398-83bb-2d55703aee77",
          "name": "deleteRestWarehousesLocations",
          "request": {
            "url": "http://example.com/rest/warehouses/locations",
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
            "description": "Deletes multiple warehouse locations"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd2a0cc6-7eeb-42e5-8ecb-ee67f813757b"
            }
          ]
        }
      ]
    },
    {
      "name": "Edit",
      "item": [
        {
          "id": "322377fd-d59e-419c-831f-cc9cc2e80b5c",
          "name": "putRestWarehousesLocationsGroup",
          "request": {
            "url": "http://example.com/rest/warehouses/locations/group",
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
            "description": "Edits the purpose and status for a group of storage locations by passing the group storage location ID (can be sent as mass assignment)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ebc763b7-6afb-4f02-89a0-4dc054a72c0b"
            }
          ]
        }
      ]
    }
  ]
}