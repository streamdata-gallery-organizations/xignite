---
swagger: "2.0"
info:
  title: Xignite Global Historical
  description: On-demand global historical quotes.
  version: 1.0.0
host: www.xignite.com
basePath: xGlobalHistorical.json/XigniteGlobalHistorical
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetAllCashDividendsByExchange:
    post:
      summary: Get All Cash Dividends By Exchange
      description: Get all cash dividends for a date range in the specified exchange
      operationId: postGetallcashdivendsbyexchange
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - cash
      - dividends
      - by
      - exchange
definitions:
  Security:
    properties:
      UsernameToken:
        description: This is a default description.
        type: post
      Timestamp:
        description: This is a default description.
        type: post
  GetGlobalLastClosingPriceInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalLastClosingPriceHeader:
    properties: []
  GetGlobalLastClosingPriceOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalLastClosingPricesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalLastClosingPricesHeader:
    properties: []
  GetGlobalLastClosingPricesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalQuoteInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalQuoteHeader:
    properties: []
  GetGlobalHistoricalQuoteOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetEndOfDayQuoteInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetEndOfDayQuoteHeader:
    properties: []
  GetEndOfDayQuoteOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetEndOfDayQuotesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetEndOfDayQuotesHeader:
    properties: []
  GetEndOfDayQuotesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetEndOfDayQuotesRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetEndOfDayQuotesRangeHeader:
    properties: []
  GetEndOfDayQuotesRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalQuotesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalQuotesHeader:
    properties: []
  GetGlobalHistoricalQuotesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalQuotesAsOfInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalQuotesAsOfHeader:
    properties: []
  GetGlobalHistoricalQuotesAsOfOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalQuotesRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalQuotesRangeHeader:
    properties: []
  GetGlobalHistoricalQuotesRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalQuotesRangeExtendedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalQuotesRangeExtendedHeader:
    properties: []
  GetGlobalHistoricalQuotesRangeExtendedOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalWeeklyQuotesRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalWeeklyQuotesRangeHeader:
    properties: []
  GetGlobalHistoricalWeeklyQuotesRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalWeeklyQuotesRangeExtendedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalWeeklyQuotesRangeExtendedHeader:
    properties: []
  GetGlobalHistoricalWeeklyQuotesRangeExtendedOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalQuarterlyQuotesRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalQuarterlyQuotesRangeHeader:
    properties: []
  GetGlobalHistoricalQuarterlyQuotesRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalStatisticsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalStatisticsHeader:
    properties: []
  GetGlobalHistoricalStatisticsOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalMonthlyQuotesRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalMonthlyQuotesRangeHeader:
    properties: []
  GetGlobalHistoricalMonthlyQuotesRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalMonthlyQuotesRangeExtendedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetGlobalHistoricalMonthlyQuotesRangeExtendedHeader:
    properties: []
  GetGlobalHistoricalMonthlyQuotesRangeExtendedOutput:
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
  GetTopGainersByExchangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopGainersByExchangeHeader:
    properties: []
  GetTopGainersByExchangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopLosersByExchangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopLosersByExchangeHeader:
    properties: []
  GetTopLosersByExchangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllSplitsByExchangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllSplitsByExchangeHeader:
    properties: []
  GetAllSplitsByExchangeOutput:
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
  GetAllCashDividendsByExchangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllCashDividendsByExchangeHeader:
    properties: []
  GetAllCashDividendsByExchangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCashDividendTotalInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCashDividendTotalHeader:
    properties: []
  GetCashDividendTotalOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCashDividendHistoryInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCashDividendHistoryHeader:
    properties: []
  GetCashDividendHistoryOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllCorporateActionsByExchangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllCorporateActionsByExchangeHeader:
    properties: []
  GetAllCorporateActionsByExchangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCorporateActionHistoryInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCorporateActionHistoryHeader:
    properties: []
  GetCorporateActionHistoryOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListSymbolsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListSymbolsHeader:
    properties: []
  ListSymbolsOutput:
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
  GetGlobalLastClosingPrice_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
  GetGlobalLastClosingPriceResponse_tns:
    properties: []
  GetGlobalLastClosingPrices_tns:
    properties:
      Identifiers:
        description: This is a default description.
        type: post
  GetGlobalLastClosingPricesResponse_tns:
    properties: []
  GetGlobalHistoricalQuote_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetGlobalHistoricalQuoteResponse_tns:
    properties: []
  GetEndOfDayQuote_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetEndOfDayQuoteResponse_tns:
    properties: []
  GetEndOfDayQuotes_tns:
    properties:
      Identifiers:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetEndOfDayQuotesResponse_tns:
    properties: []
  GetEndOfDayQuotesRange_tns:
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
  GetEndOfDayQuotesRangeResponse_tns:
    properties: []
  GetGlobalHistoricalQuotes_tns:
    properties:
      Identifiers:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetGlobalHistoricalQuotesResponse_tns:
    properties: []
  GetGlobalHistoricalQuotesAsOf_tns:
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
  GetGlobalHistoricalQuotesAsOfResponse_tns:
    properties: []
  GetGlobalHistoricalQuotesRange_tns:
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
  GetGlobalHistoricalQuotesRangeResponse_tns:
    properties: []
  GetGlobalHistoricalQuotesRangeExtended_tns:
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
  GetGlobalHistoricalQuotesRangeExtendedResponse_tns:
    properties: []
  GetGlobalHistoricalWeeklyQuotesRange_tns:
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
  GetGlobalHistoricalWeeklyQuotesRangeResponse_tns:
    properties: []
  GetGlobalHistoricalWeeklyQuotesRangeExtended_tns:
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
  GetGlobalHistoricalWeeklyQuotesRangeExtendedResponse_tns:
    properties: []
  GetGlobalHistoricalQuarterlyQuotesRange_tns:
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
  GetGlobalHistoricalQuarterlyQuotesRangeResponse_tns:
    properties: []
  GetGlobalHistoricalStatistics_tns:
    properties:
      Identifier:
        description: This is a default description.
        type: post
  GetGlobalHistoricalStatisticsResponse_tns:
    properties: []
  GetGlobalHistoricalMonthlyQuotesRange_tns:
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
  GetGlobalHistoricalMonthlyQuotesRangeResponse_tns:
    properties: []
  GetGlobalHistoricalMonthlyQuotesRangeExtended_tns:
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
  GetGlobalHistoricalMonthlyQuotesRangeExtendedResponse_tns:
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
  GetTopGainersByExchange_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
      Count:
        description: This is a default description.
        type: post
  GetTopGainersByExchangeResponse_tns:
    properties: []
  GetTopLosersByExchange_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
      Count:
        description: This is a default description.
        type: post
  GetTopLosersByExchangeResponse_tns:
    properties: []
  GetAllSplitsByExchange_tns:
    properties:
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetAllSplitsByExchangeResponse_tns:
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
  GetAllCashDividendsByExchange_tns:
    properties:
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetAllCashDividendsByExchangeResponse_tns:
    properties: []
  GetCashDividendTotal_tns:
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
  GetCashDividendTotalResponse_tns:
    properties: []
  GetCashDividendHistory_tns:
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
  GetCashDividendHistoryResponse_tns:
    properties: []
  GetAllCorporateActionsByExchange_tns:
    properties:
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetAllCorporateActionsByExchangeResponse_tns:
    properties: []
  GetCorporateActionHistory_tns:
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
  GetCorporateActionHistoryResponse_tns:
    properties: []
  ListSymbols_tns:
    properties:
      Exchange:
        description: This is a default description.
        type: post
      StartSymbol:
        description: This is a default description.
        type: post
      EndSymbol:
        description: This is a default description.
        type: post
  ListSymbolsResponse_tns:
    properties: []
  ListExchanges_tns:
    properties: []
  ListExchangesResponse_tns:
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
  ArrayOfGlobalHistoricalQuote_tns:
    properties:
      GlobalHistoricalQuote:
        description: This is a default description.
        type: post
  ArrayOfEndOfDayQuote_tns:
    properties:
      EndOfDayQuote:
        description: This is a default description.
        type: post
  ArrayOfGlobalTop_tns:
    properties:
      GlobalTop:
        description: This is a default description.
        type: post
  ArrayOfSplitHistory_tns:
    properties:
      SplitHistory:
        description: This is a default description.
        type: post
  ArrayOfDividendHistory_tns:
    properties:
      DividendHistory:
        description: This is a default description.
        type: post
  ArrayOfCorporateActionHistory_tns:
    properties:
      CorporateActionHistory:
        description: This is a default description.
        type: post
  ArrayOfGlobalHistoricalQuoteExtended_tns:
    properties:
      GlobalHistoricalQuoteExtended:
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
  ArrayOfSplit_tns:
    properties:
      Split:
        description: This is a default description.
        type: post
  ArrayOfDividend_tns:
    properties:
      Dividend:
        description: This is a default description.
        type: post
  ArrayOfCorporateAction_tns:
    properties:
      CorporateAction:
        description: This is a default description.
        type: post
  ExchangeDescription_tns:
    properties:
      MarketIdentificationCode:
        description: This is a default description.
        type: post
      Market:
        description: This is a default description.
        type: post
  ArrayOfSecurityDescription_tns:
    properties:
      SecurityDescription:
        description: This is a default description.
        type: post
  ArrayOfExchangeDescription_tns:
    properties:
      ExchangeDescription:
        description: This is a default description.
        type: post
  SecurityDescription_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      Name:
        description: This is a default description.
        type: post
      Currency:
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