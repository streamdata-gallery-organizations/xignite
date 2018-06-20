---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Holidays Get Next Date
  description: Get next date.
  version: 1.0.0
host: globalholidays.xignite.com
basePath: xGlobalHolidays.json/XigniteGlobalHolidays
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ListExchanges:
    get:
      summary: List Exchanges
      description: List exchanges.
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
      - List
      - Exchanges
  /ListCurrencies:
    get:
      summary: List Currencies
      description: List currencies.
      operationId: ListCurrencies
      x-api-path-slug: listcurrencies-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Currencies
  /ListFinancialCenters:
    get:
      summary: List Financial Centers
      description: List financial centers.
      operationId: ListFinancialCenters
      x-api-path-slug: listfinancialcenters-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Financial
      - Centers
  /GetHolidays:
    get:
      summary: Get Holidays
      description: Get holidays.
      operationId: GetHolidays
      x-api-path-slug: getholidays-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Holidays
  /ListHolidays:
    get:
      summary: List Holidays
      description: List holidays.
      operationId: ListHolidays
      x-api-path-slug: listholidays-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Holidays
  /GetNextDate:
    get:
      summary: Get Next Date
      description: Get next date.
      operationId: GetNextDate
      x-api-path-slug: getnextdate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Next
      - Date
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