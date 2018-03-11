---
swagger: "2.0"
info:
  title: Xignite Futures
  description: Provide delayed and historical commodity quote information from supported
    exchanges (NYMEX...).
  version: 1.0.0
host: www.xignite.com
basePath: xFutures.json/XigniteFutures
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetHistoricalCommodityChartCustomBinary:
    post:
      summary: Get Historical Commodity Chart Custom Binary
      description: Draw a custom historical chart for a future contract
      operationId: postGethistoricalcommoditychartcustombinary
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - historical
      - commodity
      - chart
      - custom
      - binary
definitions:
  Security:
    properties:
      UsernameToken:
        description: This is a default description.
        type: post
      Timestamp:
        description: This is a default description.
        type: post
  GetFutureSymbolInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetFutureSymbolHeader:
    properties: []
  GetFutureSymbolOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetReverseFutureSymbolInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetReverseFutureSymbolHeader:
    properties: []
  GetReverseFutureSymbolOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTerminationScheduleInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTerminationScheduleHeader:
    properties: []
  GetTerminationScheduleOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetNextFutureInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetNextFutureHeader:
    properties: []
  GetNextFutureOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetFutureInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetFutureHeader:
    properties: []
  GetFutureOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListExchangesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListExchangesHeader:
    properties: []
  ListExchangesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListFutureCategoriesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListFutureCategoriesHeader:
    properties: []
  ListFutureCategoriesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListSwapsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListSwapsHeader:
    properties: []
  ListSwapsOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListFuturesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListFuturesHeader:
    properties: []
  ListFuturesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListFrontMonthContractsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListFrontMonthContractsHeader:
    properties: []
  ListFrontMonthContractsOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListFuturesByCategoryInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListFuturesByCategoryHeader:
    properties: []
  ListFuturesByCategoryOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListFuturesByExchangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListFuturesByExchangeHeader:
    properties: []
  ListFuturesByExchangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListSwapsByExchangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListSwapsByExchangeHeader:
    properties: []
  ListSwapsByExchangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedSwapInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedSwapHeader:
    properties: []
  GetDelayedSwapOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedFutureInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedFutureHeader:
    properties: []
  GetDelayedFutureOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedFrontFutureInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedFrontFutureHeader:
    properties: []
  GetDelayedFrontFutureOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllDelayedFuturesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllDelayedFuturesHeader:
    properties: []
  GetAllDelayedFuturesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopDelayedFuturesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopDelayedFuturesHeader:
    properties: []
  GetTopDelayedFuturesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllDelayedSwapsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllDelayedSwapsHeader:
    properties: []
  GetAllDelayedSwapsOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedFuturesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedFuturesHeader:
    properties: []
  GetDelayedFuturesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedFutureStripInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedFutureStripHeader:
    properties: []
  GetDelayedFutureStripOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalFutureStripInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalFutureStripHeader:
    properties: []
  GetHistoricalFutureStripOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwapStripInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwapStripHeader:
    properties: []
  GetHistoricalSwapStripOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedSpotInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedSpotHeader:
    properties: []
  GetDelayedSpotOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedSpotsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedSpotsHeader:
    properties: []
  GetDelayedSpotsOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedFutureBySessionInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedFutureBySessionHeader:
    properties: []
  GetDelayedFutureBySessionOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllDelayedFuturesBySessionInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllDelayedFuturesBySessionHeader:
    properties: []
  GetAllDelayedFuturesBySessionOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedFuturesBySessionInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDelayedFuturesBySessionHeader:
    properties: []
  GetDelayedFuturesBySessionOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalFutureInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalFutureHeader:
    properties: []
  GetHistoricalFutureOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalFuturesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalFuturesHeader:
    properties: []
  GetHistoricalFuturesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllHistoricalFuturesWithStatusInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllHistoricalFuturesWithStatusHeader:
    properties: []
  GetAllHistoricalFuturesWithStatusOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllHistoricalFuturesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllHistoricalFuturesHeader:
    properties: []
  GetAllHistoricalFuturesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalFutureRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalFutureRangeHeader:
    properties: []
  GetHistoricalFutureRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwapInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwapHeader:
    properties: []
  GetHistoricalSwapOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwapRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwapRangeHeader:
    properties: []
  GetHistoricalSwapRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwapsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwapsHeader:
    properties: []
  GetHistoricalSwapsOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllHistoricalSwapsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllHistoricalSwapsHeader:
    properties: []
  GetAllHistoricalSwapsOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCommodityRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCommodityRangeHeader:
    properties: []
  GetHistoricalCommodityRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCommodityMonthlyRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCommodityMonthlyRangeHeader:
    properties: []
  GetHistoricalCommodityMonthlyRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSpotRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSpotRangeHeader:
    properties: []
  GetHistoricalSpotRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSpotMonthlyRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSpotMonthlyRangeHeader:
    properties: []
  GetHistoricalSpotMonthlyRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTickInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTickHeader:
    properties: []
  GetTickOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTicksInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTicksHeader:
    properties: []
  GetTicksOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalTicksInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalTicksHeader:
    properties: []
  GetHistoricalTicksOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalTicksAsOfDateInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalTicksAsOfDateHeader:
    properties: []
  GetHistoricalTicksAsOfDateOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetIntradayFutureChartInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetIntradayFutureChartHeader:
    properties: []
  GetIntradayFutureChartOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetIntradayFutureChartBinaryInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetIntradayFutureChartBinaryHeader:
    properties: []
  GetIntradayFutureChartBinaryOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetIntradayFutureChartCustomInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetIntradayFutureChartCustomHeader:
    properties: []
  GetIntradayFutureChartCustomOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetIntradayFutureChartCustomBinaryInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetIntradayFutureChartCustomBinaryHeader:
    properties: []
  GetIntradayFutureChartCustomBinaryOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalFutureChartInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalFutureChartHeader:
    properties: []
  GetHistoricalFutureChartOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalFutureChartBinaryInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalFutureChartBinaryHeader:
    properties: []
  GetHistoricalFutureChartBinaryOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalFutureChartCustomInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalFutureChartCustomHeader:
    properties: []
  GetHistoricalFutureChartCustomOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalFutureChartCustomBinaryInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalFutureChartCustomBinaryHeader:
    properties: []
  GetHistoricalFutureChartCustomBinaryOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCommodityChartInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCommodityChartHeader:
    properties: []
  GetHistoricalCommodityChartOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCommodityChartBinaryInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCommodityChartBinaryHeader:
    properties: []
  GetHistoricalCommodityChartBinaryOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCommodityChartCustomInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCommodityChartCustomHeader:
    properties: []
  GetHistoricalCommodityChartCustomOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCommodityChartCustomBinaryInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCommodityChartCustomBinaryHeader:
    properties: []
  GetHistoricalCommodityChartCustomBinaryOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetIntradayChartDesignInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetIntradayChartDesignHeader:
    properties: []
  GetIntradayChartDesignOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalChartDesignInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalChartDesignHeader:
    properties: []
  GetHistoricalChartDesignOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetFutureOptionInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetFutureOptionHeader:
    properties: []
  GetFutureOptionOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopIndustryHeadlinesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopIndustryHeadlinesHeader:
    properties: []
  GetTopIndustryHeadlinesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTodaysIndustryHeadlinesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTodaysIndustryHeadlinesHeader:
    properties: []
  GetTodaysIndustryHeadlinesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLastIndustryHeadlinesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLastIndustryHeadlinesHeader:
    properties: []
  GetLastIndustryHeadlinesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetFutureOptionChainInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetFutureOptionChainHeader:
    properties: []
  GetFutureOptionChainOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetFutureOptionsByStrikePriceInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetFutureOptionsByStrikePriceHeader:
    properties: []
  GetFutureOptionsByStrikePriceOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetFutureSymbol_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      Month:
        description: This is a default description.
        type: post
      Year:
        description: This is a default description.
        type: post
  GetFutureSymbolResponse_tns:
    properties: []
  GetReverseFutureSymbol_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
  GetReverseFutureSymbolResponse_tns:
    properties: []
  GetTerminationSchedule_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      Month:
        description: This is a default description.
        type: post
      Year:
        description: This is a default description.
        type: post
  GetTerminationScheduleResponse_tns:
    properties: []
  GetNextFuture_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
  GetNextFutureResponse_tns:
    properties: []
  GetFuture_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
  GetFutureResponse_tns:
    properties: []
  ListExchanges_tns:
    properties: []
  ListExchangesResponse_tns:
    properties: []
  ListFutureCategories_tns:
    properties: []
  ListFutureCategoriesResponse_tns:
    properties: []
  ListSwaps_tns:
    properties: []
  ListSwapsResponse_tns:
    properties: []
  ListFutures_tns:
    properties: []
  ListFuturesResponse_tns:
    properties: []
  ListFrontMonthContracts_tns:
    properties: []
  ListFrontMonthContractsResponse_tns:
    properties: []
  ListFuturesByCategory_tns:
    properties:
      Category:
        description: This is a default description.
        type: post
  ListFuturesByCategoryResponse_tns:
    properties: []
  ListFuturesByExchange_tns:
    properties:
      Exchange:
        description: This is a default description.
        type: post
  ListFuturesByExchangeResponse_tns:
    properties: []
  ListSwapsByExchange_tns:
    properties:
      Exchange:
        description: This is a default description.
        type: post
  ListSwapsByExchangeResponse_tns:
    properties: []
  GetDelayedSwap_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      Month:
        description: This is a default description.
        type: post
      Year:
        description: This is a default description.
        type: post
  GetDelayedSwapResponse_tns:
    properties: []
  GetDelayedFuture_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      Month:
        description: This is a default description.
        type: post
      Year:
        description: This is a default description.
        type: post
  GetDelayedFutureResponse_tns:
    properties: []
  GetDelayedFrontFuture_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
  GetDelayedFrontFutureResponse_tns:
    properties: []
  GetAllDelayedFutures_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
  GetAllDelayedFuturesResponse_tns:
    properties: []
  GetTopDelayedFutures_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      Count:
        description: This is a default description.
        type: post
  GetTopDelayedFuturesResponse_tns:
    properties: []
  GetAllDelayedSwaps_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
  GetAllDelayedSwapsResponse_tns:
    properties: []
  GetDelayedFutures_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
      Month:
        description: This is a default description.
        type: post
      Year:
        description: This is a default description.
        type: post
  GetDelayedFuturesResponse_tns:
    properties: []
  GetDelayedFutureStrip_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
  GetDelayedFutureStripResponse_tns:
    properties: []
  GetHistoricalFutureStrip_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetHistoricalFutureStripResponse_tns:
    properties: []
  GetHistoricalSwapStrip_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetHistoricalSwapStripResponse_tns:
    properties: []
  GetDelayedSpot_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
  GetDelayedSpotResponse_tns:
    properties: []
  GetDelayedSpots_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
  GetDelayedSpotsResponse_tns:
    properties: []
  GetDelayedFutureBySession_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      Month:
        description: This is a default description.
        type: post
      Year:
        description: This is a default description.
        type: post
  GetDelayedFutureBySessionResponse_tns:
    properties: []
  GetAllDelayedFuturesBySession_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
  GetAllDelayedFuturesBySessionResponse_tns:
    properties: []
x-collection-name: Xignite
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