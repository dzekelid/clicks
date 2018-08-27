---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly Organization Metric API Organization Clicks
  description: Returns the number of clicks on Bitlinks created by your organization
    or by other Bitly users that point to your domains.
  termsOfService: http://dev.bitly.com/best_practices.html
  version: v3
host: api-ssl.bitly.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/link/clicks:
    get:
      summary: Get Link Clicks
      description: Returns entries from a user's link history in reverse chronological
        order.
      operationId: Get_link_clicks_
      x-api-path-slug: v3linkclicks-get
      parameters:
      - in: query
        name: format
        description: Response format
      - in: query
        name: limit
        description: (optional) 1 to 1000 (default=100)
      - in: query
        name: link
        description: a bltly link
      - in: query
        name: rollup
        description: (optional) true or false
      - in: query
        name: timezone
        description: (optional) an integer hour offset from UTC (-14 to 14)
      - in: query
        name: unit
        description: minute, hour, day, week or month
      - in: query
        name: units
        description: an integer representing the time units to query data for
      responses:
        200:
          description: OK
      tags:
      - Link
      - Clicks
  /link/clicks:
    get:
      summary: Link Clicks
      description: Returns the number of clicks on a single Bitlink.
      operationId: linkClicks
      x-api-path-slug: linkclicks-get
      parameters:
      - in: query
        name: format
        description: json, xml, txt
      - in: query
        name: limit
        description: 1 to 1000 (default=100)
      - in: query
        name: link
        description: a Bitlink
      - in: query
        name: rollup
        description: Return data for multiple units rolled up to a single result instead
          of a separate value for each period of time
      - in: query
        name: timezone
        description: 'an integer hour offset from UTC (-14 to 14), or a timezone string
          default: America/New_York'
      - in: query
        name: unit
        description: 'minute, hour, day, week or month, default: day'
      - in: query
        name: units
        description: an integer representing the time units to query data for
      - in: query
        name: unit_reference_ts
        description: 'an epoch timestamp, indicating the most recent time for which
          to pull metrics, default: now'
      responses:
        200:
          description: OK
      tags:
      - Link
      - Clicks
  /v3/organization/clicks:
    get:
      summary: Organization Clicks
      description: Returns the number of clicks on Bitlinks created by your organization
        or by other Bitly users that point to your domains.
      operationId: organizationClicks
      x-api-path-slug: v3organizationclicks-get
      parameters:
      - in: query
        name: domain
        description: filter to a tracking or e2e domain for this organization
      - in: query
        name: limit
        description: "1"
      - in: query
        name: login
        description: an account in this organization
      - in: query
        name: timezone
        description: an integer hour offset from UTC (-14
      - in: query
        name: unit
        description: hour | day | week | month default:day
      - in: query
        name: units
        description: an integer representing the time units to query data for
      - in: query
        name: unit_reference_ts
        description: an epoch timestamp, indicating the most recent time for which
          to pull metrics
      responses:
        200:
          description: OK
      tags:
      - Organization
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