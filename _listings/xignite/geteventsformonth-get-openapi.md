---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Calendar Get Events For Month
  description: Get events for the specified date.
  version: 1.0.0
host: www.xignite.com
basePath: xCalendar.json/XigniteCalendar
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
      - Market Data
      - Bars
  /GetRealQuote:
    get:
      summary: Get Real Quote
      description: Returns real time stock quote for a given stock ticker
      operationId: GetRealQuote
      x-api-path-slug: getrealquote-get
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
      - Real
      - Quote
  /GetRealQuotes:
    get:
      summary: Get Real Quotes
      description: Returns a collection of real time stock quotes for a comma-separated
        list of stock quotes.
      operationId: GetRealQuotes
      x-api-path-slug: getrealquotes-get
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
      - Real
      - Quotes
  /GetRealQuotesByIdentifiers:
    get:
      summary: Get Real Quotes By Identifiers
      description: Returns a collection of real time stock quotes for a comma-separated
        list of stock quotes.
      operationId: GetRealQuotesByIdentifiers
      x-api-path-slug: getrealquotesbyidentifiers-get
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
      - Real
      - Quotes
      - Identifiers
  /GetRealQuoteByIdentifier:
    get:
      summary: Get Real Quote By Identifier
      description: Returns a real-time quote for a security based on the last trade
        execution.
      operationId: GetRealQuoteByIdentifier
      x-api-path-slug: getrealquotebyidentifier-get
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
      - Real
      - Quote
      - Identifier
  /ListTradedSymbols:
    get:
      summary: List Traded Symbols
      description: Returns all symbols and names that are traded recently
      operationId: ListTradedSymbols
      x-api-path-slug: listtradedsymbols-get
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
      - Traded
      - Symbols
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
      - Market Data
      - Bar
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
      - Market Data
      - Chart
      - Bars
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
  /GetAccruedInterest:
    get:
      summary: Get Accrued Interest
      description: Returns Accrued Interest for a specific bond reported by the price
        source selected in the input. Request against this operation counts as one
        hit.
      operationId: GetAccruedInterest
      x-api-path-slug: getaccruedinterest-get
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
      - Accrued
      - Interest
  /GetDurationAndConvexity:
    get:
      summary: Get Duration And Convexity
      description: Returns Duration and Convexity for a specific bond reported by
        the price source selected in the input. Request against this operation counts
        as one hit.
      operationId: GetDurationAndConvexity
      x-api-path-slug: getdurationandconvexity-get
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
      - Duration
      - Convexity
  /GetBondCalculation:
    get:
      summary: Get Bond Calculation
      description: Returns Price, Yield, Accrued Interest and other bond analytics
        data for a specific bond reported by the price source selected in the input.
        Request against this operation counts as four hits.
      operationId: GetBondCalculation
      x-api-path-slug: getbondcalculation-get
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
      - Bond
      - Calculation
  /GetPriceComposites:
    get:
      summary: Get Price Composites
      description: Returns price data composite including last sale price, yield and
        daily and yearly Open, High, Low prices for the list of bonds specified in
        the input. Each PriceComposite object returned in the output counts as three
        hits.
      operationId: GetPriceComposites
      x-api-path-slug: getpricecomposites-get
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
      - Composites
  /GetLastSales:
    get:
      summary: Get Last Sales
      description: Returns Last Sale price for the list of bonds specified in the
        input, as reported by the price source selected in the input. Each LastSale
        object in the result counts as one hit.
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
      - Market Data
      - Last
      - Sales
  /GetDailyOpenHighLowClosePrices:
    get:
      summary: Get Daily Open High Low Close Prices
      description: Returns daily Open, High, Low, Close (OHLC) prices for the list
        of bonds specified in the input. Daily OHLC data is provided for the most
        recent date for which data is provided by the price source. Each DailyOpenHighLowClosePrice
        object  returned counts as one hit.
      operationId: GetDailyOpenHighLowClosePrices
      x-api-path-slug: getdailyopenhighlowcloseprices-get
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
      - Prices
  /GetYearlyHighLowPrices:
    get:
      summary: Get Yearly High Low Prices
      description: Returns yearly high, low prices for the list of bonds specified
        in the input, as reported by the price source selected in the input. Each
        YearlyHighLowPrice object returned counts as one hit.
      operationId: GetYearlyHighLowPrices
      x-api-path-slug: getyearlyhighlowprices-get
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
      - Prices
  /GetYields:
    get:
      summary: Get Yields
      description: Returns Yield to maturity for the list of bonds specified in the
        input, as reported by the price source selected in the input. Each Yields
        object returned counts as one hit.
      operationId: GetYields
      x-api-path-slug: getyields-get
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
      - Yields
  /GetAccruedInterests:
    get:
      summary: Get Accrued Interests
      description: Returns Accrued Interest for the list of bonds specified in the
        input. Each AccruedInterest object in the result counts as one hit.
      operationId: GetAccruedInterests
      x-api-path-slug: getaccruedinterests-get
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
      - Accrued
      - Interests
  /GetDurationAndConvexities:
    get:
      summary: Get Duration And Convexities
      description: Returns Duration and Convexity for a list of bonds provided in
        the input. Each DurationAndConvexity object in the result counts as one hit.
      operationId: GetDurationAndConvexities
      x-api-path-slug: getdurationandconvexities-get
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
      - Duration
      - Convexities
  /GetBondCalculations:
    get:
      summary: Get Bond Calculations
      description: Returns Price, Yield, Accrued Interest and other bond analytics
        data for a list of bonds provided in the input. Each BondCalculations object
        in the result counts as four hits.
      operationId: GetBondCalculations
      x-api-path-slug: getbondcalculations-get
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
      - Bond
      - Calculations
  /ListBondTypes:
    get:
      summary: List Bond Types
      description: ""
      operationId: ListBondTypes
      x-api-path-slug: listbondtypes-get
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
      - Bond
      - Types
  /ListSymbols:
    get:
      summary: List Symbols
      description: ""
      operationId: ListSymbols
      x-api-path-slug: listsymbols-get
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
      - Symbols
  /GetEventsForNextNumberOfDays:
    get:
      summary: Get Events For Next Number Of Days
      description: Get events for the next number of days into the future.
      operationId: postGeteventsfornextnumberofdays
      x-api-path-slug: geteventsfornextnumberofdays-get
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
      - Events
      - Next
      - Number
      - Days
  /GetEventsForWeek:
    get:
      summary: Get Events For Week
      description: Get all the events released during the week specified. Weeks are
        Monday - Sunday.
      operationId: postGeteventsforweek
      x-api-path-slug: geteventsforweek-get
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
      - Events
      - Week
  /ListCountryCodes:
    get:
      summary: List Country Codes
      description: Get all of the country codes available to query on.
      operationId: postListcountrycodes
      x-api-path-slug: listcountrycodes-get
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
      - Country
      - Codes
  /ListEventCodes:
    get:
      summary: List Event Codes
      description: Get all of the event codes available to query on.
      operationId: postListeventcodes
      x-api-path-slug: listeventcodes-get
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
      - Event
      - Codes
  /GetEventDetails:
    get:
      summary: Get Event Details
      description: Get the details for the specified event.
      operationId: postGeteventdetails
      x-api-path-slug: geteventdetails-get
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
      - Event
      - Details
  /GetMultipleEventDetails:
    get:
      summary: Get Multiple Event Details
      description: Get the details for the specified events.
      operationId: postGetmultipleeventdetails
      x-api-path-slug: getmultipleeventdetails-get
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
      - Multiple
      - Event
      - Details
  /GetEventsByCountryCode:
    get:
      summary: Get Events By Country Code
      description: Get events based on the country code and optionally within a specified
        released range.
      operationId: postGeteventsbycountrycode
      x-api-path-slug: geteventsbycountrycode-get
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
      - Events
      - Country
      - Code
  /GetMostRecentEventsByEventCode:
    get:
      summary: Get Most Recent Events By Event Code
      description: Get the most recent events based on the event code and count.
      operationId: postGetmostrecenteventsbyeventcode
      x-api-path-slug: getmostrecenteventsbyeventcode-get
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
      - Most
      - Recent
      - Events
      - Event
      - Code
  /GetEventsByEventCode:
    get:
      summary: Get Events By Event Code
      description: Get events based on the event code and optionally within a specified
        released range.
      operationId: postGeteventsbyeventcode
      x-api-path-slug: geteventsbyeventcode-get
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
      - Events
      - Event
      - Code
  /GetEventsByEventName:
    get:
      summary: Get Events By Event Name
      description: Get events based on the event name and optionally within a specified
        released range.
      operationId: postGeteventsbyeventname
      x-api-path-slug: geteventsbyeventname-get
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
      - Events
      - Event
      - Name
  /GetEventsForDate:
    get:
      summary: Get Events For Date
      description: Get events for the specified date.
      operationId: postGeteventsfordate
      x-api-path-slug: geteventsfordate-get
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
      - Events
      - Date
  /GetEventsForMonth:
    get:
      summary: Get Events For Month
      description: Get events for the specified date.
      operationId: postGeteventsformonth
      x-api-path-slug: geteventsformonth-get
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
      - Events
      - Month
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