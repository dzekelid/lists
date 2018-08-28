---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Post Lists Deleteitem
  description: /lists/{LIST_ID}/additem
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
  /lists/{LIST_ID}/additem:
    post:
      summary: Post Lists Additem
      description: /lists/{LIST_ID}/suggestvenues
      operationId: listslist-idsuggestvenues
      x-api-path-slug: listslist-idadditem-post
      parameters:
      - in: query
        name: itemId
        description: Used in conjuction with listId, the id of an item on that list
          that we wish to copy to this list
      - in: query
        name: listId
        description: Used in conjuction with itemId, the id for a user created or
          followed list as well as one of USER_ID/tips, USER_ID/todos, or USER_ID/dones
      - in: query
        name: LIST_ID
        description: Id for a user-created or followed list as well as one of USER_ID/tips,
          USER_ID/todos, or USER_ID/dones
      - in: path
        name: LIST_ID
      - in: query
        name: text
        description: If the target is a user-created list, this will create a public
          tip on the venue
      - in: query
        name: tipId
        description: Used to add a tip to a list
      - in: query
        name: url
        description: If adding a new tip via text, this can associate a url with the
          tip
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: A venue to add to the list
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Item
  /lists/{LIST_ID}/deleteitem:
    post:
      summary: Post Lists Deleteitem
      description: /lists/{LIST_ID}/additem
      operationId: listslist-idadditem
      x-api-path-slug: listslist-iddeleteitem-post
      parameters:
      - in: query
        name: itemId
        description: Id of the item to delete
      - in: query
        name: LIST_ID
        description: Id for a user-created or followed list or one of USER_ID/tips,
          USER_ID/todos, or USER_ID/dones
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Item
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