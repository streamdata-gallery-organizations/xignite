---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite IPOs Get IPO Performance
  description: Post getipoperformance
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
  /GetIPOList:
    get:
      summary: Get IPO List
      description: Post getipolist
      operationId: GetIPOList
      x-api-path-slug: getipolist-get
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
      - List
  /GetIPODetails:
    get:
      summary: Get IPO Details
      description: Post getipodetails
      operationId: GetIPODetails
      x-api-path-slug: getipodetails-get
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
  /SearchIPOBySymbol:
    get:
      summary: Search IPO By Symbol
      description: Post searchipobysymbol
      operationId: SearchIPOBySymbol
      x-api-path-slug: searchipobysymbol-get
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
      - IPO
      - Symbol
  /SearchIPOByName:
    get:
      summary: Search IPO By Name
      description: Post searchipobyname
      operationId: SearchIPOByName
      x-api-path-slug: searchipobyname-get
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
      - IPO
      - Name
  /GetIPOPerformance:
    get:
      summary: Get IPO Performance
      description: Post getipoperformance
      operationId: GetIPOPerformance
      x-api-path-slug: getipoperformance-get
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
      - Performance
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