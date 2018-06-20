---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global News Top Market Headlines By Sector
  description: Returns the most recent specified number of market headlines associated
    with a specified sector.
  version: 1.0.0
host: globalnews.xignite.com
basePath: xGlobalNews.xml/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetTopReleasesBySecurity:
    get:
      summary: Get Top Releases By Security
      description: Return the top press releases for a security.
      operationId: GetTopReleasesBySecurity
      x-api-path-slug: gettopreleasesbysecurity-get
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
      - Top
      - Releases
      - Security
  /GetHistoricalReleasesBySecurity:
    get:
      summary: Get Historical Releases By Security
      description: Return press releases headlines for a security and a date range.
      operationId: GetHistoricalReleasesBySecurity
      x-api-path-slug: gethistoricalreleasesbysecurity-get
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
      - Releases
      - Security
  /GetMarketNewsDetails:
    get:
      summary: Get Market News Details
      description: Returns the summary content for a specified headline.
      operationId: GetMarketNewsDetails
      x-api-path-slug: getmarketnewsdetails-get
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
      - Market
      - News
      - Details
  /GetTodaysMarketHeadlines:
    get:
      summary: Get Todays Market Headlines
      description: Returns all market headlines that were published today.
      operationId: GetTodaysMarketHeadlines
      x-api-path-slug: gettodaysmarketheadlines-get
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
      - Todays
      - Market
      - Headlines
  /GetTopSecurityHeadlines:
    get:
      summary: Get Top Security Headlines
      description: Returns the most recent specified number of headlines for a given
        security.
      operationId: GetTopSecurityHeadlines
      x-api-path-slug: gettopsecurityheadlines-get
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
      - Top
      - Security
      - Headlines
  /GetTopMarketHeadlines:
    get:
      summary: Get Top Market Headlines
      description: Returns the most recent specified number of market headlines.
      operationId: GetTopMarketHeadlines
      x-api-path-slug: gettopmarketheadlines-get
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
      - Top
      - Market
      - Headlines
  /GetTodaysReleasesBySecurity:
    get:
      summary: Get Todays Releases By Security
      description: Return press releases for a security for today.
      operationId: GetTodaysReleasesBySecurity
      x-api-path-slug: gettodaysreleasesbysecurity-get
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
      - Todays
      - Releases
      - Security
  /GetHistoricalSecurityHeadlines:
    get:
      summary: Get Historical Security Headlines
      description: Returns all headlines that were published in a specified time frame
        for a given security.
      operationId: GetHistoricalSecurityHeadlines
      x-api-path-slug: gethistoricalsecurityheadlines-get
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
      - Security
      - Headlines
  /GetTopMarketHeadlinesBySector:
    get:
      summary: Get Top Market Headlines By Sector
      description: Returns the most recent specified number of market headlines associated
        with a specified sector.
      operationId: GetTopMarketHeadlinesBySector
      x-api-path-slug: gettopmarketheadlinesbysector-get
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
      - Top
      - Market
      - Headlines
      - Sector
  /GetTodaysMarketReleases:
    get:
      summary: Get Todays Market Releases
      description: Return press releases for today.
      operationId: GetTodaysMarketReleases
      x-api-path-slug: gettodaysmarketreleases-get
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
      - Todays
      - Market
      - Releases
  /GetTodaysMarketHeadlinesBySector:
    get:
      summary: Get Todays Market Headlines By Sector
      description: Returns all market headlines that were published today for a specified
        sector.
      operationId: GetTodaysMarketHeadlinesBySector
      x-api-path-slug: gettodaysmarketheadlinesbysector-get
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
      - Todays
      - Market
      - Headlines
      - Sector
  /GetTodaysSecurityHeadlines:
    get:
      summary: Get Todays Security Headlines
      description: Returns all headlines that were published today for a given security.
      operationId: GetTodaysSecurityHeadlines
      x-api-path-slug: gettodayssecurityheadlines-get
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
      - Todays
      - Security
      - Headlines
  /GetRecentTopSecurityHeadlines:
    get:
      summary: Get Recent Top Security Headlines
      description: Returns 14 days specified number of headlines for a given security.
      operationId: GetRecentTopSecurityHeadlines
      x-api-path-slug: getrecenttopsecurityheadlines-get
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
      - Recent
      - Top
      - Security
      - Headlines
  /GetHistoricalMarketHeadlines:
    get:
      summary: Get Historical Market Headlines
      description: Returns all market headlines that were published in a specified
        time frame.
      operationId: GetHistoricalMarketHeadlines
      x-api-path-slug: gethistoricalmarketheadlines-get
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
      - Market
      - Headlines
  /GetHistoricalMarketHeadlinesBySector:
    get:
      summary: Get Historical Market Headlines By Sector
      description: Returns all market headlines that were published in a specified
        time frame for a specified sector.
      operationId: GetHistoricalMarketHeadlinesBySector
      x-api-path-slug: gethistoricalmarketheadlinesbysector-get
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
      - Market
      - Headlines
      - Sector
  /ListSectors:
    get:
      summary: List Sectors
      description: Provides a list of all available values for a given sector.
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
      - Market Data
      - List
      - Sectors
  /GetTopSecuritySummaries:
    get:
      summary: Get Top Security Summaries
      description: Returns all headline summaries that were published today for a
        given security.
      operationId: GetTopSecuritySummaries
      x-api-path-slug: gettopsecuritysummaries-get
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
      - Top
      - Security
      - Summaries
  /GetTopReleaseSummariesBySecurity:
    get:
      summary: Get Top Release Summaries By Security
      description: Return the top press releases summaries for a security.
      operationId: GetTopReleaseSummariesBySecurity
      x-api-path-slug: gettopreleasesummariesbysecurity-get
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
      - Top
      - Release
      - Summaries
      - Security
  /GetTopMarketSummaries:
    get:
      summary: Get Top Market Summaries
      description: Return the top market summaries.
      operationId: GetTopMarketSummaries
      x-api-path-slug: gettopmarketsummaries-get
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
      - Top
      - Market
      - Summaries
  /ListExchanges:
    get:
      summary: List Exchanges
      description: List supported exchanges.
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
      - Market Data
      - List
      - Exchanges
  /ListSymbols:
    get:
      summary: List Symbols
      description: This operation returns symbols in this exchange.
      operationId: ListSymbols
      x-api-path-slug: listsymbols-get
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
      - Symbols
  GetHistoricalMarketHeadlines/:
    get:
      summary: Historical Market Headlines
      description: Returns all market headlines that were published in a specified
        time frame.
      operationId: ""
      x-api-path-slug: gethistoricalmarketheadlines-get
      parameters:
      - in: query
        name: EndDate
        description: The end date range
      - in: query
        name: startDate
        description: The start date range
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetHistoricalMarketHeadlinesBySector/:
    get:
      summary: Historical Market Headlines By Sector
      description: Returns all market headlines that were published in a specified
        time frame for a specified sector.
      operationId: ""
      x-api-path-slug: gethistoricalmarketheadlinesbysector-get
      parameters:
      - in: query
        name: EndDate
        description: The end date range
      - in: query
        name: Sector
        description: The business sector to search within
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
      - ""
  GetHistoricalReleasesBySecurity/:
    get:
      summary: Historical Releases By Security
      description: Returns all press releases that were published in a specified time
        frame for a given security.
      operationId: ""
      x-api-path-slug: gethistoricalreleasesbysecurity-get
      parameters:
      - in: query
        name: EndDate
        description: The end date range
      - in: query
        name: Identifier
        description: The ticker symbol for company
      - in: query
        name: IdentifierType
        description: The identifier to use
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
      - ""
  GetHistoricalSecurityHeadlines/:
    get:
      summary: Historical Security Headlines
      description: Returns all headlines that were published in a specified time frame
        for a given security.
      operationId: ""
      x-api-path-slug: gethistoricalsecurityheadlines-get
      parameters:
      - in: query
        name: EndDate
        description: The end date range
      - in: query
        name: Identifier
        description: The ticker symbol for company
      - in: query
        name: IdentifierType
        description: The symbol to use
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
      - ""
  GetMarketNewsDetails/:
    get:
      summary: Market News Details
      description: Returns the summary content for a specified headline.
      operationId: ""
      x-api-path-slug: getmarketnewsdetails-get
      parameters:
      - in: query
        name: Reference
        description: The URL of the news article
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetTodaysMarketHeadlines/:
    get:
      summary: Todays Market Headlines
      description: Returns all market headlines that were published today.
      operationId: ""
      x-api-path-slug: gettodaysmarketheadlines-get
      parameters:
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetTodaysMarketHeadlinesBySector/:
    get:
      summary: Todays Market Headlines By Sector
      description: Returns all market headlines that were published today for a specified
        sector.
      operationId: ""
      x-api-path-slug: gettodaysmarketheadlinesbysector-get
      parameters:
      - in: query
        name: Sector
        description: The business sector to search within
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetTodaysReleasesBySecurity/:
    get:
      summary: Todays Releases By Security
      description: Returns all press releases that were published today for a given
        security.
      operationId: ""
      x-api-path-slug: gettodaysreleasesbysecurity-get
      parameters:
      - in: query
        name: Identifier
        description: The ticker symbol for company
      - in: query
        name: IdentifierType
        description: The symbol to use
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetTodaysSecurityHeadlines/:
    get:
      summary: Todays Security Headlines
      description: Returns all headlines that were published today for a given security.
      operationId: ""
      x-api-path-slug: gettodayssecurityheadlines-get
      parameters:
      - in: query
        name: Identifier
        description: The ticker symbol for company
      - in: query
        name: IdentifierType
        description: The ticker symbol for company
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetTopMarketHeadlines/:
    get:
      summary: Get Top Market Headlines
      description: Returns the most recent specified number of market headlines.
      operationId: ""
      x-api-path-slug: gettopmarketheadlines-get
      parameters:
      - in: query
        name: Count
        description: Number of headlines to return
      - in: query
        name: _Token
        description: API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
  GetTopMarketHeadlinesBySector/:
    get:
      summary: Top Market Headlines By Sector
      description: Returns the most recent specified number of market headlines associated
        with a specified sector.
      operationId: ""
      x-api-path-slug: gettopmarketheadlinesbysector-get
      parameters:
      - in: query
        name: Count
        description: The number of news items to return
      - in: query
        name: Sector
        description: The business sector to search within
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - ""
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