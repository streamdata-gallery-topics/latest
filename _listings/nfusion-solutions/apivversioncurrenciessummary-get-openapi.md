---
swagger: "2.0"
x-collection-name: nFusion Solutions
x-complete: 0
info:
  title: nFusion API Get latest Summary for requested currency pairs
  description: Current and daily summary information combined into a single quote
  contact:
    name: nFusion Solutions
    url: https://nfusionsolutions.com/contact
    email: support@nfusionsolutions.com
  version: 1.0.0
host: api.nfusionsolutions.biz
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v{version}/Currencies/rate:
    get:
      summary: Get latest mid rate for requested currency pairs
      description: Get latest mid rate for requested currency pairs.
      operationId: ApiV{versionCurrenciesRateGet
      x-api-path-slug: apivversioncurrenciesrate-get
      parameters:
      - in: query
        name: format
        description: to override content negotiation specify a value of json or xml
      - in: query
        name: pairs
        description: comma separated list of currency pairs
      - in: query
        name: token
        description: auth token
      - in: path
        name: version
        description: The requested API version
      responses:
        200:
          description: OK
      tags:
      - Latest
      - Mid
      - Raterequested
      - Currency
      - Pairs
  /api/v{version}/Currencies/summary:
    get:
      summary: Get latest Summary for requested currency pairs
      description: Current and daily summary information combined into a single quote
      operationId: ApiV{versionCurrenciesSummaryGet
      x-api-path-slug: apivversioncurrenciessummary-get
      parameters:
      - in: query
        name: format
        description: to override content negotiation specify a value of json or xml
      - in: query
        name: pairs
        description: comma separated list of currency pairs
      - in: query
        name: token
        description: auth token
      - in: path
        name: version
        description: The requested API version
      responses:
        200:
          description: OK
      tags:
      - Latest
      - Summaryrequested
      - Currency
      - Pairs
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