---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Delete API Watchlists
  version: 1.0.0
  description: Delete api watchlists.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/WatchLists:
    get:
      summary: Get API Watchlists
      description: Get api watchlists.
      operationId: ApiWatchListsGet
      x-api-path-slug: apiwatchlists-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Watchlists
    post:
      summary: Add API Watchlists
      description: Add api watchlists.
      operationId: ApiWatchListsPost
      x-api-path-slug: apiwatchlists-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Watchlists
  /api/WatchLists/{id}:
    get:
      summary: Get API Watchlists
      description: Get api watchlists.
      operationId: ApiWatchListsByIdGet
      x-api-path-slug: apiwatchlistsid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Watchlists
    put:
      summary: Put API Watchlists
      description: Put api watchlists.
      operationId: ApiWatchListsByIdPut
      x-api-path-slug: apiwatchlistsid-put
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Watchlists
    delete:
      summary: Delete API Watchlists
      description: Delete api watchlists.
      operationId: ApiWatchListsByIdDelete
      x-api-path-slug: apiwatchlistsid-delete
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Watchlists
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