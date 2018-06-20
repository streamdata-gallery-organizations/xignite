---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite IPOs Get IPO By Status
  description: Post getipobystatus
  version: 1.0.0
host: ipos.xignite.com
basePath: xIPOs.json/XigniteIPOs
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetIPO:
    get:
      summary: Get IPO
      description: Post getipo
      operationId: GetIPO
      x-api-path-slug: getipo-get
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
      - IPO
  /GetIPOCalendar:
    get:
      summary: Get IPO Calendar
      description: Post getipocalendar
      operationId: GetIPOCalendar
      x-api-path-slug: getipocalendar-get
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
      - IPO
      - Calendar
  /GetIPOCalendarByExchange:
    get:
      summary: Get IPO Calendar By Exchange
      description: Post getipocalendarbyexchange
      operationId: GetIPOCalendarByExchange
      x-api-path-slug: getipocalendarbyexchange-get
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
      - IPO
      - Calendar
      - Exchange
  /ListExchanges:
    get:
      summary: List Exchanges
      description: Post listexchanges
      operationId: ListExchanges
      x-api-path-slug: listexchanges-get
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
      - Exchanges
  /GetIPOByStatus:
    get:
      summary: Get IPO By Status
      description: Post getipobystatus
      operationId: GetIPOByStatus
      x-api-path-slug: getipobystatus-get
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
      - IPO
      - Status
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