{
  "info": {
    "name": "Dezrez Get list of batch exports",
    "_postman_id": "64af093b-31ae-4f9f-8b58-da0235cac262",
    "description": "Get list of batch exports.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Remove",
      "item": [
        {
          "id": "c599b06b-91eb-4056-a8b4-82507cb96b6a",
          "name": "AccountingExport_RemoveFromBatchByidBypaymentId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/accounting/exports/batch/:id/removepayment"
              ],
              "query": [
                {
                  "key": "paymentId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
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
            "description": "Remove an individual payment from batch export."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "000fcc4d-6080-4734-8eee-07223a7b7c89"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "9f5f38e1-a52b-4dec-9934-74457f39b3f2",
          "name": "AccountingExport_GetBatchPaymentsBybankAccountIdByincludeProcessed",
          "request": {
            "url": "http://api.dezrez.com/api/accounting/exports/list/batches?bankAccountId=%7B%7D&includeProcessed=%7B%7D",
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
            "description": "Get list of batch exports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "860293df-c7b0-4bc6-8401-17f9f4f59ab1"
            }
          ]
        }
      ]
    }
  ]
}