{
  "info": {
    "name": "Plentymarkets Lists the debtor accounts by mode.",
    "_postman_id": "5898c270-a807-4b9b-9082-500046196935",
    "description": "Lists the debtor accounts of an accounting location by mode. The ID of the accounting location and the mode have to be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Unique",
      "item": [
        {
          "id": "b3974dfb-cdd0-474c-803d-d9daf12d9966",
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
              "id": "3e819212-6df8-43a5-84ad-9572f8d05e0f"
            }
          ]
        }
      ]
    },
    {
      "name": "Posting",
      "item": [
        {
          "id": "38f5e630-446e-4206-a858-69c0b5c51e92",
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
              "id": "a324df16-bd79-4b3e-9db2-12589874e545"
            }
          ]
        }
      ]
    },
    {
      "name": "Save",
      "item": [
        {
          "id": "abd7f861-e5b3-4b3e-9e98-43c68978cb2f",
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
              "id": "fd3e27a6-d60b-4baf-b128-22fa6e6e1e5b"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "28d7c165-6742-4066-a7e9-e5652c3829b5",
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
              "id": "47b68a70-5c85-4da6-bef4-b7b3551bdf67"
            }
          ]
        }
      ]
    }
  ]
}