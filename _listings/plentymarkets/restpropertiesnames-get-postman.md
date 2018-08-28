{
  "info": {
    "name": "Plentymarkets List names",
    "_postman_id": "8f2ac369-26b2-45d1-81c9-a48b25618bbe",
    "description": "Lists names.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "b01fd942-43f6-4473-9c80-4b40852722bd",
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
              "id": "056cd2a6-8052-461b-a8f0-973a02ad3a01"
            }
          ]
        },
        {
          "id": "940d1fc1-c70c-4fb0-92ea-dc2d996c8290",
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
              "id": "ba81b849-e624-493b-9971-d77031a47c67"
            }
          ]
        },
        {
          "id": "a3c57d12-98fb-479a-b8c3-59a0efea574a",
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
              "id": "3e349e17-9da7-41ed-8567-1b4a823d20b2"
            }
          ]
        },
        {
          "id": "fe32d563-8260-4367-a558-cba21e38ef4f",
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
              "id": "3e15a3ca-4b70-4e94-a2e9-d857f4ac69b1"
            }
          ]
        },
        {
          "id": "c59ef43b-4cb7-4f35-9040-42d0c336079b",
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
              "id": "a9c16e53-40e9-49b6-a94b-f8b7c0aa2305"
            }
          ]
        },
        {
          "id": "72dba20c-af4d-40d9-a907-99e61204d03c",
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
              "id": "7b0f2fef-9525-40aa-bb34-47262651c025"
            }
          ]
        },
        {
          "id": "78e67fc5-c4cb-4813-bbe9-47fec711b90c",
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
              "id": "5fb19621-1fb1-4246-8667-2c26cf1c7e70"
            }
          ]
        },
        {
          "id": "bef10ba1-4255-432a-a9f2-1c29619685f7",
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
              "id": "0d5017f3-02cc-458e-9fe3-a505e92d7399"
            }
          ]
        },
        {
          "id": "4d1f32d6-416e-485d-a377-972a4f61a15d",
          "name": "getRestPaymentsMethodnames",
          "request": {
            "url": "http://example.com/rest/payments/methodNames?itemsPerPage=%7B%7D&page=%7B%7D",
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
            "description": "Lists all payment method names."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15bb9dc2-a886-41f6-bd64-e06154a1dcc6"
            }
          ]
        },
        {
          "id": "3cfb8b04-2150-47c4-9798-b4da087783ab",
          "name": "getRestPropertiesGroupsNames",
          "request": {
            "url": "http://example.com/rest/properties/groups/names",
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
            "description": "Lists group names."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86753aa7-18cc-4fb9-bc56-9bfdbbc5c00a"
            }
          ]
        },
        {
          "id": "e0faee6d-485b-4408-bf33-170d8b13d9a0",
          "name": "getRestPropertiesNames",
          "request": {
            "url": "http://example.com/rest/properties/names",
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
            "description": "Lists names."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e39c5df9-3bc2-4b2b-ada1-187f82365159"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "daf558b1-b1d6-45ec-b9f8-1c1ebb32f01e",
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
              "id": "f05889fb-357d-412c-adb1-c8e1552ca757"
            }
          ]
        }
      ]
    }
  ]
}