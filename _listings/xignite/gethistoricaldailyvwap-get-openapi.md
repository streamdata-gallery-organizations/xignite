---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite VWAP Get Historical Daily VWAP
  description: Returns historical daily VWAP information for a date range
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