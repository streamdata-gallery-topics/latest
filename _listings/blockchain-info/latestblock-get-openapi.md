---
swagger: "2.0"
x-collection-name: Blockchain Info
x-complete: 0
info:
  title: Blockchain Info Latest Block
  description: Gets the latest block.
  version: 1.0.0
host: blockchain.info
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /latestblock:
    get:
      summary: Latest Block
      description: Gets the latest block.
      operationId: getLatestBlock
      x-api-path-slug: latestblock-get
      parameters:
      - in: query
        name: format
        description: The format to return (json,html)
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Latest
x-streamrank:
  polling_total_time_average: "0.23"
  polling_size_download_average: "11839.08"
  streaming_total_time_average: "0.15"
  streaming_size_download_average: "6012.8"
  change_yes: "162"
  change_no: "1319"
  time_percentage: "37"
  size_percentage: "49"
  change_percentage: "11"
  last_run: "2018-02-21"
  days_run: "1"
  minute_run: "0"
---