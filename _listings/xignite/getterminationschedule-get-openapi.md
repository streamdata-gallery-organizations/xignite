---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Futures Get Termination Schedule
  description: Provide a termination schedule for a commodity.
  version: 1.0.0
host: www.xignite.com
basePath: xFutures.json/XigniteFutures
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetFutureSymbol:
    get:
      summary: Get Future Symbol
      description: Returns the symbol for a future based on its month and year.
      operationId: postGetfuturesymbol
      x-api-path-slug: getfuturesymbol-get
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
      - Future
      - Symbol
  /GetReverseFutureSymbol:
    get:
      summary: Get Reverse Future Symbol
      description: Returns the symbol for a future based on its month and year.
      operationId: postGetreversefuturesymbol
      x-api-path-slug: getreversefuturesymbol-get
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
      - Reverse
      - Future
      - Symbol
  /GetTerminationSchedule:
    get:
      summary: Get Termination Schedule
      description: Provide a termination schedule for a commodity.
      operationId: postGetterminationschedule
      x-api-path-slug: getterminationschedule-get
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
      - Termination
      - Schedule
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