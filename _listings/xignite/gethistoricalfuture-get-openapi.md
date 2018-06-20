---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Futures Get Historical Future
  description: Returns a historical quote for a future contract.
  version: 1.0.0
host: www.xignite.com
basePath: xFutures.json/XigniteFutures
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
      description: Provide information about a commodity future.
      operationId: postGetfuture
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
      - Market Data
      - Future
  /ListExchanges:
    get:
      summary: List Exchanges
      description: List commmodities future exchanges and indicates which ones are
        supported.
      operationId: postListexchanges
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