---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Indices Historical Get Last Closing Index Value
  description: Get last closing index value.
  version: 1.0.0
host: globalindiceshistorical.xignite.com
basePath: xglobalindiceshistorical.json/XigniteGlobalIndicesHistorical
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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