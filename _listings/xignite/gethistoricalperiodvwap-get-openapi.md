---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite VWAP Get Historical Period VWAP
  description: Returns historical VWAP information for a date range.
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