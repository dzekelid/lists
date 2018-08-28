{
  "info": {
    "name": "Plentymarkets List names of property types",
    "_postman_id": "e540d48e-673f-44e3-a8f6-ab69e30a1456",
    "description": "List names of property types.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "14743658-0725-477d-a30e-47b4d17c3fb0",
          "name": "getRestItemsAttributesAttributeNamesLang",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/attributes/:attributeId/names/:lang"
              ],
              "variable": [
                {
                  "id": "attributeId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lang",
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
            "description": "Lists the attribute names of an attribute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab3b578d-8a04-43e1-9996-c8ccb5258c2a"
            }
          ]
        },
        {
          "id": "87575c17-f6dd-4601-8744-b605f9e02729",
          "name": "getRestItemsPropertiesNames",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/properties/:id/names"
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
            "description": "Lists the names of a property in all languages. The ID of the property must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e0cb701-f10f-426b-9149-849772097e7a"
            }
          ]
        },
        {
          "id": "830f2bab-02a3-4b10-b4e3-4b5250dd088a",
          "name": "getRestItemsPropertyGroupsNames",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/property_groups/:id/names"
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
            "description": "Lists the property group names of a property group in all languages. The ID of the property group must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab900c6a-a2c0-48c9-ad61-8eedaab8bcac"
            }
          ]
        },
        {
          "id": "4b2612f9-7354-4e8e-b224-a9f77ec389d8",
          "name": "getRestItemsSalesPricesNames",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/sales_prices/:id/names"
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
            "description": "Lists the names of a sales price in all languages. The ID of the sales price must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a70c10ea-017f-41c3-8fd6-044ab2a16341"
            }
          ]
        },
        {
          "id": "f3a8c112-83c1-495b-a22f-bdc6a78a84e1",
          "name": "getRestItemsUnitsNames",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/units/:id/names"
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
            "description": "Lists the unit names of a unit. The ID of the unit must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f984e1d-494b-4ad0-b147-5327dd1ba7e8"
            }
          ]
        },
        {
          "id": "7e6ef1b5-086c-4fa0-90b4-7732c51efe30",
          "name": "getRestItemsImagesImageNames",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/images/:imageId/names"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "imageId",
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
            "description": "Lists all names of an image. The image ID must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1bc8d45-5438-4105-9d4f-8d1f39095ab0"
            }
          ]
        },
        {
          "id": "894c0d29-1b36-475f-9159-0159c52771d3",
          "name": "getRestOrdersDatesTypesTypeNames",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/dates/types/:typeId/names"
              ],
              "variable": [
                {
                  "id": "typeId",
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
            "description": "Lists names in all languages available of an order date type. The ID of the date type must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de305feb-1e8a-4688-a28b-8d9c23fff0e4"
            }
          ]
        },
        {
          "id": "a576dcd7-8531-40d1-bad4-29f7ef0c326e",
          "name": "getRestPaymentPropertiesTypesNamesLang",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/payment/properties/types/names/:lang?"
              ],
              "query": [
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
                  "id": "lang?",
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
            "description": "List names of property types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57857cc9-b4be-4844-ba38-bb322f2c0e46"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "46734210-d02a-4a6e-aed3-e5bedf8555c9",
          "name": "getRestItemsAttributesAttributeValueMarketNames",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/attributes/:attributeId/value_market_names"
              ],
              "query": [
                {
                  "key": "itemsPerPage",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lang",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "referenceType",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "attributeId",
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
            "description": "Search attribute value market names."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d464d879-9d12-43bd-8f19-d845435be6b3"
            }
          ]
        }
      ]
    }
  ]
}