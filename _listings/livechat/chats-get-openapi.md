---
swagger: "2.0"
x-collection-name: LiveChat
x-complete: 0
info:
  title: LiveChat Get list of chats
  description: Returns all ended chats.
  version: 1.0.0
host: api.livechatinc.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /visitors:
    get:
      summary: List all visitors
      description: Returns a list of the visitors on the pages with the tracking code
        installed.
      operationId: VisitorsGet
      x-api-path-slug: visitors-get
      parameters:
      - in: query
        name: group[]
      - in: query
        name: state
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Visitors
  /agents:
    get:
      summary: List all agents
      description: Returns all LiveChat agents list
      operationId: AgentsGet
      x-api-path-slug: agents-get
      parameters:
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Agents
  /chats:
    get:
      summary: Get list of chats
      description: Returns all ended chats.
      operationId: ChatsGet
      x-api-path-slug: chats-get
      parameters:
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Chats
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