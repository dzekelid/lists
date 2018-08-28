---
swagger: "2.0"
x-collection-name: CoinMarketCap
x-complete: 0
info:
  title: CoinMarketCap List all market pairs (latest)
  description: |-
    Get a list of active market pairs for an exchange. Active means the market pair is open for trading. Use the "convert" option to return market values in multiple fiat and cryptocurrency conversions in the same call.'

      **This endpoint is available on the following API plans:**
      - ~~Starter~~
      - ~~Hobbyist~~
      - Standard
      - Professional
      - Enterprise

    **Cache / Update frequency:** Every ~5 minutes. This endpoint will be migrated to ~1 minute updates shortly.
  termsOfService: https://coinmarketcap.com/terms/
  version: 1.0.0
host: pro-api.coinmarketcap.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/exchange/market-pairs/latest:
    get:
      summary: List all market pairs (latest)
      description: |-
        Get a list of active market pairs for an exchange. Active means the market pair is open for trading. Use the "convert" option to return market values in multiple fiat and cryptocurrency conversions in the same call.'

          **This endpoint is available on the following API plans:**
          - ~~Starter~~
          - ~~Hobbyist~~
          - Standard
          - Professional
          - Enterprise

        **Cache / Update frequency:** Every ~5 minutes. This endpoint will be migrated to ~1 minute updates shortly.
      operationId: getV1ExchangeMarketpairsLatest
      x-api-path-slug: v1exchangemarketpairslatest-get
      parameters:
      - in: query
        name: convert
        description: Optionally calculate market quotes in up to 32 currencies at
          once by passing a comma-separated list of cryptocurrency or fiat currency
          symbols
      - in: query
        name: id
        description: A CoinMarketCap exchange ID
      - in: query
        name: limit
        description: Optionally specify the number of results to return
      - in: query
        name: slug
        description: Alternatively pass an exchange slug (URL friendly all lowercase
          shorthand version of name with spaces replaced with hyphens)
      - in: query
        name: start
        description: Optionally offset the start (1-based index) of the paginated
          list of items to return
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - List
      - ""
      - Market
      - Pairs
      - (latest)
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---