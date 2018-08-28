{
  "info": {
    "name": "nFusion API Get list of currency pairs supported by the Summary endpoint",
    "_postman_id": "f690146d-ade5-4a58-9182-0bd2963bb820",
    "description": "Only the currency pairs in the direction noted can be used with the Summary endpoint.\r\nFor example: USD/CAD is not the same as CAD/USD",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "e92cc941-1d34-4381-9448-ce3cab05b5cc",
          "name": "ApiV{versionCurrenciesRateSupportedGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nfusionsolutions.biz",
              "path": [
                "api/v:version/Currencies/rate/supported"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "version",
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
            "description": "Any of the currencies in this list can be paired with any other currency in this list when supplied to the Rate endpoint.\r\nFor example: USD/CAD,CAD/USD,USD/EUR,EUR/CAD"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1bcc108-13ef-4ec1-aada-0e17e22b62ef"
            }
          ]
        },
        {
          "id": "723bad5e-77ec-4f2a-a3b7-97568f6c9674",
          "name": "ApiV{versionMetalsSupportedCurrencyGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nfusionsolutions.biz",
              "path": [
                "api/v:version/Metals/supported/currency"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "version",
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
            "description": "Get list of currencies supported by metals endpoints for currency conversion."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56afffb5-ce28-4fe7-9fa1-d1f452768b3e"
            }
          ]
        },
        {
          "id": "79c8b536-a3bc-4600-859c-90a7ec8c4321",
          "name": "ApiV{versionCurrenciesSummarySupportedGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nfusionsolutions.biz",
              "path": [
                "api/v:version/Currencies/summary/supported"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "version",
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
            "description": "Only the currency pairs in the direction noted can be used with the Summary endpoint.\r\nFor example: USD/CAD is not the same as CAD/USD"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a65767d-d868-46c1-ae58-874098a62e2c"
            }
          ]
        },
        {
          "id": "75144115-ffa7-4cc8-bd5c-3a3d9b8a73e2",
          "name": "ApiV{versionCurrenciesHistorySupportedGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nfusionsolutions.biz",
              "path": [
                "api/v:version/Currencies/history/supported"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "version",
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
            "description": "Only the currency pairs in the direction noted can be used with the history endpoint.\r\nFor example: USD/CAD is not the same as CAD/USD"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "483c4031-2e26-48cc-a61c-3fd61c9e42dd"
            }
          ]
        }
      ]
    },
    {
      "name": "Latest",
      "item": [
        {
          "id": "a147818a-c2c3-4d3c-9c5d-8a38344a99f3",
          "name": "ApiV{versionCurrenciesRateGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nfusionsolutions.biz",
              "path": [
                "api/v:version/Currencies/rate"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pairs",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "version",
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
            "description": "Get latest mid rate for requested currency pairs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "123df9ad-0968-423a-af27-53cf0bfb7aff"
            }
          ]
        },
        {
          "id": "28cf07b0-d594-41f9-b806-c3be9fb29249",
          "name": "ApiV{versionCurrenciesSummaryGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nfusionsolutions.biz",
              "path": [
                "api/v:version/Currencies/summary"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pairs",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "version",
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
            "description": "Current and daily summary information combined into a single quote"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a23620ec-542c-4163-8bdd-15bf994fac9e"
            }
          ]
        }
      ]
    },
    {
      "name": "Historical",
      "item": [
        {
          "id": "1f17d91f-2f27-4d7a-8ef9-0fe4c69ac705",
          "name": "ApiV{versionCurrenciesHistoryGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nfusionsolutions.biz",
              "path": [
                "api/v:version/Currencies/history"
              ],
              "query": [
                {
                  "key": "end",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "interval",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pairs",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "version",
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
            "description": "Historical OHLC data for the specified period and interval size\r\n\r\nThe combination of the interval parameter and start and end dates can result in results\r\nbeing truncated to conform to result size limits. See comments on interval parameter for details on valid interval values."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1883ffc4-1789-43e8-b040-1bfde44e4df6"
            }
          ]
        }
      ]
    }
  ]
}