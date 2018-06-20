---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite NASDAQ Last Sale Get Last Sales With Fallback
  description: Returns a collection of real time stock quotes for a comma-separated
    list of stock quotes.
  version: 1.0.0
host: nasdaqlastsale.xignite.com
basePath: xNASDAQLastSale.json/XigniteNASDAQLastSale
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetLastSale:
    get:
      summary: Get Last Sale
      description: Returns real time stock quote for a given stock ticker
      operationId: GetLastSale
      x-api-path-slug: getlastsale-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Last
      - Sale
  /GetLastSales:
    get:
      summary: Get Last Sales
      description: Returns a collection of real time stock quotes for a comma-separated
        list of stock quotes.
      operationId: GetLastSales
      x-api-path-slug: getlastsales-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Last
      - Sales
  /GetBar:
    get:
      summary: Get Bar
      description: Returns a single bar for a specific time.
      operationId: GetBar
      x-api-path-slug: getbar-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bar
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
      - Bars
  ', Bars':
    get:
      summary: Get Chart Bars
      description: Returns a set of partial bars for a stock and a time range during
        the trading day.
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
      - Chart
      - Bars
  /GetLastSaleByIdentifier:
    get:
      summary: Get Last Sale By Identifier
      description: Returns a real-time quote for a security based on the last trade
        execution.
      operationId: GetLastSaleByIdentifier
      x-api-path-slug: getlastsalebyidentifier-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Last
      - Sale
      - Identifier
  /GetLastSalesByIdentifiers:
    get:
      summary: Get Last Sales By Identifiers
      description: Returns a real-time quote for a security based on the last trade
        execution.
      operationId: GetLastSalesByIdentifiers
      x-api-path-slug: getlastsalesbyidentifiers-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Last
      - Sales
      - Identifiers
  /GetLastSaleWithFallback:
    get:
      summary: Get Last Sale With Fallback
      description: Returns real time stock quote for a given stock ticker
      operationId: GetLastSaleWithFallback
      x-api-path-slug: getlastsalewithfallback-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Last
      - Sale
      - Fallback
  /GetLastSaleByIdentifierWithFallback:
    get:
      summary: Get Last Sale By Identifier With Fallback
      description: Returns a real-time quote for a security based on the last trade
        execution.
      operationId: GetLastSaleByIdentifierWithFallback
      x-api-path-slug: getlastsalebyidentifierwithfallback-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Last
      - Sale
      - Identifier
      - Fallback
  /GetLastSalesWithFallback:
    get:
      summary: Get Last Sales With Fallback
      description: Returns a collection of real time stock quotes for a comma-separated
        list of stock quotes.
      operationId: GetLastSalesWithFallback
      x-api-path-slug: getlastsaleswithfallback-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Last
      - Sales
      - Fallback
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