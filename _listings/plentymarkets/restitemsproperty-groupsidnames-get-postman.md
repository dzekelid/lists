{
  "info": {
    "name": "Plentymarkets List the property group names of a property group",
    "_postman_id": "178e1f55-1dd4-4bd6-ab0c-40c66976f65f",
    "description": "Lists the property group names of a property group in all languages. The ID of the property group must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "e607ced7-5ebc-4204-8f21-f2f01a29c4ca",
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
              "id": "99c36c48-15ea-4f16-b9ed-0494e67dffad"
            }
          ]
        },
        {
          "id": "b813033d-e347-437b-9442-f89a61ee4073",
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
              "id": "791d05c4-c1d7-460b-b64d-16325125896c"
            }
          ]
        },
        {
          "id": "b1575efc-36dc-4ea2-ab51-5e07a26eda48",
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
              "id": "76ff8eee-53a7-4b20-93c4-feee269a830a"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "a66f53c2-9461-43cb-bb72-5ed6c41da41e",
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
              "id": "f94d8d05-b3e4-4aba-890e-5801165b2f3b"
            }
          ]
        }
      ]
    }
  ]
}