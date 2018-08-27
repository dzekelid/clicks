---
swagger: "2.0"
x-collection-name: Dyn
x-complete: 0
info:
  title: Dyn Reports on Clicks
  version: 1.0.0
  description: Returns a list of links clicked for the specified account during the
    specified date range. Including a date range is highly recommended.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  reports/clicks:
    get:
      summary: Reports on Clicks
      description: Returns a list of links clicked for the specified account during
        the specified date range. Including a date range is highly recommended.
      operationId: getReportsClicks
      x-api-path-slug: reportsclicks-get
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: emailaddress
        description: Email address of recipient for filtering
      - in: query
        name: endtime
        description: Required
      - in: query
        name: sender
        description: Email address of sender for filtering
      - in: query
        name: startindex
        description: Starting index value (optional)
      - in: query
        name: starttime
        description: Required
      - in: query
        name: '[X-HeaderName]'
        description: Name of searchable custom X-header
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Clicks
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