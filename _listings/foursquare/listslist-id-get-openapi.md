---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Get Lists
  description: /tips/{TIP_ID}/unmark
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lists/add:
    post:
      summary: Post Lists Add
      description: /lists/{LIST_ID}
      operationId: listslist-id
      x-api-path-slug: listsadd-post
      parameters:
      - in: query
        name: collaborative
        description: Indicating if this list can be edited by friends
      - in: query
        name: description
        description: The description of the list
      - in: query
        name: name
        description: The name of the list
      - in: query
        name: photoId
        description: The id of a photo that should be set as the list photo
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
  /lists/{LIST_ID}:
    get:
      summary: Get Lists
      description: /tips/{TIP_ID}/unmark
      operationId: tipstip-idunmark
      x-api-path-slug: listslist-id-get
      parameters:
      - in: query
        name: limit
        description: Number of results to return, up to 200
      - in: query
        name: LIST_ID
        description: id for a user-created (e
      - in: path
        name: LIST_ID
      - in: query
        name: offset
        description: The number of results to skip
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
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