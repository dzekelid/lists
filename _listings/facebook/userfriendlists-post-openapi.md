---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Post User Friendlists
  description: Creates a FriendList for the user
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{user}/friendlists:
    post:
      summary: Post User Friendlists
      description: Creates a FriendList for the user
      operationId: postUserFriendlists
      x-api-path-slug: userfriendlists-post
      parameters:
      - in: query
        name: name
        description: Friend list name
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Friendlists
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