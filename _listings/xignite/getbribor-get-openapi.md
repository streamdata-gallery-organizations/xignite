---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Interbanks Get BRIBOR
  description: Returns a BRIBOR as of a date
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
  /GetBars:
    get:
      summary: Get Bars
      description: Get intraday bars of specified intervals within a time range.
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
      description: Get intraday bar at given time.
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
      description: Get chart bars
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
      description: This operation returns symbols in this exchange.
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
  /GetEventsForRange:
    get:
      summary: Get Events For Range
      description: Get events for the specified range.
      operationId: postGeteventsforrange
      x-api-path-slug: geteventsforrange-get
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
      - Range
  /GetEventsForRangeLength:
    get:
      summary: Get Events For Range Length
      description: Get events for the date specified and next number of days past
        it.
      operationId: postGeteventsforrangelength
      x-api-path-slug: geteventsforrangelength-get
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
      - Range
      - Length
  /GetEventsForToday:
    get:
      summary: Get Events For Today
      description: Get all the events released today.
      operationId: postGeteventsfortoday
      x-api-path-slug: geteventsfortoday-get
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
      - Today
  /GetEventsForTomorrow:
    get:
      summary: Get Events For Tomorrow
      description: Get all the events released tomorrow.
      operationId: postGeteventsfortomorrow
      x-api-path-slug: geteventsfortomorrow-get
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
      - Tomorrow
  /GetEventsReleasedForRange:
    get:
      summary: Get Events Released For Range
      description: Get events released for the specified range.
      operationId: postGeteventsreleasedforrange
      x-api-path-slug: geteventsreleasedforrange-get
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
      - Released
      - Range
  /GetEventsReleasedForRangeLength:
    get:
      summary: Get Events Released For Range Length
      description: Get events released for the date specified and next number of days
        past it.
      operationId: postGeteventsreleasedforrangelength
      x-api-path-slug: geteventsreleasedforrangelength-get
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
      - Released
      - Range
      - Length
  /SearchEvents:
    get:
      summary: Search Events
      description: Perform a complex query on events.
      operationId: postSearchevents
      x-api-path-slug: searchevents-get
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
      - Events
  /GetLatestUpdateTimeStamp:
    get:
      summary: Get Latest Update Time Stamp
      description: Get latest update TimeStamp for this service.
      operationId: postGetlatestupdatetimestamp
      x-api-path-slug: getlatestupdatetimestamp-get
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
      - Latest
      - ""
      - Time
      - Stamp
  /GetServiceDemonstration:
    get:
      summary: Get Service Demonstration
      description: Get demonstration for this service.
      operationId: postGetservicedemonstration
      x-api-path-slug: getservicedemonstration-get
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
      - Service
      - Demonstration
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
  /ListActiveCurrencies:
    get:
      summary: List Active Currencies
      description: List supported currencies.
      operationId: postListactivecurrencies
      x-api-path-slug: listactivecurrencies-get
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
      - Active
      - Currencies
  /ListOfficialRates:
    get:
      summary: List Official Rates
      description: List supported official rates.
      operationId: postListofficialrates
      x-api-path-slug: listofficialrates-get
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
      - Official
      - Rates
  /GetUnitOfAccount:
    get:
      summary: Get Unit Of Account
      description: Get Unit Of Account.
      operationId: postGetunitofaccount
      x-api-path-slug: getunitofaccount-get
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
      - Unit
      - Of
      - Account
  /ConvertRealTimeValue:
    get:
      summary: Convert Real Time Value
      description: Convert value from one currency to another in real-time.
      operationId: postConvertrealtimevalue
      x-api-path-slug: convertrealtimevalue-get
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
      - Convert
      - Real
      - Time
      - Value
  /ConvertHistoricalValue:
    get:
      summary: Convert Historical Value
      description: Convert value from one currency to another as of a historical date.
      operationId: postConverthistoricalvalue
      x-api-path-slug: converthistoricalvalue-get
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
      - Convert
      - Historical
      - Value
  /GetRealTimeForwardRate:
    get:
      summary: Get Real Time Forward Rate
      description: Returns a set of real-time currency forward rates.
      operationId: postGetrealtimeforwardrate
      x-api-path-slug: getrealtimeforwardrate-get
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
      - Time
      - Forward
      - Rate
  /GetRealTimeCrossRateAsString:
    get:
      summary: Get Real Time Cross Rate As String
      description: Returns a real-time currency cross-rate.
      operationId: postGetrealtimecrossrateasstring
      x-api-path-slug: getrealtimecrossrateasstring-get
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
      - Time
      - Cross
      - Rate
      - As
      - String
  /GetLatestCrossRate:
    get:
      summary: Get Latest Cross Rate
      description: Returns the latest possible cross rate.
      operationId: postGetlatestcrossrate
      x-api-path-slug: getlatestcrossrate-get
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
      - Latest
      - Cross
      - Rate
  /GetLatestCrossRates:
    get:
      summary: Get Latest Cross Rates
      description: Returns the latest possible cross rate.
      operationId: postGetlatestcrossrates
      x-api-path-slug: getlatestcrossrates-get
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
      - Latest
      - Cross
      - Rates
  /GetRealTimeCrossRate:
    get:
      summary: Get Real Time Cross Rate
      description: Returns a real-time currency cross-rate.
      operationId: postGetrealtimecrossrate
      x-api-path-slug: getrealtimecrossrate-get
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
      - Time
      - Cross
      - Rate
  /GetRealTimeCrossRateGMT:
    get:
      summary: Get Real Time Cross Rate G M T
      description: Returns a real-time currency cross-rate with the times in GMT.
      operationId: postGetrealtimecrossrategmt
      x-api-path-slug: getrealtimecrossrategmt-get
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
      - Time
      - Cross
      - Rate
      - G
      - M
      - T
  /GetRawCrossRate:
    get:
      summary: Get Raw Cross Rate
      description: Returns a real-time currency cross-rate.
      operationId: postGetrawcrossrate
      x-api-path-slug: getrawcrossrate-get
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
      - Raw
      - Cross
      - Rate
  /GetRawCrossRates:
    get:
      summary: Get Raw Cross Rates
      description: Returns a real-time currency cross-rate.
      operationId: postGetrawcrossrates
      x-api-path-slug: getrawcrossrates-get
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
      - Raw
      - Cross
      - Rates
  /GetRealTimeCrossRates:
    get:
      summary: Get Real Time Cross Rates
      description: Returns the latest possible cross rate.
      operationId: postGetrealtimecrossrates
      x-api-path-slug: getrealtimecrossrates-get
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
      - Time
      - Cross
      - Rates
  /GetHistoricalCrossRateTables:
    get:
      summary: Get Historical Cross Rate Tables
      description: Returns historical currency cross-rate tables for a range of dates.
      operationId: postGethistoricalcrossratetables
      x-api-path-slug: gethistoricalcrossratetables-get
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
      - Cross
      - Rate
      - Tables
  /GetHistoricalCrossRateTablesBidAsk:
    get:
      summary: Get Historical Cross Rate Tables Bid Ask
      description: Returns historical currency cross-rate tables for a range of dates.
      operationId: postGethistoricalcrossratetablesbask
      x-api-path-slug: gethistoricalcrossratetablesbidask-get
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
      - Cross
      - Rate
      - Tables
      - Bid
      - Ask
  /GetCurrencyReport:
    get:
      summary: Get Currency Report
      description: Returns historical currency cross-rate tables for a range of dates.
      operationId: postGetcurrencyreport
      x-api-path-slug: getcurrencyreport-get
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
      - Currency
      - Report
  /GetHistoricalCrossRateTable:
    get:
      summary: Get Historical Cross Rate Table
      description: Returns a historical currency cross-rate table.
      operationId: postGethistoricalcrossratetable
      x-api-path-slug: gethistoricalcrossratetable-get
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
      - Cross
      - Rate
      - Table
  /GetHistoricalCrossRateTableBidAsk:
    get:
      summary: Get Historical Cross Rate Table Bid Ask
      description: Returns a historical currency cross-rate table.
      operationId: postGethistoricalcrossratetablebask
      x-api-path-slug: gethistoricalcrossratetablebidask-get
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
      - Cross
      - Rate
      - Table
      - Bid
      - Ask
  /GetRealTimeCrossRateTable:
    get:
      summary: Get Real Time Cross Rate Table
      description: Returns a real-time currency cross-rate table.
      operationId: postGetrealtimecrossratetable
      x-api-path-slug: getrealtimecrossratetable-get
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
      - Time
      - Cross
      - Rate
      - Table
  /GetRealTimeCrossRateTableWithBidAsk:
    get:
      summary: Get Real Time Cross Rate Table With Bid Ask
      description: Returns a real-time currency cross-rate table.
      operationId: postGetrealtimecrossratetablewithbask
      x-api-path-slug: getrealtimecrossratetablewithbidask-get
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
      - Time
      - Cross
      - Rate
      - Table
      - With
      - Bid
      - Ask
  /GetAllCrossRatesForACurrency:
    get:
      summary: Get All Cross Rates For A Currency
      description: Returns all valid cross rates for a currency.
      operationId: postGetallcrossratesforacurrency
      x-api-path-slug: getallcrossratesforacurrency-get
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
      - Cross
      - Rates
      - Currency
  /GetRealTimeCrossRateTableAsHTML:
    get:
      summary: Get Real Time Cross Rate Table As H T M L
      description: Returns a real-time currency cross-rate table as an HTML Output.
      operationId: postGetrealtimecrossratetableashtml
      x-api-path-slug: getrealtimecrossratetableashtml-get
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
      - Time
      - Cross
      - Rate
      - Table
      - As
      - H
      - T
      - M
      - L
  /GetSimpleRealTimeCrossRateTableAsHTML:
    get:
      summary: Get Simple Real Time Cross Rate Table As H T M L
      description: Returns a real-time currency cross-rate table as an HTML Output.
      operationId: postGetsimplerealtimecrossratetableashtml
      x-api-path-slug: getsimplerealtimecrossratetableashtml-get
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
      - Simple
      - Real
      - Time
      - Cross
      - Rate
      - Table
      - As
      - H
      - T
      - M
      - L
  /GetHistoricalCrossRateTableAsHTML:
    get:
      summary: Get Historical Cross Rate Table As H T M L
      description: Returns a historical currency cross-rate table as an HTML Output.
      operationId: postGethistoricalcrossratetableashtml
      x-api-path-slug: gethistoricalcrossratetableashtml-get
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
      - Cross
      - Rate
      - Table
      - As
      - H
      - T
      - M
      - L
  /GetHistoricalCrossRate:
    get:
      summary: Get Historical Cross Rate
      description: Returns a cross-rate as of a historical date.
      operationId: postGethistoricalcrossrate
      x-api-path-slug: gethistoricalcrossrate-get
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
      - Cross
      - Rate
  /GetHistoricalCrossRates:
    get:
      summary: Get Historical Cross Rates
      description: Returns multiple cross-rates as of a historical date.
      operationId: postGethistoricalcrossrates
      x-api-path-slug: gethistoricalcrossrates-get
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
      - Cross
      - Rates
  /GetHistoricalCrossRateBidAsk:
    get:
      summary: Get Historical Cross Rate Bid Ask
      description: Returns a cross-rate with bid/ask as of a historical date.
      operationId: postGethistoricalcrossratebask
      x-api-path-slug: gethistoricalcrossratebidask-get
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
      - Cross
      - Rate
      - Bid
      - Ask
  /GetHistoricalCrossRatesBidAsk:
    get:
      summary: Get Historical Cross Rates Bid Ask
      description: Returns multiple cross-rates with bid/ask as of a historical date.
      operationId: postGethistoricalcrossratesbask
      x-api-path-slug: gethistoricalcrossratesbidask-get
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
      - Cross
      - Rates
      - Bid
      - Ask
  /GetHistoricalCrossRatesRange:
    get:
      summary: Get Historical Cross Rates Range
      description: This operation returns a range of cross-rates for a currency pair.
      operationId: postGethistoricalcrossratesrange
      x-api-path-slug: gethistoricalcrossratesrange-get
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
      - Cross
      - Rates
      - Range
  /GetHistoricalCrossRatesBidAskRange:
    get:
      summary: Get Historical Cross Rates Bid Ask Range
      description: This operation returns a range of cross-rates for a currency pair.
      operationId: postGethistoricalcrossratesbaskrange
      x-api-path-slug: gethistoricalcrossratesbidaskrange-get
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
      - Cross
      - Rates
      - Bid
      - Ask
      - Range
  /GetHistoricalCrossRatesAsOf:
    get:
      summary: Get Historical Cross Rates As Of
      description: This operation returns a range of cross-rates for a currency pair.
      operationId: postGethistoricalcrossratesasof
      x-api-path-slug: gethistoricalcrossratesasof-get
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
      - Cross
      - Rates
      - As
      - Of
  /GetHistoricalCrossRatesBidAskAsOf:
    get:
      summary: Get Historical Cross Rates Bid Ask As Of
      description: This operation returns a range of cross-rates for a currency pair.
      operationId: postGethistoricalcrossratesbaskasof
      x-api-path-slug: gethistoricalcrossratesbidaskasof-get
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
      - Cross
      - Rates
      - Bid
      - Ask
      - As
      - Of
  /GetOfficialCrossRate:
    get:
      summary: Get Official Cross Rate
      description: Returns an official cross-rate as of a historical date.
      operationId: postGetofficialcrossrate
      x-api-path-slug: getofficialcrossrate-get
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
      - Official
      - Cross
      - Rate
  /GetOfficialCrossRates:
    get:
      summary: Get Official Cross Rates
      description: Returns an official cross-rate as of a historical date.
      operationId: postGetofficialcrossrates
      x-api-path-slug: getofficialcrossrates-get
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
      - Official
      - Cross
      - Rates
  /GetOfficialCrossRateBidAsk:
    get:
      summary: Get Official Cross Rate Bid Ask
      description: Returns an official cross-rate as of a historical date.
      operationId: postGetofficialcrossratebask
      x-api-path-slug: getofficialcrossratebidask-get
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
      - Official
      - Cross
      - Rate
      - Bid
      - Ask
  /GetOfficialCrossRatesBidAsk:
    get:
      summary: Get Official Cross Rates Bid Ask
      description: Returns an official cross-rate as of a historical date.
      operationId: postGetofficialcrossratesbask
      x-api-path-slug: getofficialcrossratesbidask-get
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
      - Official
      - Cross
      - Rates
      - Bid
      - Ask
  /GetMutipleHistoricalCrossRates:
    get:
      summary: Get Mutiple Historical Cross Rates
      description: Returns multiple cross-rates as of a historical date.
      operationId: postGetmutiplehistoricalcrossrates
      x-api-path-slug: getmutiplehistoricalcrossrates-get
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
      - Mutiple
      - Historical
      - Cross
      - Rates
  /GetAverageHistoricalCrossRates:
    get:
      summary: Get Average Historical Cross Rates
      description: This operation returns an array average daily historical cross-rates
        for a period.
      operationId: postGetaveragehistoricalcrossrates
      x-api-path-slug: getaveragehistoricalcrossrates-get
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
      - Average
      - Historical
      - Cross
      - Rates
  /GetAverageHistoricalCrossRate:
    get:
      summary: Get Average Historical Cross Rate
      description: This operation returns an average daily historical cross-rates
        for a period.
      operationId: postGetaveragehistoricalcrossrate
      x-api-path-slug: getaveragehistoricalcrossrate-get
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
      - Average
      - Historical
      - Cross
      - Rate
  /GetHistoricalMonthlyCrossRatesRange:
    get:
      summary: Get Historical Monthly Cross Rates Range
      description: This operation returns a complete range of stock quotes for a currency
        pair.
      operationId: postGethistoricalmonthlycrossratesrange
      x-api-path-slug: gethistoricalmonthlycrossratesrange-get
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
      - Cross
      - Rates
      - Range
  /GetCrossRateChange:
    get:
      summary: Get Cross Rate Change
      description: This operation returns the changes in a cross-rates over the last
        6 months.
      operationId: postGetcrossratechange
      x-api-path-slug: getcrossratechange-get
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
      - Cross
      - Rate
      - Change
  Currency, , Custom:
    get:
      summary: Get Currency Chart Custom
      description: Draw a custom currency chart for a date range.
      operationId: postGetcurrencychartcustom
      x-api-path-slug: currency--custom-get
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
      - Currency
      - Chart
      - Custom
  Currency, , Custom, Binary:
    get:
      summary: Get Currency Chart Custom Binary
      description: Draw a custom currency chart for a date range.
      operationId: postGetcurrencychartcustombinary
      x-api-path-slug: currency--custom-binary-get
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
      - Currency
      - Chart
      - Custom
      - Binary
  'Currency, ':
    get:
      summary: Get Currency Chart
      description: Draw a historical currency chart for a date range.
      operationId: postGetcurrencychart
      x-api-path-slug: currency-get
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
      - Currency
      - Chart
  Currency, , Binary:
    get:
      summary: Get Currency Chart Binary
      description: Draw a historical currency chart for a date range in binary format.
      operationId: postGetcurrencychartbinary
      x-api-path-slug: currency--binary-get
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
      - Currency
      - Chart
      - Binary
  'Currency, Intraday, ':
    get:
      summary: Get Currency Intraday Chart
      description: Draw a intraday currency chart for a time range
      operationId: postGetcurrencyintradaychart
      x-api-path-slug: currency-intraday-get
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
      - Currency
      - Intraday
      - Chart
  Currency, Intraday, , Custom, Binary:
    get:
      summary: Get Currency Intraday Chart Custom Binary
      description: Draw a intraday currency chart for a time range in a binary format
      operationId: postGetcurrencyintradaychartcustombinary
      x-api-path-slug: currency-intraday--custom-binary-get
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
      - Currency
      - Intraday
      - Chart
      - Custom
      - Binary
  Currency, Intraday, , Custom:
    get:
      summary: Get Currency Intraday Chart Custom
      description: Draw a intraday currency chart for a time range in a binary format
      operationId: postGetcurrencyintradaychartcustom
      x-api-path-slug: currency-intraday--custom-get
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
      - Currency
      - Intraday
      - Chart
      - Custom
  ', Design':
    get:
      summary: Get Chart Design
      description: Returns the default design class for the currency Chart.
      operationId: postGetchartdesign
      x-api-path-slug: design-get
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
      - Design
  /GetTick:
    get:
      summary: Get Tick
      description: Get intraday tick at given time.
      operationId: GetTick
      x-api-path-slug: gettick-get
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
      - Tick
  /GetTicks:
    get:
      summary: Get Ticks
      description: Get intraday ticks of specified intervals within a time range.
      operationId: GetTicks
      x-api-path-slug: getticks-get
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
      - Ticks
  /GetHistoricalTicks:
    get:
      summary: Get Historical Ticks
      description: Returns a historical range of ticks for a security.
      operationId: postGethistoricalticks
      x-api-path-slug: gethistoricalticks-get
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
      - Ticks
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
  /GetIntradayHighLow:
    get:
      summary: Get Intraday High Low
      description: Returns the high and the low ticks for today.
      operationId: postGetintradayhighlow
      x-api-path-slug: getintradayhighlow-get
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
      - Intraday
      - High
      - Low
  /GetEstimates:
    get:
      summary: Get Estimates
      description: Get Estimates on AsOfDate
      operationId: GetEstimates
      x-api-path-slug: getestimates-get
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
      - Estimates
  /GetLatestRecommendationSummaries:
    get:
      summary: Get Latest Recommendation Summaries
      description: Get Latest Recommendation Summary
      operationId: GetLatestRecommendationSummaries
      x-api-path-slug: getlatestrecommendationsummaries-get
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
      - Latest
      - Recommendation
      - Summaries
  /ListExchanges:
    get:
      summary: List Exchanges
      description: List supported exchanges.
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
  /ListCompanies:
    get:
      summary: List Companies
      description: List Symbols
      operationId: ListCompanies
      x-api-path-slug: listcompanies-get
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
      - Companies
  /ListEstimates:
    get:
      summary: List Estimates
      description: List Estimates
      operationId: ListEstimates
      x-api-path-slug: listestimates-get
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
      - Estimates
  /GetLatestEstimates:
    get:
      summary: Get Latest Estimates
      description: Get Latest Estimates
      operationId: GetLatestEstimates
      x-api-path-slug: getlatestestimates-get
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
      - Latest
      - Estimates
  /GetEstimatesRange:
    get:
      summary: Get Estimates Range
      description: Get Estimates Range
      operationId: GetEstimatesRange
      x-api-path-slug: getestimatesrange-get
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
      - Estimates
      - Range
  /GetRecommendationSummaryRange:
    get:
      summary: Get Recommendation Summary Range
      description: Get Recommendation Summaries in Range
      operationId: GetRecommendationSummaryRange
      x-api-path-slug: getrecommendationsummaryrange-get
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
      - Recommendation
      - Summary
      - Range
  /GetRecommendationSummaries:
    get:
      summary: Get Recommendation Summaries
      description: Get Recommendation Summaries on AsOfDate
      operationId: GetRecommendationSummaries
      x-api-path-slug: getrecommendationsummaries-get
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
      - Recommendation
      - Summaries
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
  /GetNextFuture:
    get:
      summary: Get Next Future
      description: Get the next immediate future contract for a commodity.
      operationId: postGetnextfuture
      x-api-path-slug: getnextfuture-get
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
      - Next
      - Future
  /GetFuture:
    get:
      summary: Get Future
      description: Returns master data on a future contract
      operationId: GetFuture
      x-api-path-slug: getfuture-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Future
  /ListFutureCategories:
    get:
      summary: List Future Categories
      description: List commmodities future categories.
      operationId: postListfuturecategories
      x-api-path-slug: listfuturecategories-get
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
      - Future
      - Categories
  /ListSwaps:
    get:
      summary: List Swaps
      description: List all commodity swaps and the exchange on which they are traded.
      operationId: postListswaps
      x-api-path-slug: listswaps-get
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
      - Swaps
  /ListFutures:
    get:
      summary: List Futures
      description: List all commodity futures and the exchange on which they are traded.
      operationId: postListfutures
      x-api-path-slug: listfutures-get
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
      - Futures
  /ListFrontMonthContracts:
    get:
      summary: List Front Month Contracts
      description: List all commodity future Front Month Contracts.
      operationId: postListfrontmonthcontracts
      x-api-path-slug: listfrontmonthcontracts-get
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
      - Front
      - Month
      - Contracts
  /ListFuturesByCategory:
    get:
      summary: List Futures By Category
      description: List futures information by byfuture category.
      operationId: postListfuturesbycategory
      x-api-path-slug: listfuturesbycategory-get
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
      - Futures
      - By
      - Category
  /ListFuturesByExchange:
    get:
      summary: List Futures By Exchange
      description: List futures information by exchange.
      operationId: postListfuturesbyexchange
      x-api-path-slug: listfuturesbyexchange-get
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
      - Futures
      - By
      - Exchange
  /ListSwapsByExchange:
    get:
      summary: List Swaps By Exchange
      description: List swaps information by exchange.
      operationId: postListswapsbyexchange
      x-api-path-slug: listswapsbyexchange-get
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
      - Swaps
      - By
      - Exchange
  /GetDelayedSwap:
    get:
      summary: Get Delayed Swap
      description: Returns a delayed quote for a NYMEX swap contract.
      operationId: postGetdelayedswap
      x-api-path-slug: getdelayedswap-get
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
      - Delayed
      - Swap
  /GetDelayedFuture:
    get:
      summary: Get Delayed Future
      description: Returns a delayed quote for a future contract.
      operationId: postGetdelayedfuture
      x-api-path-slug: getdelayedfuture-get
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
      - Delayed
      - Future
  /GetDelayedFrontFuture:
    get:
      summary: Get Delayed Front Future
      description: Returns a delayed quote for a future contract.
      operationId: postGetdelayedfrontfuture
      x-api-path-slug: getdelayedfrontfuture-get
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
      - Delayed
      - Front
      - Future
  /GetAllDelayedFutures:
    get:
      summary: Get All Delayed Futures
      description: Returns delayed quotes for all contracts for a commodity.
      operationId: postGetalldelayedfutures
      x-api-path-slug: getalldelayedfutures-get
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
      - Delayed
      - Futures
  /GetTopDelayedFutures:
    get:
      summary: Get Top Delayed Futures
      description: Returns delayed quotes for a given number of contract (front-future
        first) for a commodity.
      operationId: postGettopdelayedfutures
      x-api-path-slug: gettopdelayedfutures-get
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
      - Delayed
      - Futures
  /GetAllDelayedSwaps:
    get:
      summary: Get All Delayed Swaps
      description: Returns delayed quotes for all contracts for a commodity.
      operationId: postGetalldelayedswaps
      x-api-path-slug: getalldelayedswaps-get
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
      - Delayed
      - Swaps
  /GetDelayedFutures:
    get:
      summary: Get Delayed Futures
      description: Returns delayed quotes for multiple future contracts.
      operationId: postGetdelayedfutures
      x-api-path-slug: getdelayedfutures-get
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
      - Delayed
      - Futures
  /GetDelayedFutureStrip:
    get:
      summary: Get Delayed Future Strip
      description: Returns a delayed future strip for a commodity.
      operationId: postGetdelayedfuturestrip
      x-api-path-slug: getdelayedfuturestrip-get
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
      - Delayed
      - Future
      - Strip
  /GetHistoricalFutureStrip:
    get:
      summary: Get Historical Future Strip
      description: Returns a future strip for a commodity.
      operationId: postGethistoricalfuturestrip
      x-api-path-slug: gethistoricalfuturestrip-get
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
      - Future
      - Strip
  /GetHistoricalSwapStrip:
    get:
      summary: Get Historical Swap Strip
      description: Returns a future strip for a commodity.
      operationId: postGethistoricalswapstrip
      x-api-path-slug: gethistoricalswapstrip-get
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
      - Swap
      - Strip
  /GetDelayedSpot:
    get:
      summary: Get Delayed Spot
      description: Returns a delayed spot quote for a commodity.
      operationId: postGetdelayedspot
      x-api-path-slug: getdelayedspot-get
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
      - Delayed
      - Spot
  /GetDelayedSpots:
    get:
      summary: Get Delayed Spots
      description: Returns delayed quotes for multiple commodities.
      operationId: postGetdelayedspots
      x-api-path-slug: getdelayedspots-get
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
      - Delayed
      - Spots
  /GetDelayedFutureBySession:
    get:
      summary: Get Delayed Future By Session
      description: Returns a delayed quote for a future contract by exchange session.
      operationId: postGetdelayedfuturebysession
      x-api-path-slug: getdelayedfuturebysession-get
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
      - Delayed
      - Future
      - By
      - Session
  /GetAllDelayedFuturesBySession:
    get:
      summary: Get All Delayed Futures By Session
      description: Returns delayed quotes for all contracts for a commodity by exchange
        session.
      operationId: postGetalldelayedfuturesbysession
      x-api-path-slug: getalldelayedfuturesbysession-get
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
      - Delayed
      - Futures
      - By
      - Session
  /GetDelayedFuturesBySession:
    get:
      summary: Get Delayed Futures By Session
      description: Returns delayed quotes for multiple future contracts by exchange
        session.
      operationId: postGetdelayedfuturesbysession
      x-api-path-slug: getdelayedfuturesbysession-get
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
      - Delayed
      - Futures
      - By
      - Session
  /GetHistoricalFuture:
    get:
      summary: Get Historical Future
      description: Returns a historical quote for a future contract.
      operationId: postGethistoricalfuture
      x-api-path-slug: gethistoricalfuture-get
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
      - Future
  /GetHistoricalFutures:
    get:
      summary: Get Historical Futures
      description: Returns historical quotes for multiple future contracts.
      operationId: postGethistoricalfutures
      x-api-path-slug: gethistoricalfutures-get
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
      - Futures
  /GetAllHistoricalFuturesWithStatus:
    get:
      summary: Get All Historical Futures With Status
      description: Returns historical quotes for all contracts for a commodity as
        of a specific date including status information.
      operationId: postGetallhistoricalfutureswithstatus
      x-api-path-slug: getallhistoricalfutureswithstatus-get
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
      - Futures
      - With
      - Status
  /GetAllHistoricalFutures:
    get:
      summary: Get All Historical Futures
      description: Returns historical quotes for all contracts for a commodity as
        of a specific date.
      operationId: postGetallhistoricalfutures
      x-api-path-slug: getallhistoricalfutures-get
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
      - Futures
  /GetHistoricalFutureRange:
    get:
      summary: Get Historical Future Range
      description: Returns a range of historical quotes for a future contract.
      operationId: postGethistoricalfuturerange
      x-api-path-slug: gethistoricalfuturerange-get
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
      - Future
      - Range
  /GetHistoricalSwap:
    get:
      summary: Get Historical Swap
      description: Returns a historical quote for a future swap.
      operationId: postGethistoricalswap
      x-api-path-slug: gethistoricalswap-get
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
      - Swap
  /GetHistoricalSwapRange:
    get:
      summary: Get Historical Swap Range
      description: Returns a range of historical quotes for a future swap.
      operationId: postGethistoricalswaprange
      x-api-path-slug: gethistoricalswaprange-get
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
      - Swap
      - Range
  /GetHistoricalSwaps:
    get:
      summary: Get Historical Swaps
      description: Returns historical quotes for multiple future swaps.
      operationId: postGethistoricalswaps
      x-api-path-slug: gethistoricalswaps-get
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
      - Swaps
  /GetAllHistoricalSwaps:
    get:
      summary: Get All Historical Swaps
      description: Returns historical quotes for all contracts for a commodity swap
        as of a specific date.
      operationId: postGetallhistoricalswaps
      x-api-path-slug: getallhistoricalswaps-get
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
      - Swaps
  /GetHistoricalCommodityRange:
    get:
      summary: Get Historical Commodity Range
      description: Returns a range of historical quotes for a future contract.
      operationId: postGethistoricalcommodityrange
      x-api-path-slug: gethistoricalcommodityrange-get
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
      - Commodity
      - Range
  /GetHistoricalCommodityMonthlyRange:
    get:
      summary: Get Historical Commodity Monthly Range
      description: Returns a range of historical quotes for a future contract.
      operationId: postGethistoricalcommoditymonthlyrange
      x-api-path-slug: gethistoricalcommoditymonthlyrange-get
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
      - Commodity
      - Monthly
      - Range
  /GetHistoricalSpotRange:
    get:
      summary: Get Historical Spot Range
      description: Returns a range of commodity spot prices for a commodity.
      operationId: postGethistoricalspotrange
      x-api-path-slug: gethistoricalspotrange-get
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
      - Spot
      - Range
  /GetHistoricalSpotMonthlyRange:
    get:
      summary: Get Historical Spot Monthly Range
      description: Returns a range of commodity spot prices for a commodity.
      operationId: postGethistoricalspotmonthlyrange
      x-api-path-slug: gethistoricalspotmonthlyrange-get
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
      - Spot
      - Monthly
      - Range
  /GetHistoricalTicksAsOfDate:
    get:
      summary: Get Historical Ticks As Of Date
      description: Returns a historical range of ticks for a security.
      operationId: postGethistoricalticksasofdate
      x-api-path-slug: gethistoricalticksasofdate-get
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
      - Ticks
      - As
      - Of
      - Date
  'Intraday, Future, ':
    get:
      summary: Get Intraday Future Chart
      description: Get a standard intraday price chart for a future contract.
      operationId: postGetintradayfuturechart
      x-api-path-slug: intraday-future-get
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
      - Intraday
      - Future
      - Chart
  Intraday, Future, , Binary:
    get:
      summary: Get Intraday Future Chart Binary
      description: Get a standard intraday price chart for a future contract in binary
        format.
      operationId: postGetintradayfuturechartbinary
      x-api-path-slug: intraday-future--binary-get
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
      - Intraday
      - Future
      - Chart
      - Binary
  Intraday, Future, , Custom:
    get:
      summary: Get Intraday Future Chart Custom
      description: Get a custom intraday price chart for a future contract.
      operationId: postGetintradayfuturechartcustom
      x-api-path-slug: intraday-future--custom-get
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
      - Intraday
      - Future
      - Chart
      - Custom
  Intraday, Future, , Custom, Binary:
    get:
      summary: Get Intraday Future Chart Custom Binary
      description: Get a custom intraday price chart for a future contract in binary
        format.
      operationId: postGetintradayfuturechartcustombinary
      x-api-path-slug: intraday-future--custom-binary-get
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
      - Intraday
      - Future
      - Chart
      - Custom
      - Binary
  'Historical, Future, ':
    get:
      summary: Get Historical Future Chart
      description: Get a standard historical price chart for a future contract.
      operationId: postGethistoricalfuturechart
      x-api-path-slug: historical-future-get
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
      - Future
      - Chart
  Historical, Future, , Binary:
    get:
      summary: Get Historical Future Chart Binary
      description: Get a standard historical price chart for a future contract in
        binary format.
      operationId: postGethistoricalfuturechartbinary
      x-api-path-slug: historical-future--binary-get
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
      - Future
      - Chart
      - Binary
  Historical, Future, , Custom:
    get:
      summary: Get Historical Future Chart Custom
      description: Get a custom historical chart for a future contract in binary format.
      operationId: postGethistoricalfuturechartcustom
      x-api-path-slug: historical-future--custom-get
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
      - Future
      - Chart
      - Custom
  Historical, Future, , Custom, Binary:
    get:
      summary: Get Historical Future Chart Custom Binary
      description: Draw a custom historical chart for a future contract.
      operationId: postGethistoricalfuturechartcustombinary
      x-api-path-slug: historical-future--custom-binary-get
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
      - Future
      - Chart
      - Custom
      - Binary
  'Historical, Commodity, ':
    get:
      summary: Get Historical Commodity Chart
      description: Get a historical chart for a commodity.
      operationId: postGethistoricalcommoditychart
      x-api-path-slug: historical-commodity-get
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
      - Commodity
      - Chart
  Historical, Commodity, , Binary:
    get:
      summary: Get Historical Commodity Chart Binary
      description: Get a historical chart for a commodity in binary format.
      operationId: postGethistoricalcommoditychartbinary
      x-api-path-slug: historical-commodity--binary-get
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
      - Commodity
      - Chart
      - Binary
  Historical, Commodity, , Custom:
    get:
      summary: Get Historical Commodity Chart Custom
      description: Get a custom historical chart for a commodity in binary format.
      operationId: postGethistoricalcommoditychartcustom
      x-api-path-slug: historical-commodity--custom-get
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
      - Commodity
      - Chart
      - Custom
  Historical, Commodity, , Custom, Binary:
    get:
      summary: Get Historical Commodity Chart Custom Binary
      description: Draw a custom historical chart for a future contract.
      operationId: postGethistoricalcommoditychartcustombinary
      x-api-path-slug: historical-commodity--custom-binary-get
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
      - Commodity
      - Chart
      - Custom
      - Binary
  Intraday, , Design:
    get:
      summary: Get Intraday Chart Design
      description: Returns the default settings for the intraday future chart.
      operationId: postGetintradaychartdesign
      x-api-path-slug: intraday--design-get
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
      - Intraday
      - Chart
      - Design
  Historical, , Design:
    get:
      summary: Get Historical Chart Design
      description: Returns the default settings for the historical future chart.
      operationId: postGethistoricalchartdesign
      x-api-path-slug: historical--design-get
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
      - Chart
      - Design
  /GetFutureOption:
    get:
      summary: Get Future Option
      description: Returns a specific future option.
      operationId: postGetfutureoption
      x-api-path-slug: getfutureoption-get
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
      - Option
  /GetTopIndustryHeadlines:
    get:
      summary: Get Top Industry Headlines
      description: Get top industry headlines.
      operationId: GetTopIndustryHeadlines
      x-api-path-slug: gettopindustryheadlines-get
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
      - Industry
      - Headlines
  /GetTodaysIndustryHeadlines:
    get:
      summary: Get Todays Industry Headlines
      description: Return press releases for today for an industry.
      operationId: postGettodaysindustryheadlines
      x-api-path-slug: gettodaysindustryheadlines-get
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
      - Todays
      - Industry
      - Headlines
  /GetLastIndustryHeadlines:
    get:
      summary: Get Last Industry Headlines
      description: Return the last press releases since a certain time for an industry.
      operationId: postGetlastindustryheadlines
      x-api-path-slug: getlastindustryheadlines-get
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
      - Industry
      - Headlines
  /GetFutureOptionChain:
    get:
      summary: Get Future Option Chain
      description: Returns an option chain for a future contract.
      operationId: postGetfutureoptionchain
      x-api-path-slug: getfutureoptionchain-get
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
      - Option
      - Chain
  /GetFutureOptionsByStrikePrice:
    get:
      summary: Get Future Options By Strike Price
      description: Returns an option chain for a future contract matching a list of
        prices.
      operationId: postGetfutureoptionsbystrikeprice
      x-api-path-slug: getfutureoptionsbystrikeprice-get
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
      - Options
      - By
      - Strike
      - Price
  /GetFile:
    get:
      summary: Get File
      description: Get file
      operationId: GetFile
      x-api-path-slug: getfile-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Files
  /GetFrontMonthFuture:
    get:
      summary: Get Front Month Future
      description: Returns master data on the front month future contract
      operationId: GetFrontMonthFuture
      x-api-path-slug: getfrontmonthfuture-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Front
      - Month
      - Future
  /GetFutureQuote:
    get:
      summary: Get Future Quote
      description: Returns a realtime quote for a future contract.
      operationId: GetFutureQuote
      x-api-path-slug: getfuturequote-get
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
      - Quote
  /GetLatestFutureQuote:
    get:
      summary: Get Latest Future Quote
      description: Returns the latest realtime quote for a future contract.
      operationId: GetLatestFutureQuote
      x-api-path-slug: getlatestfuturequote-get
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
      - Latest
      - Future
      - Quote
  /GetFutureQuotes:
    get:
      summary: Get Future Quotes
      description: Returns realtime quotes for multiple future contracts.
      operationId: GetFutureQuotes
      x-api-path-slug: getfuturequotes-get
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
      - Quotes
  /GetLatestFutureQuotes:
    get:
      summary: Get Latest Future Quotes
      description: Returns latest realtime quotes for multiple future contracts.
      operationId: GetLatestFutureQuotes
      x-api-path-slug: getlatestfuturequotes-get
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
      - Latest
      - Future
      - Quotes
  /GetSpotFutureQuote:
    get:
      summary: Get Spot Future Quote
      description: Returns a realtime spot quote for a future contract.
      operationId: GetSpotFutureQuote
      x-api-path-slug: getspotfuturequote-get
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
      - Spot
      - Future
      - Quote
  /GetLatestFrontMonthFutureQuotes:
    get:
      summary: Get Latest Front Month Future Quotes
      description: Returns latest quotes for front month futures
      operationId: GetLatestFrontMonthFutureQuotes
      x-api-path-slug: getlatestfrontmonthfuturequotes-get
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
      - Latest
      - Front
      - Month
      - Future
      - Quotes
  /GetAllFutureQuotes:
    get:
      summary: Get All Future Quotes
      description: Returns all delayed future quotes for a future base.
      operationId: GetAllFutureQuotes
      x-api-path-slug: getallfuturequotes-get
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
      - Quotes
  /GetLMEFutureQuote:
    get:
      summary: Get LME Future Quote
      description: Returns latest quotes for LME futures
      operationId: GetLMEFutureQuote
      x-api-path-slug: getlmefuturequote-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - LME
      - Future
      - Quote
  /GetFutureOptionQuote:
    get:
      summary: Get Future Option Quote
      description: Returns a realtime future option quote for a future option.
      operationId: GetFutureOptionQuote
      x-api-path-slug: getfutureoptionquote-get
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
      - Option
      - Quote
  /GetAllOptionQuotes:
    get:
      summary: Get All Option Quotes
      description: Returns all realtime future option quotes for a future contract.
      operationId: GetAllOptionQuotes
      x-api-path-slug: getalloptionquotes-get
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
      - Option
      - Quotes
  /GetFutureOptionQuotes:
    get:
      summary: Get Future Option Quotes
      description: Returns realtime future option quotes for multiple future options.
      operationId: GetFutureOptionQuotes
      x-api-path-slug: getfutureoptionquotes-get
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
      - Option
      - Quotes
  /GetLatestFutureOptionQuote:
    get:
      summary: Get Latest Future Option Quote
      description: Returns latest realtime quote for multiple future option.
      operationId: GetLatestFutureOptionQuote
      x-api-path-slug: getlatestfutureoptionquote-get
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
      - Latest
      - Future
      - Option
      - Quote
  /GetLatestFutureOptionQuotes:
    get:
      summary: Get Latest Future Option Quotes
      description: Returns latest realtime quotes for multiple future options.
      operationId: GetLatestFutureOptionQuotes
      x-api-path-slug: getlatestfutureoptionquotes-get
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
      - Latest
      - Future
      - Option
      - Quotes
  /ListFutureExchanges:
    get:
      summary: List Future Exchanges
      description: Returns a list of future exchanges
      operationId: ListFutureExchanges
      x-api-path-slug: listfutureexchanges-get
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
      - Future
      - Exchanges
  /ListBaseFutures:
    get:
      summary: List Base Futures
      description: Returns a list of base future symbols
      operationId: ListBaseFutures
      x-api-path-slug: listbasefutures-get
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
      - Base
      - Futures
  /ListFutureChain:
    get:
      summary: List Future Chain
      description: Returns a list of future contracts on a base future symbol
      operationId: ListFutureChain
      x-api-path-slug: listfuturechain-get
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
      - Future
      - Chain
  /ListOptionChain:
    get:
      summary: List Option Chain
      description: Returns a list of options on a future contract
      operationId: ListOptionChain
      x-api-path-slug: listoptionchain-get
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
      - Option
      - Chain
  /SearchFutures:
    get:
      summary: Search Futures
      description: Returns futures match the name
      operationId: SearchFutures
      x-api-path-slug: searchfutures-get
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
      - Futures
  /GetSwapQuote:
    get:
      summary: Get Swap Quote
      description: Returns realtime quote for a swap
      operationId: GetSwapQuote
      x-api-path-slug: getswapquote-get
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
      - Swap
      - Quote
  /GetHistoricalSwapQuotes:
    get:
      summary: Get Historical Swap Quotes
      description: Returns historical swap quotes within a date range
      operationId: GetHistoricalSwapQuotes
      x-api-path-slug: gethistoricalswapquotes-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Swap
      - Quotes
  /GetHistoricalFutureQuotesRange:
    get:
      summary: Get Historical Future Quotes Range
      description: Returns historical future quotes on a future contract within a
        date range
      operationId: GetHistoricalFutureQuotesRange
      x-api-path-slug: gethistoricalfuturequotesrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Future
      - Quotes
      - Range
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
        from NYSE, NASDAQ and AMEX.
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
  /GetAllCorporateActionsByExchange:
    get:
      summary: Get All Corporate Actions By Exchange
      description: Get all corporate actions for a date range in the specified exchange.
      operationId: postGetallcorporateactionsbyexchange
      x-api-path-slug: getallcorporateactionsbyexchange-get
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
      - Corporate
      - Actions
      - By
      - Exchange
  /GetCorporateActionHistory:
    get:
      summary: Get Corporate Action History
      description: Get the corporate action history for a stock for a date range.
      operationId: postGetcorporateactionhistory
      x-api-path-slug: getcorporateactionhistory-get
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
      - Corporate
      - Action
      - History
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
  /GetPriorDate:
    get:
      summary: Get Prior Date
      description: Get prior date.
      operationId: GetPriorDate
      x-api-path-slug: getpriordate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Prior
      - Date
  /GetDayCount:
    get:
      summary: Get Day Count
      description: Get day count.
      operationId: GetDayCount
      x-api-path-slug: getdaycount-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Day
      - Count
  /GetExchangeDateTime:
    get:
      summary: Get Exchange Date Time
      description: Get exchange date time.
      operationId: GetExchangeDateTime
      x-api-path-slug: getexchangedatetime-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Exchange
      - Date
      - Time
  /GetExchangeHours:
    get:
      summary: Get Exchange Hours
      description: Get exchange hours.
      operationId: GetExchangeHours
      x-api-path-slug: getexchangehours-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Exchange
      - Hours
  /GetExchangeHoursRange:
    get:
      summary: Get Exchange Hours Range
      description: Get exchange hours range.
      operationId: GetExchangeHoursRange
      x-api-path-slug: getexchangehoursrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Exchange
      - Hours
      - Range
  /AreExchangesOpen:
    get:
      summary: Are Exchanges Open
      description: Are exchanges open.
      operationId: AreExchangesOpen
      x-api-path-slug: areexchangesopen-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Are
      - Exchanges
      - Open
  /IsExchangeOpenOnDate:
    get:
      summary: Is Exchange Open On Date
      description: Is exchange open on date.
      operationId: IsExchangeOpenOnDate
      x-api-path-slug: isexchangeopenondate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Exchange
      - Open
      - "On"
      - Date
  /GetSettlementDate:
    get:
      summary: Get Settlement Date
      description: Get settlement date.
      operationId: GetSettlementDate
      x-api-path-slug: getsettlementdate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Settlement
      - Date
  /IsSettlementDate:
    get:
      summary: Is Settlement Date
      description: Is settlement date.
      operationId: IsSettlementDate
      x-api-path-slug: issettlementdate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Settlement
      - Date
  /GetDelayedIndicesValue:
    get:
      summary: Get Delayed Indices Value
      description: Get delayed indices value.
      operationId: GetDelayedIndicesValue
      x-api-path-slug: getdelayedindicesvalue-get
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
      - Delayed
      - Indices
      - Value
  /GetDelayedIndexValue:
    get:
      summary: Get Delayed Index Value
      description: Get delayed index value.
      operationId: GetDelayedIndexValue
      x-api-path-slug: getdelayedindexvalue-get
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
      - Delayed
      - Index
      - Value
  /GetIndexBar:
    get:
      summary: Get Index Bar
      description: Get index bar.
      operationId: GetIndexBar
      x-api-path-slug: getindexbar-get
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
      - Index
      - Bar
  /GetIndexBars:
    get:
      summary: Get Index Bars
      description: Get index bars.
      operationId: GetIndexBars
      x-api-path-slug: getindexbars-get
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
      - Index
      - Bars
  /GetIndexSymbolMappingByOldSymbol:
    get:
      summary: Get Index Symbol Mapping By Old Symbol
      description: Get index symbol mapping by old symbol.
      operationId: GetIndexSymbolMappingByOldSymbol
      x-api-path-slug: getindexsymbolmappingbyoldsymbol-get
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
      - Index
      - Symbol
      - Mapping
      - Old
      - Symbol
  /GetIndexSymbolMappingsByOldSymbols:
    get:
      summary: Get Index Symbol Mappings By Old Symbols
      description: Get index symbol mappings by old symbols.
      operationId: GetIndexSymbolMappingsByOldSymbols
      x-api-path-slug: getindexsymbolmappingsbyoldsymbols-get
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
      - Index
      - Symbol
      - Mappings
      - Old
      - Symbols
  /ListIndexGroups:
    get:
      summary: List Index Groups
      description: List index groups.
      operationId: ListIndexGroups
      x-api-path-slug: listindexgroups-get
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
      - Index
      - Groups
  /ListIndicesByIndexGroup:
    get:
      summary: List Indices By Index Group
      description: List indices by index group.
      operationId: ListIndicesByIndexGroup
      x-api-path-slug: listindicesbyindexgroup-get
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
      - Indices
      - Index
      - Group
  /SearchIndicesByName:
    get:
      summary: Search Indices By Name
      description: Search indices by name.
      operationId: SearchIndicesByName
      x-api-path-slug: searchindicesbyname-get
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
      - Indices
      - Name
  /GetHistoricalIndexValues:
    get:
      summary: Get Historical Index Values
      description: Get historical index values.
      operationId: GetHistoricalIndexValues
      x-api-path-slug: gethistoricalindexvalues-get
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
      - Index
      - Values
  /GetLastClosingIndicesValue:
    get:
      summary: Get Last Closing Indices Value
      description: Get last closing indices value.
      operationId: GetLastClosingIndicesValue
      x-api-path-slug: getlastclosingindicesvalue-get
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
      - Indices
      - Value
  /GetHistoricalIndicesValue:
    get:
      summary: Get Historical Indices Value
      description: Get historical indices value.
      operationId: GetHistoricalIndicesValue
      x-api-path-slug: gethistoricalindicesvalue-get
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
      - Indices
      - Value
  /GetLastClosingIndexValue:
    get:
      summary: Get Last Closing Index Value
      description: Get last closing index value.
      operationId: GetLastClosingIndexValue
      x-api-path-slug: getlastclosingindexvalue-get
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
      - Index
      - Value
  /GetHistoricalIndexValue:
    get:
      summary: Get Historical Index Value
      description: Get historical index value.
      operationId: GetHistoricalIndexValue
      x-api-path-slug: gethistoricalindexvalue-get
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
      - Index
      - Value
  /GetHistoricalIndexValuesTrailing:
    get:
      summary: Get Historical Index Values Trailing
      description: Get historical index values trailing.
      operationId: GetHistoricalIndexValuesTrailing
      x-api-path-slug: gethistoricalindexvaluestrailing-get
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
      - Index
      - Values
      - Trailing
  /GetRealTimeIndicesValue:
    get:
      summary: Get Real Time Indices Value
      description: Get real time indices value.
      operationId: GetRealTimeIndicesValue
      x-api-path-slug: getrealtimeindicesvalue-get
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
      - Time
      - Indices
      - Value
  /GetRealTimeIndexValue:
    get:
      summary: Get Real Time Index Value
      description: Get real time index value.
      operationId: GetRealTimeIndexValue
      x-api-path-slug: getrealtimeindexvalue-get
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
      - Time
      - Index
      - Value
  /GetSecurity:
    get:
      summary: Get Security
      description: Get a list of securities.
      operationId: GetSecurity
      x-api-path-slug: getsecurity-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Security
  /GetSecurities:
    get:
      summary: Get Securities
      description: Get a list of securities.
      operationId: GetSecurities
      x-api-path-slug: getsecurities-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Securities
  /GetInstrument:
    get:
      summary: Get Instrument
      description: Get a list of instruments.
      operationId: GetInstrument
      x-api-path-slug: getinstrument-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Instrument
  /GetInstruments:
    get:
      summary: Get Instruments
      description: Get a list of instruments.
      operationId: GetInstruments
      x-api-path-slug: getinstruments-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Instruments
  /GetIssuer:
    get:
      summary: Get Issuer
      description: Get a list of issuers.
      operationId: GetIssuer
      x-api-path-slug: getissuer-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Issuer
  /GetIssuers:
    get:
      summary: Get Issuers
      description: Get a list of issuers
      operationId: GetIssuers
      x-api-path-slug: getissuers-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Issuers
  /GetIssuerByCompanyIdentifier:
    get:
      summary: Get Issuer By Company Identifier
      description: Get a issuer by the company identifier.
      operationId: GetIssuerByCompanyIdentifier
      x-api-path-slug: getissuerbycompanyidentifier-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Issuer
      - Company
      - Identifier
  /GetMasterByIdentifier:
    get:
      summary: Get Master By Identifier
      description: Get master records by identifier.
      operationId: GetMasterByIdentifier
      x-api-path-slug: getmasterbyidentifier-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Identifier
  /GetMasterByIdentifiers:
    get:
      summary: Get Master By Identifiers
      description: Get master records by identifiers.
      operationId: GetMasterByIdentifiers
      x-api-path-slug: getmasterbyidentifiers-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Identifiers
  /GetMasterByExchange:
    get:
      summary: Get Master By Exchange
      description: Get master records by exchange.
      operationId: GetMasterByExchange
      x-api-path-slug: getmasterbyexchange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Exchange
  /GetMasterByExchangeChanges:
    get:
      summary: Get Master By Exchange Changes
      description: Get a master record by exchange and the last modified since date
      operationId: GetMasterByExchangeChanges
      x-api-path-slug: getmasterbyexchangechanges-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Exchange
      - Changes
  /GetMasterBySector:
    get:
      summary: Get Master By Sector
      description: Old version of the service. Customers should use GetMasterByGlobalSector
      operationId: GetMasterBySector
      x-api-path-slug: getmasterbysector-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Sector
  /GetMasterByIndustry:
    get:
      summary: Get Master By Industry
      description: Old version of the service. Customers should use GetMasterByGlobalIndustry
      operationId: GetMasterByIndustry
      x-api-path-slug: getmasterbyindustry-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Industry
  /GetMasterByGlobalSector:
    get:
      summary: Get Master By Global Sector
      description: Get master records by sector.
      operationId: GetMasterByGlobalSector
      x-api-path-slug: getmasterbyglobalsector-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Global
      - Sector
  /GetMasterByGlobalIndustry:
    get:
      summary: Get Master By Global Industry
      description: Get master records by industry.
      operationId: GetMasterByGlobalIndustry
      x-api-path-slug: getmasterbyglobalindustry-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Global
      - Industry
  /ListIndustries:
    get:
      summary: List Industries
      description: Get the possible industries.
      operationId: ListIndustries
      x-api-path-slug: listindustries-get
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
      - Industries
  /ListInstrumentClasses:
    get:
      summary: List Instrument Classes
      description: Get the possible instrument classes.
      operationId: ListInstrumentClasses
      x-api-path-slug: listinstrumentclasses-get
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
      - Instrument
      - Classes
  /ListSectors:
    get:
      summary: List Sectors
      description: Provides a list of all available values for a given sector.
      operationId: ListSectors
      x-api-path-slug: listsectors-get
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
      - Sectors
  /ListGlobalIndustries:
    get:
      summary: List Global Industries
      description: Get the possible industries.
      operationId: ListGlobalIndustries
      x-api-path-slug: listglobalindustries-get
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
      - Global
      - Industries
  /ListGlobalSectors:
    get:
      summary: List Global Sectors
      description: Get the possible sectors.
      operationId: ListGlobalSectors
      x-api-path-slug: listglobalsectors-get
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
      - Global
      - Sectors
  /ListMICToLegacyExchange:
    get:
      summary: List MIC To Legacy Exchange
      description: Get the legacy exchanges.
      operationId: ListMICToLegacyExchange
      x-api-path-slug: listmictolegacyexchange-get
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
      - MIC
      - Legacy
      - Exchange
  /ListMICToLegacySuffix:
    get:
      summary: List MIC To Legacy Suffix
      description: Get the legacy exchange suffix.
      operationId: ListMICToLegacySuffix
      x-api-path-slug: listmictolegacysuffix-get
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
      - MIC
      - Legacy
      - Suffix
  /ListIdentifiersByExchange:
    get:
      summary: List Identifiers By Exchange
      description: Returns all the Indetifiers and names for securities listed on
        an exchange.
      operationId: ListIdentifiersByExchange
      x-api-path-slug: listidentifiersbyexchange-get
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
      - Identifiers
      - Exchange
  /ListSymbolChanges:
    get:
      summary: List Symbol Changes
      description: This operation returns symbols changed in this exchange.
      operationId: ListSymbolChanges
      x-api-path-slug: listsymbolchanges-get
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
      - Symbol
      - Changes
  /GetMasterStatisticsByExchange:
    get:
      summary: Get Master Statistics By Exchange
      description: Get statistical information about exchanges.
      operationId: GetMasterStatisticsByExchange
      x-api-path-slug: getmasterstatisticsbyexchange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Statistics
      - Exchange
  /GetRealTimeMetalQuotes:
    get:
      summary: Get Real Time Metal Quotes
      description: Get real time exchange rate.
      operationId: GetRealTimeMetalQuotes
      x-api-path-slug: getrealtimemetalquotes-get
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
      - Time
      - Metal
      - Quotes
  /GetHistoricalMetalQuotes:
    get:
      summary: Get Historical Metal Quotes
      description: Get cross sectional historical metal quotes at a given time.
      operationId: GetHistoricalMetalQuotes
      x-api-path-slug: gethistoricalmetalquotes-get
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
      - Metal
      - Quotes
  /GetRealTimeMetalQuote:
    get:
      summary: Get Real Time Metal Quote
      description: Get real time metal quote.
      operationId: GetRealTimeMetalQuote
      x-api-path-slug: getrealtimemetalquote-get
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
      - Time
      - Metal
      - Quote
  /ListMetals:
    get:
      summary: List Metals
      description: List all Metals.
      operationId: ListMetals
      x-api-path-slug: listmetals-get
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
      - Metals
  /GetRealTimeExtendedMetalQuote:
    get:
      summary: Get Real Time Extended Metal Quote
      description: Get real time extended metal quote.
      operationId: GetRealTimeExtendedMetalQuote
      x-api-path-slug: getrealtimeextendedmetalquote-get
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
      - Time
      - Extended
      - Metal
      - Quote
  /GetHistoricalMetalQuote:
    get:
      summary: Get Historical Metal Quote
      description: Get historical metal quote at a given time.
      operationId: GetHistoricalMetalQuote
      x-api-path-slug: gethistoricalmetalquote-get
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
      - Metal
      - Quote
  /GetLatestHistoricalMetalQuote:
    get:
      summary: Get Latest Historical Metal Quote
      description: Get historical metal quote by a given time.
      operationId: GetLatestHistoricalMetalQuote
      x-api-path-slug: getlatesthistoricalmetalquote-get
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
      - Latest
      - Historical
      - Metal
      - Quote
  /GetLatestHistoricalMetalQuotes:
    get:
      summary: Get Latest Historical Metal Quotes
      description: Get cross sectional historical metal quotes by a given time.
      operationId: GetLatestHistoricalMetalQuotes
      x-api-path-slug: getlatesthistoricalmetalquotes-get
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
      - Latest
      - Historical
      - Metal
      - Quotes
  /GetHistoricalMetalQuotesRange:
    get:
      summary: Get Historical Metal Quotes Range
      description: Get historical metal quotes time series.
      operationId: GetHistoricalMetalQuotesRange
      x-api-path-slug: gethistoricalmetalquotesrange-get
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
      - Metal
      - Quotes
      - Range
  /GetLondonHistoricalMetalQuotesRange:
    get:
      summary: Get London Historical Metal Quotes Range
      description: Get historical metal quotes based on Legacy London spot prices.
      operationId: GetLondonHistoricalMetalQuotesRange
      x-api-path-slug: getlondonhistoricalmetalquotesrange-get
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
      - London
      - Historical
      - Metal
      - Quotes
      - Range
  /GetLondonFixing:
    get:
      summary: Get London Fixing
      description: Get last london fixing metal quotes.
      operationId: GetLondonFixing
      x-api-path-slug: getlondonfixing-get
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
      - London
      - Fixing
  /GetHistoricalLondonFixingRange:
    get:
      summary: Get Historical London Fixing Range
      description: Get historical london fixing metal quotes time series.
      operationId: GetHistoricalLondonFixingRange
      x-api-path-slug: gethistoricallondonfixingrange-get
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
      - London
      - Fixing
      - Range
  /GetBaseMetalPrice:
    get:
      summary: Get Base Metal Price
      description: Get base metal price.
      operationId: GetBaseMetalPrice
      x-api-path-slug: getbasemetalprice-get
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
      - Base
      - Metal
      - Price
  /GetTopReleasesBySecurity:
    get:
      summary: Get Top Releases By Security
      description: Return the top press releases for a security.
      operationId: GetTopReleasesBySecurity
      x-api-path-slug: gettopreleasesbysecurity-get
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
      - Releases
      - Security
  /GetHistoricalReleasesBySecurity:
    get:
      summary: Get Historical Releases By Security
      description: Return press releases headlines for a security and a date range.
      operationId: GetHistoricalReleasesBySecurity
      x-api-path-slug: gethistoricalreleasesbysecurity-get
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
      - Releases
      - Security
  /GetMarketNewsDetails:
    get:
      summary: Get Market News Details
      description: Returns the summary content for a specified headline.
      operationId: GetMarketNewsDetails
      x-api-path-slug: getmarketnewsdetails-get
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
      - Market
      - News
      - Details
  /GetTodaysMarketHeadlines:
    get:
      summary: Get Todays Market Headlines
      description: Returns all market headlines that were published today.
      operationId: GetTodaysMarketHeadlines
      x-api-path-slug: gettodaysmarketheadlines-get
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
      - Todays
      - Market
      - Headlines
  /GetTopSecurityHeadlines:
    get:
      summary: Get Top Security Headlines
      description: Returns the most recent specified number of headlines for a given
        security.
      operationId: GetTopSecurityHeadlines
      x-api-path-slug: gettopsecurityheadlines-get
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
      - Security
      - Headlines
  /GetTopMarketHeadlines:
    get:
      summary: Get Top Market Headlines
      description: Returns the most recent specified number of market headlines.
      operationId: GetTopMarketHeadlines
      x-api-path-slug: gettopmarketheadlines-get
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
      - Market
      - Headlines
  /GetTodaysReleasesBySecurity:
    get:
      summary: Get Todays Releases By Security
      description: Return press releases for a security for today.
      operationId: GetTodaysReleasesBySecurity
      x-api-path-slug: gettodaysreleasesbysecurity-get
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
      - Todays
      - Releases
      - Security
  /GetHistoricalSecurityHeadlines:
    get:
      summary: Get Historical Security Headlines
      description: Returns all headlines that were published in a specified time frame
        for a given security.
      operationId: GetHistoricalSecurityHeadlines
      x-api-path-slug: gethistoricalsecurityheadlines-get
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
      - Security
      - Headlines
  /GetTopMarketHeadlinesBySector:
    get:
      summary: Get Top Market Headlines By Sector
      description: Returns the most recent specified number of market headlines associated
        with a specified sector.
      operationId: GetTopMarketHeadlinesBySector
      x-api-path-slug: gettopmarketheadlinesbysector-get
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
      - Market
      - Headlines
      - Sector
  /GetTodaysMarketReleases:
    get:
      summary: Get Todays Market Releases
      description: Return press releases for today.
      operationId: GetTodaysMarketReleases
      x-api-path-slug: gettodaysmarketreleases-get
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
      - Todays
      - Market
      - Releases
  /GetTodaysMarketHeadlinesBySector:
    get:
      summary: Get Todays Market Headlines By Sector
      description: Returns all market headlines that were published today for a specified
        sector.
      operationId: GetTodaysMarketHeadlinesBySector
      x-api-path-slug: gettodaysmarketheadlinesbysector-get
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
      - Todays
      - Market
      - Headlines
      - Sector
  /GetTodaysSecurityHeadlines:
    get:
      summary: Get Todays Security Headlines
      description: Returns all headlines that were published today for a given security.
      operationId: GetTodaysSecurityHeadlines
      x-api-path-slug: gettodayssecurityheadlines-get
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
      - Todays
      - Security
      - Headlines
  /GetRecentTopSecurityHeadlines:
    get:
      summary: Get Recent Top Security Headlines
      description: Returns 14 days specified number of headlines for a given security.
      operationId: GetRecentTopSecurityHeadlines
      x-api-path-slug: getrecenttopsecurityheadlines-get
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
      - Recent
      - Top
      - Security
      - Headlines
  /GetHistoricalMarketHeadlines:
    get:
      summary: Get Historical Market Headlines
      description: Returns all market headlines that were published in a specified
        time frame.
      operationId: GetHistoricalMarketHeadlines
      x-api-path-slug: gethistoricalmarketheadlines-get
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
      - Market
      - Headlines
  /GetHistoricalMarketHeadlinesBySector:
    get:
      summary: Get Historical Market Headlines By Sector
      description: Returns all market headlines that were published in a specified
        time frame for a specified sector.
      operationId: GetHistoricalMarketHeadlinesBySector
      x-api-path-slug: gethistoricalmarketheadlinesbysector-get
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
      - Market
      - Headlines
      - Sector
  /GetTopSecuritySummaries:
    get:
      summary: Get Top Security Summaries
      description: Returns all headline summaries that were published today for a
        given security.
      operationId: GetTopSecuritySummaries
      x-api-path-slug: gettopsecuritysummaries-get
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
      - Security
      - Summaries
  /GetTopReleaseSummariesBySecurity:
    get:
      summary: Get Top Release Summaries By Security
      description: Return the top press releases summaries for a security.
      operationId: GetTopReleaseSummariesBySecurity
      x-api-path-slug: gettopreleasesummariesbysecurity-get
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
      - Release
      - Summaries
      - Security
  /GetTopMarketSummaries:
    get:
      summary: Get Top Market Summaries
      description: Return the top market summaries.
      operationId: GetTopMarketSummaries
      x-api-path-slug: gettopmarketsummaries-get
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
      - Market
      - Summaries
  GetHistoricalMarketHeadlines/:
    get:
      summary: Historical Market Headlines
      description: Returns all market headlines that were published in a specified
        time frame.
      operationId: ""
      x-api-path-slug: gethistoricalmarketheadlines-get
      parameters:
      - in: query
        name: EndDate
        description: The end date range
      - in: query
        name: startDate
        description: The start date range
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetHistoricalMarketHeadlinesBySector/:
    get:
      summary: Historical Market Headlines By Sector
      description: Returns all market headlines that were published in a specified
        time frame for a specified sector.
      operationId: ""
      x-api-path-slug: gethistoricalmarketheadlinesbysector-get
      parameters:
      - in: query
        name: EndDate
        description: The end date range
      - in: query
        name: Sector
        description: The business sector to search within
      - in: query
        name: StartDate
        description: The start date range
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetHistoricalReleasesBySecurity/:
    get:
      summary: Historical Releases By Security
      description: Returns all press releases that were published in a specified time
        frame for a given security.
      operationId: ""
      x-api-path-slug: gethistoricalreleasesbysecurity-get
      parameters:
      - in: query
        name: EndDate
        description: The end date range
      - in: query
        name: Identifier
        description: The ticker symbol for company
      - in: query
        name: IdentifierType
        description: The identifier to use
      - in: query
        name: StartDate
        description: The start date range
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetHistoricalSecurityHeadlines/:
    get:
      summary: Historical Security Headlines
      description: Returns all headlines that were published in a specified time frame
        for a given security.
      operationId: ""
      x-api-path-slug: gethistoricalsecurityheadlines-get
      parameters:
      - in: query
        name: EndDate
        description: The end date range
      - in: query
        name: Identifier
        description: The ticker symbol for company
      - in: query
        name: IdentifierType
        description: The symbol to use
      - in: query
        name: StartDate
        description: The start date range
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetMarketNewsDetails/:
    get:
      summary: Market News Details
      description: Returns the summary content for a specified headline.
      operationId: ""
      x-api-path-slug: getmarketnewsdetails-get
      parameters:
      - in: query
        name: Reference
        description: The URL of the news article
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetTodaysMarketHeadlines/:
    get:
      summary: Todays Market Headlines
      description: Returns all market headlines that were published today.
      operationId: ""
      x-api-path-slug: gettodaysmarketheadlines-get
      parameters:
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetTodaysMarketHeadlinesBySector/:
    get:
      summary: Todays Market Headlines By Sector
      description: Returns all market headlines that were published today for a specified
        sector.
      operationId: ""
      x-api-path-slug: gettodaysmarketheadlinesbysector-get
      parameters:
      - in: query
        name: Sector
        description: The business sector to search within
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetTodaysReleasesBySecurity/:
    get:
      summary: Todays Releases By Security
      description: Returns all press releases that were published today for a given
        security.
      operationId: ""
      x-api-path-slug: gettodaysreleasesbysecurity-get
      parameters:
      - in: query
        name: Identifier
        description: The ticker symbol for company
      - in: query
        name: IdentifierType
        description: The symbol to use
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetTodaysSecurityHeadlines/:
    get:
      summary: Todays Security Headlines
      description: Returns all headlines that were published today for a given security.
      operationId: ""
      x-api-path-slug: gettodayssecurityheadlines-get
      parameters:
      - in: query
        name: Identifier
        description: The ticker symbol for company
      - in: query
        name: IdentifierType
        description: The ticker symbol for company
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetTopMarketHeadlines/:
    get:
      summary: Get Top Market Headlines
      description: Returns the most recent specified number of market headlines.
      operationId: ""
      x-api-path-slug: gettopmarketheadlines-get
      parameters:
      - in: query
        name: Count
        description: Number of headlines to return
      - in: query
        name: _Token
        description: API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetTopMarketHeadlinesBySector/:
    get:
      summary: Top Market Headlines By Sector
      description: Returns the most recent specified number of market headlines associated
        with a specified sector.
      operationId: ""
      x-api-path-slug: gettopmarketheadlinesbysector-get
      parameters:
      - in: query
        name: Count
        description: The number of news items to return
      - in: query
        name: Sector
        description: The business sector to search within
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetTopReleasesBySecurity:
    get:
      summary: Top Releases By Security
      description: Returns the most recent specified number of press releases for
        a given security.
      operationId: ""
      x-api-path-slug: gettopreleasesbysecurity-get
      parameters:
      - in: query
        name: country
        description: Number of items to return
      - in: query
        name: Identifier
        description: The ticker symbol for company
      - in: query
        name: IdentifierType
        description: The identifier to use
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetTopSecurityHeadlines/:
    get:
      summary: Get Top Security Headlines
      description: Returns the most recent specified number of headlines for a given
        security.
      operationId: ""
      x-api-path-slug: gettopsecurityheadlines-get
      parameters:
      - in: query
        name: Count
        description: The number of news items to return
      - in: query
        name: Identifier
        description: The ticker symbol for company
      - in: query
        name: IdentifierType
        description: The ticker symbol for company
      - in: query
        name: _Token
        description: API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  ListSectors/:
    get:
      summary: List Sectors
      description: Provides a list of all available values for a given sector.
      operationId: ""
      x-api-path-slug: listsectors-get
      parameters:
      - in: query
        name: _Token
        description: API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  /GetUnderlyingForOption:
    get:
      summary: Get Underlying For Option
      description: Get details on an underlying instrument for the option symbol provided.
      operationId: GetUnderlyingForOption
      x-api-path-slug: getunderlyingforoption-get
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
      - Underlying
      - Option
  /GetOptionBySymbol:
    get:
      summary: Get Option By Symbol
      description: Get details on an option.
      operationId: GetOptionBySymbol
      x-api-path-slug: getoptionbysymbol-get
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
      - Option
      - Symbol
  /GetOptionChain:
    get:
      summary: Get Option Chain
      description: Get the option chain for the underlying instrument.
      operationId: GetOptionChain
      x-api-path-slug: getoptionchain-get
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
      - Option
      - Chain
  /GetAllEquityOptionChain:
    get:
      summary: Get All Equity Option Chain
      description: Returns options chains for an equity.
      operationId: GetAllEquityOptionChain
      x-api-path-slug: getallequityoptionchain-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Equity
      - Option
      - Chain
  /GetEquityOptionChain:
    get:
      summary: Get Equity Option Chain
      description: Returns options chain for an equity.
      operationId: GetEquityOptionChain
      x-api-path-slug: getequityoptionchain-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Equity
      - Option
      - Chain
  /GetEquityOptionBySymbols:
    get:
      summary: Get Equity Option By Symbols
      description: Returns an array of specific equity options.
      operationId: GetEquityOptionBySymbols
      x-api-path-slug: getequityoptionbysymbols-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Equity
      - Option
      - Symbols
  /GetBlackScholesOptionValue:
    get:
      summary: Get Black Scholes Option Value
      description: Calculates the value of an option using the Black-Scholes formula.
      operationId: GetBlackScholesOptionValue
      x-api-path-slug: getblackscholesoptionvalue-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Black
      - Scholes
      - Option
      - Value
  /GetAllExtendedEquityOptionChain:
    get:
      summary: Get All Extended Equity Option Chain
      description: Returns extended options chains for an equity.
      operationId: GetAllExtendedEquityOptionChain
      x-api-path-slug: getallextendedequityoptionchain-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Extended
      - Equity
      - Option
      - Chain
  /GetExtendedEquityOptionChain:
    get:
      summary: Get Extended Equity Option Chain
      description: Returns extended options chain for an equity.
      operationId: GetExtendedEquityOptionChain
      x-api-path-slug: getextendedequityoptionchain-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Extended
      - Equity
      - Option
      - Chain
  /GetEquityOption:
    get:
      summary: Get Equity Option
      description: Returns a specific equity option.
      operationId: GetEquityOption
      x-api-path-slug: getequityoption-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Equity
      - Option
  /GetExtendedEquityOption:
    get:
      summary: Get Extended Equity Option
      description: Returns a specific equity extended option.
      operationId: GetExtendedEquityOption
      x-api-path-slug: getextendedequityoption-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Extended
      - Equity
      - Option
  /GetEquityOptionSymbol:
    get:
      summary: Get Equity Option Symbol
      description: Returns the symbol for an equity option based on month, year and
        strike price.
      operationId: GetEquityOptionSymbol
      x-api-path-slug: getequityoptionsymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Equity
      - Option
      - Symbol
  /GetEquityOptionBySymbol:
    get:
      summary: Get Equity Option By Symbol
      description: Returns a specific equity option.
      operationId: GetEquityOptionBySymbol
      x-api-path-slug: getequityoptionbysymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Equity
      - Option
      - Symbol
  /GetExtendedEquityOptionBySymbol:
    get:
      summary: Get Extended Equity Option By Symbol
      description: Returns a specific equity extended option.
      operationId: GetExtendedEquityOptionBySymbol
      x-api-path-slug: getextendedequityoptionbysymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Extended
      - Equity
      - Option
      - Symbol
  /GetExtendedEquityOptionBySymbols:
    get:
      summary: Get Extended Equity Option By Symbols
      description: Returns an array of specific equity extended options.
      operationId: GetExtendedEquityOptionBySymbols
      x-api-path-slug: getextendedequityoptionbysymbols-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Extended
      - Equity
      - Option
      - Symbols
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
  /GetTopMovers:
    get:
      summary: Get Top Movers
      description: This operation returns quote information about the top moving equities
        from NYSE, NASDAQ and AMEX.
      operationId: postGettopmovers
      x-api-path-slug: gettopmovers-get
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
  /GetTopGainers:
    get:
      summary: Get Top Gainers
      description: This operation returns quote information about the top gaining
        equities from NYSE, NASDAQ and AMEX.
      operationId: postGettopgainers
      x-api-path-slug: gettopgainers-get
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
  /GetTopLosers:
    get:
      summary: Get Top Losers
      description: This operation returns quote information about the top losing equities
        from NYSE, NASDAQ and AMEX.
      operationId: postGettoplosers
      x-api-path-slug: gettoplosers-get
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
  /GetTopMoversByMarketCapitalization:
    get:
      summary: Get Top Movers By Market Capitalization
      description: This operation returns quote information about the top moving equities
        filtered by market capitalization from NYSE, NASDAQ and AMEX.
      operationId: postGettopmoversbymarketcapitalization
      x-api-path-slug: gettopmoversbymarketcapitalization-get
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
      - Market
      - Capitalization
  /GetTopGainersByMarketCapitalization:
    get:
      summary: Get Top Gainers By Market Capitalization
      description: This operation returns quote information about the top gaining
        equities filtered by market capitalization from NYSE, NASDAQ and AMEX.
      operationId: postGettopgainersbymarketcapitalization
      x-api-path-slug: gettopgainersbymarketcapitalization-get
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
      - Market
      - Capitalization
  /GetTopLosersByMarketCapitalization:
    get:
      summary: Get Top Losers By Market Capitalization
      description: This operation returns quote information about the top losing equities
        filtered by market capitalization from NYSE, NASDAQ and AMEX.
      operationId: postGettoplosersbymarketcapitalization
      x-api-path-slug: gettoplosersbymarketcapitalization-get
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
      - Market
      - Capitalization
  /GetDividendHistory:
    get:
      summary: Get Dividend History
      description: Get dividend history for a stock.
      operationId: postGetdivendhistory
      x-api-path-slug: getdividendhistory-get
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
      - Dividend
      - History
  /GetDividendHistoryRange:
    get:
      summary: Get Dividend History Range
      description: Get dividend history for a stock.
      operationId: postGetdivendhistoryrange
      x-api-path-slug: getdividendhistoryrange-get
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
      - Dividend
      - History
      - Range
  /GetExtendedDividendHistory:
    get:
      summary: Get Extended Dividend History
      description: Get extended dividend history for a stock.
      operationId: postGetextendeddivendhistory
      x-api-path-slug: getextendeddividendhistory-get
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
      - Extended
      - Dividend
      - History
  /GetExtendedDividendHistoryRange:
    get:
      summary: Get Extended Dividend History Range
      description: Get extended dividend history range for a stock.
      operationId: postGetextendeddivendhistoryrange
      x-api-path-slug: getextendeddividendhistoryrange-get
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
      - Extended
      - Dividend
      - History
      - Range
  /GetCompleteDividendHistoryRange:
    get:
      summary: Get Complete Dividend History Range
      description: Get extended dividend history range for a stock.
      operationId: postGetcompletedivendhistoryrange
      x-api-path-slug: getcompletedividendhistoryrange-get
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
      - Complete
      - Dividend
      - History
      - Range
  /GetAllSplits:
    get:
      summary: Get All Splits
      description: Get all splits for a date range.
      operationId: postGetallsplits
      x-api-path-slug: getallsplits-get
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
  /GetAllExtendedDividends:
    get:
      summary: Get All Extended Dividends
      description: Get all extended dividend for a date range.
      operationId: postGetallextendeddivends
      x-api-path-slug: getallextendeddividends-get
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
      - Extended
      - Dividends
  /GetAllDividends:
    get:
      summary: Get All Dividends
      description: Get all splits for a date range.
      operationId: postGetalldivends
      x-api-path-slug: getalldividends-get
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
      - Dividends
  /GetSymbols:
    get:
      summary: Get Symbols
      description: Returns a list of symbols available in the historical database.
      operationId: postGetsymbols
      x-api-path-slug: getsymbols-get
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
      - Symbols
  /GetAdvancesAndDeclines:
    get:
      summary: Get Advances And Declines
      description: Returns numbers of advancing and declining stocks by price and
        volume across exchanges. For more information, go to http://www.xignite.com/
      operationId: postGetadvancesanddeclines
      x-api-path-slug: getadvancesanddeclines-get
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
      - Advances
      - Declines
  /GetHistoricalStatistics:
    get:
      summary: Get Historical Statistics
      description: Returns Historical statistics for a security. For more information,
        go to http://www.xignite.com/
      operationId: postGethistoricalstatistics
      x-api-path-slug: gethistoricalstatistics-get
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
      - Statistics
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
  /GetSOFIBOR:
    get:
      summary: Get SOFIBOR
      description: Returns a SOFIBOR as of a date
      operationId: postGetsofibor
      x-api-path-slug: getsofibor-get
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
      - SOFIBOR
  /GetREIBID:
    get:
      summary: Get REIBID
      description: Returns a REIBID as of a date
      operationId: postGetreib
      x-api-path-slug: getreibid-get
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
      - REIBID
  /GetOIBOR:
    get:
      summary: Get OIBOR
      description: Returns a OIBOR as of a date
      operationId: postGetoibor
      x-api-path-slug: getoibor-get
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
      - OIBOR
  /GetSIBOR:
    get:
      summary: Get SIBOR
      description: Returns a SIBOR as of a date
      operationId: postGetsibor
      x-api-path-slug: getsibor-get
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
      - SIBOR
  /GetCIBOR:
    get:
      summary: Get CIBOR
      description: Returns a CIBOR as of a date
      operationId: postGetcibor
      x-api-path-slug: getcibor-get
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
      - CIBOR
  /GetSTIBOR:
    get:
      summary: Get STIBOR
      description: Returns a STIBOR as of a date
      operationId: postGetstibor
      x-api-path-slug: getstibor-get
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
      - STIBOR
  /GetWIBOR:
    get:
      summary: Get WIBOR
      description: Returns a WIBOR as of a date
      operationId: postGetwibor
      x-api-path-slug: getwibor-get
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
      - WIBOR
  /GetVILIBOR:
    get:
      summary: Get VILIBOR
      description: Returns a VILIBOR as of a date
      operationId: postGetvilibor
      x-api-path-slug: getvilibor-get
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
      - VILIBOR
  /GetEURIBOR:
    get:
      summary: Get EURIBOR
      description: Returns a EURIBOR as of a date
      operationId: postGeteuribor
      x-api-path-slug: geteuribor-get
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
      - EURIBOR
  /GetPRIBOR:
    get:
      summary: Get PRIBOR
      description: Returns a PRIBOR as of a date
      operationId: postGetpribor
      x-api-path-slug: getpribor-get
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
      - PRIBOR
  /GetKORIBOR:
    get:
      summary: Get KORIBOR
      description: Returns a KORIBOR as of a date
      operationId: postGetkoribor
      x-api-path-slug: getkoribor-get
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
      - KORIBOR
  /GetMIBOR:
    get:
      summary: Get MIBOR
      description: Returns a MIBOR as of a date
      operationId: postGetmibor
      x-api-path-slug: getmibor-get
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
      - MIBOR
  /GetMIBID:
    get:
      summary: Get MIBID
      description: Returns a MIBOID as of a date
      operationId: postGetmib
      x-api-path-slug: getmibid-get
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
      - MIBID
  /GetSABOR:
    get:
      summary: Get SABOR
      description: Returns a SABOR as of a date
      operationId: postGetsabor
      x-api-path-slug: getsabor-get
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
      - SABOR
  /GetTAIBOR:
    get:
      summary: Get TAIBOR
      description: Returns a TAIBOR as of a date
      operationId: postGettaibor
      x-api-path-slug: gettaibor-get
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
      - TAIBOR
  /GetTURKIBOR:
    get:
      summary: Get TURKIBOR
      description: Returns a TURKIBOR as of a date
      operationId: postGetturkibor
      x-api-path-slug: getturkibor-get
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
      - TURKIBOR
  /GetMEXIBOR:
    get:
      summary: Get MEXIBOR
      description: Returns a MEXIBOR as of a date
      operationId: postGetmexibor
      x-api-path-slug: getmexibor-get
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
      - MEXIBOR
  /GetTELBOR:
    get:
      summary: Get TELBOR
      description: Returns a TELBOR as of a date
      operationId: postGettelbor
      x-api-path-slug: gettelbor-get
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
      - TELBOR
  /GetCHILIBOR:
    get:
      summary: Get CHILIBOR
      description: Returns a TELBOR as of a date
      operationId: postGetchilibor
      x-api-path-slug: getchilibor-get
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
      - CHILIBOR
  /GetCHIBOR:
    get:
      summary: Get CHIBOR
      description: Returns a CHIBOR as of a date
      operationId: postGetchibor
      x-api-path-slug: getchibor-get
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
      - CHIBOR
  /GetCDOR:
    get:
      summary: Get CDOR
      description: Returns a CDOR as of a date
      operationId: postGetcdor
      x-api-path-slug: getcdor-get
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
      - CDOR
  /GetKAIBOR:
    get:
      summary: Get KAIBOR
      description: Returns a KAIBOR as of a date
      operationId: postGetkaibor
      x-api-path-slug: getkaibor-get
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
      - KAIBOR
  /GetKIBOR:
    get:
      summary: Get KIBOR
      description: Returns a KIBOR as of a date
      operationId: postGetkibor
      x-api-path-slug: getkibor-get
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
      - KIBOR
  /GetKIBID:
    get:
      summary: Get KIBID
      description: Returns a KIBID as of a date
      operationId: postGetkib
      x-api-path-slug: getkibid-get
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
      - KIBID
  /GetSHIBOR:
    get:
      summary: Get SHIBOR
      description: Returns a SHIBOR as of a date
      operationId: postGetshibor
      x-api-path-slug: getshibor-get
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
      - SHIBOR
  /GetJIBOR:
    get:
      summary: Get JIBOR
      description: Returns a JIBOR as of a date
      operationId: postGetjibor
      x-api-path-slug: getjibor-get
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
      - JIBOR
  /GetKLIBOR:
    get:
      summary: Get KLIBOR
      description: Returns a KLIBOR as of a date
      operationId: postGetklibor
      x-api-path-slug: getklibor-get
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
      - KLIBOR
  /GetTIBOR:
    get:
      summary: Get TIBOR
      description: Returns a TIBOR as of a date
      operationId: postGettibor
      x-api-path-slug: gettibor-get
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
      - TIBOR
  /GetPHIBOR:
    get:
      summary: Get PHIBOR
      description: Returns a PHIBOR as of a date
      operationId: postGetphibor
      x-api-path-slug: getphibor-get
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
      - PHIBOR
  /GetBKIBOR:
    get:
      summary: Get BKIBOR
      description: Returns a BKIBOR as of a date
      operationId: postGetbkibor
      x-api-path-slug: getbkibor-get
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
      - BKIBOR
  /GetVNIBOR:
    get:
      summary: Get VNIBOR
      description: Returns a VNIBOR as of a date
      operationId: postGetvnibor
      x-api-path-slug: getvnibor-get
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
      - VNIBOR
  /GetMOSIBOR:
    get:
      summary: Get MOSIBOR
      description: Returns a MOSIBOR as of a date
      operationId: postGetmosibor
      x-api-path-slug: getmosibor-get
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
      - MOSIBOR
  /GetMOSIBID:
    get:
      summary: Get MOSIBID
      description: Returns a MOSIBID as of a date
      operationId: postGetmosib
      x-api-path-slug: getmosibid-get
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
      - MOSIBID
  /GetHistoricalLIBOR:
    get:
      summary: Get Historical LIBOR
      description: ""
      operationId: postGethistoricallibor
      x-api-path-slug: gethistoricallibor-get
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
      - LIBOR
  /GetBRAZIBOR:
    get:
      summary: Get BRAZIBOR
      description: Returns a BRAZIBOR as of a date
      operationId: postGetbrazibor
      x-api-path-slug: getbrazibor-get
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
      - BRAZIBOR
  /GetTRLIBOR:
    get:
      summary: Get TRLIBOR
      description: Returns a TRLIBOR as of a date
      operationId: postGettrlibor
      x-api-path-slug: gettrlibor-get
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
      - TRLIBOR
  /GetTRLIBID:
    get:
      summary: Get TRLIBID
      description: Returns a TRLIBID as of a date
      operationId: postGettrlib
      x-api-path-slug: gettrlibid-get
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
      - TRLIBID
  /GetBRIBOR:
    get:
      summary: Get BRIBOR
      description: Returns a BRIBOR as of a date
      operationId: postGetbribor
      x-api-path-slug: getbribor-get
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
      - BRIBOR
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