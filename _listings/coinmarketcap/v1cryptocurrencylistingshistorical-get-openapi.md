---
swagger: "2.0"
x-collection-name: CoinMarketCap
x-complete: 0
info:
  title: CoinMarketCap List all cryptocurrencies (historical)
  description: |-
    **This endpoint is not yet available. It is slated for release in Q3 2018.**


    Get a paginated list of all cryptocurrencies with market data for a given historical time. Use the "convert" option to return market values in multiple fiat and cryptocurrency conversions in the same call.
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
  /v1/exchange/listings/latest:
    get:
      summary: List all exchanges (latest)
      description: "Get a paginated list of all cryptocurrency exchanges with 24 hour
        volume. Additional market data fields will be available in the future. You
        can configure this call to sort by 24 hour volume or another field. Use the
        \"convert\" option to return market values in multiple fiat and cryptocurrency
        conversions in the same call.  \n  \n**This endpoint is available on the following
        API plans:**\n  - ~~Starter~~\n  - ~~Hobbyist~~\n  - Standard\n  - Professional\n
        \ - Enterprise\n\n**Cache / Update frequency:** Every ~5 minutes. This endpoint
        will be migrated to ~1 minute updates shortly.  \n  \n  *NOTE: Use this endpoint
        if you need a sorted and paginated list of exchanges. If you want to query
        for market data on a few specific exchanges use /v1/exchange/quotes/latest
        which is optimized for that purpose. The response data between these endpoints
        is otherwise the same.*"
      operationId: getV1ExchangeListingsLatest
      x-api-path-slug: v1exchangelistingslatest-get
      parameters:
      - in: query
        name: convert
        description: Optionally calculate market quotes in up to 32 currencies at
          once by passing a comma-separated list of cryptocurrency or fiat currency
          symbols
      - in: query
        name: limit
        description: Optionally specify the number of results to return
      - in: query
        name: market_type
        description: The type of exchange markets to include in rankings
      - in: query
        name: sort
        description: What field to sort the list of exchanges by
      - in: query
        name: sort_dir
        description: The direction in which to order exchanges against the specified
          sort
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
      - Exchanges
      - (latest)
  /v1/exchange/listings/historical:
    get:
      summary: List all exchanges (historical)
      description: |-
        **This endpoint is not yet available. It is slated for release in Q3 2018.**


        Get a paginated list of all cryptocurrency exchanges with historical market data for a given point in time. Use the "convert" option to return market values in multiple fiat and cryptocurrency conversions in the same call.
      operationId: getV1ExchangeListingsHistorical
      x-api-path-slug: v1exchangelistingshistorical-get
      parameters:
      - in: query
        name: convert
        description: Optionally calculate market quotes in up to 32 currencies at
          once by passing a comma-separated list of cryptocurrency or fiat currency
          symbols
      - in: query
        name: limit
        description: Optionally specify the number of results to return
      - in: query
        name: market_type
        description: The type of exchange markets to include in rankings
      - in: query
        name: sort
        description: What field to sort the list of exchanges by
      - in: query
        name: sort_dir
        description: The direction in which to order exchanges against the specified
          sort
      - in: query
        name: start
        description: Optionally offset the start (1-based index) of the paginated
          list of items to return
      - in: query
        name: timestamp
        description: Timestamp (Unix or ISO 8601) to return historical exchange listings
          for
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - List
      - ""
      - Exchanges
      - (historical)
  /v1/cryptocurrency/listings/latest:
    get:
      summary: List all cryptocurrencies (latest)
      description: "Get a paginated list of all cryptocurrencies with latest market
        data. You can configure this call to sort by market cap or another market
        ranking field. Use the \"convert\" option to return market values in multiple
        fiat and cryptocurrency conversions in the same call.   \n\n\nCryptocurrencies
        are listed by CoinMarketCap Rank by default. You may optionally sort against
        any of the following:\n**name**: The cryptocurrency name.\n**symbol**: The
        cryptocurrency symbol.\n**date_added**: Date cryptocurrency was added to the
        system.\n**market_cap**: market cap (latest trade price x circulating supply).\n**price**:
        latest average trade price across markets.\n**circulating_supply**: approximate
        number of coins currently in circulation.\n**total_supply**: approximate total
        amount of coins in existence right now (minus any coins that have been verifiably
        burned).\n**max_supply**: our best approximation of the maximum amount of
        coins that will ever exist in the lifetime of the currency.\n**num_market_pairs**:
        number of market pairs across all exchanges trading each currency.\n**volume_24h**:
        24 hour trading volume for each currency.\n**percent_change_1h**: 1 hour trading
        price percentage change for each currency.\n**percent_change_24h**: 24 hour
        trading price percentage change for each currency.\n**percent_change_7d**:
        7 day trading price percentage change for each currency.\n\n  **This endpoint
        is available on the following API plans:**\n  - Starter\n  - Hobbyist\n  -
        Standard\n  - Professional\n  - Enterprise\n\n**Cache / Update frequency:**
        Every ~1 minute. \n  \n*NOTE: Use this endpoint if you need a sorted and paginated
        list of cryptocurrencies. If you want to query for market data on a few specific
        cryptocurrencies use /v1/cryptocurrency/quotes/latest which is optimized for
        that purpose. The response data between these endpoints is otherwise the same.*"
      operationId: getV1CryptocurrencyListingsLatest
      x-api-path-slug: v1cryptocurrencylistingslatest-get
      parameters:
      - in: query
        name: convert
        description: Optionally calculate market quotes in up to 32 currencies at
          once by passing a comma-separated list of cryptocurrency or fiat currency
          symbols
      - in: query
        name: cryptocurrency_type
        description: The type of cryptocurrency to include
      - in: query
        name: limit
        description: Optionally specify the number of results to return
      - in: query
        name: sort
        description: What field to sort the list of cryptocurrencies by
      - in: query
        name: sort_dir
        description: The direction in which to order cryptocurrencies against the
          specified sort
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
      - Cryptocurrencies
      - (latest)
  /v1/cryptocurrency/listings/historical:
    get:
      summary: List all cryptocurrencies (historical)
      description: |-
        **This endpoint is not yet available. It is slated for release in Q3 2018.**


        Get a paginated list of all cryptocurrencies with market data for a given historical time. Use the "convert" option to return market values in multiple fiat and cryptocurrency conversions in the same call.
      operationId: getV1CryptocurrencyListingsHistorical
      x-api-path-slug: v1cryptocurrencylistingshistorical-get
      parameters:
      - in: query
        name: convert
        description: Optionally calculate market quotes in up to 32 currencies at
          once by passing a comma-separated list of cryptocurrency or fiat currency
          symbols
      - in: query
        name: cryptocurrency_type
        description: The type of cryptocurrency to include
      - in: query
        name: limit
        description: Optionally specify the number of results to return
      - in: query
        name: sort
        description: What field to sort the list of cryptocurrencies by
      - in: query
        name: sort_dir
        description: The direction in which to order cryptocurrencies against the
          specified sort
      - in: query
        name: start
        description: Optionally offset the start (1-based index) of the paginated
          list of items to return
      - in: query
        name: timestamp
        description: Timestamp (Unix or ISO 8601) to return historical cryptocurrency
          listings for
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - List
      - ""
      - Cryptocurrencies
      - (historical)
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