---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Releases Get Historical Security Headlines
  description: Returns headlines for a company and a date range.
  version: v1
host: http://www.xignite.com/
basePath: xReleases.xml/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  GetHistoricalMarketHeadlines/:
    get:
      summary: Get Historical Market Headlines
      description: Returns market headlines for a date range.
      operationId: getGethistoricalmarketheadlines
      x-api-path-slug: gethistoricalmarketheadlines-get
      parameters:
      - in: query
        name: EndDate
        description: The end date range
      - in: query
        name: Source
        description: The source of the news
      - in: query
        name: StartDate
        description: The start date range
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Market
      - Headlines
  GetHistoricalSecurityHeadlines/:
    get:
      summary: Get Historical Security Headlines
      description: Returns headlines for a company and a date range.
      operationId: getGethistoricalsecurityheadlines
      x-api-path-slug: gethistoricalsecurityheadlines-get
      parameters:
      - in: query
        name: EndDate
        description: EndDate
      - in: query
        name: Identifier
        description: The ticker symbol for company
      - in: query
        name: IdentifierType
        description: The identifier to use
      - in: query
        name: Source
        description: The source of the news
      - in: query
        name: StartDate
        description: The start date range
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Security
      - Headlines
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