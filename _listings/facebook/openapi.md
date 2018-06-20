---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  description: connect-to-the-social-network-with-the-graph-api-
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
---