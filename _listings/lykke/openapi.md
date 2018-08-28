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
  /api/Assets/description/list:
    post:
      summary: Add API Assets Description List
      description: Add api assets description list.
      operationId: ApiAssetsDescriptionListPost
      x-api-path-slug: apiassetsdescriptionlist-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Assets
      - Description
      - List
  /api/offchain/limit/list:
    get:
      summary: Get API Offchain Limit List
      description: Get api offchain limit list.
      operationId: ApiOffchainLimitListGet
      x-api-path-slug: apioffchainlimitlist-get
      parameters:
      - in: query
        name: assetPair
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Offchain
      - Limit
      - List
  /api/Operations/list/{status}:
    get:
      summary: Get API Operations List Status
      description: Get api operations list status.
      operationId: ApiOperationsListByStatusGet
      x-api-path-slug: apioperationsliststatus-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: status
      responses:
        200:
          description: OK
      tags:
      - Operations
      - List
      - Status