---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Indices Get Delayed Index Value
  description: Get delayed index value.
  version: 1.0.0
host: globalindices.xignite.com
basePath: xglobalindices.json/XigniteGlobalIndices
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetDelayedIndicesValue:
    get:
      summary: Get Delayed Indices Value
      description: Get delayed indices value.
      operationId: GetDelayedIndicesValue
      x-api-path-slug: getdelayedindicesvalue-get
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
      - Indices
      - Value
  /GetDelayedIndexValue:
    get:
      summary: Get Delayed Index Value
      description: Get delayed index value.
      operationId: GetDelayedIndexValue
      x-api-path-slug: getdelayedindexvalue-get
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