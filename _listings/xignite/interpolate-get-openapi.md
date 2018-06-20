---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Rates Interpolate
  description: Interpolate a data series using various methodologies.
  version: 1.0.0
host: www.xignite.com
basePath: xRates.json/XigniteRates
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
  /GetStateRate:
    get:
      summary: Get State Rate
      description: Returns a state rate
      operationId: postGetstaterate
      x-api-path-slug: getstaterate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - State
      - Rate
  /GetStateRates:
    get:
      summary: Get State Rates
      description: Returns state rates for a date range.
      operationId: postGetstaterates
      x-api-path-slug: getstaterates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - State
      - Rates
  /GetFederalRate:
    get:
      summary: Get Federal Rate
      description: Returns a federal discount borrowing rate
      operationId: postGetfederalrate
      x-api-path-slug: getfederalrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Federal
      - Rate
  /GetFederalRates:
    get:
      summary: Get Federal Rates
      description: Returns federal discount borrowing for a date range.
      operationId: postGetfederalrates
      x-api-path-slug: getfederalrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Federal
      - Rates
  /GetForwardRateAgreement:
    get:
      summary: Get Forward Rate Agreement
      description: Returns a calculated Forward Rate Agreement as of a date
      operationId: postGetforwardrateagreement
      x-api-path-slug: getforwardrateagreement-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Forward
      - Rate
      - Agreement
  /GetEuroDollarFRAStrip:
    get:
      summary: Get Euro DollarFRA Strip
      description: Returns an IMM EuroDollar Synthetic Forward Rate strip
      operationId: postGeteurodollarfrastrip
      x-api-path-slug: geteurodollarfrastrip-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Euro
      - DollarFRStrip
  /GetSwapRate:
    get:
      summary: Get Swap Rate
      description: Returns a Swap rate
      operationId: postGetswaprate
      x-api-path-slug: getswaprate-get
      parameters:
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
      - Rate
  /GetSwapRateFamily:
    get:
      summary: Get Swap Rate Family
      description: Returns a Swap rate Family
      operationId: postGetswapratefamily
      x-api-path-slug: getswapratefamily-get
      parameters:
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
      - Rate
      - Family
  /GetHistoricalSwapRate:
    get:
      summary: Get Historical Swap Rate
      description: Returns a Swap rate as of a historical date
      operationId: postGethistoricalswaprate
      x-api-path-slug: gethistoricalswaprate-get
      parameters:
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
      - Rate
  /GetHistoricalSwapRateRange:
    get:
      summary: Get Historical Swap Rate Range
      description: Returns a Swap rate as of a historical date
      operationId: postGethistoricalswapraterange
      x-api-path-slug: gethistoricalswapraterange-get
      parameters:
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
      - Rate
      - Range
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
      summary: Get HIBOR
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
      - HIBOR
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
  /GetWSJRate:
    get:
      summary: Get WSJ Rate
      description: Returns a specific interest rate.
      operationId: postGetwsjrate
      x-api-path-slug: getwsjrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - WSJ
      - Rate
  /GetTelerate3750:
    get:
      summary: Get Telerate3750
      description: Returns LIBOR rates as published daily on the Telerate 3750 screen
        at about 11:00 AM London time.
      operationId: postGettelerate3750
      x-api-path-slug: gettelerate3750-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Telerate3750
  /GetLastLondonFixing:
    get:
      summary: Get Last London Fixing
      description: Returns last UK Gold or Silver Fixings.
      operationId: postGetlastlondonfixing
      x-api-path-slug: getlastlondonfixing-get
      parameters:
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
      - London
      - Fixing
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
  /ListRatesByRateFamily:
    get:
      summary: List Rates By Rate Family
      description: List supported interest rates from a RateFamilyType.
      operationId: postListratesbyratefamily
      x-api-path-slug: listratesbyratefamily-get
      parameters:
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
      - Rate
      - Family
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
  /GetRateSymbol:
    get:
      summary: Get Rate Symbol
      description: Returns the symbol for a rate.
      operationId: postGetratesymbol
      x-api-path-slug: getratesymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - Symbol
  /GetRateFromSymbol:
    get:
      summary: Get Rate From Symbol
      description: Returns the symbol for a rate.
      operationId: postGetratefromsymbol
      x-api-path-slug: getratefromsymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - From
      - Symbol
  /GetRate:
    get:
      summary: Get Rate
      description: Returns a rate as of a specific date.
      operationId: postGetrate
      x-api-path-slug: getrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
  /GetRateFamilyTable:
    get:
      summary: Get Rate Family Table
      description: Returns a rate table for a rate family.
      operationId: postGetratefamilytable
      x-api-path-slug: getratefamilytable-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - Family
      - Table
  /GetAverageRate:
    get:
      summary: Get Average Rate
      description: Returns an average rate as of a specific date.
      operationId: postGetaveragerate
      x-api-path-slug: getaveragerate-get
      parameters:
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
      - Rate
  /GetAverageRates:
    get:
      summary: Get Average Rates
      description: Returns average rate for a period.
      operationId: postGetaveragerates
      x-api-path-slug: getaveragerates-get
      parameters:
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
      - Rates
  /GetRateMovingAverage:
    get:
      summary: Get Rate Moving Average
      description: Returns a moving  average rate as of a specific date
      operationId: postGetratemovingaverage
      x-api-path-slug: getratemovingaverage-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - Moving
      - Average
  /GetDailyAverage:
    get:
      summary: Get Daily Average
      description: Returns a daily average rate as of a specific date
      operationId: postGetdailyaverage
      x-api-path-slug: getdailyaverage-get
      parameters:
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
      - Average
  /GetMonthlyTreasuryAverage:
    get:
      summary: Get Monthly Treasury Average
      description: Returns a daily average rate as of a specific date
      operationId: postGetmonthlytreasuryaverage
      x-api-path-slug: getmonthlytreasuryaverage-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Monthly
      - Treasury
      - Average
  /GetRateFamily:
    get:
      summary: Get Rate Family
      description: Returns a collection of related rate as of a specific date
      operationId: postGetratefamily
      x-api-path-slug: getratefamily-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - Family
  /GetTodaysRate:
    get:
      summary: Get Todays Rate
      description: Returns end of day closing value for a rate
      operationId: postGettodaysrate
      x-api-path-slug: gettodaysrate-get
      parameters:
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
      - Rate
  /GetLatestRate:
    get:
      summary: Get Latest Rate
      description: Returns latest value for a rate.
      operationId: postGetlatestrate
      x-api-path-slug: getlatestrate-get
      parameters:
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
      - Rate
  /GetLatestRateSpecial:
    get:
      summary: Get Latest Rate Special
      description: Returns latest value for a rate.
      operationId: postGetlatestratespecial
      x-api-path-slug: getlatestratespecial-get
      parameters:
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
      - Rate
      - Special
  /GetLatestRateFamily:
    get:
      summary: Get Latest Rate Family
      description: Returns latest values for a rate family.
      operationId: postGetlatestratefamily
      x-api-path-slug: getlatestratefamily-get
      parameters:
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
      - Rate
      - Family
  /GetRealTimeRate:
    get:
      summary: Get Real Time Rate
      description: Returns the value for a rate as of a specific time in the day.
      operationId: postGetrealtimerate
      x-api-path-slug: getrealtimerate-get
      parameters:
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
      - Rate
  /GetRateAsOfTime:
    get:
      summary: Get Rate As Of Time
      description: Returns the value for a rate as of a specific time in the day.
      operationId: postGetrateasoftime
      x-api-path-slug: getrateasoftime-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - As
      - Time
  /GetHistoricalRates:
    get:
      summary: Get Historical Rates
      description: Returns a rate for a range of dates.
      operationId: postGethistoricalrates
      x-api-path-slug: gethistoricalrates-get
      parameters:
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
      - Rates
  /GetHistoricalWeeklyRates:
    get:
      summary: Get Historical Weekly Rates
      description: Returns a rate for a range of dates.
      operationId: postGethistoricalweeklyrates
      x-api-path-slug: gethistoricalweeklyrates-get
      parameters:
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
      - Rates
  /GetHistoricalRateFamily:
    get:
      summary: Get Historical Rate Family
      description: Returns a rate family and for a range of dates.
      operationId: postGethistoricalratefamily
      x-api-path-slug: gethistoricalratefamily-get
      parameters:
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
      - Rate
      - Family
  /GetRateDescription:
    get:
      summary: Get Rate Description
      description: Returns a description for a rate.
      operationId: postGetratedescription
      x-api-path-slug: getratedescription-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - Description
  /GetRateStatistics:
    get:
      summary: Get Rate Statistics
      description: Returns statistics for available rates.
      operationId: postGetratestatistics
      x-api-path-slug: getratestatistics-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - Statistics
  Draw, Rate, , Custom:
    get:
      summary: Draw Rate Chart Custom
      description: Draw a custom rate chart for a date range.
      operationId: postDrawratechartcustom
      x-api-path-slug: draw-rate--custom-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Rate
      - Chart
      - Custom
  'Draw, Rate, ':
    get:
      summary: Draw Rate Chart
      description: Draw a standard rate chart for a date range.
      operationId: postDrawratechart
      x-api-path-slug: draw-rate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Rate
      - Chart
  Draw, Rate, , Preset:
    get:
      summary: Draw Rate Chart Preset
      description: Draw a standard rate chart for a date range.
      operationId: postDrawratechartpreset
      x-api-path-slug: draw-rate--preset-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Rate
      - Chart
      - Preset
  ', Design':
    get:
      summary: Get Chart Design
      description: Returns the default design class for the rate Chart.
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
  /DrawYieldCurve:
    get:
      summary: Draw Yield Curve
      description: Draw a yield curve for a rate family.
      operationId: postDrawyieldcurve
      x-api-path-slug: drawyieldcurve-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Yield
      - Curve
  /DrawYieldCurvePreset:
    get:
      summary: Draw Yield Curve Preset
      description: Draw a yield curve for a rate family.
      operationId: postDrawyieldcurvepreset
      x-api-path-slug: drawyieldcurvepreset-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Yield
      - Curve
      - Preset
  /DrawYieldCurveCustom:
    get:
      summary: Draw Yield Curve Custom
      description: Draw a yield curve for a rate family.
      operationId: postDrawyieldcurvecustom
      x-api-path-slug: drawyieldcurvecustom-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Yield
      - Curve
      - Custom
  /Interpolate:
    get:
      summary: Interpolate
      description: Interpolate a data series using various methodologies.
      operationId: postInterpolate
      x-api-path-slug: interpolate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Interpolate
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