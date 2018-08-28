{
  "info": {
    "name": "Plentymarkets List the property names",
    "_postman_id": "b87d5ae6-2ed3-4d12-ab00-d63892126e35",
    "description": "Lists the names of a property in all languages. The ID of the property must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "ea77354d-6a1a-43c5-8396-2020416ae4be",
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
              "id": "bcca05d2-709d-45e6-a4fd-1850ccd54eef"
            }
          ]
        },
        {
          "id": "442c2d82-7693-4aad-8954-4fc232921159",
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
              "id": "73411c06-7ecf-41f5-a43c-03e9fed22398"
            }
          ]
        }
      ]
    },
    {
      "name": "Search",
      "item": [
        {
          "id": "178c2919-23b6-4b02-aaf0-6fc7c872cfa2",
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
              "id": "05fc8011-8f6b-43cc-8de4-dca9da5bfea2"
            }
          ]
        }
      ]
    }
  ]
}