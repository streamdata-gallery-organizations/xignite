---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Option Master Get Underlying For Option
  description: Get details on an underlying instrument for the option symbol provided.
  version: 1.0.0
host: globaloptionmaster.xignite.com
basePath: xGlobalOptionMaster.json/XigniteGlobalOptionMaster
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetUnderlyingForOption:
    get:
      summary: Get Underlying For Option
      description: Get details on an underlying instrument for the option symbol provided.
      operationId: GetUnderlyingForOption
      x-api-path-slug: getunderlyingforoption-get
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
      - Underlying
      - Option
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