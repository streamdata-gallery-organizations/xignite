---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Calendar List Country Codes
  description: Get all of the country codes available to query on.
  version: 1.0.0
host: www.xignite.com
basePath: xCalendar.json/XigniteCalendar
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetEventsForNextNumberOfDays:
    get:
      summary: Get Events For Next Number Of Days
      description: Get events for the next number of days into the future.
      operationId: postGeteventsfornextnumberofdays
      x-api-path-slug: geteventsfornextnumberofdays-get
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
      - Events
      - Next
      - Number
      - Days
  /GetEventsForWeek:
    get:
      summary: Get Events For Week
      description: Get all the events released during the week specified. Weeks are
        Monday - Sunday.
      operationId: postGeteventsforweek
      x-api-path-slug: geteventsforweek-get
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
      - Events
      - Week
  /ListCountryCodes:
    get:
      summary: List Country Codes
      description: Get all of the country codes available to query on.
      operationId: postListcountrycodes
      x-api-path-slug: listcountrycodes-get
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
      - Country
      - Codes
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