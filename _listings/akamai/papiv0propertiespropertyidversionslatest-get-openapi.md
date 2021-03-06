---
swagger: "2.0"
x-collection-name: Akamai
x-complete: 0
info:
  title: Akamai API Get a Property&#8217;s Latest Version
  description: Get a Property&#8217;s Latest Version
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /papi/v0/properties/{propertyId}/versions/latest:
    get:
      summary: Get a Property&#8217;s Latest Version
      description: Get a Property&#8217;s Latest Version
      operationId: papiv0propertiespropertyidversionslatestcontractidgroupidactivatedon
      x-api-path-slug: papiv0propertiespropertyidversionslatest-get
      parameters:
      - in: query
        name: activatedOn
        description: If present, returns the latest version activated on the given
          network, either STAGING or PRODUCTION
        type: string
      - in: query
        name: contractId
        description: Unique identifier for the contract
        type: string
      - in: query
        name: groupId
        description: Unique identifier for the group
        type: string
      - in: query
        name: propertyId
        description: Unique identifier for the property
        type: string
      responses:
        200:
          description: OK
      tags:
      - Papi
      - V0
      - Properties
      - Property
      - Versions
      - Latest
      - Contract
      - group
      - activatedon
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