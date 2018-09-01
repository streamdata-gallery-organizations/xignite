---
swagger: "2.0"
info:
  title: Xignite InterBanks
  description: Provide information about global interbank interest rates.
  version: 1.0.0
host: www.xignite.com
basePath: xInterBanks.json/XigniteInterBanks
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetMEXIBOR:
    post:
      summary: Get MEXIBOR
      description: Returns a MEXIBOR as of a date
      operationId: postGetmexibor
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - mexibor
definitions:
  Security:
    properties:
      UsernameToken:
        description: This is a default description.
        type: post
      Timestamp:
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
  GetLIBORSecureInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLIBORSecureHeader:
    properties: []
  GetLIBORSecureOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLIBORHeader:
    properties: []
  GetLIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetREIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetREIBORHeader:
    properties: []
  GetREIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHIBORHeader:
    properties: []
  GetHIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetBUBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetBUBORHeader:
    properties: []
  GetBUBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSOFIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSOFIBORHeader:
    properties: []
  GetSOFIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetREIBIDInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetREIBIDHeader:
    properties: []
  GetREIBIDOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetOIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetOIBORHeader:
    properties: []
  GetOIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSIBORHeader:
    properties: []
  GetSIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCIBORHeader:
    properties: []
  GetCIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSTIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSTIBORHeader:
    properties: []
  GetSTIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetWIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetWIBORHeader:
    properties: []
  GetWIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetVILIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetVILIBORHeader:
    properties: []
  GetVILIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetEURIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetEURIBORHeader:
    properties: []
  GetEURIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetPRIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetPRIBORHeader:
    properties: []
  GetPRIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetKORIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetKORIBORHeader:
    properties: []
  GetKORIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetMIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetMIBORHeader:
    properties: []
  GetMIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetMIBIDInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetMIBIDHeader:
    properties: []
  GetMIBIDOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSABORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSABORHeader:
    properties: []
  GetSABOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTAIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTAIBORHeader:
    properties: []
  GetTAIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTURKIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTURKIBORHeader:
    properties: []
  GetTURKIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetMEXIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetMEXIBORHeader:
    properties: []
  GetMEXIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTELBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTELBORHeader:
    properties: []
  GetTELBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCHILIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCHILIBORHeader:
    properties: []
  GetCHILIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCHIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCHIBORHeader:
    properties: []
  GetCHIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCDORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCDORHeader:
    properties: []
  GetCDOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetKAIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetKAIBORHeader:
    properties: []
  GetKAIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetKIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetKIBORHeader:
    properties: []
  GetKIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetKIBIDInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetKIBIDHeader:
    properties: []
  GetKIBIDOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSHIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetSHIBORHeader:
    properties: []
  GetSHIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetJIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetJIBORHeader:
    properties: []
  GetJIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetKLIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetKLIBORHeader:
    properties: []
  GetKLIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTIBORHeader:
    properties: []
  GetTIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetPHIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetPHIBORHeader:
    properties: []
  GetPHIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetBKIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetBKIBORHeader:
    properties: []
  GetBKIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetVNIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetVNIBORHeader:
    properties: []
  GetVNIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetMOSIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetMOSIBORHeader:
    properties: []
  GetMOSIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetMOSIBIDInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetMOSIBIDHeader:
    properties: []
  GetMOSIBIDOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalLIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalLIBORHeader:
    properties: []
  GetHistoricalLIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetBRAZIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetBRAZIBORHeader:
    properties: []
  GetBRAZIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTRLIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTRLIBORHeader:
    properties: []
  GetTRLIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTRLIBIDInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTRLIBIDHeader:
    properties: []
  GetTRLIBIDOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetBRIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetBRIBORHeader:
    properties: []
  GetBRIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetBRIBIDInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetBRIBIDHeader:
    properties: []
  GetBRIBIDOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRIGIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRIGIBORHeader:
    properties: []
  GetRIGIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRIGIBIDInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRIGIBIDHeader:
    properties: []
  GetRIGIBIDOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAIDIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAIDIBORHeader:
    properties: []
  GetAIDIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetJIBARInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetJIBARHeader:
    properties: []
  GetJIBAROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetBAIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetBAIBORHeader:
    properties: []
  GetBAIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCOLIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCOLIBORHeader:
    properties: []
  GetCOLIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTALIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTALIBORHeader:
    properties: []
  GetTALIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTALIBIDInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTALIBIDHeader:
    properties: []
  GetTALIBIDOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRateInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRateHeader:
    properties: []
  GetRateOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRateFamilyTableInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRateFamilyTableHeader:
    properties: []
  GetRateFamilyTableOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRateFamilyInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRateFamilyHeader:
    properties: []
  GetRateFamilyOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTodaysRateInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTodaysRateHeader:
    properties: []
  GetTodaysRateOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLatestRateInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLatestRateHeader:
    properties: []
  GetLatestRateOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLatestLIBORInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLatestLIBORHeader:
    properties: []
  GetLatestLIBOROutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLatestRateFamilyInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLatestRateFamilyHeader:
    properties: []
  GetLatestRateFamilyOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalRatesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalRatesHeader:
    properties: []
  GetHistoricalRatesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalRateFamilyInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetHistoricalRateFamilyHeader:
    properties: []
  GetHistoricalRateFamilyOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRateDescriptionInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetRateDescriptionHeader:
    properties: []
  GetRateDescriptionOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  DrawRateChartCustomInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  DrawRateChartCustomHeader:
    properties: []
  DrawRateChartCustomOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  DrawRateChartInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  DrawRateChartHeader:
    properties: []
  DrawRateChartOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  DrawRateChartPresetInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  DrawRateChartPresetHeader:
    properties: []
  DrawRateChartPresetOutput:
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
  DrawYieldCurveInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  DrawYieldCurveHeader:
    properties: []
  DrawYieldCurveOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  DrawYieldCurvePresetInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  DrawYieldCurvePresetHeader:
    properties: []
  DrawYieldCurvePresetOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  DrawYieldCurveCustomInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  DrawYieldCurveCustomHeader:
    properties: []
  DrawYieldCurveCustomOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
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
  GetLIBORSecure_tns:
    properties:
      Username:
        description: This is a default description.
        type: post
      AsOfDate:
        description: This is a default description.
        type: post
  GetLIBORSecureResponse_tns:
    properties: []
  GetLIBOR_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetLIBORResponse_tns:
    properties: []
  GetREIBOR_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetREIBORResponse_tns:
    properties: []
  GetHIBOR_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetHIBORResponse_tns:
    properties: []
  GetBUBOR_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetBUBORResponse_tns:
    properties: []
  GetSOFIBOR_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetSOFIBORResponse_tns:
    properties: []
  GetREIBID_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetREIBIDResponse_tns:
    properties: []
  GetOIBOR_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetOIBORResponse_tns:
    properties: []
  GetSIBOR_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetSIBORResponse_tns:
    properties: []
  GetCIBOR_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetCIBORResponse_tns:
    properties: []
  GetSTIBOR_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetSTIBORResponse_tns:
    properties: []
  GetWIBOR_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetWIBORResponse_tns:
    properties: []
  GetVILIBOR_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetVILIBORResponse_tns:
    properties: []
  GetEURIBOR_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetEURIBORResponse_tns:
    properties: []
  GetPRIBOR_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetPRIBORResponse_tns:
    properties: []
  GetKORIBOR_tns:
    properties:
      AsOfDate:
        description: This is a default description.
        type: post
  GetKORIBORResponse_tns:
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