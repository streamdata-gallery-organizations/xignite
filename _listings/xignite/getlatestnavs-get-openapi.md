---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite NAVs Get Latest NAVs
  description: This operation returns the latest NAV information for a list of funds.
  version: 1.0.0
host: navs.xignite.com
basePath: v2/xNAVs.json/XigniteNAVs
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetLatestNAV:
    get:
      summary: Get Latest NAV
      description: This operation returns the latest NAV information for a funds.
      operationId: GetLatestNAV
      x-api-path-slug: getlatestnav-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Latest
      - NAV
  /GetLatestNAVs:
    get:
      summary: Get Latest NAVs
      description: This operation returns the latest NAV information for a list of
        funds.
      operationId: GetLatestNAVs
      x-api-path-slug: getlatestnavs-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Latest
      - NAVs
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