---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite VWAP Get10 Minute VWAP
  description: Returns an intraday VWAP for a security based on trades executed in
    the last 10 minutes of the 15/20 minutes delayed quote.
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetHistoricalDailyVWAP:
    get:
      summary: Get Historical Daily VWAP
      description: Returns historical daily VWAP information for a date range
      operationId: GetHistoricalDailyVWAP
      x-api-path-slug: gethistoricaldailyvwap-get
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
      - Daily
      - VWAP
  /GetHistoricalVWAP:
    get:
      summary: Get Historical VWAP
      description: Returns historical VWAP information for a date range
      operationId: GetHistoricalVWAP
      x-api-path-slug: gethistoricalvwap-get
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
      - VWAP
  /GetHistoricalMonthlyVWAP:
    get:
      summary: Get Historical Monthly VWAP
      description: Returns historical monthly VWAP information for a date range.
      operationId: GetHistoricalMonthlyVWAP
      x-api-path-slug: gethistoricalmonthlyvwap-get
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
      - Monthly
      - VWAP
  /GetHistoricalWeeklyVWAP:
    get:
      summary: Get Historical Weekly VWAP
      description: Returns historical weekly VWAP information for a date range.
      operationId: GetHistoricalWeeklyVWAP
      x-api-path-slug: gethistoricalweeklyvwap-get
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
      - Weekly
      - VWAP
  /GetHistoricalPeriodVWAP:
    get:
      summary: Get Historical Period VWAP
      description: Returns historical VWAP information for a date range.
      operationId: GetHistoricalPeriodVWAP
      x-api-path-slug: gethistoricalperiodvwap-get
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
      - Period
      - VWAP
  /GetIntradayVWAP:
    get:
      summary: Get Intraday VWAP
      description: Returns an intraday VWAP for a security based on the trades performed
        in a time range.
      operationId: GetIntradayVWAP
      x-api-path-slug: getintradayvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Intraday
      - VWAP
  /GetHistoricalIntradayVWAP:
    get:
      summary: Get Historical Intraday VWAP
      description: Returns a historical intraday VWAP for a security based on the
        trades performed in a time range.
      operationId: GetHistoricalIntradayVWAP
      x-api-path-slug: gethistoricalintradayvwap-get
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
      - Intraday
      - VWAP
  /GetCorporateIntradayVWAP:
    get:
      summary: Get Corporate Intraday VWAP
      description: Returns a corporate intraday VWAP for a security based on the trades
        performed in a time range.
      operationId: GetCorporateIntradayVWAP
      x-api-path-slug: getcorporateintradayvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Corporate
      - Intraday
      - VWAP
  /GetCorporateHistoricalVWAP:
    get:
      summary: Get Corporate Historical VWAP
      description: Returns a corporate intraday VWAP for a security based on the trades
        performed in a time range.
      operationId: GetCorporateHistoricalVWAP
      x-api-path-slug: getcorporatehistoricalvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Corporate
      - Historical
      - VWAP
  /GetDelayedVWAP:
    get:
      summary: Get Delayed VWAP
      description: Returns an intraday VWAP for a security based on all trades for
        the day up to the 15/20 minutes delayed quote.
      operationId: GetDelayedVWAP
      x-api-path-slug: getdelayedvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Delayed
      - VWAP
  /GetRealTimeVWAP:
    get:
      summary: Get Real Time VWAP
      description: Returns a real-time VWAP for a security based on all INET trades.
      operationId: GetRealTimeVWAP
      x-api-path-slug: getrealtimevwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Real
      - Time
      - VWAP
  /Get1MinuteVWAP:
    get:
      summary: Get1 Minute VWAP
      description: Returns an intraday VWAP for a security based on trades executed
        in the last 1 minute of the 15/20 minutes delayed quote.
      operationId: Get1MinuteVWAP
      x-api-path-slug: get1minutevwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - "1"
      - Minute
      - VWAP
  /Get5MinuteVWAP:
    get:
      summary: Get5 Minute VWAP
      description: Returns an intraday VWAP for a security based on trades executed
        in the last 5 minutes of the 15/20 minutes delayed quote.
      operationId: Get5MinuteVWAP
      x-api-path-slug: get5minutevwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - "5"
      - Minute
      - VWAP
  /Get10MinuteVWAP:
    get:
      summary: Get10 Minute VWAP
      description: Returns an intraday VWAP for a security based on trades executed
        in the last 10 minutes of the 15/20 minutes delayed quote.
      operationId: Get10MinuteVWAP
      x-api-path-slug: get10minutevwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - "10"
      - Minute
      - VWAP
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