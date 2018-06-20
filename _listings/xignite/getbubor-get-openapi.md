---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Interbanks Get BUBOR
  description: Returns a BUBOR as of a date
  version: 1.0.0
host: www.xignite.com
basePath: xInterBanks.json/XigniteInterBanks
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
  /GetLIBORSecure:
    get:
      summary: Get LIBOR Secure
      description: Returns Libor as of a date
      operationId: postGetliborsecure
      x-api-path-slug: getliborsecure-get
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
      - LIBOR
      - Secure
  /GetLIBOR:
    get:
      summary: Get LIBOR
      description: Returns Libor as of a date
      operationId: postGetlibor
      x-api-path-slug: getlibor-get
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
      - LIBOR
  /GetREIBOR:
    get:
      summary: Get REIBOR
      description: Returns a REIBOR as of a date
      operationId: postGetreibor
      x-api-path-slug: getreibor-get
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
      - REIBOR
  /GetHIBOR:
    get:
      summary: Get H I BOR
      description: Returns a HIBOR as of a date
      operationId: postGethibor
      x-api-path-slug: gethibor-get
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
      - H
      - I
      - BOR
  /GetBUBOR:
    get:
      summary: Get BUBOR
      description: Returns a BUBOR as of a date
      operationId: postGetbubor
      x-api-path-slug: getbubor-get
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
      - BUBOR
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