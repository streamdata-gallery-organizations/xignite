---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Master Get Instrument
  description: Get a list of instruments.
  version: 1.0.0
host: globalmaster.xignite.com
basePath: xglobalmaster.json/XigniteGlobalMaster
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetSecurity:
    get:
      summary: Get Security
      description: Get a list of securities.
      operationId: GetSecurity
      x-api-path-slug: getsecurity-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Security
  /GetSecurities:
    get:
      summary: Get Securities
      description: Get a list of securities.
      operationId: GetSecurities
      x-api-path-slug: getsecurities-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Securities
  /GetInstrument:
    get:
      summary: Get Instrument
      description: Get a list of instruments.
      operationId: GetInstrument
      x-api-path-slug: getinstrument-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Instrument
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