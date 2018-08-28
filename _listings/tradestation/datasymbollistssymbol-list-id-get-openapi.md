---
swagger: "2.0"
x-collection-name: TradeStation
x-complete: 0
info:
  title: TradeStation Get Symbol List
  description: Gets a specific Symbol List
  termsOfService: http://elasticbeanstalk-us-east-1-525856068889.s3.amazonaws.com/wp-content/uploads/2014/03/Guidelines_For_Acceptance.pdf
  contact:
    name: TradeStation API Team
    url: https://developer.tradestation.com/webapi
    email: webapi@tradestation.com
  version: 1.0.0
host: api.tradestation.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /data/symbollists:
    get:
      summary: Get all Symbol Lists
      description: Gets a list of all Symbol Lists
      operationId: getSymbolLists
      x-api-path-slug: datasymbollists-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      responses:
        200:
          description: Successful response
      tags:
      - Symbol
      - Lists
  /data/symbollists/{symbol_list_id}:
    get:
      summary: Get Symbol List
      description: Gets a specific Symbol List
      operationId: getSymbolListByID
      x-api-path-slug: datasymbollistssymbol-list-id-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: symbol_list_id
        description: A valid Symbol List ID
      responses:
        200:
          description: Successful response
      tags:
      - Symbol
      - List
  /data/symbollists/{symbol_list_id}/symbols:
    get:
      summary: Get Symbols in a Symbol List
      description: Gets the Symbols for a specific Symbol List
      operationId: getSymbolListSymbolsByID
      x-api-path-slug: datasymbollistssymbol-list-idsymbols-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: symbol_list_id
        description: A valid Symbol List ID
      responses:
        200:
          description: Successful response
      tags:
      - Symbols
      - In
      - Symbol
      - List
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