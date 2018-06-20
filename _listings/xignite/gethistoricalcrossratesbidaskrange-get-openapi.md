---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Currencies Get Historical Cross Rates Bid Ask Range
  description: This operation returns a range of cross-rates for a currency pair.
  version: 1.0.0
host: www.xignite.com/xCurrencies.json
basePath: /XigniteCurrencies
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ListCurrencies:
    get:
      summary: List Currencies
      description: List supported currencies.
      operationId: postListcurrencies
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
      - Market Data
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