---
swagger: "2.0"
x-collection-name: Akamai
x-complete: 0
info:
  title: Akamai API List Availability Reports
  description: List Availability Reports
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
  /sla-api/v1/tests:
    get:
      summary: List Test Configurations
      description: List Test Configurations
      operationId: slaapiv1testsslatestids
      x-api-path-slug: slaapiv1tests-get
      parameters:
      - in: query
        name: slaTestIds
        description: One or more IDs of SLA tests, comma separated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Sla
      - Tests
      - Slatests
  /sla-api/v1/tests/{slaTestId}/reports/performance:
    get:
      summary: List Performance Reports
      description: List Performance Reports
      operationId: slaapiv1testsslatestidreportsperformancestartend
      x-api-path-slug: slaapiv1testsslatestidreportsperformance-get
      parameters:
      - in: query
        name: end
        description: Timestamp for the end of the data window, in UTC 8601 format
        type: string
      - in: query
        name: slaTestId
        description: Unique identifier for the test you wish to run a report on
        type: string
      - in: query
        name: start
        description: Timestamp for the start of the data window, in UTC 8601 format
        type: string
      responses:
        200:
          description: OK
      tags:
      - Sla
      - Tests
      - Slatest
      - Reports
      - Performance
      - Start
      - end
  /sla-api/v1/tests/{slaTestId}/reports/availability:
    get:
      summary: List Availability Reports
      description: List Availability Reports
      operationId: slaapiv1testsslatestidreportsavailabilitystartend
      x-api-path-slug: slaapiv1testsslatestidreportsavailability-get
      parameters:
      - in: query
        name: end
        description: Timestamp for the end of data window, in UTC 8601 format
        type: string
      - in: query
        name: slaTestId
        description: Unique identifier for the test you wish to run a report on
        type: string
      - in: query
        name: start
        description: Timestamp for the start of the data window, in UTC 8601 format
        type: string
      responses:
        200:
          description: OK
      tags:
      - Sla
      - Tests
      - Slatest
      - Reports
      - Availability
      - Start
      - end
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