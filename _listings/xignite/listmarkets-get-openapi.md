---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Logos List Markets
  description: List markets which have avalilable logos.
  version: 1.0.0
host: www.xignite.com
basePath: xLogos.json/XigniteLogos
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetLogo:
    get:
      summary: Get Logo
      description: Save an archive.
      operationId: postGetlogo
      x-api-path-slug: getlogo-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Logo
  /GetLogosList:
    get:
      summary: Get Logos List
      description: Get all symbols which have available logos.
      operationId: postGetlogoslist
      x-api-path-slug: getlogoslist-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Logos
      - List
  /ListMarkets:
    get:
      summary: List Markets
      description: List markets which have avalilable logos.
      operationId: postListmarkets
      x-api-path-slug: listmarkets-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Markets
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