---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Fact Set Estimates List Companies
  description: List Symbols
  version: 1.0.0
host: factsetestimates.xignite.com
basePath: xFactSetEstimates.json/XigniteFactSetEstimates
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ListTradedSymbols:
    get:
      summary: List Traded Symbols
      description: Returns all symbols and names that are traded recently
      operationId: ListTradedSymbols
      x-api-path-slug: listtradedsymbols-get
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
      - Traded
      - Symbols
  /ListBondTypes:
    get:
      summary: List Bond Types
      description: ""
      operationId: ListBondTypes
      x-api-path-slug: listbondtypes-get
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
      - Bond
      - Types
  /ListSymbols:
    get:
      summary: List Symbols
      description: ""
      operationId: ListSymbols
      x-api-path-slug: listsymbols-get
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
      - Symbols
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
  /ListEventCodes:
    get:
      summary: List Event Codes
      description: Get all of the event codes available to query on.
      operationId: postListeventcodes
      x-api-path-slug: listeventcodes-get
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
      - Event
      - Codes
  /ListCurrencies:
    get:
      summary: List Currencies
      description: List supported currencies.
      operationId: postListcurrencies
      x-api-path-slug: listcurrencies-get
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
      - Currencies
  /ListActiveCurrencies:
    get:
      summary: List Active Currencies
      description: List supported currencies.
      operationId: postListactivecurrencies
      x-api-path-slug: listactivecurrencies-get
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
      - Active
      - Currencies
  /ListOfficialRates:
    get:
      summary: List Official Rates
      description: List supported official rates.
      operationId: postListofficialrates
      x-api-path-slug: listofficialrates-get
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
      - Official
      - Rates
  /ListExchanges:
    get:
      summary: List Exchanges
      description: List Exchanges
      operationId: ListExchanges
      x-api-path-slug: listexchanges-get
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
      - Exchanges
  /ListCompanies:
    get:
      summary: List Companies
      description: List Symbols
      operationId: ListCompanies
      x-api-path-slug: listcompanies-get
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
      - Companies
  /ListEstimates:
    get:
      summary: List Estimates
      description: List Estimates
      operationId: ListEstimates
      x-api-path-slug: listestimates-get
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
      - Estimates
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