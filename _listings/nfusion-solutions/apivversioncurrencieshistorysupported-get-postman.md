{
  "info": {
    "name": "nFusion API Get list of currency pairs supported by the history endpoint",
    "_postman_id": "d8977dc0-c493-425a-abc0-114cb8003dae",
    "description": "Only the currency pairs in the direction noted can be used with the history endpoint.\r\nFor example: USD/CAD is not the same as CAD/USD",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "50a78f77-9d84-4a77-b858-53e3c260c213",
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
              "id": "ff77955d-972a-4bd9-a404-f6400eb42f64"
            }
          ]
        },
        {
          "id": "ed1f39d8-791a-4498-b801-9c0d692f81eb",
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
              "id": "cc2b7ccb-4633-4635-8e8b-08c0ee200337"
            }
          ]
        },
        {
          "id": "27dc3c0d-1fbf-4f61-86ef-e00f0debb1aa",
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
              "id": "dbe86bb1-c9a6-48b9-a9b8-4ebd7264084c"
            }
          ]
        },
        {
          "id": "ba0ca89e-33ec-41c2-99c1-e1bb53e4579b",
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
              "id": "e7388737-f5ad-42d5-9ab9-c1182f3f31f4"
            }
          ]
        }
      ]
    },
    {
      "name": "Latest",
      "item": [
        {
          "id": "b152338a-3957-42de-bba7-92592bb03b03",
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
              "id": "f7ebd544-1de7-4f32-b841-bb4775b65b97"
            }
          ]
        },
        {
          "id": "93695201-2d46-45f3-8a50-5b1178cfe0b8",
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
              "id": "d6df1258-f4d4-4fa8-a598-b61cd34129ea"
            }
          ]
        }
      ]
    },
    {
      "name": "Historical",
      "item": [
        {
          "id": "d78afcc6-1283-4574-b72f-8f9f3c4ac7dc",
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
              "id": "2fd5d5ca-4cd8-4d6e-9b03-0017fa9dea64"
            }
          ]
        }
      ]
    }
  ]
}