---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Fact Set Estimates Get Latest Recommendation Summaries
  description: Get Latest Recommendation Summary
  version: 1.0.0
host: factsetestimates.xignite.com
basePath: xFactSetEstimates.json/XigniteFactSetEstimates
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetLatestRecommendationSummaries:
    post:
      summary: Get Latest Recommendation Summaries
      description: Get Latest Recommendation Summary
      operationId: GetLatestRecommendationSummaries
      x-api-path-slug: getlatestrecommendationsummaries-post
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
      - Recommendation
      - Summaries
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