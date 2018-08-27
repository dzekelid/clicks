swagger: "2.0"
x-collection-name: Postmark
x-complete: 1
info:
  title: Postmark Account-level
  description: postmark-makes-sending-and-receiving-email-incredibly-easy--the-accountlevel-api-allows-users-toconfigure-all-servers-domains-and-sender-signatures-associated-with-an-account-
  version: 0.9.0
host: api.postmarkapp.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /messages/outbound/clicks:
    get:
      summary: Get Messages Outbound Clicks
      description: Get messages outbound clicks.
      operationId: getMessagesOutboundClicks
      x-api-path-slug: messagesoutboundclicks-get
      parameters:
      - in: query
        name: city
        description: Filter by full name of region messages were opened in, i
      - in: query
        name: client_company
        description: Filter by company, i
      - in: query
        name: client_family
        description: Filter by client family, i
      - in: query
        name: client_name
        description: Filter by client name, i
      - in: query
        name: count
        description: Number of message clicks to return per request
      - in: query
        name: country
        description: Filter by country messages were opened in, i
      - in: query
        name: offset
        description: Number of messages to skip
      - in: query
        name: os_company
        description: Filter by company which produced the OS, i
      - in: query
        name: os_family
        description: Filter by kind of OS used without specific version, i
      - in: query
        name: os_name
        description: Filter by full OS name and specific version, i
      - in: query
        name: platform
        description: Filter by platform, i
      - in: query
        name: recipient
        description: Filter by To, Cc, Bcc
      - in: query
        name: region
        description: Filter by full name of region messages were opened in, i
      - in: query
        name: tag
        description: Filter by tag
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Outbound
      - Clicks
  /messages/outbound/clicks/{messageid}:
    get:
      summary: Get Messages Outbound Clicks Message
      description: Get messages outbound clicks message.
      operationId: getMessagesOutboundClicksMessage
      x-api-path-slug: messagesoutboundclicksmessageid-get
      parameters:
      - in: query
        name: count
        description: Number of message clicks to return per request
      - in: path
        name: messageid
        description: The ID of the Outbound Message for which click statistics should
          be retrieved
      - in: query
        name: offset
        description: Number of messages to skip
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Outbound
      - Clicks
      - Messageid
  /stats/outbound/clicks:
    get:
      summary: Get Stats Outbound Clicks
      description: Get stats outbound clicks.
      operationId: getStatsOutboundClicks
      x-api-path-slug: statsoutboundclicks-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Clicks
  /stats/outbound/clicks/browserfamilies:
    get:
      summary: Get Stats Outbound Clicks Browserfamilies
      description: Get stats outbound clicks browserfamilies.
      operationId: getStatsOutboundClicksBrowserfamilies
      x-api-path-slug: statsoutboundclicksbrowserfamilies-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Clicks
      - Browserfamilies
  /stats/outbound/clicks/location:
    get:
      summary: Get Stats Outbound Clicks Location
      description: Get stats outbound clicks location.
      operationId: getStatsOutboundClicksLocation
      x-api-path-slug: statsoutboundclickslocation-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Clicks
      - Location
  /stats/outbound/clicks/platforms:
    get:
      summary: Get Stats Outbound Clicks Platforms
      description: Get stats outbound clicks platforms.
      operationId: getStatsOutboundClicksPlatforms
      x-api-path-slug: statsoutboundclicksplatforms-get
      parameters:
      - in: query
        name: fromdate
        description: Filter stats starting from the date specified
      - in: query
        name: tag
        description: Filter by tag
      - in: query
        name: todate
        description: Filter stats up to the date specified
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Stats
      - Outbound
      - Clicks
      - Platforms