---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Master Get Master Statistics By Exchange
  description: Get statistical information about exchanges.
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
  /GetMasterByExchange:
    get:
      summary: Get Master By Exchange
      description: Get master records by exchange.
      operationId: GetMasterByExchange
      x-api-path-slug: getmasterbyexchange-get
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
      - Exchange
  /GetMasterByExchangeChanges:
    get:
      summary: Get Master By Exchange Changes
      description: Get a master record by exchange and the last modified since date
      operationId: GetMasterByExchangeChanges
      x-api-path-slug: getmasterbyexchangechanges-get
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
      - Exchange
      - Changes
  /GetMasterBySector:
    get:
      summary: Get Master By Sector
      description: Old version of the service. Customers should use GetMasterByGlobalSector
      operationId: GetMasterBySector
      x-api-path-slug: getmasterbysector-get
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
      - Sector
  /GetMasterByIndustry:
    get:
      summary: Get Master By Industry
      description: Old version of the service. Customers should use GetMasterByGlobalIndustry
      operationId: GetMasterByIndustry
      x-api-path-slug: getmasterbyindustry-get
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
      - Industry
  /GetMasterByGlobalSector:
    get:
      summary: Get Master By Global Sector
      description: Get master records by sector.
      operationId: GetMasterByGlobalSector
      x-api-path-slug: getmasterbyglobalsector-get
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
      - Global
      - Sector
  /GetMasterByGlobalIndustry:
    get:
      summary: Get Master By Global Industry
      description: Get master records by industry.
      operationId: GetMasterByGlobalIndustry
      x-api-path-slug: getmasterbyglobalindustry-get
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
      - Global
      - Industry
  /ListExchanges:
    get:
      summary: List Exchanges
      description: Get the possible exchanges.
      operationId: ListExchanges
      x-api-path-slug: listexchanges-get
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
      - Exchanges
  /ListIndustries:
    get:
      summary: List Industries
      description: Get the possible industries.
      operationId: ListIndustries
      x-api-path-slug: listindustries-get
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
      - Industries
  /ListInstrumentClasses:
    get:
      summary: List Instrument Classes
      description: Get the possible instrument classes.
      operationId: ListInstrumentClasses
      x-api-path-slug: listinstrumentclasses-get
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
      - Instrument
      - Classes
  /ListSectors:
    get:
      summary: List Sectors
      description: Get the possible sectors.
      operationId: ListSectors
      x-api-path-slug: listsectors-get
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
      - Sectors
  /ListGlobalIndustries:
    get:
      summary: List Global Industries
      description: Get the possible industries.
      operationId: ListGlobalIndustries
      x-api-path-slug: listglobalindustries-get
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
      - Global
      - Industries
  /ListGlobalSectors:
    get:
      summary: List Global Sectors
      description: Get the possible sectors.
      operationId: ListGlobalSectors
      x-api-path-slug: listglobalsectors-get
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
      - Global
      - Sectors
  /ListMICToLegacyExchange:
    get:
      summary: List MIC To Legacy Exchange
      description: Get the legacy exchanges.
      operationId: ListMICToLegacyExchange
      x-api-path-slug: listmictolegacyexchange-get
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
      - MIC
      - Legacy
      - Exchange
  /ListMICToLegacySuffix:
    get:
      summary: List MIC To Legacy Suffix
      description: Get the legacy exchange suffix.
      operationId: ListMICToLegacySuffix
      x-api-path-slug: listmictolegacysuffix-get
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
      - MIC
      - Legacy
      - Suffix
  /ListIdentifiersByExchange:
    get:
      summary: List Identifiers By Exchange
      description: Returns all the Indetifiers and names for securities listed on
        an exchange.
      operationId: ListIdentifiersByExchange
      x-api-path-slug: listidentifiersbyexchange-get
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
      - Identifiers
      - Exchange
  /ListSymbolChanges:
    get:
      summary: List Symbol Changes
      description: This operation returns symbols changed in this exchange.
      operationId: ListSymbolChanges
      x-api-path-slug: listsymbolchanges-get
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
      - Symbol
      - Changes
  /GetMasterStatisticsByExchange:
    get:
      summary: Get Master Statistics By Exchange
      description: Get statistical information about exchanges.
      operationId: GetMasterStatisticsByExchange
      x-api-path-slug: getmasterstatisticsbyexchange-get
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
      - Statistics
      - Exchange
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