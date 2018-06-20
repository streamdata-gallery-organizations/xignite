---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Indices Real Time Get Index Bars
  description: Get index bars.
  version: 1.0.0
host: globalindicesrealtime.xignite.com
basePath: xglobalindicesrealtime.json/XigniteGlobalIndicesRealTime
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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