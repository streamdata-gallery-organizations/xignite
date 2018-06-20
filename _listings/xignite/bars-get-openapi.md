---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Super Quotes Get Chart Bars
  description: Returns ChartBars for given security.
  version: 1.0.0
host: superquotes.xignite.com
basePath: xSuperQuotes.json/XigniteSuperQuotes
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetQuote:
    get:
      summary: Get Quote
      description: Returns a quote for a given security.
      operationId: GetQuote
      x-api-path-slug: getquote-get
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
      - Quote
  /GetQuotes:
    get:
      summary: Get Quotes
      description: Returns quotes for given securities.
      operationId: GetQuotes
      x-api-path-slug: getquotes-get
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
      - Quotes
  ', Bars':
    get:
      summary: Get Chart Bars
      description: Returns ChartBars for given security.
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