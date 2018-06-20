---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Rates Get Average Rates
  description: Returns average rate for a period.
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