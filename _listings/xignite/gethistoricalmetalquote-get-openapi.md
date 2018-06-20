---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Metals Get Historical Metal Quote
  description: Get historical metal quote at a given time.
  version: 1.0.0
host: globalmetals.xignite.com
basePath: xGlobalMetals.json/XigniteGlobalMetals
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetRealTimeMetalQuotes:
    get:
      summary: Get Real Time Metal Quotes
      description: Get real time exchange rate.
      operationId: GetRealTimeMetalQuotes
      x-api-path-slug: getrealtimemetalquotes-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Real
      - Time
      - Metal
      - Quotes
  /GetHistoricalMetalQuotes:
    get:
      summary: Get Historical Metal Quotes
      description: Get cross sectional historical metal quotes at a given time.
      operationId: GetHistoricalMetalQuotes
      x-api-path-slug: gethistoricalmetalquotes-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Metal
      - Quotes
  /GetRealTimeMetalQuote:
    get:
      summary: Get Real Time Metal Quote
      description: Get real time metal quote.
      operationId: GetRealTimeMetalQuote
      x-api-path-slug: getrealtimemetalquote-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Real
      - Time
      - Metal
      - Quote
  ', Bars':
    get:
      summary: Get Chart Bars
      description: Get intraday bars of specified intervals within a time range.
      operationId: GetChartBars
      x-api-path-slug: bars-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Chart
      - Bars
  /ListMetals:
    get:
      summary: List Metals
      description: List all Metals.
      operationId: ListMetals
      x-api-path-slug: listmetals-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Metals
  /GetRealTimeExtendedMetalQuote:
    get:
      summary: Get Real Time Extended Metal Quote
      description: Get real time extended metal quote.
      operationId: GetRealTimeExtendedMetalQuote
      x-api-path-slug: getrealtimeextendedmetalquote-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Real
      - Time
      - Extended
      - Metal
      - Quote
  /GetHistoricalMetalQuote:
    get:
      summary: Get Historical Metal Quote
      description: Get historical metal quote at a given time.
      operationId: GetHistoricalMetalQuote
      x-api-path-slug: gethistoricalmetalquote-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Metal
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