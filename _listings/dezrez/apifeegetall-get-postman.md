{
  "info": {
    "name": "Dezrez Get list of all fees stored",
    "_postman_id": "9956470a-fd11-4088-884e-6a7cea4274e0",
    "description": "Get list of all fees stored.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieves",
      "item": [
        {
          "id": "5fac0b5d-93a8-483c-93b4-11abccd989e2",
          "name": "Cache_GetObjectByitemKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/cache/:itemKey"
              ],
              "variable": [
                {
                  "id": "itemKey",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves an object stored in the cache system by its {itemkey}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1e695a7-b835-403c-8ae1-3966dc437429"
            }
          ]
        },
        {
          "id": "e89213b3-8c74-4517-a22e-4dd997822a48",
          "name": "Cache_GetListBylistKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/cache/List/:listKey"
              ],
              "variable": [
                {
                  "id": "listKey",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of objects stored in the cache system by its {listkey}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "524958e1-7993-4744-8b5f-b8d240e76734"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "2a686433-5fcd-45d4-830f-b2277e3db7aa",
          "name": "Cache_DeleteItemByitemKey",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/cache/:itemKey"
              ],
              "variable": [
                {
                  "id": "itemKey",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the item stored at {itemkey}."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ffe8327-8d62-464e-9b44-fe97c80ad250"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "f5c5fd3d-db5e-4668-a31c-a7adb7d257af",
          "name": "Fee_GetFeesBypageSizeBypageNumber",
          "request": {
            "url": "http://api.dezrez.com/api/fee/getall?pageNumber=%7B%7D&pageSize=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get list of all fees stored."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98fd14ab-b3b6-44e2-aed2-1aa6c22a1691"
            }
          ]
        }
      ]
    }
  ]
}