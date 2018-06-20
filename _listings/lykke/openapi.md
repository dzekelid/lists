---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
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
---