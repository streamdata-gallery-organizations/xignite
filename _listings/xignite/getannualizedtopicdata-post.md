---
swagger: "2.0"
info:
  title: Xignite Statistics
  description: Delivers and charts more than 1400 economical time-series fom the Federal
    Reserve Bank.
  version: 1.0.0
host: www.xignite.com
basePath: xStatistics.json/XigniteStatistics
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetAnnualizedTopicData:
    post:
      summary: Get Annualized Topic Data
      description: Get annualized time-series data for a topic
      operationId: postGetannualizedtopicdata
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - annualized
      - topic
      - data
definitions:
  Security:
    properties:
      UsernameToken:
        description: This is a default description.
        type: post
      Timestamp:
        description: This is a default description.
        type: post
  GetCategoriesAndTopicsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCategoriesAndTopicsHeader:
    properties: []
  GetCategoriesAndTopicsOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCategoriesInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetCategoriesHeader:
    properties: []
  GetCategoriesOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicsHeader:
    properties: []
  GetTopicsOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicDetailsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicDetailsHeader:
    properties: []
  GetTopicDetailsOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicStatisticsInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicStatisticsHeader:
    properties: []
  GetTopicStatisticsOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicDataInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicDataHeader:
    properties: []
  GetTopicDataOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLatestTopicDataInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetLatestTopicDataHeader:
    properties: []
  GetLatestTopicDataOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAnnualizedTopicDataInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetAnnualizedTopicDataHeader:
    properties: []
  GetAnnualizedTopicDataOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicChartInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicChartHeader:
    properties: []
  GetTopicChartOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicChartPresetInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicChartPresetHeader:
    properties: []
  GetTopicChartPresetOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicChartCustomInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicChartCustomHeader:
    properties: []
  GetTopicChartCustomOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicBinaryChartInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicBinaryChartHeader:
    properties: []
  GetTopicBinaryChartOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicBinaryChartPresetInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicBinaryChartPresetHeader:
    properties: []
  GetTopicBinaryChartPresetOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicBinaryChartCustomInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetTopicBinaryChartCustomHeader:
    properties: []
  GetTopicBinaryChartCustomOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetChartUrlInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetChartUrlHeader:
    properties: []
  GetChartUrlOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetChartUrlPresetInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetChartUrlPresetHeader:
    properties: []
  GetChartUrlPresetOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetChartUrlCustomInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetChartUrlCustomHeader:
    properties: []
  GetChartUrlCustomOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetChartBinaryInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetChartBinaryHeader:
    properties: []
  GetChartBinaryOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetChartBinaryPresetInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetChartBinaryPresetHeader:
    properties: []
  GetChartBinaryPresetOutput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetChartBinaryCustomInput:
    properties:
      Envelope:
        description: This is a default description.
        type: post
  GetChartBinaryCustomHeader:
    properties: []
  GetChartBinaryCustomOutput:
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
  GetCategoriesAndTopics_tns:
    properties: []
  GetCategoriesAndTopicsResponse_tns:
    properties: []
  GetCategories_tns:
    properties: []
  GetCategoriesResponse_tns:
    properties: []
  GetTopics_tns:
    properties:
      CategoryCode:
        description: This is a default description.
        type: post
  GetTopicsResponse_tns:
    properties: []
  GetTopicDetails_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
  GetTopicDetailsResponse_tns:
    properties: []
  GetTopicStatistics_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetTopicStatisticsResponse_tns:
    properties: []
  GetTopicData_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetTopicDataResponse_tns:
    properties: []
  GetLatestTopicData_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
  GetLatestTopicDataResponse_tns:
    properties: []
  GetAnnualizedTopicData_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
  GetAnnualizedTopicDataResponse_tns:
    properties: []
  GetTopicChart_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
      ChartWidth:
        description: This is a default description.
        type: post
      ChartHeight:
        description: This is a default description.
        type: post
  GetTopicChartResponse_tns:
    properties: []
  GetTopicChartPreset_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
      ChartWidth:
        description: This is a default description.
        type: post
      ChartHeight:
        description: This is a default description.
        type: post
      Preset:
        description: This is a default description.
        type: post
  GetTopicChartPresetResponse_tns:
    properties: []
  GetTopicChartCustom_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
      ChartWidth:
        description: This is a default description.
        type: post
      ChartHeight:
        description: This is a default description.
        type: post
  GetTopicChartCustomResponse_tns:
    properties: []
  GetTopicBinaryChart_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
      ChartWidth:
        description: This is a default description.
        type: post
      ChartHeight:
        description: This is a default description.
        type: post
      Preset:
        description: This is a default description.
        type: post
  GetTopicBinaryChartResponse_tns:
    properties: []
  GetTopicBinaryChartPreset_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
      ChartWidth:
        description: This is a default description.
        type: post
      ChartHeight:
        description: This is a default description.
        type: post
      Preset:
        description: This is a default description.
        type: post
  GetTopicBinaryChartPresetResponse_tns:
    properties: []
  GetTopicBinaryChartCustom_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
      ChartWidth:
        description: This is a default description.
        type: post
      ChartHeight:
        description: This is a default description.
        type: post
  GetTopicBinaryChartCustomResponse_tns:
    properties: []
  GetChartUrl_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
      ChartWidth:
        description: This is a default description.
        type: post
      ChartHeight:
        description: This is a default description.
        type: post
  GetChartUrlResponse_tns:
    properties: []
  GetChartUrlPreset_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
      ChartWidth:
        description: This is a default description.
        type: post
      ChartHeight:
        description: This is a default description.
        type: post
      Preset:
        description: This is a default description.
        type: post
  GetChartUrlPresetResponse_tns:
    properties: []
  GetChartUrlCustom_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
      ChartWidth:
        description: This is a default description.
        type: post
      ChartHeight:
        description: This is a default description.
        type: post
  GetChartUrlCustomResponse_tns:
    properties: []
  GetChartBinary_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
      ChartWidth:
        description: This is a default description.
        type: post
      ChartHeight:
        description: This is a default description.
        type: post
  GetChartBinaryResponse_tns:
    properties: []
  GetChartBinaryPreset_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
      ChartWidth:
        description: This is a default description.
        type: post
      ChartHeight:
        description: This is a default description.
        type: post
      Preset:
        description: This is a default description.
        type: post
  GetChartBinaryPresetResponse_tns:
    properties: []
  GetChartBinaryCustom_tns:
    properties:
      TopicCode:
        description: This is a default description.
        type: post
      StartDate:
        description: This is a default description.
        type: post
      EndDate:
        description: This is a default description.
        type: post
      ChartWidth:
        description: This is a default description.
        type: post
      ChartHeight:
        description: This is a default description.
        type: post
  GetChartBinaryCustomResponse_tns:
    properties: []
  GetChartDesign_tns:
    properties: []
  GetChartDesignResponse_tns:
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
  ArrayOfCategory_tns:
    properties:
      Category:
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
  ArrayOfTopic_tns:
    properties:
      Topic:
        description: This is a default description.
        type: post
  ArrayOfSeriesData_tns:
    properties:
      SeriesData:
        description: This is a default description.
        type: post
  SeriesData_tns:
    properties:
      Date:
        description: This is a default description.
        type: post
      Value:
        description: This is a default description.
        type: post
      Change:
        description: This is a default description.
        type: post
      PercentChange:
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