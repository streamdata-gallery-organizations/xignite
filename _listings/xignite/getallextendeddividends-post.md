---
swagger: "2.0"
info:
  title: Xignite Historical
  description: This web service provides historical security pricing for US equities.
  version: 1.0.0
host: www.xignite.com
basePath: xHistorical.json/XigniteHistorical
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetAllExtendedDividends:
    post:
      summary: Get All Extended Dividends
      description: Get all extended dividend for a date range
      operationId: postGetallextendeddivends
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - extended
      - dividends
definitions:
  Security:
    properties:
      UsernameToken:
        description: This is a default description.
        type: post
      Timestamp:
        description: This is a default description.
        type: post
  GetHistoricalQuoteAdjustedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuoteAdjustedHeader:
    properties: []
  GetHistoricalQuoteAdjustedOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuotesAdjustedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuotesAdjustedHeader:
    properties: []
  GetHistoricalQuotesAdjustedOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalMonthlyQuotesRangeAdjustedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalMonthlyQuotesRangeAdjustedHeader:
    properties: []
  GetHistoricalMonthlyQuotesRangeAdjustedOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuotesAsOfAdjustedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuotesAsOfAdjustedHeader:
    properties: []
  GetHistoricalQuotesAsOfAdjustedOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuotesRangeAdjustedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuotesRangeAdjustedHeader:
    properties: []
  GetHistoricalQuotesRangeAdjustedOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalWeeklyQuotesRangeAdjustedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalWeeklyQuotesRangeAdjustedHeader:
    properties: []
  GetHistoricalWeeklyQuotesRangeAdjustedOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuarterlyQuotesRangeAdjustedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuarterlyQuotesRangeAdjustedHeader:
    properties: []
  GetHistoricalQuarterlyQuotesRangeAdjustedOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLastClosingPriceInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLastClosingPriceHeader:
    properties: []
  GetLastClosingPriceOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLastClosingPriceAdjustedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLastClosingPriceAdjustedHeader:
    properties: []
  GetLastClosingPriceAdjustedOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLastClosingPricesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLastClosingPricesHeader:
    properties: []
  GetLastClosingPricesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLastClosingPricesAdjustedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLastClosingPricesAdjustedHeader:
    properties: []
  GetLastClosingPricesAdjustedOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLastClosingPricesOrderedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLastClosingPricesOrderedHeader:
    properties: []
  GetLastClosingPricesOrderedOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLastClosingPricesOrderedAdjustedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLastClosingPricesOrderedAdjustedHeader:
    properties: []
  GetLastClosingPricesOrderedAdjustedOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalHighLowInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalHighLowHeader:
    properties: []
  GetHistoricalHighLowOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuoteInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuoteHeader:
    properties: []
  GetHistoricalQuoteOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuotesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuotesHeader:
    properties: []
  GetHistoricalQuotesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuotesAsOfInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuotesAsOfHeader:
    properties: []
  GetHistoricalQuotesAsOfOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuotesRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuotesRangeHeader:
    properties: []
  GetHistoricalQuotesRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalMonthlyQuotesRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalMonthlyQuotesRangeHeader:
    properties: []
  GetHistoricalMonthlyQuotesRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalWeeklyQuotesRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalWeeklyQuotesRangeHeader:
    properties: []
  GetHistoricalWeeklyQuotesRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuarterlyQuotesRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuarterlyQuotesRangeHeader:
    properties: []
  GetHistoricalQuarterlyQuotesRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopMoversInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopMoversHeader:
    properties: []
  GetTopMoversOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopMoversByExchangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopMoversByExchangeHeader:
    properties: []
  GetTopMoversByExchangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopGainersInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopGainersHeader:
    properties: []
  GetTopGainersOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopLosersInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopLosersHeader:
    properties: []
  GetTopLosersOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopMoversByMarketCapitalizationInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopMoversByMarketCapitalizationHeader:
    properties: []
  GetTopMoversByMarketCapitalizationOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopGainersByMarketCapitalizationInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopGainersByMarketCapitalizationHeader:
    properties: []
  GetTopGainersByMarketCapitalizationOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopLosersByMarketCapitalizationInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopLosersByMarketCapitalizationHeader:
    properties: []
  GetTopLosersByMarketCapitalizationOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDividendHistoryInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDividendHistoryHeader:
    properties: []
  GetDividendHistoryOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDividendHistoryRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetDividendHistoryRangeHeader:
    properties: []
  GetDividendHistoryRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetExtendedDividendHistoryInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetExtendedDividendHistoryHeader:
    properties: []
  GetExtendedDividendHistoryOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetExtendedDividendHistoryRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetExtendedDividendHistoryRangeHeader:
    properties: []
  GetExtendedDividendHistoryRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCompleteDividendHistoryRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCompleteDividendHistoryRangeHeader:
    properties: []
  GetCompleteDividendHistoryRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSplitHistoryInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSplitHistoryHeader:
    properties: []
  GetSplitHistoryOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllSplitsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllSplitsHeader:
    properties: []
  GetAllSplitsOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllExtendedDividendsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllExtendedDividendsHeader:
    properties: []
  GetAllExtendedDividendsOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllDividendsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllDividendsHeader:
    properties: []
  GetAllDividendsOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSplitRatioInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSplitRatioHeader:
    properties: []
  GetSplitRatioOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSymbolsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSymbolsHeader:
    properties: []
  GetSymbolsOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAdvancesAndDeclinesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAdvancesAndDeclinesHeader:
    properties: []
  GetAdvancesAndDeclinesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalStatisticsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalStatisticsHeader:
    properties: []
  GetHistoricalStatisticsOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalQuoteAdjusted_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetHistoricalQuoteAdjustedResponse_tns:
    properties: []
  GetHistoricalQuotesAdjusted_tns:
    properties:
      Identifiers:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetHistoricalQuotesAdjustedResponse_tns:
    properties: []
  GetHistoricalMonthlyQuotesRangeAdjusted_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetHistoricalMonthlyQuotesRangeAdjustedResponse_tns:
    properties: []
  GetHistoricalQuotesAsOfAdjusted_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
      Periods:
        description: This is a default description.
        type: post
  GetHistoricalQuotesAsOfAdjustedResponse_tns:
    properties: []
  GetHistoricalQuotesRangeAdjusted_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetHistoricalQuotesRangeAdjustedResponse_tns:
    properties: []
  GetHistoricalWeeklyQuotesRangeAdjusted_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetHistoricalWeeklyQuotesRangeAdjustedResponse_tns:
    properties: []
  GetHistoricalQuarterlyQuotesRangeAdjusted_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetHistoricalQuarterlyQuotesRangeAdjustedResponse_tns:
    properties: []
  GetLastClosingPrice_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
  GetLastClosingPriceResponse_tns:
    properties: []
  GetLastClosingPriceAdjusted_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
  GetLastClosingPriceAdjustedResponse_tns:
    properties: []
  GetLastClosingPrices_tns:
    properties:
      Identifiers:
        description: This is a default description.
        type: post
  GetLastClosingPricesResponse_tns:
    properties: []
  GetLastClosingPricesAdjusted_tns:
    properties:
      Identifiers:
        description: This is a default description.
        type: post
  GetLastClosingPricesAdjustedResponse_tns:
    properties: []
  GetLastClosingPricesOrdered_tns:
    properties:
      Identifiers:
        description: This is a default description.
        type: post
  GetLastClosingPricesOrderedResponse_tns:
    properties: []
  GetLastClosingPricesOrderedAdjusted_tns:
    properties:
      Identifiers:
        description: This is a default description.
        type: post
  GetLastClosingPricesOrderedAdjustedResponse_tns:
    properties: []
  GetHistoricalHighLow_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetHistoricalHighLowResponse_tns:
    properties: []
  GetHistoricalQuote_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetHistoricalQuoteResponse_tns:
    properties: []
  GetHistoricalQuotes_tns:
    properties:
      Identifiers:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetHistoricalQuotesResponse_tns:
    properties: []
  GetHistoricalQuotesAsOf_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
      Periods:
        description: This is a default description.
        type: post
  GetHistoricalQuotesAsOfResponse_tns:
    properties: []
  GetHistoricalQuotesRange_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetHistoricalQuotesRangeResponse_tns:
    properties: []
  GetHistoricalMonthlyQuotesRange_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetHistoricalMonthlyQuotesRangeResponse_tns:
    properties: []
  GetHistoricalWeeklyQuotesRange_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetHistoricalWeeklyQuotesRangeResponse_tns:
    properties: []
  GetHistoricalQuarterlyQuotesRange_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetHistoricalQuarterlyQuotesRangeResponse_tns:
    properties: []
  GetTopMovers_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
      Count:
        description: This is a default description.
        type: post
  GetTopMoversResponse_tns:
    properties: []
  GetTopMoversByExchange_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
      Count:
        description: This is a default description.
        type: post
  GetTopMoversByExchangeResponse_tns:
    properties: []
  GetTopGainers_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
      Count:
        description: This is a default description.
        type: post
  GetTopGainersResponse_tns:
    properties: []
  GetTopLosers_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
      Count:
        description: This is a default description.
        type: post
  GetTopLosersResponse_tns:
    properties: []
  GetTopMoversByMarketCapitalization_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
      LowCapitalization:
        description: This is a default description.
        type: post
      HighCapitalization:
        description: This is a default description.
        type: post
      Count:
        description: This is a default description.
        type: post
  GetTopMoversByMarketCapitalizationResponse_tns:
    properties: []
  GetTopGainersByMarketCapitalization_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
      LowCapitalization:
        description: This is a default description.
        type: post
      HighCapitalization:
        description: This is a default description.
        type: post
      Count:
        description: This is a default description.
        type: post
  GetTopGainersByMarketCapitalizationResponse_tns:
    properties: []
  GetTopLosersByMarketCapitalization_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
      LowCapitalization:
        description: This is a default description.
        type: post
      HighCapitalization:
        description: This is a default description.
        type: post
      Count:
        description: This is a default description.
        type: post
  GetTopLosersByMarketCapitalizationResponse_tns:
    properties: []
  GetDividendHistory_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
  GetDividendHistoryResponse_tns:
    properties: []
  GetDividendHistoryRange_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetDividendHistoryRangeResponse_tns:
    properties: []
  GetExtendedDividendHistory_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
  GetExtendedDividendHistoryResponse_tns:
    properties: []
  GetExtendedDividendHistoryRange_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetExtendedDividendHistoryRangeResponse_tns:
    properties: []
  GetCompleteDividendHistoryRange_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetCompleteDividendHistoryRangeResponse_tns:
    properties: []
  GetSplitHistory_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetSplitHistoryResponse_tns:
    properties: []
  GetAllSplits_tns:
    properties:
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetAllSplitsResponse_tns:
    properties: []
  GetAllExtendedDividends_tns:
    properties:
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetAllExtendedDividendsResponse_tns:
    properties: []
  GetAllDividends_tns:
    properties:
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetAllDividendsResponse_tns:
    properties: []
  GetSplitRatio_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetSplitRatioResponse_tns:
    properties: []
  GetSymbols_tns:
    properties: []
  GetSymbolsResponse_tns:
    properties: []
  GetAdvancesAndDeclines_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetAdvancesAndDeclinesResponse_tns:
    properties: []
  GetHistoricalStatistics_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
  GetHistoricalStatisticsResponse_tns:
    properties: []
  Header_tns:
    properties:
      Username:
        description: This is a default description.
        type: post
      Password:
        description: This is a default description.
        type: post
      Tracer:
        description: This is a default description.
        type: post
      IHeader_Username:
        description: This is a default description.
        type: post
      IHeader_Password:
        description: This is a default description.
        type: post
      IHeader_Tracer:
        description: This is a default description.
        type: post
  ArrayOfHistoricalQuote_tns:
    properties:
      HistoricalQuote:
        description: This is a default description.
        type: post
  ArrayOfTop_tns:
    properties:
      Top:
        description: This is a default description.
        type: post
  ArrayOfTopByCapitalization_tns:
    properties:
      TopByCapitalization:
        description: This is a default description.
        type: post
  ArrayOfSplitHistory_tns:
    properties:
      SplitHistory:
        description: This is a default description.
        type: post
  Common_tns:
    properties:
      Message:
        description: This is a default description.
        type: post
      Identity:
        description: This is a default description.
        type: post
      Delay:
        description: This is a default description.
        type: post
  ArrayOfDividend_tns:
    properties:
      Dividend:
        description: This is a default description.
        type: post
  ArrayOfExtendedDividend_tns:
    properties:
      ExtendedDividend:
        description: This is a default description.
        type: post
  ArrayOfCompleteDividend_tns:
    properties:
      CompleteDividend:
        description: This is a default description.
        type: post
  ArrayOfSplit_tns:
    properties:
      Split:
        description: This is a default description.
        type: post
  ArrayOfString_tns:
    properties:
      string:
        description: This is a default description.
        type: post
  ArrayOfMarketChange_tns:
    properties:
      MarketChange:
        description: This is a default description.
        type: post
  ExtendedDividend_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      ExDate:
        description: This is a default description.
        type: post
      RecordDate:
        description: This is a default description.
        type: post
      PayDate:
        description: This is a default description.
        type: post
      Amount:
        description: This is a default description.
        type: post
      Yield:
        description: This is a default description.
        type: post
  CompleteDividend_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      ExDate:
        description: This is a default description.
        type: post
      RecordDate:
        description: This is a default description.
        type: post
      PayDate:
        description: This is a default description.
        type: post
      Amount:
        description: This is a default description.
        type: post
      Yield:
        description: This is a default description.
        type: post
      Currency:
        description: This is a default description.
        type: post
      Type:
        description: This is a default description.
        type: post
      Code:
        description: This is a default description.
        type: post
      PaymentFrequency:
        description: This is a default description.
        type: post
  Split_tns:
    properties:
      Date:
        description: This is a default description.
        type: post
      Ratio:
        description: This is a default description.
        type: post
      CumulatedRatio:
        description: This is a default description.
        type: post
      Text:
        description: This is a default description.
        type: post
  MarketChange_tns:
    properties:
      Exchange:
        description: This is a default description.
        type: post
      Type:
        description: This is a default description.
        type: post
      Count:
        description: This is a default description.
        type: post
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