---
swagger: "2.0"
info:
  title: Xignite Money Markets
  description: Provide information about money market derivatives.
  version: 1.0.0
host: www.xignite.com
basePath: xMoneyMarkets.json/XigniteMoneyMarkets
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /SearchRates:
    post:
      summary: Search Rates
      description: Search rate names and description
      operationId: postSearchrates
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - search
      - rates
definitions:
  Security:
    properties:
      UsernameToken:
        description: This is a default description.
        type: post
      Timestamp:
        description: This is a default description.
        type: post
  GetSwapRateInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSwapRateHeader:
    properties: []
  GetSwapRateOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListRatesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListRatesHeader:
    properties: []
  ListRatesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  SearchRatesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  SearchRatesHeader:
    properties: []
  SearchRatesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetForwardRateAgreementInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetForwardRateAgreementHeader:
    properties: []
  GetForwardRateAgreementOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetEuroDollarFRAStripInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetEuroDollarFRAStripHeader:
    properties: []
  GetEuroDollarFRAStripOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSwaptionInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSwaptionHeader:
    properties: []
  GetSwaptionOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSwaptionFamilyInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSwaptionFamilyHeader:
    properties: []
  GetSwaptionFamilyOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwaptionInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwaptionHeader:
    properties: []
  GetHistoricalSwaptionOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwaptionFamilyInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwaptionFamilyHeader:
    properties: []
  GetHistoricalSwaptionFamilyOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSwapRateFamilyInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSwapRateFamilyHeader:
    properties: []
  GetSwapRateFamilyOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwapRateInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwapRateHeader:
    properties: []
  GetHistoricalSwapRateOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwapRateRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwapRateRangeHeader:
    properties: []
  GetHistoricalSwapRateRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSwapRateExtendedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSwapRateExtendedHeader:
    properties: []
  GetSwapRateExtendedOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSwapRateFamilyExtendedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSwapRateFamilyExtendedHeader:
    properties: []
  GetSwapRateFamilyExtendedOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwapRateExtendedInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwapRateExtendedHeader:
    properties: []
  GetHistoricalSwapRateExtendedOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwapRateExtendedRangeInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalSwapRateExtendedRangeHeader:
    properties: []
  GetHistoricalSwapRateExtendedRangeOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListSwapRatesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  ListSwapRatesHeader:
    properties: []
  ListSwapRatesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTreasuryRateInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTreasuryRateHeader:
    properties: []
  GetTreasuryRateOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTreasuryRateFamilyInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTreasuryRateFamilyHeader:
    properties: []
  GetTreasuryRateFamilyOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSwapRate_tns:
    properties: []
  GetSwapRateResponse_tns:
    properties: []
  ListRates_tns:
    properties: []
  ListRatesResponse_tns:
    properties: []
  SearchRates_tns:
    properties:
      Pattern:
        description: This is a default description.
        type: post
  SearchRatesResponse_tns:
    properties: []
  GetForwardRateAgreement_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetForwardRateAgreementResponse_tns:
    properties: []
  GetEuroDollarFRAStrip_tns:
    properties: []
  GetEuroDollarFRAStripResponse_tns:
    properties: []
  GetSwaption_tns:
    properties: []
  GetSwaptionResponse_tns:
    properties: []
  GetSwaptionFamily_tns:
    properties: []
  GetSwaptionFamilyResponse_tns:
    properties: []
  GetHistoricalSwaption_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetHistoricalSwaptionResponse_tns:
    properties: []
  GetHistoricalSwaptionFamily_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetHistoricalSwaptionFamilyResponse_tns:
    properties: []
  GetSwapRateFamily_tns:
    properties: []
  GetSwapRateFamilyResponse_tns:
    properties: []
  GetHistoricalSwapRate_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetHistoricalSwapRateResponse_tns:
    properties: []
  GetHistoricalSwapRateRange_tns:
    properties:
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetHistoricalSwapRateRangeResponse_tns:
    properties: []
  GetSwapRateExtended_tns:
    properties:
      SwapType:
        description: This is a default description.
        type: post
      Currency:
        description: This is a default description.
        type: post
      Tenor:
        description: This is a default description.
        type: post
  GetSwapRateExtendedResponse_tns:
    properties: []
  GetSwapRateFamilyExtended_tns:
    properties:
      SwapType:
        description: This is a default description.
        type: post
      Currency:
        description: This is a default description.
        type: post
  GetSwapRateFamilyExtendedResponse_tns:
    properties: []
  GetHistoricalSwapRateExtended_tns:
    properties:
      SwapType:
        description: This is a default description.
        type: post
      Currency:
        description: This is a default description.
        type: post
      Tenor:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetHistoricalSwapRateExtendedResponse_tns:
    properties: []
  GetHistoricalSwapRateExtendedRange_tns:
    properties:
      SwapType:
        description: This is a default description.
        type: post
      Currency:
        description: This is a default description.
        type: post
      Tenor:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetHistoricalSwapRateExtendedRangeResponse_tns:
    properties: []
  ListSwapRates_tns:
    properties:
      SwapType:
        description: This is a default description.
        type: post
      Currency:
        description: This is a default description.
        type: post
  ListSwapRatesResponse_tns:
    properties: []
  GetTreasuryRate_tns:
    properties: []
  GetTreasuryRateResponse_tns:
    properties: []
  GetTreasuryRateFamily_tns:
    properties: []
  GetTreasuryRateFamilyResponse_tns:
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
  ArrayOfRateDescription_tns:
    properties:
      RateDescription:
        description: This is a default description.
        type: post
  ArrayOfEuroDollarFRA_tns:
    properties:
      EuroDollarFRA:
        description: This is a default description.
        type: post
  ArrayOfSwaption_tns:
    properties:
      Swaption:
        description: This is a default description.
        type: post
  ArrayOfSwapRate_tns:
    properties:
      SwapRate:
        description: This is a default description.
        type: post
  ArrayOfSwapRateExtended_tns:
    properties:
      SwapRateExtended:
        description: This is a default description.
        type: post
  ArrayOfSwapRateDescription_tns:
    properties:
      SwapRateDescription:
        description: This is a default description.
        type: post
  ArrayOfInterestRate_tns:
    properties:
      InterestRate:
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