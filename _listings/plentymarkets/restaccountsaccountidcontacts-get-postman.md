{
  "info": {
    "name": "Plentymarkets List contacts",
    "_postman_id": "3b235270-9ddb-44aa-84a6-2cb8961f5e05",
    "description": "Lists contacts of the account. The ID of the account must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "8eff4d9f-642e-4edc-8667-64d5d8444ab2",
          "name": "getRestAccountsContacts",
          "request": {
            "url": "http://example.com/rest/accounts/contacts?billingAddressId=%7B%7D&contactAddress=%7B%7D&contactEmail=%7B%7D&contactId=%7B%7D&countryId=%7B%7D&createdAtAfter=%7B%7D&createdAtBefore=%7B%7D&deliveryAddressId=%7B%7D&email=%7B%7D&externalId=%7B%7D&fullText=%7B%7D&itemsPerPage=%7B%7D&name=%7B%7D&newsletterAllowance=%7B%7D&newsletterAllowanceAfter=%7B%7D&newsletterAllowanceBefore=%7B%7D&number=%7B%7D&page=%7B%7D&plentyId=%7B%7D&postalCode=%7B%7D&privatePhone=%7B%7D&referrerId=%7B%7D&town=%7B%7D&typeId=%7B%7D&updatedAtAfter=%7B%7D&updatedAtBefore=%7B%7D&userId=%7B%7D&with=%7B%7D",
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
            "description": "List contacts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47f7d4a7-58a4-4399-ba70-5ba40920df89"
            }
          ]
        },
        {
          "id": "43658196-bbb2-4f75-b478-df1b4b97edae",
          "name": "getRestAccountsContactsContactAddressesAddresstype",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/contacts/:contactId/addresses/:addressTypeId?"
              ],
              "variable": [
                {
                  "id": "addressTypeId?",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "contactId",
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
            "description": "Lists addresses of the contact. The ID of the contact must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7cae558a-cb58-419d-be77-b25f67b6270f"
            }
          ]
        },
        {
          "id": "02bca8ca-9530-41d0-8cd6-c1331d2c3513",
          "name": "getRestAccountsAccountContacts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/:accountId/contacts"
              ],
              "variable": [
                {
                  "id": "accountId",
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
            "description": "Lists contacts of the account. The ID of the account must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8f8c844-f61a-4029-bf3a-1bff239cdd4e"
            }
          ]
        }
      ]
    }
  ]
}