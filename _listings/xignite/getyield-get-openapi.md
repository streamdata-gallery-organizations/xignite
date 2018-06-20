---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Bonds Get Yield
  description: Returns Yield to maturity for a specific bond reported by the price
    source selected in the input. Request against this operation counts as one hit.
  version: 1.0.0
host: bonds.xignite.com
basePath: xBonds.json/XigniteBonds
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetPriceComposite:
    get:
      summary: Get Price Composite
      description: Returns price data composite including last sale price, yield and
        daily and yearly Open, High, Low prices for a specific bond reported by price
        source selected in the input. Return against this operation counts as three
        hits.
      operationId: GetPriceComposite
      x-api-path-slug: getpricecomposite-get
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
      - Price
      - Composite
  /GetLastSale:
    get:
      summary: Get Last Sale
      description: Returns Last Sale price for a specific bond as reported by the
        price source selected in the input. Request against this operation counts
        as one hit.
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
      - Market Data
      - Last
      - Sale
  /GetDailyOpenHighLowClosePrice:
    get:
      summary: Get Daily Open High Low Close Price
      description: Returns daily Open, High, Low, Close (OHLC) prices for a specific
        bond reported by the price source selected in the input. Daily OHLC data is
        provided for the most recent date for which data is provided by the price
        source. Request against this operation counts as one hit.
      operationId: GetDailyOpenHighLowClosePrice
      x-api-path-slug: getdailyopenhighlowcloseprice-get
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
      - Daily
      - Open
      - High
      - Low
      - Close
      - Price
  /GetYearlyHighLowPrice:
    get:
      summary: Get Yearly High Low Price
      description: Returns yearly high, low prices for a specific bond reported by
        the price source selected in the input. Request against this operation counts
        as one hit.
      operationId: GetYearlyHighLowPrice
      x-api-path-slug: getyearlyhighlowprice-get
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
      - Yearly
      - High
      - Low
      - Price
  /GetYield:
    get:
      summary: Get Yield
      description: Returns Yield to maturity for a specific bond reported by the price
        source selected in the input. Request against this operation counts as one
        hit.
      operationId: GetYield
      x-api-path-slug: getyield-get
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
      - Yield
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