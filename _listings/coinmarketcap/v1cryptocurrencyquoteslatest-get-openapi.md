---
swagger: "2.0"
x-collection-name: CoinMarketCap
x-complete: 0
info:
  title: CoinMarketCap Get market quotes (latest)
  description: |-
    Get the latest market quote for 1 or more cryptocurrencies. Use the "convert" option to return market values in multiple fiat and cryptocurrency conversions in the same call.

    **This endpoint is available on the following API plans:**
    - Starter
    - Hobbyist
    - Standard
    - Professional
    - Enterprise

    **Cache / Update frequency:** Every ~1 minute.
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
  /v1/global-metrics/quotes/latest:
    get:
      summary: Get aggregate market metrics (latest)
      description: |-
        Get the latest quote of aggregate market metrics. Use the "convert" option to return market values in multiple fiat and cryptocurrency conversions in the same call.

        **This endpoint is available on the following API plans:**
        - Starter
        - Hobbyist
        - Standard
        - Professional
        - Enterprise

        **Cache / Update frequency:** Every ~5 minutes. This endpoint will be migrated to ~1 minute updates shortly.
      operationId: getV1GlobalmetricsQuotesLatest
      x-api-path-slug: v1globalmetricsquoteslatest-get
      parameters:
      - in: query
        name: convert
        description: Optionally calculate market quotes in up to 32 currencies at
          once by passing a comma-separated list of cryptocurrency or fiat currency
          symbols
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Aggregate
      - Market
      - Metrics
      - (latest)
  /v1/exchange/quotes/latest:
    get:
      summary: Get market quotes (latest)
      description: |-
        Get the latest 24 hour volume quote for 1 or more exchanges. Additional market data fields will be available in the future. Use the "convert" option to return market values in multiple fiat and cryptocurrency conversions in the same call.

        **This endpoint is available on the following API plans:**
        - ~~Starter~~
        - ~~Hobbyist~~
        - Standard
        - Professional
        - Enterprise

        **Cache / Update frequency:** Every ~5 minutes. This endpoint will be migrated to ~1 minute updates shortly.
      operationId: getV1ExchangeQuotesLatest
      x-api-path-slug: v1exchangequoteslatest-get
      parameters:
      - in: query
        name: convert
        description: Optionally calculate market quotes in up to 32 currencies at
          once by passing a comma-separated list of cryptocurrency or fiat currency
          symbols
      - in: query
        name: id
        description: One or more comma-separated CoinMarketCap exchange IDs
      - in: query
        name: slug
        description: Alternatively, pass a comma-separated list of exchange slugs
          (URL friendly all lowercase shorthand version of name with spaces replaced
          with hyphens)
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Market
      - Quotes
      - (latest)
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
  /v1/cryptocurrency/quotes/latest:
    get:
      summary: Get market quotes (latest)
      description: |-
        Get the latest market quote for 1 or more cryptocurrencies. Use the "convert" option to return market values in multiple fiat and cryptocurrency conversions in the same call.

        **This endpoint is available on the following API plans:**
        - Starter
        - Hobbyist
        - Standard
        - Professional
        - Enterprise

        **Cache / Update frequency:** Every ~1 minute.
      operationId: getV1CryptocurrencyQuotesLatest
      x-api-path-slug: v1cryptocurrencyquoteslatest-get
      parameters:
      - in: query
        name: convert
        description: Optionally calculate market quotes in up to 32 currencies at
          once by passing a comma-separated list of cryptocurrency or fiat currency
          symbols
      - in: query
        name: id
        description: One or more comma-separated cryptocurrency CoinMarketCap IDs
      - in: query
        name: symbol
        description: Alternatively pass one or more comma-separated cryptocurrency
          symbols
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Market
      - Quotes
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