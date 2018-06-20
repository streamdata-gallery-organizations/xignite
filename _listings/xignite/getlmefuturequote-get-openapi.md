---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Futures Get LME Future Quote
  description: Returns latest quotes for LME futures
  version: 1.0.0
host: globalfutures.xignite.com
basePath: xGlobalFutures.json/XigniteGlobalFutures
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetFrontMonthFuture:
    get:
      summary: Get Front Month Future
      description: Returns master data on the front month future contract
      operationId: GetFrontMonthFuture
      x-api-path-slug: getfrontmonthfuture-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Front
      - Month
      - Future
  /GetFutureQuote:
    get:
      summary: Get Future Quote
      description: Returns a delayed quote for a future contract.
      operationId: GetFutureQuote
      x-api-path-slug: getfuturequote-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Future
      - Quote
  /GetLatestFutureQuote:
    get:
      summary: Get Latest Future Quote
      description: Returns the latest delayed quote for a future contract.
      operationId: GetLatestFutureQuote
      x-api-path-slug: getlatestfuturequote-get
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
      - Future
      - Quote
  /GetFutureQuotes:
    get:
      summary: Get Future Quotes
      description: Returns delayed quotes for multiple future contracts.
      operationId: GetFutureQuotes
      x-api-path-slug: getfuturequotes-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Future
      - Quotes
  /GetLatestFutureQuotes:
    get:
      summary: Get Latest Future Quotes
      description: Returns latest delayed quotes for multiple future contracts.
      operationId: GetLatestFutureQuotes
      x-api-path-slug: getlatestfuturequotes-get
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
      - Future
      - Quotes
  /GetSpotFutureQuote:
    get:
      summary: Get Spot Future Quote
      description: Returns a delayed spot quote for a future contract.
      operationId: GetSpotFutureQuote
      x-api-path-slug: getspotfuturequote-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Spot
      - Future
      - Quote
  /GetLatestFrontMonthFutureQuotes:
    get:
      summary: Get Latest Front Month Future Quotes
      description: Returns latest quotes for front month futures
      operationId: GetLatestFrontMonthFutureQuotes
      x-api-path-slug: getlatestfrontmonthfuturequotes-get
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
      - Front
      - Month
      - Future
      - Quotes
  /GetAllFutureQuotes:
    get:
      summary: Get All Future Quotes
      description: Returns all delayed future quotes for a future base.
      operationId: GetAllFutureQuotes
      x-api-path-slug: getallfuturequotes-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Future
      - Quotes
  /GetLMEFutureQuote:
    get:
      summary: Get LME Future Quote
      description: Returns latest quotes for LME futures
      operationId: GetLMEFutureQuote
      x-api-path-slug: getlmefuturequote-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - LME
      - Future
      - Quote
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