---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Rates Get Latest Rate Family
  description: Returns latest values for a rate family.
  version: 1.0.0
host: www.xignite.com
basePath: xRates.json/XigniteRates
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetLatestRate:
    post:
      summary: Get Latest Rate
      description: Returns latest value for a rate.
      operationId: postGetlatestrate
      x-api-path-slug: getlatestrate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Latest
      - Rate
  /GetLatestRateSpecial:
    post:
      summary: Get Latest Rate Special
      description: Returns latest value for a rate.
      operationId: postGetlatestratespecial
      x-api-path-slug: getlatestratespecial-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Latest
      - Rate
      - Special
  /GetLatestRateFamily:
    post:
      summary: Get Latest Rate Family
      description: Returns latest values for a rate family.
      operationId: postGetlatestratefamily
      x-api-path-slug: getlatestratefamily-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Latest
      - Rate
      - Family
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