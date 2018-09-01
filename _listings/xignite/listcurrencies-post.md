---
swagger: "2.0"
info:
  title: Xignite Currencies
  description: Provide real-time currency foreign exchange information and calculations.
  version: 1.0.0
host: www.xignite.com/xCurrencies.json
basePath: /XigniteCurrencies
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ListCurrencies:
    post:
      summary: List Currencies
      description: List supported currencies
      operationId: postListcurrencies
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - list
      - currencies
definitions:
  Security:
    properties:
      UsernameToken:
        description: This is a default description.
        type: post
      Timestamp:
        description: This is a default description.
        type: post
  ListCurrenciesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListCurrenciesHeader:
    properties: []
  ListCurrenciesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListActiveCurrenciesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListActiveCurrenciesHeader:
    properties: []
  ListActiveCurrenciesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListOfficialRatesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListOfficialRatesHeader:
    properties: []
  ListOfficialRatesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetUnitOfAccountInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetUnitOfAccountHeader:
    properties: []
  GetUnitOfAccountOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ConvertRealTimeValueInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ConvertRealTimeValueHeader:
    properties: []
  ConvertRealTimeValueOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ConvertHistoricalValueInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ConvertHistoricalValueHeader:
    properties: []
  ConvertHistoricalValueOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRealTimeForwardRateInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRealTimeForwardRateHeader:
    properties: []
  GetRealTimeForwardRateOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRealTimeCrossRateAsStringInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRealTimeCrossRateAsStringHeader:
    properties: []
  GetRealTimeCrossRateAsStringOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLatestCrossRateInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLatestCrossRateHeader:
    properties: []
  GetLatestCrossRateOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLatestCrossRatesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLatestCrossRatesHeader:
    properties: []
  GetLatestCrossRatesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRealTimeCrossRateInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRealTimeCrossRateHeader:
    properties: []
  GetRealTimeCrossRateOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRealTimeCrossRateGMTInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRealTimeCrossRateGMTHeader:
    properties: []
  GetRealTimeCrossRateGMTOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRawCrossRateInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRawCrossRateHeader:
    properties: []
  GetRawCrossRateOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRawCrossRatesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRawCrossRatesHeader:
    properties: []
  GetRawCrossRatesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRealTimeCrossRatesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRealTimeCrossRatesHeader:
    properties: []
  GetRealTimeCrossRatesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateTablesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateTablesHeader:
    properties: []
  GetHistoricalCrossRateTablesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateTablesBidAskInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateTablesBidAskHeader:
    properties: []
  GetHistoricalCrossRateTablesBidAskOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCurrencyReportInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCurrencyReportHeader:
    properties: []
  GetCurrencyReportOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateTableInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateTableHeader:
    properties: []
  GetHistoricalCrossRateTableOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateTableBidAskInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateTableBidAskHeader:
    properties: []
  GetHistoricalCrossRateTableBidAskOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRealTimeCrossRateTableInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRealTimeCrossRateTableHeader:
    properties: []
  GetRealTimeCrossRateTableOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRealTimeCrossRateTableWithBidAskInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRealTimeCrossRateTableWithBidAskHeader:
    properties: []
  GetRealTimeCrossRateTableWithBidAskOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllCrossRatesForACurrencyInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAllCrossRatesForACurrencyHeader:
    properties: []
  GetAllCrossRatesForACurrencyOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRealTimeCrossRateTableAsHTMLInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRealTimeCrossRateTableAsHTMLHeader:
    properties: []
  GetRealTimeCrossRateTableAsHTMLOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSimpleRealTimeCrossRateTableAsHTMLInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSimpleRealTimeCrossRateTableAsHTMLHeader:
    properties: []
  GetSimpleRealTimeCrossRateTableAsHTMLOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateTableAsHTMLInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateTableAsHTMLHeader:
    properties: []
  GetHistoricalCrossRateTableAsHTMLOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateHeader:
    properties: []
  GetHistoricalCrossRateOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesHeader:
    properties: []
  GetHistoricalCrossRatesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateBidAskInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateBidAskHeader:
    properties: []
  GetHistoricalCrossRateBidAskOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesBidAskInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesBidAskHeader:
    properties: []
  GetHistoricalCrossRatesBidAskOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesRangeHeader:
    properties: []
  GetHistoricalCrossRatesRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesBidAskRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesBidAskRangeHeader:
    properties: []
  GetHistoricalCrossRatesBidAskRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesAsOfInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesAsOfHeader:
    properties: []
  GetHistoricalCrossRatesAsOfOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesBidAskAsOfInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesBidAskAsOfHeader:
    properties: []
  GetHistoricalCrossRatesBidAskAsOfOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetOfficialCrossRateInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetOfficialCrossRateHeader:
    properties: []
  GetOfficialCrossRateOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetOfficialCrossRatesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetOfficialCrossRatesHeader:
    properties: []
  GetOfficialCrossRatesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetOfficialCrossRateBidAskInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetOfficialCrossRateBidAskHeader:
    properties: []
  GetOfficialCrossRateBidAskOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetOfficialCrossRatesBidAskInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetOfficialCrossRatesBidAskHeader:
    properties: []
  GetOfficialCrossRatesBidAskOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetMutipleHistoricalCrossRatesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetMutipleHistoricalCrossRatesHeader:
    properties: []
  GetMutipleHistoricalCrossRatesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAverageHistoricalCrossRatesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAverageHistoricalCrossRatesHeader:
    properties: []
  GetAverageHistoricalCrossRatesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAverageHistoricalCrossRateInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAverageHistoricalCrossRateHeader:
    properties: []
  GetAverageHistoricalCrossRateOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalMonthlyCrossRatesRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalMonthlyCrossRatesRangeHeader:
    properties: []
  GetHistoricalMonthlyCrossRatesRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCrossRateChangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCrossRateChangeHeader:
    properties: []
  GetCrossRateChangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCurrencyChartCustomInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCurrencyChartCustomHeader:
    properties: []
  GetCurrencyChartCustomOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCurrencyChartCustomBinaryInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCurrencyChartCustomBinaryHeader:
    properties: []
  GetCurrencyChartCustomBinaryOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCurrencyChartInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCurrencyChartHeader:
    properties: []
  GetCurrencyChartOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCurrencyChartBinaryInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCurrencyChartBinaryHeader:
    properties: []
  GetCurrencyChartBinaryOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCurrencyIntradayChartInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCurrencyIntradayChartHeader:
    properties: []
  GetCurrencyIntradayChartOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCurrencyIntradayChartCustomBinaryInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCurrencyIntradayChartCustomBinaryHeader:
    properties: []
  GetCurrencyIntradayChartCustomBinaryOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCurrencyIntradayChartCustomInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCurrencyIntradayChartCustomHeader:
    properties: []
  GetCurrencyIntradayChartCustomOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetChartDesignInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetChartDesignHeader:
    properties: []
  GetChartDesignOutput:
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
  GetIntradayHighLowInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetIntradayHighLowHeader:
    properties: []
  GetIntradayHighLowOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListCurrencies_tns:
    properties: []
  ListCurrenciesResponse_tns:
    properties: []
  ListActiveCurrencies_tns:
    properties: []
  ListActiveCurrenciesResponse_tns:
    properties: []
  ListOfficialRates_tns:
    properties: []
  ListOfficialRatesResponse_tns:
    properties: []
  GetUnitOfAccount_tns:
    properties:
      Currency:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetUnitOfAccountResponse_tns:
    properties: []
  ConvertRealTimeValue_tns:
    properties:
      From:
        description: This is a default description.
        type: post
      To:
        description: This is a default description.
        type: post
      Amount:
        description: This is a default description.
        type: post
  ConvertRealTimeValueResponse_tns:
    properties: []
  ConvertHistoricalValue_tns:
    properties:
      From:
        description: This is a default description.
        type: post
      To:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
      Amount:
        description: This is a default description.
        type: post
  ConvertHistoricalValueResponse_tns:
    properties: []
  GetRealTimeForwardRate_tns:
    properties:
      From:
        description: This is a default description.
        type: post
      To:
        description: This is a default description.
        type: post
  GetRealTimeForwardRateResponse_tns:
    properties: []
  GetRealTimeCrossRateAsString_tns:
    properties:
      From:
        description: This is a default description.
        type: post
      To:
        description: This is a default description.
        type: post
  GetRealTimeCrossRateAsStringResponse_tns:
    properties: []
  GetLatestCrossRate_tns:
    properties:
      From:
        description: This is a default description.
        type: post
      To:
        description: This is a default description.
        type: post
  GetLatestCrossRateResponse_tns:
    properties: []
  GetLatestCrossRates_tns:
    properties:
      From:
        description: This is a default description.
        type: post
      Tos:
        description: This is a default description.
        type: post
  GetLatestCrossRatesResponse_tns:
    properties: []
  GetRealTimeCrossRate_tns:
    properties: []
  GetRealTimeCrossRateResponse_tns:
    properties: []
  GetRealTimeCrossRateGMT_tns:
    properties: []
  GetRealTimeCrossRateGMTResponse_tns:
    properties: []
  GetRawCrossRate_tns:
    properties: []
  GetRawCrossRateResponse_tns:
    properties: []
  GetRawCrossRates_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
  GetRawCrossRatesResponse_tns:
    properties: []
  GetRealTimeCrossRates_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
  GetRealTimeCrossRatesResponse_tns:
    properties: []
  GetHistoricalCrossRateTables_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateTablesResponse_tns:
    properties: []
  GetHistoricalCrossRateTablesBidAsk_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateTablesBidAskResponse_tns:
    properties: []
  GetCurrencyReport_tns:
    properties:
      From:
        description: This is a default description.
        type: post
      To:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetCurrencyReportResponse_tns:
    properties: []
  GetHistoricalCrossRateTable_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateTableResponse_tns:
    properties: []
  GetHistoricalCrossRateTableBidAsk_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateTableBidAskResponse_tns:
    properties: []
  GetRealTimeCrossRateTable_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
  GetRealTimeCrossRateTableResponse_tns:
    properties: []
  GetRealTimeCrossRateTableWithBidAsk_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
  GetRealTimeCrossRateTableWithBidAskResponse_tns:
    properties: []
  GetAllCrossRatesForACurrency_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
  GetAllCrossRatesForACurrencyResponse_tns:
    properties: []
  GetRealTimeCrossRateTableAsHTML_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
      ColumnHeaderStyle:
        description: This is a default description.
        type: post
      LineHeaderStyle:
        description: This is a default description.
        type: post
      CellStyle:
        description: This is a default description.
        type: post
  GetRealTimeCrossRateTableAsHTMLResponse_tns:
    properties: []
  GetSimpleRealTimeCrossRateTableAsHTML_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
      ColumnHeaderStyle:
        description: This is a default description.
        type: post
      LineHeaderStyle:
        description: This is a default description.
        type: post
      CellStyle:
        description: This is a default description.
        type: post
  GetSimpleRealTimeCrossRateTableAsHTMLResponse_tns:
    properties: []
  GetHistoricalCrossRateTableAsHTML_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
      ColumnHeaderStyle:
        description: This is a default description.
        type: post
      LineHeaderStyle:
        description: This is a default description.
        type: post
      CellStyle:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateTableAsHTMLResponse_tns:
    properties: []
  GetHistoricalCrossRate_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateResponse_tns:
    properties: []
  GetHistoricalCrossRates_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesResponse_tns:
    properties: []
  GetHistoricalCrossRateBidAsk_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetHistoricalCrossRateBidAskResponse_tns:
    properties: []
  GetHistoricalCrossRatesBidAsk_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesBidAskResponse_tns:
    properties: []
  GetHistoricalCrossRatesRange_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesRangeResponse_tns:
    properties: []
  GetHistoricalCrossRatesBidAskRange_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesBidAskRangeResponse_tns:
    properties: []
  GetHistoricalCrossRatesAsOf_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
      Periods:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesAsOfResponse_tns:
    properties: []
  GetHistoricalCrossRatesBidAskAsOf_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
      Periods:
        description: This is a default description.
        type: post
  GetHistoricalCrossRatesBidAskAsOfResponse_tns:
    properties: []
  GetOfficialCrossRate_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetOfficialCrossRateResponse_tns:
    properties: []
  GetOfficialCrossRates_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetOfficialCrossRatesResponse_tns:
    properties: []
  GetOfficialCrossRateBidAsk_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetOfficialCrossRateBidAskResponse_tns:
    properties: []
  GetOfficialCrossRatesBidAsk_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetOfficialCrossRatesBidAskResponse_tns:
    properties: []
  GetMutipleHistoricalCrossRates_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetMutipleHistoricalCrossRatesResponse_tns:
    properties: []
  GetAverageHistoricalCrossRates_tns:
    properties:
      Symbols:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetAverageHistoricalCrossRatesResponse_tns:
    properties: []
  GetAverageHistoricalCrossRate_tns:
    properties:
      Symbol:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
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