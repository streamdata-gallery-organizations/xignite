---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Indices Real Time List Indices By Index Group
  description: List indices by index group.
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
  ', Bars':
    get:
      summary: Get Chart Bars
      description: Get chart bars.
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