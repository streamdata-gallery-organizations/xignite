---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Historical Get Cash Dividend History
  description: Get cash dividend history for a stock for a date range.
  version: 1.0.0
host: www.xignite.com
basePath: xGlobalHistorical.json/XigniteGlobalHistorical
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetGlobalLastClosingPrice:
    get:
      summary: Get Global Last Closing Price
      description: Returns last closing price for a security.
      operationId: postGetgloballastclosingprice
      x-api-path-slug: getgloballastclosingprice-get
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
      - Global
      - Last
      - Closing
      - Price
  /GetGlobalLastClosingPrices:
    get:
      summary: Get Global Last Closing Prices
      description: Returns last closing price for a collection of securities.
      operationId: postGetgloballastclosingprices
      x-api-path-slug: getgloballastclosingprices-get
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
      - Global
      - Last
      - Closing
      - Prices
  /GetGlobalHistoricalQuote:
    get:
      summary: Get Global Historical Quote
      description: Returns a quote as of a historical date. This includes the adjusted
        price as specified.
      operationId: postGetglobalhistoricalquote
      x-api-path-slug: getglobalhistoricalquote-get
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
      - Global
      - Historical
      - Quote
  /GetEndOfDayQuote:
    get:
      summary: Get End Of Day Quote
      description: Returns a quote as of a historical date. This includes the adjusted
        price as specified.
      operationId: postGetendofdayquote
      x-api-path-slug: getendofdayquote-get
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
      - End
      - Of
      - Day
      - Quote
  /GetEndOfDayQuotes:
    get:
      summary: Get End Of Day Quotes
      description: Returns a quote as of a historical date. This includes the adjusted
        price as specified.
      operationId: postGetendofdayquotes
      x-api-path-slug: getendofdayquotes-get
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
      - End
      - Of
      - Day
      - Quotes
  /GetEndOfDayQuotesRange:
    get:
      summary: Get End Of Day Quotes Range
      description: Returns a quote a complete range of stock quotes for a given equity.
        This includes the adjusted price as specified.
      operationId: postGetendofdayquotesrange
      x-api-path-slug: getendofdayquotesrange-get
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
      - End
      - Of
      - Day
      - Quotes
      - Range
  /GetGlobalHistoricalQuotes:
    get:
      summary: Get Global Historical Quotes
      description: Returns quotes as of a historical date. This includes the adjusted
        price as specified.
      operationId: postGetglobalhistoricalquotes
      x-api-path-slug: getglobalhistoricalquotes-get
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
      - Global
      - Historical
      - Quotes
  /GetGlobalHistoricalQuotesAsOf:
    get:
      summary: Get Global Historical Quotes As Of
      description: This operation returns a range of quotes for a security.
      operationId: postGetglobalhistoricalquotesasof
      x-api-path-slug: getglobalhistoricalquotesasof-get
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
      - Global
      - Historical
      - Quotes
      - As
      - Of
  /GetGlobalHistoricalQuotesRange:
    get:
      summary: Get Global Historical Quotes Range
      description: This operation returns a complete range of stock quotes for a given
        equity. This includes the adjusted price as specified.
      operationId: postGetglobalhistoricalquotesrange
      x-api-path-slug: getglobalhistoricalquotesrange-get
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
      - Global
      - Historical
      - Quotes
      - Range
  /GetGlobalHistoricalQuotesRangeExtended:
    get:
      summary: Get Global Historical Quotes Range Extended
      description: This operation returns a complete range of global historical quotes
        extended for a given equity. This includes the adjusted price as specified.
      operationId: postGetglobalhistoricalquotesrangeextended
      x-api-path-slug: getglobalhistoricalquotesrangeextended-get
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
      - Global
      - Historical
      - Quotes
      - Range
      - Extended
  /GetGlobalHistoricalWeeklyQuotesRange:
    get:
      summary: Get Global Historical Weekly Quotes Range
      description: Returns a range of weekly Global Historical quotes for a security.
        For more information, go to http://www.xignite.com/
      operationId: postGetglobalhistoricalweeklyquotesrange
      x-api-path-slug: getglobalhistoricalweeklyquotesrange-get
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
      - Global
      - Historical
      - Weekly
      - Quotes
      - Range
  /GetGlobalHistoricalWeeklyQuotesRangeExtended:
    get:
      summary: Get Global Historical Weekly Quotes Range Extended
      description: Returns a range of weekly Global Historical quotes extended for
        a security. For more information, go to http://www.xignite.com/
      operationId: postGetglobalhistoricalweeklyquotesrangeextended
      x-api-path-slug: getglobalhistoricalweeklyquotesrangeextended-get
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
      - Global
      - Historical
      - Weekly
      - Quotes
      - Range
      - Extended
  /GetGlobalHistoricalQuarterlyQuotesRange:
    get:
      summary: Get Global Historical Quarterly Quotes Range
      description: Returns a range of quarterly Global Historical quotes for a security.
        For more information, go to http://www.xignite.com/
      operationId: postGetglobalhistoricalquarterlyquotesrange
      x-api-path-slug: getglobalhistoricalquarterlyquotesrange-get
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
      - Global
      - Historical
      - Quarterly
      - Quotes
      - Range
  /GetGlobalHistoricalStatistics:
    get:
      summary: Get Global Historical Statistics
      description: Returns Global Historical statistics for a security. For more information,
        go to http://www.xignite.com/
      operationId: postGetglobalhistoricalstatistics
      x-api-path-slug: getglobalhistoricalstatistics-get
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
      - Global
      - Historical
      - Statistics
  /GetGlobalHistoricalMonthlyQuotesRange:
    get:
      summary: Get Global Historical Monthly Quotes Range
      description: This operation returns a range of monthly quotes for an equity
        based on the specified date range. This includes the adjusted price as specified.
      operationId: postGetglobalhistoricalmonthlyquotesrange
      x-api-path-slug: getglobalhistoricalmonthlyquotesrange-get
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
      - Global
      - Historical
      - Monthly
      - Quotes
      - Range
  /GetGlobalHistoricalMonthlyQuotesRangeExtended:
    get:
      summary: Get Global Historical Monthly Quotes Range Extended
      description: This operation returns a range of monthly quotes extended for an
        equity based on the specified date range. This includes the adjusted price
        as specified.
      operationId: postGetglobalhistoricalmonthlyquotesrangeextended
      x-api-path-slug: getglobalhistoricalmonthlyquotesrangeextended-get
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
      - Global
      - Historical
      - Monthly
      - Quotes
      - Range
      - Extended
  /GetTopMoversByExchange:
    get:
      summary: Get Top Movers By Exchange
      description: This operation returns quote information about the top moving equities
        for the requested exchange.
      operationId: postGettopmoversbyexchange
      x-api-path-slug: gettopmoversbyexchange-get
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
      - Top
      - Movers
      - By
      - Exchange
  /GetTopGainersByExchange:
    get:
      summary: Get Top Gainers By Exchange
      description: This operation returns quote information about the top gaining
        equities for the requested exchange.
      operationId: postGettopgainersbyexchange
      x-api-path-slug: gettopgainersbyexchange-get
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
      - Top
      - Gainers
      - By
      - Exchange
  /GetTopLosersByExchange:
    get:
      summary: Get Top Losers By Exchange
      description: This operation returns quote information about the top losing equities
        for the requested exchange.
      operationId: postGettoplosersbyexchange
      x-api-path-slug: gettoplosersbyexchange-get
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
      - Top
      - Losers
      - By
      - Exchange
  /GetAllSplitsByExchange:
    get:
      summary: Get All Splits By Exchange
      description: Get all splits for a date range in the specified exchange.
      operationId: postGetallsplitsbyexchange
      x-api-path-slug: getallsplitsbyexchange-get
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
      - Splits
      - By
      - Exchange
  /GetSplitRatio:
    get:
      summary: Get Split Ratio
      description: Return the cumulative split ratio for a security between two dates.
        For instance, if a security saw a 3:1 split and 2:1 split during the period,
        the split ratio 6 is returned. Returns 1 if no split occurred.
      operationId: postGetsplitratio
      x-api-path-slug: getsplitratio-get
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
      - Split
      - Ratio
  /GetSplitHistory:
    get:
      summary: Get Split History
      description: Get split history for a stock for a date range.
      operationId: postGetsplithistory
      x-api-path-slug: getsplithistory-get
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
      - Split
      - History
  /GetAllCashDividendsByExchange:
    get:
      summary: Get All Cash Dividends By Exchange
      description: Get all cash dividends for a date range in the specified exchange.
      operationId: postGetallcashdivendsbyexchange
      x-api-path-slug: getallcashdividendsbyexchange-get
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
      - Cash
      - Dividends
      - By
      - Exchange
  /GetCashDividendTotal:
    get:
      summary: Get Cash Dividend Total
      description: Return the cumulative cash dividend total for a security between
        two dates.
      operationId: postGetcashdivendtotal
      x-api-path-slug: getcashdividendtotal-get
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
      - Cash
      - Dividend
      - Total
  /GetCashDividendHistory:
    get:
      summary: Get Cash Dividend History
      description: Get cash dividend history for a stock for a date range.
      operationId: postGetcashdivendhistory
      x-api-path-slug: getcashdividendhistory-get
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
      - Cash
      - Dividend
      - History
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