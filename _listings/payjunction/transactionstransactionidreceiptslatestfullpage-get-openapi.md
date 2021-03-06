---
swagger: "2.0"
x-collection-name: PayJunction
x-complete: 0
info:
  title: PayJunction Get Transactions Receipts Latest Fullpage
  description: Get the most recent version of the full page (8.5x11) receipt HTML
    document
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /transactions/{transactionId}/receipts/latest/email:
    post:
      summary: Post Transactions Receipts Latest Email
      description: /transactions/{transactionid}/receipts/latest/email.
      operationId: TransactionsReceiptsLatestEmailByTransactionIdPost
      x-api-path-slug: transactionstransactionidreceiptslatestemail-post
      parameters:
      - in: formData
        name: replyTo
      - in: formData
        name: requestSignature
      - in: formData
        name: to
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Receipts
      - Latest
      - Email
  /transactions/{transactionId}/receipts/latest:
    get:
      summary: Get Transactions Receipts Latest
      description: Retrieve the most recent version of the receipt.
      operationId: TransactionsReceiptsLatestByTransactionIdGet
      x-api-path-slug: transactionstransactionidreceiptslatest-get
      parameters:
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Receipts
      - Latest
  /transactions/{transactionId}/receipts/latest/thermal:
    get:
      summary: Get Transactions Receipts Latest Thermal
      description: Get the most recent version of the thermal receipt HTML Document
      operationId: TransactionsReceiptsLatestThermalByTransactionIdGet
      x-api-path-slug: transactionstransactionidreceiptslatestthermal-get
      parameters:
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Receipts
      - Latest
      - Thermal
  /transactions/{transactionId}/receipts/latest/fullpage:
    get:
      summary: Get Transactions Receipts Latest Fullpage
      description: Get the most recent version of the full page (8.5x11) receipt HTML
        document
      operationId: TransactionsReceiptsLatestFullpageByTransactionIdGet
      x-api-path-slug: transactionstransactionidreceiptslatestfullpage-get
      parameters:
      - in: path
        name: transactionId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Transactions
      - Receipts
      - Latest
      - Fullpage
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