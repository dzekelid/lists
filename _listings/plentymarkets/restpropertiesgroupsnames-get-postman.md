{
  "info": {
    "name": "Plentymarkets List group names",
    "_postman_id": "84ae6fa9-7676-4635-be15-c40c223891f6",
    "description": "Lists group names.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "bbe4b351-28e9-4442-984c-b4f2518f2ed6",
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
              "id": "99fc5b1f-1911-4df5-9af6-938b5b6ef5f4"
            }
          ]
        },
        {
          "id": "bc50a848-648d-46b4-a287-3360ce6729eb",
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
              "id": "b4e8ddd2-1cd0-47ae-936d-0e3445142bc7"
            }
          ]
        },
        {
          "id": "ae5ea9ac-a6ff-4093-80f9-273f65f7f80a",
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
              "id": "a94bb06e-b64a-4b47-9402-75be2646e246"
            }
          ]
        },
        {
          "id": "2dcc0a69-0f05-4f90-bf95-daeee1e2b73f",
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
              "id": "e1e90a7a-a140-4ca1-943e-c84e4d5d3336"
            }
          ]
        },
        {
          "id": "f6b28440-3fb5-4f13-a4f4-ea117476fcd9",
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
              "id": "0a38c6ca-90fc-42d5-8362-c65fb287ab25"
            }
          ]
        },
        {
          "id": "2e0c3b98-93fe-4015-8b4d-630c2317018c",
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
              "id": "c9ed21ab-20d5-4763-b87f-034ed0843baf"
            }
          ]
        },
        {
          "id": "a5fcdce2-d8aa-4240-bfe1-91a189060fe0",
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
              "id": "0a4c9626-4f22-4e36-878a-68cde63896b8"
            }
          ]
        },
        {
          "id": "9d227482-efa3-4b65-a6e9-169e858f584e",
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
              "id": "0693a5cd-d15a-42ba-873c-1b61bdef027d"
            }
          ]
        },
        {
          "id": "240347ed-9172-4067-bfd3-e0ddc4c24522",
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
              "id": "aadca667-5edc-4aa1-97ca-ad35e054b6b6"
            }
          ]
        },
        {
          "id": "fe63ecba-d2f0-47b2-b7a3-dcfc9f8d11ec",
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
              "id": "a5100c4c-c068-40da-8976-5806292c5ed3"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "2d1a9d9f-6592-422c-abd9-2a7020c51716",
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
              "id": "b741733e-bbe0-409d-80b4-7dffb892b83c"
            }
          ]
        }
      ]
    }
  ]
}