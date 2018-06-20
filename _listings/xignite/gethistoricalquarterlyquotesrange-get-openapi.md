---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Historical Get Historical Quarterly Quotes Range
  description: This operation returns end of quarter quotes for a US equity. This
    includes split adjusted price.
  version: 1.0.0
host: www.xignite.com
basePath: xHistorical.json/XigniteHistorical
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetHistoricalQuoteAdjusted:
    get:
      summary: Get Historical Quote Adjusted
      description: Returns a quote as of a historical date. This includes split and
        dividends adjusted price.
      operationId: postGethistoricalquoteadjusted
      x-api-path-slug: gethistoricalquoteadjusted-get
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
      - Historical
      - Quote
      - Adjusted
  /GetHistoricalQuotesAdjusted:
    get:
      summary: Get Historical Quotes Adjusted
      description: Returns a quote as of a historical date. This includes split and
        dividends adjusted price.
      operationId: postGethistoricalquotesadjusted
      x-api-path-slug: gethistoricalquotesadjusted-get
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
      - Historical
      - Quotes
      - Adjusted
  /GetHistoricalMonthlyQuotesRangeAdjusted:
    get:
      summary: Get Historical Monthly Quotes Range Adjusted
      description: This operation returns end of month quotes for a US equity. This
        includes split and dividends adjusted price.
      operationId: postGethistoricalmonthlyquotesrangeadjusted
      x-api-path-slug: gethistoricalmonthlyquotesrangeadjusted-get
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
      - Historical
      - Monthly
      - Quotes
      - Range
      - Adjusted
  /GetHistoricalQuotesAsOfAdjusted:
    get:
      summary: Get Historical Quotes As Of Adjusted
      description: This operation returns a range of quotes for a security. This includes
        split and dividends adjusted price.
      operationId: postGethistoricalquotesasofadjusted
      x-api-path-slug: gethistoricalquotesasofadjusted-get
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
      - Historical
      - Quotes
      - As
      - Adjusted
  /GetHistoricalQuotesRangeAdjusted:
    get:
      summary: Get Historical Quotes Range Adjusted
      description: This operation returns a complete range of stock quotes for a US
        equity. This includes and dividends adjusted price.
      operationId: postGethistoricalquotesrangeadjusted
      x-api-path-slug: gethistoricalquotesrangeadjusted-get
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
      - Historical
      - Quotes
      - Range
      - Adjusted
  /GetHistoricalWeeklyQuotesRangeAdjusted:
    get:
      summary: Get Historical Weekly Quotes Range Adjusted
      description: This operation returns end of week quotes for a US equity. This
        includes split and dividends adjusted price.
      operationId: postGethistoricalweeklyquotesrangeadjusted
      x-api-path-slug: gethistoricalweeklyquotesrangeadjusted-get
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
      - Historical
      - Weekly
      - Quotes
      - Range
      - Adjusted
  /GetHistoricalQuarterlyQuotesRangeAdjusted:
    get:
      summary: Get Historical Quarterly Quotes Range Adjusted
      description: This operation returns end of quarter quotes for a US equity. This
        includes split and dividends adjusted price.
      operationId: postGethistoricalquarterlyquotesrangeadjusted
      x-api-path-slug: gethistoricalquarterlyquotesrangeadjusted-get
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
      - Historical
      - Quarterly
      - Quotes
      - Range
      - Adjusted
  /GetLastClosingPrice:
    get:
      summary: Get Last Closing Price
      description: Returns last closing price for a security.
      operationId: postGetlastclosingprice
      x-api-path-slug: getlastclosingprice-get
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
      - Closing
      - Price
  /GetLastClosingPriceAdjusted:
    get:
      summary: Get Last Closing Price Adjusted
      description: Returns last closing price for a security. This include the splits
        and dividends adjusted price
      operationId: postGetlastclosingpriceadjusted
      x-api-path-slug: getlastclosingpriceadjusted-get
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
      - Closing
      - Price
      - Adjusted
  /GetLastClosingPrices:
    get:
      summary: Get Last Closing Prices
      description: Returns last closing price for a collection of securities.
      operationId: postGetlastclosingprices
      x-api-path-slug: getlastclosingprices-get
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
      - Closing
      - Prices
  /GetLastClosingPricesAdjusted:
    get:
      summary: Get Last Closing Prices Adjusted
      description: Returns last closing price for a collection of securities.This
        include the splits and dividends adjusted price
      operationId: postGetlastclosingpricesadjusted
      x-api-path-slug: getlastclosingpricesadjusted-get
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
      - Closing
      - Prices
      - Adjusted
  /GetLastClosingPricesOrdered:
    get:
      summary: Get Last Closing Prices Ordered
      description: Returns last closing price for a collection of securities.
      operationId: postGetlastclosingpricesordered
      x-api-path-slug: getlastclosingpricesordered-get
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
      - Closing
      - Prices
      - Ordered
  /GetLastClosingPricesOrderedAdjusted:
    get:
      summary: Get Last Closing Prices Ordered Adjusted
      description: Returns last closing price for a collection of securities.This
        include the splits and dividends adjusted price
      operationId: postGetlastclosingpricesorderedadjusted
      x-api-path-slug: getlastclosingpricesorderedadjusted-get
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
      - Closing
      - Prices
      - Ordered
      - Adjusted
  /GetHistoricalHighLow:
    get:
      summary: Get Historical High Low
      description: Returns a historical high low for a time range.
      operationId: postGethistoricalhighlow
      x-api-path-slug: gethistoricalhighlow-get
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
      - Historical
      - High
      - Low
  /GetHistoricalQuote:
    get:
      summary: Get Historical Quote
      description: Returns a quote as of a historical date. This includes split adjusted
        price.
      operationId: postGethistoricalquote
      x-api-path-slug: gethistoricalquote-get
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
      - Historical
      - Quote
  /GetHistoricalQuotes:
    get:
      summary: Get Historical Quotes
      description: Returns a quote as of a historical date. This includes split adjusted
        price.
      operationId: postGethistoricalquotes
      x-api-path-slug: gethistoricalquotes-get
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
      - Historical
      - Quotes
  /GetHistoricalQuotesAsOf:
    get:
      summary: Get Historical Quotes As Of
      description: This operation returns a range of quotes for a security.
      operationId: postGethistoricalquotesasof
      x-api-path-slug: gethistoricalquotesasof-get
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
      - Historical
      - Quotes
      - As
      - Of
  /GetHistoricalQuotesRange:
    get:
      summary: Get Historical Quotes Range
      description: This operation returns a complete range of stock quotes for a US
        equity. This includes split adjusted price.
      operationId: postGethistoricalquotesrange
      x-api-path-slug: gethistoricalquotesrange-get
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
      - Historical
      - Quotes
      - Range
  /GetHistoricalMonthlyQuotesRange:
    get:
      summary: Get Historical Monthly Quotes Range
      description: This operation returns end of month quotes for a US equity. This
        includes split adjusted price.
      operationId: postGethistoricalmonthlyquotesrange
      x-api-path-slug: gethistoricalmonthlyquotesrange-get
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
      - Historical
      - Monthly
      - Quotes
      - Range
  /GetHistoricalWeeklyQuotesRange:
    get:
      summary: Get Historical Weekly Quotes Range
      description: This operation returns end of week quotes for a US equity. This
        includes split adjusted price.
      operationId: postGethistoricalweeklyquotesrange
      x-api-path-slug: gethistoricalweeklyquotesrange-get
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
      - Historical
      - Weekly
      - Quotes
      - Range
  /GetHistoricalQuarterlyQuotesRange:
    get:
      summary: Get Historical Quarterly Quotes Range
      description: This operation returns end of quarter quotes for a US equity. This
        includes split adjusted price.
      operationId: postGethistoricalquarterlyquotesrange
      x-api-path-slug: gethistoricalquarterlyquotesrange-get
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
      - Historical
      - Quarterly
      - Quotes
      - Range
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