{
  "info": {
    "name": "Plentymarkets List accounts",
    "_postman_id": "3ddebc4d-e600-4896-98a3-ecee32c7a723",
    "description": "List accounts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Unique",
      "item": [
        {
          "id": "b3b009df-e683-4d62-8f5b-7c187901f571",
          "name": "getRestAccountingLocationsExistingAccounts",
          "request": {
            "url": "http://example.com/rest/accounting/locations/existing_accounts",
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
            "description": "Get all unique posting accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25322335-e0c5-40c0-8288-53827c302ae8"
            }
          ]
        }
      ]
    },
    {
      "name": "Posting",
      "item": [
        {
          "id": "ca36f73f-1365-4cc0-a763-fc550c540678",
          "name": "getRestAccountingLocationsAddingAccounts",
          "request": {
            "url": "http://example.com/rest/accounting/locations/posting_accounts",
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
            "description": "Get all posting accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cfacd0ae-480b-4265-93d0-2e9acaf0be38"
            }
          ]
        },
        {
          "id": "b19e2d75-64e1-405c-b232-4bc9b88a310b",
          "name": "getRestAccountingLocationsLocationAddingAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/posting_accounts"
              ],
              "variable": [
                {
                  "id": "locationId",
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
            "description": "Get all posting accounts by locationid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d4a9ac4-02b8-4b87-8928-bf10a9c3fb7f"
            }
          ]
        },
        {
          "id": "d57f76db-f112-42aa-8225-afe72676fc2e",
          "name": "getRestAccountingLocationsLocationTypeAddingAccounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/:type/posting_accounts"
              ],
              "variable": [
                {
                  "id": "locationId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "type",
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
            "description": "Get all posting accounts by locationid and type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53e3a755-6a26-4ec2-b130-44757fda39b8"
            }
          ]
        }
      ]
    },
    {
      "name": "Save",
      "item": [
        {
          "id": "4deb6254-4b2c-4921-87ab-3fb451574003",
          "name": "postRestAccountingLocationsAddingAccounts",
          "request": {
            "url": "http://example.com/rest/accounting/locations/posting_accounts",
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
            "description": "Save posting accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d867ee29-8871-4f28-9d81-f0d1a84f800a"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "1f95e96f-a426-4eaf-a660-8829e97ee535",
          "name": "getRestAccountingLocationsLocationDebtorAccountsMode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounting/locations/:locationId/debtor_accounts/:mode"
              ],
              "variable": [
                {
                  "id": "locationId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "mode",
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
            "description": "Lists the debtor accounts of an accounting location by mode. The ID of the accounting location and the mode have to be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0bfa6a03-9515-4495-b697-da119a59a7c1"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "52714ad8-1b7c-4230-8edc-43688483f3bc",
          "name": "getRestAccounts",
          "request": {
            "url": "http://example.com/rest/accounts?createdAt=%7B%7D&updatedAt=%7B%7D",
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
            "description": "List accounts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56122b28-0250-406d-9008-82ba24e78e4d"
            }
          ]
        }
      ]
    }
  ]
}