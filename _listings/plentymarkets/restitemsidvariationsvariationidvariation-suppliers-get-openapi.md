---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Lists suppliers for a variation
  description: Lists all supplier data linked to a variation. The ID of the variation
    must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounting/locations/{locationId}/debtor_accounts/{mode}:
    get:
      summary: Lists the debtor accounts by mode.
      description: Lists the debtor accounts of an accounting location by mode. The
        ID of the accounting location and the mode have to be specified.
      operationId: getRestAccountingLocationsLocationDebtorAccountsMode
      x-api-path-slug: restaccountinglocationslocationiddebtor-accountsmode-get
      parameters:
      - in: path
        name: locationId
      - in: path
        name: mode
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Debtor
      - Accounts
      - By
      - Mode
  /rest/boards:
    get:
      summary: Lists all boards.
      description: Lists all boards..
      operationId: getRestBoards
      x-api-path-slug: restboards-get
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Boards
  /rest/boards/{boardId}/columns:
    get:
      summary: Lists all columns for a given board
      description: Lists all columns for a given board.
      operationId: getRestBoardsBoardColumns
      x-api-path-slug: restboardsboardidcolumns-get
      parameters:
      - in: path
        name: boardId
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Columnsa
      - Given
      - Board
  /rest/boards/{boardId}/columns/{columnId}/tasks:
    get:
      summary: Lists all tasks for a given column.
      description: Lists all tasks for a given column..
      operationId: getRestBoardsBoardColumnsColumnTasks
      x-api-path-slug: restboardsboardidcolumnscolumnidtasks-get
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: query
        name: startAt
        description: Position of a task to start listing at
      - in: query
        name: tasksPerPage
        description: Number of tasks to list per page
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Tasksa
      - Given
      - Column
  /rest/items/attributes/maps:
    get:
      summary: Lists all attribute maps.
      description: Lists all attribute maps..
      operationId: getRestItemsAttributesMaps
      x-api-path-slug: restitemsattributesmaps-get
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Attribute
      - Maps
  /rest/items/attributes/values/maps:
    get:
      summary: Lists all attribute value maps.
      description: Lists all attribute value maps..
      operationId: getRestItemsAttributesValuesMaps
      x-api-path-slug: restitemsattributesvaluesmaps-get
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Attribute
      - Value
      - Maps
  /rest/items/{id}/variations/{variationId}/variation_suppliers:
    get:
      summary: Lists suppliers for a variation
      description: Lists all supplier data linked to a variation. The ID of the variation
        must be specified.
      operationId: getRestItemsVariationsVariationVariationSuppliers
      x-api-path-slug: restitemsidvariationsvariationidvariation-suppliers-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Suppliersa
      - Variation
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