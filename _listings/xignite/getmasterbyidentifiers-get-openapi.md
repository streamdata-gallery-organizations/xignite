---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Master Get Master By Identifiers
  description: Get master records by identifiers.
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
  /GetInstruments:
    get:
      summary: Get Instruments
      description: Get a list of instruments.
      operationId: GetInstruments
      x-api-path-slug: getinstruments-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Instruments
  /GetIssuer:
    get:
      summary: Get Issuer
      description: Get a list of issuers.
      operationId: GetIssuer
      x-api-path-slug: getissuer-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Issuer
  /GetIssuers:
    get:
      summary: Get Issuers
      description: Get a list of issuers
      operationId: GetIssuers
      x-api-path-slug: getissuers-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Issuers
  /GetIssuerByCompanyIdentifier:
    get:
      summary: Get Issuer By Company Identifier
      description: Get a issuer by the company identifier.
      operationId: GetIssuerByCompanyIdentifier
      x-api-path-slug: getissuerbycompanyidentifier-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Issuer
      - Company
      - Identifier
  /GetMasterByIdentifier:
    get:
      summary: Get Master By Identifier
      description: Get master records by identifier.
      operationId: GetMasterByIdentifier
      x-api-path-slug: getmasterbyidentifier-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Identifier
  /GetMasterByIdentifiers:
    get:
      summary: Get Master By Identifiers
      description: Get master records by identifiers.
      operationId: GetMasterByIdentifiers
      x-api-path-slug: getmasterbyidentifiers-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Master
      - Identifiers
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