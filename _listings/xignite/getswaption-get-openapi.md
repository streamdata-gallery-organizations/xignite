---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Money Markets Get Swaption
  description: Returns a Swaption rate
  version: 1.0.0
host: www.xignite.com
basePath: xMoneyMarkets.json/XigniteMoneyMarkets
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetSwapRate:
    get:
      summary: Get Swap Rate
      description: Returns a Swap rate
      operationId: postGetswaprate
      x-api-path-slug: getswaprate-get
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
      - Swap
      - Rate
  /ListRates:
    get:
      summary: List Rates
      description: List supported interest rates.
      operationId: postListrates
      x-api-path-slug: listrates-get
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
      - Rates
  /SearchRates:
    get:
      summary: Search Rates
      description: Search rate names and description
      operationId: postSearchrates
      x-api-path-slug: searchrates-get
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
      - Search
      - Rates
  /GetForwardRateAgreement:
    get:
      summary: Get Forward Rate Agreement
      description: Returns a calculated Forward Rate Agreement as of a date
      operationId: postGetforwardrateagreement
      x-api-path-slug: getforwardrateagreement-get
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
      - Forward
      - Rate
      - Agreement
  /GetEuroDollarFRAStrip:
    get:
      summary: Get Euro Dollar FRA Strip
      description: Returns an IMM EuroDollar Synthetic Forward Rate strip
      operationId: postGeteurodollarfrastrip
      x-api-path-slug: geteurodollarfrastrip-get
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
      - Euro
      - Dollar
      - Strip
  /GetSwaption:
    get:
      summary: Get Swaption
      description: Returns a Swaption rate
      operationId: postGetswaption
      x-api-path-slug: getswaption-get
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
      - Swaption
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