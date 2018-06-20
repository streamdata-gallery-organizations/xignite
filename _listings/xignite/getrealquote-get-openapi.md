---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite BATS Real Time Get Real Quote
  description: Returns real time stock quote for a given stock ticker
  version: 1.0.0
host: batsrealtime.xignite.com
basePath: xBATSRealTime.json/XigniteBATSRealTime
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetBars:
    get:
      summary: Get Bars
      description: Returns a set of bars for a stock and a time range during the trading
        day.
      operationId: GetBars
      x-api-path-slug: getbars-get
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
      - Bars
  /GetRealQuote:
    get:
      summary: Get Real Quote
      description: Returns real time stock quote for a given stock ticker
      operationId: GetRealQuote
      x-api-path-slug: getrealquote-get
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