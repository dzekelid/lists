---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API Lists all of a location's Favorites pages in Square Register.
  description: Lists all of a location's Favorites pages in Square Register.
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{location_id}/categories:
    get:
      summary: Lists all of a location's item categories.
      description: Lists all of a location's item categories.
      operationId: ListCategories
      x-api-path-slug: v1location-idcategories-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list categories for
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Locations
      - Item
      - Categories
  /v1/{location_id}/discounts:
    get:
      summary: Lists all of a location's discounts.
      description: Lists all of a location's discounts.
      operationId: ListDiscounts
      x-api-path-slug: v1location-iddiscounts-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list categories for
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Locations
      - Discounts
  /v1/{location_id}/fees:
    get:
      summary: Lists all of a location's fees (taxes).
      description: Lists all of a location's fees (taxes).
      operationId: ListFees
      x-api-path-slug: v1location-idfees-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list fees for
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Locations
      - Fees
      - (taxes)
  /v1/{location_id}/items/{item_id}:
    get:
      summary: Provides the details for a single item, including associated modifier
        lists and fees.
      description: Provides the details for a single item, including associated modifier
        lists and fees.
      operationId: RetrieveItem
      x-api-path-slug: v1location-iditemsitem-id-get
      parameters:
      - in: path
        name: item_id
        description: The items ID
      - in: path
        name: location_id
        description: The ID of the items associated location
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Detailsa
      - Single
      - Item
      - ""
      - Including
      - Associated
      - Modifier
      - Lists
      - Fees
  /v1/{location_id}/modifier-lists:
    get:
      summary: Lists all of a location's modifier lists.
      description: Lists all of a location's modifier lists.
      operationId: ListModifierLists
      x-api-path-slug: v1location-idmodifierlists-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list modifier lists for
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Locations
      - Modifier
      - Lists
  /v1/{location_id}/pages:
    get:
      summary: Lists all of a location's Favorites pages in Square Register.
      description: Lists all of a location's Favorites pages in Square Register.
      operationId: ListPages
      x-api-path-slug: v1location-idpages-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list Favorites pages for
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Locations
      - Favorites
      - Pages
      - In
      - Square
      - Register
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---